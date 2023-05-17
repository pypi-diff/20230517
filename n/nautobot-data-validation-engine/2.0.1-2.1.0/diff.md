# Comparing `tmp/nautobot_data_validation_engine-2.0.1.tar.gz` & `tmp/nautobot_data_validation_engine-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_data_validation_engine-2.0.1.tar", max compression
+gzip compressed data, was "nautobot_data_validation_engine-2.1.0.tar", max compression
```

## Comparing `nautobot_data_validation_engine-2.0.1.tar` & `nautobot_data_validation_engine-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,39 @@
--rw-r--r--   0        0        0      591 2023-04-28 17:25:51.701840 nautobot_data_validation_engine-2.0.1/LICENSE
--rw-r--r--   0        0        0     4876 2023-04-28 17:25:51.701840 nautobot_data_validation_engine-2.0.1/README.md
--rw-r--r--   0        0        0     1026 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/__init__.py
--rw-r--r--   0        0        0       66 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/__init__.py
--rw-r--r--   0        0        0     2598 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/nested_serializers.py
--rw-r--r--   0        0        0     4258 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/serializers.py
--rw-r--r--   0        0        0      605 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/urls.py
--rw-r--r--   0        0        0     1727 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/views.py
--rw-r--r--   0        0        0     5509 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/custom_validators.py
--rw-r--r--   0        0        0     4261 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/filters.py
--rw-r--r--   0        0        0    11119 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/forms.py
--rw-r--r--   0        0        0     3452 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/migrations/0001_initial.py
--rw-r--r--   0        0        0     5786 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/migrations/0002_required_unique_types_regex_context.py
--rw-r--r--   0        0        0        0 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/migrations/__init__.py
--rw-r--r--   0        0        0    13313 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/models.py
--rw-r--r--   0        0        0     4248 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/navigation.py
--rw-r--r--   0        0        0     3392 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tables.py
--rw-r--r--   0        0        0     1110 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/minmaxvalidationrule_retrieve.html
--rw-r--r--   0        0        0     1204 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/regularexpressionvalidationrule_retrieve.html
--rw-r--r--   0        0        0      907 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/requiredvalidationrule_retrieve.html
--rw-r--r--   0        0        0     1017 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/uniquevalidationrule_retrieve.html
--rw-r--r--   0        0        0       61 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/__init__.py
--rw-r--r--   0        0        0     8124 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_api.py
--rw-r--r--   0        0        0     1536 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_basic.py
--rw-r--r--   0        0        0    13489 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_custom_validators.py
--rw-r--r--   0        0        0     9131 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_filters.py
--rw-r--r--   0        0        0    11014 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_models.py
--rw-r--r--   0        0        0     8877 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_views.py
--rw-r--r--   0        0        0     2246 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/urls.py
--rw-r--r--   0        0        0     2994 2023-04-28 17:25:51.709840 nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/views.py
--rw-r--r--   0        0        0     3700 2023-04-28 17:26:02.073921 nautobot_data_validation_engine-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     5911 1970-01-01 00:00:00.000000 nautobot_data_validation_engine-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-05-17 19:23:37.781689 nautobot_data_validation_engine-2.1.0/LICENSE
+-rw-r--r--   0        0        0     4876 2023-05-17 19:23:37.781689 nautobot_data_validation_engine-2.1.0/README.md
+-rw-r--r--   0        0        0     1089 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/__init__.py
+-rw-r--r--   0        0        0       66 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/api/__init__.py
+-rw-r--r--   0        0        0     2598 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/api/nested_serializers.py
+-rw-r--r--   0        0        0     4495 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/api/serializers.py
+-rw-r--r--   0        0        0      688 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/api/urls.py
+-rw-r--r--   0        0        0     1932 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/api/views.py
+-rw-r--r--   0        0        0    12283 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/custom_validators.py
+-rw-r--r--   0        0        0      996 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/datasources.py
+-rw-r--r--   0        0        0     5823 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/filters.py
+-rw-r--r--   0        0        0    11938 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/forms.py
+-rw-r--r--   0        0        0     3508 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/jobs.py
+-rw-r--r--   0        0        0     3452 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/migrations/0001_initial.py
+-rw-r--r--   0        0        0     5786 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/migrations/0002_required_unique_types_regex_context.py
+-rw-r--r--   0        0        0     2564 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/migrations/0003_datacompliance.py
+-rw-r--r--   0        0        0        0 2023-05-17 19:23:37.789689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/migrations/__init__.py
+-rw-r--r--   0        0        0    15526 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/models.py
+-rw-r--r--   0        0        0     4573 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/navigation.py
+-rw-r--r--   0        0        0     6299 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tables.py
+-rw-r--r--   0        0        0     1453 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/template_content.py
+-rw-r--r--   0        0        0     1396 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/datacompliance_retrieve.html
+-rw-r--r--   0        0        0      238 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/datacompliance_tab.html
+-rw-r--r--   0        0        0     1110 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/minmaxvalidationrule_retrieve.html
+-rw-r--r--   0        0        0     1204 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/regularexpressionvalidationrule_retrieve.html
+-rw-r--r--   0        0        0      907 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/requiredvalidationrule_retrieve.html
+-rw-r--r--   0        0        0     1017 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/uniquevalidationrule_retrieve.html
+-rw-r--r--   0        0        0       61 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/__init__.py
+-rw-r--r--   0        0        0     8124 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/test_api.py
+-rw-r--r--   0        0        0     1536 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/test_basic.py
+-rw-r--r--   0        0        0    13489 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/test_custom_validators.py
+-rw-r--r--   0        0        0     2587 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/test_data_compliance_rules.py
+-rw-r--r--   0        0        0     9131 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/test_filters.py
+-rw-r--r--   0        0        0    11014 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/test_models.py
+-rw-r--r--   0        0        0    11195 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/test_views.py
+-rw-r--r--   0        0        0     2835 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/urls.py
+-rw-r--r--   0        0        0     5178 2023-05-17 19:23:37.793689 nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/views.py
+-rw-r--r--   0        0        0     3700 2023-05-17 19:23:48.037544 nautobot_data_validation_engine-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5911 1970-01-01 00:00:00.000000 nautobot_data_validation_engine-2.1.0/PKG-INFO
```

### Comparing `nautobot_data_validation_engine-2.0.1/LICENSE` & `nautobot_data_validation_engine-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/README.md` & `nautobot_data_validation_engine-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/__init__.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,21 @@
     from importlib import metadata
 except ImportError:
     # Python version < 3.8
     import importlib_metadata as metadata
 
 __version__ = metadata.version(__name__)
 
