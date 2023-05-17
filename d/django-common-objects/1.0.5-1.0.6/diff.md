# Comparing `tmp/django-common-objects-1.0.5.tar.gz` & `tmp/django-common-objects-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-objects-1.0.5.tar", last modified: Fri Apr  7 08:59:16 2023, max compression
+gzip compressed data, was "django-common-objects-1.0.6.tar", last modified: Wed May 17 03:16:49 2023, max compression
```

## Comparing `django-common-objects-1.0.5.tar` & `django-common-objects-1.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 08:59:16.297664 django-common-objects-1.0.5/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:17:44.000000 django-common-objects-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      296 2023-04-07 08:59:16.297664 django-common-objects-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-02-28 03:17:44.000000 django-common-objects-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 08:59:16.241406 django-common-objects-1.0.5/django_common_objects/
--rw-rw-rw-   0        0        0        0 2023-02-28 03:21:57.000000 django-common-objects-1.0.5/django_common_objects/__init__.py
--rw-rw-rw-   0        0        0     5521 2023-02-28 03:24:51.000000 django-common-objects-1.0.5/django_common_objects/admin.py
--rw-rw-rw-   0        0        0      155 2023-02-28 03:45:02.000000 django-common-objects-1.0.5/django_common_objects/apps.py
--rw-rw-rw-   0        0        0     2580 2023-02-28 03:45:52.000000 django-common-objects-1.0.5/django_common_objects/choices.py
--rw-rw-rw-   0        0        0     1498 2023-02-28 03:29:27.000000 django-common-objects-1.0.5/django_common_objects/fields.py
--rw-rw-rw-   0        0        0     1374 2023-04-04 01:25:03.000000 django-common-objects-1.0.5/django_common_objects/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-07 08:59:16.284383 django-common-objects-1.0.5/django_common_objects/migrations/
--rw-rw-rw-   0        0        0     4311 2023-03-07 07:19:54.000000 django-common-objects-1.0.5/django_common_objects/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      832 2023-04-04 01:15:03.000000 django-common-objects-1.0.5/django_common_objects/migrations/0002_alter_commoncategory_model_and_more.py
--rw-rw-rw-   0        0        0      826 2023-04-07 08:58:05.000000 django-common-objects-1.0.5/django_common_objects/migrations/0003_alter_commoncategory_unique_together_and_more.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:13:25.000000 django-common-objects-1.0.5/django_common_objects/migrations/__init__.py
--rw-rw-rw-   0        0        0     4035 2023-04-07 08:56:28.000000 django-common-objects-1.0.5/django_common_objects/models.py
--rw-rw-rw-   0        0        0      488 2023-02-16 05:39:51.000000 django-common-objects-1.0.5/django_common_objects/rest_view.py
--rw-rw-rw-   0        0        0      738 2023-02-16 09:09:26.000000 django-common-objects-1.0.5/django_common_objects/serializers.py
--rw-rw-rw-   0        0        0      439 2023-03-13 09:48:04.000000 django-common-objects-1.0.5/django_common_objects/settings.py
--rw-rw-rw-   0        0        0      804 2023-03-13 09:30:10.000000 django-common-objects-1.0.5/django_common_objects/site.py
--rw-rw-rw-   0        0        0       63 2023-02-28 03:21:57.000000 django-common-objects-1.0.5/django_common_objects/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-07 08:59:16.296381 django-common-objects-1.0.5/django_common_objects/utils/
--rw-rw-rw-   0        0        0        0 2023-02-16 03:57:14.000000 django-common-objects-1.0.5/django_common_objects/utils/__init__.py
--rw-rw-rw-   0        0        0      166 2023-02-28 03:30:14.000000 django-common-objects-1.0.5/django_common_objects/utils/admin.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-objects-1.0.5/django_common_objects/utils/algorithm.py
--rw-rw-rw-   0        0        0      522 2023-02-28 03:46:13.000000 django-common-objects-1.0.5/django_common_objects/utils/foreign_key.py
--rw-rw-rw-   0        0        0      880 2023-02-15 06:14:26.000000 django-common-objects-1.0.5/django_common_objects/validator.py
--rw-rw-rw-   0        0        0       66 2023-02-28 03:21:57.000000 django-common-objects-1.0.5/django_common_objects/views.py
--rw-rw-rw-   0        0        0     2183 2023-03-07 02:46:25.000000 django-common-objects-1.0.5/django_common_objects/widgets.py
-drwxrwxrwx   0        0        0        0 2023-04-07 08:59:16.268898 django-common-objects-1.0.5/django_common_objects.egg-info/
--rw-rw-rw-   0        0        0      296 2023-04-07 08:59:16.000000 django-common-objects-1.0.5/django_common_objects.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1176 2023-04-07 08:59:16.000000 django-common-objects-1.0.5/django_common_objects.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 08:59:16.000000 django-common-objects-1.0.5/django_common_objects.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-07 08:59:16.000000 django-common-objects-1.0.5/django_common_objects.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-07 08:59:16.000000 django-common-objects-1.0.5/django_common_objects.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 08:59:16.297664 django-common-objects-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-04-04 01:29:04.000000 django-common-objects-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 08:59:16.296381 django-common-objects-1.0.5/tests/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:09:57.000000 django-common-objects-1.0.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:16:49.919515 django-common-objects-1.0.6/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:17:44.000000 django-common-objects-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      296 2023-05-17 03:16:49.919515 django-common-objects-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-02-28 03:17:44.000000 django-common-objects-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 03:16:49.865767 django-common-objects-1.0.6/django_common_objects/
+-rw-rw-rw-   0        0        0        0 2023-02-28 03:21:57.000000 django-common-objects-1.0.6/django_common_objects/__init__.py
+-rw-rw-rw-   0        0        0     5521 2023-02-28 03:24:51.000000 django-common-objects-1.0.6/django_common_objects/admin.py
+-rw-rw-rw-   0        0        0      155 2023-02-28 03:45:02.000000 django-common-objects-1.0.6/django_common_objects/apps.py
+-rw-rw-rw-   0        0        0     2580 2023-02-28 03:45:52.000000 django-common-objects-1.0.6/django_common_objects/choices.py
+-rw-rw-rw-   0        0        0     1498 2023-02-28 03:29:27.000000 django-common-objects-1.0.6/django_common_objects/fields.py
+-rw-rw-rw-   0        0        0     2033 2023-05-17 02:59:55.000000 django-common-objects-1.0.6/django_common_objects/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:16:49.897309 django-common-objects-1.0.6/django_common_objects/migrations/
+-rw-rw-rw-   0        0        0     4132 2023-05-17 03:14:17.000000 django-common-objects-1.0.6/django_common_objects/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      832 2023-04-04 01:15:03.000000 django-common-objects-1.0.6/django_common_objects/migrations/0002_alter_commoncategory_model_and_more.py
+-rw-rw-rw-   0        0        0      751 2023-05-17 03:14:29.000000 django-common-objects-1.0.6/django_common_objects/migrations/0003_alter_commoncategory_unique_together_and_more.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:13:25.000000 django-common-objects-1.0.6/django_common_objects/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3612 2023-05-17 03:13:33.000000 django-common-objects-1.0.6/django_common_objects/models.py
+-rw-rw-rw-   0        0        0      488 2023-02-16 05:39:51.000000 django-common-objects-1.0.6/django_common_objects/rest_view.py
+-rw-rw-rw-   0        0        0      738 2023-02-16 09:09:26.000000 django-common-objects-1.0.6/django_common_objects/serializers.py
+-rw-rw-rw-   0        0        0      439 2023-03-13 09:48:04.000000 django-common-objects-1.0.6/django_common_objects/settings.py
+-rw-rw-rw-   0        0        0      804 2023-03-13 09:30:10.000000 django-common-objects-1.0.6/django_common_objects/site.py
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:21:57.000000 django-common-objects-1.0.6/django_common_objects/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:16:49.917308 django-common-objects-1.0.6/django_common_objects/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-16 03:57:14.000000 django-common-objects-1.0.6/django_common_objects/utils/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-02-28 03:30:14.000000 django-common-objects-1.0.6/django_common_objects/utils/admin.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-objects-1.0.6/django_common_objects/utils/algorithm.py
+-rw-rw-rw-   0        0        0      522 2023-02-28 03:46:13.000000 django-common-objects-1.0.6/django_common_objects/utils/foreign_key.py
+-rw-rw-rw-   0        0        0      880 2023-02-15 06:14:26.000000 django-common-objects-1.0.6/django_common_objects/validator.py
+-rw-rw-rw-   0        0        0       66 2023-02-28 03:21:57.000000 django-common-objects-1.0.6/django_common_objects/views.py
+-rw-rw-rw-   0        0        0     2183 2023-03-07 02:46:25.000000 django-common-objects-1.0.6/django_common_objects/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:16:49.888407 django-common-objects-1.0.6/django_common_objects.egg-info/
+-rw-rw-rw-   0        0        0      296 2023-05-17 03:16:49.000000 django-common-objects-1.0.6/django_common_objects.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1176 2023-05-17 03:16:49.000000 django-common-objects-1.0.6/django_common_objects.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 03:16:49.000000 django-common-objects-1.0.6/django_common_objects.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-17 03:16:49.000000 django-common-objects-1.0.6/django_common_objects.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-05-17 03:16:49.000000 django-common-objects-1.0.6/django_common_objects.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 03:16:49.919515 django-common-objects-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-05-17 03:16:16.000000 django-common-objects-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 03:16:49.918506 django-common-objects-1.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:09:57.000000 django-common-objects-1.0.6/tests/__init__.py
```

### Comparing `django-common-objects-1.0.5/LICENSE` & `django-common-objects-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.5/django_common_objects/admin.py` & `django-common-objects-1.0.6/django_common_objects/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.5/django_common_objects/choices.py` & `django-common-objects-1.0.6/django_common_objects/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.5/django_common_objects/fields.py` & `django-common-objects-1.0.6/django_common_objects/fields.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.5/django_common_objects/forms.py` & `django-common-objects-1.0.6/django_common_objects/forms.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import json
+
 from django import forms
 from .choices import CategoryModelChoices, TagModelChoices, FieldConfigModelChoices
