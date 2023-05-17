# Comparing `tmp/inpost-0.0.9.tar.gz` & `tmp/inpost-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inpost-0.0.9.tar", max compression
+gzip compressed data, was "inpost-0.1.0.tar", max compression
```

## Comparing `inpost-0.0.9.tar` & `inpost-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,29 @@
--rw-r--r--   0        0        0       31 2023-01-08 12:39:56.709189 inpost-0.0.9/README.md
--rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.0.9/inpost/__init__.py
--rw-r--r--   0        0        0    48840 2023-04-14 09:52:35.751540 inpost-0.0.9/inpost/api.py
--rw-r--r--   0        0        0     1105 2023-04-14 08:22:00.444589 inpost-0.0.9/inpost/static/__init__.py
--rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.0.9/inpost/static/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.0.9/inpost/static/__pycache__/endpoints.cpython-310.pyc
--rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.0.9/inpost/static/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.0.9/inpost/static/__pycache__/friends.cpython-310.pyc
--rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.0.9/inpost/static/__pycache__/headers.cpython-310.pyc
--rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.0.9/inpost/static/__pycache__/parcels.cpython-310.pyc
--rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.0.9/inpost/static/__pycache__/statuses.cpython-310.pyc
--rw-r--r--   0        0        0     1771 2023-03-04 13:33:30.709374 inpost-0.0.9/inpost/static/endpoints.py
--rw-r--r--   0        0        0     2515 2023-02-09 09:51:30.001451 inpost-0.0.9/inpost/static/exceptions.py
--rw-r--r--   0        0        0     1779 2023-02-09 12:35:10.844655 inpost-0.0.9/inpost/static/friends.py
--rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.0.9/inpost/static/headers.py
--rw-r--r--   0        0        0    27210 2023-04-14 10:17:16.303881 inpost-0.0.9/inpost/static/parcels.py
--rw-r--r--   0        0        0     7066 2023-04-14 08:22:00.461255 inpost-0.0.9/inpost/static/statuses.py
--rw-r--r--   0        0        0     1026 2023-04-14 10:19:18.478358 inpost-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 inpost-0.0.9/setup.py
--rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 inpost-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      646 2023-04-25 09:56:56.661671 inpost-0.1.0/README.md
+-rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.1.0/inpost/__init__.py
+-rw-r--r--   0        0        0    45360 2023-05-16 17:51:57.264181 inpost-0.1.0/inpost/api.py
+-rw-r--r--   0        0        0     1173 2023-05-08 21:18:45.284128 inpost-0.1.0/inpost/static/__init__.py
+-rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.1.0/inpost/static/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2644 2023-05-16 17:58:27.019865 inpost-0.1.0/inpost/static/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.1.0/inpost/static/__pycache__/endpoints.cpython-310.pyc
+-rw-r--r--   0        0        0     7733 2023-05-16 17:58:27.079865 inpost-0.1.0/inpost/static/__pycache__/endpoints.cpython-311.pyc
+-rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.1.0/inpost/static/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     5421 2023-05-16 17:58:27.079865 inpost-0.1.0/inpost/static/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.1.0/inpost/static/__pycache__/friends.cpython-310.pyc
+-rw-r--r--   0        0        0     3107 2023-05-16 17:58:27.083199 inpost-0.1.0/inpost/static/__pycache__/friends.cpython-311.pyc
+-rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.1.0/inpost/static/__pycache__/headers.cpython-310.pyc
+-rw-r--r--   0        0        0      223 2023-05-16 17:58:27.076532 inpost-0.1.0/inpost/static/__pycache__/headers.cpython-311.pyc
+-rw-r--r--   0        0        0     1243 2023-05-16 17:58:27.086532 inpost-0.1.0/inpost/static/__pycache__/notifications.cpython-311.pyc
+-rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.1.0/inpost/static/__pycache__/parcels.cpython-310.pyc
+-rw-r--r--   0        0        0    44251 2023-05-16 17:58:27.049865 inpost-0.1.0/inpost/static/__pycache__/parcels.cpython-311.pyc
+-rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.1.0/inpost/static/__pycache__/statuses.cpython-310.pyc
+-rw-r--r--   0        0        0    12027 2023-05-16 18:02:18.314615 inpost-0.1.0/inpost/static/__pycache__/statuses.cpython-311.pyc
+-rw-r--r--   0        0        0     1958 2023-05-17 18:25:42.850624 inpost-0.1.0/inpost/static/endpoints.py
+-rw-r--r--   0        0        0     2515 2023-02-09 09:51:30.001451 inpost-0.1.0/inpost/static/exceptions.py
+-rw-r--r--   0        0        0     1779 2023-02-09 12:35:10.844655 inpost-0.1.0/inpost/static/friends.py
+-rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.1.0/inpost/static/headers.py
+-rw-r--r--   0        0        0      670 2023-05-08 21:18:45.284128 inpost-0.1.0/inpost/static/notifications.py
+-rw-r--r--   0        0        0    27776 2023-05-16 17:55:27.607968 inpost-0.1.0/inpost/static/parcels.py
+-rw-r--r--   0        0        0     7066 2023-05-16 18:03:15.934872 inpost-0.1.0/inpost/static/statuses.py
+-rw-r--r--   0        0        0     1072 2023-05-17 18:26:22.780859 inpost-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 inpost-0.1.0/setup.py
+-rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 inpost-0.1.0/PKG-INFO
```

### Comparing `inpost-0.0.9/inpost/api.py` & `inpost-0.1.0/inpost/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from aiohttp import ClientSession
+from aiohttp import ClientSession, ClientResponse
+from aiohttp.typedefs import StrOrURL
 from typing import List
 import logging
-
+from arrow import utcnow
 from inpost.static import *
 
 
 class Inpost:
     """Python representation of an Inpost app. Essentially implements methods to manage all incoming parcels"""
 
     def __init__(self):
@@ -23,27 +24,104 @@
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         return self.logout()
 
+    async def request(
+            self,
+            method: str,
+            action: str,
+            url: StrOrURL,
+            auth: bool = True,
+            headers: dict | None = None,
+            data: dict | None = None,
+            autorefresh: bool = True,
+            **kwargs,
+    ) -> ClientResponse:
+
+        """Validates sent data and fetches required compartment properties for opening
+
+                :param method: HTTP method of request
+                :type method: str
+                :param action: action type (e.g. "get parcels" or "send sms code") for logging purposes
+                :type action: str
+                :param url: HTTP request url
+                :type url: aiohttp.typedefs.StrOrURL
+                :param auth: True if request should contain authorization header else False
+                :type auth: bool
+                :param headers: Additional headers for HTTP request (don't put authorization header here)
+                :type headers: dict | None
+                :param data: Data to be sent in HTTP request
+                :type data: dict | None
+                :param autorefresh: Let method automatically try to refresh token if API returns HTTP 401 Unauthorized status code
+                :type autorefresh: bool
+                :return: response of http request
+                :rtype: aiohttp.ClientResponse
+                :raises UnauthorizedError: User not authenticated in inpost service
+                :raises NotFoundError: URL not found
+                :raises UnidentifiedAPIError: Unexpected things happened"""
+
+        if auth and headers:
+            if 'Authorization' in headers:
+                raise ValueError('Both auth==True and Authorization in additional headers')
+
+        headers_ = {} if headers is None else headers
+
+        if auth:
+            headers_.update(
+                {'Authorization': self.auth_token}
+            )
+
+        resp = await self.sess.request(method, url, headers=headers_, json=data, **kwargs)
+
+        if autorefresh and resp.status == 401:
+            await self.refresh_token()
+            resp = await self.sess.request(method, url, headers=headers_, json=data, **kwargs)
+
+        match resp.status:
+            case 200:
+                self._log.debug(f'{action} done')
+                return resp
+            case 401:
+                self._log.error(f'could not perform {action}, unauthorized')
+                raise UnauthorizedError(reason=resp)
+            case 404:
+                self._log.error(f'could not perform {action}, not found')
+                raise NotFoundError(reason=resp)
+            case _:
+                self._log.error(f'could not perform {action}, unhandled status')
+
+        raise UnidentifiedAPIError(reason=resp)
+
     @classmethod
     async def from_phone_number(cls, phone_number: str | int):
         """`Classmethod` to initialize :class:`Inpost` object with phone number
 
         :param phone_number: User's Inpost phone number
         :type phone_number: str | int"""
         if isinstance(phone_number, int):
             phone_number = str(phone_number)
         inp = cls()
         await inp.set_phone_number(phone_number=phone_number)
         inp._log.info(f'initialized by from_phone_number')
         return inp
 
