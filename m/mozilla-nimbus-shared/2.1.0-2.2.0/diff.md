# Comparing `tmp/mozilla_nimbus_shared-2.1.0.tar.gz` & `tmp/mozilla_nimbus_shared-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla_nimbus_shared-2.1.0.tar", max compression
+gzip compressed data, was "mozilla_nimbus_shared-2.2.0.tar", max compression
```

## Comparing `mozilla_nimbus_shared-2.1.0.tar` & `mozilla_nimbus_shared-2.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      628 2022-06-16 17:41:54.490623 mozilla_nimbus_shared-2.1.0/README.md
--rw-r--r--   0        0        0     1660 2022-06-16 17:38:10.474193 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/__init__.py
--rw-r--r--   0        0        0    27260 2023-04-19 19:47:10.411062 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/data.json
--rw-r--r--   0        0        0    13449 2023-04-19 19:47:10.414966 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/experiments/NimbusExperiment.json
--rw-r--r--   0        0        0     2559 2023-04-19 19:47:10.415194 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/features/Feature.json
--rw-r--r--   0        0        0    25972 2022-06-16 17:43:18.606633 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/messaging/SimpleCFRMessage.json
--rw-r--r--   0        0        0     9789 2022-06-16 17:43:18.606730 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/messaging/SpecialMessageActionSchemas.json
--rw-r--r--   0        0        0     4368 2022-06-16 17:43:18.606822 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/messaging/TriggerActionSchemas.json
--rw-r--r--   0        0        0      493 2023-04-19 19:47:10.416449 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/AddonRollbackArguments.json
--rw-r--r--   0        0        0      689 2023-04-19 19:47:10.415992 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/AddonRolloutArguments.json
--rw-r--r--   0        0        0     2015 2023-04-19 19:47:10.416322 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/BranchedAddonStudyArguments.json
--rw-r--r--   0        0        0      434 2023-04-19 19:47:10.415427 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/ConsoleLogArguments.json
--rw-r--r--   0        0        0     2528 2023-04-19 19:47:10.416210 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/MessagingExperimentArguments.json
--rw-r--r--   0        0        0     4064 2023-04-19 19:47:10.416561 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/MultiPreferenceExperimentArguments.json
--rw-r--r--   0        0        0    18244 2023-04-19 19:47:10.415881 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/NormandyRecipe.json
--rw-r--r--   0        0        0     1149 2023-04-19 19:47:10.416666 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/OptOutStudyArguments.json
--rw-r--r--   0        0        0     3038 2023-04-19 19:47:10.415646 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/PreferenceExperimentArguments.json
--rw-r--r--   0        0        0      467 2023-04-19 19:47:10.415539 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRollbackArguments.json
--rw-r--r--   0        0        0     1280 2023-04-19 19:47:10.416097 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRolloutArguments.json
--rw-r--r--   0        0        0     2077 2023-04-19 19:47:10.415756 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/ShowHeartbeatArguments.json
--rw-r--r--   0        0        0    13302 2023-03-08 17:02:15.454267 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/experiments/NimbusExperiment.json
--rw-r--r--   0        0        0     2559 2023-03-08 17:02:15.454465 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/features/Feature.json
--rw-r--r--   0        0        0      493 2023-03-08 17:02:15.455590 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRollbackArguments.json
--rw-r--r--   0        0        0      689 2023-03-08 17:02:15.455191 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRolloutArguments.json
--rw-r--r--   0        0        0     2015 2023-03-08 17:02:15.455491 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/BranchedAddonStudyArguments.json
--rw-r--r--   0        0        0      434 2023-03-08 17:02:15.454671 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/ConsoleLogArguments.json
--rw-r--r--   0        0        0     2528 2023-03-08 17:02:15.455393 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/MessagingExperimentArguments.json
--rw-r--r--   0        0        0     4064 2023-03-08 17:02:15.455693 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/MultiPreferenceExperimentArguments.json
--rw-r--r--   0        0        0    18244 2023-03-08 17:02:15.455095 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/NormandyRecipe.json
--rw-r--r--   0        0        0     1149 2023-03-08 17:02:15.455786 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/OptOutStudyArguments.json
--rw-r--r--   0        0        0     3038 2023-03-08 17:02:15.454883 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceExperimentArguments.json
--rw-r--r--   0        0        0      467 2023-03-08 17:02:15.454780 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRollbackArguments.json
--rw-r--r--   0        0        0     1280 2023-03-08 17:02:15.455291 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRolloutArguments.json
--rw-r--r--   0        0        0     2077 2023-03-08 17:02:15.454991 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/ShowHeartbeatArguments.json
--rw-r--r--   0        0        0      736 2023-03-08 17:02:15.454067 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/targeting/Audience.json
--rw-r--r--   0        0        0      449 2023-03-08 17:02:15.453853 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/test/FoodColors.json
--rw-r--r--   0        0        0      736 2023-04-19 19:47:10.414726 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/targeting/Audience.json
--rw-r--r--   0        0        0      449 2023-04-19 19:47:10.413024 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/test/FoodColors.json
--rw-r--r--   0        0        0      999 2022-06-16 17:38:10.474263 mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/test.py
--rw-r--r--   0        0        0      524 2023-04-19 19:47:10.403971 mozilla_nimbus_shared-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 mozilla_nimbus_shared-2.1.0/setup.py
--rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 mozilla_nimbus_shared-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      628 2022-06-16 17:41:54.490623 mozilla_nimbus_shared-2.2.0/README.md
+-rw-r--r--   0        0        0     1660 2022-06-16 17:38:10.474193 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/__init__.py
+-rw-r--r--   0        0        0    29846 2023-05-17 18:08:57.000088 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/data.json
+-rw-r--r--   0        0        0    13910 2023-05-17 18:09:38.991999 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/experiments/NimbusExperiment.json
+-rw-r--r--   0        0        0     2559 2023-05-17 18:09:38.992208 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/features/Feature.json
+-rw-r--r--   0        0        0    25972 2022-06-16 17:43:18.606633 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/messaging/SimpleCFRMessage.json
+-rw-r--r--   0        0        0     9789 2022-06-16 17:43:18.606730 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/messaging/SpecialMessageActionSchemas.json
+-rw-r--r--   0        0        0     4368 2022-06-16 17:43:18.606822 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/messaging/TriggerActionSchemas.json
+-rw-r--r--   0        0        0      493 2023-05-17 18:09:38.993350 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/AddonRollbackArguments.json
+-rw-r--r--   0        0        0      689 2023-05-17 18:09:38.992946 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/AddonRolloutArguments.json
+-rw-r--r--   0        0        0     2015 2023-05-17 18:09:38.993253 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/BranchedAddonStudyArguments.json
+-rw-r--r--   0        0        0      434 2023-05-17 18:09:38.992411 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/ConsoleLogArguments.json
+-rw-r--r--   0        0        0     2528 2023-05-17 18:09:38.993151 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/MessagingExperimentArguments.json
+-rw-r--r--   0        0        0     4094 2023-05-17 18:09:38.993450 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/MultiPreferenceExperimentArguments.json
+-rw-r--r--   0        0        0    18274 2023-05-17 18:09:38.992838 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/NormandyRecipe.json
+-rw-r--r--   0        0        0     1149 2023-05-17 18:09:38.993555 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/OptOutStudyArguments.json
+-rw-r--r--   0        0        0     3038 2023-05-17 18:09:38.992622 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/PreferenceExperimentArguments.json
+-rw-r--r--   0        0        0      467 2023-05-17 18:09:38.992515 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRollbackArguments.json
+-rw-r--r--   0        0        0     1280 2023-05-17 18:09:38.993048 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRolloutArguments.json
+-rw-r--r--   0        0        0     2077 2023-05-17 18:09:38.992722 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/ShowHeartbeatArguments.json
+-rw-r--r--   0        0        0    13302 2023-03-08 17:02:15.454267 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/experiments/NimbusExperiment.json
+-rw-r--r--   0        0        0     2559 2023-03-08 17:02:15.454465 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/features/Feature.json
+-rw-r--r--   0        0        0      493 2023-03-08 17:02:15.455590 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRollbackArguments.json
+-rw-r--r--   0        0        0      689 2023-03-08 17:02:15.455191 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRolloutArguments.json
+-rw-r--r--   0        0        0     2015 2023-03-08 17:02:15.455491 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/BranchedAddonStudyArguments.json
+-rw-r--r--   0        0        0      434 2023-03-08 17:02:15.454671 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/ConsoleLogArguments.json
+-rw-r--r--   0        0        0     2528 2023-03-08 17:02:15.455393 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/MessagingExperimentArguments.json
+-rw-r--r--   0        0        0     4064 2023-03-08 17:02:15.455693 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/MultiPreferenceExperimentArguments.json
+-rw-r--r--   0        0        0    18244 2023-03-08 17:02:15.455095 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/NormandyRecipe.json
+-rw-r--r--   0        0        0     1149 2023-03-08 17:02:15.455786 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/OptOutStudyArguments.json
+-rw-r--r--   0        0        0     3038 2023-03-08 17:02:15.454883 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceExperimentArguments.json
+-rw-r--r--   0        0        0      467 2023-03-08 17:02:15.454780 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRollbackArguments.json
+-rw-r--r--   0        0        0     1280 2023-03-08 17:02:15.455291 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRolloutArguments.json
+-rw-r--r--   0        0        0     2077 2023-03-08 17:02:15.454991 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/ShowHeartbeatArguments.json
+-rw-r--r--   0        0        0      736 2023-03-08 17:02:15.454067 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/targeting/Audience.json
+-rw-r--r--   0        0        0      449 2023-03-08 17:02:15.453853 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/test/FoodColors.json
+-rw-r--r--   0        0        0      736 2023-05-17 18:09:38.991791 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/targeting/Audience.json
+-rw-r--r--   0        0        0      449 2023-05-17 18:09:38.991560 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/test/FoodColors.json
+-rw-r--r--   0        0        0      999 2022-06-16 17:38:10.474263 mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/test.py
+-rw-r--r--   0        0        0      524 2023-05-17 18:09:38.985287 mozilla_nimbus_shared-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 mozilla_nimbus_shared-2.2.0/setup.py
+-rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 mozilla_nimbus_shared-2.2.0/PKG-INFO
```

### Comparing `mozilla_nimbus_shared-2.1.0/README.md` & `mozilla_nimbus_shared-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/__init__.py` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/data.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/data.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99%*

 * *Differences: {"'experiment-recipe-samples'": "{'desktop-115-locales': OrderedDict([('appId', "*

 * *                                "'firefox-desktop'), ('appName', 'firefox_desktop'), "*

 * *                                "('application', 'firefox-desktop'), ('arguments', OrderedDict()), "*

 * *                                "('branches', [OrderedDict([('feature', OrderedDict([('featureId', "*

 * *                                "'unused-feature-id-for-legacy-support'), ('enabled', False), "*

 * *                                "('value', Or […]*

```diff
@@ -311,14 +311,107 @@
             "schemaVersion": "1.7.1",
             "slug": "firefox-desktop-localization-test",
             "startDate": "2021-10-26",
             "targeting": "true",
             "userFacingDescription": "Test data for a localized experiment",
             "userFacingName": "MR2 Upgrade Spotlight Holdback"
         },
