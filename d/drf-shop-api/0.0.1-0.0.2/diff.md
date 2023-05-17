# Comparing `tmp/drf_shop_api-0.0.1.tar.gz` & `tmp/drf_shop_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_shop_api-0.0.1.tar", max compression
+gzip compressed data, was "drf_shop_api-0.0.2.tar", max compression
```

## Comparing `drf_shop_api-0.0.1.tar` & `drf_shop_api-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0     2110 2023-05-08 07:44:18.468849 drf_shop_api-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-18 12:58:19.167199 drf_shop_api-0.0.1/drf_shop_api/__init__.py
--rw-r--r--   0        0        0     1695 2023-05-08 05:10:39.171976 drf_shop_api-0.0.1/drf_shop_api/abstract_models.py
--rw-r--r--   0        0        0     4311 2023-05-08 06:16:13.348913 drf_shop_api-0.0.1/drf_shop_api/admin.py
--rw-r--r--   0        0        0      151 2023-05-02 06:11:20.327034 drf_shop_api-0.0.1/drf_shop_api/apps.py
--rw-r--r--   0        0        0        0 2023-04-21 05:04:18.787953 drf_shop_api-0.0.1/drf_shop_api/customers/__init__.py
--rw-r--r--   0        0        0     1065 2023-05-02 06:09:39.859540 drf_shop_api-0.0.1/drf_shop_api/customers/filters.py
--rw-r--r--   0        0        0     1270 2023-05-02 08:18:38.014458 drf_shop_api-0.0.1/drf_shop_api/customers/models.py
--rw-r--r--   0        0        0     2326 2023-05-08 05:14:38.330078 drf_shop_api-0.0.1/drf_shop_api/customers/serializers.py
--rw-r--r--   0        0        0     8155 2023-05-02 08:46:22.747635 drf_shop_api-0.0.1/drf_shop_api/customers/tests.py
--rw-r--r--   0        0        0      475 2023-05-02 06:09:38.972303 drf_shop_api-0.0.1/drf_shop_api/customers/urls.py
--rw-r--r--   0        0        0     4706 2023-05-02 06:09:38.982956 drf_shop_api-0.0.1/drf_shop_api/customers/views.py
--rw-r--r--   0        0        0      402 2023-05-02 08:53:44.985101 drf_shop_api-0.0.1/drf_shop_api/decorators.py
--rw-r--r--   0        0        0    17700 2023-05-08 06:09:19.888504 drf_shop_api-0.0.1/drf_shop_api/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-18 12:58:19.170967 drf_shop_api-0.0.1/drf_shop_api/migrations/__init__.py
--rw-r--r--   0        0        0     1786 2023-05-08 07:43:30.570782 drf_shop_api-0.0.1/drf_shop_api/models.py
--rw-r--r--   0        0        0        0 2023-04-21 07:03:32.137480 drf_shop_api-0.0.1/drf_shop_api/orders/__init__.py
--rw-r--r--   0        0        0      328 2023-05-02 04:46:36.310896 drf_shop_api-0.0.1/drf_shop_api/orders/constants.py
--rw-r--r--   0        0        0        0 2023-05-02 05:45:04.690248 drf_shop_api-0.0.1/drf_shop_api/orders/filters.py
--rw-r--r--   0        0        0     1421 2023-05-08 05:27:34.535897 drf_shop_api-0.0.1/drf_shop_api/orders/models.py
--rw-r--r--   0        0        0     3645 2023-05-08 06:03:59.465591 drf_shop_api-0.0.1/drf_shop_api/orders/serializers.py
--rw-r--r--   0        0        0     3197 2023-05-08 05:26:36.572837 drf_shop_api-0.0.1/drf_shop_api/orders/tests.py
--rw-r--r--   0        0        0      236 2023-05-02 06:09:55.984725 drf_shop_api-0.0.1/drf_shop_api/orders/urls.py
--rw-r--r--   0        0        0     2171 2023-05-02 06:09:37.461581 drf_shop_api-0.0.1/drf_shop_api/orders/views.py
--rw-r--r--   0        0        0      692 2023-04-28 08:02:54.619717 drf_shop_api-0.0.1/drf_shop_api/paginators.py
--rw-r--r--   0        0        0     2271 2023-04-28 09:57:02.058215 drf_shop_api-0.0.1/drf_shop_api/permissions.py
--rw-r--r--   0        0        0        0 2023-04-19 12:14:02.155874 drf_shop_api-0.0.1/drf_shop_api/products/__init__.py
--rw-r--r--   0        0        0      208 2023-05-01 14:26:40.198927 drf_shop_api-0.0.1/drf_shop_api/products/constants.py
--rw-r--r--   0        0        0     1155 2023-05-02 06:09:55.334922 drf_shop_api-0.0.1/drf_shop_api/products/filters.py
--rw-r--r--   0        0        0     2495 2023-05-02 09:34:49.695511 drf_shop_api-0.0.1/drf_shop_api/products/models.py
--rw-r--r--   0        0        0     2580 2023-05-05 12:07:25.605250 drf_shop_api-0.0.1/drf_shop_api/products/serializers.py
--rw-r--r--   0        0        0     7877 2023-05-02 06:09:47.704951 drf_shop_api-0.0.1/drf_shop_api/products/tests.py
--rw-r--r--   0        0        0      435 2023-05-02 06:09:43.493734 drf_shop_api-0.0.1/drf_shop_api/products/urls.py
--rw-r--r--   0        0        0        0 2023-04-21 09:52:46.128283 drf_shop_api-0.0.1/drf_shop_api/products/utils.py
--rw-r--r--   0        0        0     3491 2023-05-02 06:09:28.026351 drf_shop_api-0.0.1/drf_shop_api/products/views.py
--rw-r--r--   0        0        0     2397 2023-05-08 05:14:56.407108 drf_shop_api-0.0.1/drf_shop_api/serializers.py
--rw-r--r--   0        0        0        0 2023-04-19 12:27:36.021705 drf_shop_api-0.0.1/drf_shop_api/tasks.py
--rw-r--r--   0        0        0     1055 2023-05-02 08:30:25.003346 drf_shop_api-0.0.1/drf_shop_api/tests.py
--rw-r--r--   0        0        0      305 2023-05-02 06:12:22.345106 drf_shop_api-0.0.1/drf_shop_api/urls.py
--rw-r--r--   0        0        0     5326 2023-05-08 07:18:04.625784 drf_shop_api-0.0.1/drf_shop_api/utils.py
--rw-r--r--   0        0        0       27 2023-04-19 12:27:10.142562 drf_shop_api-0.0.1/drf_shop_api/views.py
--rw-r--r--   0        0        0      598 2023-05-08 07:46:44.952090 drf_shop_api-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 drf_shop_api-0.0.1/setup.py
--rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 drf_shop_api-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3060 2023-05-16 08:05:31.955824 drf_shop_api-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 12:58:19.167199 drf_shop_api-0.0.2/drf_shop_api/__init__.py
+-rw-r--r--   0        0        0     2003 2023-05-16 07:14:02.635612 drf_shop_api-0.0.2/drf_shop_api/abstract_models.py
+-rw-r--r--   0        0        0     4476 2023-05-17 13:30:50.707985 drf_shop_api-0.0.2/drf_shop_api/admin.py
+-rw-r--r--   0        0        0      151 2023-05-02 06:11:20.327034 drf_shop_api-0.0.2/drf_shop_api/apps.py
+-rw-r--r--   0        0        0        0 2023-04-21 05:04:18.787953 drf_shop_api-0.0.2/drf_shop_api/customers/__init__.py
+-rw-r--r--   0        0        0     1065 2023-05-02 06:09:39.859540 drf_shop_api-0.0.2/drf_shop_api/customers/filters.py
+-rw-r--r--   0        0        0     1919 2023-05-17 13:31:21.619254 drf_shop_api-0.0.2/drf_shop_api/customers/models.py
+-rw-r--r--   0        0        0     4586 2023-05-17 13:32:46.291563 drf_shop_api-0.0.2/drf_shop_api/customers/serializers.py
+-rw-r--r--   0        0        0    11443 2023-05-17 13:29:55.510681 drf_shop_api-0.0.2/drf_shop_api/customers/tests.py
+-rw-r--r--   0        0        0      742 2023-05-17 13:23:30.248336 drf_shop_api-0.0.2/drf_shop_api/customers/urls.py
+-rw-r--r--   0        0        0     6595 2023-05-17 13:21:18.774078 drf_shop_api-0.0.2/drf_shop_api/customers/views.py
+-rw-r--r--   0        0        0      537 2023-05-16 05:52:21.374090 drf_shop_api-0.0.2/drf_shop_api/decorators.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:43:27.864812 drf_shop_api-0.0.2/drf_shop_api/migrations/.gitignore
+-rw-r--r--   0        0        0        0 2023-04-18 12:58:19.170967 drf_shop_api-0.0.2/drf_shop_api/migrations/__init__.py
+-rw-r--r--   0        0        0     1800 2023-05-16 11:42:24.294850 drf_shop_api-0.0.2/drf_shop_api/models.py
+-rw-r--r--   0        0        0        0 2023-04-21 07:03:32.137480 drf_shop_api-0.0.2/drf_shop_api/orders/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-16 08:12:07.125840 drf_shop_api-0.0.2/drf_shop_api/orders/constants.py
+-rw-r--r--   0        0        0        0 2023-05-02 05:45:04.690248 drf_shop_api-0.0.2/drf_shop_api/orders/filters.py
+-rw-r--r--   0        0        0     2119 2023-05-16 11:44:39.145565 drf_shop_api-0.0.2/drf_shop_api/orders/models.py
+-rw-r--r--   0        0        0     4212 2023-05-16 13:22:57.000875 drf_shop_api-0.0.2/drf_shop_api/orders/serializers.py
+-rw-r--r--   0        0        0     3365 2023-05-16 09:33:08.141979 drf_shop_api-0.0.2/drf_shop_api/orders/tests.py
+-rw-r--r--   0        0        0      236 2023-05-02 06:09:55.984725 drf_shop_api-0.0.2/drf_shop_api/orders/urls.py
+-rw-r--r--   0        0        0      142 2023-05-16 09:41:43.338239 drf_shop_api-0.0.2/drf_shop_api/orders/utils.py
+-rw-r--r--   0        0        0     2227 2023-05-16 12:44:19.399851 drf_shop_api-0.0.2/drf_shop_api/orders/views.py
+-rw-r--r--   0        0        0      692 2023-04-28 08:02:54.619717 drf_shop_api-0.0.2/drf_shop_api/paginators.py
+-rw-r--r--   0        0        0     2271 2023-04-28 09:57:02.058215 drf_shop_api-0.0.2/drf_shop_api/permissions.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:14:02.155874 drf_shop_api-0.0.2/drf_shop_api/products/__init__.py
+-rw-r--r--   0        0        0      208 2023-05-01 14:26:40.198927 drf_shop_api-0.0.2/drf_shop_api/products/constants.py
+-rw-r--r--   0        0        0     1155 2023-05-02 06:09:55.334922 drf_shop_api-0.0.2/drf_shop_api/products/filters.py
+-rw-r--r--   0        0        0     2839 2023-05-16 11:55:54.791725 drf_shop_api-0.0.2/drf_shop_api/products/models.py
+-rw-r--r--   0        0        0     2637 2023-05-17 11:45:51.736626 drf_shop_api-0.0.2/drf_shop_api/products/serializers.py
+-rw-r--r--   0        0        0     7877 2023-05-16 11:59:24.701138 drf_shop_api-0.0.2/drf_shop_api/products/tests.py
+-rw-r--r--   0        0        0      435 2023-05-16 05:40:10.692883 drf_shop_api-0.0.2/drf_shop_api/products/urls.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:52:46.128283 drf_shop_api-0.0.2/drf_shop_api/products/utils.py
+-rw-r--r--   0        0        0     3491 2023-05-02 06:09:28.026351 drf_shop_api-0.0.2/drf_shop_api/products/views.py
+-rw-r--r--   0        0        0     2397 2023-05-08 05:14:56.407108 drf_shop_api-0.0.2/drf_shop_api/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:27:36.021705 drf_shop_api-0.0.2/drf_shop_api/tasks.py
+-rw-r--r--   0        0        0     1055 2023-05-02 08:30:25.003346 drf_shop_api-0.0.2/drf_shop_api/tests.py
+-rw-r--r--   0        0        0      305 2023-05-02 06:12:22.345106 drf_shop_api-0.0.2/drf_shop_api/urls.py
+-rw-r--r--   0        0        0     3629 2023-05-17 13:12:43.981890 drf_shop_api-0.0.2/drf_shop_api/utils.py
+-rw-r--r--   0        0        0       27 2023-04-19 12:27:10.142562 drf_shop_api-0.0.2/drf_shop_api/views.py
+-rw-r--r--   0        0        0      598 2023-05-17 13:44:55.819900 drf_shop_api-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 drf_shop_api-0.0.2/setup.py
+-rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 drf_shop_api-0.0.2/PKG-INFO
```

### Comparing `drf_shop_api-0.0.1/README.md` & `drf_shop_api-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # Features
 
 Features:
 
