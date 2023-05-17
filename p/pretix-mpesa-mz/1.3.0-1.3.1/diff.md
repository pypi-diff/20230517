# Comparing `tmp/pretix-mpesa-mz-1.3.0.tar.gz` & `tmp/pretix-mpesa-mz-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-mpesa-mz-1.3.0.tar", last modified: Fri May 12 16:03:57 2023, max compression
+gzip compressed data, was "pretix-mpesa-mz-1.3.1.tar", last modified: Wed May 17 15:08:12 2023, max compression
```

## Comparing `pretix-mpesa-mz-1.3.0.tar` & `pretix-mpesa-mz-1.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:57.154429 pretix-mpesa-mz-1.3.0/
--rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1844 2023-05-12 16:03:57.155430 pretix-mpesa-mz-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1549 2023-05-12 13:58:54.000000 pretix-mpesa-mz-1.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:56.974432 pretix-mpesa-mz-1.3.0/pretix_mpesa_mz.egg-info/
--rw-rw-rw-   0        0        0     1844 2023-05-12 16:03:56.000000 pretix-mpesa-mz-1.3.0/pretix_mpesa_mz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1156 2023-05-12 16:03:56.000000 pretix-mpesa-mz-1.3.0/pretix_mpesa_mz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 16:03:56.000000 pretix-mpesa-mz-1.3.0/pretix_mpesa_mz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-12 16:03:56.000000 pretix-mpesa-mz-1.3.0/pretix_mpesa_mz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-12 16:03:56.000000 pretix-mpesa-mz-1.3.0/pretix_mpesa_mz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:57.007427 pretix-mpesa-mz-1.3.0/pretix_mpesamz/
--rw-rw-rw-   0        0        0       23 2023-05-12 16:02:21.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/__init__.py
--rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:56.905431 pretix-mpesa-mz-1.3.0/pretix_mpesamz/locale/
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:56.903432 pretix-mpesa-mz-1.3.0/pretix_mpesamz/locale/de/
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:57.020431 pretix-mpesa-mz-1.3.0/pretix_mpesamz/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:57.027432 pretix-mpesa-mz-1.3.0/pretix_mpesamz/locale/de_Informal/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/locale/de_Informal/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:57.036427 pretix-mpesa-mz-1.3.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     8670 2023-05-12 14:15:41.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/mpesa_api.py
--rw-rw-rw-   0        0        0    14964 2023-05-12 16:01:52.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/payment.py
--rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/signals.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:56.911431 pretix-mpesa-mz-1.3.0/pretix_mpesamz/static/
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:57.044429 pretix-mpesa-mz-1.3.0/pretix_mpesamz/static/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:56.914431 pretix-mpesa-mz-1.3.0/pretix_mpesamz/templates/
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:57.137433 pretix-mpesa-mz-1.3.0/pretix_mpesamz/templates/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
--rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
--rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
--rw-rw-rw-   0        0        0      377 2023-05-11 17:08:48.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/templates/pretix_mpesamz/control.html
--rw-rw-rw-   0        0        0      225 2023-05-11 16:56:59.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/templates/pretix_mpesamz/order.html
--rw-rw-rw-   0        0        0      452 2023-05-11 14:57:44.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/templates/pretix_mpesamz/payment_pending.html
--rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
--rw-rw-rw-   0        0        0      295 2023-05-12 15:41:12.000000 pretix-mpesa-mz-1.3.0/pretix_mpesamz/templates/pretix_mpesamz/refund_control.html
--rw-rw-rw-   0        0        0      903 2023-05-12 16:03:57.161431 pretix-mpesa-mz-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-05-11 17:36:42.000000 pretix-mpesa-mz-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:03:57.146430 pretix-mpesa-mz-1.3.0/tests/
--rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.0/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.858750 pretix-mpesa-mz-1.3.1/
+-rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1844 2023-05-17 15:08:12.858750 pretix-mpesa-mz-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1549 2023-05-12 13:58:54.000000 pretix-mpesa-mz-1.3.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.632745 pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/
+-rw-rw-rw-   0        0        0     1844 2023-05-17 15:08:11.000000 pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1156 2023-05-17 15:08:12.000000 pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 15:08:11.000000 pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-17 15:08:11.000000 pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-05-17 15:08:11.000000 pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.697746 pretix-mpesa-mz-1.3.1/pretix_mpesamz/
+-rw-rw-rw-   0        0        0       23 2023-05-17 15:05:58.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.535745 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.531745 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de/
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.713746 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.722754 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de_Informal/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de_Informal/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.742749 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     8665 2023-05-17 14:50:26.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/mpesa_api.py
+-rw-rw-rw-   0        0        0    15276 2023-05-17 14:49:07.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/payment.py
+-rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/signals.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.545749 pretix-mpesa-mz-1.3.1/pretix_mpesamz/static/
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.747748 pretix-mpesa-mz-1.3.1/pretix_mpesamz/static/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.551747 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.827750 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
+-rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
+-rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
+-rw-rw-rw-   0        0        0      377 2023-05-11 17:08:48.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/control.html
+-rw-rw-rw-   0        0        0      225 2023-05-11 16:56:59.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/order.html
+-rw-rw-rw-   0        0        0      452 2023-05-11 14:57:44.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/payment_pending.html
+-rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
+-rw-rw-rw-   0        0        0      295 2023-05-12 15:41:12.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/refund_control.html
+-rw-rw-rw-   0        0        0      903 2023-05-17 15:08:12.864749 pretix-mpesa-mz-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-05-11 17:36:42.000000 pretix-mpesa-mz-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.842753 pretix-mpesa-mz-1.3.1/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/tests/test_main.py
```

### Comparing `pretix-mpesa-mz-1.3.0/LICENSE` & `pretix-mpesa-mz-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.0/PKG-INFO` & `pretix-mpesa-mz-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.3.0
+Version: 1.3.1
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
```

### Comparing `pretix-mpesa-mz-1.3.0/README.rst` & `pretix-mpesa-mz-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.0/pretix_mpesa_mz.egg-info/PKG-INFO` & `pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.3.0
+Version: 1.3.1
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
```

### Comparing `pretix-mpesa-mz-1.3.0/pretix_mpesa_mz.egg-info/SOURCES.txt` & `pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.0/pretix_mpesamz/apps.py` & `pretix-mpesa-mz-1.3.1/pretix_mpesamz/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.0/pretix_mpesamz/mpesa_api.py` & `pretix-mpesa-mz-1.3.1/pretix_mpesamz/mpesa_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 
 def execute_mpesa_c2b(config, payload):
     api_context = APIContext()
     api_context.api_key = config['api_key']
     api_context.public_key = config['public_key']
     api_context.ssl = True
     api_context.method_type = APIMethodType.POST
