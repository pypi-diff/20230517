# Comparing `tmp/microsoft-kiota-serialization-json-0.3.3.tar.gz` & `tmp/microsoft_kiota_serialization_json-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft-kiota-serialization-json-0.3.3.tar", last modified: Wed May 10 20:23:50 2023, max compression
+gzip compressed data, was "microsoft_kiota_serialization_json-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft-kiota-serialization-json-0.3.3.tar` & `microsoft_kiota_serialization_json-0.3.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       82 2023-05-10 20:23:45.894541 microsoft-kiota-serialization-json-0.3.3/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-05-10 20:23:45.894541 microsoft-kiota-serialization-json-0.3.3/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-05-10 20:23:45.894541 microsoft-kiota-serialization-json-0.3.3/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1870 2023-05-10 20:23:45.894541 microsoft-kiota-serialization-json-0.3.3/.github/workflows/build_publish.yml
--rw-r--r--   0        0        0     2538 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/.gitignore
--rw-r--r--   0        0        0    15976 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/.pylintrc
--rw-r--r--   0        0        0      885 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/LICENSE
--rw-r--r--   0        0        0      350 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/Pipfile
--rw-r--r--   0        0        0    35817 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/Pipfile.lock
--rw-r--r--   0        0        0     2545 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/README.md
--rw-r--r--   0        0        0     2757 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/SUPPORT.md
--rw-r--r--   0        0        0      119 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/__init__.py
--rw-r--r--   0        0        0       23 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/_version.py
--rw-r--r--   0        0        0    10604 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_parse_node.py
--rw-r--r--   0        0        0     1445 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_parse_node_factory.py
--rw-r--r--   0        0        0    17554 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_serialization_writer.py
--rw-r--r--   0        0        0     1297 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_serialization_writer_factory.py
--rw-r--r--   0        0        0     1344 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      221 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/__init__.py
--rw-r--r--   0        0        0       94 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1710 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/helpers/entity.py
--rw-r--r--   0        0        0      105 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/helpers/office_location.py
--rw-r--r--   0        0        0     5687 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/helpers/user.py
--rw-r--r--   0        0        0        0 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/unit/__init__.py
--rw-r--r--   0        0        0     5930 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_parse_node.py
--rw-r--r--   0        0        0     1747 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_parse_node_factory.py
--rw-r--r--   0        0        0     6947 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_serialization_writer.py
--rw-r--r--   0        0        0     1101 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_serialization_writer_factory.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft-kiota-serialization-json-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       82 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1870 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.github/workflows/build_publish.yml
+-rw-r--r--   0        0        0     2538 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1799 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.gitignore
+-rw-r--r--   0        0        0    15976 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.pylintrc
+-rw-r--r--   0        0        0      978 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/LICENSE
+-rw-r--r--   0        0        0      350 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/Pipfile
+-rw-r--r--   0        0        0    35819 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/Pipfile.lock
+-rw-r--r--   0        0        0     2545 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/README.md
+-rw-r--r--   0        0        0     2757 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/SUPPORT.md
+-rw-r--r--   0        0        0      119 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/_version.py
+-rw-r--r--   0        0        0    10696 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_parse_node.py
+-rw-r--r--   0        0        0     1445 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_parse_node_factory.py
+-rw-r--r--   0        0        0    17554 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_serialization_writer.py
+-rw-r--r--   0        0        0     1297 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     1344 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1456 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/__init__.py
+-rw-r--r--   0        0        0       94 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1710 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/helpers/entity.py
+-rw-r--r--   0        0        0      105 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/helpers/office_location.py
+-rw-r--r--   0        0        0     5687 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/helpers/user.py
+-rw-r--r--   0        0        0        0 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/unit/__init__.py
+-rw-r--r--   0        0        0     5930 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_parse_node.py
+-rw-r--r--   0        0        0     1747 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_parse_node_factory.py
+-rw-r--r--   0        0        0     6947 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_serialization_writer.py
+-rw-r--r--   0        0        0     1101 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft_kiota_serialization_json-0.3.4/PKG-INFO
```

### Comparing `microsoft-kiota-serialization-json-0.3.3/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_serialization_json-0.3.4/.github/workflows/auto-merge-dependabot.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/.github/workflows/build_publish.yml` & `microsoft_kiota_serialization_json-0.3.4/.github/workflows/build_publish.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_serialization_json-0.3.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_serialization_json-0.3.4/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/.gitignore` & `microsoft_kiota_serialization_json-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/.pylintrc` & `microsoft_kiota_serialization_json-0.3.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/CHANGELOG.md` & `microsoft_kiota_serialization_json-0.3.4/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [0.3.2] - 2023-04-27
+## [0.3.4] - 2023-05-17
+
+### Added
+
+### Changed
+
+- Fixed a bug with assigning field values.
+
+## [0.3.3] - 2023-04-27
 
 ### Added
 
 ### Changed
 
 - Fixed a bug with deserializing collection of enum values.