+- products (multiple images + main image, title, description, etc.)
+- products categories (parent/child categories)
+- product dynamic stats (for filtering like on Rozetka, ek.ua)
+- product comments
+- wish lists
+- cart
+- compare lists
+- orders
+- order reports (+ ability to generate pdf)
+- history
+- contact online support via web-sockets (or offline via email)
+- connect implemented payment systems
+- shipment
+- taxes
+- bonuses wallet
+- search for products/categories
+- filter for products in the category
+- statuses of buy / payment / shipment
+
+Features:
+
 - Products
   - products (multiple images + main image, title, description, etc.)
   - products categories (parent/child categories)
   - product dynamic stats (for filtering like on Rozetka, ek.ua)
   - product comments
   - search for products/categories
   - filter for products in the category
@@ -19,41 +40,42 @@
   - currencies
 - Orders
   - orders
   - order reports (view and generation of pdf)
   - shipping
   - statuses of order / payment / shipment
 
-## Customers
+## Installation
 
-This app will hold User related data:
+- Install library
 
-`CustomerCart`
-`CustomerWishList`
-`CustomerBonusWallet`
-`CustomerOrderHistory`
+```bash
+pip install drf-shop-api
+```
 
-## Settings requirements
+- Add to installed apps
 
-- DRF settings
+  ```python
 
-```json
-"DEFAULT_AUTHENTICATION_CLASSES": ("rest_framework_simplejwt.authentication.JWTAuthentication",)
-```
+  INSTALLED_APPS = [
+    ...
+    'drf_shop_api'
+  ]
+  ```
 
