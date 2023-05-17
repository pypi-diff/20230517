# Comparing `tmp/balcony-0.0.93.tar.gz` & `tmp/balcony-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balcony-0.0.93.tar", max compression
+gzip compressed data, was "balcony-0.1.0.tar", max compression
```

## Comparing `balcony-0.0.93.tar` & `balcony-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.0.93/LICENSE
--rw-r--r--   0        0        0     2094 2023-05-07 07:30:46.231541 balcony-0.0.93/README.md
--rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.0.93/balcony/__init__.py
--rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.0.93/balcony/__main__.py
--rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.0.93/balcony/aws.py
--rw-r--r--   0        0        0    11892 2023-04-21 17:50:16.401554 balcony-0.0.93/balcony/botocore_utils.py
--rw-r--r--   0        0        0    14364 2023-05-09 17:42:32.497330 balcony-0.0.93/balcony/cli.py
--rw-r--r--   0        0        0     2978 2023-04-30 21:07:33.646010 balcony-0.0.93/balcony/config.py
--rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.0.93/balcony/custom_nodes/__init__.py
--rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.0.93/balcony/custom_nodes/codebuild.py
--rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.0.93/balcony/custom_nodes/ecs.py
--rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.0.93/balcony/custom_nodes/iam.py
--rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.0.93/balcony/custom_nodes/lambda_functions.py
--rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.0.93/balcony/custom_nodes/s3.py
--rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.0.93/balcony/custom_nodes/ses.py
--rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.0.93/balcony/custom_nodes/ssm.py
--rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.0.93/balcony/custom_yamls/_example_service.yaml
--rw-r--r--   0        0        0      517 2023-04-06 12:50:36.974851 balcony-0.0.93/balcony/custom_yamls/ec2.yaml
--rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.0.93/balcony/custom_yamls/ecs.yaml
--rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.0.93/balcony/custom_yamls/iam.yaml
--rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.0.93/balcony/custom_yamls/s3.yaml
--rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.0.93/balcony/errors.py
--rw-r--r--   0        0        0    48117 2023-04-29 22:05:26.837497 balcony-0.0.93/balcony/nodes.py
--rw-r--r--   0        0        0    17113 2023-05-01 12:20:53.387726 balcony-0.0.93/balcony/reader.py
--rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.0.93/balcony/registries.py
--rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.0.93/balcony/relations.py
--rw-r--r--   0        0        0     2533 2023-04-21 19:19:57.046512 balcony-0.0.93/balcony/test.py
--rw-r--r--   0        0        0     5373 2023-05-09 17:56:32.379928 balcony-0.0.93/balcony/utils.py
--rw-r--r--   0        0        0     2739 2023-04-30 21:55:13.504191 balcony-0.0.93/balcony/yaml_config.py
--rw-r--r--   0        0        0     2049 2023-04-29 22:16:26.774034 balcony-0.0.93/balcony/yaml_validators.py
--rw-r--r--   0        0        0      664 2023-05-10 17:36:18.494368 balcony-0.0.93/pyproject.toml
--rw-r--r--   0        0        0     3179 1970-01-01 00:00:00.000000 balcony-0.0.93/setup.py
--rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 balcony-0.0.93/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2250 2023-05-17 18:38:17.580378 balcony-0.1.0/README.md
+-rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.0/balcony/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.0/balcony/__main__.py
+-rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.0/balcony/aws.py
+-rw-r--r--   0        0        0    11892 2023-04-21 17:50:16.401554 balcony-0.1.0/balcony/botocore_utils.py
+-rw-r--r--   0        0        0    14364 2023-05-09 17:42:32.497330 balcony-0.1.0/balcony/cli.py
+-rw-r--r--   0        0        0     2978 2023-04-30 21:07:33.646010 balcony-0.1.0/balcony/config.py
+-rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.0/balcony/custom_nodes/__init__.py
+-rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.0/balcony/custom_nodes/codebuild.py
+-rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.0/balcony/custom_nodes/ecs.py
+-rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.0/balcony/custom_nodes/iam.py
+-rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.0/balcony/custom_nodes/lambda_functions.py
+-rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.0/balcony/custom_nodes/s3.py
+-rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.0/balcony/custom_nodes/ses.py
+-rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.0/balcony/custom_nodes/ssm.py
+-rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.1.0/balcony/custom_yamls/_example_service.yaml
+-rw-r--r--   0        0        0      517 2023-04-06 12:50:36.974851 balcony-0.1.0/balcony/custom_yamls/ec2.yaml
+-rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.1.0/balcony/custom_yamls/ecs.yaml
+-rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.0/balcony/custom_yamls/iam.yaml
+-rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.0/balcony/custom_yamls/s3.yaml
+-rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.0/balcony/errors.py
+-rw-r--r--   0        0        0    48117 2023-04-29 22:05:26.837497 balcony-0.1.0/balcony/nodes.py
+-rw-r--r--   0        0        0    17113 2023-05-01 12:20:53.387726 balcony-0.1.0/balcony/reader.py
+-rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.0/balcony/registries.py
+-rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.0/balcony/relations.py
+-rw-r--r--   0        0        0     2533 2023-04-21 19:19:57.046512 balcony-0.1.0/balcony/test.py
+-rw-r--r--   0        0        0     5373 2023-05-09 17:56:32.379928 balcony-0.1.0/balcony/utils.py
+-rw-r--r--   0        0        0     2739 2023-04-30 21:55:13.504191 balcony-0.1.0/balcony/yaml_config.py
+-rw-r--r--   0        0        0     2049 2023-04-29 22:16:26.774034 balcony-0.1.0/balcony/yaml_validators.py
+-rw-r--r--   0        0        0      663 2023-05-17 18:36:50.877883 balcony-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3344 1970-01-01 00:00:00.000000 balcony-0.1.0/setup.py
+-rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 balcony-0.1.0/PKG-INFO
```

### Comparing `balcony-0.0.93/LICENSE` & `balcony-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/README.md` & `balcony-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,131 +1,141 @@
-00000000: 2320 6261 6c63 6f6e 7920 2d20 4157 5320  # balcony - AWS 
-00000010: 4150 4920 666f 7220 6875 6d61 6e73 0a0a  API for humans..
-00000020: 6261 6c63 6f6e 7920 6973 2061 2072 6561  balcony is a rea
-00000030: 642d 6f6e 6c79 2043 4c49 2074 6f6f 6c20  d-only CLI tool 
-00000040: 7468 6174 2073 696d 706c 6966 6965 7320  that simplifies 
-00000050: 7468 6520 7072 6f63 6573 7320 6f66 206c  the process of l
-00000060: 6973 7469 6e67 2061 6c6c 2072 6573 6f75  isting all resou
-00000070: 7263 6573 206f 6e20 7468 6520 4157 5320  rces on the AWS 
-00000080: 6163 636f 756e 742e 0a0a 6261 6c63 6f6e  account...balcon
-00000090: 7920 6479 6e61 6d69 6361 6c6c 7920 7061  y dynamically pa
-000000a0: 7273 6573 2041 5753 2053 444b 2860 626f  rses AWS SDK(`bo
-000000b0: 746f 3360 206c 6962 7261 7279 2920 616e  to3` library) an
-000000c0: 6420 616e 616c 797a 6573 2072 6571 7569  d analyzes requi
-000000d0: 7265 6420 7061 7261 6d65 7465 7273 2066  red parameters f
-000000e0: 6f72 2065 6163 6820 6f70 6572 6174 696f  or each operatio
-000000f0: 6e2e 200a 0a42 7920 2a2a 6573 7461 626c  n. ..By **establ
-00000100: 6973 6869 6e67 2072 656c 6174 696f 6e73  ishing relations
-00000110: 2062 6574 7765 656e 206f 7065 7261 7469   between operati
-00000120: 6f6e 7320 6f76 6572 2072 6571 7569 7265  ons over require
-00000130: 6420 7061 7261 6d65 7465 7273 2a2a 2c20  d parameters**, 
-00000140: 6974 2773 202a 2a61 626c 6520 746f 2061  it's **able to a
-00000150: 7574 6f2d 6669 6c6c 2a2a 2074 6865 6d20  uto-fill** them 
-00000160: 6279 2072 6561 6469 6e67 2074 6865 2072  by reading the r
-00000170: 656c 6174 6564 206f 7065 7261 7469 6f6e  elated operation
-00000180: 2062 6566 6f72 6568 616e 642e 0a0a 4279   beforehand...By
-00000190: 2073 696d 706c 7920 656e 7465 7269 6e67   simply entering
-000001a0: 2074 6865 6972 206e 616d 652c 2062 616c   their name, bal
-000001b0: 636f 6e79 2065 6e61 626c 6573 2064 6576  cony enables dev
-000001c0: 656c 6f70 6572 7320 746f 2065 6173 696c  elopers to easil
-000001d0: 7920 6c69 7374 2074 6865 6972 2041 5753  y list their AWS
-000001e0: 2072 6573 6f75 7263 6573 2e0a 0a3c 212d   resources...<!-
-000001f0: 2d20 4974 2075 7365 7320 5f72 6561 642d  - It uses _read-
-00000200: 6f6e 6c79 5f20 6f70 6572 6174 696f 6e73  only_ operations
-00000210: 2c20 6974 2064 6f65 7320 6e6f 7420 7461  , it does not ta
-00000220: 6b65 2061 6e79 2061 6374 696f 6e20 6f6e  ke any action on
-00000230: 2074 6865 2075 7365 6420 4157 5320 6163   the used AWS ac
-00000240: 636f 756e 742e 202d 2d3e 0a5b 215b 4275  count. -->.[![Bu
-00000250: 696c 6420 616e 6420 7075 626c 6973 6820  ild and publish 
-00000260: 6120 446f 636b 6572 2069 6d61 6765 2074  a Docker image t
-00000270: 6f20 6768 6372 2e69 6f5d 2868 7474 7073  o ghcr.io](https
-00000280: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f67  ://github.com/og
-00000290: 757a 6861 6e2d 7969 6c6d 617a 2f62 616c  uzhan-yilmaz/bal
-000002a0: 636f 6e79 2f61 6374 696f 6e73 2f77 6f72  cony/actions/wor
-000002b0: 6b66 6c6f 7773 2f64 6f63 6b65 722d 7075  kflows/docker-pu
-000002c0: 626c 6973 682e 796d 6c2f 6261 6467 652e  blish.yml/badge.
-000002d0: 7376 673f 6272 616e 6368 3d6d 6169 6e29  svg?branch=main)
-000002e0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000002f0: 2e63 6f6d 2f6f 6775 7a68 616e 2d79 696c  .com/oguzhan-yil
-00000300: 6d61 7a2f 6261 6c63 6f6e 792f 6163 7469  maz/balcony/acti
-00000310: 6f6e 732f 776f 726b 666c 6f77 732f 646f  ons/workflows/do
-00000320: 636b 6572 2d70 7562 6c69 7368 2e79 6d6c  cker-publish.yml
-00000330: 290a 2323 2049 6e73 7461 6c6c 6174 696f  ).## Installatio
-00000340: 6e20 2620 446f 6375 6d65 6e74 6174 696f  n & Documentatio
-00000350: 6e20 0a0a 2a2a 5b68 7474 7073 3a2f 2f6f  n ..**[https://o
-00000360: 6775 7a68 616e 2d79 696c 6d61 7a2e 6769  guzhan-yilmaz.gi
-00000370: 7468 7562 2e69 6f2f 6261 6c63 6f6e 792f  thub.io/balcony/
-00000380: 5d28 6874 7470 733a 2f2f 6f67 757a 6861  ](https://oguzha
-00000390: 6e2d 7969 6c6d 617a 2e67 6974 6875 622e  n-yilmaz.github.
-000003a0: 696f 2f62 616c 636f 6e79 2f71 7569 636b  io/balcony/quick
-000003b0: 7374 6172 7429 2a2a 0a0a 4261 6c63 6f6e  start)**..Balcon
-000003c0: 7927 7320 646f 6375 6d65 6e74 6174 696f  y's documentatio
-000003d0: 6e20 7765 6273 6974 6520 636f 6e74 6169  n website contai
-000003e0: 6e73 2071 7569 636b 7374 6172 7420 6775  ns quickstart gu
-000003f0: 6964 652c 2075 7361 6765 2063 6f6f 6b62  ide, usage cookb
-00000400: 6f6f 6b20 616e 6420 6d6f 7265 2e0a 2323  ook and more..##
-00000410: 2046 6561 7475 7265 7320 2620 4749 4673   Features & GIFs
-00000420: 0a0a 2323 2320 4c69 7374 2061 7661 696c  ..### List avail
-00000430: 6162 6c65 2041 5753 2053 6572 7669 6365  able AWS Service
-00000440: 7320 0a60 6261 6c63 6f6e 7920 6177 7360  s .`balcony aws`
-00000450: 2074 6f20 7365 6520 6576 6572 7920 4157   to see every AW
-00000460: 5320 7365 7276 6963 6520 6176 6169 6c61  S service availa
-00000470: 626c 652e 0a0a 215b 5d28 6874 7470 733a  ble...![](https:
-00000480: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 6775  //github.com/ogu
-00000490: 7a68 616e 2d79 696c 6d61 7a2f 6261 6c63  zhan-yilmaz/balc
-000004a0: 6f6e 792f 626c 6f62 2f6d 6169 6e2f 646f  ony/blob/main/do
-000004b0: 6373 2f76 6973 7561 6c73 2f61 7773 2d73  cs/visuals/aws-s
-000004c0: 6572 7669 6365 732d 6c69 7374 2e67 6966  ervices-list.gif
-000004d0: 290a 0a0a 2323 2320 4c69 7374 2052 6573  )...### List Res
-000004e0: 6f75 7263 6520 4e6f 6465 7320 6f66 2061  ource Nodes of a
-000004f0: 6e20 4157 5320 5365 7276 6963 6520 0a60  n AWS Service .`
-00000500: 6261 6c63 6f6e 7920 6177 7320 3c73 6572  balcony aws <ser
-00000510: 7669 6365 2d6e 616d 653e 6020 746f 2073  vice-name>` to s
-00000520: 6565 2065 7665 7279 2052 6573 6f75 7263  ee every Resourc
-00000530: 6520 4e6f 6465 206f 6620 6120 7365 7276  e Node of a serv
-00000540: 6963 652e 0a0a 215b 5d28 6874 7470 733a  ice...![](https:
-00000550: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 6775  //github.com/ogu
-00000560: 7a68 616e 2d79 696c 6d61 7a2f 6261 6c63  zhan-yilmaz/balc
-00000570: 6f6e 792f 626c 6f62 2f6d 6169 6e2f 646f  ony/blob/main/do
-00000580: 6373 2f76 6973 7561 6c73 2f72 6573 6f75  cs/visuals/resou
-00000590: 7263 652d 6e6f 6465 2d6c 6973 742e 6769  rce-node-list.gi
-000005a0: 6629 0a0a 0a23 2323 2052 6561 6469 6e67  f)...### Reading
-000005b0: 2061 2052 6573 6f75 7263 6520 4e6f 6465   a Resource Node
-000005c0: 200a 6062 616c 636f 6e79 2061 7773 203c   .`balcony aws <
-000005d0: 7365 7276 6963 652d 6e61 6d65 3e20 3c72  service-name> <r
-000005e0: 6573 6f75 7263 652d 6e6f 6465 3e60 2074  esource-node>` t
-000005f0: 6f20 7265 6164 206f 7065 7261 7469 6f6e  o read operation
-00000600: 7320 6f66 2061 2052 6573 6f75 7263 6520  s of a Resource 
-00000610: 4e6f 6465 2e0a 0a21 5b5d 2868 7474 7073  Node...![](https
-00000620: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f67  ://github.com/og
-00000630: 757a 6861 6e2d 7969 6c6d 617a 2f62 616c  uzhan-yilmaz/bal
-00000640: 636f 6e79 2f62 6c6f 622f 6d61 696e 2f64  cony/blob/main/d
-00000650: 6f63 732f 7669 7375 616c 732f 7265 6164  ocs/visuals/read
-00000660: 696e 672d 612d 7265 736f 7572 6365 2d6e  ing-a-resource-n
-00000670: 6f64 652e 6769 6629 0a0a 0a23 2323 2044  ode.gif)...### D
-00000680: 6f63 756d 656e 7461 7469 6f6e 2061 6e64  ocumentation and
-00000690: 2049 6e70 7574 2026 204f 7574 7075 7420   Input & Output 
-000006a0: 6f66 204f 7065 7261 7469 6f6e 730a 5573  of Operations.Us
-000006b0: 6520 7468 6520 602d 2d6c 6973 7460 2c20  e the `--list`, 
-000006c0: 602d 6c60 2066 6c61 6720 746f 2070 7269  `-l` flag to pri
-000006d0: 6e74 2074 6865 2067 6976 656e 2041 5753  nt the given AWS
-000006e0: 2041 5049 204f 7065 7261 7469 6f6e 7320   API Operations 
-000006f0: 646f 6375 6d65 6e74 6174 696f 6e2c 2069  documentation, i
-00000700: 6e70 7574 2026 206f 7574 7075 7420 7374  nput & output st
-00000710: 7275 6374 7572 652e 200a 200a 0a21 5b5d  ructure. . ..![]
-00000720: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000730: 636f 6d2f 6f67 757a 6861 6e2d 7969 6c6d  com/oguzhan-yilm
-00000740: 617a 2f62 616c 636f 6e79 2f62 6c6f 622f  az/balcony/blob/
-00000750: 6d61 696e 2f64 6f63 732f 7669 7375 616c  main/docs/visual
-00000760: 732f 6c69 7374 2d6f 7074 696f 6e2e 6769  s/list-option.gi
-00000770: 6629 0a0a 0a23 2323 2045 6e61 626c 6520  f)...### Enable 
-00000780: 4465 6275 6720 6d65 7373 6167 6573 200a  Debug messages .
-00000790: 5573 6520 7468 6520 602d 2d64 6562 7567  Use the `--debug
-000007a0: 602c 2060 2d64 6020 666c 6167 2074 6f20  `, `-d` flag to 
-000007b0: 7365 6520 7768 6174 2773 2067 6f69 6e67  see what's going
-000007c0: 206f 6e20 756e 6465 7220 7468 6520 686f   on under the ho
-000007d0: 6f64 210a 0a21 5b5d 2868 7474 7073 3a2f  od!..![](https:/
-000007e0: 2f67 6974 6875 622e 636f 6d2f 6f67 757a  /github.com/oguz
-000007f0: 6861 6e2d 7969 6c6d 617a 2f62 616c 636f  han-yilmaz/balco
-00000800: 6e79 2f62 6c6f 622f 6d61 696e 2f64 6f63  ny/blob/main/doc
-00000810: 732f 7669 7375 616c 732f 6465 6275 672d  s/visuals/debug-
-00000820: 6d65 7373 6167 6573 2e67 6966 290a       messages.gif).
+00000000: 2320 6261 6c63 6f6e 790a 0a0a 3c64 6976  # balcony...<div
+00000010: 2073 7479 6c65 3d22 6469 7370 6c61 793a   style="display:
+00000020: 2066 6c65 783b 223e 0a20 203c 6120 6872   flex;">.  <a hr
+00000030: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000040: 7562 2e63 6f6d 2f6f 6775 7a68 616e 2d79  ub.com/oguzhan-y
+00000050: 696c 6d61 7a2f 6261 6c63 6f6e 792f 6163  ilmaz/balcony/ac
+00000060: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000070: 646f 636b 6572 2d70 7562 6c69 7368 2e79  docker-publish.y
+00000080: 6d6c 223e 3c69 6d67 2073 7263 3d22 6874  ml"><img src="ht
+00000090: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000000a0: 2f6f 6775 7a68 616e 2d79 696c 6d61 7a2f  /oguzhan-yilmaz/
+000000b0: 6261 6c63 6f6e 792f 6163 7469 6f6e 732f  balcony/actions/
+000000c0: 776f 726b 666c 6f77 732f 646f 636b 6572  workflows/docker
+000000d0: 2d70 7562 6c69 7368 2e79 6d6c 2f62 6164  -publish.yml/bad
+000000e0: 6765 2e73 7667 2220 616c 743d 2242 7569  ge.svg" alt="Bui
+000000f0: 6c64 2061 6e64 2070 7562 6c69 7368 2061  ld and publish a
+00000100: 2044 6f63 6b65 7220 696d 6167 6520 746f   Docker image to
+00000110: 2067 6863 722e 696f 223e 3c2f 613e 0a20   ghcr.io"></a>. 
+00000120: 203c 7370 616e 2073 7479 6c65 3d22 7769   <span style="wi
+00000130: 6474 683a 2035 7078 223e 3c2f 7370 616e  dth: 5px"></span
+00000140: 3e0a 0a3c 6120 6872 6566 3d22 6874 7470  >..<a href="http
+00000150: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
+00000160: 6775 7a68 616e 2d79 696c 6d61 7a2f 6261  guzhan-yilmaz/ba
+00000170: 6c63 6f6e 792f 6163 7469 6f6e 732f 776f  lcony/actions/wo
+00000180: 726b 666c 6f77 732f 7061 6765 732f 7061  rkflows/pages/pa
+00000190: 6765 732d 6275 696c 642d 6465 706c 6f79  ges-build-deploy
+000001a0: 6d65 6e74 223e 3c69 6d67 2073 7263 3d22  ment"><img src="
+000001b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000001c0: 6f6d 2f6f 6775 7a68 616e 2d79 696c 6d61  om/oguzhan-yilma
+000001d0: 7a2f 6261 6c63 6f6e 792f 6163 7469 6f6e  z/balcony/action
+000001e0: 732f 776f 726b 666c 6f77 732f 7061 6765  s/workflows/page
+000001f0: 732f 7061 6765 732d 6275 696c 642d 6465  s/pages-build-de
+00000200: 706c 6f79 6d65 6e74 2f62 6164 6765 2e73  ployment/badge.s
+00000210: 7667 2220 616c 743d 2242 7569 6c64 2061  vg" alt="Build a
+00000220: 6e64 2044 6570 6c6f 7920 446f 6375 6d65  nd Deploy Docume
+00000230: 6e74 6174 696f 6e20 7765 6273 6974 6522  ntation website"
+00000240: 3e3c 2f61 3e0a 3c2f 6469 763e 0a0a 0a0a  ></a>.</div>....
+00000250: 6261 6c63 6f6e 7920 6479 6e61 6d69 6361  balcony dynamica
+00000260: 6c6c 7920 7061 7273 6573 2041 5753 2053  lly parses AWS S
+00000270: 444b 2860 626f 746f 3360 206c 6962 7261  DK(`boto3` libra
+00000280: 7279 2920 616e 6420 616e 616c 797a 6573  ry) and analyzes
+00000290: 2072 6571 7569 7265 6420 7061 7261 6d65   required parame
+000002a0: 7465 7273 2066 6f72 2065 6163 6820 6f70  ters for each op
+000002b0: 6572 6174 696f 6e2e 200a 0a42 7920 2a2a  eration. ..By **
+000002c0: 6573 7461 626c 6973 6869 6e67 2072 656c  establishing rel
+000002d0: 6174 696f 6e73 2062 6574 7765 656e 206f  ations between o
+000002e0: 7065 7261 7469 6f6e 7320 6f76 6572 2072  perations over r
+000002f0: 6571 7569 7265 6420 7061 7261 6d65 7465  equired paramete
+00000300: 7273 2a2a 2c20 6974 2773 202a 2a61 626c  rs**, it's **abl
+00000310: 6520 746f 2061 7574 6f2d 6669 6c6c 2a2a  e to auto-fill**
+00000320: 2074 6865 6d20 6279 2072 6561 6469 6e67   them by reading
+00000330: 2074 6865 2072 656c 6174 6564 206f 7065   the related ope
+00000340: 7261 7469 6f6e 2062 6566 6f72 6568 616e  ration beforehan
+00000350: 642e 0a0a 4279 2073 696d 706c 7920 656e  d...By simply en
+00000360: 7465 7269 6e67 2074 6865 6972 206e 616d  tering their nam
+00000370: 652c 2062 616c 636f 6e79 2065 6e61 626c  e, balcony enabl
+00000380: 6573 2064 6576 656c 6f70 6572 7320 746f  es developers to
+00000390: 2065 6173 696c 7920 6c69 7374 2074 6865   easily list the
+000003a0: 6972 2041 5753 2072 6573 6f75 7263 6573  ir AWS resources
+000003b0: 2e0a 0a0a 2323 2049 6e73 7461 6c6c 6174  ....## Installat
+000003c0: 696f 6e20 2620 446f 6375 6d65 6e74 6174  ion & Documentat
+000003d0: 696f 6e20 0a0a 2a2a 5b68 7474 7073 3a2f  ion ..**[https:/
+000003e0: 2f6f 6775 7a68 616e 2d79 696c 6d61 7a2e  /oguzhan-yilmaz.
+000003f0: 6769 7468 7562 2e69 6f2f 6261 6c63 6f6e  github.io/balcon
+00000400: 792f 5d28 6874 7470 733a 2f2f 6f67 757a  y/](https://oguz
+00000410: 6861 6e2d 7969 6c6d 617a 2e67 6974 6875  han-yilmaz.githu
+00000420: 622e 696f 2f62 616c 636f 6e79 2f71 7569  b.io/balcony/qui
+00000430: 636b 7374 6172 7429 2a2a 0a0a 4261 6c63  ckstart)**..Balc
+00000440: 6f6e 7927 7320 646f 6375 6d65 6e74 6174  ony's documentat
+00000450: 696f 6e20 7765 6273 6974 6520 636f 6e74  ion website cont
+00000460: 6169 6e73 2071 7569 636b 7374 6172 7420  ains quickstart 
+00000470: 6775 6964 652c 2075 7361 6765 2063 6f6f  guide, usage coo
+00000480: 6b62 6f6f 6b20 616e 6420 6d6f 7265 2e0a  kbook and more..
+00000490: 2323 2046 6561 7475 7265 7320 2620 4749  ## Features & GI
+000004a0: 4673 0a3e 2063 6c69 636b 2074 6f20 706c  Fs.> click to pl
+000004b0: 6179 2074 6865 2076 6964 656f 730a 2323  ay the videos.##
+000004c0: 2320 4c69 7374 2061 7661 696c 6162 6c65  # List available
+000004d0: 2041 5753 2053 6572 7669 6365 7320 0a60   AWS Services .`
+000004e0: 6261 6c63 6f6e 7920 6177 7360 2074 6f20  balcony aws` to 
+000004f0: 7365 6520 6576 6572 7920 4157 5320 7365  see every AWS se
+00000500: 7276 6963 6520 6176 6169 6c61 626c 652e  rvice available.
+00000510: 0a0a 215b 5d28 6874 7470 733a 2f2f 6769  ..![](https://gi
+00000520: 7468 7562 2e63 6f6d 2f6f 6775 7a68 616e  thub.com/oguzhan
+00000530: 2d79 696c 6d61 7a2f 6261 6c63 6f6e 792f  -yilmaz/balcony/
+00000540: 626c 6f62 2f6d 6169 6e2f 646f 6373 2f76  blob/main/docs/v
+00000550: 6973 7561 6c73 2f61 7773 2d73 6572 7669  isuals/aws-servi
+00000560: 6365 732d 6c69 7374 2e67 6966 290a 0a0a  ces-list.gif)...
+00000570: 2323 2320 4c69 7374 2052 6573 6f75 7263  ### List Resourc
+00000580: 6520 4e6f 6465 7320 6f66 2061 6e20 4157  e Nodes of an AW
+00000590: 5320 5365 7276 6963 6520 0a60 6261 6c63  S Service .`balc
+000005a0: 6f6e 7920 6177 7320 3c73 6572 7669 6365  ony aws <service
+000005b0: 2d6e 616d 653e 6020 746f 2073 6565 2065  -name>` to see e
+000005c0: 7665 7279 2052 6573 6f75 7263 6520 4e6f  very Resource No
+000005d0: 6465 206f 6620 6120 7365 7276 6963 652e  de of a service.
+000005e0: 0a0a 215b 5d28 6874 7470 733a 2f2f 6769  ..![](https://gi
+000005f0: 7468 7562 2e63 6f6d 2f6f 6775 7a68 616e  thub.com/oguzhan
+00000600: 2d79 696c 6d61 7a2f 6261 6c63 6f6e 792f  -yilmaz/balcony/
+00000610: 626c 6f62 2f6d 6169 6e2f 646f 6373 2f76  blob/main/docs/v
+00000620: 6973 7561 6c73 2f72 6573 6f75 7263 652d  isuals/resource-
+00000630: 6e6f 6465 2d6c 6973 742e 6769 6629 0a0a  node-list.gif)..
+00000640: 0a23 2323 2052 6561 6469 6e67 2061 2052  .### Reading a R
+00000650: 6573 6f75 7263 6520 4e6f 6465 200a 6062  esource Node .`b
+00000660: 616c 636f 6e79 2061 7773 203c 7365 7276  alcony aws <serv
+00000670: 6963 652d 6e61 6d65 3e20 3c72 6573 6f75  ice-name> <resou
+00000680: 7263 652d 6e6f 6465 3e60 2074 6f20 7265  rce-node>` to re
+00000690: 6164 206f 7065 7261 7469 6f6e 7320 6f66  ad operations of
+000006a0: 2061 2052 6573 6f75 7263 6520 4e6f 6465   a Resource Node
+000006b0: 2e0a 0a21 5b5d 2868 7474 7073 3a2f 2f67  ...![](https://g
+000006c0: 6974 6875 622e 636f 6d2f 6f67 757a 6861  ithub.com/oguzha
+000006d0: 6e2d 7969 6c6d 617a 2f62 616c 636f 6e79  n-yilmaz/balcony
+000006e0: 2f62 6c6f 622f 6d61 696e 2f64 6f63 732f  /blob/main/docs/
+000006f0: 7669 7375 616c 732f 7265 6164 696e 672d  visuals/reading-
+00000700: 612d 7265 736f 7572 6365 2d6e 6f64 652e  a-resource-node.
+00000710: 6769 6629 0a0a 0a23 2323 2044 6f63 756d  gif)...### Docum
+00000720: 656e 7461 7469 6f6e 2061 6e64 2049 6e70  entation and Inp
+00000730: 7574 2026 204f 7574 7075 7420 6f66 204f  ut & Output of O
+00000740: 7065 7261 7469 6f6e 730a 5573 6520 7468  perations.Use th
+00000750: 6520 602d 2d6c 6973 7460 2c20 602d 6c60  e `--list`, `-l`
+00000760: 2066 6c61 6720 746f 2070 7269 6e74 2074   flag to print t
+00000770: 6865 2067 6976 656e 2041 5753 2041 5049  he given AWS API
+00000780: 204f 7065 7261 7469 6f6e 7320 646f 6375   Operations docu
+00000790: 6d65 6e74 6174 696f 6e2c 2069 6e70 7574  mentation, input
+000007a0: 2026 206f 7574 7075 7420 7374 7275 6374   & output struct
+000007b0: 7572 652e 200a 200a 0a21 5b5d 2868 7474  ure. . ..![](htt
+000007c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000007d0: 6f67 757a 6861 6e2d 7969 6c6d 617a 2f62  oguzhan-yilmaz/b
+000007e0: 616c 636f 6e79 2f62 6c6f 622f 6d61 696e  alcony/blob/main
+000007f0: 2f64 6f63 732f 7669 7375 616c 732f 6c69  /docs/visuals/li
+00000800: 7374 2d6f 7074 696f 6e2e 6769 6629 0a0a  st-option.gif)..
+00000810: 0a23 2323 2045 6e61 626c 6520 4465 6275  .### Enable Debu
+00000820: 6720 6d65 7373 6167 6573 200a 5573 6520  g messages .Use 
+00000830: 7468 6520 602d 2d64 6562 7567 602c 2060  the `--debug`, `
+00000840: 2d64 6020 666c 6167 2074 6f20 7365 6520  -d` flag to see 
+00000850: 7768 6174 2773 2067 6f69 6e67 206f 6e20  what's going on 
+00000860: 756e 6465 7220 7468 6520 686f 6f64 210a  under the hood!.
+00000870: 0a21 5b5d 2868 7474 7073 3a2f 2f67 6974  .![](https://git
+00000880: 6875 622e 636f 6d2f 6f67 757a 6861 6e2d  hub.com/oguzhan-
+00000890: 7969 6c6d 617a 2f62 616c 636f 6e79 2f62  yilmaz/balcony/b
+000008a0: 6c6f 622f 6d61 696e 2f64 6f63 732f 7669  lob/main/docs/vi
+000008b0: 7375 616c 732f 6465 6275 672d 6d65 7373  suals/debug-mess
+000008c0: 6167 6573 2e67 6966 290a                 ages.gif).
```

### Comparing `balcony-0.0.93/balcony/__init__.py` & `balcony-0.1.0/balcony/__init__.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/aws.py` & `balcony-0.1.0/balcony/aws.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/botocore_utils.py` & `balcony-0.1.0/balcony/botocore_utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/cli.py` & `balcony-0.1.0/balcony/cli.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/config.py` & `balcony-0.1.0/balcony/config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/custom_nodes/codebuild.py` & `balcony-0.1.0/balcony/custom_nodes/codebuild.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/custom_nodes/ecs.py` & `balcony-0.1.0/balcony/custom_nodes/ecs.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/custom_nodes/iam.py` & `balcony-0.1.0/balcony/custom_nodes/iam.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/custom_nodes/lambda_functions.py` & `balcony-0.1.0/balcony/custom_nodes/lambda_functions.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/custom_nodes/s3.py` & `balcony-0.1.0/balcony/custom_nodes/s3.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/custom_nodes/ses.py` & `balcony-0.1.0/balcony/custom_nodes/ses.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/custom_nodes/ssm.py` & `balcony-0.1.0/balcony/custom_nodes/ssm.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/custom_yamls/_example_service.yaml` & `balcony-0.1.0/balcony/custom_yamls/_example_service.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/custom_yamls/ec2.yaml` & `balcony-0.1.0/balcony/custom_yamls/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/custom_yamls/iam.yaml` & `balcony-0.1.0/balcony/custom_yamls/iam.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/nodes.py` & `balcony-0.1.0/balcony/nodes.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/reader.py` & `balcony-0.1.0/balcony/reader.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/registries.py` & `balcony-0.1.0/balcony/registries.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/relations.py` & `balcony-0.1.0/balcony/relations.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/test.py` & `balcony-0.1.0/balcony/test.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/utils.py` & `balcony-0.1.0/balcony/utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/yaml_config.py` & `balcony-0.1.0/balcony/yaml_config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/balcony/yaml_validators.py` & `balcony-0.1.0/balcony/yaml_validators.py`

 * *Files identical despite different names*

### Comparing `balcony-0.0.93/pyproject.toml` & `balcony-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "balcony"
-version = "0.0.93"
+version = "0.1.0"
 description = "AWS API for humans"
 authors = ["Oguzhan Yilmaz <oguzhanylmz271@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 balcony = "balcony.cli:run_app"
```

### Comparing `balcony-0.0.93/setup.py` & `balcony-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,169 +31,179 @@
 000001e0: 706f 696e 7473 203d 205c 0a7b 2763 6f6e  points = \.{'con
 000001f0: 736f 6c65 5f73 6372 6970 7473 273a 205b  sole_scripts': [
 00000200: 2762 616c 636f 6e79 203d 2062 616c 636f  'balcony = balco
 00000210: 6e79 2e63 6c69 3a72 756e 5f61 7070 275d  ny.cli:run_app']
 00000220: 7d0a 0a73 6574 7570 5f6b 7761 7267 7320  }..setup_kwargs 
 00000230: 3d20 7b0a 2020 2020 276e 616d 6527 3a20  = {.    'name': 
 00000240: 2762 616c 636f 6e79 272c 0a20 2020 2027  'balcony',.    '
-00000250: 7665 7273 696f 6e27 3a20 2730 2e30 2e39  version': '0.0.9
-00000260: 3327 2c0a 2020 2020 2764 6573 6372 6970  3',.    'descrip
-00000270: 7469 6f6e 273a 2027 4157 5320 4150 4920  tion': 'AWS API 
-00000280: 666f 7220 6875 6d61 6e73 272c 0a20 2020  for humans',.   
-00000290: 2027 6c6f 6e67 5f64 6573 6372 6970 7469   'long_descripti
-000002a0: 6f6e 273a 2022 2320 6261 6c63 6f6e 7920  on': "# balcony 
-000002b0: 2d20 4157 5320 4150 4920 666f 7220 6875  - AWS API for hu
-000002c0: 6d61 6e73 5c6e 5c6e 6261 6c63 6f6e 7920  mans\n\nbalcony 
-000002d0: 6973 2061 2072 6561 642d 6f6e 6c79 2043  is a read-only C
-000002e0: 4c49 2074 6f6f 6c20 7468 6174 2073 696d  LI tool that sim
-000002f0: 706c 6966 6965 7320 7468 6520 7072 6f63  plifies the proc
-00000300: 6573 7320 6f66 206c 6973 7469 6e67 2061  ess of listing a
-00000310: 6c6c 2072 6573 6f75 7263 6573 206f 6e20  ll resources on 
-00000320: 7468 6520 4157 5320 6163 636f 756e 742e  the AWS account.
-00000330: 5c6e 5c6e 6261 6c63 6f6e 7920 6479 6e61  \n\nbalcony dyna
-00000340: 6d69 6361 6c6c 7920 7061 7273 6573 2041  mically parses A
-00000350: 5753 2053 444b 2860 626f 746f 3360 206c  WS SDK(`boto3` l
-00000360: 6962 7261 7279 2920 616e 6420 616e 616c  ibrary) and anal
-00000370: 797a 6573 2072 6571 7569 7265 6420 7061  yzes required pa
-00000380: 7261 6d65 7465 7273 2066 6f72 2065 6163  rameters for eac
-00000390: 6820 6f70 6572 6174 696f 6e2e 205c 6e5c  h operation. \n\
-000003a0: 6e42 7920 2a2a 6573 7461 626c 6973 6869  nBy **establishi
-000003b0: 6e67 2072 656c 6174 696f 6e73 2062 6574  ng relations bet
-000003c0: 7765 656e 206f 7065 7261 7469 6f6e 7320  ween operations 
-000003d0: 6f76 6572 2072 6571 7569 7265 6420 7061  over required pa
-000003e0: 7261 6d65 7465 7273 2a2a 2c20 6974 2773  rameters**, it's
-000003f0: 202a 2a61 626c 6520 746f 2061 7574 6f2d   **able to auto-
-00000400: 6669 6c6c 2a2a 2074 6865 6d20 6279 2072  fill** them by r
-00000410: 6561 6469 6e67 2074 6865 2072 656c 6174  eading the relat
-00000420: 6564 206f 7065 7261 7469 6f6e 2062 6566  ed operation bef
-00000430: 6f72 6568 616e 642e 5c6e 5c6e 4279 2073  orehand.\n\nBy s
-00000440: 696d 706c 7920 656e 7465 7269 6e67 2074  imply entering t
-00000450: 6865 6972 206e 616d 652c 2062 616c 636f  heir name, balco
-00000460: 6e79 2065 6e61 626c 6573 2064 6576 656c  ny enables devel
-00000470: 6f70 6572 7320 746f 2065 6173 696c 7920  opers to easily 
-00000480: 6c69 7374 2074 6865 6972 2041 5753 2072  list their AWS r
-00000490: 6573 6f75 7263 6573 2e5c 6e5c 6e3c 212d  esources.\n\n<!-
-000004a0: 2d20 4974 2075 7365 7320 5f72 6561 642d  - It uses _read-
-000004b0: 6f6e 6c79 5f20 6f70 6572 6174 696f 6e73  only_ operations
-000004c0: 2c20 6974 2064 6f65 7320 6e6f 7420 7461  , it does not ta
-000004d0: 6b65 2061 6e79 2061 6374 696f 6e20 6f6e  ke any action on
-000004e0: 2074 6865 2075 7365 6420 4157 5320 6163   the used AWS ac
-000004f0: 636f 756e 742e 202d 2d3e 5c6e 5b21 5b42  count. -->\n[![B
-00000500: 7569 6c64 2061 6e64 2070 7562 6c69 7368  uild and publish
-00000510: 2061 2044 6f63 6b65 7220 696d 6167 6520   a Docker image 
-00000520: 746f 2067 6863 722e 696f 5d28 6874 7470  to ghcr.io](http
-00000530: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
-00000540: 6775 7a68 616e 2d79 696c 6d61 7a2f 6261  guzhan-yilmaz/ba
-00000550: 6c63 6f6e 792f 6163 7469 6f6e 732f 776f  lcony/actions/wo
-00000560: 726b 666c 6f77 732f 646f 636b 6572 2d70  rkflows/docker-p
-00000570: 7562 6c69 7368 2e79 6d6c 2f62 6164 6765  ublish.yml/badge
-00000580: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
-00000590: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-000005a0: 622e 636f 6d2f 6f67 757a 6861 6e2d 7969  b.com/oguzhan-yi
-000005b0: 6c6d 617a 2f62 616c 636f 6e79 2f61 6374  lmaz/balcony/act
-000005c0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f64  ions/workflows/d
-000005d0: 6f63 6b65 722d 7075 626c 6973 682e 796d  ocker-publish.ym
-000005e0: 6c29 5c6e 2323 2049 6e73 7461 6c6c 6174  l)\n## Installat
-000005f0: 696f 6e20 2620 446f 6375 6d65 6e74 6174  ion & Documentat
-00000600: 696f 6e20 5c6e 5c6e 2a2a 5b68 7474 7073  ion \n\n**[https
-00000610: 3a2f 2f6f 6775 7a68 616e 2d79 696c 6d61  ://oguzhan-yilma
-00000620: 7a2e 6769 7468 7562 2e69 6f2f 6261 6c63  z.github.io/balc
-00000630: 6f6e 792f 5d28 6874 7470 733a 2f2f 6f67  ony/](https://og
-00000640: 757a 6861 6e2d 7969 6c6d 617a 2e67 6974  uzhan-yilmaz.git
-00000650: 6875 622e 696f 2f62 616c 636f 6e79 2f71  hub.io/balcony/q
-00000660: 7569 636b 7374 6172 7429 2a2a 5c6e 5c6e  uickstart)**\n\n
-00000670: 4261 6c63 6f6e 7927 7320 646f 6375 6d65  Balcony's docume
-00000680: 6e74 6174 696f 6e20 7765 6273 6974 6520  ntation website 
-00000690: 636f 6e74 6169 6e73 2071 7569 636b 7374  contains quickst
-000006a0: 6172 7420 6775 6964 652c 2075 7361 6765  art guide, usage
-000006b0: 2063 6f6f 6b62 6f6f 6b20 616e 6420 6d6f   cookbook and mo
-000006c0: 7265 2e5c 6e23 2320 4665 6174 7572 6573  re.\n## Features
-000006d0: 2026 2047 4946 735c 6e5c 6e23 2323 204c   & GIFs\n\n### L
-000006e0: 6973 7420 6176 6169 6c61 626c 6520 4157  ist available AW
-000006f0: 5320 5365 7276 6963 6573 205c 6e60 6261  S Services \n`ba
-00000700: 6c63 6f6e 7920 6177 7360 2074 6f20 7365  lcony aws` to se
-00000710: 6520 6576 6572 7920 4157 5320 7365 7276  e every AWS serv
-00000720: 6963 6520 6176 6169 6c61 626c 652e 5c6e  ice available.\n
-00000730: 5c6e 215b 5d28 6874 7470 733a 2f2f 6769  \n![](https://gi
-00000740: 7468 7562 2e63 6f6d 2f6f 6775 7a68 616e  thub.com/oguzhan
-00000750: 2d79 696c 6d61 7a2f 6261 6c63 6f6e 792f  -yilmaz/balcony/
-00000760: 626c 6f62 2f6d 6169 6e2f 646f 6373 2f76  blob/main/docs/v
-00000770: 6973 7561 6c73 2f61 7773 2d73 6572 7669  isuals/aws-servi
-00000780: 6365 732d 6c69 7374 2e67 6966 295c 6e5c  ces-list.gif)\n\
-00000790: 6e5c 6e23 2323 204c 6973 7420 5265 736f  n\n### List Reso
-000007a0: 7572 6365 204e 6f64 6573 206f 6620 616e  urce Nodes of an
-000007b0: 2041 5753 2053 6572 7669 6365 205c 6e60   AWS Service \n`
-000007c0: 6261 6c63 6f6e 7920 6177 7320 3c73 6572  balcony aws <ser
-000007d0: 7669 6365 2d6e 616d 653e 6020 746f 2073  vice-name>` to s
-000007e0: 6565 2065 7665 7279 2052 6573 6f75 7263  ee every Resourc
-000007f0: 6520 4e6f 6465 206f 6620 6120 7365 7276  e Node of a serv
-00000800: 6963 652e 5c6e 5c6e 215b 5d28 6874 7470  ice.\n\n![](http
-00000810: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
-00000820: 6775 7a68 616e 2d79 696c 6d61 7a2f 6261  guzhan-yilmaz/ba
-00000830: 6c63 6f6e 792f 626c 6f62 2f6d 6169 6e2f  lcony/blob/main/
-00000840: 646f 6373 2f76 6973 7561 6c73 2f72 6573  docs/visuals/res
-00000850: 6f75 7263 652d 6e6f 6465 2d6c 6973 742e  ource-node-list.
-00000860: 6769 6629 5c6e 5c6e 5c6e 2323 2320 5265  gif)\n\n\n### Re
-00000870: 6164 696e 6720 6120 5265 736f 7572 6365  ading a Resource
-00000880: 204e 6f64 6520 5c6e 6062 616c 636f 6e79   Node \n`balcony
-00000890: 2061 7773 203c 7365 7276 6963 652d 6e61   aws <service-na
-000008a0: 6d65 3e20 3c72 6573 6f75 7263 652d 6e6f  me> <resource-no
-000008b0: 6465 3e60 2074 6f20 7265 6164 206f 7065  de>` to read ope
-000008c0: 7261 7469 6f6e 7320 6f66 2061 2052 6573  rations of a Res
-000008d0: 6f75 7263 6520 4e6f 6465 2e5c 6e5c 6e21  ource Node.\n\n!
-000008e0: 5b5d 2868 7474 7073 3a2f 2f67 6974 6875  [](https://githu
-000008f0: 622e 636f 6d2f 6f67 757a 6861 6e2d 7969  b.com/oguzhan-yi
-00000900: 6c6d 617a 2f62 616c 636f 6e79 2f62 6c6f  lmaz/balcony/blo
-00000910: 622f 6d61 696e 2f64 6f63 732f 7669 7375  b/main/docs/visu
-00000920: 616c 732f 7265 6164 696e 672d 612d 7265  als/reading-a-re
-00000930: 736f 7572 6365 2d6e 6f64 652e 6769 6629  source-node.gif)
-00000940: 5c6e 5c6e 5c6e 2323 2320 446f 6375 6d65  \n\n\n### Docume
-00000950: 6e74 6174 696f 6e20 616e 6420 496e 7075  ntation and Inpu
-00000960: 7420 2620 4f75 7470 7574 206f 6620 4f70  t & Output of Op
-00000970: 6572 6174 696f 6e73 5c6e 5573 6520 7468  erations\nUse th
-00000980: 6520 602d 2d6c 6973 7460 2c20 602d 6c60  e `--list`, `-l`
-00000990: 2066 6c61 6720 746f 2070 7269 6e74 2074   flag to print t
-000009a0: 6865 2067 6976 656e 2041 5753 2041 5049  he given AWS API
-000009b0: 204f 7065 7261 7469 6f6e 7320 646f 6375   Operations docu
-000009c0: 6d65 6e74 6174 696f 6e2c 2069 6e70 7574  mentation, input
-000009d0: 2026 206f 7574 7075 7420 7374 7275 6374   & output struct
-000009e0: 7572 652e 205c 6e20 5c6e 5c6e 215b 5d28  ure. \n \n\n![](
-000009f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000a00: 6f6d 2f6f 6775 7a68 616e 2d79 696c 6d61  om/oguzhan-yilma
-00000a10: 7a2f 6261 6c63 6f6e 792f 626c 6f62 2f6d  z/balcony/blob/m
-00000a20: 6169 6e2f 646f 6373 2f76 6973 7561 6c73  ain/docs/visuals
-00000a30: 2f6c 6973 742d 6f70 7469 6f6e 2e67 6966  /list-option.gif
-00000a40: 295c 6e5c 6e5c 6e23 2323 2045 6e61 626c  )\n\n\n### Enabl
-00000a50: 6520 4465 6275 6720 6d65 7373 6167 6573  e Debug messages
-00000a60: 205c 6e55 7365 2074 6865 2060 2d2d 6465   \nUse the `--de
-00000a70: 6275 6760 2c20 602d 6460 2066 6c61 6720  bug`, `-d` flag 
-00000a80: 746f 2073 6565 2077 6861 7427 7320 676f  to see what's go
-00000a90: 696e 6720 6f6e 2075 6e64 6572 2074 6865  ing on under the
-00000aa0: 2068 6f6f 6421 5c6e 5c6e 215b 5d28 6874   hood!\n\n![](ht
-00000ab0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000ac0: 2f6f 6775 7a68 616e 2d79 696c 6d61 7a2f  /oguzhan-yilmaz/
-00000ad0: 6261 6c63 6f6e 792f 626c 6f62 2f6d 6169  balcony/blob/mai
-00000ae0: 6e2f 646f 6373 2f76 6973 7561 6c73 2f64  n/docs/visuals/d
-00000af0: 6562 7567 2d6d 6573 7361 6765 732e 6769  ebug-messages.gi
-00000b00: 6629 5c6e 222c 0a20 2020 2027 6175 7468  f)\n",.    'auth
-00000b10: 6f72 273a 2027 4f67 757a 6861 6e20 5969  or': 'Oguzhan Yi
-00000b20: 6c6d 617a 272c 0a20 2020 2027 6175 7468  lmaz',.    'auth
-00000b30: 6f72 5f65 6d61 696c 273a 2027 6f67 757a  or_email': 'oguz
-00000b40: 6861 6e79 6c6d 7a32 3731 4067 6d61 696c  hanylmz271@gmail
-00000b50: 2e63 6f6d 272c 0a20 2020 2027 6d61 696e  .com',.    'main
-00000b60: 7461 696e 6572 273a 2027 4e6f 6e65 272c  tainer': 'None',
-00000b70: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
-00000b80: 5f65 6d61 696c 273a 2027 4e6f 6e65 272c  _email': 'None',
-00000b90: 0a20 2020 2027 7572 6c27 3a20 274e 6f6e  .    'url': 'Non
-00000ba0: 6527 2c0a 2020 2020 2770 6163 6b61 6765  e',.    'package
-00000bb0: 7327 3a20 7061 636b 6167 6573 2c0a 2020  s': packages,.  
-00000bc0: 2020 2770 6163 6b61 6765 5f64 6174 6127    'package_data'
-00000bd0: 3a20 7061 636b 6167 655f 6461 7461 2c0a  : package_data,.
-00000be0: 2020 2020 2769 6e73 7461 6c6c 5f72 6571      'install_req
-00000bf0: 7569 7265 7327 3a20 696e 7374 616c 6c5f  uires': install_
-00000c00: 7265 7175 6972 6573 2c0a 2020 2020 2765  requires,.    'e
-00000c10: 6e74 7279 5f70 6f69 6e74 7327 3a20 656e  ntry_points': en
-00000c20: 7472 795f 706f 696e 7473 2c0a 2020 2020  try_points,.    
-00000c30: 2770 7974 686f 6e5f 7265 7175 6972 6573  'python_requires
-00000c40: 273a 2027 3e3d 332e 372c 3c34 2e30 272c  ': '>=3.7,<4.0',
-00000c50: 0a7d 0a0a 0a73 6574 7570 282a 2a73 6574  .}...setup(**set
-00000c60: 7570 5f6b 7761 7267 7329 0a              up_kwargs).
+00000250: 7665 7273 696f 6e27 3a20 2730 2e31 2e30  version': '0.1.0
+00000260: 272c 0a20 2020 2027 6465 7363 7269 7074  ',.    'descript
+00000270: 696f 6e27 3a20 2741 5753 2041 5049 2066  ion': 'AWS API f
+00000280: 6f72 2068 756d 616e 7327 2c0a 2020 2020  or humans',.    
+00000290: 276c 6f6e 675f 6465 7363 7269 7074 696f  'long_descriptio
+000002a0: 6e27 3a20 2723 2062 616c 636f 6e79 5c6e  n': '# balcony\n
+000002b0: 5c6e 5c6e 3c64 6976 2073 7479 6c65 3d22  \n\n<div style="
+000002c0: 6469 7370 6c61 793a 2066 6c65 783b 223e  display: flex;">
+000002d0: 5c6e 2020 3c61 2068 7265 663d 2268 7474  \n  <a href="htt
+000002e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000002f0: 6f67 757a 6861 6e2d 7969 6c6d 617a 2f62  oguzhan-yilmaz/b
+00000300: 616c 636f 6e79 2f61 6374 696f 6e73 2f77  alcony/actions/w
+00000310: 6f72 6b66 6c6f 7773 2f64 6f63 6b65 722d  orkflows/docker-
+00000320: 7075 626c 6973 682e 796d 6c22 3e3c 696d  publish.yml"><im
+00000330: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
+00000340: 6974 6875 622e 636f 6d2f 6f67 757a 6861  ithub.com/oguzha
+00000350: 6e2d 7969 6c6d 617a 2f62 616c 636f 6e79  n-yilmaz/balcony
+00000360: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000370: 7773 2f64 6f63 6b65 722d 7075 626c 6973  ws/docker-publis
+00000380: 682e 796d 6c2f 6261 6467 652e 7376 6722  h.yml/badge.svg"
+00000390: 2061 6c74 3d22 4275 696c 6420 616e 6420   alt="Build and 
+000003a0: 7075 626c 6973 6820 6120 446f 636b 6572  publish a Docker
+000003b0: 2069 6d61 6765 2074 6f20 6768 6372 2e69   image to ghcr.i
+000003c0: 6f22 3e3c 2f61 3e5c 6e20 203c 7370 616e  o"></a>\n  <span
+000003d0: 2073 7479 6c65 3d22 7769 6474 683a 2035   style="width: 5
+000003e0: 7078 223e 3c2f 7370 616e 3e5c 6e5c 6e3c  px"></span>\n\n<
+000003f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000400: 6769 7468 7562 2e63 6f6d 2f6f 6775 7a68  github.com/oguzh
+00000410: 616e 2d79 696c 6d61 7a2f 6261 6c63 6f6e  an-yilmaz/balcon
+00000420: 792f 6163 7469 6f6e 732f 776f 726b 666c  y/actions/workfl
+00000430: 6f77 732f 7061 6765 732f 7061 6765 732d  ows/pages/pages-
+00000440: 6275 696c 642d 6465 706c 6f79 6d65 6e74  build-deployment
+00000450: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000460: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
+00000470: 6775 7a68 616e 2d79 696c 6d61 7a2f 6261  guzhan-yilmaz/ba
+00000480: 6c63 6f6e 792f 6163 7469 6f6e 732f 776f  lcony/actions/wo
+00000490: 726b 666c 6f77 732f 7061 6765 732f 7061  rkflows/pages/pa
+000004a0: 6765 732d 6275 696c 642d 6465 706c 6f79  ges-build-deploy
+000004b0: 6d65 6e74 2f62 6164 6765 2e73 7667 2220  ment/badge.svg" 
+000004c0: 616c 743d 2242 7569 6c64 2061 6e64 2044  alt="Build and D
+000004d0: 6570 6c6f 7920 446f 6375 6d65 6e74 6174  eploy Documentat
+000004e0: 696f 6e20 7765 6273 6974 6522 3e3c 2f61  ion website"></a
+000004f0: 3e5c 6e3c 2f64 6976 3e5c 6e5c 6e5c 6e5c  >\n</div>\n\n\n\
+00000500: 6e62 616c 636f 6e79 2064 796e 616d 6963  nbalcony dynamic
+00000510: 616c 6c79 2070 6172 7365 7320 4157 5320  ally parses AWS 
+00000520: 5344 4b28 6062 6f74 6f33 6020 6c69 6272  SDK(`boto3` libr
+00000530: 6172 7929 2061 6e64 2061 6e61 6c79 7a65  ary) and analyze
+00000540: 7320 7265 7175 6972 6564 2070 6172 616d  s required param
+00000550: 6574 6572 7320 666f 7220 6561 6368 206f  eters for each o
+00000560: 7065 7261 7469 6f6e 2e20 5c6e 5c6e 4279  peration. \n\nBy
+00000570: 202a 2a65 7374 6162 6c69 7368 696e 6720   **establishing 
+00000580: 7265 6c61 7469 6f6e 7320 6265 7477 6565  relations betwee
+00000590: 6e20 6f70 6572 6174 696f 6e73 206f 7665  n operations ove
+000005a0: 7220 7265 7175 6972 6564 2070 6172 616d  r required param
+000005b0: 6574 6572 732a 2a2c 2069 745c 2773 202a  eters**, it\'s *
+000005c0: 2a61 626c 6520 746f 2061 7574 6f2d 6669  *able to auto-fi
+000005d0: 6c6c 2a2a 2074 6865 6d20 6279 2072 6561  ll** them by rea
+000005e0: 6469 6e67 2074 6865 2072 656c 6174 6564  ding the related
+000005f0: 206f 7065 7261 7469 6f6e 2062 6566 6f72   operation befor
+00000600: 6568 616e 642e 5c6e 5c6e 4279 2073 696d  ehand.\n\nBy sim
+00000610: 706c 7920 656e 7465 7269 6e67 2074 6865  ply entering the
+00000620: 6972 206e 616d 652c 2062 616c 636f 6e79  ir name, balcony
+00000630: 2065 6e61 626c 6573 2064 6576 656c 6f70   enables develop
+00000640: 6572 7320 746f 2065 6173 696c 7920 6c69  ers to easily li
+00000650: 7374 2074 6865 6972 2041 5753 2072 6573  st their AWS res
+00000660: 6f75 7263 6573 2e5c 6e5c 6e5c 6e23 2320  ources.\n\n\n## 
+00000670: 496e 7374 616c 6c61 7469 6f6e 2026 2044  Installation & D
+00000680: 6f63 756d 656e 7461 7469 6f6e 205c 6e5c  ocumentation \n\
+00000690: 6e2a 2a5b 6874 7470 733a 2f2f 6f67 757a  n**[https://oguz
+000006a0: 6861 6e2d 7969 6c6d 617a 2e67 6974 6875  han-yilmaz.githu
+000006b0: 622e 696f 2f62 616c 636f 6e79 2f5d 2868  b.io/balcony/](h
+000006c0: 7474 7073 3a2f 2f6f 6775 7a68 616e 2d79  ttps://oguzhan-y
+000006d0: 696c 6d61 7a2e 6769 7468 7562 2e69 6f2f  ilmaz.github.io/
+000006e0: 6261 6c63 6f6e 792f 7175 6963 6b73 7461  balcony/quicksta
+000006f0: 7274 292a 2a5c 6e5c 6e42 616c 636f 6e79  rt)**\n\nBalcony
+00000700: 5c27 7320 646f 6375 6d65 6e74 6174 696f  \'s documentatio
+00000710: 6e20 7765 6273 6974 6520 636f 6e74 6169  n website contai
+00000720: 6e73 2071 7569 636b 7374 6172 7420 6775  ns quickstart gu
+00000730: 6964 652c 2075 7361 6765 2063 6f6f 6b62  ide, usage cookb
+00000740: 6f6f 6b20 616e 6420 6d6f 7265 2e5c 6e23  ook and more.\n#
+00000750: 2320 4665 6174 7572 6573 2026 2047 4946  # Features & GIF
+00000760: 735c 6e3e 2063 6c69 636b 2074 6f20 706c  s\n> click to pl
+00000770: 6179 2074 6865 2076 6964 656f 735c 6e23  ay the videos\n#
+00000780: 2323 204c 6973 7420 6176 6169 6c61 626c  ## List availabl
+00000790: 6520 4157 5320 5365 7276 6963 6573 205c  e AWS Services \
+000007a0: 6e60 6261 6c63 6f6e 7920 6177 7360 2074  n`balcony aws` t
+000007b0: 6f20 7365 6520 6576 6572 7920 4157 5320  o see every AWS 
+000007c0: 7365 7276 6963 6520 6176 6169 6c61 626c  service availabl
+000007d0: 652e 5c6e 5c6e 215b 5d28 6874 7470 733a  e.\n\n![](https:
+000007e0: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 6775  //github.com/ogu
+000007f0: 7a68 616e 2d79 696c 6d61 7a2f 6261 6c63  zhan-yilmaz/balc
+00000800: 6f6e 792f 626c 6f62 2f6d 6169 6e2f 646f  ony/blob/main/do
+00000810: 6373 2f76 6973 7561 6c73 2f61 7773 2d73  cs/visuals/aws-s
+00000820: 6572 7669 6365 732d 6c69 7374 2e67 6966  ervices-list.gif
+00000830: 295c 6e5c 6e5c 6e23 2323 204c 6973 7420  )\n\n\n### List 
+00000840: 5265 736f 7572 6365 204e 6f64 6573 206f  Resource Nodes o
+00000850: 6620 616e 2041 5753 2053 6572 7669 6365  f an AWS Service
+00000860: 205c 6e60 6261 6c63 6f6e 7920 6177 7320   \n`balcony aws 
+00000870: 3c73 6572 7669 6365 2d6e 616d 653e 6020  <service-name>` 
+00000880: 746f 2073 6565 2065 7665 7279 2052 6573  to see every Res
+00000890: 6f75 7263 6520 4e6f 6465 206f 6620 6120  ource Node of a 
+000008a0: 7365 7276 6963 652e 5c6e 5c6e 215b 5d28  service.\n\n![](
+000008b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000008c0: 6f6d 2f6f 6775 7a68 616e 2d79 696c 6d61  om/oguzhan-yilma
+000008d0: 7a2f 6261 6c63 6f6e 792f 626c 6f62 2f6d  z/balcony/blob/m
+000008e0: 6169 6e2f 646f 6373 2f76 6973 7561 6c73  ain/docs/visuals
+000008f0: 2f72 6573 6f75 7263 652d 6e6f 6465 2d6c  /resource-node-l
+00000900: 6973 742e 6769 6629 5c6e 5c6e 5c6e 2323  ist.gif)\n\n\n##
+00000910: 2320 5265 6164 696e 6720 6120 5265 736f  # Reading a Reso
+00000920: 7572 6365 204e 6f64 6520 5c6e 6062 616c  urce Node \n`bal
+00000930: 636f 6e79 2061 7773 203c 7365 7276 6963  cony aws <servic
+00000940: 652d 6e61 6d65 3e20 3c72 6573 6f75 7263  e-name> <resourc
+00000950: 652d 6e6f 6465 3e60 2074 6f20 7265 6164  e-node>` to read
+00000960: 206f 7065 7261 7469 6f6e 7320 6f66 2061   operations of a
+00000970: 2052 6573 6f75 7263 6520 4e6f 6465 2e5c   Resource Node.\
+00000980: 6e5c 6e21 5b5d 2868 7474 7073 3a2f 2f67  n\n![](https://g
+00000990: 6974 6875 622e 636f 6d2f 6f67 757a 6861  ithub.com/oguzha
+000009a0: 6e2d 7969 6c6d 617a 2f62 616c 636f 6e79  n-yilmaz/balcony
+000009b0: 2f62 6c6f 622f 6d61 696e 2f64 6f63 732f  /blob/main/docs/
+000009c0: 7669 7375 616c 732f 7265 6164 696e 672d  visuals/reading-
+000009d0: 612d 7265 736f 7572 6365 2d6e 6f64 652e  a-resource-node.
+000009e0: 6769 6629 5c6e 5c6e 5c6e 2323 2320 446f  gif)\n\n\n### Do
+000009f0: 6375 6d65 6e74 6174 696f 6e20 616e 6420  cumentation and 
+00000a00: 496e 7075 7420 2620 4f75 7470 7574 206f  Input & Output o
+00000a10: 6620 4f70 6572 6174 696f 6e73 5c6e 5573  f Operations\nUs
+00000a20: 6520 7468 6520 602d 2d6c 6973 7460 2c20  e the `--list`, 
+00000a30: 602d 6c60 2066 6c61 6720 746f 2070 7269  `-l` flag to pri
+00000a40: 6e74 2074 6865 2067 6976 656e 2041 5753  nt the given AWS
+00000a50: 2041 5049 204f 7065 7261 7469 6f6e 7320   API Operations 
+00000a60: 646f 6375 6d65 6e74 6174 696f 6e2c 2069  documentation, i
+00000a70: 6e70 7574 2026 206f 7574 7075 7420 7374  nput & output st
+00000a80: 7275 6374 7572 652e 205c 6e20 5c6e 5c6e  ructure. \n \n\n
+00000a90: 215b 5d28 6874 7470 733a 2f2f 6769 7468  ![](https://gith
+00000aa0: 7562 2e63 6f6d 2f6f 6775 7a68 616e 2d79  ub.com/oguzhan-y
+00000ab0: 696c 6d61 7a2f 6261 6c63 6f6e 792f 626c  ilmaz/balcony/bl
+00000ac0: 6f62 2f6d 6169 6e2f 646f 6373 2f76 6973  ob/main/docs/vis
+00000ad0: 7561 6c73 2f6c 6973 742d 6f70 7469 6f6e  uals/list-option
+00000ae0: 2e67 6966 295c 6e5c 6e5c 6e23 2323 2045  .gif)\n\n\n### E
+00000af0: 6e61 626c 6520 4465 6275 6720 6d65 7373  nable Debug mess
+00000b00: 6167 6573 205c 6e55 7365 2074 6865 2060  ages \nUse the `
+00000b10: 2d2d 6465 6275 6760 2c20 602d 6460 2066  --debug`, `-d` f
+00000b20: 6c61 6720 746f 2073 6565 2077 6861 745c  lag to see what\
+00000b30: 2773 2067 6f69 6e67 206f 6e20 756e 6465  's going on unde
+00000b40: 7220 7468 6520 686f 6f64 215c 6e5c 6e21  r the hood!\n\n!
+00000b50: 5b5d 2868 7474 7073 3a2f 2f67 6974 6875  [](https://githu
+00000b60: 622e 636f 6d2f 6f67 757a 6861 6e2d 7969  b.com/oguzhan-yi
+00000b70: 6c6d 617a 2f62 616c 636f 6e79 2f62 6c6f  lmaz/balcony/blo
+00000b80: 622f 6d61 696e 2f64 6f63 732f 7669 7375  b/main/docs/visu
+00000b90: 616c 732f 6465 6275 672d 6d65 7373 6167  als/debug-messag
+00000ba0: 6573 2e67 6966 295c 6e27 2c0a 2020 2020  es.gif)\n',.    
+00000bb0: 2761 7574 686f 7227 3a20 274f 6775 7a68  'author': 'Oguzh
+00000bc0: 616e 2059 696c 6d61 7a27 2c0a 2020 2020  an Yilmaz',.    
+00000bd0: 2761 7574 686f 725f 656d 6169 6c27 3a20  'author_email': 
+00000be0: 276f 6775 7a68 616e 796c 6d7a 3237 3140  'oguzhanylmz271@
+00000bf0: 676d 6169 6c2e 636f 6d27 2c0a 2020 2020  gmail.com',.    
+00000c00: 276d 6169 6e74 6169 6e65 7227 3a20 274e  'maintainer': 'N
+00000c10: 6f6e 6527 2c0a 2020 2020 276d 6169 6e74  one',.    'maint
+00000c20: 6169 6e65 725f 656d 6169 6c27 3a20 274e  ainer_email': 'N
+00000c30: 6f6e 6527 2c0a 2020 2020 2775 726c 273a  one',.    'url':
+00000c40: 2027 4e6f 6e65 272c 0a20 2020 2027 7061   'None',.    'pa
+00000c50: 636b 6167 6573 273a 2070 6163 6b61 6765  ckages': package
+00000c60: 732c 0a20 2020 2027 7061 636b 6167 655f  s,.    'package_
+00000c70: 6461 7461 273a 2070 6163 6b61 6765 5f64  data': package_d
+00000c80: 6174 612c 0a20 2020 2027 696e 7374 616c  ata,.    'instal
+00000c90: 6c5f 7265 7175 6972 6573 273a 2069 6e73  l_requires': ins
+00000ca0: 7461 6c6c 5f72 6571 7569 7265 732c 0a20  tall_requires,. 
+00000cb0: 2020 2027 656e 7472 795f 706f 696e 7473     'entry_points
+00000cc0: 273a 2065 6e74 7279 5f70 6f69 6e74 732c  ': entry_points,
+00000cd0: 0a20 2020 2027 7079 7468 6f6e 5f72 6571  .    'python_req
+00000ce0: 7569 7265 7327 3a20 273e 3d33 2e37 2c3c  uires': '>=3.7,<
+00000cf0: 342e 3027 2c0a 7d0a 0a0a 7365 7475 7028  4.0',.}...setup(
+00000d00: 2a2a 7365 7475 705f 6b77 6172 6773 290a  **setup_kwargs).
```

### Comparing `balcony-0.0.93/PKG-INFO` & `balcony-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,194 +1,204 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6261 6c63  : 2.1.Name: balc
-00000020: 6f6e 790a 5665 7273 696f 6e3a 2030 2e30  ony.Version: 0.0
-00000030: 2e39 330a 5375 6d6d 6172 793a 2041 5753  .93.Summary: AWS
-00000040: 2041 5049 2066 6f72 2068 756d 616e 730a   API for humans.
-00000050: 4c69 6365 6e73 653a 2047 504c 2d33 2e30  License: GPL-3.0
-00000060: 2d6f 722d 6c61 7465 720a 4175 7468 6f72  -or-later.Author
-00000070: 3a20 4f67 757a 6861 6e20 5969 6c6d 617a  : Oguzhan Yilmaz
-00000080: 0a41 7574 686f 722d 656d 6169 6c3a 206f  .Author-email: o
-00000090: 6775 7a68 616e 796c 6d7a 3237 3140 676d  guzhanylmz271@gm
-000000a0: 6169 6c2e 636f 6d0a 5265 7175 6972 6573  ail.com.Requires
-000000b0: 2d50 7974 686f 6e3a 203e 3d33 2e37 2c3c  -Python: >=3.7,<
-000000c0: 342e 300a 436c 6173 7369 6669 6572 3a20  4.0.Classifier: 
-000000d0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-000000e0: 7070 726f 7665 6420 3a3a 2047 4e55 2047  pproved :: GNU G
-000000f0: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
-00000100: 6365 6e73 6520 7633 206f 7220 6c61 7465  cense v3 or late
-00000110: 7220 2847 504c 7633 2b29 0a43 6c61 7373  r (GPLv3+).Class
-00000120: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000130: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000140: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
-00000150: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000160: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000170: 7974 686f 6e20 3a3a 2033 2e37 0a43 6c61  ython :: 3.7.Cla
-00000180: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000190: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001a0: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
-000001b0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000001c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
-000001e0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000001f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000200: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000210: 2e31 300a 5265 7175 6972 6573 2d44 6973  .10.Requires-Dis
-00000220: 743a 2050 7959 414d 4c20 283e 3d36 2e30  t: PyYAML (>=6.0
-00000230: 2c3c 372e 3029 0a52 6571 7569 7265 732d  ,<7.0).Requires-
-00000240: 4469 7374 3a20 626f 746f 3320 283e 3d31  Dist: boto3 (>=1
-00000250: 2e32 342e 3830 2c3c 322e 302e 3029 0a52  .24.80,<2.0.0).R
-00000260: 6571 7569 7265 732d 4469 7374 3a20 696e  equires-Dist: in
-00000270: 666c 6563 7420 283e 3d36 2e30 2e30 2c3c  flect (>=6.0.0,<
-00000280: 372e 302e 3029 0a52 6571 7569 7265 732d  7.0.0).Requires-
-00000290: 4469 7374 3a20 6a6d 6573 7061 7468 2028  Dist: jmespath (
-000002a0: 3e3d 312e 302e 312c 3c32 2e30 2e30 290a  >=1.0.1,<2.0.0).
-000002b0: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
-000002c0: 6b64 6f63 732d 6175 746f 7265 6673 2028  kdocs-autorefs (
-000002d0: 3e3d 302e 342e 312c 3c30 2e35 2e30 290a  >=0.4.1,<0.5.0).
-000002e0: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
-000002f0: 6b64 6f63 732d 6d61 7465 7269 616c 2028  kdocs-material (
-00000300: 3e3d 382e 352e 372c 3c31 302e 302e 3029  >=8.5.7,<10.0.0)
-00000310: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000320: 6d6b 646f 6373 7472 696e 6773 5b70 7974  mkdocstrings[pyt
-00000330: 686f 6e5d 2028 3e3d 302e 3231 2e32 2c3c  hon] (>=0.21.2,<
-00000340: 302e 3232 2e30 290a 5265 7175 6972 6573  0.22.0).Requires
-00000350: 2d44 6973 743a 2070 7964 616e 7469 6320  -Dist: pydantic 
-00000360: 283e 3d31 2e31 302e 372c 3c32 2e30 2e30  (>=1.10.7,<2.0.0
-00000370: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000380: 2072 6963 6820 283e 3d31 332e 332e 342c   rich (>=13.3.4,
-00000390: 3c31 342e 302e 3029 0a52 6571 7569 7265  <14.0.0).Require
-000003a0: 732d 4469 7374 3a20 7479 7065 7220 283e  s-Dist: typer (>
-000003b0: 3d30 2e37 2e30 2c3c 302e 382e 3029 0a44  =0.7.0,<0.8.0).D
-000003c0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-000003d0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-000003e0: 726b 646f 776e 0a0a 2320 6261 6c63 6f6e  rkdown..# balcon
-000003f0: 7920 2d20 4157 5320 4150 4920 666f 7220  y - AWS API for 
-00000400: 6875 6d61 6e73 0a0a 6261 6c63 6f6e 7920  humans..balcony 
-00000410: 6973 2061 2072 6561 642d 6f6e 6c79 2043  is a read-only C
-00000420: 4c49 2074 6f6f 6c20 7468 6174 2073 696d  LI tool that sim
-00000430: 706c 6966 6965 7320 7468 6520 7072 6f63  plifies the proc
-00000440: 6573 7320 6f66 206c 6973 7469 6e67 2061  ess of listing a
-00000450: 6c6c 2072 6573 6f75 7263 6573 206f 6e20  ll resources on 
-00000460: 7468 6520 4157 5320 6163 636f 756e 742e  the AWS account.
-00000470: 0a0a 6261 6c63 6f6e 7920 6479 6e61 6d69  ..balcony dynami
-00000480: 6361 6c6c 7920 7061 7273 6573 2041 5753  cally parses AWS
-00000490: 2053 444b 2860 626f 746f 3360 206c 6962   SDK(`boto3` lib
-000004a0: 7261 7279 2920 616e 6420 616e 616c 797a  rary) and analyz
-000004b0: 6573 2072 6571 7569 7265 6420 7061 7261  es required para
-000004c0: 6d65 7465 7273 2066 6f72 2065 6163 6820  meters for each 
-000004d0: 6f70 6572 6174 696f 6e2e 200a 0a42 7920  operation. ..By 
-000004e0: 2a2a 6573 7461 626c 6973 6869 6e67 2072  **establishing r
-000004f0: 656c 6174 696f 6e73 2062 6574 7765 656e  elations between
-00000500: 206f 7065 7261 7469 6f6e 7320 6f76 6572   operations over
-00000510: 2072 6571 7569 7265 6420 7061 7261 6d65   required parame
-00000520: 7465 7273 2a2a 2c20 6974 2773 202a 2a61  ters**, it's **a
-00000530: 626c 6520 746f 2061 7574 6f2d 6669 6c6c  ble to auto-fill
-00000540: 2a2a 2074 6865 6d20 6279 2072 6561 6469  ** them by readi
-00000550: 6e67 2074 6865 2072 656c 6174 6564 206f  ng the related o
-00000560: 7065 7261 7469 6f6e 2062 6566 6f72 6568  peration beforeh
-00000570: 616e 642e 0a0a 4279 2073 696d 706c 7920  and...By simply 
-00000580: 656e 7465 7269 6e67 2074 6865 6972 206e  entering their n
-00000590: 616d 652c 2062 616c 636f 6e79 2065 6e61  ame, balcony ena
-000005a0: 626c 6573 2064 6576 656c 6f70 6572 7320  bles developers 
-000005b0: 746f 2065 6173 696c 7920 6c69 7374 2074  to easily list t
-000005c0: 6865 6972 2041 5753 2072 6573 6f75 7263  heir AWS resourc
-000005d0: 6573 2e0a 0a3c 212d 2d20 4974 2075 7365  es...<!-- It use
-000005e0: 7320 5f72 6561 642d 6f6e 6c79 5f20 6f70  s _read-only_ op
-000005f0: 6572 6174 696f 6e73 2c20 6974 2064 6f65  erations, it doe
-00000600: 7320 6e6f 7420 7461 6b65 2061 6e79 2061  s not take any a
-00000610: 6374 696f 6e20 6f6e 2074 6865 2075 7365  ction on the use
-00000620: 6420 4157 5320 6163 636f 756e 742e 202d  d AWS account. -
-00000630: 2d3e 0a5b 215b 4275 696c 6420 616e 6420  ->.[![Build and 
-00000640: 7075 626c 6973 6820 6120 446f 636b 6572  publish a Docker
-00000650: 2069 6d61 6765 2074 6f20 6768 6372 2e69   image to ghcr.i
-00000660: 6f5d 2868 7474 7073 3a2f 2f67 6974 6875  o](https://githu
-00000670: 622e 636f 6d2f 6f67 757a 6861 6e2d 7969  b.com/oguzhan-yi
-00000680: 6c6d 617a 2f62 616c 636f 6e79 2f61 6374  lmaz/balcony/act
-00000690: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f64  ions/workflows/d
-000006a0: 6f63 6b65 722d 7075 626c 6973 682e 796d  ocker-publish.ym
-000006b0: 6c2f 6261 6467 652e 7376 673f 6272 616e  l/badge.svg?bran
-000006c0: 6368 3d6d 6169 6e29 5d28 6874 7470 733a  ch=main)](https:
-000006d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 6775  //github.com/ogu
-000006e0: 7a68 616e 2d79 696c 6d61 7a2f 6261 6c63  zhan-yilmaz/balc
-000006f0: 6f6e 792f 6163 7469 6f6e 732f 776f 726b  ony/actions/work
-00000700: 666c 6f77 732f 646f 636b 6572 2d70 7562  flows/docker-pub
-00000710: 6c69 7368 2e79 6d6c 290a 2323 2049 6e73  lish.yml).## Ins
-00000720: 7461 6c6c 6174 696f 6e20 2620 446f 6375  tallation & Docu
-00000730: 6d65 6e74 6174 696f 6e20 0a0a 2a2a 5b68  mentation ..**[h
-00000740: 7474 7073 3a2f 2f6f 6775 7a68 616e 2d79  ttps://oguzhan-y
-00000750: 696c 6d61 7a2e 6769 7468 7562 2e69 6f2f  ilmaz.github.io/
-00000760: 6261 6c63 6f6e 792f 5d28 6874 7470 733a  balcony/](https:
-00000770: 2f2f 6f67 757a 6861 6e2d 7969 6c6d 617a  //oguzhan-yilmaz
-00000780: 2e67 6974 6875 622e 696f 2f62 616c 636f  .github.io/balco
-00000790: 6e79 2f71 7569 636b 7374 6172 7429 2a2a  ny/quickstart)**
-000007a0: 0a0a 4261 6c63 6f6e 7927 7320 646f 6375  ..Balcony's docu
-000007b0: 6d65 6e74 6174 696f 6e20 7765 6273 6974  mentation websit
-000007c0: 6520 636f 6e74 6169 6e73 2071 7569 636b  e contains quick
-000007d0: 7374 6172 7420 6775 6964 652c 2075 7361  start guide, usa
-000007e0: 6765 2063 6f6f 6b62 6f6f 6b20 616e 6420  ge cookbook and 
-000007f0: 6d6f 7265 2e0a 2323 2046 6561 7475 7265  more..## Feature
-00000800: 7320 2620 4749 4673 0a0a 2323 2320 4c69  s & GIFs..### Li
-00000810: 7374 2061 7661 696c 6162 6c65 2041 5753  st available AWS
-00000820: 2053 6572 7669 6365 7320 0a60 6261 6c63   Services .`balc
-00000830: 6f6e 7920 6177 7360 2074 6f20 7365 6520  ony aws` to see 
-00000840: 6576 6572 7920 4157 5320 7365 7276 6963  every AWS servic
-00000850: 6520 6176 6169 6c61 626c 652e 0a0a 215b  e available...![
-00000860: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000870: 2e63 6f6d 2f6f 6775 7a68 616e 2d79 696c  .com/oguzhan-yil
-00000880: 6d61 7a2f 6261 6c63 6f6e 792f 626c 6f62  maz/balcony/blob
-00000890: 2f6d 6169 6e2f 646f 6373 2f76 6973 7561  /main/docs/visua
-000008a0: 6c73 2f61 7773 2d73 6572 7669 6365 732d  ls/aws-services-
-000008b0: 6c69 7374 2e67 6966 290a 0a0a 2323 2320  list.gif)...### 
-000008c0: 4c69 7374 2052 6573 6f75 7263 6520 4e6f  List Resource No
-000008d0: 6465 7320 6f66 2061 6e20 4157 5320 5365  des of an AWS Se
-000008e0: 7276 6963 6520 0a60 6261 6c63 6f6e 7920  rvice .`balcony 
-000008f0: 6177 7320 3c73 6572 7669 6365 2d6e 616d  aws <service-nam
-00000900: 653e 6020 746f 2073 6565 2065 7665 7279  e>` to see every
-00000910: 2052 6573 6f75 7263 6520 4e6f 6465 206f   Resource Node o
-00000920: 6620 6120 7365 7276 6963 652e 0a0a 215b  f a service...![
-00000930: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000940: 2e63 6f6d 2f6f 6775 7a68 616e 2d79 696c  .com/oguzhan-yil
-00000950: 6d61 7a2f 6261 6c63 6f6e 792f 626c 6f62  maz/balcony/blob
-00000960: 2f6d 6169 6e2f 646f 6373 2f76 6973 7561  /main/docs/visua
-00000970: 6c73 2f72 6573 6f75 7263 652d 6e6f 6465  ls/resource-node
-00000980: 2d6c 6973 742e 6769 6629 0a0a 0a23 2323  -list.gif)...###
-00000990: 2052 6561 6469 6e67 2061 2052 6573 6f75   Reading a Resou
-000009a0: 7263 6520 4e6f 6465 200a 6062 616c 636f  rce Node .`balco
-000009b0: 6e79 2061 7773 203c 7365 7276 6963 652d  ny aws <service-
-000009c0: 6e61 6d65 3e20 3c72 6573 6f75 7263 652d  name> <resource-
-000009d0: 6e6f 6465 3e60 2074 6f20 7265 6164 206f  node>` to read o
-000009e0: 7065 7261 7469 6f6e 7320 6f66 2061 2052  perations of a R
-000009f0: 6573 6f75 7263 6520 4e6f 6465 2e0a 0a21  esource Node...!
-00000a00: 5b5d 2868 7474 7073 3a2f 2f67 6974 6875  [](https://githu
-00000a10: 622e 636f 6d2f 6f67 757a 6861 6e2d 7969  b.com/oguzhan-yi
-00000a20: 6c6d 617a 2f62 616c 636f 6e79 2f62 6c6f  lmaz/balcony/blo
-00000a30: 622f 6d61 696e 2f64 6f63 732f 7669 7375  b/main/docs/visu
-00000a40: 616c 732f 7265 6164 696e 672d 612d 7265  als/reading-a-re
-00000a50: 736f 7572 6365 2d6e 6f64 652e 6769 6629  source-node.gif)
-00000a60: 0a0a 0a23 2323 2044 6f63 756d 656e 7461  ...### Documenta
-00000a70: 7469 6f6e 2061 6e64 2049 6e70 7574 2026  tion and Input &
-00000a80: 204f 7574 7075 7420 6f66 204f 7065 7261   Output of Opera
-00000a90: 7469 6f6e 730a 5573 6520 7468 6520 602d  tions.Use the `-
-00000aa0: 2d6c 6973 7460 2c20 602d 6c60 2066 6c61  -list`, `-l` fla
-00000ab0: 6720 746f 2070 7269 6e74 2074 6865 2067  g to print the g
-00000ac0: 6976 656e 2041 5753 2041 5049 204f 7065  iven AWS API Ope
-00000ad0: 7261 7469 6f6e 7320 646f 6375 6d65 6e74  rations document
-00000ae0: 6174 696f 6e2c 2069 6e70 7574 2026 206f  ation, input & o
-00000af0: 7574 7075 7420 7374 7275 6374 7572 652e  utput structure.
-00000b00: 200a 200a 0a21 5b5d 2868 7474 7073 3a2f   . ..![](https:/
-00000b10: 2f67 6974 6875 622e 636f 6d2f 6f67 757a  /github.com/oguz
-00000b20: 6861 6e2d 7969 6c6d 617a 2f62 616c 636f  han-yilmaz/balco
-00000b30: 6e79 2f62 6c6f 622f 6d61 696e 2f64 6f63  ny/blob/main/doc
-00000b40: 732f 7669 7375 616c 732f 6c69 7374 2d6f  s/visuals/list-o
-00000b50: 7074 696f 6e2e 6769 6629 0a0a 0a23 2323  ption.gif)...###
-00000b60: 2045 6e61 626c 6520 4465 6275 6720 6d65   Enable Debug me
-00000b70: 7373 6167 6573 200a 5573 6520 7468 6520  ssages .Use the 
-00000b80: 602d 2d64 6562 7567 602c 2060 2d64 6020  `--debug`, `-d` 
-00000b90: 666c 6167 2074 6f20 7365 6520 7768 6174  flag to see what
-00000ba0: 2773 2067 6f69 6e67 206f 6e20 756e 6465  's going on unde
-00000bb0: 7220 7468 6520 686f 6f64 210a 0a21 5b5d  r the hood!..![]
-00000bc0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000bd0: 636f 6d2f 6f67 757a 6861 6e2d 7969 6c6d  com/oguzhan-yilm
-00000be0: 617a 2f62 616c 636f 6e79 2f62 6c6f 622f  az/balcony/blob/
-00000bf0: 6d61 696e 2f64 6f63 732f 7669 7375 616c  main/docs/visual
-00000c00: 732f 6465 6275 672d 6d65 7373 6167 6573  s/debug-messages
-00000c10: 2e67 6966 290a 0a                        .gif)..
+00000020: 6f6e 790a 5665 7273 696f 6e3a 2030 2e31  ony.Version: 0.1
+00000030: 2e30 0a53 756d 6d61 7279 3a20 4157 5320  .0.Summary: AWS 
+00000040: 4150 4920 666f 7220 6875 6d61 6e73 0a4c  API for humans.L
+00000050: 6963 656e 7365 3a20 4750 4c2d 332e 302d  icense: GPL-3.0-
+00000060: 6f72 2d6c 6174 6572 0a41 7574 686f 723a  or-later.Author:
+00000070: 204f 6775 7a68 616e 2059 696c 6d61 7a0a   Oguzhan Yilmaz.
+00000080: 4175 7468 6f72 2d65 6d61 696c 3a20 6f67  Author-email: og
+00000090: 757a 6861 6e79 6c6d 7a32 3731 4067 6d61  uzhanylmz271@gma
+000000a0: 696c 2e63 6f6d 0a52 6571 7569 7265 732d  il.com.Requires-
+000000b0: 5079 7468 6f6e 3a20 3e3d 332e 372c 3c34  Python: >=3.7,<4
+000000c0: 2e30 0a43 6c61 7373 6966 6965 723a 204c  .0.Classifier: L
+000000d0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000000e0: 7072 6f76 6564 203a 3a20 474e 5520 4765  proved :: GNU Ge
+000000f0: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
+00000100: 656e 7365 2076 3320 6f72 206c 6174 6572  ense v3 or later
+00000110: 2028 4750 4c76 332b 290a 436c 6173 7369   (GPLv3+).Classi
+00000120: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000130: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000140: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
+00000150: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000160: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000170: 7468 6f6e 203a 3a20 332e 370a 436c 6173  thon :: 3.7.Clas
+00000180: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000190: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001a0: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
+000001b0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000001c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001d0: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
+000001e0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000001f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000200: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000210: 3130 0a52 6571 7569 7265 732d 4469 7374  10.Requires-Dist
+00000220: 3a20 5079 5941 4d4c 2028 3e3d 362e 302c  : PyYAML (>=6.0,
+00000230: 3c37 2e30 290a 5265 7175 6972 6573 2d44  <7.0).Requires-D
+00000240: 6973 743a 2062 6f74 6f33 2028 3e3d 312e  ist: boto3 (>=1.
+00000250: 3234 2e38 302c 3c32 2e30 2e30 290a 5265  24.80,<2.0.0).Re
+00000260: 7175 6972 6573 2d44 6973 743a 2069 6e66  quires-Dist: inf
+00000270: 6c65 6374 2028 3e3d 362e 302e 302c 3c37  lect (>=6.0.0,<7
+00000280: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
+00000290: 6973 743a 206a 6d65 7370 6174 6820 283e  ist: jmespath (>
+000002a0: 3d31 2e30 2e31 2c3c 322e 302e 3029 0a52  =1.0.1,<2.0.0).R
+000002b0: 6571 7569 7265 732d 4469 7374 3a20 6d6b  equires-Dist: mk
+000002c0: 646f 6373 2d61 7574 6f72 6566 7320 283e  docs-autorefs (>
+000002d0: 3d30 2e34 2e31 2c3c 302e 352e 3029 0a52  =0.4.1,<0.5.0).R
+000002e0: 6571 7569 7265 732d 4469 7374 3a20 6d6b  equires-Dist: mk
+000002f0: 646f 6373 2d6d 6174 6572 6961 6c20 283e  docs-material (>
+00000300: 3d38 2e35 2e37 2c3c 3130 2e30 2e30 290a  =8.5.7,<10.0.0).
+00000310: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
+00000320: 6b64 6f63 7374 7269 6e67 735b 7079 7468  kdocstrings[pyth
+00000330: 6f6e 5d20 283e 3d30 2e32 312e 322c 3c30  on] (>=0.21.2,<0
+00000340: 2e32 322e 3029 0a52 6571 7569 7265 732d  .22.0).Requires-
+00000350: 4469 7374 3a20 7079 6461 6e74 6963 2028  Dist: pydantic (
+00000360: 3e3d 312e 3130 2e37 2c3c 322e 302e 3029  >=1.10.7,<2.0.0)
+00000370: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000380: 7269 6368 2028 3e3d 3133 2e33 2e34 2c3c  rich (>=13.3.4,<
+00000390: 3134 2e30 2e30 290a 5265 7175 6972 6573  14.0.0).Requires
+000003a0: 2d44 6973 743a 2074 7970 6572 2028 3e3d  -Dist: typer (>=
+000003b0: 302e 372e 302c 3c30 2e38 2e30 290a 4465  0.7.0,<0.8.0).De
+000003c0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+000003d0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+000003e0: 6b64 6f77 6e0a 0a23 2062 616c 636f 6e79  kdown..# balcony
+000003f0: 0a0a 0a3c 6469 7620 7374 796c 653d 2264  ...<div style="d
+00000400: 6973 706c 6179 3a20 666c 6578 3b22 3e0a  isplay: flex;">.
+00000410: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000420: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f67  ://github.com/og
+00000430: 757a 6861 6e2d 7969 6c6d 617a 2f62 616c  uzhan-yilmaz/bal
+00000440: 636f 6e79 2f61 6374 696f 6e73 2f77 6f72  cony/actions/wor
+00000450: 6b66 6c6f 7773 2f64 6f63 6b65 722d 7075  kflows/docker-pu
+00000460: 626c 6973 682e 796d 6c22 3e3c 696d 6720  blish.yml"><img 
+00000470: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00000480: 6875 622e 636f 6d2f 6f67 757a 6861 6e2d  hub.com/oguzhan-
+00000490: 7969 6c6d 617a 2f62 616c 636f 6e79 2f61  yilmaz/balcony/a
+000004a0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+000004b0: 2f64 6f63 6b65 722d 7075 626c 6973 682e  /docker-publish.
+000004c0: 796d 6c2f 6261 6467 652e 7376 6722 2061  yml/badge.svg" a
+000004d0: 6c74 3d22 4275 696c 6420 616e 6420 7075  lt="Build and pu
+000004e0: 626c 6973 6820 6120 446f 636b 6572 2069  blish a Docker i
+000004f0: 6d61 6765 2074 6f20 6768 6372 2e69 6f22  mage to ghcr.io"
+00000500: 3e3c 2f61 3e0a 2020 3c73 7061 6e20 7374  ></a>.  <span st
+00000510: 796c 653d 2277 6964 7468 3a20 3570 7822  yle="width: 5px"
+00000520: 3e3c 2f73 7061 6e3e 0a0a 3c61 2068 7265  ></span>..<a hre
+00000530: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00000540: 622e 636f 6d2f 6f67 757a 6861 6e2d 7969  b.com/oguzhan-yi
+00000550: 6c6d 617a 2f62 616c 636f 6e79 2f61 6374  lmaz/balcony/act
+00000560: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
+00000570: 6167 6573 2f70 6167 6573 2d62 7569 6c64  ages/pages-build
+00000580: 2d64 6570 6c6f 796d 656e 7422 3e3c 696d  -deployment"><im
+00000590: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
+000005a0: 6974 6875 622e 636f 6d2f 6f67 757a 6861  ithub.com/oguzha
+000005b0: 6e2d 7969 6c6d 617a 2f62 616c 636f 6e79  n-yilmaz/balcony
+000005c0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+000005d0: 7773 2f70 6167 6573 2f70 6167 6573 2d62  ws/pages/pages-b
+000005e0: 7569 6c64 2d64 6570 6c6f 796d 656e 742f  uild-deployment/
+000005f0: 6261 6467 652e 7376 6722 2061 6c74 3d22  badge.svg" alt="
+00000600: 4275 696c 6420 616e 6420 4465 706c 6f79  Build and Deploy
+00000610: 2044 6f63 756d 656e 7461 7469 6f6e 2077   Documentation w
+00000620: 6562 7369 7465 223e 3c2f 613e 0a3c 2f64  ebsite"></a>.</d
+00000630: 6976 3e0a 0a0a 0a62 616c 636f 6e79 2064  iv>....balcony d
+00000640: 796e 616d 6963 616c 6c79 2070 6172 7365  ynamically parse
+00000650: 7320 4157 5320 5344 4b28 6062 6f74 6f33  s AWS SDK(`boto3
+00000660: 6020 6c69 6272 6172 7929 2061 6e64 2061  ` library) and a
+00000670: 6e61 6c79 7a65 7320 7265 7175 6972 6564  nalyzes required
+00000680: 2070 6172 616d 6574 6572 7320 666f 7220   parameters for 
+00000690: 6561 6368 206f 7065 7261 7469 6f6e 2e20  each operation. 
+000006a0: 0a0a 4279 202a 2a65 7374 6162 6c69 7368  ..By **establish
+000006b0: 696e 6720 7265 6c61 7469 6f6e 7320 6265  ing relations be
+000006c0: 7477 6565 6e20 6f70 6572 6174 696f 6e73  tween operations
+000006d0: 206f 7665 7220 7265 7175 6972 6564 2070   over required p
+000006e0: 6172 616d 6574 6572 732a 2a2c 2069 7427  arameters**, it'
+000006f0: 7320 2a2a 6162 6c65 2074 6f20 6175 746f  s **able to auto
+00000700: 2d66 696c 6c2a 2a20 7468 656d 2062 7920  -fill** them by 
+00000710: 7265 6164 696e 6720 7468 6520 7265 6c61  reading the rela
+00000720: 7465 6420 6f70 6572 6174 696f 6e20 6265  ted operation be
+00000730: 666f 7265 6861 6e64 2e0a 0a42 7920 7369  forehand...By si
+00000740: 6d70 6c79 2065 6e74 6572 696e 6720 7468  mply entering th
+00000750: 6569 7220 6e61 6d65 2c20 6261 6c63 6f6e  eir name, balcon
+00000760: 7920 656e 6162 6c65 7320 6465 7665 6c6f  y enables develo
+00000770: 7065 7273 2074 6f20 6561 7369 6c79 206c  pers to easily l
+00000780: 6973 7420 7468 6569 7220 4157 5320 7265  ist their AWS re
+00000790: 736f 7572 6365 732e 0a0a 0a23 2320 496e  sources....## In
+000007a0: 7374 616c 6c61 7469 6f6e 2026 2044 6f63  stallation & Doc
+000007b0: 756d 656e 7461 7469 6f6e 200a 0a2a 2a5b  umentation ..**[
+000007c0: 6874 7470 733a 2f2f 6f67 757a 6861 6e2d  https://oguzhan-
+000007d0: 7969 6c6d 617a 2e67 6974 6875 622e 696f  yilmaz.github.io
+000007e0: 2f62 616c 636f 6e79 2f5d 2868 7474 7073  /balcony/](https
+000007f0: 3a2f 2f6f 6775 7a68 616e 2d79 696c 6d61  ://oguzhan-yilma
+00000800: 7a2e 6769 7468 7562 2e69 6f2f 6261 6c63  z.github.io/balc
+00000810: 6f6e 792f 7175 6963 6b73 7461 7274 292a  ony/quickstart)*
+00000820: 2a0a 0a42 616c 636f 6e79 2773 2064 6f63  *..Balcony's doc
+00000830: 756d 656e 7461 7469 6f6e 2077 6562 7369  umentation websi
+00000840: 7465 2063 6f6e 7461 696e 7320 7175 6963  te contains quic
+00000850: 6b73 7461 7274 2067 7569 6465 2c20 7573  kstart guide, us
+00000860: 6167 6520 636f 6f6b 626f 6f6b 2061 6e64  age cookbook and
+00000870: 206d 6f72 652e 0a23 2320 4665 6174 7572   more..## Featur
+00000880: 6573 2026 2047 4946 730a 3e20 636c 6963  es & GIFs.> clic
+00000890: 6b20 746f 2070 6c61 7920 7468 6520 7669  k to play the vi
+000008a0: 6465 6f73 0a23 2323 204c 6973 7420 6176  deos.### List av
+000008b0: 6169 6c61 626c 6520 4157 5320 5365 7276  ailable AWS Serv
+000008c0: 6963 6573 200a 6062 616c 636f 6e79 2061  ices .`balcony a
+000008d0: 7773 6020 746f 2073 6565 2065 7665 7279  ws` to see every
+000008e0: 2041 5753 2073 6572 7669 6365 2061 7661   AWS service ava
+000008f0: 696c 6162 6c65 2e0a 0a21 5b5d 2868 7474  ilable...![](htt
+00000900: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000910: 6f67 757a 6861 6e2d 7969 6c6d 617a 2f62  oguzhan-yilmaz/b
+00000920: 616c 636f 6e79 2f62 6c6f 622f 6d61 696e  alcony/blob/main
+00000930: 2f64 6f63 732f 7669 7375 616c 732f 6177  /docs/visuals/aw
+00000940: 732d 7365 7276 6963 6573 2d6c 6973 742e  s-services-list.
+00000950: 6769 6629 0a0a 0a23 2323 204c 6973 7420  gif)...### List 
+00000960: 5265 736f 7572 6365 204e 6f64 6573 206f  Resource Nodes o
+00000970: 6620 616e 2041 5753 2053 6572 7669 6365  f an AWS Service
+00000980: 200a 6062 616c 636f 6e79 2061 7773 203c   .`balcony aws <
+00000990: 7365 7276 6963 652d 6e61 6d65 3e60 2074  service-name>` t
+000009a0: 6f20 7365 6520 6576 6572 7920 5265 736f  o see every Reso
+000009b0: 7572 6365 204e 6f64 6520 6f66 2061 2073  urce Node of a s
+000009c0: 6572 7669 6365 2e0a 0a21 5b5d 2868 7474  ervice...![](htt
+000009d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000009e0: 6f67 757a 6861 6e2d 7969 6c6d 617a 2f62  oguzhan-yilmaz/b
+000009f0: 616c 636f 6e79 2f62 6c6f 622f 6d61 696e  alcony/blob/main
+00000a00: 2f64 6f63 732f 7669 7375 616c 732f 7265  /docs/visuals/re
+00000a10: 736f 7572 6365 2d6e 6f64 652d 6c69 7374  source-node-list
+00000a20: 2e67 6966 290a 0a0a 2323 2320 5265 6164  .gif)...### Read
+00000a30: 696e 6720 6120 5265 736f 7572 6365 204e  ing a Resource N
+00000a40: 6f64 6520 0a60 6261 6c63 6f6e 7920 6177  ode .`balcony aw
+00000a50: 7320 3c73 6572 7669 6365 2d6e 616d 653e  s <service-name>
+00000a60: 203c 7265 736f 7572 6365 2d6e 6f64 653e   <resource-node>
+00000a70: 6020 746f 2072 6561 6420 6f70 6572 6174  ` to read operat
+00000a80: 696f 6e73 206f 6620 6120 5265 736f 7572  ions of a Resour
+00000a90: 6365 204e 6f64 652e 0a0a 215b 5d28 6874  ce Node...![](ht
+00000aa0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000ab0: 2f6f 6775 7a68 616e 2d79 696c 6d61 7a2f  /oguzhan-yilmaz/
+00000ac0: 6261 6c63 6f6e 792f 626c 6f62 2f6d 6169  balcony/blob/mai
+00000ad0: 6e2f 646f 6373 2f76 6973 7561 6c73 2f72  n/docs/visuals/r
+00000ae0: 6561 6469 6e67 2d61 2d72 6573 6f75 7263  eading-a-resourc
+00000af0: 652d 6e6f 6465 2e67 6966 290a 0a0a 2323  e-node.gif)...##
+00000b00: 2320 446f 6375 6d65 6e74 6174 696f 6e20  # Documentation 
+00000b10: 616e 6420 496e 7075 7420 2620 4f75 7470  and Input & Outp
+00000b20: 7574 206f 6620 4f70 6572 6174 696f 6e73  ut of Operations
+00000b30: 0a55 7365 2074 6865 2060 2d2d 6c69 7374  .Use the `--list
+00000b40: 602c 2060 2d6c 6020 666c 6167 2074 6f20  `, `-l` flag to 
+00000b50: 7072 696e 7420 7468 6520 6769 7665 6e20  print the given 
+00000b60: 4157 5320 4150 4920 4f70 6572 6174 696f  AWS API Operatio
+00000b70: 6e73 2064 6f63 756d 656e 7461 7469 6f6e  ns documentation
+00000b80: 2c20 696e 7075 7420 2620 6f75 7470 7574  , input & output
+00000b90: 2073 7472 7563 7475 7265 2e20 0a20 0a0a   structure. . ..
+00000ba0: 215b 5d28 6874 7470 733a 2f2f 6769 7468  ![](https://gith
+00000bb0: 7562 2e63 6f6d 2f6f 6775 7a68 616e 2d79  ub.com/oguzhan-y
+00000bc0: 696c 6d61 7a2f 6261 6c63 6f6e 792f 626c  ilmaz/balcony/bl
+00000bd0: 6f62 2f6d 6169 6e2f 646f 6373 2f76 6973  ob/main/docs/vis
+00000be0: 7561 6c73 2f6c 6973 742d 6f70 7469 6f6e  uals/list-option
+00000bf0: 2e67 6966 290a 0a0a 2323 2320 456e 6162  .gif)...### Enab
+00000c00: 6c65 2044 6562 7567 206d 6573 7361 6765  le Debug message
+00000c10: 7320 0a55 7365 2074 6865 2060 2d2d 6465  s .Use the `--de
+00000c20: 6275 6760 2c20 602d 6460 2066 6c61 6720  bug`, `-d` flag 
+00000c30: 746f 2073 6565 2077 6861 7427 7320 676f  to see what's go
+00000c40: 696e 6720 6f6e 2075 6e64 6572 2074 6865  ing on under the
+00000c50: 2068 6f6f 6421 0a0a 215b 5d28 6874 7470   hood!..![](http
+00000c60: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
+00000c70: 6775 7a68 616e 2d79 696c 6d61 7a2f 6261  guzhan-yilmaz/ba
+00000c80: 6c63 6f6e 792f 626c 6f62 2f6d 6169 6e2f  lcony/blob/main/
+00000c90: 646f 6373 2f76 6973 7561 6c73 2f64 6562  docs/visuals/deb
+00000ca0: 7567 2d6d 6573 7361 6765 732e 6769 6629  ug-messages.gif)
+00000cb0: 0a0a                                     ..
```