-from nautobot.extras.plugins import PluginConfig
+import logging
+from nautobot.extras.plugins import NautobotAppConfig
 
+logger = logging.getLogger(__name__)
 
-class NautobotDataValidationEngineConfig(PluginConfig):
+
+class NautobotDataValidationEngineConfig(NautobotAppConfig):
     """Plugin configuration for the nautobot_data_validation_engine plugin."""
 
     name = "nautobot_data_validation_engine"
     verbose_name = "Data Validation Engine"
     version = __version__
     author = "Network to Code, LLC"
     description = "Provides UI to build custom data validation rules for data in Nautobot."
```

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/nested_serializers.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/serializers.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from rest_framework import serializers
 
 from nautobot.core.api import ContentTypeField
 from nautobot.extras.api.serializers import NautobotModelSerializer
 from nautobot.extras.utils import FeatureQuery
 
 from nautobot_data_validation_engine.models import (
+    DataCompliance,
     MinMaxValidationRule,
     RegularExpressionValidationRule,
     RequiredValidationRule,
     UniqueValidationRule,
 )
 
 # Not all of these variable(s) are not actually used anywhere in this file, but required for the
@@ -135,7 +136,17 @@
             "field",
             "max_instances",
             "enabled",
             "error_message",
             "created",
             "last_updated",
         ]
+
+
+class DataComplianceSerializer(NautobotModelSerializer):
+    """Serializer for DataCompliance."""
+
+    class Meta:
+        """Meta class for serializer."""
+
+        model = DataCompliance
+        fields = "__all__"
```

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/api/views.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/api/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,7 +42,14 @@
 
 class UniqueValidationRuleViewSet(NautobotModelViewSet):
     """View to manage min max expression validation rules."""
 
     queryset = models.UniqueValidationRule.objects.all()
     serializer_class = serializers.UniqueValidationRuleSerializer
     filterset_class = filters.UniqueValidationRuleFilterSet