-- DRF_SHOP settings:
-  - DRF_SHOP_PAGE_SIZE on will be default 10
-  - DRF_SHOP_PAYMENT_MODEL = "projects.payments.models.Payment"
-  - DRF_SHOP_PAYMENT_STATUS_CHOICES = "project.payments.choices.PaymentStatus"
-  - DRF_SHOP_BONUS_RATE = percentage value for each order that will go to bonus wallet (e.g. 10)
+- Add api path to you root urls.py
 
-> Statuses should be aligned as regular flow then cancel followed by refund
+```python
+   urlpatterns = [
+    ...
+    path("shop/", include("drf_shop_api.urls")),
+]
+```
 
-Modify user management:
-For creation of related models please use create_shop_profile decorator on you UserManager class
+- Use `create_shop_profile` decorator on create_user method of your UserManager
 
 ```python
 from django.contrib.auth.base_user import BaseUserManager
 
 from drf_shop_api.decorators import create_shop_profile
 
 
@@ -62,17 +84,47 @@
     def create_user(self, email, password=None):
         if not email:
             raise ValueError("Enter the email")
         user = self.model(email=self.normalize_email(email))
         user.set_password(password)
         user.save(using=self._db)
         return user
+```
+
+- Setup `AUTH_USER_MODEL` in settings.py
 
+- Run `python manage.py makemigrations` and `python manage.py migrate` (Due to optional Payment model from root project)
+
+## Features overview
+
+### Customers
+
+This app will hold User related data:
+
+`CustomerCart`
+`CustomerWishList`
+`CustomerBonusWallet`
+`CustomerOrderHistory`
+
+## Settings requirements
+
+- DRF settings
+
+```json
+"DEFAULT_AUTHENTICATION_CLASSES": ("rest_framework_simplejwt.authentication.JWTAuthentication",)
 ```
 
+- DRF_SHOP settings:
+  - DRF_SHOP_PAGE_SIZE on will be default 10
+  - DRF_SHOP_PAYMENT_MODEL = "projects.payments.models.Payment"
+  - DRF_SHOP_PAYMENT_STATUS_CHOICES = "project.payments.choices.PaymentStatus"
+  - DRF_SHOP_BONUS_RATE = percentage value for each order that will go to bonus wallet
+
+> Statuses should be aligned as regular flow then cancel followed by refund
+
 ## Dependencies
 
     django
     drf
     drf-yasg 1.21.5
     rest_framework_simplejwt
     mixer
@@ -80,8 +132,7 @@
 
 ### TODO
 
 - Add DB indexes
 - Task for currency rate update
 - Review permissions
 - Add custom migration to create all related model for auth user model