-from .models import CommonCategory
+from .models import CommonCategory, CommonFieldConfig, CommonTag
 from .utils import foreign_key
 
 
 class FieldConfigForm(forms.ModelForm):
     model = forms.ChoiceField(choices=FieldConfigModelChoices.choices, label="所属模型", required=True)
 
 
@@ -14,14 +16,17 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         instance: CommonCategory = self.instance
         if instance.id:
             self.fields['parent'].queryset = CommonCategory.objects.filter(
                 model=instance.model, user=instance.user
             ).exclude(id__in=foreign_key.get_related_object_ids(instance))
+        else:
+            fields = CommonFieldConfig.objects.filter(model=instance._meta.label).values_list('key', 'value')
+            self.fields['config'].initial = {k: v for k, v in fields}
 
     def clean(self):
         cleaned_data = super().clean()
         model = cleaned_data.get('model')
         parent = cleaned_data.get('parent')
         if model and parent and model != parent.model:
             raise forms.ValidationError('所属模型不一致')
@@ -30,7 +35,18 @@
     class Meta:
         model = CommonCategory
         fields = "__all__"
 
 
 class TagForm(forms.ModelForm):
     model = forms.ChoiceField(choices=TagModelChoices.choices, label="所属模型", required=True)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        instance: CommonTag = self.instance
