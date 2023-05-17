# Comparing `tmp/pulumi_opsgenie-1.3.0a1684216670.tar.gz` & `tmp/pulumi_opsgenie-1.3.0a1684331251.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opsgenie-1.3.0a1684216670.tar", last modified: Tue May 16 06:03:33 2023, max compression
+gzip compressed data, was "pulumi_opsgenie-1.3.0a1684331251.tar", last modified: Wed May 17 13:51:55 2023, max compression
```

## Comparing `pulumi_opsgenie-1.3.0a1684216670.tar` & `pulumi_opsgenie-1.3.0a1684331251.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:33.441231 pulumi_opsgenie-1.3.0a1684216670/
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-16 06:03:33.441231 pulumi_opsgenie-1.3.0a1684216670/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:33.441231 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179290 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    57892 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/alert_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    32958 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/api_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:33.441231 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/custom_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/email_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/escalation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_escalation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/incident_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    26894 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/integration_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    34667 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)   159991 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25289 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/schedule_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/service_incident_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/team_routing_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    26257 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/user_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:33.441231 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 06:03:33.441231 pulumi_opsgenie-1.3.0a1684216670/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:55.783903 pulumi_opsgenie-1.3.0a1684331251/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-17 13:51:55.783903 pulumi_opsgenie-1.3.0a1684331251/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:55.783903 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179600 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57892 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/alert_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33460 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/api_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:55.783903 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/custom_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23692 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/email_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/escalation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/get_escalation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/get_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/get_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/incident_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27020 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/integration_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34667 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160301 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25415 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/schedule_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/service_incident_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/team_routing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26257 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/user_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:51:55.783903 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:51:55.783903 pulumi_opsgenie-1.3.0a1684331251/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-17 13:51:55.000000 pulumi_opsgenie-1.3.0a1684331251/setup.py
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/PKG-INFO` & `pulumi_opsgenie-1.3.0a1684331251/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_opsgenie
-Version: 1.3.0a1684216670
+Version: 1.3.0a1684331251
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi opsgenie
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-opsgenie/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-opsgenie/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fopsgenie.svg)](https://npmjs.com/package/@pulumi/opsgenie)
 [![NuGet version](https://badge.fury.io/nu/pulumi.opsgenie.svg)](https://badge.fury.io/nu/pulumi.opsgenie)
 [![Python version](https://badge.fury.io/py/pulumi-opsgenie.svg)](https://pypi.org/project/pulumi-opsgenie)
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/README.md` & `pulumi_opsgenie-1.3.0a1684331251/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/__init__.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/_inputs.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -3627,14 +3627,16 @@
                  start_day: pulumi.Input[str],
                  start_hour: pulumi.Input[int],
                  start_min: pulumi.Input[int]):
         """
         :param pulumi.Input[str] end_day: Value of the day that frame will end.
         :param pulumi.Input[int] end_hour: Value of the hour that frame will end.
         :param pulumi.Input[int] end_min: Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+               
+               Both `start_day` and `end_day` can assume only `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday` values.
         :param pulumi.Input[str] start_day: Value of the day that frame will start.
         :param pulumi.Input[int] start_hour: Value of the hour that frame will start
         :param pulumi.Input[int] start_min: Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
         """
         pulumi.set(__self__, "end_day", end_day)
         pulumi.set(__self__, "end_hour", end_hour)
         pulumi.set(__self__, "end_min", end_min)
@@ -3667,14 +3669,16 @@
         pulumi.set(self, "end_hour", value)
 
     @property
     @pulumi.getter(name="endMin")
     def end_min(self) -> pulumi.Input[int]:
         """
         Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+
+        Both `start_day` and `end_day` can assume only `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday` values.
         """
         return pulumi.get(self, "end_min")
 
     @end_min.setter
     def end_min(self, value: pulumi.Input[int]):
         pulumi.set(self, "end_min", value)
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/_utilities.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/alert_policy.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/alert_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/api_integration.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/api_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -383,37 +383,37 @@
         import pulumi_opsgenie as opsgenie
 
         example_api_integration_api_integration = opsgenie.ApiIntegration("example-api-integrationApiIntegration",
             type="API",
             responders=[
                 opsgenie.ApiIntegrationResponderArgs(
                     type="user",
-                    id=opsgenie_user["user"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 ),
                 opsgenie.ApiIntegrationResponderArgs(
                     type="user",
-                    id=opsgenie_user["fahri"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 ),
             ])
         example_api_integration_index_api_integration_api_integration = opsgenie.ApiIntegration("example-api-integrationIndex/apiIntegrationApiIntegration",
             type="Prometheus",
             responders=[opsgenie.ApiIntegrationResponderArgs(
                 type="user",
-                id=opsgenie_user["user"]["id"],
+                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
             )],
             enabled=False,
             allow_write_access=False,
             ignore_responders_from_payload=True,
             suppress_notifications=True,
             owner_team_id=opsgenie_team["team"]["id"])
         test3 = opsgenie.ApiIntegration("test3",
             type="Webhook",
             responders=[opsgenie.ApiIntegrationResponderArgs(
                 type="user",
-                id=opsgenie_user["user"]["id"],
+                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
             )],
             enabled=False,
             allow_write_access=False,
             suppress_notifications=True,
             webhook_url="https://api.example.com/v1",
             headers={
                 "header1": value1,
@@ -456,37 +456,37 @@
         import pulumi_opsgenie as opsgenie
 
         example_api_integration_api_integration = opsgenie.ApiIntegration("example-api-integrationApiIntegration",
             type="API",
             responders=[
                 opsgenie.ApiIntegrationResponderArgs(
                     type="user",
-                    id=opsgenie_user["user"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 ),
                 opsgenie.ApiIntegrationResponderArgs(
                     type="user",
-                    id=opsgenie_user["fahri"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 ),
             ])
         example_api_integration_index_api_integration_api_integration = opsgenie.ApiIntegration("example-api-integrationIndex/apiIntegrationApiIntegration",
             type="Prometheus",
             responders=[opsgenie.ApiIntegrationResponderArgs(
                 type="user",
-                id=opsgenie_user["user"]["id"],
+                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
             )],
             enabled=False,
             allow_write_access=False,
             ignore_responders_from_payload=True,
             suppress_notifications=True,
             owner_team_id=opsgenie_team["team"]["id"])
         test3 = opsgenie.ApiIntegration("test3",
             type="Webhook",
             responders=[opsgenie.ApiIntegrationResponderArgs(
                 type="user",
-                id=opsgenie_user["user"]["id"],
+                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
             )],
             enabled=False,
             allow_write_access=False,
             suppress_notifications=True,
             webhook_url="https://api.example.com/v1",
             headers={
                 "header1": value1,
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/config/vars.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/custom_role.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/custom_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/email_integration.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/email_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -267,37 +267,37 @@
         import pulumi_opsgenie as opsgenie
 
         test_email_integration = opsgenie.EmailIntegration("testEmailIntegration", email_username="fahri")
         test_index_email_integration_email_integration = opsgenie.EmailIntegration("testIndex/emailIntegrationEmailIntegration",
             responders=[
                 opsgenie.EmailIntegrationResponderArgs(
                     type="user",
-                    id=opsgenie_user["test"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 ),
                 opsgenie.EmailIntegrationResponderArgs(
                     type="schedule",
-                    id=opsgenie_schedule["test"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 ),
                 opsgenie.EmailIntegrationResponderArgs(
                     type="escalation",
-                    id=opsgenie_escalation["test"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 ),
                 opsgenie.EmailIntegrationResponderArgs(
                     type="team",
-                    id=opsgenie_team["test2"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 ),
             ],
             email_username="test",
             enabled=True,
             ignore_responders_from_payload=True,
             suppress_notifications=True)
         test_opsgenie_index_email_integration_email_integration = opsgenie.EmailIntegration("testOpsgenieIndex/emailIntegrationEmailIntegration",
             responders=[opsgenie.EmailIntegrationResponderArgs(
                 type="user",
-                id=opsgenie_user["test"]["id"],
+                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
             )],
             email_username="test",
             enabled=True,
             ignore_responders_from_payload=True,
             suppress_notifications=True,
             owner_team_id=opsgenie_team_genies["id"])
         ```
@@ -335,37 +335,37 @@
         import pulumi_opsgenie as opsgenie
 
         test_email_integration = opsgenie.EmailIntegration("testEmailIntegration", email_username="fahri")
         test_index_email_integration_email_integration = opsgenie.EmailIntegration("testIndex/emailIntegrationEmailIntegration",
             responders=[
                 opsgenie.EmailIntegrationResponderArgs(
                     type="user",
-                    id=opsgenie_user["test"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 ),
                 opsgenie.EmailIntegrationResponderArgs(
                     type="schedule",
-                    id=opsgenie_schedule["test"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 ),
                 opsgenie.EmailIntegrationResponderArgs(
                     type="escalation",
-                    id=opsgenie_escalation["test"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 ),
                 opsgenie.EmailIntegrationResponderArgs(
                     type="team",
-                    id=opsgenie_team["test2"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 ),
             ],
             email_username="test",
             enabled=True,
             ignore_responders_from_payload=True,
             suppress_notifications=True)
         test_opsgenie_index_email_integration_email_integration = opsgenie.EmailIntegration("testOpsgenieIndex/emailIntegrationEmailIntegration",
             responders=[opsgenie.EmailIntegrationResponderArgs(
                 type="user",
-                id=opsgenie_user["test"]["id"],
+                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
             )],
             email_username="test",
             enabled=True,
             ignore_responders_from_payload=True,
             suppress_notifications=True,
             owner_team_id=opsgenie_team_genies["id"])
         ```
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/escalation.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/escalation.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,23 +219,23 @@
             )],
             rules=[opsgenie.EscalationRuleArgs(
                 condition="if-not-acked",
                 delay=1,
                 notify_type="default",
                 recipients=[
                     opsgenie.EscalationRuleRecipientArgs(
-                        id=opsgenie_user["test"]["id"],
+                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                         type="user",
                     ),
                     opsgenie.EscalationRuleRecipientArgs(
-                        id=opsgenie_team["test"]["id"],
+                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                         type="team",
                     ),
                     opsgenie.EscalationRuleRecipientArgs(
-                        id=opsgenie_schedule["test"]["id"],
+                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                         type="schedule",
                     ),
                 ],
             )])
         ```
 
         ## Import
@@ -280,23 +280,23 @@
             )],
             rules=[opsgenie.EscalationRuleArgs(
                 condition="if-not-acked",
                 delay=1,
                 notify_type="default",
                 recipients=[
                     opsgenie.EscalationRuleRecipientArgs(
-                        id=opsgenie_user["test"]["id"],
+                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                         type="user",
                     ),
                     opsgenie.EscalationRuleRecipientArgs(
-                        id=opsgenie_team["test"]["id"],
+                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                         type="team",
                     ),
                     opsgenie.EscalationRuleRecipientArgs(
-                        id=opsgenie_schedule["test"]["id"],
+                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                         type="schedule",
                     ),
                 ],
             )])
         ```
 
         ## Import
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_escalation.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/get_escalation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_heartbeat.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/get_heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_schedule.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/get_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_service.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/get_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,16 @@
 
     this = opsgenie.get_service(name="Payment")
     ```
 
 
     :param str description: Description field of the service that is generally used to provide a detailed information about the service.
     :param str name: Name of the service. This field must not be longer than 100 characters.
+           
+           The following attributes are exported:
     :param str team_id: Team id of the service.
     """
     __args__ = dict()
     __args__['description'] = description
     __args__['name'] = name
     __args__['teamId'] = team_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -122,10 +124,12 @@
 
     this = opsgenie.get_service(name="Payment")
     ```
 
 
     :param str description: Description field of the service that is generally used to provide a detailed information about the service.
     :param str name: Name of the service. This field must not be longer than 100 characters.
+           
+           The following attributes are exported:
     :param str team_id: Team id of the service.
     """
     ...
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_team.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/get_team.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,14 +89,16 @@
     sre_team = opsgenie.get_team(name="sre-team")
     ```
 
 
     :param str description: A description for this team.
     :param Sequence[pulumi.InputType['GetTeamMemberArgs']] members: A Member block as documented below.
     :param str name: The name associated with this team. Opsgenie defines that this must not be longer than 100 characters.
+           
+           The following attributes are exported:
     """
     __args__ = dict()
     __args__['description'] = description
     __args__['members'] = members
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('opsgenie:index/getTeam:getTeam', __args__, opts=opts, typ=GetTeamResult).value
@@ -125,9 +127,11 @@
     sre_team = opsgenie.get_team(name="sre-team")
     ```
 
 
     :param str description: A description for this team.
     :param Sequence[pulumi.InputType['GetTeamMemberArgs']] members: A Member block as documented below.
     :param str name: The name associated with this team. Opsgenie defines that this must not be longer than 100 characters.
+           
+           The following attributes are exported:
     """
     ...
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_user.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/heartbeat.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/incident_template.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/incident_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/integration_action.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/integration_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
                         conditions=[opsgenie.IntegrationActionCreateFilterConditionArgs(
                             field="priority",
                             operation="equals",
                             expected_value="P1",
                         )],
                     )],
                     responders=[opsgenie.IntegrationActionCreateResponderArgs(
-                        id=opsgenie_team["test"]["id"],
+                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                         type="team",
                     )],
                 ),
                 opsgenie.IntegrationActionCreateArgs(
                     name="Create medium priority alerts",
                     tags=[
                         "SEVERE",
@@ -383,15 +383,15 @@
                         conditions=[opsgenie.IntegrationActionCreateFilterConditionArgs(
                             field="priority",
                             operation="equals",
                             expected_value="P1",
                         )],
                     )],
                     responders=[opsgenie.IntegrationActionCreateResponderArgs(
-                        id=opsgenie_team["test"]["id"],
+                        id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                         type="team",
                     )],
                 ),
                 opsgenie.IntegrationActionCreateArgs(
                     name="Create medium priority alerts",
                     tags=[
                         "SEVERE",
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/maintenance.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/maintenance.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Maintenance("test",
             description="geniemaintenance-%s",
             rules=[opsgenie.MaintenanceRuleArgs(
                 entities=[opsgenie.MaintenanceRuleEntityArgs(
-                    id=opsgenie_email_integration["test"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     type="integration",
                 )],
                 state="enabled",
             )],
             times=[opsgenie.MaintenanceTimeArgs(
                 end_date="2019-06-%dT17:50:00Z",
                 start_date="2019-06-20T17:45:00Z",
@@ -186,15 +186,15 @@
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Maintenance("test",
             description="geniemaintenance-%s",
             rules=[opsgenie.MaintenanceRuleArgs(
                 entities=[opsgenie.MaintenanceRuleEntityArgs(
-                    id=opsgenie_email_integration["test"]["id"],
+                    id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     type="integration",
                 )],
                 state="enabled",
             )],
             times=[opsgenie.MaintenanceTimeArgs(
                 end_date="2019-06-%dT17:50:00Z",
                 start_date="2019-06-20T17:45:00Z",
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/notification_policy.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/notification_rule.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/notification_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/outputs.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3411,14 +3411,16 @@
                  start_day: str,
                  start_hour: int,
                  start_min: int):
         """
         :param str end_day: Value of the day that frame will end.
         :param int end_hour: Value of the hour that frame will end.
         :param int end_min: Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+               
+               Both `start_day` and `end_day` can assume only `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday` values.
         :param str start_day: Value of the day that frame will start.
         :param int start_hour: Value of the hour that frame will start
         :param int start_min: Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
         """
         pulumi.set(__self__, "end_day", end_day)
         pulumi.set(__self__, "end_hour", end_hour)
         pulumi.set(__self__, "end_min", end_min)
@@ -3443,14 +3445,16 @@
         return pulumi.get(self, "end_hour")
 
     @property
     @pulumi.getter(name="endMin")
     def end_min(self) -> int:
         """
         Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
+
+        Both `start_day` and `end_day` can assume only `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday` values.
         """
         return pulumi.get(self, "end_min")
 
     @property
     @pulumi.getter(name="startDay")
     def start_day(self) -> str:
         """
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/provider.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/schedule.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/schedule_rotation.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/schedule_rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.ScheduleRotation("test",
             end_date="2019-06-20T17:30:00Z",
             length=6,
             participants=[opsgenie.ScheduleRotationParticipantArgs(
-                id=opsgenie_user["test"]["id"],
+                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 type="user",
             )],
             schedule_id=opsgenie_schedule["test"]["id"],
             start_date="2019-06-18T17:00:00Z",
             time_restrictions=[opsgenie.ScheduleRotationTimeRestrictionArgs(
                 restriction=[opsgenie.ScheduleRotationTimeRestrictionRestrictionArgs(
                     end_hour=10,
@@ -350,15 +350,15 @@
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.ScheduleRotation("test",
             end_date="2019-06-20T17:30:00Z",
             length=6,
             participants=[opsgenie.ScheduleRotationParticipantArgs(
-                id=opsgenie_user["test"]["id"],
+                id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                 type="user",
             )],
             schedule_id=opsgenie_schedule["test"]["id"],
             start_date="2019-06-18T17:00:00Z",
             time_restrictions=[opsgenie.ScheduleRotationTimeRestrictionArgs(
                 restriction=[opsgenie.ScheduleRotationTimeRestrictionRestrictionArgs(
                     end_hour=10,
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/service.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/service_incident_rule.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/service_incident_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/team.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/team_routing_rule.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/team_routing_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/user.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/user_contact.py` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie/user_contact.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/PKG-INFO` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-opsgenie
-Version: 1.3.0a1684216670
+Version: 1.3.0a1684331251
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi opsgenie
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-opsgenie/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-opsgenie/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fopsgenie.svg)](https://npmjs.com/package/@pulumi/opsgenie)
 [![NuGet version](https://badge.fury.io/nu/pulumi.opsgenie.svg)](https://badge.fury.io/nu/pulumi.opsgenie)
 [![Python version](https://badge.fury.io/py/pulumi-opsgenie.svg)](https://pypi.org/project/pulumi-opsgenie)
```

### Comparing `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/SOURCES.txt` & `pulumi_opsgenie-1.3.0a1684331251/pulumi_opsgenie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1684216670/setup.py` & `pulumi_opsgenie-1.3.0a1684331251/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.3.0a1684216670"
-PLUGIN_VERSION = "1.3.0-alpha.1684216670+113c1638"
+VERSION = "1.3.0a1684331251"
+PLUGIN_VERSION = "1.3.0-alpha.1684331251+ec22fa69"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opsgenie', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "opsgenie Pulumi Package - Development Version"
 
 
 setup(name='pulumi_opsgenie',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing opsgenie cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