-- Integrate payment from external project
```

### Comparing `drf_shop_api-0.0.1/drf_shop_api/abstract_models.py` & `drf_shop_api-0.0.2/drf_shop_api/abstract_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -76,7 +76,17 @@
     ``user.customerwishlist``
     """
 
     user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, related_name="%(class)s")
 
     class Meta:
         abstract = True
+
+
+class AbstractPayment(OwnershipMultipleModel):
+    total_price = models.FloatField(null=True, blank=True)
+    is_refundable = models.BooleanField(default=True)
+    created = models.DateTimeField(auto_now_add=True)
+    modified = models.DateTimeField(auto_now=True)
+
+    class Meta:
+        abstract = True
```

### Comparing `drf_shop_api-0.0.1/drf_shop_api/admin.py` & `drf_shop_api-0.0.2/drf_shop_api/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from django.contrib import admin
 
+from drf_shop_api.customers.models import CustomerSupportRequest
+from drf_shop_api.orders.models import OrderPayment
+
 from .models import (
     Currency,
     CurrencyRate,
     CustomerBonusWallet,
     CustomerCart,
     CustomerCartProduct,
     CustomerWishList,
@@ -17,14 +20,27 @@
     ProductProperty,
     Property,
     ShippingMethod,
     Tax,
 )
 
 
+@admin.register(CustomerSupportRequest)
+class CustomerSupportRequestAdmin(admin.ModelAdmin):
+    list_display = (
+        "id",
+        "created_at",
+        "updated_at",
+    )
+    list_filter = (
+        "created_at",
+        "updated_at",
+    )
+
+
 @admin.register(ProductCategory)
 class ProductCategoryAdmin(admin.ModelAdmin):
     list_display = (
         "id",
         "description",
         "title",
         "created_at",
@@ -33,14 +49,29 @@
         "parent",
         "is_active",
     )
     list_filter = ("created_at", "updated_at", "parent", "is_active")
     date_hierarchy = "created_at"
 
 
+class ProductImageInline(admin.TabularInline):
+    model = ProductImage
+    extra = 3
+
+
+class ProductPropertyInline(admin.TabularInline):
+    model = ProductProperty
+    extra = 1
+
+
+class ProductCommentInline(admin.TabularInline):
+    model = ProductComment
+    extra = 1
+
+
 @admin.register(Product)
 class ProductAdmin(admin.ModelAdmin):
     list_display = (
         "id",
         "description",
         "title",
         "created_at",
@@ -53,40 +84,27 @@
     list_filter = (
         "created_at",
         "updated_at",
         "currency",
         "category",
         "is_active",
     )
+    inlines = (
+        ProductImageInline,
+        ProductPropertyInline,
+        ProductCommentInline,
+    )
     date_hierarchy = "created_at"
 
 
-@admin.register(ProductImage)
-class ProductImageAdmin(admin.ModelAdmin):
-    list_display = ("id", "product", "image", "is_main")
-    list_filter = ("product", "is_main")
-
-
 @admin.register(Property)
 class PropertyAdmin(admin.ModelAdmin):
     list_display = ("id", "description", "title", "unit")
 
 
-@admin.register(ProductProperty)
-class ProductPropertyAdmin(admin.ModelAdmin):
-    list_display = ("id", "product", "property", "value")
-    list_filter = ("product", "property")
-
-
-@admin.register(ProductComment)
-class ProductCommentAdmin(admin.ModelAdmin):
-    list_display = ("id", "user", "product", "content")
-    list_filter = ("user", "product")
-
-
 @admin.register(CustomerBonusWallet)
 class CustomerBonusWalletAdmin(admin.ModelAdmin):
     list_display = ("id", "user", "amount")
     list_filter = ("user",)
 
 
 @admin.register(CustomerWishList)
@@ -100,46 +118,52 @@
         "user",
     )
     list_filter = ("created_at", "updated_at", "user")
     raw_id_fields = ("products",)
     date_hierarchy = "created_at"
 
 
+class CustomerCartProductInline(admin.TabularInline):
+    model = CustomerCartProduct
+
+
 @admin.register(CustomerCart)
 class CustomerCartAdmin(admin.ModelAdmin):
     list_display = ("id", "created_at", "updated_at", "user")
+    inlines = [
+        CustomerCartProductInline,
+    ]
     list_filter = ("created_at", "updated_at", "user")
     date_hierarchy = "created_at"
 
 
-@admin.register(CustomerCartProduct)
-class CustomerCartProductAdmin(admin.ModelAdmin):
-    list_display = ("id", "cart", "product", "quantity")
-    list_filter = ("cart", "product")
+class OrderShippingInline(admin.TabularInline):
+    model = OrderShipping
+
+
+class OrderProductInline(admin.TabularInline):
+    model = OrderProduct
+
+
+class OrderPaymentInline(admin.TabularInline):
+    model = OrderPayment
 
 
 @admin.register(Order)
 class OrderAdmin(admin.ModelAdmin):
     list_display = ("id", "created_at", "updated_at", "user", "status")
     list_filter = ("created_at", "updated_at", "user")
+    inlines = [
+        OrderShippingInline,
+        OrderProductInline,
+        OrderPaymentInline,
+    ]
     date_hierarchy = "created_at"
 
 
-@admin.register(OrderShipping)
-class OrderShippingAdmin(admin.ModelAdmin):
-    list_display = ("id", "order", "method", "address", "status")
-    list_filter = ("order", "method")
-
-
-@admin.register(OrderProduct)
-class OrderProductAdmin(admin.ModelAdmin):
-    list_display = ("id", "order", "product", "quantity")
-    list_filter = ("order", "product")
-
-
 @admin.register(Currency)
 class CurrencyAdmin(admin.ModelAdmin):
     list_display = (
         "id",
         "description",
         "title",
         "dlm",
```

### Comparing `drf_shop_api-0.0.1/drf_shop_api/customers/filters.py` & `drf_shop_api-0.0.2/drf_shop_api/customers/filters.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.1/drf_shop_api/customers/serializers.py` & `drf_shop_api-0.0.2/drf_shop_api/products/serializers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,89 @@
-from django.db import transaction
 from rest_framework import serializers
 
-from drf_shop_api.customers.models import CustomerBonusWallet, CustomerCart, CustomerCartProduct, CustomerWishList
-from drf_shop_api.products.models import Product
-from drf_shop_api.products.serializers import ProductSerializer
-from drf_shop_api.utils import update_related_objects
+from drf_shop_api.products.models import (
+    Product,
+    ProductCategory,
+    ProductComment,
+    ProductImage,
+    ProductProperty,
+    Property,
+)
+from drf_shop_api.serializers import BaseCurrencySerializer
 
 
-class BaseCustomerBonusWalletSerializer(serializers.ModelSerializer):
+class BaseProductCommentSerializer(serializers.ModelSerializer):
     class Meta:
-        model = CustomerBonusWallet
-        fields = ("id", "user", "amount")
+        model = ProductComment
+        fields = ("id",)
 
 
-# TODO: Add expanded serializer based on user profile serializer from parent project
-class BaseCustomerWishListSerializer(serializers.ModelSerializer):
+class ProductCommentSerializer(BaseProductCommentSerializer):
+    user = serializers.HiddenField(default=serializers.CurrentUserDefault())
+    product = serializers.PrimaryKeyRelatedField(queryset=Product.objects.all())
+
+    class Meta(BaseProductCommentSerializer.Meta):
+        fields = (*BaseProductCommentSerializer.Meta.fields, "product", "content", "user")
+
+
+class ProductImageSerializer(serializers.ModelSerializer):
     class Meta:
-        model = CustomerWishList
-        fields = ("id", "user", "products")
+        model = ProductImage
+        fields = (
+            "id",
+            "image",
+            "is_main",
+        )
 
 
-class CustomerWishListSerializer(BaseCustomerWishListSerializer):
-    id = serializers.IntegerField(required=False)
-    products = ProductSerializer(many=True)
+class BasePropertySerializer(serializers.ModelSerializer):
+    class Meta:
+        model = Property
+        fields = (
+            "id",
+            "title",
+        )
+
 
-    @transaction.atomic
-    def update(self, instance: CustomerWishList, validated_data: dict) -> CustomerWishList:
-        products = validated_data.pop("products", [])
-        wish_list = super().update(instance, validated_data)
-        product_list = [Product.objects.get(id=product["id"]) for product in products]
-        wish_list.products.set(product_list)
-        return super().update(instance, validated_data)
+class PropertySerializer(BasePropertySerializer):
+    class Meta(BasePropertySerializer.Meta):
+        fields = (*BasePropertySerializer.Meta.fields, "unit", "description")
 
 
-class CustomerCartProductSerializer(serializers.ModelSerializer):
+class ProductPropertySerializer(serializers.ModelSerializer):
+    property = PropertySerializer(many=False)
+
+    class Meta:
+        model = ProductProperty
+        fields = ("property", "value")
+
+
+class BaseProductCategorySerializer(serializers.ModelSerializer):
     id = serializers.IntegerField(required=False)
-    product = ProductSerializer(read_only=True)
 
     class Meta:
-        model = CustomerCartProduct
-        fields = ("id", "product", "quantity")
+        model = ProductCategory
+        fields = ("id", "title", "url")
 
 
-class BaseCustomerCartSerializer(serializers.ModelSerializer):
-    products = CustomerCartProductSerializer(many=True)
+class BaseProductSerializer(serializers.ModelSerializer):
+    id = serializers.IntegerField(required=False)
+    main_image = serializers.SerializerMethodField()
+    category = BaseProductCategorySerializer(many=False, read_only=True)
+    comments = BaseProductCommentSerializer(many=True)
+    currency = BaseCurrencySerializer(many=False)
 
     class Meta:
-        model = CustomerCart
-        fields = ("id", "user", "products")
+        model = Product
+        fields = ("id", "price", "title", "description", "comments", "main_image", "currency", "category")
+
+    def get_main_image(self, obj):
+        return ProductImageSerializer(obj.images.filter(is_main=True).first()).data
 
 
-class CustomerCartSerializer(BaseCustomerCartSerializer):
-    products = CustomerCartProductSerializer(many=True)
+class ProductSerializer(BaseProductSerializer):
+    images = ProductImageSerializer(many=True)
+    properties = ProductPropertySerializer(many=True)
+    comments = ProductCommentSerializer(many=True)
 
-    @transaction.atomic
-    def update(self, instance: CustomerCart, validated_data: dict) -> CustomerCart:
-        products = validated_data.pop("products", None)
-        cart = super().update(instance, validated_data)
-        if products is not None:
-            update_related_objects(self, "cart", cart, "products", products, CustomerCartProductSerializer)
-        return cart
+    class Meta(BaseProductSerializer.Meta):
+        fields = (*BaseProductSerializer.Meta.fields, "images", "properties")
```

### Comparing `drf_shop_api-0.0.1/drf_shop_api/customers/tests.py` & `drf_shop_api-0.0.2/drf_shop_api/customers/tests.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from django.apps import apps
 from django.conf import settings
 from django.urls import reverse
 from mixer.backend.django import mixer
 
-from drf_shop_api.customers.models import CustomerBonusWallet, CustomerCart, CustomerCartProduct, CustomerWishList
+from drf_shop_api.customers.models import (
+    CustomerBonusWallet,
+    CustomerCart,
+    CustomerCartProduct,
+    CustomerComparisonList,
+    CustomerSupportRequest,
+    CustomerWishList,
+)
 from drf_shop_api.customers.serializers import (
     BaseCustomerBonusWalletSerializer,
     BaseCustomerWishListSerializer,
     CustomerCartSerializer,
     CustomerWishListSerializer,
 )
 from drf_shop_api.products.models import Product
@@ -163,13 +170,92 @@
         self.target.refresh_from_db()
         self.assertEqual(resp.status_code, 200)
         self.assertEqual(resp.data["user"], self.target.user.id)
         self.assertEqual(resp.data["products"][0]["id"], product.id)
         self.assertEqual(resp.data["products"][0]["quantity"], quantity)
 
 
+class TestCustomerComparisonList(BaseAPITest):
+    def setUp(self):
+        self.admin = self.create_and_login(email="admin@example.com", is_staff=True, is_superuser=True)
+        self.list_count: int = 10
+        self.list_url: str = reverse("customers:comparisons-list")
+        user_list = mixer.cycle(self.list_count).blend(
+            apps.get_model(f"{settings.AUTH_USER_MODEL}"),
+            is_active=True,
+        )
+        product_list = []
+        for i in range(self.list_count):
+            product_list.append(mixer.blend(Product, price=(i + 1) * 10))
+        for i, user in zip(range(self.list_count), user_list):
+            _ = mixer.blend(CustomerComparisonList, user=user, products=product_list[i])
+        self.target = CustomerComparisonList.objects.first()
+
+    def test_list_admin(self):
+        resp = self.client.get(self.list_url)
+        self.assertEqual(resp.status_code, 200)
+        self.assertEqual(resp.data["count"], self.list_count)
+
+    def test_list_admin_custom_page_size(self):
+        qty = 5
+        resp = self.client.get(f"{self.list_url}?page_size={qty}")
+        self.assertEqual(resp.status_code, 200)
+        self.assertEqual(len(resp.data["results"]), qty)
+
+    def test_list_admin_custom_page_size_and_page(self):
+        qty = 6
+        page_count = self.list_count - qty
+        resp = self.client.get(f"{self.list_url}?page=2&page_size={qty}")
+        self.assertEqual(resp.status_code, 200)
+        self.assertEqual(len(resp.data["results"]), page_count)
+
+    def test_detail_admin(self):
+        resp = self.client.get(f"{self.list_url}{self.target.id}/")
+        self.assertEqual(resp.status_code, 200)
+
+    def test_create_comparison(self):
+        product = Product.objects.first()
+        data = {
+            "products": [ProductSerializer(product).data],
+        }
+        self.authorize(self.target.user)
+        resp = self.client.post(f"{self.list_url}", data)
+        self.assertEqual(resp.status_code, 201)
+
+
+class TestCustomerSupportRequest(BaseAPITest):
+    def setUp(self):
+        self.request_count: int = 10
+        self.list_url: str = reverse("customers:support-request-list")
+        user_list = mixer.cycle(self.request_count).blend(
+            apps.get_model(f"{settings.AUTH_USER_MODEL}"),
+            is_active=True,
+        )
+        product_list = []
+        for i in range(self.request_count):
+            product_list.append(mixer.blend(Product, price=(i + 1) * 10))
+        for i, user in zip(range(self.request_count), user_list):
+            _ = mixer.blend(CustomerSupportRequest, user=user, product=product_list[i])
+        self.target = CustomerSupportRequest.objects.first()
+
+    def test_list_as_admin(self):
+        self.create_and_login(email="admin@example.com", is_staff=True, is_superuser=True)
+        resp = self.client.get(self.list_url)
+        self.assertEqual(resp.status_code, 200)
+
+    def test_list_as_owner(self):
+        self.authorize(self.target.user)
+        resp = self.client.get(self.list_url)
+        self.assertEqual(resp.status_code, 200)
+
+    def test_list_as_non_auth(self):
+        self.logout()
+        resp = self.client.get(self.list_url)
+        self.assertEqual(resp.status_code, 401)
+
+
 class CustomUserManager(BaseAPITest):
     def test_customer_manager(self):
         user = self.create(email="admin@example.com")
         self.assertEqual(CustomerBonusWallet.objects.first().user.id, user.id)
         self.assertEqual(CustomerCart.objects.first().user.id, user.id)
         self.assertEqual(CustomerWishList.objects.first().user.id, user.id)
```

### Comparing `drf_shop_api-0.0.1/drf_shop_api/customers/views.py` & `drf_shop_api-0.0.2/drf_shop_api/customers/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 from django_filters.rest_framework import DjangoFilterBackend
 from rest_framework import mixins, viewsets
 
 from drf_shop_api.customers.filters import CustomerBonusWalletFilter, CustomerCartFilter, CustomerWishListFilter
-from drf_shop_api.customers.models import CustomerBonusWallet, CustomerCart, CustomerWishList
+from drf_shop_api.customers.models import (
+    CustomerBonusWallet,
+    CustomerCart,
+    CustomerComparisonList,
+    CustomerSupportRequest,
+    CustomerWishList,
+)
 from drf_shop_api.customers.serializers import (
     BaseCustomerBonusWalletSerializer,
     BaseCustomerCartSerializer,
+    BaseCustomerComparisonListSerializer,
+    BaseCustomerSupportRequestSerializer,
     BaseCustomerWishListSerializer,
     CustomerCartSerializer,
+    CustomerComparisonListSerializer,
+    CustomerSupportRequestSerializer,
     CustomerWishListSerializer,
 )
 from drf_shop_api.paginators import OwnershipPaginator
 from drf_shop_api.permissions import GetByAuthOrAdminEditByAdmin
 from drf_shop_api.serializers import ListSerializerMixin
 from drf_shop_api.utils import qs_admin_or_author
 
@@ -154,7 +164,71 @@
     list_serializer_class = BaseCustomerCartSerializer
     pagination_class = OwnershipPaginator
     filter_backends = (DjangoFilterBackend,)
     filterset_class = CustomerCartFilter
 
     def get_queryset(self):
         return qs_admin_or_author(self, CustomerCart.objects.all())
+
+
+class CustomerComparisonListViewSet(
+    ListSerializerMixin,
+    mixins.CreateModelMixin,
+    mixins.ListModelMixin,
+    mixins.RetrieveModelMixin,
+    mixins.UpdateModelMixin,
+    viewsets.GenericViewSet,
+):
+    """
+    create:
+    Create Comparison list
+
+    As authenticated user you can create comparison list
+
+    ```
+    ```
+
+    list:
+    All comparison lists.
+
+    In case of admin user list all comparison lists
+    In case of regular user return only his comparison lists
+
+    retrieve:
+    Details of single comparison list
+
+    As admin retrieve comparison list details by `id`
+
+
+
+    partial_update:
+    Update comparison list
+
+    As owner you can update your comparison list
+    """
+
+    permission_classes = (GetByAuthOrAdminEditByAdmin,)
+    serializer_class = CustomerComparisonListSerializer
+    list_serializer_class = BaseCustomerComparisonListSerializer
+    pagination_class = OwnershipPaginator
+    filter_backends = (DjangoFilterBackend,)
+
+    def get_queryset(self):
+        return qs_admin_or_author(self, CustomerComparisonList.objects.all())
+
+
+class CustomerSupportRequestViewSet(
+    ListSerializerMixin,
+    mixins.CreateModelMixin,
+    mixins.ListModelMixin,
+    mixins.RetrieveModelMixin,
+    mixins.UpdateModelMixin,
+    viewsets.GenericViewSet,
+):
+    permission_classes = (GetByAuthOrAdminEditByAdmin,)
+    serializer_class = CustomerSupportRequestSerializer
+    list_serializer_class = BaseCustomerSupportRequestSerializer
+    pagination_class = OwnershipPaginator
+    filter_backends = (DjangoFilterBackend,)
+
+    def get_queryset(self):
+        return qs_admin_or_author(self, CustomerSupportRequest.objects.all())
```

### Comparing `drf_shop_api-0.0.1/drf_shop_api/models.py` & `drf_shop_api-0.0.2/drf_shop_api/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     class Meta:
         db_table = "taxes"
         verbose_name_plural = "taxes"
         ordering = ("-id",)
 
     def __str__(self):
-        return f"{self.value}"
+        return f"{self.value}%:{self.title}"
 
 
 class ShippingMethod(TitleDescriptionModel):
     logo = models.ImageField(upload_to="shipping-methods", blank=True, null=True)
 
     class Meta:
         db_table = "shipping-methods"
```

### Comparing `drf_shop_api-0.0.1/drf_shop_api/orders/models.py` & `drf_shop_api-0.0.2/drf_shop_api/orders/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+from django.conf import settings
+from django.core.validators import MinValueValidator
 from django.db import models
 
 from drf_shop_api.abstract_models import OwnershipMultipleModel, TimeStampedModel
-from drf_shop_api.orders.constants import OrderStatus, ShipmentStatus
+from drf_shop_api.orders.constants import OrderStatus, PaymentStatus, ShipmentStatus
 from drf_shop_api.products.models import Product
 
 
 class Order(TimeStampedModel, OwnershipMultipleModel):
     status = models.CharField(
         max_length=255,
         choices=[(v.name, v.value) for v in OrderStatus],
         null=True,
         blank=True,
         default=OrderStatus.CREATED.name,
     )
+    total = models.DecimalField(max_digits=6, default=0, decimal_places=2, validators=[MinValueValidator(0)])
 
     class Meta:
         db_table = "orders"
         ordering = ("-id",)
 
 
 class OrderShipping(models.Model):
@@ -32,14 +35,28 @@
     )
 
     class Meta:
         db_table = "order-shippings"
         ordering = ("-id",)
 
 
+class OrderPayment(models.Model):
+    order = models.OneToOneField(Order, models.CASCADE, related_name="payment")
+    if settings.DRF_SHOP_PAYMENT_MODEL:
+        payment = models.ForeignKey(settings.DRF_SHOP_PAYMENT_MODEL, models.CASCADE)
+    else:
+        status = models.CharField(
+            max_length=255,
+            choices=[(v.name, v.value) for v in PaymentStatus],
+            null=True,
+            blank=True,
+            default=PaymentStatus.UNCOMPLETED.name,
+        )
+
+
 class OrderProduct(models.Model):
     order = models.ForeignKey(Order, models.CASCADE, related_name="products")
     product = models.ForeignKey(Product, models.CASCADE, related_name="order_products")
     quantity = models.IntegerField(default=1)
 
     class Meta:
         db_table = "order-products"
```

### Comparing `drf_shop_api-0.0.1/drf_shop_api/orders/serializers.py` & `drf_shop_api-0.0.2/drf_shop_api/orders/serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.db import transaction
 from rest_framework import serializers
 
 from drf_shop_api.models import ShippingMethod
 from drf_shop_api.orders.models import Order, OrderProduct, OrderShipping
+from drf_shop_api.orders.utils import total_products_price
 from drf_shop_api.products.models import Product
 from drf_shop_api.products.serializers import ProductSerializer
 from drf_shop_api.serializers import BaseShippingMethodSerializer
 from drf_shop_api.utils import nested_write, update_related_objects
 
 
 class BaseOrderShippingSerializer(serializers.ModelSerializer):
@@ -44,15 +45,16 @@
         validated_data = nested_write(validated_data, "product", Product)
         return super().update(instance, validated_data)
 
 
 class BaseOrderSerializer(serializers.ModelSerializer):
     class Meta:
         model = Order
-        fields = ("id", "user", "products", "shipping")
+        fields = ("id", "user", "products", "shipping", "total")
+        read_only_fields = ("user",)
 
 
 class OrderSerializer(BaseOrderSerializer):
     user = serializers.HiddenField(default=serializers.CurrentUserDefault())
     products = OrderProductSerializer(many=True)
     shipping = BaseOrderShippingSerializer(required=True)
 
@@ -63,14 +65,17 @@
         order_shipping = validated_data.pop("shipping", None)
         order_shipping_serializer = BaseOrderShippingSerializer(data=order_shipping, context=self.context)
         order = super().create(validated_data)
         if order_products_serializer.is_valid():
             order_products_serializer.save(order=order)
         if order_shipping_serializer.is_valid():
             order_shipping_serializer.save(order=order)
+        quantities = [product["quantity"] for product in order_products]
+        prices = [item["product"]["price"] for _ in order_products for item in order_products]
+        order.total = total_products_price(prices, quantities)
         return order
 
     @transaction.atomic
     def update(self, instance: Order, validated_data: dict) -> Order:
         order_products = validated_data.pop("products", None)
         order_shipping = validated_data.pop("shipping", None)
         order = super().update(instance, validated_data)
@@ -78,8 +83,11 @@
             update_related_objects(self, "order", order, "products", order_products, OrderProductSerializer)
         if order_shipping is not None:
             old_shipping = OrderShipping.objects.get(order=instance)
             new_shipping = BaseOrderShippingSerializer(data=order_shipping, context=self.context)
             if new_shipping.is_valid():
                 old_shipping.delete()
                 new_shipping.save(order=order)
+        quantities = [product["quantity"] for product in order_products]
+        prices = [item["product"]["price"] for _ in order_products for item in order_products]
+        order.total = total_products_price(prices, quantities)
         return order
```

### Comparing `drf_shop_api-0.0.1/drf_shop_api/orders/tests.py` & `drf_shop_api-0.0.2/drf_shop_api/orders/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,21 +53,24 @@
         self.assertEqual(resp.status_code, 200)
 
     def test_create_order(self):
         product = Product.objects.first()
         data = {
             "shipping": {"address": "Home", "method": BaseShippingMethodSerializer(self.shipping_method).data},
             "products": [{"product": ProductSerializer(product).data, "quantity": 10}],
+            "total": 1,
         }
         self.authorize(self.target.user)
         resp = self.client.post(f"{self.list_url}", data)
         self.assertEqual(resp.status_code, 201)
+        self.assertEqual(float(resp.data["total"]), product.price * 10)
 
     def test_update_order_products(self):
         product = Product.objects.first()
         data = {
             "shipping": {"address": "Home", "method": BaseShippingMethodSerializer(self.shipping_method).data},
             "products": [{"product": ProductSerializer(product).data, "quantity": 50}],
         }
         self.authorize(self.target.user)
         resp = self.client.patch(f"{self.list_url}{self.target.id}/", data)
         self.assertEqual(resp.status_code, 200)
+        self.assertEqual(float(resp.data["total"]), product.price * 50)
```

### Comparing `drf_shop_api-0.0.1/drf_shop_api/orders/views.py` & `drf_shop_api-0.0.2/drf_shop_api/orders/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,30 +14,34 @@
     mixins.ListModelMixin,
     mixins.RetrieveModelMixin,
     mixins.CreateModelMixin,
     mixins.UpdateModelMixin,
     viewsets.GenericViewSet,
 ):
     """