-    api_context.address = 'api.sandbox.vm.co.mz'
+    api_context.address = config['api_url']
     api_context.port = 18352
     api_context.path = '/ipg/v1x/c2bPayment/singleStage/'
 
     api_context.add_header('Origin', '*')
 
     api_context.add_parameter(
         'input_TransactionReference', payload['reference'])
```

### Comparing `pretix-mpesa-mz-1.3.0/pretix_mpesamz/payment.py` & `pretix-mpesa-mz-1.3.1/pretix_mpesamz/payment.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,19 @@
     @property
     def settings_form_fields(self):
         service_provider_code_field = forms.CharField(
             label=_('Código de Provedor de Serviço M-Pesa'),
             help_text=_('Identificador da entidade fornecido pelo M-Pesa')
         )
 
+        api_url_field = forms.CharField(
+            label=_('API URL'),
+            help_text=_('API URL fornecido pelo M-Pesa')
+        )
+
         api_key_field = forms.CharField(
             label=_('API Key'),
             help_text=_('API Key fornecido pelo M-Pesa')
         )
 
         public_key_field = forms.CharField(
             label=_('Public Key'),
@@ -83,14 +88,15 @@
             help_text=_(
                 'Shown to the user when viewing an order with completed payment.'),
             widget=I18nTextarea,
         )
 
         settingsList = [
             ('service_provider_code', service_provider_code_field),
+            ('api_url', api_url_field),
             ('api_key', api_key_field),
             ('public_key', public_key_field),
             ('information_text', info_field),
             ('payment_pending_text', pending_field),
             ('payment_completed_text', completed_field)
         ]
 
@@ -148,28 +154,29 @@
         return template.render(ctx)
 
     def execute_payment(self, request, payment):
         msisdn = request.session.get('payment_%s_msisdn' % self.identifier, '')
 
         try:
             config = {
+                'api_url': self.settings.get('api_url'),
                 'api_key': self.settings.get('api_key'),
                 'public_key': self.settings.get('public_key')
             }
 
             payment_data = {
                 'msisdn': "258" + str(msisdn),
-                'reference': 'TKT' + str(randint(0, 10000)),
+                'reference': payment.order.event.slug.replace('-', ''),
                 'third_party_reference': payment.order.code,
                 'amount': str(int(float(payment.amount))),
                 'service_provider_code': self.settings.get('service_provider_code')
             }
 
             result = execute_mpesa_c2b(config, payment_data)
-            # pprint(result)
+            pprint(result)
 
             if result['output_ResponseCode'] == 'INS-0':
                 success_payload = json.dumps({
                     'success': True,
                     'code': result['output_ResponseCode'],
                     'msisdn': msisdn,
                     'conversation': result['output_ConversationID'],
@@ -299,14 +306,15 @@
         return False
 
     def execute_refund(self, refund: OrderRefund):
         try:
             # pprint(vars(refund.payment))
             payment_info = json.loads(refund.payment.info)
             config = {
+                'api_url': self.settings.get('api_url'),
                 'api_key': self.settings.get('api_key'),
                 'public_key': self.settings.get('public_key')
             }
 
             payment_data = {
                 'transaction': payment_info['transaction'],
                 'third_party_reference': refund.order.code,
```

### Comparing `pretix-mpesa-mz-1.3.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html` & `pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.0/pretix_mpesamz/templates/pretix_mpesamz/redirect.html` & `pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/redirect.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.0/setup.cfg` & `pretix-mpesa-mz-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.0/setup.py` & `pretix-mpesa-mz-1.3.1/setup.py`

 * *Files identical despite different names*