+    @classmethod
+    async def from_dict(cls, data: dict):
+        inp = cls()
+        await inp.set_phone_number(data['phone_number'])
+        inp.sms_code = data['sms_code']
+        inp.auth_token = data['auth_token']
+        inp.refr_token = data['refr_token']
+
+        inp._log.info(f'initialized by from_dict')
+        return inp
+
     async def set_phone_number(self, phone_number: str | int) -> bool:
         """Set :class:`Inpost` phone number required for verification
 
         :param phone_number: User's Inpost phone number
         :type phone_number: str | int
         :return: True if `Inpost.phone_number` is set
         :rtype: bool
@@ -70,32 +148,24 @@
         :raises NotFoundError: Phone number not found
         :raises UnidentifiedAPIError: Unexpected things happened
         """
         if not self.phone_number:  # can't log it cuz if there's no phone number no logger initialized @shrug
             raise PhoneNumberError('Phone number missing')
 
         self._log.info(f'sending sms code')
-        async with await self.sess.post(url=send_sms_code,
-                                        json={
-                                            'phoneNumber': f'{self.phone_number}'
-                                        }) as phone:
-            match phone.status:
-                case 200:
-                    self._log.debug(f'sms code sent')
-                    return True
-                case 401:
-                    self._log.error(f'could not send sms code, unauthorized')
-                    raise UnauthorizedError(reason=phone)
-                case 404:
-                    self._log.error(f'could not send sms code, not found')
-                    raise NotFoundError(reason=phone)
-                case _:
-                    self._log.error(f'could not send sms code, unhandled status')
 
-            raise UnidentifiedAPIError(reason=phone)
+        resp = await self.request(method='post',
+                                  action='send sms code',
+                                  url=send_sms_code,
+                                  auth=False,
+                                  headers=None,
+                                  data={'phoneNumber': f'{self.phone_number}'},
+                                  autorefresh=False)
+
+        return True if resp.status == 200 else False
 
     async def confirm_sms_code(self, sms_code: str | int) -> bool:
         """Confirms sms code sent to `Inpost.phone_number` and fetches tokens
 
         :param sms_code: sms code sent to Inpost.phone_number device
         :type sms_code: str | int
         :return: True if sms code gets confirmed and tokens fetched
@@ -112,39 +182,36 @@
         if isinstance(sms_code, int):
             sms_code = str(sms_code)
 
         if len(sms_code) != 6 or not sms_code.isdigit():
             raise SmsCodeError(reason=f'Wrong sms code format: {sms_code} (should be 6 digits)')
 
         self._log.info(f'confirming sms code')
-        async with await self.sess.post(url=confirm_sms_code,
-                                        headers=appjson,
-                                        json={
-                                            "phoneNumber": self.phone_number,
-                                            "smsCode": sms_code,
-                                            "phoneOS": "Android"
-                                        }) as confirmation:
-            match confirmation.status:
-                case 200:
-                    resp = await confirmation.json()
-                    self.sms_code = sms_code
-                    self.refr_token = resp['refreshToken']
-                    self.auth_token = resp['authToken']
-                    self._log.debug(f'sms code confirmed')
-                    return True
-                case 401:
-                    self._log.error(f'could not confirm sms code, unauthorized')
-                    raise UnauthorizedError(reason=confirmation)
-                case 404:
-                    self._log.error(f'could not confirm sms code, not found')
-                    raise NotFoundError(reason=confirmation)
-                case _:
-                    self._log.error(f'could not confirm sms code, unhandled status')
 
-            raise UnidentifiedAPIError(reason=confirmation)
+        resp = await self.request(method='post',
+                                  action='confirm sms code',
+                                  url=confirm_sms_code,
+                                  auth=False,
+                                  headers=appjson,
+                                  data={
+                                      "phoneNumber": self.phone_number,
+                                      "smsCode": sms_code,
+                                      "phoneOS": "Android"
+                                  },
+                                  autorefresh=False)
+
+        if resp.status == 200:
+            auth_token_data = await resp.json()
+            self.sms_code = sms_code
+            self.refr_token = auth_token_data['refreshToken']
+            self.auth_token = auth_token_data['authToken']
+            self._log.debug(f'sms code confirmed')
+            return True
+        else:
+            return False
 
     async def refresh_token(self) -> bool:
         """Refreshes authorization token using refresh token
 
         :return: True if Inpost.auth_token gets refreshed
         :rtype: bool
         :raises RefreshTokenError: Missing refresh token
@@ -154,40 +221,36 @@
         """
         self._log.info(f'refreshing token')
 
         if not self.refr_token:
             self._log.error(f'refresh token missing')
             raise RefreshTokenError(reason='Refresh token missing')
 
-        async with await self.sess.post(url=refresh_token,
-                                        headers=appjson,
-                                        json={
-                                            "refreshToken": self.refr_token,
-                                            "phoneOS": "Android"
-                                        }) as confirmation:
-            match confirmation.status:
-                case 200:
-                    resp = await confirmation.json()
-                    if resp['reauthenticationRequired']:
-                        self._log.error(f'could not refresh token, log in again')
-                        raise ReAuthenticationError(reason='You need to log in again!')
+        resp = await self.request(method='post',
+                                  action='refresh token',
+                                  url=refresh_token,
+                                  auth=False,
+                                  headers=appjson,
+                                  data={
+                                      "refreshToken": self.refr_token,
+                                      "phoneOS": "Android"
+                                  },
+                                  autorefresh=False)
+
+        if resp.status == 200:
+            confirmation = await resp.json()
+            if confirmation['reauthenticationRequired']:
+                self._log.error(f'could not refresh token, log in again')
+                raise ReAuthenticationError(reason='You need to log in again!')
 
-                    self.auth_token = resp['authToken']
-                    self._log.debug(f'token refreshed')
-                    return True
-                case 401:
-                    self._log.error(f'could not refresh token, unauthorized')
-                    raise UnauthorizedError(reason=confirmation)
-                case 404:
-                    self._log.error(f'could not refresh token, not found')
-                    raise NotFoundError(reason=confirmation)
-                case _:
-                    self._log.error(f'could not refresh token, unhandled status')
-
-            raise UnidentifiedAPIError(reason=confirmation)
+            self.auth_token = confirmation['authToken']
+            self._log.debug(f'token refreshed')
+            return True
+        else:
+            return False
 
     async def logout(self) -> bool:
         """Logouts user from inpost api service
 
         :return: True if the user is logged out
         :rtype: bool
         :raises NotAuthenticatedError: User not authenticated in inpost service
@@ -196,34 +259,31 @@
         :raises UnidentifiedAPIError: Unexpected thing happened"""
         self._log.info(f'logging out')
 
         if not self.auth_token:
             self._log.error(f'authorization token missing')
             raise NotAuthenticatedError(reason='Not logged in')
 
-        async with await self.sess.post(url=logout,
-                                        headers={'Authorization': self.auth_token}) as resp:
-            match resp.status:
-                case 200:
-                    self.phone_number = None
-                    self.refr_token = None
-                    self.auth_token = None
-                    self.sms_code = None
-                    self._log.debug('logged out')
-                    return True
-                case 401:
-                    self._log.error('could not log out, unauthorized')
-                    raise UnauthorizedError(reason=resp)
-                case 404:
-                    self._log.error('could not log out, not found')
-                    raise NotFoundError(reason=resp)
-                case _:
-                    self._log.error('could not log out, unhandled status')
-
-            raise UnidentifiedAPIError(reason=resp)
+        resp = await self.request(method='post',
+                                  action='logout',
+                                  url=logout,
+                                  auth=True,
+                                  headers=None,
+                                  data=None,
+                                  autorefresh=True)
+
+        if resp.status == 200:
+            self.phone_number = None
+            self.refr_token = None
+            self.auth_token = None
+            self.sms_code = None
+            self._log.debug('logged out')
+            return True
+        else:
+            return False
 
     async def disconnect(self) -> bool:
         """Simplified method to logout and close user's session
 
         :return: True if user is logged out and session is closed else False
         :raises NotAuthenticatedError: User not authenticated in inpost service"""
         self._log.info(f'disconnecting')
@@ -254,31 +314,25 @@
         :raises UnidentifiedAPIError: Unexpected thing happened"""
         self._log.info(f'getting parcel with shipment number: {shipment_number}')
 
         if not self.auth_token:
             self._log.error(f'authorization token missing')
             raise NotAuthenticatedError(reason='Not logged in')
 