+    create:
+    Create order
+
+    As authenticated user you can create order by providing product and quantity
+
     list:
-    All customer carts.
+    All orders.
 
-    In case of admin user list all Customer cart
-    In case of regular user return only his cart
-    Can be filtered by: `user`
+    In case of admin user list all orders
+    In case of regular user return only his orders
 
     retrieve:
-    Details of single customer cart
+    Details of single customer order
 
-    As admin retrieve customer cart details by `id`
+    As admin retrieve customer order details by `id`
 
     update:
-    Update customer cart
+    Update order
 
-    As owner you can update your cart by providing product and quantity with payload like this
+    As owner you can update your order by providing product and quantity with payload like this
     ```
     {"id": 10,
     "user": 63,
     "products": [
         {"id": 10, "product":
                 {"id": 10,
                 "price": "100.00",
@@ -49,17 +53,17 @@
                 "images": [],
                 "properties": []},
                 "quantity": 15}
         ]}
     ```
 
     partial_update:
-    Update customer cart
+    Update order
 
-    As owner you can update your cart
+    As owner you can update your order
     """
 
     permission_classes = [GetByAuthOrAdminEditByAdmin]
     serializer_class = OrderSerializer
     list_serializer_class = BaseOrderSerializer
     pagination_class = OwnershipPaginator
     filter_backends = (DjangoFilterBackend,)
```

### Comparing `drf_shop_api-0.0.1/drf_shop_api/paginators.py` & `drf_shop_api-0.0.2/drf_shop_api/paginators.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.1/drf_shop_api/permissions.py` & `drf_shop_api-0.0.2/drf_shop_api/permissions.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.1/drf_shop_api/products/filters.py` & `drf_shop_api-0.0.2/drf_shop_api/products/filters.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.1/drf_shop_api/products/models.py` & `drf_shop_api-0.0.2/drf_shop_api/products/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,36 +10,42 @@
     url = models.SlugField(unique=True, max_length=255)
     parent = models.ForeignKey("self", on_delete=models.CASCADE, null=True, blank=True, related_name="children")
     is_active = models.BooleanField(default=True)
 
     class Meta:
         db_table = "product-categories"
         indexes = [models.Index(fields=["url"])]
+        verbose_name_plural = "Product categories"
 
     def is_parent_category(self):
         return bool(self.parent is None)
 
+    @property
     def parent_category_id(self):
         return self.parent.id if self.parent is not None else None
 
     def save(self, *args, **kwargs):
         self.url = slugify(self.title)
         super(ProductCategory, self).save(*args, **kwargs)
 
 
 class Product(TitleDescriptionModel, TimeStampedModel):
     price = models.DecimalField(max_digits=6, decimal_places=2, validators=[MinValueValidator(0)])
     currency = models.ForeignKey("drf_shop_api.Currency", on_delete=models.CASCADE)
     category = models.ForeignKey(ProductCategory, on_delete=models.CASCADE)
     is_active = models.BooleanField(default=True)
+    quantity = models.IntegerField(default=1)
 
     class Meta:
         db_table = "products"
         ordering = ("-id",)
 
+    def __str__(self) -> str:
+        return f"{self.title}: {self.price}"
+
 
 class ProductImage(models.Model):
     product = models.ForeignKey(Product, models.CASCADE, related_name="images")
     image = models.ImageField()
     is_main = models.BooleanField(default=False)
 
     class Meta:
@@ -48,27 +54,31 @@
 
 class Property(TitleDescriptionModel):
     unit = models.CharField(max_length=255, choices=[(v.name, v.value) for v in Units], null=True, blank=True)
 
     class Meta:
         db_table = "properties"
         ordering = ("-id",)
+        verbose_name_plural = "Properties"
+
+    def __str__(self):
+        return f"{self.title} ({self.unit})" if self.unit else self.title
 
 
 class ProductProperty(models.Model):
     product = models.ForeignKey(Product, models.CASCADE, related_name="properties")
     property = models.ForeignKey(Property, models.CASCADE)
     value = models.CharField(max_length=200)
 
     class Meta:
         db_table = "product-properties"
         ordering = ("-id",)
+        verbose_name_plural = "Product properties"
 
 
-# TODO: Extend with rating options
 class ProductComment(OwnershipMultipleModel):
     product = models.ForeignKey(Product, models.CASCADE, related_name="comments")
     content = models.TextField()
 
     class Meta:
         db_table = "product-comments"
         ordering = ("-id",)
```

### Comparing `drf_shop_api-0.0.1/drf_shop_api/products/tests.py` & `drf_shop_api-0.0.2/drf_shop_api/products/tests.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.1/drf_shop_api/products/views.py` & `drf_shop_api-0.0.2/drf_shop_api/products/views.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.1/drf_shop_api/serializers.py` & `drf_shop_api-0.0.2/drf_shop_api/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.1/drf_shop_api/tests.py` & `drf_shop_api-0.0.2/drf_shop_api/tests.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.1/pyproject.toml` & `drf_shop_api-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-shop-api"
-version = "0.0.1"
+version = "0.0.2"
 description = "Standalone shop app, that you can add to your project"
 authors = ["Oleksandr Korol <oleksandr.korol@coaxsoft.com>"]
 readme = "README.md"
 packages = [{include = "drf_shop_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `drf_shop_api-0.0.1/setup.py` & `drf_shop_api-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'django-filter>=23.2,<24.0',
  'djangorestframework>=3.14.0,<4.0.0',
  'drf-yasg>=1.21.5,<2.0.0',
  'rest-framework-simplejwt>=0.0.2,<0.0.3']
 
 setup_kwargs = {
     'name': 'drf-shop-api',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Standalone shop app, that you can add to your project',
-    'long_description': '# Features\n\nFeatures:\n\n- Products\n  - products (multiple images + main image, title, description, etc.)\n  - products categories (parent/child categories)\n  - product dynamic stats (for filtering like on Rozetka, ek.ua)\n  - product comments\n  - search for products/categories\n  - filter for products in the category\n- Customers\n  - wish lists\n  - cart\n  - compare lists\n  - bonuses wallet\n- Settings\n  - taxes\n  - currencies\n- Orders\n  - orders\n  - order reports (view and generation of pdf)\n  - shipping\n  - statuses of order / payment / shipment\n\n## Customers\n\nThis app will hold User related data:\n\n`CustomerCart`\n`CustomerWishList`\n`CustomerBonusWallet`\n`CustomerOrderHistory`\n\n## Settings requirements\n\n- DRF settings\n\n```json\n"DEFAULT_AUTHENTICATION_CLASSES": ("rest_framework_simplejwt.authentication.JWTAuthentication",)\n```\n\n- DRF_SHOP settings:\n  - DRF_SHOP_PAGE_SIZE on will be default 10\n  - DRF_SHOP_PAYMENT_MODEL = "projects.payments.models.Payment"\n  - DRF_SHOP_PAYMENT_STATUS_CHOICES = "project.payments.choices.PaymentStatus"\n  - DRF_SHOP_BONUS_RATE = percentage value for each order that will go to bonus wallet (e.g. 10)\n\n> Statuses should be aligned as regular flow then cancel followed by refund\n\nModify user management:\nFor creation of related models please use create_shop_profile decorator on you UserManager class\n\n```python\nfrom django.contrib.auth.base_user import BaseUserManager\n\nfrom drf_shop_api.decorators import create_shop_profile\n\n\nclass UserManager(BaseUserManager):\n    @create_shop_profile\n    def create_user(self, email, password=None):\n        if not email:\n            raise ValueError("Enter the email")\n        user = self.model(email=self.normalize_email(email))\n        user.set_password(password)\n        user.save(using=self._db)\n        return user\n\n```\n\n## Dependencies\n\n    django\n    drf\n    drf-yasg 1.21.5\n    rest_framework_simplejwt\n    mixer\n    django-filter\n\n### TODO\n\n- Add DB indexes\n- Task for currency rate update\n- Review permissions\n- Add custom migration to create all related model for auth user model\n- Integrate payment from external project\n',
+    'long_description': '# Features\n\nFeatures:\n\n- products (multiple images + main image, title, description, etc.)\n- products categories (parent/child categories)\n- product dynamic stats (for filtering like on Rozetka, ek.ua)\n- product comments\n- wish lists\n- cart\n- compare lists\n- orders\n- order reports (+ ability to generate pdf)\n- history\n- contact online support via web-sockets (or offline via email)\n- connect implemented payment systems\n- shipment\n- taxes\n- bonuses wallet\n- search for products/categories\n- filter for products in the category\n- statuses of buy / payment / shipment\n\nFeatures:\n\n- Products\n  - products (multiple images + main image, title, description, etc.)\n  - products categories (parent/child categories)\n  - product dynamic stats (for filtering like on Rozetka, ek.ua)\n  - product comments\n  - search for products/categories\n  - filter for products in the category\n- Customers\n  - wish lists\n  - cart\n  - compare lists\n  - bonuses wallet\n- Settings\n  - taxes\n  - currencies\n- Orders\n  - orders\n  - order reports (view and generation of pdf)\n  - shipping\n  - statuses of order / payment / shipment\n\n## Installation\n\n- Install library\n\n```bash\npip install drf-shop-api\n```\n\n- Add to installed apps\n\n  ```python\n\n  INSTALLED_APPS = [\n    ...\n    \'drf_shop_api\'\n  ]\n  ```\n\n- Add api path to you root urls.py\n\n```python\n   urlpatterns = [\n    ...\n    path("shop/", include("drf_shop_api.urls")),\n]\n```\n\n- Use `create_shop_profile` decorator on create_user method of your UserManager\n\n```python\nfrom django.contrib.auth.base_user import BaseUserManager\n\nfrom drf_shop_api.decorators import create_shop_profile\n\n\nclass UserManager(BaseUserManager):\n    @create_shop_profile\n    def create_user(self, email, password=None):\n        if not email:\n            raise ValueError("Enter the email")\n        user = self.model(email=self.normalize_email(email))\n        user.set_password(password)\n        user.save(using=self._db)\n        return user\n```\n\n- Setup `AUTH_USER_MODEL` in settings.py\n\n- Run `python manage.py makemigrations` and `python manage.py migrate` (Due to optional Payment model from root project)\n\n## Features overview\n\n### Customers\n\nThis app will hold User related data:\n\n`CustomerCart`\n`CustomerWishList`\n`CustomerBonusWallet`\n`CustomerOrderHistory`\n\n## Settings requirements\n\n- DRF settings\n\n```json\n"DEFAULT_AUTHENTICATION_CLASSES": ("rest_framework_simplejwt.authentication.JWTAuthentication",)\n```\n\n- DRF_SHOP settings:\n  - DRF_SHOP_PAGE_SIZE on will be default 10\n  - DRF_SHOP_PAYMENT_MODEL = "projects.payments.models.Payment"\n  - DRF_SHOP_PAYMENT_STATUS_CHOICES = "project.payments.choices.PaymentStatus"\n  - DRF_SHOP_BONUS_RATE = percentage value for each order that will go to bonus wallet\n\n> Statuses should be aligned as regular flow then cancel followed by refund\n\n## Dependencies\n\n    django\n    drf\n    drf-yasg 1.21.5\n    rest_framework_simplejwt\n    mixer\n    django-filter\n\n### TODO\n\n- Add DB indexes\n- Task for currency rate update\n- Review permissions\n- Add custom migration to create all related model for auth user model\n',
     'author': 'Oleksandr Korol',
     'author_email': 'oleksandr.korol@coaxsoft.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

