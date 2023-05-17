# Comparing `tmp/cert-schema-3.4.0.tar.gz` & `tmp/cert-schema-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cert-schema-3.4.0.tar", last modified: Thu Mar 30 13:06:31 2023, max compression
+gzip compressed data, was "cert-schema-3.4.2.tar", last modified: Wed May 17 13:48:56 2023, max compression
```

## Comparing `cert-schema-3.4.0.tar` & `cert-schema-3.4.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.140180 cert-schema-3.4.0/
--rw-r--r--   0 julien     (503) staff       (20)     1096 2021-04-08 16:27:50.000000 cert-schema-3.4.0/LICENSE
--rw-r--r--   0 julien     (503) staff       (20)       47 2021-04-08 16:27:50.000000 cert-schema-3.4.0/MANIFEST.in
--rw-r--r--   0 julien     (503) staff       (20)     4156 2023-03-30 13:06:31.140576 cert-schema-3.4.0/PKG-INFO
--rw-r--r--   0 julien     (503) staff       (20)     3283 2021-04-08 16:27:50.000000 cert-schema-3.4.0/README.md
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.054056 cert-schema-3.4.0/cert_schema/
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.064229 cert-schema-3.4.0/cert_schema/1.1/
--rw-r--r--   0 julien     (503) staff       (20)     8207 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/1.1/certificate-schema-v1-1.json
--rw-r--r--   0 julien     (503) staff       (20)     1558 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/1.1/issuer-schema-v1-1.json
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.072311 cert-schema-3.4.0/cert_schema/1.2/
--rw-r--r--   0 julien     (503) staff       (20)     4174 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/1.2/assertion-1.2.json
--rw-r--r--   0 julien     (503) staff       (20)     2406 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/1.2/blockchain-certificate-1.2.json
--rw-r--r--   0 julien     (503) staff       (20)     2912 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/1.2/blockchain-receipt-1.2.json
--rw-r--r--   0 julien     (503) staff       (20)     3607 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/1.2/certificate-1.2.json
--rw-r--r--   0 julien     (503) staff       (20)     5557 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/1.2/certificate-document-1.2.json
--rw-r--r--   0 julien     (503) staff       (20)     5343 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/1.2/context.json
--rw-r--r--   0 julien     (503) staff       (20)     3321 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/1.2/issuer-1.2.json
--rw-r--r--   0 julien     (503) staff       (20)     3240 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/1.2/issuer-id-1.2.json
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.079712 cert-schema-3.4.0/cert_schema/2.0/
--rw-r--r--   0 julien     (503) staff       (20)     1888 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0/context.json
--rw-r--r--   0 julien     (503) staff       (20)     6472 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0/issuerSchema.json
--rw-r--r--   0 julien     (503) staff       (20)     1521 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0/merkleProof2017Schema.json
--rw-r--r--   0 julien     (503) staff       (20)     4494 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0/obi.json
--rw-r--r--   0 julien     (503) staff       (20)     1085 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0/recipientSchema.json
--rw-r--r--   0 julien     (503) staff       (20)    11948 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0/schema.json
--rw-r--r--   0 julien     (503) staff       (20)     1237 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0/signatureLineSchema.json
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.087052 cert-schema-3.4.0/cert_schema/2.0-alpha/
--rw-r--r--   0 julien     (503) staff       (20)     1951 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0-alpha/context.json
--rw-r--r--   0 julien     (503) staff       (20)     7035 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0-alpha/issuerSchema.json
--rw-r--r--   0 julien     (503) staff       (20)     1430 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0-alpha/merkleProof2017Schema.json
--rw-r--r--   0 julien     (503) staff       (20)     1085 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0-alpha/recipientSchema.json
--rw-r--r--   0 julien     (503) staff       (20)    14584 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0-alpha/schema.json
--rw-r--r--   0 julien     (503) staff       (20)     1237 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.0-alpha/signatureLineSchema.json
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.094206 cert-schema-3.4.0/cert_schema/2.1/
--rw-r--r--   0 julien     (503) staff       (20)     1888 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.1/context.json
--rw-r--r--   0 julien     (503) staff       (20)     6472 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.1/issuerSchema.json
--rw-r--r--   0 julien     (503) staff       (20)     1521 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.1/merkleProof2017Schema.json
--rw-r--r--   0 julien     (503) staff       (20)     4494 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.1/obi.json
--rw-r--r--   0 julien     (503) staff       (20)     1085 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.1/recipientSchema.json
--rw-r--r--   0 julien     (503) staff       (20)    11948 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.1/schema.json
--rw-r--r--   0 julien     (503) staff       (20)     1237 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/2.1/signatureLineSchema.json
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.106823 cert-schema-3.4.0/cert_schema/3.0/
--rw-r--r--   0 julien     (503) staff       (20)      703 2021-12-03 14:49:12.000000 cert-schema-3.4.0/cert_schema/3.0/claimSchema.json
--rw-r--r--   0 julien     (503) staff       (20)     1800 2022-06-16 15:34:06.000000 cert-schema-3.4.0/cert_schema/3.0/context.json
--rw-r--r--   0 julien     (503) staff       (20)     7308 2021-10-05 15:30:06.000000 cert-schema-3.4.0/cert_schema/3.0/credential.json
--rw-r--r--   0 julien     (503) staff       (20)     1499 2022-03-08 17:50:38.000000 cert-schema-3.4.0/cert_schema/3.0/credentialSubjectSchema.json
--rw-r--r--   0 julien     (503) staff       (20)      796 2021-12-03 13:09:37.000000 cert-schema-3.4.0/cert_schema/3.0/displaySchema.json
--rw-r--r--   0 julien     (503) staff       (20)      929 2022-06-16 15:34:40.000000 cert-schema-3.4.0/cert_schema/3.0/merkleProof2019Context.json
--rw-r--r--   0 julien     (503) staff       (20)     2823 2021-12-03 14:53:56.000000 cert-schema-3.4.0/cert_schema/3.0/merkleProof2019Schema.json
--rw-r--r--   0 julien     (503) staff       (20)     5078 2021-12-08 14:45:05.000000 cert-schema-3.4.0/cert_schema/3.0/schema.json
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.113387 cert-schema-3.4.0/cert_schema/3.0-alpha/
--rw-r--r--   0 julien     (503) staff       (20)     1142 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/3.0-alpha/context.json
--rw-r--r--   0 julien     (503) staff       (20)     7308 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/3.0-alpha/credential.json
--rw-r--r--   0 julien     (503) staff       (20)     1767 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/3.0-alpha/exampleCredential.json
--rw-r--r--   0 julien     (503) staff       (20)     7477 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/3.0-alpha/issuerSchema.json
--rw-r--r--   0 julien     (503) staff       (20)      934 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/3.0-alpha/merkleProof2019Context.json
--rw-r--r--   0 julien     (503) staff       (20)     2829 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/3.0-alpha/merkleProof2019Schema.json
--rw-r--r--   0 julien     (503) staff       (20)     3883 2021-10-05 15:30:06.000000 cert-schema-3.4.0/cert_schema/3.0-alpha/schema.json
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.121906 cert-schema-3.4.0/cert_schema/3.0-beta/
--rw-r--r--   0 julien     (503) staff       (20)     1810 2021-10-05 15:30:06.000000 cert-schema-3.4.0/cert_schema/3.0-beta/context.json
--rw-r--r--   0 julien     (503) staff       (20)     7308 2021-10-05 15:30:06.000000 cert-schema-3.4.0/cert_schema/3.0-beta/credential.json
--rw-r--r--   0 julien     (503) staff       (20)      755 2021-10-05 15:30:06.000000 cert-schema-3.4.0/cert_schema/3.0-beta/displaySchema.json
--rw-r--r--   0 julien     (503) staff       (20)     1767 2021-10-05 15:30:06.000000 cert-schema-3.4.0/cert_schema/3.0-beta/exampleCredential.json
--rw-r--r--   0 julien     (503) staff       (20)      934 2021-10-05 15:30:06.000000 cert-schema-3.4.0/cert_schema/3.0-beta/merkleProof2019Context.json
--rw-r--r--   0 julien     (503) staff       (20)     2829 2021-10-05 15:30:06.000000 cert-schema-3.4.0/cert_schema/3.0-beta/merkleProof2019Schema.json
--rw-r--r--   0 julien     (503) staff       (20)     4432 2021-12-08 14:45:05.000000 cert-schema-3.4.0/cert_schema/3.0-beta/schema.json
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.135389 cert-schema-3.4.0/cert_schema/3.1/
--rw-r--r--   0 julien     (503) staff       (20)     2575 2022-06-20 17:53:03.000000 cert-schema-3.4.0/cert_schema/3.1/chainedProof2021Context.json
--rw-r--r--   0 julien     (503) staff       (20)      703 2021-12-03 14:49:12.000000 cert-schema-3.4.0/cert_schema/3.1/claimSchema.json
--rw-r--r--   0 julien     (503) staff       (20)     1753 2022-05-10 14:38:30.000000 cert-schema-3.4.0/cert_schema/3.1/context.json
--rw-r--r--   0 julien     (503) staff       (20)     7308 2021-10-05 15:30:06.000000 cert-schema-3.4.0/cert_schema/3.1/credential.json
--rw-r--r--   0 julien     (503) staff       (20)     1499 2022-03-08 17:50:38.000000 cert-schema-3.4.0/cert_schema/3.1/credentialSubjectSchema.json
--rw-r--r--   0 julien     (503) staff       (20)      796 2021-12-03 13:09:37.000000 cert-schema-3.4.0/cert_schema/3.1/displaySchema.json
--rw-r--r--   0 julien     (503) staff       (20)     2321 2022-06-20 17:53:03.000000 cert-schema-3.4.0/cert_schema/3.1/merkleProof2019Context.json
--rw-r--r--   0 julien     (503) staff       (20)     2823 2021-12-03 14:53:56.000000 cert-schema-3.4.0/cert_schema/3.1/merkleProof2019Schema.json
--rw-r--r--   0 julien     (503) staff       (20)     5078 2021-12-08 14:45:05.000000 cert-schema-3.4.0/cert_schema/3.1/schema.json
--rw-r--r--   0 julien     (503) staff       (20)     1274 2023-03-30 13:05:28.000000 cert-schema-3.4.0/cert_schema/3.1/statusList2021Context.json
--rw-r--r--   0 julien     (503) staff       (20)      779 2022-09-12 12:16:52.000000 cert-schema-3.4.0/cert_schema/__init__.py
--rw-r--r--   0 julien     (503) staff       (20)       21 2023-03-30 13:06:27.000000 cert-schema-3.4.0/cert_schema/__version__.py
--rw-r--r--   0 julien     (503) staff       (20)     1435 2023-03-30 13:05:28.000000 cert-schema-3.4.0/cert_schema/context_urls.json
--rw-r--r--   0 julien     (503) staff       (20)     2534 2023-03-30 13:05:28.000000 cert-schema-3.4.0/cert_schema/context_urls.py
--rw-r--r--   0 julien     (503) staff       (20)       97 2021-04-08 16:27:50.000000 cert-schema-3.4.0/cert_schema/errors.py
--rw-r--r--   0 julien     (503) staff       (20)    10982 2023-03-30 13:05:28.000000 cert-schema-3.4.0/cert_schema/jsonld_helpers.py
--rw-r--r--   0 julien     (503) staff       (20)     4263 2021-12-08 14:45:05.000000 cert-schema-3.4.0/cert_schema/schema_validator.py
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.058312 cert-schema-3.4.0/cert_schema.egg-info/
--rw-r--r--   0 julien     (503) staff       (20)     4156 2023-03-30 13:06:30.000000 cert-schema-3.4.0/cert_schema.egg-info/PKG-INFO
--rw-r--r--   0 julien     (503) staff       (20)     2892 2023-03-30 13:06:30.000000 cert-schema-3.4.0/cert_schema.egg-info/SOURCES.txt
--rw-r--r--   0 julien     (503) staff       (20)        1 2023-03-30 13:06:30.000000 cert-schema-3.4.0/cert_schema.egg-info/dependency_links.txt
--rw-r--r--   0 julien     (503) staff       (20)       77 2023-03-30 13:06:30.000000 cert-schema-3.4.0/cert_schema.egg-info/requires.txt
--rw-r--r--   0 julien     (503) staff       (20)       18 2023-03-30 13:06:30.000000 cert-schema-3.4.0/cert_schema.egg-info/top_level.txt
--rw-r--r--   0 julien     (503) staff       (20)       77 2021-04-08 16:27:50.000000 cert-schema-3.4.0/requirements.txt
--rw-r--r--   0 julien     (503) staff       (20)      137 2023-03-30 13:06:31.141489 cert-schema-3.4.0/setup.cfg
--rw-r--r--   0 julien     (503) staff       (20)      994 2022-10-13 15:39:33.000000 cert-schema-3.4.0/setup.py
-drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-03-30 13:06:31.138831 cert-schema-3.4.0/tests/
--rw-r--r--   0 julien     (503) staff       (20)        0 2021-04-08 16:27:50.000000 cert-schema-3.4.0/tests/__init__.py
--rw-r--r--   0 julien     (503) staff       (20)     4296 2023-03-30 13:05:28.000000 cert-schema-3.4.0/tests/test_context_urls.py
--rw-r--r--   0 julien     (503) staff       (20)     2973 2022-06-17 18:10:03.000000 cert-schema-3.4.0/tests/test_jsonld_helpers.py
--rw-r--r--   0 julien     (503) staff       (20)     3218 2021-12-08 14:45:05.000000 cert-schema-3.4.0/tests/test_schema_validator.py
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.403968 cert-schema-3.4.2/
+-rw-r--r--   0 julien     (503) staff       (20)     1096 2021-04-08 16:27:50.000000 cert-schema-3.4.2/LICENSE
+-rw-r--r--   0 julien     (503) staff       (20)       47 2021-04-08 16:27:50.000000 cert-schema-3.4.2/MANIFEST.in
+-rw-r--r--   0 julien     (503) staff       (20)     4156 2023-05-17 13:48:56.404506 cert-schema-3.4.2/PKG-INFO
+-rw-r--r--   0 julien     (503) staff       (20)     3283 2021-04-08 16:27:50.000000 cert-schema-3.4.2/README.md
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.324014 cert-schema-3.4.2/cert_schema/
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.327717 cert-schema-3.4.2/cert_schema/1.1/
+-rw-r--r--   0 julien     (503) staff       (20)     8207 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/1.1/certificate-schema-v1-1.json
+-rw-r--r--   0 julien     (503) staff       (20)     1558 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/1.1/issuer-schema-v1-1.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.333840 cert-schema-3.4.2/cert_schema/1.2/
+-rw-r--r--   0 julien     (503) staff       (20)     4174 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/1.2/assertion-1.2.json
+-rw-r--r--   0 julien     (503) staff       (20)     2406 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/1.2/blockchain-certificate-1.2.json
+-rw-r--r--   0 julien     (503) staff       (20)     2912 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/1.2/blockchain-receipt-1.2.json
+-rw-r--r--   0 julien     (503) staff       (20)     3607 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/1.2/certificate-1.2.json
+-rw-r--r--   0 julien     (503) staff       (20)     5557 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/1.2/certificate-document-1.2.json
+-rw-r--r--   0 julien     (503) staff       (20)     5343 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/1.2/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     3321 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/1.2/issuer-1.2.json
+-rw-r--r--   0 julien     (503) staff       (20)     3240 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/1.2/issuer-id-1.2.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.341166 cert-schema-3.4.2/cert_schema/2.0/
+-rw-r--r--   0 julien     (503) staff       (20)     1888 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     6472 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0/issuerSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1521 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0/merkleProof2017Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     4494 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0/obi.json
+-rw-r--r--   0 julien     (503) staff       (20)     1085 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0/recipientSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)    11948 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0/schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1237 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0/signatureLineSchema.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.346632 cert-schema-3.4.2/cert_schema/2.0-alpha/
+-rw-r--r--   0 julien     (503) staff       (20)     1951 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0-alpha/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     7035 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0-alpha/issuerSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1430 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0-alpha/merkleProof2017Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1085 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0-alpha/recipientSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)    14584 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0-alpha/schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1237 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.0-alpha/signatureLineSchema.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.354650 cert-schema-3.4.2/cert_schema/2.1/
+-rw-r--r--   0 julien     (503) staff       (20)     1888 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.1/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     6472 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.1/issuerSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1521 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.1/merkleProof2017Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     4494 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.1/obi.json
+-rw-r--r--   0 julien     (503) staff       (20)     1085 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.1/recipientSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)    11948 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.1/schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1237 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/2.1/signatureLineSchema.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.364636 cert-schema-3.4.2/cert_schema/3.0/
+-rw-r--r--   0 julien     (503) staff       (20)      703 2021-12-03 14:49:12.000000 cert-schema-3.4.2/cert_schema/3.0/claimSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1800 2022-06-16 15:34:06.000000 cert-schema-3.4.2/cert_schema/3.0/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     7308 2021-10-05 15:30:06.000000 cert-schema-3.4.2/cert_schema/3.0/credential.json
+-rw-r--r--   0 julien     (503) staff       (20)     1499 2022-03-08 17:50:38.000000 cert-schema-3.4.2/cert_schema/3.0/credentialSubjectSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)      796 2021-12-03 13:09:37.000000 cert-schema-3.4.2/cert_schema/3.0/displaySchema.json
+-rw-r--r--   0 julien     (503) staff       (20)      929 2022-06-16 15:34:40.000000 cert-schema-3.4.2/cert_schema/3.0/merkleProof2019Context.json
+-rw-r--r--   0 julien     (503) staff       (20)     2823 2021-12-03 14:53:56.000000 cert-schema-3.4.2/cert_schema/3.0/merkleProof2019Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     5078 2021-12-08 14:45:05.000000 cert-schema-3.4.2/cert_schema/3.0/schema.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.372803 cert-schema-3.4.2/cert_schema/3.0-alpha/
+-rw-r--r--   0 julien     (503) staff       (20)     1142 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/3.0-alpha/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     7308 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/3.0-alpha/credential.json
+-rw-r--r--   0 julien     (503) staff       (20)     1767 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/3.0-alpha/exampleCredential.json
+-rw-r--r--   0 julien     (503) staff       (20)     7477 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/3.0-alpha/issuerSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)      934 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/3.0-alpha/merkleProof2019Context.json
+-rw-r--r--   0 julien     (503) staff       (20)     2829 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/3.0-alpha/merkleProof2019Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     3883 2021-10-05 15:30:06.000000 cert-schema-3.4.2/cert_schema/3.0-alpha/schema.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.380904 cert-schema-3.4.2/cert_schema/3.0-beta/
+-rw-r--r--   0 julien     (503) staff       (20)     1810 2021-10-05 15:30:06.000000 cert-schema-3.4.2/cert_schema/3.0-beta/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     7308 2021-10-05 15:30:06.000000 cert-schema-3.4.2/cert_schema/3.0-beta/credential.json
+-rw-r--r--   0 julien     (503) staff       (20)      755 2021-10-05 15:30:06.000000 cert-schema-3.4.2/cert_schema/3.0-beta/displaySchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1767 2021-10-05 15:30:06.000000 cert-schema-3.4.2/cert_schema/3.0-beta/exampleCredential.json
+-rw-r--r--   0 julien     (503) staff       (20)      934 2021-10-05 15:30:06.000000 cert-schema-3.4.2/cert_schema/3.0-beta/merkleProof2019Context.json
+-rw-r--r--   0 julien     (503) staff       (20)     2829 2021-10-05 15:30:06.000000 cert-schema-3.4.2/cert_schema/3.0-beta/merkleProof2019Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     4432 2021-12-08 14:45:05.000000 cert-schema-3.4.2/cert_schema/3.0-beta/schema.json
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.392333 cert-schema-3.4.2/cert_schema/3.1/
+-rw-r--r--   0 julien     (503) staff       (20)     2575 2022-06-20 17:53:03.000000 cert-schema-3.4.2/cert_schema/3.1/chainedProof2021Context.json
+-rw-r--r--   0 julien     (503) staff       (20)      703 2021-12-03 14:49:12.000000 cert-schema-3.4.2/cert_schema/3.1/claimSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1753 2022-05-10 14:38:30.000000 cert-schema-3.4.2/cert_schema/3.1/context.json
+-rw-r--r--   0 julien     (503) staff       (20)     7308 2021-10-05 15:30:06.000000 cert-schema-3.4.2/cert_schema/3.1/credential.json
+-rw-r--r--   0 julien     (503) staff       (20)     1499 2022-03-08 17:50:38.000000 cert-schema-3.4.2/cert_schema/3.1/credentialSubjectSchema.json
+-rw-r--r--   0 julien     (503) staff       (20)      796 2021-12-03 13:09:37.000000 cert-schema-3.4.2/cert_schema/3.1/displaySchema.json
+-rw-r--r--   0 julien     (503) staff       (20)     2321 2022-06-20 17:53:03.000000 cert-schema-3.4.2/cert_schema/3.1/merkleProof2019Context.json
+-rw-r--r--   0 julien     (503) staff       (20)     2823 2021-12-03 14:53:56.000000 cert-schema-3.4.2/cert_schema/3.1/merkleProof2019Schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     5078 2021-12-08 14:45:05.000000 cert-schema-3.4.2/cert_schema/3.1/schema.json
+-rw-r--r--   0 julien     (503) staff       (20)     1274 2023-03-30 13:05:28.000000 cert-schema-3.4.2/cert_schema/3.1/statusList2021Context.json
+-rw-r--r--   0 julien     (503) staff       (20)      814 2023-05-17 13:48:13.000000 cert-schema-3.4.2/cert_schema/__init__.py
+-rw-r--r--   0 julien     (503) staff       (20)       21 2023-05-17 13:48:45.000000 cert-schema-3.4.2/cert_schema/__version__.py
+-rw-r--r--   0 julien     (503) staff       (20)     1435 2023-03-30 13:05:28.000000 cert-schema-3.4.2/cert_schema/context_urls.json
+-rw-r--r--   0 julien     (503) staff       (20)     2534 2023-03-30 13:05:28.000000 cert-schema-3.4.2/cert_schema/context_urls.py
+-rw-r--r--   0 julien     (503) staff       (20)       97 2021-04-08 16:27:50.000000 cert-schema-3.4.2/cert_schema/errors.py
+-rw-r--r--   0 julien     (503) staff       (20)    10982 2023-03-30 13:05:28.000000 cert-schema-3.4.2/cert_schema/jsonld_helpers.py
+-rw-r--r--   0 julien     (503) staff       (20)     4263 2021-12-08 14:45:05.000000 cert-schema-3.4.2/cert_schema/schema_validator.py
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.326449 cert-schema-3.4.2/cert_schema.egg-info/
+-rw-r--r--   0 julien     (503) staff       (20)     4156 2023-05-17 13:48:55.000000 cert-schema-3.4.2/cert_schema.egg-info/PKG-INFO
+-rw-r--r--   0 julien     (503) staff       (20)     2892 2023-05-17 13:48:56.000000 cert-schema-3.4.2/cert_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 julien     (503) staff       (20)        1 2023-05-17 13:48:55.000000 cert-schema-3.4.2/cert_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 julien     (503) staff       (20)       77 2023-05-17 13:48:55.000000 cert-schema-3.4.2/cert_schema.egg-info/requires.txt
+-rw-r--r--   0 julien     (503) staff       (20)       18 2023-05-17 13:48:55.000000 cert-schema-3.4.2/cert_schema.egg-info/top_level.txt
+-rw-r--r--   0 julien     (503) staff       (20)       77 2021-04-08 16:27:50.000000 cert-schema-3.4.2/requirements.txt
+-rw-r--r--   0 julien     (503) staff       (20)      137 2023-05-17 13:48:56.410104 cert-schema-3.4.2/setup.cfg
+-rw-r--r--   0 julien     (503) staff       (20)      994 2022-10-13 15:39:33.000000 cert-schema-3.4.2/setup.py
+drwxr-xr-x   0 julien     (503) staff       (20)        0 2023-05-17 13:48:56.399660 cert-schema-3.4.2/tests/
+-rw-r--r--   0 julien     (503) staff       (20)        0 2021-04-08 16:27:50.000000 cert-schema-3.4.2/tests/__init__.py
+-rw-r--r--   0 julien     (503) staff       (20)     4296 2023-03-30 13:05:28.000000 cert-schema-3.4.2/tests/test_context_urls.py
+-rw-r--r--   0 julien     (503) staff       (20)     2973 2022-06-17 18:10:03.000000 cert-schema-3.4.2/tests/test_jsonld_helpers.py
+-rw-r--r--   0 julien     (503) staff       (20)     3218 2021-12-08 14:45:05.000000 cert-schema-3.4.2/tests/test_schema_validator.py
```

### Comparing `cert-schema-3.4.0/LICENSE` & `cert-schema-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/PKG-INFO` & `cert-schema-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cert-schema
-Version: 3.4.0
+Version: 3.4.2
 Summary: Blockchain certificates JSON-LD context and JSON schemas
 Home-page: https://github.com/blockchain-certificates/cert-schema
 Author: info@blockcerts.org
 Author-email: info@blockcerts.org
 License: MIT
 Description: [![Build Status](https://travis-ci.org/blockchain-certificates/cert-schema.svg?branch=master)](https://travis-ci.org/blockchain-certificates/cert-schema)
         [![PyPI version](https://badge.fury.io/py/cert-schema.svg)](https://badge.fury.io/py/cert-schema)
```

### Comparing `cert-schema-3.4.0/README.md` & `cert-schema-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/1.1/certificate-schema-v1-1.json` & `cert-schema-3.4.2/cert_schema/1.1/certificate-schema-v1-1.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/1.1/issuer-schema-v1-1.json` & `cert-schema-3.4.2/cert_schema/1.1/issuer-schema-v1-1.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/1.2/assertion-1.2.json` & `cert-schema-3.4.2/cert_schema/1.2/assertion-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/1.2/blockchain-certificate-1.2.json` & `cert-schema-3.4.2/cert_schema/1.2/blockchain-certificate-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/1.2/blockchain-receipt-1.2.json` & `cert-schema-3.4.2/cert_schema/1.2/blockchain-receipt-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/1.2/certificate-1.2.json` & `cert-schema-3.4.2/cert_schema/1.2/certificate-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/1.2/certificate-document-1.2.json` & `cert-schema-3.4.2/cert_schema/1.2/certificate-document-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/1.2/context.json` & `cert-schema-3.4.2/cert_schema/1.2/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/1.2/issuer-1.2.json` & `cert-schema-3.4.2/cert_schema/1.2/issuer-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/1.2/issuer-id-1.2.json` & `cert-schema-3.4.2/cert_schema/1.2/issuer-id-1.2.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0/context.json` & `cert-schema-3.4.2/cert_schema/2.0/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0/issuerSchema.json` & `cert-schema-3.4.2/cert_schema/2.0/issuerSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0/merkleProof2017Schema.json` & `cert-schema-3.4.2/cert_schema/2.0/merkleProof2017Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0/obi.json` & `cert-schema-3.4.2/cert_schema/2.0/obi.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0/recipientSchema.json` & `cert-schema-3.4.2/cert_schema/2.0/recipientSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0/schema.json` & `cert-schema-3.4.2/cert_schema/2.0/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0/signatureLineSchema.json` & `cert-schema-3.4.2/cert_schema/2.0/signatureLineSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0-alpha/context.json` & `cert-schema-3.4.2/cert_schema/2.0-alpha/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0-alpha/issuerSchema.json` & `cert-schema-3.4.2/cert_schema/2.0-alpha/issuerSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0-alpha/merkleProof2017Schema.json` & `cert-schema-3.4.2/cert_schema/2.0-alpha/merkleProof2017Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0-alpha/recipientSchema.json` & `cert-schema-3.4.2/cert_schema/2.0-alpha/recipientSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0-alpha/schema.json` & `cert-schema-3.4.2/cert_schema/2.0-alpha/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.0-alpha/signatureLineSchema.json` & `cert-schema-3.4.2/cert_schema/2.0-alpha/signatureLineSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.1/context.json` & `cert-schema-3.4.2/cert_schema/2.1/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.1/issuerSchema.json` & `cert-schema-3.4.2/cert_schema/2.1/issuerSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.1/merkleProof2017Schema.json` & `cert-schema-3.4.2/cert_schema/2.1/merkleProof2017Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.1/obi.json` & `cert-schema-3.4.2/cert_schema/2.1/obi.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.1/recipientSchema.json` & `cert-schema-3.4.2/cert_schema/2.1/recipientSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.1/schema.json` & `cert-schema-3.4.2/cert_schema/2.1/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/2.1/signatureLineSchema.json` & `cert-schema-3.4.2/cert_schema/2.1/signatureLineSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0/claimSchema.json` & `cert-schema-3.4.2/cert_schema/3.0/claimSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0/context.json` & `cert-schema-3.4.2/cert_schema/3.0/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0/credential.json` & `cert-schema-3.4.2/cert_schema/3.0/credential.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0/credentialSubjectSchema.json` & `cert-schema-3.4.2/cert_schema/3.0/credentialSubjectSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0/displaySchema.json` & `cert-schema-3.4.2/cert_schema/3.0/displaySchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0/merkleProof2019Context.json` & `cert-schema-3.4.2/cert_schema/3.0/merkleProof2019Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0/merkleProof2019Schema.json` & `cert-schema-3.4.2/cert_schema/3.0/merkleProof2019Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0/schema.json` & `cert-schema-3.4.2/cert_schema/3.0/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-alpha/context.json` & `cert-schema-3.4.2/cert_schema/3.0-alpha/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-alpha/credential.json` & `cert-schema-3.4.2/cert_schema/3.0-alpha/credential.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-alpha/exampleCredential.json` & `cert-schema-3.4.2/cert_schema/3.0-alpha/exampleCredential.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-alpha/issuerSchema.json` & `cert-schema-3.4.2/cert_schema/3.0-alpha/issuerSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-alpha/merkleProof2019Context.json` & `cert-schema-3.4.2/cert_schema/3.0-alpha/merkleProof2019Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-alpha/merkleProof2019Schema.json` & `cert-schema-3.4.2/cert_schema/3.0-alpha/merkleProof2019Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-alpha/schema.json` & `cert-schema-3.4.2/cert_schema/3.0-alpha/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-beta/context.json` & `cert-schema-3.4.2/cert_schema/3.0-beta/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-beta/credential.json` & `cert-schema-3.4.2/cert_schema/3.0-beta/credential.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-beta/displaySchema.json` & `cert-schema-3.4.2/cert_schema/3.0-beta/displaySchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-beta/exampleCredential.json` & `cert-schema-3.4.2/cert_schema/3.0-beta/exampleCredential.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-beta/merkleProof2019Context.json` & `cert-schema-3.4.2/cert_schema/3.0-beta/merkleProof2019Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-beta/merkleProof2019Schema.json` & `cert-schema-3.4.2/cert_schema/3.0-beta/merkleProof2019Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.0-beta/schema.json` & `cert-schema-3.4.2/cert_schema/3.0-beta/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.1/chainedProof2021Context.json` & `cert-schema-3.4.2/cert_schema/3.1/chainedProof2021Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.1/claimSchema.json` & `cert-schema-3.4.2/cert_schema/3.1/claimSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.1/context.json` & `cert-schema-3.4.2/cert_schema/3.1/context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.1/credential.json` & `cert-schema-3.4.2/cert_schema/3.1/credential.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.1/credentialSubjectSchema.json` & `cert-schema-3.4.2/cert_schema/3.1/credentialSubjectSchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.1/displaySchema.json` & `cert-schema-3.4.2/cert_schema/3.1/displaySchema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.1/merkleProof2019Context.json` & `cert-schema-3.4.2/cert_schema/3.1/merkleProof2019Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.1/merkleProof2019Schema.json` & `cert-schema-3.4.2/cert_schema/3.1/merkleProof2019Schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.1/schema.json` & `cert-schema-3.4.2/cert_schema/3.1/schema.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/3.1/statusList2021Context.json` & `cert-schema-3.4.2/cert_schema/3.1/statusList2021Context.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/__init__.py` & `cert-schema-3.4.2/cert_schema/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from cert_schema.jsonld_helpers import jsonld_document_loader, normalize_jsonld, extend_preloaded_context
+from cert_schema.jsonld_helpers import jsonld_document_loader, normalize_jsonld, extend_preloaded_context, preloaded_context_document_loader
 from cert_schema.schema_validator import validate_unsigned_v1_2, validate_v1_2, validate_v2, validate_v2_1,\
     validate_v3
 from cert_schema.context_urls import ContextUrls
 
 # Prefer consuming from ContextUrls, maintained here for backwards compatibility, will not get updated
 from cert_schema.jsonld_helpers import BLOCKCERTS_V3_CANONICAL_CONTEXT, BLOCKCERTS_V3_CONTEXT, \
     VERIFIABLE_CREDENTIAL_V1_CONTEXT, BLOCKCERTS_V2_CONTEXT, \
```

### Comparing `cert-schema-3.4.0/cert_schema/context_urls.json` & `cert-schema-3.4.2/cert_schema/context_urls.json`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/context_urls.py` & `cert-schema-3.4.2/cert_schema/context_urls.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/jsonld_helpers.py` & `cert-schema-3.4.2/cert_schema/jsonld_helpers.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema/schema_validator.py` & `cert-schema-3.4.2/cert_schema/schema_validator.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/cert_schema.egg-info/PKG-INFO` & `cert-schema-3.4.2/cert_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cert-schema
-Version: 3.4.0
+Version: 3.4.2
 Summary: Blockchain certificates JSON-LD context and JSON schemas
 Home-page: https://github.com/blockchain-certificates/cert-schema
 Author: info@blockcerts.org
 Author-email: info@blockcerts.org
 License: MIT
 Description: [![Build Status](https://travis-ci.org/blockchain-certificates/cert-schema.svg?branch=master)](https://travis-ci.org/blockchain-certificates/cert-schema)
         [![PyPI version](https://badge.fury.io/py/cert-schema.svg)](https://badge.fury.io/py/cert-schema)
```

### Comparing `cert-schema-3.4.0/cert_schema.egg-info/SOURCES.txt` & `cert-schema-3.4.2/cert_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/setup.py` & `cert-schema-3.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/tests/test_context_urls.py` & `cert-schema-3.4.2/tests/test_context_urls.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/tests/test_jsonld_helpers.py` & `cert-schema-3.4.2/tests/test_jsonld_helpers.py`

 * *Files identical despite different names*

### Comparing `cert-schema-3.4.0/tests/test_schema_validator.py` & `cert-schema-3.4.2/tests/test_schema_validator.py`

 * *Files identical despite different names*