-        async with await self.sess.get(url=f"{parcel}{shipment_number}",
-                                       headers={'Authorization': self.auth_token},
-                                       ) as resp:
-            match resp.status:
-                case 200:
-                    self._log.debug(f'parcel with shipment number {shipment_number} received')
-                    return await resp.json() if not parse else Parcel(await resp.json(), logger=self._log)
-                case 401:
-                    self._log.error(f'could not get parcel with shipment number {shipment_number}, unauthorized')
-                    raise UnauthorizedError(reason=resp)
-                case 404:
-                    self._log.error(f'could not get parcel with shipment number {shipment_number}, not found')
-                    raise NotFoundError(reason=resp)
-                case _:
-                    self._log.error(f'could not get parcel with shipment number {shipment_number}, unhandled status')
-
-            raise UnidentifiedAPIError(reason=resp)
+        resp = await self.request(method='get',
+                                  action=f"parcel with shipment number {shipment_number}",
+                                  url=f"{parcel}{shipment_number}",
+                                  auth=True,
+                                  headers=None,
+                                  data=None,
+                                  autorefresh=True)
+
+        if resp.status == 200:
+            self._log.debug(f'parcel with shipment number {shipment_number} received')
+            return await resp.json() if not parse else Parcel(await resp.json(), logger=self._log)
 
     async def get_parcels(self,
                           parcel_type: ParcelType = ParcelType.TRACKED,
                           status: ParcelStatus | List[ParcelStatus] | None = None,
                           pickup_point: str | List[str] | None = None,
                           shipment_type: ParcelShipmentType | List[ParcelShipmentType] | None = None,
                           parcel_size: ParcelLockerSize | ParcelCarrierSize | None = None,
@@ -324,91 +378,78 @@
             case ParcelType.RETURNS:
                 self._log.debug(f'getting parcel type {parcel_type}')
                 url = returns
             case _:
                 self._log.error(f'wrong parcel type {parcel_type}')
                 raise ParcelTypeError(reason=f'Unknown parcel type: {parcel_type}')
 
-        async with await self.sess.get(url=url,
-                                       headers={'Authorization': self.auth_token},
-                                       ) as resp:
-            match resp.status:
-                case 200:
-                    self._log.debug(f'received {parcel_type} parcels')
-                    _parcels = (await resp.json())['parcels']
-
-                    if status is not None:
-                        if isinstance(status, ParcelStatus):
-                            status = [status]
-
-                        _parcels = (_parcel for _parcel in _parcels if ParcelStatus[_parcel['status']] in status)
-
-                    if pickup_point is not None:
-                        if isinstance(pickup_point, str):
-                            pickup_point = [pickup_point]
-
-                        _parcels = (_parcel for _parcel in _parcels if
-                                    _parcel['pickUpPoint']['name'] in pickup_point)
-
-                    if shipment_type is not None:
-                        if isinstance(shipment_type, ParcelShipmentType):
-                            shipment_type = [shipment_type]
-
-                        _parcels = (_parcel for _parcel in _parcels if
-                                    ParcelShipmentType[_parcel['shipmentType']] in shipment_type)
-
-                    if parcel_size is not None:
-                        if isinstance(parcel_size, ParcelCarrierSize):
-                            parcel_size = [parcel_size]
-
-                            _parcels = (_parcel for _parcel in _parcels if
-                                        ParcelCarrierSize[_parcel['parcelSize']] in parcel_size)
-
-                        if isinstance(parcel_size, ParcelLockerSize):
-                            parcel_size = [parcel_size]
-
-                            _parcels = (_parcel for _parcel in _parcels if
-                                        ParcelLockerSize[_parcel['parcelSize']] in parcel_size)
-
-                    return _parcels if not parse else [Parcel(parcel_data=data, logger=self._log) for data in
-                                                       _parcels]
-                case 401:
-                    self._log.error(f'could not get parcels, unauthorized')
-                    raise UnauthorizedError(reason=resp)
-                case 404:
-                    self._log.error(f'could not get parcels, not found')
-                    raise NotFoundError(reason=resp)
-                case _:
-                    self._log.error(f'could not get parcels, unhandled status')
+        resp = await self.request(method='get',
+                                  action='get parcels',
+                                  url=url,
+                                  auth=True,
+                                  headers=None,
+                                  data=None,
+                                  autorefresh=True)
+
+        if resp.status == 200:
+            self._log.debug(f'received {parcel_type} parcels')
+            _parcels = (await resp.json())['parcels']
+
+            if status is not None:
+                if isinstance(status, ParcelStatus):
+                    status = [status]
+
+                _parcels = (_parcel for _parcel in _parcels if ParcelStatus[_parcel['status']] in status)
+
+            if pickup_point is not None:
+                if isinstance(pickup_point, str):
+                    pickup_point = [pickup_point]
 
-            raise UnidentifiedAPIError(reason=resp)
+                _parcels = (_parcel for _parcel in _parcels if
+                            _parcel['pickUpPoint']['name'] in pickup_point)
+
+            if shipment_type is not None:
+                if isinstance(shipment_type, ParcelShipmentType):
+                    shipment_type = [shipment_type]
+
+                _parcels = (_parcel for _parcel in _parcels if
+                            ParcelShipmentType[_parcel['shipmentType']] in shipment_type)
+
+            if parcel_size is not None:
+                if isinstance(parcel_size, ParcelCarrierSize):
+                    parcel_size = [parcel_size]
+
+                    _parcels = (_parcel for _parcel in _parcels if
+                                ParcelCarrierSize[_parcel['parcelSize']] in parcel_size)
+
+                if isinstance(parcel_size, ParcelLockerSize):
+                    parcel_size = [parcel_size]
+
+                    _parcels = (_parcel for _parcel in _parcels if
+                                ParcelLockerSize[_parcel['parcelSize']] in parcel_size)
+
+            return list(_parcels) if not parse else [Parcel(parcel_data=data, logger=self._log) for data in _parcels]
 
     async def get_multi_compartment(self, multi_uuid: str | int, parse: bool = False) -> dict | List[Parcel]:
         if not self.auth_token:
             self._log.error(f'authorization token missing')
             raise NotAuthenticatedError(reason='Not logged in')
 
-        async with await self.sess.get(url=f"{multi}{multi_uuid}",
-                                       headers={'Authorization': self.auth_token},
-                                       ) as resp:
-            match resp.status:
-                case 200:
-                    self._log.debug(f'parcel with multicompartment uuid {multi_uuid} received')
-                    return await resp.json() if not parse else [Parcel(data, logger=self._log) for data in
-                                                                (await resp.json())['parcels']]
-                case 401:
-                    self._log.error(f'could not get parcel with multicompartment uuid {multi_uuid}, unauthorized')
-                    raise UnauthorizedError(reason=resp)
-                case 404:
-                    self._log.error(f'could not get parcel with multicompartment uuid {multi_uuid}, not found')
-                    raise NotFoundError(reason=resp)
-                case _:
-                    self._log.error(f'could not get parcel with multicompartment uuid {multi_uuid}, unhandled status')
-
-            raise UnidentifiedAPIError(reason=resp)
+        resp = await self.request(method='get',
+                                  action=f"parcel with multicompartment uuid {multi_uuid}",
+                                  url=f"{multi}{multi_uuid}",
+                                  auth=True,
+                                  headers=None,
+                                  data=None,
+                                  autorefresh=True)
+
+        if resp.status == 200:
+            self._log.debug(f'parcel with multicompartment uuid {multi_uuid} received')
+            return (await resp.json())['parcels'] if not parse else [Parcel(data, logger=self._log) for data in
+                                                                     (await resp.json())['parcels']]
 
     async def collect_compartment_properties(self, shipment_number: str | int | None = None,
                                              parcel_obj: Parcel | None = None, location: dict | None = None) -> bool:
         """Validates sent data and fetches required compartment properties for opening
 
         :param shipment_number: Parcel's shipment number
         :type shipment_number: int | str | None
@@ -436,39 +477,30 @@
 
         if shipment_number is not None and parcel_obj is None:
             self._log.debug(f'parcel_obj not provided, getting from shipment number {shipment_number}')
             parcel_obj = await self.get_parcel(shipment_number=shipment_number, parse=True)
 
         self._log.info(f'collecting compartment properties for {parcel_obj.shipment_number}')
 
-        async with await self.sess.post(url=collect,
-                                        headers={'Authorization': self.auth_token},
-                                        json={
-                                            'parcel': parcel_obj.compartment_open_data,
-                                            'geoPoint': location if location is not None else parcel_obj.mocked_location
-                                        }) as collect_resp:
-            match collect_resp.status:
-                case 200:
-                    self._log.debug(f'collected compartment properties for {parcel_obj.shipment_number}')
-                    parcel_obj.compartment_properties = await collect_resp.json()
-                    self.parcel = parcel_obj
-                    return True
-                case 401:
-                    self._log.error(f'could not collect compartment properties for {parcel_obj.shipment_number}, '
-                                    f'unauthorized')
-                    raise UnauthorizedError(reason=collect_resp)
-                case 404:
-                    self._log.error(f'could not collect compartment properties for {parcel_obj.shipment_number}, not '
-                                    f'found')
-                    raise NotFoundError(reason=collect_resp)
-                case _:
-                    self._log.error(f'could not collect compartment properties for {parcel_obj.shipment_number}, '
-                                    f'unhandled status')
-
-            raise UnidentifiedAPIError(reason=collect_resp)
+        resp = await self.request(method='post',
+                                  action='collect compartment properties',
+                                  url=collect,
+                                  auth=True,
+                                  headers=None,
+                                  data={
+                                      'parcel': parcel_obj.compartment_open_data,
+                                      'geoPoint': location if location is not None else parcel_obj.mocked_location
+                                  },
+                                  autorefresh=True)
+
+        if resp.status == 200:
+            self._log.debug(f'collected compartment properties for {parcel_obj.shipment_number}')
+            parcel_obj.compartment_properties = await resp.json()
+            self.parcel = parcel_obj
+            return True
 
     async def open_compartment(self) -> bool:
         """Opens compartment for `Inpost.parcel` object
 
         :return: True if compartment gets opened
         :rtype: bool
         :raises NotAuthenticatedError: User not authenticated in inpost service
@@ -477,34 +509,25 @@
         :raises UnidentifiedAPIError: Unexpected thing happened"""
         self._log.info(f'opening compartment for {self.parcel.shipment_number}')
 
         if not self.auth_token:
             self._log.debug(f'authorization token missing')
             raise NotAuthenticatedError(reason='Not logged in')
 
-        async with await self.sess.post(url=compartment_open,
-                                        headers={'Authorization': self.auth_token},
-                                        json={
-                                            'sessionUuid': self.parcel.compartment_properties.session_uuid
-                                        }) as compartment_open_resp:
-            match compartment_open_resp.status:
-                case 200:
-                    self._log.debug(f'opened comaprtment for {self.parcel.shipment_number}')
-                    self.parcel.compartment_properties.location = await compartment_open_resp.json()
-                    return True
-                case 401:
-                    self._log.error(f'could not open compartment for {self.parcel.shipment_number}, unauthorized')
-                    raise UnauthorizedError(reason=compartment_open_resp)
-                case 404:
-                    self._log.error(f'could not open compartment for {self.parcel.shipment_number}, not found')
-                    raise NotFoundError(reason=compartment_open_resp)
-                case _:
-                    self._log.error(f'could not open compartment for {self.parcel.shipment_number}, unhandled status')
+        resp = await self.request(method='post',
+                                  action=f"open compartment for {self.parcel.shipment_number}",
+                                  url=compartment_open,
+                                  auth=True,
+                                  headers=None,
+                                  data={'sessionUuid': self.parcel.compartment_properties.session_uuid},
+                                  autorefresh=True)
 
-            raise UnidentifiedAPIError(reason=compartment_open_resp)
+        if resp.status == 200:
+            self._log.debug(f'opened compartment for {self.parcel.shipment_number}')
+            return True
 
     async def check_compartment_status(self,
                                        expected_status: CompartmentExpectedStatus = CompartmentExpectedStatus.OPENED) -> bool:
         """Checks and compare compartment status (e.g. opened, closed) with expected status
 
         :param expected_status: Compartment expected status
         :type expected_status: CompartmentExpectedStatus
@@ -520,38 +543,29 @@
             self._log.debug(f'authorization token missing')
             raise NotAuthenticatedError(reason='Not logged in')
 
         if not self.parcel:
             self._log.debug(f'parcel missing')
             raise NoParcelError(reason='Parcel is not set')
 
-        async with await self.sess.post(url=compartment_status,
-                                        headers={'Authorization': self.auth_token},
-                                        json={
-                                            'sessionUuid': self.parcel.compartment_properties.session_uuid,
-                                            'expectedStatus': expected_status.name
-                                        }) as compartment_status_resp:
-            match compartment_status_resp.status:
-                case 200:
-                    self._log.debug(f'checked compartment status for {self.parcel.shipment_number}')
-                    self.parcel.compartment_status = (await compartment_status_resp.json())['status']
-                    return CompartmentExpectedStatus[
-                        (await compartment_status_resp.json())['status']] == expected_status
-                case 401:
-                    self._log.error(
-                        f'could not check compartment status for {self.parcel.shipment_number}, unauthorized')
-                    raise UnauthorizedError(reason=compartment_status_resp)
-                case 404:
-                    self._log.error(f'could not check compartment status for {self.parcel.shipment_number}, not found')
-                    raise NotFoundError(reason=compartment_status_resp)
-                case _:
-                    self._log.error(
-                        f'could not check compartment status for {self.parcel.shipment_number}, unhandled status')
-
-            raise UnidentifiedAPIError(reason=compartment_status_resp)
+        resp = await self.request(method='post',
+                                  action='check compartment status',
+                                  url=compartment_status,
+                                  auth=True,
+                                  headers=None,
+                                  data={
+                                      'sessionUuid': self.parcel.compartment_properties.session_uuid,
+                                      'expectedStatus': expected_status.name
+                                  },
+                                  autorefresh=True)
+
+        if resp.status == 200:
+            self._log.debug(f'checked compartment status for {self.parcel.shipment_number}')
+            self.parcel.compartment_status = (await resp.json())['status']
+            return CompartmentExpectedStatus[(await resp.json())['status']] == expected_status
 
     async def terminate_collect_session(self) -> bool:
         """Terminates user session in inpost api service
 
         :return: True if the user session is terminated
         :rtype: bool
         :raises NotAuthenticatedError: User not authenticated in inpost service
@@ -560,35 +574,26 @@
         :raises UnidentifiedAPIError: Unexpected thing happened"""
         self._log.info(f'terminating collect session for {self.parcel.shipment_number}')
 
         if not self.auth_token:
             self._log.debug(f'authorization token missing')
             raise NotAuthenticatedError(reason='Not logged in')
 
-        async with await self.sess.post(url=terminate_collect_session,
-                                        headers={'Authorization': self.auth_token},
-                                        json={
-                                            'sessionUuid': self.parcel.compartment_properties.session_uuid
-                                        }) as terminate_resp:
-            match terminate_resp.status:
-                case 200:
-                    self._log.debug(f'terminated collect session for {self.parcel.shipment_number}')
-                    return True
-                case 401:
-                    self._log.error(
-                        f'could not terminate collect session for {self.parcel.shipment_number}, unauthorized')
-                    raise UnauthorizedError(reason=terminate_resp)
-                case 404:
-                    self._log.error(f'could not terminate collect session for {self.parcel.shipment_number}, not found')
-                    raise NotFoundError(reason=terminate_resp)
-                case _:
-                    self._log.error(
-                        f'could not terminate collect session for {self.parcel.shipment_number}, unhandled status')
-
-            raise UnidentifiedAPIError(reason=terminate_resp)
+        resp = await self.request(method='post',
+                                  action='terminate collect session',
+                                  url=terminate_collect_session,
+                                  auth=True,
+                                  headers=None,
+                                  data={
+                                      'sessionUuid': self.parcel.compartment_properties.session_uuid
+                                  },
+                                  autorefresh=True)
+        if resp.status == 200:
+            self._log.debug(f'terminated collect session for {self.parcel.shipment_number}')
+            return True
 
     async def collect(self, shipment_number: str | None = None, parcel_obj: Parcel | None = None,
                       location: dict | None = None) -> bool:
         """Simplified method to open compartment
 
         :param shipment_number: Parcel's shipment number
         :type shipment_number: int | str | None
@@ -613,36 +618,64 @@
         if not self.auth_token:
             self._log.error(f'authorization token missing')
             raise NotAuthenticatedError(reason='Not logged in')
 
         if shipment_number is not None and parcel_obj is None:
             parcel_obj = await self.get_parcel(shipment_number=shipment_number, parse=True)
 
-        self._log.info(f'collecing parcel with shipment number {parcel_obj.shipment_number}')
+        self._log.info(f'collecting parcel with shipment number {parcel_obj.shipment_number}')
 
         if await self.collect_compartment_properties(parcel_obj=parcel_obj, location=location):
             if await self.open_compartment():
                 if await self.check_compartment_status():
                     return True
 
         return False
 
     async def close_compartment(self) -> bool:
-        """Checks whether actual compartment status and expected one matches then notifies inpost api that compartment is closed
+        """Checks whether actual compartment status and expected one matches then notifies inpost api that
+        compartment is closed
 
         :return: True if compartment status is closed and successfully terminates user's session else False
         :rtype: bool"""
         self._log.info(f'closing compartment for {self.parcel.shipment_number}')
 
         if await self.check_compartment_status(expected_status=CompartmentExpectedStatus.CLOSED):
             if await self.terminate_collect_session():
                 return True
 
         return False
 
+    async def reopen_compartment(self) -> bool:
+        """Reopens compartment for `Inpost.parcel` object
+
+        :return: True if compartment gets reopened
+        :rtype: bool
+        :raises NotAuthenticatedError: User not authenticated in inpost service
+        :raises UnauthorizedError: Unauthorized access to inpost services,
+        :raises NotFoundError: Phone number not found
+        :raises UnidentifiedAPIError: Unexpected thing happened"""
+        self._log.info(f'reopening compartment for {self.parcel.shipment_number}')
+
+        if not self.auth_token:
+            self._log.debug(f'authorization token missing')
+            raise NotAuthenticatedError(reason='Not logged in')
+
+        resp = await self.request(method='post',
+                                  action=f"reopen compartment for {self.parcel.shipment_number}",
+                                  url=compartment_open,
+                                  auth=True,
+                                  headers=None,
+                                  data={'sessionUuid': self.parcel.compartment_properties.session_uuid},
+                                  autorefresh=True)
+
+        if resp.status == 200:
+            self._log.debug(f'opened compartment for {self.parcel.shipment_number}')
+            return True
+
     async def get_prices(self) -> dict:
         """Fetches prices for inpost services
 
         :return: :class:`dict` of prices for inpost services
         :rtype: dict
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
@@ -650,30 +683,24 @@
         :raises UnidentifiedAPIError: Unexpected thing happened"""
         self._log.info(f'getting parcel prices')
 
         if not self.auth_token:
             self._log.debug(f'authorization token missing')
             raise NotAuthenticatedError(reason='Not logged in')
 
-        async with await self.sess.get(url=parcel_prices,
-                                       headers={'Authorization': self.auth_token}) as resp:
-            match resp.status:
-                case 200:
-                    self._log.debug(f'got parcel prices')
-                    return await resp.json()
-                case 401:
-                    self._log.error('could not get parcel prices, unauthorized')
-                    raise UnauthorizedError(reason=resp)
-                case 404:
-                    self._log.error('could not get parcel prices, not found')
-                    raise NotFoundError(reason=resp)
-                case _:
-                    self._log.error('could not get parcel prices, unhandled status')
-
-            raise UnidentifiedAPIError(reason=resp)
+        resp = await self.request(method='get',
+                                  action='get prices',
+                                  url=parcel_prices,
+                                  auth=True,
+                                  headers=None,
+                                  data=None,
+                                  autorefresh=True)
+        if resp.status == 200:
+            self._log.debug(f'got parcel prices')
+            return await resp.json()
 
     async def get_friends(self, parse=False) -> dict | List[Friend]:
         """Fetches user friends for inpost services
 
         :param parse: switch for parsing response
         :type parse: bool
         :return: :class:`dict` of user friends for inpost services
@@ -684,63 +711,52 @@
         :raises UnidentifiedAPIError: Unexpected thing happened"""
         self._log.info(f'getting friends')
 
         if not self.auth_token:
             self._log.debug(f'authorization token missing')
             raise NotAuthenticatedError(reason='Not logged in')
 
-        async with await self.sess.get(url=friendship,
-                                       headers={'Authorization': self.auth_token}) as resp:
-            match resp.status:
-                case 200:
-                    self._log.debug(f'got user friends')
-                    r = await resp.json()
-                    return r if not parse else [Friend(friend_data=friend, logger=self._log) for friend in r['friends']]
-                case 401:
-                    self._log.error('could not get user friends, unauthorized')
-                    raise UnauthorizedError(reason=resp)
-                case 404:
-                    self._log.error('could not get user friends, not found')
-                    raise NotFoundError(reason=resp)
-                case _:
-                    self._log.error('could not get user friends, unhandled status')
-
-            raise UnidentifiedAPIError(reason=resp)
+        resp = await self.request(method='get',
+                                  action='get friends',
+                                  url=friendship,
+                                  auth=True,
+                                  headers=None,
+                                  data=None,
+                                  autorefresh=True)
+        if resp.status == 200:
+            self._log.debug(f'got user friends')
+            _friends = await resp.json()
+            return _friends if not parse else [Friend(friend_data=friend, logger=self._log) for friend in
+                                               _friends['friends']]
 
     async def get_parcel_friends(self, shipment_number: int | str, parse=False) -> dict:
         self._log.info(f'getting parcel friends')
 
         if not self.auth_token:
             self._log.debug(f'authorization token missing')
             raise NotAuthenticatedError(reason='Not logged in')
 
-        async with await self.sess.get(url=f"{friendship}{shipment_number}",
-                                       headers={'Authorization': self.auth_token}) as resp:
-            match resp.status:
-                case 200:
-                    self._log.debug(f'got user friends')
-                    r = await resp.json()
-                    if 'sharedWith' in r:
-                        return r if not parse else {
-                            'friends': [Friend(friend_data=friend, logger=self._log) for friend in r['friends']],
-                            'shared_with': [Friend(friend_data=friend, logger=self._log) for friend in r['sharedWith']]}
-                    return r if not parse else {
-                        'friends': [Friend(friend_data=friend, logger=self._log) for friend in r['friends']]
-                    }
-
-                case 401:
-                    self._log.error('could not get user friends, unauthorized')
-                    raise UnauthorizedError(reason=resp)
-                case 404:
-                    self._log.error('could not get user friends, not found')
-                    raise NotFoundError(reason=resp)
-                case _:
-                    self._log.error('could not get user friends, unhandled status')
-
-            raise UnidentifiedAPIError(reason=resp)
+        resp = await self.request(method='get',
+                                  action='get parcel friends',
+                                  url=f"{friendship}{shipment_number}",
+                                  auth=True,
+                                  headers=None,
+                                  data=None,
+                                  autorefresh=True)
+
+        if resp.status == 200:
+            self._log.debug(f'got parcel friends')
+            r = await resp.json()
+            if 'sharedWith' in r:
+                return r if not parse else {
+                    'friends': [Friend(friend_data=friend, logger=self._log) for friend in r['friends']],
+                    'shared_with': [Friend(friend_data=friend, logger=self._log) for friend in r['sharedWith']]}
+            return r if not parse else {
+                'friends': [Friend(friend_data=friend, logger=self._log) for friend in r['friends']]
+            }
 
     async def add_friend(self, name: str, phone_number: str | int, code: str | int, parse=False) -> dict | Friend:
         """Adds user friends for inpost services
 
         :param name: name of further inpost friend
         :type name: str
         :param phone_number: further friend phone number
@@ -766,80 +782,53 @@
         if len(name) > 20:
             raise ValueError(f'Name too long: {name} (over 20 characters')
 
         if code:
             if isinstance(code, int):
                 code = str(code)
 
-            async with await self.sess.post(url=validate_friendship,
-                                            headers={'Authorization': self.auth_token},
-                                            json={'invitationCode': code}) as resp:
-                match resp.status:
-                    case 200:
-                        self._log.debug(f'validated friendship code')
-                        async with await self.sess.post(url=accept_friendship,
-                                                        headers={'Authorization': self.auth_token},
-                                                        json={'invitationCode': code,
-                                                              'friendName': name}):
-                            match resp.status:
-                                case 200:
-                                    self._log.debug(f'added user friend')
-                                    return await resp.json() if not parse else Friend(await resp.json(),
-                                                                                      logger=self._log)
-
-                                case 401:
-                                    self._log.error('could not add user friends, unauthorized')
-                                    raise UnauthorizedError(reason=resp)
-                                case 404:
-                                    self._log.error('could not add user friends, not found')
-                                    raise NotFoundError(reason=resp)
-                                case _:
-                                    self._log.error('could not add user friends, unhandled status')
-                    case 401:
-                        self._log.error('could not validate friendship code, unauthorized')
-                        raise UnauthorizedError(reason=resp)
-                    case 404:
-                        self._log.error('could not validate friendship code, not found')
-                        raise NotFoundError(reason=resp)
-                    case _:
-                        self._log.error('could not validate friendship code, unhandled status')
-
-                raise UnidentifiedAPIError(reason=resp)
+            resp = await self.request(method='post',
+                                      action='add friend',
+                                      url=validate_friendship,
+                                      auth=True,
+                                      headers=None,
+                                      data={'invitationCode': code},
+                                      autorefresh=True)
+
+            if resp.status == 200:
+                self._log.debug(f'added user friend')
+                return await resp.json() if not parse else Friend(await resp.json(), logger=self._log)
 
         else:
             if isinstance(phone_number, int):
                 phone_number = str(phone_number)
 
-            async with await self.sess.post(url=friendship,
-                                            headers={'Authorization': self.auth_token},
-                                            json={'phoneNumber': phone_number,
-                                                  'name': name}) as resp:
-                match resp.status:
-                    case 200:
-                        self._log.debug(f'added user friend')
-                        r = await resp.json()
-                        if r['status'] == "AUTO_ACCEPT":
-                            return {'phoneNumber': phone_number, 'name': name} if not parse \
-                                else Friend({'phoneNumber': phone_number, 'name': name}, logger=self._log)
-
-                        elif r['status'] == "RETURN_INVITATION_CODE":
-                            return r if not parse else Friend.from_invitation(invitation_data=r, logger=self._log)
-
-                        else:
-                            ...
-                    case 401:
-                        self._log.error('could not add user friends, unauthorized')
-                        raise UnauthorizedError(reason=resp)
-                    case 404:
-                        self._log.error('could not add user friends, not found')
-                        raise NotFoundError(reason=resp)
-                    case _:
-                        self._log.error('could not add user friends, unhandled status')
+            resp = await self.request(method='post',
+                                      action='add friend',
+                                      url=friendship,
+                                      auth=True,
+                                      headers=None,
+                                      data={
+                                          'phoneNumber': phone_number,
+                                          'name': name
+                                      },
+                                      autorefresh=True)
+
+            if resp.status == 200:
+                self._log.debug(f'added user friend')
+                r = await resp.json()
+                if r['status'] == "AUTO_ACCEPT":
+                    return {'phoneNumber': phone_number, 'name': name} if not parse \
+                        else Friend({'phoneNumber': phone_number, 'name': name}, logger=self._log)
 
-                raise UnidentifiedAPIError(reason=resp)
+                elif r['status'] == "RETURN_INVITATION_CODE":
+                    return r if not parse else Friend.from_invitation(invitation_data=r, logger=self._log)
+
+                else:
+                    self._log.debug(r)
 
     async def remove_friend(self, uuid: str | None, name: str | None, phone_number: str | int | None) -> bool:
         """Removes user friend for inpost services with specified `uuid`/`phone_number`/`name`
 
         :param uuid: uuid of inpost friend to remove
         :type uuid: str | None
         :param name: name of inpost friend to remove
@@ -869,30 +858,27 @@
         if uuid is None:
             f = await self.get_friends()
             if phone_number:
                 uuid = next((friend['uuid'] for friend in f['friends'] if friend['phoneNumber'] == phone_number))
             else:
                 uuid = next((friend['uuid'] for friend in f['friends'] if friend['name'] == name))
 
-        async with await self.sess.delete(url=f'{friendship}{uuid}',
-                                          headers={'Authorization': self.auth_token}) as resp:
-            match resp.status:
-                case 200:
-                    self._log.debug(f'removed user friend')
-                    return True
-                case 401:
-                    self._log.error('could not remove user friend, unauthorized')
-                    raise UnauthorizedError(reason=resp)
-                case 404:
-                    self._log.error('could not remove user friend, not found')
-                    raise NotFoundError(reason=resp)
-                case _:
-                    self._log.error('could not remove user friend, unhandled status')
+        resp = await self.request(method='delete',
+                                  action='remove user friend',
+                                  url=f'{friendship}{uuid}',
+                                  auth=True,
+                                  headers=None,
+                                  data=None,
+                                  autorefresh=True)
 
-            raise UnidentifiedAPIError(reason=resp)
+        if resp.status == 200:
+            self._log.debug(f'removed user friend')
+            return True
+
+        return False
 
     async def update_friend(self, uuid: str | None, phone_number: str | int | None, name: str):
         """Updates user friend for inpost services with specified `name`
 
         :param uuid: uuid of inpost friend to update
         :type uuid: str | None
         :param name: new name of inpost friend
@@ -917,33 +903,30 @@
             raise ValueError(f'Name too long: {name} (over 20 characters')
 
         if isinstance(phone_number, int):
             phone_number = str(phone_number)
 
         if uuid is None:
             uuid = next(
-                (friend['uuid'] for friend in (await self.get_friends())['friends'] if friend['phoneNumber'] == phone_number))
+                (friend['uuid'] for friend in (await self.get_friends())['friends'] if
+                 friend['phoneNumber'] == phone_number))
 
-        async with await self.sess.patch(url=f'{friends}{uuid}',
-                                         headers={'Authorization': self.auth_token},
-                                         json={'name': name}) as resp:
-            match resp.status:
-                case 200:
-                    self._log.debug(f'updated user friend')
-                    return True
-                case 401:
-                    self._log.error('could not update user friend, unauthorized')
-                    raise UnauthorizedError(reason=resp)
-                case 404:
-                    self._log.error('could not update user friend, not found')
-                    raise NotFoundError(reason=resp)
-                case _:
-                    self._log.error('could not update user friend, unhandled status')
+        resp = await self.request(method='patch',
+                                  action='update user friend',
+                                  url=f'{friends}{uuid}',
+                                  auth=True,
+                                  headers=None,
+                                  data=None,
+                                  autorefresh=True)
 
-            raise UnidentifiedAPIError(reason=resp)
+        if resp.status == 200:
+            self._log.debug(f'updated user friend')
+            return True
+
+        return False
 
     async def share_parcel(self, uuid: str, shipment_number: int | str):
         """Shares parcel to a pre-initialized friend
 
         :param uuid: uuid of inpost friend to update
         :type uuid: str
         :param shipment_number: Parcel's shipment number
@@ -957,33 +940,61 @@
 
         self._log.info(f'sharing parcel: {shipment_number}')
 
         if not self.auth_token:
             self._log.debug(f'authorization token missing')
             raise NotAuthenticatedError(reason='Not logged in')
 
-        async with await self.sess.post(url=shared,
-                                        headers={'Authorization': self.auth_token},
-                                        json={
-                                            'parcels': [
-                                                {
-                                                    'shipmentNumber': shipment_number,
-                                                    'friendUuids': [
-                                                        uuid
-                                                    ]
-                                                }
-                                            ],
-                                        }) as share:
-            match share.status:
-                case 200:
-                    self._log.debug(f'shared parcel: {shipment_number}')
-                    return True
-                case 401:
-                    self._log.error(f'could not share parcel: {shipment_number}, unauthorized')
-                    raise UnauthorizedError(reason=share)
-                case 404:
-                    self._log.error(f'could not share parcel: {shipment_number}, not found')
-                    raise NotFoundError(reason=share)
-                case _:
-                    self._log.error(f'could not share parcel: {shipment_number}, unhandled status')
+        resp = await self.request(method='post',
+                                  action=f'share parcel: {shipment_number}',
+                                  url=shared,
+                                  auth=True,
+                                  headers=None,
+                                  data={'parcels': [
+                                      {
+                                          'shipmentNumber': shipment_number,
+                                          'friendUuids': [
+                                              uuid
+                                          ]
+                                      }
+                                  ],
+                                  },
+                                  autorefresh=True)
+
+        if resp.status == 200:
+            self._log.debug(f'updated user friend')
+            return True
+
+        return False
 
-            raise UnidentifiedAPIError(reason=share)
+    # async def get_return_parcels(self):
+    #     """Fetches all available parcels for set `Inpost.phone_number`
+    #
+    #         :return: Fetched returned parcels data
+    #         :rtype: dict | Parcel
+    #         :raises NotAuthenticatedError: User not authenticated in inpost service
+    #         :raises UnauthorizedError: Unauthorized access to inpost services,
+    #         :raises NotFoundError: Phone number not found
+    #         :raises UnidentifiedAPIError: Unexpected thing happened"""
+    #     self._log.info(f'getting all returned parcels')
+    #
+    #     if not self.auth_token:
+    #         self._log.error(f'authorization token missing')
+    #         raise NotAuthenticatedError(reason='Not logged in')
+    #
+    #     async with await self.sess.get(url=returns,
+    #                                    headers={'Authorization': self.auth_token},
+    #                                    ) as resp:
+    #         match resp.status:
+    #             case 200:
+    #                 self._log.debug(f'parcel with shipment number {shipment_number} received')
+    #                 return await resp.json() if not parse else Parcel(await resp.json(), logger=self._log)
+    #             case 401:
+    #                 self._log.error(f'could not get parcel with shipment number {shipment_number}, unauthorized')
+    #                 raise UnauthorizedError(reason=resp)
+    #             case 404:
+    #                 self._log.error(f'could not get parcel with shipment number {shipment_number}, not found')
+    #                 raise NotFoundError(reason=resp)
+    #             case _:
+    #                 self._log.error(f'could not get parcel with shipment number {shipment_number}, unhandled status')
+    #
+    #         raise UnidentifiedAPIError(reason=resp)
```

### Comparing `inpost-0.0.9/inpost/static/__init__.py` & `inpost-0.1.0/inpost/static/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from .parcels import Parcel, Receiver, Sender, PickupPoint, MultiCompartment, Operations, EventLog, SharedTo, \
     QRCode, CompartmentLocation, CompartmentProperties
 from .headers import appjson
 from .statuses import ParcelCarrierSize, ParcelLockerSize, ParcelDeliveryType, ParcelShipmentType, \
     ParcelAdditionalInsurance, ParcelType, ParcelOwnership, CompartmentExpectedStatus, CompartmentActualStatus, \
     ParcelServiceName, ParcelStatus, ReturnsStatus
-from .exceptions import NoParcelError, UnidentifiedParcelError, ParcelTypeError, NotAuthenticatedError, ReAuthenticationError, \
+from .exceptions import NoParcelError, UnidentifiedParcelError, ParcelTypeError, NotAuthenticatedError, \
+    ReAuthenticationError, \
     PhoneNumberError, SmsCodeError, RefreshTokenError, UnidentifiedAPIError, UserLocationError, \
     UnidentifiedError, NotFoundError, UnauthorizedError, SingleParamError, MissingParamsError
 from .endpoints import login, send_sms_code, confirm_sms_code, refresh_token, parcels, parcel, collect, \
     compartment_open, compartment_status, terminate_collect_session, friendship, shared, sent, returns, parcel_prices, \
-    tickets, logout, multi, validate_friendship, accept_friendship
+    tickets, logout, multi, validate_friendship, accept_friendship, parcel_notifications
 from .friends import Friend
+from .notifications import Notification
```

### Comparing `inpost-0.0.9/inpost/static/__pycache__/__init__.cpython-310.pyc` & `inpost-0.1.0/inpost/static/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.9/inpost/static/__pycache__/endpoints.cpython-310.pyc` & `inpost-0.1.0/inpost/static/__pycache__/endpoints.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.9/inpost/static/__pycache__/exceptions.cpython-310.pyc` & `inpost-0.1.0/inpost/static/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.9/inpost/static/__pycache__/friends.cpython-310.pyc` & `inpost-0.1.0/inpost/static/__pycache__/friends.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.9/inpost/static/__pycache__/parcels.cpython-310.pyc` & `inpost-0.1.0/inpost/static/__pycache__/parcels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.9/inpost/static/__pycache__/statuses.cpython-310.pyc` & `inpost-0.1.0/inpost/static/__pycache__/statuses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.9/inpost/static/endpoints.py` & `inpost-0.1.0/inpost/static/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 login: str = 'https://api-inmobile-pl.easypack24.net/v1/authenticate'
 send_sms_code: str = 'https://api-inmobile-pl.easypack24.net/v1/sendSMSCode/'  # get
 confirm_sms_code: str = 'https://api-inmobile-pl.easypack24.net/v1/confirmSMSCode'  # post
 
-# \/ Secured by JWT \/
 
 refresh_token: str = 'https://api-inmobile-pl.easypack24.net/v1/authenticate'  # post
 parcels: str = 'https://api-inmobile-pl.easypack24.net/v3/parcels/tracked'  # get
 parcel: str = 'https://api-inmobile-pl.easypack24.net/v3/parcels/tracked/'  # get
 multi: str = 'https://api-inmobile-pl.easypack24.net/v3/parcels/multi/'  # get
 collect: str = 'https://api-inmobile-pl.easypack24.net/v1/collect/validate'  # post
+reopen: str = 'https://api-inmobile-pl.easypack24.net/v1/collect/compartment/reopen'  # post
 compartment_open: str = 'https://api-inmobile-pl.easypack24.net/v1/collect/compartment/open'  # post
 compartment_status: str = 'https://api-inmobile-pl.easypack24.net/v1/collect/compartment/status'  # post
 terminate_collect_session: str = 'https://api-inmobile-pl.easypack24.net/v1/collect/terminate'  # post
 friendship: str = 'https://api-inmobile-pl.easypack24.net/v1/friends/'  # get, post, patch, delete
 validate_friendship: str = 'https://api-inmobile-pl.easypack24.net/v1/invitations/validate'  # post
 accept_friendship: str = 'https://api-inmobile-pl.easypack24.net/v1/invitations/accept'  # post
 shared: str = 'https://api-inmobile-pl.easypack24.net/v1/parcels/shared'  # post
 sent: str = 'https://api-inmobile-pl.easypack24.net/v3/parcels/sent/'  # get
 returns: str = 'https://api-inmobile-pl.easypack24.net/v1/returns/parcels/'  # get
 parcel_prices: str = 'https://api-inmobile-pl.easypack24.net/v1/prices/parcels'  # get
 tickets: str = 'https://api-inmobile-pl.easypack24.net/v1/returns/tickets'  # get
 logout: str = 'https://api-inmobile-pl.easypack24.net/v1/logout'  # post
+parcel_notifications: str = 'https://api-inmobile-pl.easypack24.net/v2/notifications?type=PUSH%2CNEWS%2CTILE'  # get
```

### Comparing `inpost-0.0.9/inpost/static/exceptions.py` & `inpost-0.1.0/inpost/static/exceptions.py`

 * *Files identical despite different names*

### Comparing `inpost-0.0.9/inpost/static/friends.py` & `inpost-0.1.0/inpost/static/friends.py`

 * *Files identical despite different names*

### Comparing `inpost-0.0.9/inpost/static/parcels.py` & `inpost-0.1.0/inpost/static/parcels.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 
 
 class BaseParcel:
     def __init__(self, parcel_data: dict, logger: logging.Logger):
         self.shipment_number: str = parcel_data['shipmentNumber']
         self._log: logging.Logger = logger.getChild(f'{__class__.__name__}.{self.shipment_number}')
         self.status: ParcelStatus = ParcelStatus[parcel_data['status']]
-        # self.parcel_size: ParcelLockerSize | ParcelCarrierSize = ParcelLockerSize[parcel_data['parcelSize']] \
-        #     if self.shipment_type == ParcelShipmentType.parcel else ParcelCarrierSize[parcel_data['parcelSize']]
         self.expiry_date: arrow | None = get(parcel_data['expiryDate']) if 'expiryDate' in parcel_data else None
         self.operations: Operations = Operations(operations_data=parcel_data['operations'], logger=self._log)
         self.event_log: List[EventLog] = [EventLog(eventlog_data=event, logger=self._log)
                                           for event in parcel_data['eventLog']]
 
 
 class Parcel(BaseParcel):
@@ -29,36 +27,31 @@
     :type parcel_data: dict
     :param logger: :class:`logging.Logger` parent instance
     :type logger: logging.Logger"""
 
     def __init__(self, parcel_data: dict, logger: logging.Logger):
         """Constructor method"""
         super().__init__(parcel_data, logger)
-        # self.shipment_number: str = parcel_data['shipmentNumber']
         self._log: logging.Logger = logger.getChild(f'{__class__.__name__}.{self.shipment_number}')
         self.shipment_type: ParcelShipmentType = ParcelShipmentType[parcel_data['shipmentType']]
         self._open_code: str | None = parcel_data['openCode'] if 'openCode' in parcel_data else None
         self._qr_code: QRCode | None = QRCode(qrcode_data=parcel_data['qrCode'], logger=self._log) \
             if 'qrCode' in parcel_data else None
         self.stored_date: arrow | None = get(parcel_data['storedDate']) if 'storedDate' in parcel_data else None
         self.pickup_date: arrow | None = get(parcel_data['pickUpDate']) if 'pickUpDate' in parcel_data else None
-        # self.expiry_date: arrow | None = get(parcel_data['expiryDate']) if 'expiryDate' in parcel_data else None
         self.parcel_size: ParcelLockerSize | ParcelCarrierSize = ParcelLockerSize[parcel_data['parcelSize']] \
             if self.shipment_type == ParcelShipmentType.parcel else ParcelCarrierSize[parcel_data['parcelSize']]
         self.receiver: Receiver = Receiver(receiver_data=parcel_data['receiver'], logger=self._log)
         self.sender: Sender = Sender(sender_data=parcel_data['sender'], logger=self._log)
         self.pickup_point: PickupPoint = PickupPoint(pickuppoint_data=parcel_data['pickUpPoint'], logger=self._log) \
             if 'pickUpPoint' in parcel_data else None
         self.multi_compartment: MultiCompartment | None = MultiCompartment(
             parcel_data['multiCompartment'], logger=self._log) if 'multiCompartment' in parcel_data else None
         self.is_end_off_week_collection: bool = parcel_data['endOfWeekCollection']
-        # self.operations: Operations = Operations(operations_data=parcel_data['operations'], logger=self._log)
         self.status: ParcelStatus = ParcelStatus[parcel_data['status']]
-        # self.event_log: List[EventLog] = [EventLog(eventlog_data=event, logger=self._log)
-        #                                   for event in parcel_data['eventLog']]
         self.avizo_transaction_status: str = parcel_data['avizoTransactionStatus']
         self.shared_to: List[SharedTo] = [SharedTo(sharedto_data=person, logger=self._log)
                                           for person in parcel_data['sharedTo']]
         self.ownership_status: ParcelOwnership = ParcelOwnership[parcel_data['ownershipStatus']]
         self._compartment_properties: CompartmentProperties | None = None
 
         self._log.debug(f'created parcel with shipment number {self.shipment_number}')
@@ -334,14 +327,15 @@
         self.point_type: str = pickuppoint_data['pointType']
         self.type: List[ParcelDeliveryType] = [ParcelDeliveryType[data] for data in pickuppoint_data['type']]
         self.location_round_the_clock: bool = pickuppoint_data['location247']
         self.doubled: bool = pickuppoint_data['doubled']
         self.image_url: str = pickuppoint_data['imageUrl']
         self.easy_access_zone: bool = pickuppoint_data['easyAccessZone']
         self.air_sensor: bool = pickuppoint_data['airSensor']
+        self.air_sensor_data: AirSensorData | None = AirSensorData(pickuppoint_data['airSensorData']) if 'airSensorData' in pickuppoint_data else None
 
         self._log: logging.Logger = logger.getChild(__class__.__name__)
         self._log.debug('created')
 
         if ParcelDeliveryType.UNKNOWN in self.type:
             self._log.debug(f'unknown delivery type: {pickuppoint_data["type"]}')
 
@@ -600,7 +594,29 @@
     def status(self, status_data: str | CompartmentActualStatus):
         self._log.debug('setting status')
         self._status = status_data if isinstance(status_data, CompartmentActualStatus) \
             else CompartmentActualStatus[status_data]
 
         if self._status == CompartmentActualStatus.UNKNOWN and isinstance(status_data, str):
             self._log.debug(f'unexpected compartment actual status: {status_data}')
+
+
+class AirSensorData:
+    """Object representation of :class:`Parcel` air sensor data
+
+    :param airsensor_data: :class:`dict` containing air sensor data for :class:`Parcel`
+    :type airsensor_data: dict
+    :param logger: :class:`logging.Logger` parent instance
+    :type logger: logging.Logger"""
+    def __init__(self, airsensor_data: dict, logger: logging.Logger):
+        self.updated_until: arrow = airsensor_data['updatedUntil']
+        self.air_quality: str = airsensor_data['airQuality']
+        self.temperature: float = airsensor_data['temperature']
+        self.humidity: float = airsensor_data['humidity']
+        self.pressure: float = airsensor_data['pressure']
+        self.pm25_value: float = airsensor_data['pollutants']['pm25']['value']
+        self.pm25_percent: float = airsensor_data['pollutants']['pm25']['percent']
+        self.pm10_value: float = airsensor_data['pollutants']['pm10']['value']
+        self.pm10_percent: float = airsensor_data['pollutants']['pm10']['percent']
+
+        self._log: logging.Logger = logger.getChild(__class__.__name__)
+        self._log.debug('created')
```

### Comparing `inpost-0.0.9/inpost/static/statuses.py` & `inpost-0.1.0/inpost/static/statuses.py`

 * *Files identical despite different names*

### Comparing `inpost-0.0.9/pyproject.toml` & `inpost-0.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "inpost"
-version = "0.0.9"
+version = "0.1.0"
 description = "Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app"
 authors = ["loboda4450 <loboda4450@gmail.com>", "MrKazik99 <mrkazik99@gmail.com>"]
 maintainers = ["loboda4450 <loboda4450@gmail.com>"]
 documentation = 'https://inpost-python.readthedocs.io/en/latest/index.html'
 repository = "https://github.com/IFOSSA/inpost-python"
 readme = "README.md"
 packages = [
         {include = 'inpost'},
         {include = 'inpost/static'}
     ]
 classifiers = [
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: aiohttp",
         "Intended Audience :: Developers",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
-        "Development Status :: 2 - Pre-Alpha"
+        "Development Status :: 3 - Alpha"
     ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.1"
 arrow = "^1.2.3"
 qrcode = "^7.3.1"
```

### Comparing `inpost-0.0.9/PKG-INFO` & `inpost-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,68 @@
 Metadata-Version: 2.1
 Name: inpost
-Version: 0.0.9
+Version: 0.1.0
 Summary: Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app
 Home-page: https://github.com/IFOSSA/inpost-python
 Author: loboda4450
 Author-email: loboda4450@gmail.com
 Maintainer: loboda4450
 Maintainer-email: loboda4450@gmail.com
 Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: aiohttp
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.4.0,<10.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: qrcode (>=7.3.1,<8.0.0)
 Project-URL: Documentation, https://inpost-python.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/IFOSSA/inpost-python
 Description-Content-Type: text/markdown
 
-Fully async Inpost API library
+
+# Inpost Python
+
+Fully async Inpost library using Python 3.10.
+
+
+
+
+## Documentation
+
+[Readthedocs.io](https://inpost-python.readthedocs.io/en/latest/)
+
+
+## Usage/Examples
+
+
+```python
+from inpost.api import Inpost
+
+inp = await Inpost.from_phone_number('555333444')
+await inp.send_sms_code():
+...
+if await inp.confirm_sms_code(123321):
+   print('Congratulations, you initialized successfully!')
+```
+
+
+## Authors
+
+- [@loboda4450](https://www.github.com/loboda4450)
+- [@mrkazik99](https://www.github.com/mrkazik99)
+
+
+## Used By
+
+This project is used by the following repos:
+
+[Inpost Telegram Bot](https://github.com/loboda4450/inpost-telegram-bot)
+
```