+
+
+class DataComplianceAPIView(NautobotModelViewSet):
+    """API Views for DataCompliance."""
+
+    queryset = models.DataCompliance.objects.all()
+    serializer_class = serializers.DataComplianceSerializer
```

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/forms.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,22 @@
 from nautobot.utilities.forms import (
     BootstrapMixin,
     BulkEditForm,
     BulkEditNullBooleanSelect,
     CSVContentTypeField,
     CSVMultipleContentTypeField,
     CSVModelForm,
+    MultipleContentTypeField,
     SlugField,
+    StaticSelect2,
 )
+from nautobot.utilities.forms.constants import BOOLEAN_WITH_BLANK_CHOICES
 
 from nautobot_data_validation_engine.models import (
+    DataCompliance,
     MinMaxValidationRule,
     RegularExpressionValidationRule,
     RequiredValidationRule,
     UniqueValidationRule,
 )
 
 
@@ -357,7 +361,28 @@
     content_type = CSVMultipleContentTypeField(
         queryset=ContentType.objects.filter(FeatureQuery("custom_validators").get_query()).order_by(
             "app_label", "model"
         ),
         required=False,
     )
     max_instances = forms.IntegerField(required=False)
+
+
+#
+# DataCompliance
+#
+
+
+class DataComplianceFilterForm(BootstrapMixin, forms.Form):
+    """Form for DataCompliance instances."""
+
+    model = DataCompliance
+    compliance_class_name = forms.CharField(max_length=20, required=False)
+    validated_attribute = forms.CharField(max_length=20, required=False)
+    valid = forms.NullBooleanField(required=False, widget=StaticSelect2(choices=BOOLEAN_WITH_BLANK_CHOICES))
+    content_type = MultipleContentTypeField(
+        feature=None,
+        queryset=ContentType.objects.all().order_by("app_label", "model"),
+        choices_as_strings=True,
+        required=False,
+    )
+    q = forms.CharField(required=False, label="Search")
```

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/migrations/0001_initial.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/migrations/0002_required_unique_types_regex_context.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/migrations/0002_required_unique_types_regex_context.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/models.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Django models."""
 
 import re
 
 from django.contrib.contenttypes.models import ContentType
+from django.contrib.contenttypes.fields import GenericForeignKey
 from django.core.validators import MinValueValidator, ValidationError
 from django.db import models
 from django.shortcuts import reverse
 
 from nautobot.core.models.generics import PrimaryModel
 from nautobot.extras.utils import FeatureQuery, extras_features
 from nautobot.utilities.querysets import RestrictedQuerySet
@@ -362,7 +363,64 @@
         model_field = self.content_type.model_class()._meta.get_field(self.field)
 
         if self.field.startswith("_") or not model_field.editable or isinstance(model_field, blacklisted_field_types):
             raise ValidationError({"field": "This field's type does not support uniqueness validation."})
 
         if getattr(model_field, "unique", False):
             raise ValidationError({"field": "This field is already unique by default."})
+
+
+class DataCompliance(PrimaryModel):
+    """Model to represent the results of an audit method."""
+
+    compliance_class_name = models.CharField(max_length=100, blank=False, null=False)
+    last_validation_date = models.DateTimeField(blank=False, null=False, auto_now=True)
+    content_type = models.ForeignKey(ContentType, on_delete=models.PROTECT, blank=False, null=False)
+    object_id = models.CharField(max_length=200, blank=False, null=False)
+    validated_object = GenericForeignKey("content_type", "object_id")
+    validated_object_str = models.CharField(max_length=200, blank=True, null=True)
+    validated_attribute = models.CharField(max_length=100, blank=True, null=True)
+    validated_attribute_value = models.CharField(max_length=200, blank=True, null=True)
+    valid = models.BooleanField(blank=False, null=False)
+    message = models.TextField(blank=True, null=True)
+
+    csv_headers = [
+        "compliance_class_name",
+        "last_validation_date",
+        "validated_object",
+        "validated_attribute",
+        "validated_attribute_value",
+        "valid",
+        "message",
+    ]
+
+    class Meta:
+        """Meta class for Audit model."""
+
+        verbose_name_plural = "Data Compliance"
+
+        unique_together = (
+            "compliance_class_name",
+            "content_type",
+            "object_id",
+            "validated_attribute",
+        )
+
+    def to_csv(self):
+        """Return a tuple of data that should be exported to CSV."""
+        return (
+            self.compliance_class_name,
+            self.last_validation_date,
+            self.validated_object,
+            self.validated_attribute,
+            self.validated_attribute_value,
+            self.valid,
+            self.message,
+        )
+
+    def __str__(self):
+        """Return a string representation of this DataCompliance object."""
+        return f"{self.compliance_class_name}: {self.validated_attribute} compliance for {self.validated_object}"
+
+    def get_absolute_url(self):
+        """Return the absolute URL to this Audit object."""
+        return reverse("plugins:nautobot_data_validation_engine:datacompliance", args=[self.pk])
```

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/navigation.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/navigation.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,12 +67,18 @@
                             ),
                             NavMenuImportButton(
                                 link="plugins:nautobot_data_validation_engine:uniquevalidationrule_import",
                                 permissions=["nautobot_data_validation_engine.add_uniquevalidationrule"],
                             ),
                         ),
                     ),
+                    NavMenuItem(
+                        link="plugins:nautobot_data_validation_engine:datacompliance_list",
+                        name="Data Compliance",
+                        permissions=["nautobot_data_validation_engine.view_datacompliance"],
+                        buttons=(),
+                    ),
                 ),
             ),
         ),
     ),
 )
```

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/minmaxvalidationrule_retrieve.html` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/minmaxvalidationrule_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/regularexpressionvalidationrule_retrieve.html` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/regularexpressionvalidationrule_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/requiredvalidationrule_retrieve.html` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/requiredvalidationrule_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/uniquevalidationrule_retrieve.html` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/templates/nautobot_data_validation_engine/uniquevalidationrule_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_api.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_basic.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_custom_validators.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/test_custom_validators.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_filters.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/tests/test_models.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_data_validation_engine-2.0.1/nautobot_data_validation_engine/urls.py` & `nautobot_data_validation_engine-2.1.0/nautobot_data_validation_engine/urls.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,22 +5,39 @@
 from nautobot.core.views.routers import NautobotUIViewSetRouter
 from nautobot.extras.views import ObjectChangeLogView, ObjectNotesView
 
 from nautobot_data_validation_engine import views, models
 
 
 router = NautobotUIViewSetRouter()
+router.register("data-compliance", views.DataComplianceListView)
 router.register("regex-rules", views.RegularExpressionValidationRuleUIViewSet)
 router.register("min-max-rules", views.MinMaxValidationRuleUIViewSet)
 router.register("required-rules", views.RequiredValidationRuleUIViewSet)
 router.register("unique-rules", views.UniqueValidationRuleUIViewSet)
 
-
 urlpatterns = [
     path(
+        "data-compliance/<uuid:pk>/changelog/",
+        ObjectChangeLogView.as_view(),
+        name="datacompliance_changelog",
+        kwargs={"model": models.DataCompliance},
+    ),
+    path(
+        "data-compliance/<uuid:pk>/notes/",
+        ObjectNotesView.as_view(),
+        name="datacompliance_notes",
+        kwargs={"model": models.DataCompliance},
+    ),
+    path(
+        "data-compliance/<model>/<uuid:id>/",
+        views.DataComplianceObjectView.as_view(),
+        name="data-compliance-tab",
+    ),
+    path(
         "regex-rules/<uuid:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="regularexpressionvalidationrule_changelog",
         kwargs={"model": models.RegularExpressionValidationRule},
     ),
     path(
         "regex-rules/<uuid:pk>/notes/",
```

### Comparing `nautobot_data_validation_engine-2.0.1/pyproject.toml` & `nautobot_data_validation_engine-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-data-validation-engine"
-version = "v2.0.1"
+version = "v2.1.0"
 description = "Provides UI to build custom data validation rules for data in Nautobot"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-data-validation-engine"
 repository = "https://github.com/nautobot/nautobot-plugin-data-validation-engine"
 keywords = ["nautobot", "nautobot-plugin", "data", "validation", "django"]
```

### Comparing `nautobot_data_validation_engine-2.0.1/PKG-INFO` & `nautobot_data_validation_engine-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-data-validation-engine
-Version: 2.0.1
+Version: 2.1.0
 Summary: Provides UI to build custom data validation rules for data in Nautobot
 Home-page: https://github.com/nautobot/nautobot-plugin-data-validation-engine
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin,data,validation,django
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nautobot-data-validation-engine Version: 2.0.1
+Metadata-Version: 2.1 Name: nautobot-data-validation-engine Version: 2.1.0
 Summary: Provides UI to build custom data validation rules for data in Nautobot
 Home-page: https://github.com/nautobot/nautobot-plugin-data-validation-engine
 License: Apache-2.0 Keywords: nautobot,nautobot-plugin,data,validation,django
 Author: Network to Code, LLC Author-email: info@networktocode.com Requires-
 Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