+        "desktop-115-locales": {
+            "appId": "firefox-desktop",
+            "appName": "firefox_desktop",
+            "application": "firefox-desktop",
+            "arguments": {},
+            "branches": [
+                {
+                    "feature": {
+                        "enabled": false,
+                        "featureId": "unused-feature-id-for-legacy-support",
+                        "value": {}
+                    },
+                    "features": [
+                        {
+                            "featureId": "nimbus-qa-1",
+                            "value": {
+                                "value": {
+                                    "$l10n": {
+                                        "comment": "Text for the control branch.",
+                                        "id": "control-text",
+                                        "text": "English text"
+                                    }
+                                }
+                            }
+                        }
+                    ],
+                    "ratio": 1,
+                    "slug": "control"
+                },
+                {
+                    "feature": {
+                        "enabled": false,
+                        "featureId": "unused-feature-id-for-legacy-support",
+                        "value": {}
+                    },
+                    "features": [
+                        {
+                            "featureId": "nimbus-qa-1",
+                            "value": {
+                                "value": {
+                                    "$l10n": {
+                                        "comment": "Text for the treatment branch.",
+                                        "id": "treatment-text",
+                                        "text": "More English text"
+                                    }
+                                }
+                            }
+                        }
+                    ],
+                    "ratio": 1,
+                    "slug": "treatment"
+                }
+            ],
+            "bucketConfig": {
+                "count": 10000,
+                "namespace": "firefox-desktop-localization-test",
+                "randomizationUnit": "normandy_id",
+                "start": 0,
+                "total": 10000
+            },
+            "channel": "nightly",
+            "endDate": null,
+            "featureIds": [
+                "nimbus-qa-1"
+            ],
+            "id": "firefox-desktop-localization-test",
+            "isEnrollmentPaused": false,
+            "locales": [
+                "en-US",
+                "fr"
+            ],
+            "localizations": {
+                "en-US": {
+                    "control-text": "English text",
+                    "treatment-test": "More English text"
+                },
+                "fr": {
+                    "control-text": "Texte en fran\u00e7ais",
+                    "treatment-text": "Plus de texte en fran\u00e7ais"
+                }
+            },
+            "outcomes": [],
+            "probeSets": [],
+            "proposedDuration": 63,
+            "proposedEnrollment": 7,
+            "referenceBranch": "control",
+            "schemaVersion": "1.7.1",
+            "slug": "firefox-desktop-localization-test",
+            "startDate": "2021-10-26",
+            "targeting": "true",
+            "userFacingDescription": "Test data for a localized experiment",
+            "userFacingName": "MR2 Upgrade Spotlight Holdback"
+        },
         "desktop-90": {
             "appId": "firefox-desktop",
             "appName": "firefox_desktop",
             "application": "firefox-desktop",
             "arguments": {},
             "branches": [
                 {
```

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/experiments/NimbusExperiment.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/experiments/NimbusExperiment.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998301630434782%*

 * *Differences: {"'definitions'": "{'NimbusExperiment': {'properties': {'localizations': {'type': 'object', "*

 * *                  "'additionalProperties': OrderedDict([('type', 'object'), "*

 * *                  "('additionalProperties', OrderedDict([('type', 'string')]))]), delete: "*

 * *                  "['anyOf']}}}}"}*

```diff
@@ -245,29 +245,22 @@
                     "type": "boolean"
                 },
                 "isRollout": {
                     "description": "When this property is set to true, treat this experiment as a rollout. Rollouts are currently handled as single-branch experiments separated from the bucketing namespace for normal experiments. See also: https://mozilla-hub.atlassian.net/browse/SDK-405",
                     "type": "boolean"
                 },
                 "localizations": {
-                    "anyOf": [
-                        {
-                            "additionalProperties": {
-                                "additionalProperties": {
-                                    "type": "string"
-                                },
-                                "type": "object"
-                            },
-                            "type": "object"
+                    "additionalProperties": {
+                        "additionalProperties": {
+                            "type": "string"
                         },
-                        {
-                            "type": "null"
-                        }
-                    ],
-                    "description": "Per-locale localization substitutions.\n\nThe top level key is the locale (e.g., \"en-US\" or \"fr\"). Each entry is a mapping of string IDs to their localized equivalents.\n\nOnly supported on desktop."
+                        "type": "object"
+                    },
+                    "description": "Per-locale localization substitutions.\n\nThe top level key is the locale (e.g., \"en-US\" or \"fr\"). Each entry is a mapping of string IDs to their localized equivalents.\n\nOnly supported on desktop.",
+                    "type": "object"
                 },
                 "outcomes": {
                     "description": "A list of outcomes relevant to the experiment analysis.",
                     "items": {
                         "properties": {
                             "priority": {
                                 "description": "e.g. \"primary\" or \"secondary\"",
```

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/features/Feature.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/features/Feature.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/messaging/SimpleCFRMessage.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/messaging/SimpleCFRMessage.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/messaging/SpecialMessageActionSchemas.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/messaging/SpecialMessageActionSchemas.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/messaging/TriggerActionSchemas.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/messaging/TriggerActionSchemas.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/AddonRolloutArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/AddonRolloutArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/BranchedAddonStudyArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/BranchedAddonStudyArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/MessagingExperimentArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/MessagingExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/MultiPreferenceExperimentArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/MultiPreferenceExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/NormandyRecipe.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/NormandyRecipe.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/OptOutStudyArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/OptOutStudyArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/PreferenceExperimentArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/PreferenceExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRolloutArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/PreferenceRolloutArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/normandy/ShowHeartbeatArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/ShowHeartbeatArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/experiments/NimbusExperiment.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/experiments/NimbusExperiment.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994032118055557%*

 * *Differences: {"'definitions'": "{'NimbusExperiment': {'properties': {'localizations': {'anyOf': "*

 * *                  "[OrderedDict([('type', 'object'), ('additionalProperties', "*

 * *                  "OrderedDict([('type', 'object'), ('additionalProperties', OrderedDict([('type', "*

 * *                  "'string')])), ('propertyNames', OrderedDict([('description', 'A string ID.'), "*

 * *                  "('pattern', '^[A-Za-z0-9\\\\-]+$'), ('minLength', 9)]))]))]), "*

 * *                  "OrderedDict([('type', 'null')])], delete: ['t […]*

```diff
@@ -244,23 +244,42 @@
                     "description": "When this property is set to true, the the SDK should not enroll new users into the experiment that have not already been enrolled.",
                     "type": "boolean"
                 },
                 "isRollout": {
                     "description": "When this property is set to true, treat this experiment as a rollout. Rollouts are currently handled as single-branch experiments separated from the bucketing namespace for normal experiments. See also: https://mozilla-hub.atlassian.net/browse/SDK-405",
                     "type": "boolean"
                 },
+                "locales": {
+                    "description": "The list of locale codes (e.g., \"en-US\" or \"fr\") that this experiment is targeting.\n\nIf null, all locales are targeted.",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
                 "localizations": {
-                    "additionalProperties": {
-                        "additionalProperties": {
-                            "type": "string"
+                    "anyOf": [
+                        {
+                            "additionalProperties": {
+                                "additionalProperties": {
+                                    "type": "string"
+                                },
+                                "propertyNames": {
+                                    "description": "A string ID.",
+                                    "minLength": 9,
+                                    "pattern": "^[A-Za-z0-9\\-]+$"
+                                },
+                                "type": "object"
+                            },
+                            "type": "object"
                         },
-                        "type": "object"
-                    },
-                    "description": "Per-locale localization substitutions.\n\nThe top level key is the locale (e.g., \"en-US\" or \"fr\"). Each entry is a mapping of string IDs to their localized equivalents.\n\nOnly supported on desktop.",
-                    "type": "object"
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "description": "Per-locale localization substitutions.\n\nThe top level key is the locale (e.g., \"en-US\" or \"fr\"). Each entry is a mapping of string IDs to their localized equivalents.\n\nOnly supported on desktop."
                 },
                 "outcomes": {
                     "description": "A list of outcomes relevant to the experiment analysis.",
                     "items": {
                         "properties": {
                             "priority": {
                                 "description": "e.g. \"primary\" or \"secondary\"",
```

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/features/Feature.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/features/Feature.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRolloutArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/AddonRolloutArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/BranchedAddonStudyArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/BranchedAddonStudyArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/MessagingExperimentArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/MessagingExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/MultiPreferenceExperimentArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/MultiPreferenceExperimentArguments.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999782986111111%*

 * *Differences: {"'definitions'": "{'MultiPreferenceExperimentArguments': {'properties': {'isHighVolume': "*

 * *                  "{'deprecated': True}}}}"}*

```diff
@@ -82,14 +82,15 @@
                 },
                 "isHighPopulation": {
                     "default": false,
                     "description": "Marks the preference experiment as a high population experiment, that should be excluded from certain types of telemetry.",
                     "type": "boolean"
                 },
                 "isHighVolume": {
+                    "deprecated": true,
                     "description": "Incorrect version of `isHighPopulation`. Included here for compatibility, but should not be used.",
                     "type": "boolean"
                 },
                 "slug": {
                     "description": "Unique identifier for this experiment",
                     "pattern": "^[A-Za-z0-9\\-_]+$",
                     "type": "string"
```

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/NormandyRecipe.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/normandy/NormandyRecipe.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999802714646465%*

 * *Differences: {"'definitions'": "{'MultiPreferenceExperimentArguments': {'properties': {'isHighVolume': "*

 * *                  "{'deprecated': True}}}}"}*

```diff
@@ -251,14 +251,15 @@
                 },
                 "isHighPopulation": {
                     "default": false,
                     "description": "Marks the preference experiment as a high population experiment, that should be excluded from certain types of telemetry.",
                     "type": "boolean"
                 },
                 "isHighVolume": {
+                    "deprecated": true,
                     "description": "Incorrect version of `isHighPopulation`. Included here for compatibility, but should not be used.",
                     "type": "boolean"
                 },
                 "slug": {
                     "description": "Unique identifier for this experiment",
                     "pattern": "^[A-Za-z0-9\\-_]+$",
                     "type": "string"
```

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/OptOutStudyArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/OptOutStudyArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceExperimentArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceExperimentArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRolloutArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/PreferenceRolloutArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/normandy/ShowHeartbeatArguments.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/normandy/ShowHeartbeatArguments.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/schemas/targeting/Audience.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/schemas/targeting/Audience.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/schemas/targeting/Audience.json` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/schemas/targeting/Audience.json`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/mozilla_nimbus_shared/test.py` & `mozilla_nimbus_shared-2.2.0/mozilla_nimbus_shared/test.py`

 * *Files identical despite different names*

### Comparing `mozilla_nimbus_shared-2.1.0/pyproject.toml` & `mozilla_nimbus_shared-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "mozilla_nimbus_shared"
 description = "Shared data and schemas for Project Nimbus"
 readme = "README.md"
 authors = ["Michael Cooper <mcooper@mozilla.com>"]
-version = "2.1.0"
+version = "2.2.0"
 license = "MPL-2.0"
 include = [
   "mozilla_nimbus_shared/schemas/**/*.json",
   "mozilla_nimbus_shared/data.json",
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `mozilla_nimbus_shared-2.1.0/setup.py` & `mozilla_nimbus_shared-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                            'schemas/test/*']}
 
 install_requires = \
 ['jsonschema>=4.17.3,<5.0.0']
 
 setup_kwargs = {
     'name': 'mozilla-nimbus-shared',
-    'version': '2.1.0',
+    'version': '2.2.0',
     'description': 'Shared data and schemas for Project Nimbus',
     'long_description': '# Nimbus Shared ![CircleCI](https://img.shields.io/circleci/build/github/mozilla/nimbus-shared) ![npm (scoped)](https://img.shields.io/npm/v/@mozilla/nimbus-shared)\n\nThis is a place to define data and schemas used across Project Nimbus.\n\nAny data that moves between systems should have TypeScript types defined here, which will be\nautomatically converted to JSON Schema. Any data that needs to be re-used by multiple systems should\nbe stored here to be shared.\n\nFor more information on the data and schemas included here, how to use them, and how to add to them,\nsee the documentation at https://mozilla.github.io/nimbus-shared\n',
     'author': 'Michael Cooper',
     'author_email': 'mcooper@mozilla.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mozilla_nimbus_shared-2.1.0/PKG-INFO` & `mozilla_nimbus_shared-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-nimbus-shared
-Version: 2.1.0
+Version: 2.2.0
 Summary: Shared data and schemas for Project Nimbus
 License: MPL-2.0
 Author: Michael Cooper
 Author-email: mcooper@mozilla.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