```

### Comparing `microsoft-kiota-serialization-json-0.3.3/LICENSE` & `microsoft_kiota_serialization_json-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/Pipfile.lock` & `microsoft_kiota_serialization_json-0.3.4/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9836910774410774%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'88a0e22fe9b8aaf260dbf54096e74e09026b3f309b81b79f80959ca81abff153'}}",*

 * * "'develop'": "{'astroid': {'hashes': "*

 * *              "['sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324', "*

 * *              "'sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f'], "*

 * *              "'version': '==2.15.5'}, 'docutils': {'hashes': "*

 * *              "['sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6', "*

 * *           […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "e80eb193cf8aeb2c98926555e2e5bae634273d94b6fb009e705500b09b3d80d5"
+            "sha256": "88a0e22fe9b8aaf260dbf54096e74e09026b3f309b81b79f80959ca81abff153"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
@@ -46,19 +46,19 @@
             "markers": "python_version >= '3.6'",
             "version": "==4.1.1"
         }
     },
     "develop": {
         "astroid": {
             "hashes": [
-                "sha256:a1b8543ef9d36ea777194bc9b17f5f8678d2c56ee6a45b2c2f17eec96f242347",
-                "sha256:c81e1c7fbac615037744d067a9bb5f9aeb655edf59b63ee8b59585475d6f80d8"
+                "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324",
+                "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.4"
+            "version": "==2.15.5"
         },
         "certifi": {
             "hashes": [
                 "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
                 "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
@@ -219,43 +219,43 @@
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
             "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
-                "sha256:a428f10de4de4774389734c986a01b4af2d802d26717108b0f1b9356862937c5",
-                "sha256:f75a5a52fbcacd81b47e42888ad2b380748aaccfb3f13af0fe69deb759f01eb6"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.20"
+            "version": "==0.20.1"
         },
         "exceptiongroup": {
             "hashes": [
                 "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
                 "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
             "version": "==1.1.1"
         },
         "flit": {
             "hashes": [
-                "sha256:5ee0f88fd1cfa4160d1a8fa01237e96d06d677ae0403a0bbabbb277cb37c5e9c",
-                "sha256:d0f2a8f4bd45dc794befbf5839ecc0fd3830d65a57bd52b5997542fac5d5e937"
+                "sha256:076c3aaba5ac24cf0ad3251f910900d95a08218e6bcb26f21fef1036cc4679ca",
+                "sha256:d75edf5eb324da20d53570a6a6f87f51e606eee8384925cd66a90611140844c7"
             ],
             "index": "pypi",
-            "version": "==3.8.0"
+            "version": "==3.9.0"
         },
         "flit-core": {
             "hashes": [
-                "sha256:64a29ec845164a6abe1136bf4bc5ae012bdfe758ed42fc7571a9059a7c80bd83",
-                "sha256:b305b30c99526df5e63d6022dd2310a0a941a187bd3884f4c8ef0418df6c39f3"
+                "sha256:72ad266176c4a3fcfab5f2930d76896059851240570ce9a98733b658cb786eba",
+                "sha256:7aada352fb0c7f5538c4fafeddf314d3a6a92ee8e2b1de70482329e42de70301"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==3.8.0"
+            "version": "==3.9.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -325,43 +325,43 @@
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.0"
         },
         "mypy": {
             "hashes": [
-                "sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521",
-                "sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140",
-                "sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48",
-                "sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128",
-                "sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336",
-                "sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a",
-                "sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41",
-                "sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f",
-                "sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e",
-                "sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8",
-                "sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238",
-                "sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119",
-                "sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb",
-                "sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d",
-                "sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed",
-                "sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9",
-                "sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e",
-                "sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a",
-                "sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5",
-                "sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950",
-                "sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937",
-                "sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394",
-                "sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6",
-                "sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602",
-                "sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1",
-                "sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba"
+                "sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703",
+                "sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf",
+                "sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4",
+                "sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85",
+                "sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd",
+                "sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae",
+                "sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd",
+                "sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca",
+                "sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305",
+                "sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409",
+                "sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c",
+                "sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb",
+                "sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee",
+                "sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a",
+                "sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228",
+                "sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897",
+                "sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d",
+                "sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f",
+                "sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152",
+                "sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf",
+                "sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8",
+                "sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11",
+                "sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017",
+                "sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929",
+                "sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e",
+                "sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a"
             ],
             "index": "pypi",
-            "version": "==1.2.0"
+            "version": "==1.3.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
@@ -373,19 +373,19 @@
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
-                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.0"
+            "version": "==3.5.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -453,19 +453,19 @@
                 "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.11.8"
         },
         "types-python-dateutil": {
             "hashes": [
-                "sha256:355b2cb82b31e556fd18e7b074de7c350c680ab80608f0cc55ba6770d986d67d",
-                "sha256:fe5b545e678ec13e3ddc83a0eee1545c1b5e2fba4cfc39b276ab6f4e7604a923"
+                "sha256:09a0275f95ee31ce68196710ed2c3d1b9dc42e0b61cc43acc369a42cb939134f",
+                "sha256:0b0e7c68e7043b0354b26a1e0225cb1baea7abb1b324d02b50e2d08f1221043f"
             ],
             "index": "pypi",
-            "version": "==2.8.19.12"
+            "version": "==2.8.19.13"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
```

### Comparing `microsoft-kiota-serialization-json-0.3.3/README.md` & `microsoft_kiota_serialization_json-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/SECURITY.md` & `microsoft_kiota_serialization_json-0.3.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/SUPPORT.md` & `microsoft_kiota_serialization_json-0.3.4/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_parse_node.py` & `microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_parse_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,17 @@
 
         item_additional_data = None
 
         # if object is null
         if not object_dict:
             return
 
+        if isinstance(object_dict, str):
+            object_dict = json.loads(object_dict)
+
         if isinstance(item, AdditionalDataHolder):
             item_additional_data = item.additional_data
 
         field_deserializers = item.get_field_deserializers()
 
         for key, val in object_dict.items():
             deserializer = field_deserializers.get(key)
```

### Comparing `microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_parse_node_factory.py` & `microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_serialization_writer.py` & `microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_serialization_writer_factory.py` & `microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/pyproject.toml` & `microsoft_kiota_serialization_json-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/tests/helpers/entity.py` & `microsoft_kiota_serialization_json-0.3.4/tests/helpers/entity.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/tests/helpers/user.py` & `microsoft_kiota_serialization_json-0.3.4/tests/helpers/user.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_parse_node.py` & `microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_parse_node.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_parse_node_factory.py` & `microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_serialization_writer.py` & `microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_serialization_writer_factory.py` & `microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.3/PKG-INFO` & `microsoft_kiota_serialization_json-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-serialization-json
-Version: 0.3.3
+Version: 0.3.4
 Summary: Implementation of Kiota Serialization interfaces for JSON
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

