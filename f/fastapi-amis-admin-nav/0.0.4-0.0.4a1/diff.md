# Comparing `tmp/fastapi_amis_admin_nav-0.0.4.tar.gz` & `tmp/fastapi_amis_admin_nav-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin_nav-0.0.4.tar", last modified: Wed May 17 07:13:22 2023, max compression
+gzip compressed data, was "fastapi_amis_admin_nav-0.0.4a1.tar", last modified: Sat Apr 15 09:28:24 2023, max compression
```

## Comparing `fastapi_amis_admin_nav-0.0.4.tar` & `fastapi_amis_admin_nav-0.0.4a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3037 2023-02-19 04:26:35.599654 fastapi_amis_admin_nav-0.0.4/README.md
--rw-r--r--   0        0        0      380 2023-05-17 07:13:02.878647 fastapi_amis_admin_nav-0.0.4/fastapi_amis_admin_nav/__init__.py
--rw-r--r--   0        0        0     5168 2023-03-23 08:41:54.647360 fastapi_amis_admin_nav-0.0.4/fastapi_amis_admin_nav/admin.py
--rw-r--r--   0        0        0     4715 2023-04-15 09:15:19.759421 fastapi_amis_admin_nav-0.0.4/fastapi_amis_admin_nav/models.py
--rw-r--r--   0        0        0     8570 2023-05-04 01:29:09.446260 fastapi_amis_admin_nav-0.0.4/fastapi_amis_admin_nav/utils.py
--rw-r--r--   0        0        0     1645 2023-03-22 07:48:40.603529 fastapi_amis_admin_nav-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 fastapi_amis_admin_nav-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3037 2023-02-19 04:26:35.599654 fastapi_amis_admin_nav-0.0.4a1/README.md
+-rw-r--r--   0        0        0      382 2023-04-15 09:28:19.081403 fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/__init__.py
+-rw-r--r--   0        0        0     5168 2023-03-23 08:41:54.647360 fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/admin.py
+-rw-r--r--   0        0        0     4715 2023-04-15 09:15:19.759421 fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/models.py
+-rw-r--r--   0        0        0     8437 2023-03-23 11:45:23.744360 fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/utils.py
+-rw-r--r--   0        0        0     1645 2023-03-22 07:48:40.603529 fastapi_amis_admin_nav-0.0.4a1/pyproject.toml
+-rw-r--r--   0        0        0     4110 1970-01-01 00:00:00.000000 fastapi_amis_admin_nav-0.0.4a1/PKG-INFO
```

### Comparing `fastapi_amis_admin_nav-0.0.4/README.md` & `fastapi_amis_admin_nav-0.0.4a1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.4/fastapi_amis_admin_nav/admin.py` & `fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/admin.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.4/fastapi_amis_admin_nav/models.py` & `fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.4/fastapi_amis_admin_nav/utils.py` & `fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,14 @@
             if not admin_.page_schema:  # 如果不存在page_schema,则不保存到数据库
                 return None
             unique_id = str(admin_.unique_id)
             page = self.db_pages_uid_map.get(unique_id)
             # print('unique_id', unique_id, page)
             if page:  # 如果存在数据库中,则读取数据库中设置,并且更新到admin
                 page.is_active = True  # 设置为激活
-                page.icon = admin_.page_schema.icon or page.icon
-                page.label = admin_.page_schema.label or page.label
                 return page.id
             # 保存到数据库
             kwargs = {
                 "parent_id": parent_id,
                 "unique_id": unique_id,
             }
             if isinstance(admin_, AdminGroup):
```

### Comparing `fastapi_amis_admin_nav-0.0.4/pyproject.toml` & `fastapi_amis_admin_nav-0.0.4a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.4/PKG-INFO` & `fastapi_amis_admin_nav-0.0.4a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_amis_admin_nav
-Version: 0.0.4
+Version: 0.0.4a1
 Summary: FastAPI-Amis-Admin-Nav是一个基于FastAPI-Amis-Admin并且为FastAPI-Amis-Admin提供可视化导航页面管理的拓展库.
 Keywords: fastapi,fastapi-user-auth,fastapi-amis-admin,fastapi-amis-admin-nav
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
```