+        if not instance.id:
+            fields = CommonFieldConfig.objects.filter(model=instance._meta.label).values_list('key', 'value')
+            self.fields['config'].initial = {k: v for k, v in fields}
+
+    class Meta:
+        model = CommonTag
+        fields = "__all__"
```

### Comparing `django-common-objects-1.0.5/django_common_objects/migrations/0001_initial.py` & `django-common-objects-1.0.6/django_common_objects/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.1.7 on 2023-03-07 15:13
 
 import django_common_objects.fields
 import django_common_objects.models
 from django.conf import settings
 from django.db import migrations, models
-import django.db.models.deletion
 import django.utils.timezone
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
@@ -37,15 +36,15 @@
         ),
         migrations.CreateModel(
             name='CommonTag',
             fields=[
                 ('id', models.AutoField(primary_key=True, serialize=False)),
                 ('model', models.CharField(max_length=30, verbose_name='所属模型')),
                 ('name', models.CharField(max_length=50, verbose_name='标签名')),
-                ('config', django_common_objects.fields.ConfigField(blank=True, default=django_common_objects.models.get_default_config('CommonTag'), null=True, verbose_name='详细')),
+                ('config', django_common_objects.fields.ConfigField(blank=True, null=True, verbose_name='详细')),
                 ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
                 ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
                 ('user', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户')),
             ],
             options={
                 'verbose_name': '通用标签',
                 'verbose_name_plural': '通用标签',
@@ -55,15 +54,15 @@
         ),
         migrations.CreateModel(
             name='CommonCategory',
             fields=[
                 ('id', models.AutoField(primary_key=True, serialize=False)),
                 ('model', models.CharField(max_length=30, verbose_name='所属模型')),
                 ('name', models.CharField(max_length=50, verbose_name='名称')),
-                ('config', django_common_objects.fields.ConfigField(blank=True, default=django_common_objects.models.get_default_config('CommonCategory'), null=True, verbose_name='详细')),
+                ('config', django_common_objects.fields.ConfigField(blank=True, null=True, verbose_name='详细')),
                 ('create_time', models.DateTimeField(default=django.utils.timezone.now, verbose_name='创建时间')),
                 ('update_time', models.DateTimeField(auto_now=True, verbose_name='更新时间')),
                 ('parent', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.CASCADE, related_name='children', to='django_common_objects.commoncategory', verbose_name='父类别')),
                 ('user', models.ForeignKey(db_constraint=False, on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL, verbose_name='用户')),
             ],
             options={
                 'verbose_name': '通用类别',
```

### Comparing `django-common-objects-1.0.5/django_common_objects/migrations/0002_alter_commoncategory_model_and_more.py` & `django-common-objects-1.0.6/django_common_objects/migrations/0002_alter_commoncategory_model_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.5/django_common_objects/migrations/0003_alter_commoncategory_unique_together_and_more.py` & `django-common-objects-1.0.6/django_common_objects/migrations/0003_alter_commoncategory_unique_together_and_more.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,10 +16,10 @@
         migrations.AlterUniqueTogether(
             name='commoncategory',
             unique_together={('name', 'user')},
         ),
         migrations.AlterField(
             model_name='commoncategory',
             name='config',
-            field=models.JSONField(blank=True, default=django_common_objects.models.get_default_config('CommonCategory'), null=True, verbose_name='详细'),
+            field=models.JSONField(blank=True, null=True, verbose_name='详细'),
         ),
     ]
```

### Comparing `django-common-objects-1.0.5/django_common_objects/models.py` & `django-common-objects-1.0.6/django_common_objects/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,31 +3,19 @@
 from django.utils import timezone
 from .utils import foreign_key
 from .choices import CommonFieldConfigType
 from .fields import ConfigField
 from .widgets import JSONWidget
 from django.contrib.admin.options import FORMFIELD_FOR_DBFIELD_DEFAULTS
 from django.forms import fields as _form_fields
-from django.utils.deconstruct import deconstructible
 
 
 UserModel = get_user_model()
 
 
-@deconstructible
-class get_default_config:
-
-    def __init__(self, model):
-        self.model = model
-
-    def __call__(self):
-        fields = CommonFieldConfig.objects.filter(model=self.model).values_list('key', 'value')
-        return {k: v for k, v in fields}
-
-
 class CommonFieldConfig(models.Model):
     id = models.AutoField(primary_key=True)
     model = models.CharField(max_length=100, verbose_name='所属模型')
     key = models.CharField(max_length=20, verbose_name='字段')
     value = models.CharField(max_length=200, null=True, blank=True, verbose_name='值')
     type = models.CharField(max_length=10, default=CommonFieldConfigType.STR, verbose_name='类型',
                             choices=CommonFieldConfigType.choices)
@@ -47,15 +35,15 @@
 
 class CommonCategory(models.Model):
     id = models.AutoField(primary_key=True)
     model = models.CharField(max_length=100, verbose_name='所属模型')
     parent = models.ForeignKey('self', blank=True, null=True, db_constraint=False, on_delete=models.CASCADE,
                                related_name='children', verbose_name='父类别')
     name = models.CharField(max_length=50, verbose_name='名称')
-    config = models.JSONField(default=get_default_config('CommonCategory'), blank=True, null=True, verbose_name='详细')
+    config = ConfigField(blank=True, null=True, verbose_name='详细')
     user = models.ForeignKey(UserModel, on_delete=models.CASCADE, db_constraint=False, verbose_name='用户')
     create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
     update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
 
     @property
     def related_categories_ids(self):
         return foreign_key.get_related_object_ids(self)
@@ -71,15 +59,15 @@
     __repr__ = __str__
 
 
 class CommonTag(models.Model):
     id = models.AutoField(primary_key=True)
     model = models.CharField(max_length=100, verbose_name='所属模型')
     name = models.CharField(max_length=50, verbose_name='标签名')
-    config = ConfigField(default=get_default_config('CommonTag'), blank=True, null=True, verbose_name='详细')
+    config = ConfigField(blank=True, null=True, verbose_name='详细')
     user = models.ForeignKey(UserModel, on_delete=models.CASCADE, db_constraint=False, verbose_name='用户')
     create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
     update_time = models.DateTimeField(auto_now=True, verbose_name='更新时间')
 
     class Meta:
         db_table = 'common_tag'
         verbose_name = verbose_name_plural = '通用标签'
```

### Comparing `django-common-objects-1.0.5/django_common_objects/serializers.py` & `django-common-objects-1.0.6/django_common_objects/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.5/django_common_objects/site.py` & `django-common-objects-1.0.6/django_common_objects/site.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.5/django_common_objects/utils/algorithm.py` & `django-common-objects-1.0.6/django_common_objects/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.5/django_common_objects/utils/foreign_key.py` & `django-common-objects-1.0.6/django_common_objects/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.5/django_common_objects/validator.py` & `django-common-objects-1.0.6/django_common_objects/validator.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.5/django_common_objects/widgets.py` & `django-common-objects-1.0.6/django_common_objects/widgets.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.5/django_common_objects.egg-info/SOURCES.txt` & `django-common-objects-1.0.6/django_common_objects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

