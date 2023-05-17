# Comparing `tmp/keystoneauth1-5.1.2.tar.gz` & `tmp/keystoneauth1-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keystoneauth1-5.1.2.tar", last modified: Mon Feb 13 15:49:32 2023, max compression
+gzip compressed data, was "keystoneauth1-5.2.0.tar", last modified: Wed May 17 11:03:14 2023, max compression
```

## Comparing `keystoneauth1-5.1.2.tar` & `keystoneauth1-5.2.0.tar`

### file list

```diff
@@ -1,318 +1,323 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:32.015777 keystoneauth1-5.1.2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8348 2023-02-13 15:49:31.000000 keystoneauth1-5.1.2/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43559 2023-02-13 15:49:31.000000 keystoneauth1-5.1.2/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11891 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2470 2023-02-13 15:49:32.015777 keystoneauth1-5.1.2/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.963777 keystoneauth1-5.1.2/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3174 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/Makefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.963777 keystoneauth1-5.1.2/doc/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/ext/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/ext/list_plugins.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.963777 keystoneauth1-5.1.2/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20548 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/source/authentication-plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7567 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2450 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/source/extras.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.967777 keystoneauth1-5.1.2/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3014 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/source/images/graphs_authComp.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/source/images/graphs_authCompDelegate.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3769 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/source/migrating.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2816 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/source/plugin-options.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25823 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/doc/source/using-sessions.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.967777 keystoneauth1-5.1.2/keystoneauth1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3855 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/_fair_semaphore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2444 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.971777 keystoneauth1-5.1.2/keystoneauth1/access/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/access/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19872 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/access/access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24165 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/access/service_catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1590 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/access/service_providers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24392 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/adapter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    63274 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/discover.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.971777 keystoneauth1-5.1.2/keystoneauth1/exceptions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/exceptions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1329 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/exceptions/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2932 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/exceptions/auth_plugins.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/exceptions/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/exceptions/catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1568 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/exceptions/connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1909 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/exceptions/discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12371 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/exceptions/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1657 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/exceptions/oidc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/exceptions/response.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/exceptions/service_providers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.971777 keystoneauth1-5.1.2/keystoneauth1/extras/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/extras/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.971777 keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2570 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/_loading.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.975777 keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18693 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/v3/adfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/v3/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11111 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/v3/saml2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.975777 keystoneauth1-5.1.2/keystoneauth1/extras/kerberos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3306 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/extras/kerberos/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2839 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/extras/kerberos/_loading.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.975777 keystoneauth1-5.1.2/keystoneauth1/extras/oauth1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/extras/oauth1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/extras/oauth1/_loading.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2777 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/extras/oauth1/v3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.975777 keystoneauth1-5.1.2/keystoneauth1/fixture/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/fixture/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11625 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/fixture/discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/fixture/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2320 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/fixture/hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5560 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/fixture/keystoneauth_betamax.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6281 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/fixture/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3000 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/fixture/serializer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7705 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/fixture/v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17592 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/fixture/v3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.975777 keystoneauth1-5.1.2/keystoneauth1/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1229 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1585 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/http_basic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.979777 keystoneauth1-5.1.2/keystoneauth1/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2642 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1852 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32518 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.979777 keystoneauth1-5.1.2/keystoneauth1/identity/generic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/generic/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9153 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/generic/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3447 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/generic/password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1463 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/generic/token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6306 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.979777 keystoneauth1-5.1.2/keystoneauth1/identity/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1960 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4036 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/application_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12515 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4174 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6852 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/k2k.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2804 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/multi_factor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5133 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/oauth2_client_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19130 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/oidc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3111 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1231 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/receipt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4727 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/tokenless_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3239 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/identity/v3/totp.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.983777 keystoneauth1-5.1.2/keystoneauth1/loading/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2958 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.983777 keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/admin_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1628 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/http_basic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.983777 keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/identity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2728 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/identity/generic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/identity/v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13083 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/identity/v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1282 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/noauth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16394 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/adapter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6377 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3759 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4918 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6452 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/identity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5612 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11147 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/loading/session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/noauth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15084 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2959 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/service_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    63339 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/session.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.983777 keystoneauth1-5.1.2/keystoneauth1/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.987777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.991777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/access/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/access/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8066 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/access/test_v2_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11106 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/access/test_v2_service_catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12168 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/access/test_v3_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20956 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/access/test_v3_service_catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4854 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/client_fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.991777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/keystone_v2_sample_request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/keystone_v2_sample_response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/keystone_v3_sample_request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/keystone_v3_sample_response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2286 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/ksa_betamax_test_cassette.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/ksa_serializer_data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/test_pre_record_hook.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.991777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/exceptions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/exceptions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1275 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/exceptions/test_exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.991777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.995777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1808 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/test_fedkerb_loading.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/test_kerberos_loading.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4754 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/test_mapped.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/test_v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3078 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.995777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/oauth1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/oauth1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4625 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/oauth1/test_oauth1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2149 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/oauth1/test_oauth1_loading.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.995777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.959777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/examples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.995777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/examples/xml/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14138 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_RequestSecurityTokenResponse.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_fault.xml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.995777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/fixtures/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3549 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/fixtures/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.995777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      971 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/authn_request.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3698 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/saml_assertion.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1993 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/soap_response.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10762 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/test_auth_adfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12305 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/test_auth_saml2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1120 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.999777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2769 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    94611 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_identity_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14472 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_identity_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42381 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_identity_v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11263 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_identity_v3_federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16093 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_identity_v3_oidc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3974 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4615 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_tokenless_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6780 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5454 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/k2k_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2378 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/keystoneauth_fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.999777 keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11815 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_adapter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8123 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8381 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_entry_points.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3438 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3106 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_generic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4279 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_loading.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3702 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20553 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3223 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/matchers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3130 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/oidc_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4628 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_betamax_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6708 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_betamax_hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_betamax_serializer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51952 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2929 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_fair_sempahore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13686 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_hacking_checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1872 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_http_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3401 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_matchers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_noauth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4733 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_service_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    79385 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2633 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_token_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5540 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/tests/unit/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3230 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/keystoneauth1/token_endpoint.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.971777 keystoneauth1-5.1.2/keystoneauth1.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2470 2023-02-13 15:49:31.000000 keystoneauth1-5.1.2/keystoneauth1.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11816 2023-02-13 15:49:31.000000 keystoneauth1-5.1.2/keystoneauth1.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-13 15:49:31.000000 keystoneauth1-5.1.2/keystoneauth1.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2023-02-13 15:49:31.000000 keystoneauth1-5.1.2/keystoneauth1.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-13 15:49:31.000000 keystoneauth1-5.1.2/keystoneauth1.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-13 15:49:31.000000 keystoneauth1-5.1.2/keystoneauth1.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2023-02-13 15:49:31.000000 keystoneauth1-5.1.2/keystoneauth1.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-02-13 15:49:31.000000 keystoneauth1-5.1.2/keystoneauth1.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:31.959777 keystoneauth1-5.1.2/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:32.011777 keystoneauth1-5.1.2/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/1583780-700f99713e06324e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/add-oidc-client-credentials-2be065926ba4b849.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/add-oidc-discovery-document-support-b07fe54f83286d62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/add-prompt-to-opt-d083acc357a7f07b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/add-totp-auth-plugin-0650d220899c25b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/additional-headers-f2d16f85f5abe942.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/allow_version_hack-flag-9b53b72d9b084c04.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/api-sig-error-guideline-handler.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/basic-http-auth-45bea4298209df75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bp-application-credentials-416a1f8bb2311e04.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bp-oauth2-client-credentials-ext-06271700d4f33a7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bp-system-scope-29e9c597039ddb1e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bug-1582774-49af731b6dfc6f2f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bug-1614688-c4a1bd54f4ba5644.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bug-1616105-cc8b85eb056e99e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bug-1654847-acdf9543158329ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bug-1689424-set-adfspassword-endpointreference-f186d84a54007b09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bug-1733052-1b4af3b3fe1b05bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bug-1766235wq-0de60d0f996c6bfb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bug-1839748-5d8dfc99c43aaefc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bug-1840235-ef2946d149ac329c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/bug-1876317-1db97d1b12a3e4b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/cache-trailing-slash-3663c86cd9754379.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/cleanup-session-on-delete-1ed6177d4c5c1f83.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/client-side-rate-limiting-dec43fc9b54f5b70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/collect-timing-85f007f0d86c8b26.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/drop-py-2-7-f90c67a5db0dfeb8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/drop-python-3-6-and-3-7-c407d5898c5eafec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/drop-python-3.5-362bb9d47f830353.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/expose-endpoint-status-6195a6b76d8a8de8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/filter-versions-service-type-763af68092344b7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/fix-get-all-version-data-a01ee58524755b9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/get-auth-ref-7418e13bd0942060.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/global_request_id-per-request-bd66c7e0f1a71d9f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/improve-http-error-handling.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/ironic-discovery-fe41793ef97027bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/ironic-microversions-a69bf92ab21f0cf5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/ksa_2.2.0-81145229d4b43043.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/microversion-header-support-901acd820a21d788.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/noauth-discovery-c26d82a32c36d41d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/none-auth-dab13ab9af6f5c86.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/oslo-config-split-loggers-6bda266d657fe921.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/retries-limit-dbaedcb3207934ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/retries-options-99e4dbc240941557.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/retry-authenticated-discovery-19c4354ff983f507.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/retry-delay-68d0c0a1dffcf2fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/serice-type-aliases-249454829c57f39a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/status-code-retries-75052a43efa4edb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/support-api-wg-discovery-2cb4b0186619e124.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/user-agent-generation-b069100508c06177.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/notes/version-between-b4b0bcf4cecfb9e4.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:32.015777 keystoneauth1-5.1.2/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:32.015777 keystoneauth1-5.1.2/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:49:32.015777 keystoneauth1-5.1.2/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9107 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1127 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2725 2023-02-13 15:49:32.015777 keystoneauth1-5.1.2/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3169 2023-02-13 15:48:53.000000 keystoneauth1-5.1.2/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.175093 keystoneauth1-5.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8539 2023-05-17 11:03:13.000000 keystoneauth1-5.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43955 2023-05-17 11:03:13.000000 keystoneauth1-5.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11891 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2493 2023-05-17 11:03:14.175093 keystoneauth1-5.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.139093 keystoneauth1-5.2.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3174 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/Makefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.139093 keystoneauth1-5.2.0/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/ext/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/ext/list_plugins.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.143093 keystoneauth1-5.2.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20657 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/authentication-plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7567 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2450 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/extras.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.143093 keystoneauth1-5.2.0/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3014 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/images/graphs_authComp.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/images/graphs_authCompDelegate.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3769 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/migrating.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2816 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/plugin-options.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25823 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/doc/source/using-sessions.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.143093 keystoneauth1-5.2.0/keystoneauth1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3838 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/_fair_semaphore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2413 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/access/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/access/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20111 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/access/access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24136 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/access/service_catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1590 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/access/service_providers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24392 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/adapter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    63222 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/discover.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/exceptions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1329 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2932 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/auth_plugins.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1568 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1909 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12371 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/oidc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/response.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/exceptions/service_providers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/extras/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2570 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/_loading.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18677 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/adfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11111 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/saml2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/extras/kerberos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3306 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/kerberos/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2839 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/kerberos/_loading.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.147093 keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/_loading.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2777 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/v3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.151093 keystoneauth1-5.2.0/keystoneauth1/fixture/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11625 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2320 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5560 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/keystoneauth_betamax.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6281 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2969 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/serializer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7705 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18080 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/fixture/v3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.151093 keystoneauth1-5.2.0/keystoneauth1/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1229 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1585 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/http_basic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.151093 keystoneauth1-5.2.0/keystoneauth1/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2991 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1852 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32471 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.151093 keystoneauth1-5.2.0/keystoneauth1/identity/generic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/generic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9114 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/generic/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3447 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/generic/password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1463 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/generic/token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6285 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.151093 keystoneauth1-5.2.0/keystoneauth1/identity/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2092 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4036 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/application_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12468 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4235 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6830 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/k2k.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2804 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/multi_factor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5133 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/oauth2_client_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5082 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/oauth2_mtls_client_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24908 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/oidc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3111 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1231 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/receipt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4706 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/tokenless_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3239 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/identity/v3/totp.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.155093 keystoneauth1-5.2.0/keystoneauth1/loading/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2958 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.155093 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/admin_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1628 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/http_basic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.155093 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2728 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/generic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15077 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1282 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/noauth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16394 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/adapter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6349 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3759 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4918 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6452 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/identity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5612 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11147 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/loading/session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/noauth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15084 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2959 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/service_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62863 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/session.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.155093 keystoneauth1-5.2.0/keystoneauth1/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8066 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v2_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11106 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v2_service_catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12168 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v3_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20956 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v3_service_catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4854 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/client_fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/keystone_v2_sample_request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/keystone_v2_sample_response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/keystone_v3_sample_request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/keystone_v3_sample_response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2286 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/ksa_betamax_test_cassette.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/ksa_serializer_data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/test_pre_record_hook.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/exceptions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/exceptions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1275 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/exceptions/test_exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1808 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_fedkerb_loading.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_kerberos_loading.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4754 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_mapped.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3078 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/oauth1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/oauth1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4601 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/oauth1/test_oauth1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2149 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/oauth1/test_oauth1_loading.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.159093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.135093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/examples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.163093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/examples/xml/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14138 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_RequestSecurityTokenResponse.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_fault.xml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.163093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3549 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.163093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      971 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/authn_request.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3698 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/saml_assertion.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1993 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/soap_response.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10747 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/test_auth_adfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12305 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/test_auth_saml2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1120 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.163093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2769 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    94579 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14472 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51660 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11461 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v3_federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16077 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v3_oidc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3974 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4615 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_tokenless_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6780 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5454 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/k2k_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2378 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/keystoneauth_fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.163093 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11815 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_adapter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8123 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8381 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_entry_points.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3438 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3106 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_generic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4279 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_loading.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3702 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24004 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3223 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/matchers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3279 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/oidc_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4628 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_betamax_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6708 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_betamax_hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_betamax_serializer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51952 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2914 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_fair_sempahore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14190 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_hacking_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1872 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_http_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3401 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_matchers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_noauth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4733 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_service_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    79474 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2633 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_token_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5556 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/tests/unit/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3230 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/keystoneauth1/token_endpoint.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.143093 keystoneauth1-5.2.0/keystoneauth1.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2493 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12051 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-05-17 11:03:14.000000 keystoneauth1-5.2.0/keystoneauth1.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.139093 keystoneauth1-5.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.171093 keystoneauth1-5.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/1583780-700f99713e06324e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/add-oidc-client-credentials-2be065926ba4b849.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/add-oidc-discovery-document-support-b07fe54f83286d62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/add-prompt-to-opt-d083acc357a7f07b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/add-totp-auth-plugin-0650d220899c25b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/additional-headers-f2d16f85f5abe942.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/allow_version_hack-flag-9b53b72d9b084c04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/api-sig-error-guideline-handler.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/basic-http-auth-45bea4298209df75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bp-application-credentials-416a1f8bb2311e04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bp-oauth2-client-credentials-ext-06271700d4f33a7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bp-support-oauth2-mtls-177cda05265ae65c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bp-system-scope-29e9c597039ddb1e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1582774-49af731b6dfc6f2f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1614688-c4a1bd54f4ba5644.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1616105-cc8b85eb056e99e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1654847-acdf9543158329ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1689424-set-adfspassword-endpointreference-f186d84a54007b09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1733052-1b4af3b3fe1b05bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1766235wq-0de60d0f996c6bfb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1839748-5d8dfc99c43aaefc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1840235-ef2946d149ac329c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1876317-1db97d1b12a3e4b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/bug-1998366-27cd486b46fb56b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/cache-trailing-slash-3663c86cd9754379.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/cleanup-session-on-delete-1ed6177d4c5c1f83.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/client-side-rate-limiting-dec43fc9b54f5b70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/collect-timing-85f007f0d86c8b26.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/drop-py-2-7-f90c67a5db0dfeb8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/drop-python-3-6-and-3-7-c407d5898c5eafec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/drop-python-3.5-362bb9d47f830353.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/expose-endpoint-status-6195a6b76d8a8de8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/filter-versions-service-type-763af68092344b7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/fix-get-all-version-data-a01ee58524755b9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/get-auth-ref-7418e13bd0942060.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/global_request_id-per-request-bd66c7e0f1a71d9f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/improve-http-error-handling.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/ironic-discovery-fe41793ef97027bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/ironic-microversions-a69bf92ab21f0cf5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/ksa_2.2.0-81145229d4b43043.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/microversion-header-support-901acd820a21d788.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/noauth-discovery-c26d82a32c36d41d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/none-auth-dab13ab9af6f5c86.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/oslo-config-split-loggers-6bda266d657fe921.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/retries-limit-dbaedcb3207934ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/retries-options-99e4dbc240941557.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/retry-authenticated-discovery-19c4354ff983f507.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/retry-delay-68d0c0a1dffcf2fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/serice-type-aliases-249454829c57f39a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/status-code-retries-75052a43efa4edb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/support-api-wg-discovery-2cb4b0186619e124.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/user-agent-generation-b069100508c06177.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/notes/version-between-b4b0bcf4cecfb9e4.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.175093 keystoneauth1-5.2.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.175093 keystoneauth1-5.2.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:03:14.175093 keystoneauth1-5.2.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9107 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2023-05-17 11:03:14.175093 keystoneauth1-5.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3169 2023-05-17 11:02:35.000000 keystoneauth1-5.2.0/tox.ini
```

### Comparing `keystoneauth1-5.1.2/AUTHORS` & `keystoneauth1-5.2.0/AUTHORS`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 Alexander Makarov <amakarov@mirantis.com>
 Alexey Stepanov <astepanov@mirantis.com>
 Alvaro Lopez Garcia <aloga@ifca.unican.es>
 Andreas Jaeger <aj@suse.com>
 Andrey Kurilin <akurilin@mirantis.com>
 Antoni Segura Puimedon <antonisp@celebdor.com>
 Antoni Segura Puimedon <toni@midokura.com>
+Arvid Requate <requate@univention.de>
 Ben Nemec <bnemec@redhat.com>
 Bernhard M. Wiedemann <bwiedemann@suse.de>
 Bhuvan Arumugam <bhuvan@apache.org>
 Blake Covarrubias <blake@platform9.com>
 Boris Bobrov <b.bobrov@corp.mail.ru>
 Boris Bobrov <bbobrov@mirantis.com>
 Boris Pavlovic <boris@pavlovic.me>
@@ -125,14 +126,15 @@
 Monty Taylor <mordred@inaugust.com>
 Morgan Fainberg <morgan.fainberg@gmail.com>
 Navid Pustchi <npustchi@gmail.com>
 Ngo Quoc Cuong <cuongnq@vn.fujitsu.com>
 Ondřej Nový <ondrej.novy@firma.seznam.cz>
 OpenStack Release Bot <infra-root@openstack.org>
 Pavlo Shchelokovskyy <shchelokovskyy@gmail.com>
+Pete Zaitcev <zaitcev@kotori.zaitcev.us>
 Pradeep Kilambi <pkilambi@cisco.com>
 Prosunjit Biswas <prosun.csedu@gmail.com>
 Q.hongtao <qihongtao@inspur.com>
 Rabi Mishra <ramishra@redhat.com>
 Raildo Mascena <raildo@lsd.ufcg.edu.br>
 Rodrigo Duarte <rduartes@redhat.com>
 Rodrigo Duarte Sousa <rduartes@redhat.com>
@@ -147,14 +149,15 @@
 Sascha Peilicke <saschpe@suse.de>
 Sean Dague <sean@dague.net>
 Sean McGinnis <sean.mcginnis@gmail.com>
 Sean Perry <sean.perry@hpe.com>
 Sergey Kraynev <skraynev@mirantis.com>
 Sergio Cazzolato <sergio.j.cazzolato@intel.com>
 Simon Li <libo04@inspur.com>
+Stephen Finucane <stephenfin@redhat.com>
 Steve Baker <sbaker@redhat.com>
 Steve Martinelli <s.martinelli@gmail.com>
 Steve Martinelli <stevemar@ca.ibm.com>
 Steven Hardy <shardy@redhat.com>
 Stuart McLaren <stuart.mclaren@hp.com>
 Sushil Kumar <sushil.kumar2@globallogic.com>
 Takashi Kajinami <tkajinam@redhat.com>
@@ -202,22 +205,24 @@
 jakedahn <jake@ansolabs.com>
 ji-xuepeng <ji.xuepeng@zte.com.cn>
 lilintan <lintan.li@easystack.cn>
 lin-hua-cheng <lin-hua.cheng@hp.com>
 lin-hua-cheng <os.lcheng@gmail.com>
 liuqing <jing.liuqing@99cloud.net>
 liushuobj <liushuobj@inspur.com>
+ljhuang <huang.liujie@99cloud.net>
 llg8212 <lilinguo@huawei.com>
 maaoyu <maaoyu@inspur.com>
 melanie witt <melwittt@gmail.com>
 melissaml <ma.lei@99cloud.net>
 ricolin <rico.lin.guanyu@gmail.com>
 ricolin <rico.lin@easystack.cn>
 shanyunfan33 <shanyunfan@inspur.com>
 sridhargaddam <sridhar.gaddam@enovance.com>
+sunyonggen <sunyonggen@fujitsu.com>
 wanghong <w.wanghong@huawei.com>
 wangqiangbj <wangqiangbj@inspur.com>
 wangxiyuan <wangxiyuan1007@gmail.com>
 wangxiyuan <wangxiyuan@huawei.com>
 wangzhenyu <wangzy@fiberhome.com>
 zhangboye <zhangboye@inspur.com>
 zhangguoqing <zhang.guoqing@99cloud.net>
```

### Comparing `keystoneauth1-5.1.2/CONTRIBUTING.rst` & `keystoneauth1-5.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/ChangeLog` & `keystoneauth1-5.2.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 CHANGES
 =======
 
+5.2.0
+-----
+
+* Update master for stable/2023.1
+* New auth plugin v3oidcdeviceauthz
+* OAuth 2.0 Mutual-TLS Support
+
 5.1.2
 -----
 
 * Fix docs build for tox4
 
 5.1.1
 -----
 
 * Allow passing of version header
+* Remove six
+* setup.cfg: Restore python\_requires after a typo
+* Allow federation to work with unversioned auth\_url
 * Enforce scope mutual exclusion for system
 * Fix linters and bindep on jammy
+* Switch to 2023.1 Python3 unit tests and generic template name
+* Update master for stable/zed
 
 5.1.0
 -----
 
 * OAuth2.0 Client Credentials Grant Flow Support
+* Replace abc.abstractproperty with property and abc.abstractmethod
 
 5.0.0
 -----
 
 * Update python testing as per zed cycle teting runtime
 
 4.6.0
```

### Comparing `keystoneauth1-5.1.2/HACKING.rst` & `keystoneauth1-5.2.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/LICENSE` & `keystoneauth1-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/PKG-INFO` & `keystoneauth1-5.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystoneauth1
-Version: 5.1.2
+Version: 5.2.0
 Summary: Authentication Library for OpenStack Identity
 Home-page: https://docs.openstack.org/keystoneauth/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -52,12 +52,13 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
 Provides-Extra: betamax
 Provides-Extra: kerberos
 Provides-Extra: oauth1
 Provides-Extra: saml2
 Provides-Extra: test
```

### Comparing `keystoneauth1-5.1.2/README.rst` & `keystoneauth1-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/doc/Makefile` & `keystoneauth1-5.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/doc/ext/list_plugins.py` & `keystoneauth1-5.2.0/doc/ext/list_plugins.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/doc/requirements.txt` & `keystoneauth1-5.2.0/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/doc/source/authentication-plugins.rst` & `keystoneauth1-5.2.0/doc/source/authentication-plugins.rst`

 * *Files 1% similar despite different names*

```diff
@@ -422,14 +422,15 @@
 - v3password: :py:class:`keystoneauth1.identity.v3.Password`
 - v3token: :py:class:`keystoneauth1.identity.v3.Token`
 - v3fedkerb: :py:class:`keystoneauth1.extras.kerberos.MappedKerberos`
 - v3kerberos: :py:class:`keystoneauth1.extras.kerberos.Kerberos`
 - v3oauth1: :py:class:`keystoneauth1.extras.oauth1.v3.OAuth1`
 - v3oidcaccesstoken: :py:class:`keystoneauth1.identity.v3:OpenIDConnectAccessToken`
 - v3oidcauthcode: :py:class:`keystoneauth1.identity.v3:OpenIDConnectAuthorizationCode`
+- v3oidcdeviceauthz: :py:class:`keystoneauth1.loading._plugins.identity.v3:OpenIDConnectDeviceAuthorization`
 - v3oidcclientcredentials: :py:class:`keystoneauth1.identity.v3:OpenIDConnectClientCredentials`
 - v3oidcpassword: :py:class:`keystoneauth1.identity.v3:OpenIDConnectPassword`
 - v3samlpassword: :py:class:`keystoneauth1.extras._saml2.v3.Password`
 - v3tokenlessauth: :py:class:`keystoneauth1.identity.v3.TokenlessAuth`
 - v3totp: :py:class:`keystoneauth1.identity.v3.TOTP`
```

### Comparing `keystoneauth1-5.1.2/doc/source/conf.py` & `keystoneauth1-5.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/doc/source/extras.rst` & `keystoneauth1-5.2.0/doc/source/extras.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/doc/source/images/graphs_authComp.svg` & `keystoneauth1-5.2.0/doc/source/images/graphs_authComp.svg`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/doc/source/images/graphs_authCompDelegate.svg` & `keystoneauth1-5.2.0/doc/source/images/graphs_authCompDelegate.svg`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/doc/source/index.rst` & `keystoneauth1-5.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/doc/source/migrating.rst` & `keystoneauth1-5.2.0/doc/source/migrating.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/doc/source/plugin-options.rst` & `keystoneauth1-5.2.0/doc/source/plugin-options.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/doc/source/using-sessions.rst` & `keystoneauth1-5.2.0/doc/source/using-sessions.rst`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/_fair_semaphore.py` & `keystoneauth1-5.2.0/keystoneauth1/_fair_semaphore.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+import queue
 import threading
 import time
 
 
-from six.moves import queue
-
-
 class FairSemaphore(object):
     """Semaphore class that notifies in order of request.
 
     We cannot use a normal Semaphore because it doesn't give any ordering,
     which could lead to a request starving. Instead, handle them in the
     order we receive them.
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/_utils.py` & `keystoneauth1-5.2.0/keystoneauth1/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import datetime
 import logging
 
 import iso8601
-import six
 
 
 def get_logger(name):
     name = name.replace(__name__.split('.')[0], 'keystoneauth')
     return logging.getLogger(name)
 
 
@@ -34,17 +33,17 @@
 
 
 def parse_isotime(timestr):
     """Parse time from ISO 8601 format."""
     try:
         return iso8601.parse_date(timestr)
     except iso8601.ParseError as e:
-        raise ValueError(six.text_type(e))
+        raise ValueError(str(e))
     except TypeError as e:
-        raise ValueError(six.text_type(e))
+        raise ValueError(str(e))
 
 
 def from_utcnow(**timedelta_kwargs):
     r"""Calculate the time in the future from utcnow.
 
     :param \*\*timedelta_kwargs:
         Passed directly to :class:`datetime.timedelta` to add to the current
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/access/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/access/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/access/access.py` & `keystoneauth1-5.2.0/keystoneauth1/access/access.py`

 * *Files 1% similar despite different names*

```diff
@@ -778,7 +778,15 @@
                 service_providers.ServiceProviders.from_token(self._data))
 
         return self._service_providers
 
     @_missingproperty
     def bind(self):
         return self._data['token']['bind']
+
+    @property
+    def oauth2_credential(self):
+        return self._data['token']['oauth2_credential']
+
+    @_missingproperty
+    def oauth2_credential_thumbprint(self):
+        return self._data['token']['oauth2_credential']['x5t#S256']
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/access/service_catalog.py` & `keystoneauth1-5.2.0/keystoneauth1/access/service_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,22 +15,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
 import copy
 
-import six
-
 from keystoneauth1 import discover
 from keystoneauth1 import exceptions
 
 
-@six.add_metaclass(abc.ABCMeta)
-class ServiceCatalog(object):
+class ServiceCatalog(metaclass=abc.ABCMeta):
     """Helper methods for dealing with a Keystone Service Catalog."""
 
     def __init__(self, catalog):
         self._catalog = catalog
 
     def _get_endpoint_region(self, endpoint):
         return endpoint.get('region_id') or endpoint.get('region')
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/access/service_providers.py` & `keystoneauth1-5.2.0/keystoneauth1/access/service_providers.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/adapter.py` & `keystoneauth1-5.2.0/keystoneauth1/adapter.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/discover.py` & `keystoneauth1-5.2.0/keystoneauth1/discover.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,17 @@
 The Discover object in this file provides the querying components of Discovery.
 This includes functions like url_for which allow you to retrieve URLs and the
 raw data specified in version discovery responses.
 """
 
 import copy
 import re
+import urllib
 
 import os_service_types
-import six
-from six.moves import urllib
 
 from keystoneauth1 import _utils as utils
 from keystoneauth1 import exceptions
 
 
 _LOGGER = utils.get_logger(__name__)
 
@@ -204,26 +203,26 @@
     :raises TypeError: If the input version cannot be interpreted.
     """  # noqa: D412
     # Copy the input var so the error presents the original value
     ver = version
 
     # If it's a non-string iterable, turn it into a string for subsequent
     # processing.  This ensures at least 1 decimal point if e.g. [1] is given.
-    if not isinstance(ver, six.string_types):
+    if not isinstance(ver, str):
         try:
             ver = '.'.join(map(_str_or_latest, ver))
         except TypeError:
             # Not an iterable
             pass
 
     # If it's a numeric or an integer as a string then normalize it to a
     # float string. This ensures 1 decimal point.
     # If it's a float as a string, don't do that, the split/map below will do
     # what we want. (Otherwise, we wind up with 3.20 -> (3, 2))
-    if isinstance(ver, six.string_types):
+    if isinstance(ver, str):
         # trim the v from a 'v2.0' or similar
         ver = ver.lstrip('v')
         try:
             # If version is a pure int, like '1' or '200' this will produce
             # a stringified version with a .0 added. If it's any other number,
             # such as '1.1' - int(version) raises an Exception
             ver = str(float(int(ver)))
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/exceptions/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/exceptions/auth.py` & `keystoneauth1-5.2.0/keystoneauth1/exceptions/auth.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/exceptions/auth_plugins.py` & `keystoneauth1-5.2.0/keystoneauth1/exceptions/auth_plugins.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/exceptions/base.py` & `keystoneauth1-5.2.0/keystoneauth1/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/exceptions/catalog.py` & `keystoneauth1-5.2.0/keystoneauth1/exceptions/catalog.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/exceptions/connection.py` & `keystoneauth1-5.2.0/keystoneauth1/exceptions/connection.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/exceptions/discovery.py` & `keystoneauth1-5.2.0/keystoneauth1/exceptions/discovery.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/exceptions/http.py` & `keystoneauth1-5.2.0/keystoneauth1/exceptions/http.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/exceptions/oidc.py` & `keystoneauth1-5.2.0/keystoneauth1/exceptions/oidc.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,13 +32,22 @@
     message = "OpenID Connect access token endpoint not provided."
 
 
 class OidcAuthorizationEndpointNotFound(auth_plugins.AuthPluginException):
     message = "OpenID Connect authorization endpoint not provided."
 
 
+class OidcDeviceAuthorizationEndpointNotFound(
+        auth_plugins.AuthPluginException):
+    message = "OpenID Connect device authorization endpoint not provided."
+
+
+class OidcDeviceAuthorizationTimeOut(auth_plugins.AuthPluginException):
+    message = "Timeout for OpenID Connect device authorization."
+
+
 class OidcGrantTypeMissmatch(auth_plugins.AuthPluginException):
     message = "Missmatch between OpenID Connect plugin and grant_type argument"
 
 
 class OidcPluginNotSupported(auth_plugins.AuthPluginException):
     message = "OpenID Connect grant type not supported by provider."
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/exceptions/response.py` & `keystoneauth1-5.2.0/keystoneauth1/exceptions/response.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/exceptions/service_providers.py` & `keystoneauth1-5.2.0/keystoneauth1/exceptions/service_providers.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/extras/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/_loading.py` & `keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/v3/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/v3/adfs.py` & `keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/adfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import datetime
+import urllib
 import uuid
 
 try:
     from lxml import etree
 except ImportError:
     etree = None
 
-from six.moves import urllib
-
 from keystoneauth1 import access
 from keystoneauth1 import exceptions
 from keystoneauth1.extras._saml2.v3 import base
 
 
 class Password(base.BaseSAMLPlugin):
     """Authentication plugin for Microsoft ADFS2.0 IdPs."""
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/v3/base.py` & `keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/base.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/extras/_saml2/v3/saml2.py` & `keystoneauth1-5.2.0/keystoneauth1/extras/_saml2/v3/saml2.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/extras/kerberos/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/extras/kerberos/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/extras/kerberos/_loading.py` & `keystoneauth1-5.2.0/keystoneauth1/extras/kerberos/_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/extras/oauth1/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/extras/oauth1/_loading.py` & `keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/extras/oauth1/v3.py` & `keystoneauth1-5.2.0/keystoneauth1/extras/oauth1/v3.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/fixture/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/fixture/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/fixture/discovery.py` & `keystoneauth1-5.2.0/keystoneauth1/fixture/discovery.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/fixture/exception.py` & `keystoneauth1-5.2.0/keystoneauth1/fixture/exception.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/fixture/hooks.py` & `keystoneauth1-5.2.0/keystoneauth1/fixture/hooks.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/fixture/keystoneauth_betamax.py` & `keystoneauth1-5.2.0/keystoneauth1/fixture/keystoneauth_betamax.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/fixture/plugin.py` & `keystoneauth1-5.2.0/keystoneauth1/fixture/plugin.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/fixture/serializer.py` & `keystoneauth1-5.2.0/keystoneauth1/fixture/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 """A serializer to emit YAML but with request body in nicely formatted JSON."""
 
 import json
 import os
 
 import betamax.serializers.base
-import six
 import yaml
 
 
 def _should_use_block(value):
     for c in u"\u000a\u000d\u001c\u001d\u001e\u0085\u2028\u2029":
         if c in value:
             return True
@@ -48,15 +47,15 @@
 def _indent_json(val):
     if not val:
         return ''
 
     return json.dumps(
         json.loads(val), indent=2,
         separators=(',', ': '), sort_keys=False,
-        default=six.text_type)
+        default=str)
 
 
 def _is_json_body(interaction):
     content_type = interaction['headers'].get('Content-Type', [])
     return 'application/json' in content_type
 
 
@@ -78,15 +77,15 @@
                         interaction[key]['body']['string'])
 
         class MyDumper(yaml.Dumper):
             """Specialized Dumper which does nice blocks and unicode."""
 
         yaml.representer.BaseRepresenter.represent_scalar = _represent_scalar
 
-        MyDumper.add_representer(six.text_type, _unicode_representer)
+        MyDumper.add_representer(str, _unicode_representer)
 
         return yaml.dump(
             cassette_data, Dumper=MyDumper, default_flow_style=False)
 
     def deserialize(self, cassette_data):
         try:
             deserialized = yaml.safe_load(cassette_data)
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/fixture/v2.py` & `keystoneauth1-5.2.0/keystoneauth1/fixture/v2.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/fixture/v3.py` & `keystoneauth1-5.2.0/keystoneauth1/fixture/v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,16 @@
                  project_id=None, project_name=None, project_domain_id=None,
                  project_domain_name=None, domain_id=None, domain_name=None,
                  trust_id=None, trust_impersonation=None, trustee_user_id=None,
                  trustor_user_id=None, application_credential_id=None,
                  application_credential_access_rules=None,
                  oauth_access_token_id=None, oauth_consumer_id=None,
                  audit_id=None, audit_chain_id=None,
-                 is_admin_project=None, project_is_domain=None):
+                 is_admin_project=None, project_is_domain=None,
+                 oauth2_thumbprint=None):
         super(Token, self).__init__()
 
         self.user_id = user_id or uuid.uuid4().hex
         self.user_name = user_name or uuid.uuid4().hex
         self.user_domain_id = user_domain_id or uuid.uuid4().hex
         self.user_domain_name = user_domain_name or uuid.uuid4().hex
         self.audit_id = audit_id or uuid.uuid4().hex
@@ -125,14 +126,17 @@
 
         if audit_chain_id:
             self.audit_chain_id = audit_chain_id
 
         if is_admin_project is not None:
             self.is_admin_project = is_admin_project
 
+        if oauth2_thumbprint:
+            self.oauth2_thumbprint = oauth2_thumbprint
+
     @property
     def root(self):
         return self.setdefault('token', {})
 
     @property
     def expires_str(self):
         return self.root.get('expires_at')
@@ -391,14 +395,26 @@
     def is_admin_project(self, value):
         self.root['is_admin_project'] = value
 
     @is_admin_project.deleter
     def is_admin_project(self):
         self.root.pop('is_admin_project', None)
 
+    @property
+    def oauth2_thumbprint(self):
+        return self.root.get('oauth2_credential', {}).get('x5t#S256')
+
+    @oauth2_thumbprint.setter
+    def oauth2_thumbprint(self, value):
+        self.root.setdefault('oauth2_credential', {})['x5t#S256'] = value
+
+    @property
+    def oauth2_credential(self):
+        return self.root.get('oauth2_credential')
+
     def validate(self):
         project = self.root.get('project')
         domain = self.root.get('domain')
         system = self.root.get('system')
         trust = self.root.get('OS-TRUST:trust')
         catalog = self.root.get('catalog')
         roles = self.root.get('roles')
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/hacking/checks.py` & `keystoneauth1-5.2.0/keystoneauth1/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/http_basic.py` & `keystoneauth1-5.2.0/keystoneauth1/http_basic.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 
 V3OidcAuthorizationCode = oidc.OidcAuthorizationCode
 """See :class:`keystoneauth1.identity.v3.oidc.OidcAuthorizationCode`"""
 
 V3OidcAccessToken = oidc.OidcAccessToken
 """See :class:`keystoneauth1.identity.v3.oidc.OidcAccessToken`"""
 
+V3OidcDeviceAuthorization = oidc.OidcDeviceAuthorization
+"""See :class:`keystoneauth1.identity.v3.oidc.OidcDeviceAuthorization`"""
+
 V3TOTP = v3.TOTP
 """See :class:`keystoneauth1.identity.v3.TOTP`"""
 
 V3TokenlessAuth = v3.TokenlessAuth
 """See :class:`keystoneauth1.identity.v3.TokenlessAuth`"""
 
 V3ApplicationCredential = v3.ApplicationCredential
@@ -60,22 +63,27 @@
 
 V3MultiFactor = v3.MultiFactor
 """See :class:`keystoneauth1.identity.v3.MultiFactor`"""
 
 V3OAuth2ClientCredential = v3.OAuth2ClientCredential
 """See :class:`keystoneauth1.identity.v3.OAuth2ClientCredential`"""
 
+V3OAuth2mTlsClientCredential = v3.OAuth2mTlsClientCredential
+"""See :class:`keystoneauth1.identity.v3.OAuth2mTlsClientCredential`"""
+
 __all__ = ('BaseIdentityPlugin',
            'Password',
            'Token',
            'V2Password',
            'V2Token',
            'V3Password',
            'V3Token',
            'V3OidcPassword',
            'V3OidcAuthorizationCode',
            'V3OidcAccessToken',
+           'V3OidcDeviceAuthorization',
            'V3TOTP',
            'V3TokenlessAuth',
            'V3ApplicationCredential',
            'V3MultiFactor',
-           'V3OAuth2ClientCredential')
+           'V3OAuth2ClientCredential',
+           'V3OAuth2mTlsClientCredential')
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/access.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/access.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/base.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,27 +13,24 @@
 import abc
 import base64
 import functools
 import hashlib
 import json
 import threading
 
-import six
-
 from keystoneauth1 import _utils as utils
 from keystoneauth1 import access
 from keystoneauth1 import discover
 from keystoneauth1 import exceptions
 from keystoneauth1 import plugin
 
 LOG = utils.get_logger(__name__)
 
 
-@six.add_metaclass(abc.ABCMeta)
-class BaseIdentityPlugin(plugin.BaseAuthPlugin):
+class BaseIdentityPlugin(plugin.BaseAuthPlugin, metaclass=abc.ABCMeta):
 
     # we count a token as valid (not needing refreshing) if it is valid for at
     # least this many seconds before the token expiry time
     MIN_TOKEN_LIFE_SECONDS = 120
 
     def __init__(self, auth_url=None, reauthenticate=True):
 
@@ -643,17 +640,17 @@
             return None
 
         hasher = hashlib.sha256()
 
         for k, v in sorted(elements.items()):
             if v is not None:
                 # NOTE(jamielennox): in python3 you need to pass bytes to hash
-                if isinstance(k, six.string_types):
+                if isinstance(k, str):
                     k = k.encode('utf-8')
-                if isinstance(v, six.string_types):
+                if isinstance(v, str):
                     v = v.encode('utf-8')
 
                 hasher.update(k)
                 hasher.update(v)
 
         return base64.b64encode(hasher.digest()).decode('utf-8')
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/generic/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/generic/base.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/generic/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,29 +7,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import abc
-
-import six
-import six.moves.urllib.parse as urlparse
+import urllib.parse
 
 from keystoneauth1 import _utils as utils
 from keystoneauth1 import discover
 from keystoneauth1 import exceptions
 from keystoneauth1.identity import base
 
 
 LOG = utils.get_logger(__name__)
 
 
-@six.add_metaclass(abc.ABCMeta)
-class BaseGenericPlugin(base.BaseIdentityPlugin):
+class BaseGenericPlugin(base.BaseIdentityPlugin, metaclass=abc.ABCMeta):
     """An identity plugin that is not version dependent.
 
     Internally we will construct a version dependent plugin with the resolved
     URL and then proxy all calls from the base plugin to the versioned one.
     """
 
     def __init__(self, auth_url,
@@ -140,15 +137,15 @@
                 exceptions.HttpError,
                 exceptions.SSLError,
                 exceptions.ConnectionError) as e:
             LOG.warning('Failed to discover available identity versions when '
                         'contacting %s. Attempting to parse version from URL.',
                         self.auth_url)
 
-            url_parts = urlparse.urlparse(self.auth_url)
+            url_parts = urllib.parse.urlparse(self.auth_url)
             path = url_parts.path.lower()
 
             if path.startswith('/v2.0'):
                 if self._has_domain_scope:
                     raise exceptions.DiscoveryFailure(
                         'Cannot use v2 authentication with domain scope')
                 plugin = self.create_plugin(session, (2, 0), self.auth_url)
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/generic/password.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/generic/password.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/generic/token.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/generic/token.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v2.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import abc
 
-import six
-
 from keystoneauth1 import _utils as utils
 from keystoneauth1 import access
 from keystoneauth1 import exceptions
 from keystoneauth1.identity import base
 
 _logger = utils.get_logger(__name__)
 
 
-@six.add_metaclass(abc.ABCMeta)
-class Auth(base.BaseIdentityPlugin):
+class Auth(base.BaseIdentityPlugin, metaclass=abc.ABCMeta):
     """Identity V2 Authentication Plugin.
 
     :param string auth_url: Identity service endpoint for authorization.
     :param string trust_id: Trust ID for trust scoping.
     :param string tenant_id: Tenant ID for project scoping.
     :param string tenant_name: Tenant name for project scoping.
     :param bool reauthenticate: Allow fetching a new token if the current one
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from keystoneauth1.identity.v3.oidc import *  # noqa
 from keystoneauth1.identity.v3.password import *  # noqa
 from keystoneauth1.identity.v3.receipt import *  # noqa
 from keystoneauth1.identity.v3.token import *  # noqa
 from keystoneauth1.identity.v3.totp import *  # noqa
 from keystoneauth1.identity.v3.tokenless_auth import *  # noqa
 from keystoneauth1.identity.v3.oauth2_client_credential import *  # noqa
+from keystoneauth1.identity.v3.oauth2_mtls_client_credential import *  # noqa
 
 
 __all__ = ('ApplicationCredential',
            'ApplicationCredentialMethod',
 
            'Auth',
            'AuthConstructor',
@@ -55,8 +56,11 @@
            'TokenlessAuth',
 
            'ReceiptMethod',
 
            'MultiFactor',
 
            'OAuth2ClientCredential',
-           'OAuth2ClientCredentialMethod',)
+           'OAuth2ClientCredentialMethod',
+
+           'OAuth2mTlsClientCredential',
+           )
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/application_credential.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/application_credential.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/base.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,25 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import abc
 import json
 
-import six
-
 from keystoneauth1 import _utils as utils
 from keystoneauth1 import access
 from keystoneauth1 import exceptions
 from keystoneauth1.identity import base
 
 _logger = utils.get_logger(__name__)
 
 __all__ = ('Auth', 'AuthMethod', 'AuthConstructor', 'BaseAuth')
 
 
-@six.add_metaclass(abc.ABCMeta)
-class BaseAuth(base.BaseIdentityPlugin):
+class BaseAuth(base.BaseIdentityPlugin, metaclass=abc.ABCMeta):
     """Identity V3 Authentication Plugin.
 
     :param string auth_url: Identity service endpoint for authentication.
     :param string trust_id: Trust ID for trust scoping.
     :param string system_scope: System information to scope to.
     :param string domain_id: Domain ID for domain scoping.
     :param string domain_name: Domain name for domain scoping.
@@ -220,16 +217,15 @@
                 return None
 
             params.update(elements)
 
         return params
 
 
-@six.add_metaclass(abc.ABCMeta)
-class AuthMethod(object):
+class AuthMethod(metaclass=abc.ABCMeta):
     """One part of a V3 Authentication strategy.
 
     V3 Tokens allow multiple methods to be presented when authentication
     against the server. Each one of these methods is implemented by an
     AuthMethod.
 
     Note: When implementing an AuthMethod use the method_parameters
@@ -280,16 +276,15 @@
         To avoid collision or overrides the keys of the returned dictionary
         should be prefixed with the plugin identifier. For example the password
         plugin returns its username value as 'password_username'.
         """
         raise NotImplementedError()
 
 
-@six.add_metaclass(abc.ABCMeta)
-class AuthConstructor(Auth):
+class AuthConstructor(Auth, metaclass=abc.ABCMeta):
     """Abstract base class for creating an Auth Plugin.
 
     The Auth Plugin created contains only one authentication method. This
     is generally the required usage.
 
     An AuthConstructor creates an AuthMethod based on the method's
     arguments and the auth_method_class defined by the plugin. It then
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/federation.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/federation.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import abc
 
-import six
-
 from keystoneauth1.identity.v3 import base
 from keystoneauth1.identity.v3 import token
 
 __all__ = ('FederationBaseAuth',)
 
 
-@six.add_metaclass(abc.ABCMeta)
-class _Rescoped(base.BaseAuth):
+class _Rescoped(base.BaseAuth, metaclass=abc.ABCMeta):
     """A plugin that is always going to go through a rescope process.
 
     The original keystone plugins could simply pass a project or domain to
     along with the credentials and get a scoped token. For federation, K2K and
     newer mechanisms we always get an unscoped token first and then rescope.
 
     This is currently not public as it's generally an abstraction of a flow
@@ -99,16 +96,19 @@
         super(FederationBaseAuth, self).__init__(auth_url=auth_url, **kwargs)
         self.identity_provider = identity_provider
         self.protocol = protocol
 
     @property
     def federated_token_url(self):
         """Full URL where authorization data is sent."""
+        host = self.auth_url.rstrip('/')
+        if not host.endswith('v3'):
+            host += '/v3'
         values = {
-            'host': self.auth_url.rstrip('/'),
+            'host': host,
             'identity_provider': self.identity_provider,
             'protocol': self.protocol
         }
         url = ("%(host)s/OS-FEDERATION/identity_providers/"
                "%(identity_provider)s/protocols/%(protocol)s/auth")
         url = url % values
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/k2k.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/k2k.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-import six
-
 from keystoneauth1 import access
 from keystoneauth1 import exceptions
 from keystoneauth1.identity.v3 import federation
 from keystoneauth1 import plugin
 
 __all__ = ('Keystone2Keystone',)
 
@@ -115,15 +113,15 @@
                    "exit code: %(status_code)d, reason: %(err)s")
             msg = msg % {'status_code': resp.status_code, 'err': resp.reason}
             raise exceptions.AuthorizationFailure(msg)
 
         if not resp.text:
             raise exceptions.InvalidResponse(resp)
 
-        return six.text_type(resp.text)
+        return str(resp.text)
 
     def _send_service_provider_ecp_authn_response(self, session, sp_url,
                                                   sp_auth_url):
         """Present ECP wrapped SAML assertion to the keystone SP.
 
         The assertion is issued by the keystone IdP and it is targeted to the
         keystone that will serve as Service Provider.
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/multi_factor.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/multi_factor.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/oauth2_client_credential.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/oauth2_client_credential.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/oidc.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/oidc.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,33 +7,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import abc
+import time
+from urllib import parse as urlparse
 import warnings
 
-import six
-
 from keystoneauth1 import _utils as utils
 from keystoneauth1 import access
 from keystoneauth1 import exceptions
 from keystoneauth1.identity.v3 import federation
 
 _logger = utils.get_logger(__name__)
 
 __all__ = ('OidcAuthorizationCode',
            'OidcClientCredentials',
            'OidcPassword',
            'OidcAccessToken')
 
 
-@six.add_metaclass(abc.ABCMeta)
-class _OidcBase(federation.FederationBaseAuth):
+class _OidcBase(federation.FederationBaseAuth, metaclass=abc.ABCMeta):
     """Base class for different OpenID Connect based flows.
 
     The OpenID Connect specification can be found at::
     ``http://openid.net/specs/openid-connect-core-1_0.html``
     """
 
     grant_type = None
@@ -127,16 +126,16 @@
         :param session: a session object to send out HTTP requests.
         :type session: keystoneauth1.session.Session
 
         :returns: a python dictionary containing the discovery document if any,
                   otherwise it will return an empty dict.
         :rtype: dict
         """
-        if (self.discovery_endpoint is not None and
-                not self._discovery_document):
+        if (self.discovery_endpoint is not None
+                and not self._discovery_document):
             try:
                 resp = session.get(self.discovery_endpoint,
                                    authenticated=False)
             except exceptions.HttpError:
                 _logger.error("Cannot fetch discovery document %(discovery)s" %
                               {"discovery": self.discovery_endpoint})
                 raise
@@ -243,17 +242,16 @@
 
         :returns: a token data representation
         :rtype: :py:class:`keystoneauth1.access.AccessInfoV3`
         """
         # First of all, check if the grant type is supported
         discovery = self._get_discovery_document(session)
         grant_types = discovery.get("grant_types_supported")
-        if (grant_types and
-                self.grant_type is not None and
-                self.grant_type not in grant_types):
+        if (grant_types and self.grant_type is not None
+                and self.grant_type not in grant_types):
             raise exceptions.OidcPluginNotSupported()
 
         # Get the payload
         payload = self.get_payload(session)
         payload.setdefault('grant_type', self.grant_type)
 
         # get an access token
@@ -469,7 +467,139 @@
         :type session: keystoneauth1.session.Session
 
         :returns: a token data representation
         :rtype: :py:class:`keystoneauth1.access.AccessInfoV3`
         """
         response = self._get_keystone_token(session, self.access_token)
         return access.create(resp=response)
+
+
+class OidcDeviceAuthorization(_OidcBase):
+    """Implementation for OAuth 2.0 Device Authorization Grant."""
+
+    grant_type = "urn:ietf:params:oauth:grant-type:device_code"
+    HEADER_X_FORM = {"Content-Type": "application/x-www-form-urlencoded"}
+
+    def __init__(self, auth_url, identity_provider, protocol,  # nosec
+                 client_id, client_secret,
+                 access_token_endpoint=None,
+                 device_authorization_endpoint=None,
+                 discovery_endpoint=None,
+                 **kwargs):
+        """The OAuth 2.0 Device Authorization plugin expects the following.
+
+        :param device_authorization_endpoint: OAuth 2.0 Device Authorization
+                                  Endpoint, for example:
+                                  https://localhost:8020/oidc/authorize/device
+                                  Note that if a discovery document is
+                                  provided this value will override
+                                  the discovered one.
+        :type device_authorization_endpoint: string
+        """
+        # RFC 8628 only allows to retrieve an access_token
+        self.access_token_type = 'access_token'
+        self.device_authorization_endpoint = device_authorization_endpoint
+
+        super(OidcDeviceAuthorization, self).__init__(
+            auth_url=auth_url,
+            identity_provider=identity_provider,
+            protocol=protocol,
+            client_id=client_id,
+            client_secret=client_secret,
+            access_token_endpoint=access_token_endpoint,
+            discovery_endpoint=discovery_endpoint,
+            access_token_type=self.access_token_type,
+            **kwargs)
+
+    def _get_device_authorization_endpoint(self, session):
+        """Get the endpoint for the OAuth 2.0 Device Authorization flow.
+
+        This method will return the correct device authorization endpoint to
+        be used.
+        If the user has explicitly passed an device_authorization_endpoint to
+        the constructor that will be returned. If there is no explicit endpoint
+        and a discovery url is provided, it will try to get it from the
+        discovery document. If nothing is found, an exception will be raised.
+
+        :param session: a session object to send out HTTP requests.
+        :type session: keystoneauth1.session.Session
+
+        :return: the endpoint to use
+        :rtype: string or None if no endpoint is found
+        """
+        if self.device_authorization_endpoint is not None:
+            return self.device_authorization_endpoint
+
+        discovery = self._get_discovery_document(session)
+        endpoint = discovery.get("device_authorization_endpoint")
+        if endpoint is None:
+            raise exceptions.oidc.OidcDeviceAuthorizationEndpointNotFound()
+        return endpoint
+
+    def get_payload(self, session):
+        """Get an authorization grant for the "device_code" grant type.
+
+        :param session: a session object to send out HTTP requests.
+        :type session: keystoneauth1.session.Session
+
+        :returns: a python dictionary containing the payload to be exchanged
+        :rtype: dict
+        """
+        client_auth = (self.client_id, self.client_secret)
+        device_authz_endpoint = \
+            self._get_device_authorization_endpoint(session)
+        op_response = session.post(device_authz_endpoint,
+                                   requests_auth=client_auth,
+                                   data={},
+                                   authenticated=False)
+
+        self.expires_in = int(op_response.json()["expires_in"])
+        self.timeout = time.time() + self.expires_in
+        self.device_code = op_response.json()["device_code"]
+        self.interval = int(op_response.json()["interval"])
+        self.user_code = op_response.json()["user_code"]
+        self.verification_uri = op_response.json()["verification_uri"]
+        self.verification_uri_complete = \
+            op_response.json()["verification_uri_complete"]
+
+        payload = {'device_code': self.device_code}
+        return payload
+
+    def _get_access_token(self, session, payload):
+        """Poll token endpoint for an access token.
+
+        :param session: a session object to send out HTTP requests.
+        :type session: keystoneauth1.session.Session
+
+        :param payload: a dict containing various OpenID Connect values,
+                for example::
+                {'grant_type': 'urn:ietf:params:oauth:grant-type:device_code',
+                 'device_code': self.device_code}
+        :type payload: dict
+        """
+        print(f"\nTo authenticate please go to: "
+              f"{self.verification_uri_complete}")
+
+        client_auth = (self.client_id, self.client_secret)
+        access_token_endpoint = self._get_access_token_endpoint(session)
+        encoded_payload = urlparse.urlencode(payload)
+
+        while time.time() < self.timeout:
+            try:
+                op_response = session.post(access_token_endpoint,
+                                           requests_auth=client_auth,
+                                           data=encoded_payload,
+                                           headers=self.HEADER_X_FORM,
+                                           authenticated=False)
+            except exceptions.http.BadRequest as exc:
+                error = exc.response.json().get("error")
+                if error != "authorization_pending":
+                    raise
+                time.sleep(self.interval)
+                continue
+            break
+        else:
+            if error == "authorization_pending":
+                raise exceptions.oidc.OidcDeviceAuthorizationTimeOut()
+
+        access_token = op_response.json()[self.access_token_type]
+        return access_token
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/password.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/password.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/receipt.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/receipt.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/token.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/token.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/tokenless_auth.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/tokenless_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import abc
 
-import six
-
 from keystoneauth1 import _utils as utils
 from keystoneauth1 import plugin
 
 LOG = utils.get_logger(__name__)
 
 
-@six.add_metaclass(abc.ABCMeta)
-class TokenlessAuth(plugin.BaseAuthPlugin):
+class TokenlessAuth(plugin.BaseAuthPlugin, metaclass=abc.ABCMeta):
     """A plugin for authenticating with Tokenless Auth.
 
     This is for Tokenless Authentication. Scoped information
     like domain name and project ID will be passed in the headers and
     token validation request will be authenticated based on
     the provided HTTPS certificate along with the scope information.
     """
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/identity/v3/totp.py` & `keystoneauth1-5.2.0/keystoneauth1/identity/v3/totp.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/admin_token.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/admin_token.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/http_basic.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/http_basic.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/identity/generic.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/generic.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/identity/v2.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/v2.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/identity/v3.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/identity/v3.py`

 * *Files 18% similar despite different names*

```diff
@@ -187,14 +187,37 @@
         options.extend([
             loading.Opt('access-token', secret=True, required=True,
                         help='OAuth 2.0 Access Token'),
         ])
         return options
 
 
+class OpenIDConnectDeviceAuthorization(_OpenIDConnectBase):
+
+    @property
+    def plugin_class(self):
+        return identity.V3OidcDeviceAuthorization
+
+    def get_options(self):
+        options = super(OpenIDConnectDeviceAuthorization, self).get_options()
+
+        # RFC 8628 doesn't support id_token
+        options = [opt for opt in options if opt.name != 'access-token-type']
+
+        options.extend([
+            loading.Opt('device-authorization-endpoint',
+                        help='OAuth 2.0 Device Authorization Endpoint. Note '
+                        'that if a discovery document is being passed this '
+                        'option will override the endpoint provided by the '
+                        'server in the discovery document.'),
+        ])
+
+        return options
+
+
 class TOTP(loading.BaseV3Loader):
 
     @property
     def plugin_class(self):
         return identity.V3TOTP
 
     def get_options(self):
@@ -375,7 +398,38 @@
             m = 'You must provide an OAuth2.0 client credential ID.'
             raise exceptions.OptionError(m)
         if not kwargs.get('oauth2_client_secret'):
             m = 'You must provide an OAuth2.0 client credential auth secret.'
             raise exceptions.OptionError(m)
 
         return super(OAuth2ClientCredential, self).load_from_options(**kwargs)
+
+
+class OAuth2mTlsClientCredential(loading.BaseV3Loader):
+
+    @property
+    def plugin_class(self):
+        return identity.V3OAuth2mTlsClientCredential
+
+    def get_options(self):
+        options = super(OAuth2mTlsClientCredential, self).get_options()
+        options.extend([
+            loading.Opt('oauth2-endpoint',
+                        required=True,
+                        help='Endpoint for OAuth2.0 Mutual-TLS Authorization'),
+            loading.Opt('oauth2-client-id',
+                        required=True,
+                        help='Client credential ID for OAuth2.0 Mutual-TLS '
+                             'Authorization')
+        ])
+        return options
+
+    def load_from_options(self, **kwargs):
+        if not kwargs.get('oauth2_endpoint'):
+            m = 'You must provide an OAuth2.0 Mutual-TLS endpoint.'
+            raise exceptions.OptionError(m)
+        if not kwargs.get('oauth2_client_id'):
+            m = ('You must provide an client credential ID for '
+                 'OAuth2.0 Mutual-TLS Authorization.')
+            raise exceptions.OptionError(m)
+        return super(OAuth2mTlsClientCredential,
+                     self).load_from_options(**kwargs)
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/_plugins/noauth.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/_plugins/noauth.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/_utils.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/_utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/adapter.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/adapter.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/base.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import abc
 
-import six
 import stevedore
 
 from keystoneauth1 import exceptions
 
 PLUGIN_NAMESPACE = 'keystoneauth1.plugin'
 
 
@@ -95,16 +94,15 @@
 
     :raises keystoneauth1.exceptions.auth_plugins.NoMatchingPlugin:
         if a plugin cannot be created.
     """
     return get_plugin_loader(name).get_options()
 
 
-@six.add_metaclass(abc.ABCMeta)
-class BaseLoader(object):
+class BaseLoader(metaclass=abc.ABCMeta):
 
     @property
     def plugin_class(self):
         raise NotImplementedError()
 
     def create_plugin(self, **kwargs):
         """Create a plugin from the options available for the loader.
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/cli.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/cli.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/conf.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/conf.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/identity.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/identity.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/opts.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/opts.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/loading/session.py` & `keystoneauth1-5.2.0/keystoneauth1/loading/session.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/noauth.py` & `keystoneauth1-5.2.0/keystoneauth1/noauth.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/plugin.py` & `keystoneauth1-5.2.0/keystoneauth1/plugin.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/service_token.py` & `keystoneauth1-5.2.0/keystoneauth1/service_token.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/session.py` & `keystoneauth1-5.2.0/keystoneauth1/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,18 @@
 import json
 import logging
 import os
 import platform
 import socket
 import sys
 import time
+import urllib
 import uuid
 
 import requests
-import six
-from six.moves import urllib
 
 import keystoneauth1
 from keystoneauth1 import _utils as utils
 from keystoneauth1 import discover
 from keystoneauth1 import exceptions
 
 try:
@@ -88,26 +87,19 @@
     return headers
 
 
 def _sanitize_headers(headers):
     """Ensure headers are strings and not bytes."""
     str_dict = {}
     for k, v in headers.items():
-        if six.PY3:
-            # requests expects headers to be str type in python3, which means
-            # if we get a bytes we need to decode it into a str
-            k = k.decode('ASCII') if isinstance(k, six.binary_type) else k
-            if v is not None:
-                v = v.decode('ASCII') if isinstance(v, six.binary_type) else v
-        else:
-            # requests expects headers to be str type in python2, which means
-            # if we get a unicode we need to encode it to ASCII into a str
-            k = k.encode('ASCII') if isinstance(k, six.text_type) else k
-            if v is not None:
-                v = v.encode('ASCII') if isinstance(v, six.text_type) else v
+        # requests expects headers to be str type in python3, which means
+        # if we get a bytes we need to decode it into a str
+        k = k.decode('ASCII') if isinstance(k, bytes) else k
+        if v is not None:
+            v = v.decode('ASCII') if isinstance(v, bytes) else v
         str_dict[k] = v
     return str_dict
 
 
 class NoOpSemaphore(object):
     """Empty context manager for use as a default semaphore."""
 
@@ -122,17 +114,17 @@
 
 class _JSONEncoder(json.JSONEncoder):
 
     def default(self, o):
         if isinstance(o, datetime.datetime):
             return o.isoformat()
         if isinstance(o, uuid.UUID):
-            return six.text_type(o)
+            return str(o)
         if netaddr and isinstance(o, netaddr.IPAddress):
-            return six.text_type(o)
+            return str(o)
 
         return super(_JSONEncoder, self).default(o)
 
 
 class _StringFormatter(object):
     """A String formatter that fetches values on demand."""
 
@@ -481,15 +473,15 @@
 
         string_parts.append('curl -g -i')
 
         # NOTE(jamielennox): None means let requests do its default validation
         # so we need to actually check that this is False.
         if self.verify is False:
             string_parts.append('--insecure')
-        elif isinstance(self.verify, six.string_types):
+        elif isinstance(self.verify, str):
             string_parts.append('--cacert "%s"' % self.verify)
 
         if method:
             string_parts.extend(['-X', method])
 
         if query_params:
             # Don't check against `is not None` as this can be
@@ -505,15 +497,15 @@
             # Sort headers so that testing can work consistently.
             for header in sorted(headers.items()):
                 string_parts.append('-H "%s: %s"'
                                     % self._process_header(header))
         if json:
             data = self._json.encode(json)
         if data:
-            if isinstance(data, six.binary_type):
+            if isinstance(data, bytes):
                 try:
                     data = data.decode("ascii")
                 except UnicodeDecodeError:
                     data = "<binary_data>"
             string_parts.append("-d '%s'" % data)
 
         logger.debug(' '.join(string_parts))
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/access/test_v2_access.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v2_access.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/access/test_v2_service_catalog.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v2_service_catalog.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/access/test_v3_access.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v3_access.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/access/test_v3_service_catalog.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/access/test_v3_service_catalog.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/client_fixtures.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/keystone_v2_sample_response.json` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/keystone_v2_sample_response.json`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/keystone_v3_sample_response.json` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/keystone_v3_sample_response.json`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/ksa_betamax_test_cassette.yaml` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/ksa_betamax_test_cassette.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/data/ksa_serializer_data.json` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/data/ksa_serializer_data.json`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/exceptions/test_exceptions.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/exceptions/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/base.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/base.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/test_fedkerb_loading.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_fedkerb_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/test_kerberos_loading.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_kerberos_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/test_mapped.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_mapped.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/test_v3.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/test_v3.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/kerberos/utils.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/kerberos/utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/oauth1/test_oauth1.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/oauth1/test_oauth1.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import uuid
 
 from oauthlib import oauth1
-import six
 from testtools import matchers
 
 from keystoneauth1.extras import oauth1 as ksa_oauth1
 from keystoneauth1 import fixture
 from keystoneauth1 import session
 from keystoneauth1.tests.unit import utils as test_utils
 
@@ -43,15 +42,15 @@
         """
         self.assertThat(auth_header, matchers.StartsWith('OAuth '))
         parameters = dict(
             oauth1.rfc5849.utils.parse_authorization_header(auth_header))
 
         self.assertEqual('HMAC-SHA1', parameters['oauth_signature_method'])
         self.assertEqual('1.0', parameters['oauth_version'])
-        self.assertIsInstance(parameters['oauth_nonce'], six.string_types)
+        self.assertIsInstance(parameters['oauth_nonce'], str)
         self.assertEqual(oauth_client.client_key,
                          parameters['oauth_consumer_key'])
         if oauth_client.resource_owner_key:
             self.assertEqual(oauth_client.resource_owner_key,
                              parameters['oauth_token'],)
         if oauth_client.verifier:
             self.assertEqual(oauth_client.verifier,
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/oauth1/test_oauth1_loading.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/oauth1/test_oauth1_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_RequestSecurityTokenResponse.xml` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_RequestSecurityTokenResponse.xml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_fault.xml` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/examples/xml/ADFS_fault.xml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/fixtures/__init__.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/authn_request.xml` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/authn_request.xml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/saml_assertion.xml` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/saml_assertion.xml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/soap_response.xml` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/fixtures/templates/soap_response.xml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/test_auth_adfs.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/test_auth_adfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+import urllib
 import uuid
 
 from lxml import etree
-from six.moves import urllib
 
 from keystoneauth1 import exceptions
 from keystoneauth1.extras import _saml2 as saml2
 from keystoneauth1.tests.unit import client_fixtures
 from keystoneauth1.tests.unit.extras.saml2 import fixtures as saml2_fixtures
 from keystoneauth1.tests.unit.extras.saml2 import utils
 from keystoneauth1.tests.unit import matchers
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/test_auth_saml2.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/test_auth_saml2.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/extras/saml2/utils.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/extras/saml2/utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_access.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_access.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_identity_common.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import abc
 import collections
+import urllib
 import uuid
 
-import six
-from six.moves import urllib
-
 from keystoneauth1 import _utils
 from keystoneauth1 import access
 from keystoneauth1 import adapter
 from keystoneauth1 import discover
 from keystoneauth1 import exceptions
 from keystoneauth1 import fixture
 from keystoneauth1 import identity
@@ -72,16 +70,15 @@
         url = urllib.parse.urljoin(self.base_url + '/', interface)
         for part in parts:
             if part:
                 url = urllib.parse.urljoin(url + '/', part)
         return url
 
 
-@six.add_metaclass(abc.ABCMeta)
-class CommonIdentityTests(object):
+class CommonIdentityTests(metaclass=abc.ABCMeta):
 
     PROJECT_ID = uuid.uuid4().hex
     TEST_ROOT_URL = 'http://127.0.0.1:5000/'
     TEST_ROOT_ADMIN_URL = 'http://127.0.0.1:35357/'
 
     TEST_COMPUTE_BASE = 'https://compute.example.com'
     TEST_COMPUTE_PUBLIC = TEST_COMPUTE_BASE + '/nova/public'
@@ -129,15 +126,16 @@
         try:
             self.project_id = token.project_id
         except AttributeError:
             self.project_id = token.tenant_id
 
         self.stub_auth(json=token)
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def version(self):
         """The API version being tested."""
 
     def test_discovering(self):
         disc = fixture.DiscoveryList(v2=False, v3=False)
 
         disc.add_nova_microversion(
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_identity_v2.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v2.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_identity_v3.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v3.py`

 * *Files 13% similar despite different names*

```diff
@@ -221,14 +221,45 @@
                 },
                 "issued_at": "2013-05-29T16:55:21.468960Z",
                 "catalog": self.TEST_SERVICE_CATALOG,
                 "service_providers": self.TEST_SERVICE_PROVIDERS,
                 "application_credential_restricted": True
             },
         }
+        self.TEST_OAUTH2_MTLS_TOKEN_RESPONSE = {
+            "token": {
+                "methods": [
+                    "oauth2_credential"
+                ],
+
+                "expires_at": "%i-02-01T00:00:10.000123Z" % nextyear,
+                "project": {
+                    "domain": {
+                        "id": self.TEST_DOMAIN_ID,
+                        "name": self.TEST_DOMAIN_NAME
+                    },
+                    "id": self.TEST_TENANT_ID,
+                    "name": self.TEST_TENANT_NAME
+                },
+                "user": {
+                    "domain": {
+                        "id": self.TEST_DOMAIN_ID,
+                        "name": self.TEST_DOMAIN_NAME
+                    },
+                    "id": self.TEST_USER,
+                    "name": self.TEST_USER
+                },
+                "issued_at": "2013-05-29T16:55:21.468960Z",
+                "catalog": self.TEST_SERVICE_CATALOG,
+                "service_providers": self.TEST_SERVICE_PROVIDERS,
+                "oauth2_credential": {
+                    "x5t#S256": "7UN-z4yFIm9s4jakecGoKa4rc353pDCuFUo9fsDD_1s="
+                }
+            },
+        }
         self.TEST_RECEIPT_RESPONSE = {
             "receipt": {
                 "methods": ["password"],
                 "expires_at": "%i-02-01T00:00:10.000123Z" % nextyear,
                 "user": {
                     "domain": {
                         "id": self.TEST_DOMAIN_ID,
@@ -1081,7 +1112,219 @@
                                  resp_ok])
 
         resp = sess.post(f'{base_https}/auth/tokens', authenticated=True)
         self.assertRequestHeaderEqual('Authorization',
                                       f'Bearer {oauth2_token}')
         self.assertEqual(200, resp.status_code)
         self.assertEqual(resp_text, resp.text)
+
+    def test_oauth2_mtls_client_credential_method(self):
+        base_https = self.TEST_URL.replace('http:', 'https:')
+        token_endpoint = f'{self.TEST_URL}/auth/tokens'
+        oauth2_endpoint = f'{base_https}/OS-OAUTH2/token'
+        oauth2_token = 'HW9bB6oYWJywz6mAN_KyIBXlof15Pk'
+        a = v3.OAuth2mTlsClientCredential(
+            self.TEST_URL,
+            oauth2_endpoint=oauth2_endpoint,
+            oauth2_client_id=self.TEST_CLIENT_CRED_ID
+        )
+
+        oauth2_post_resp = {
+            'status_code': 200,
+            'json': {
+                'access_token': oauth2_token,
+                'expires_in': 3600,
+                'token_type': 'Bearer'
+            }
+        }
+        self.requests_mock.post(oauth2_endpoint, [oauth2_post_resp])
+        token_verify_resp = {
+            'status_code': 200,
+            'json': {
+                **self.TEST_OAUTH2_MTLS_TOKEN_RESPONSE
+            }
+        }
+        self.requests_mock.get(token_endpoint, [token_verify_resp])
+
+        sess = session.Session(auth=a)
+        auth_ref = a.get_auth_ref(sess)
+        self.assertEqual(auth_ref.auth_token, oauth2_token)
+        self.assertEqual(auth_ref._data,
+                         self.TEST_OAUTH2_MTLS_TOKEN_RESPONSE)
+        self.assertEqual(
+            auth_ref.project_id,
+            self.TEST_OAUTH2_MTLS_TOKEN_RESPONSE.get(
+                'token', {}).get('project', {}).get('id'))
+        self.assertIsNone(auth_ref.domain_id)
+        self.assertEqual(
+            auth_ref.oauth2_credential,
+            self.TEST_OAUTH2_MTLS_TOKEN_RESPONSE.get(
+                'token', {}).get('oauth2_credential'))
+        self.assertEqual(
+            auth_ref.oauth2_credential_thumbprint,
+            self.TEST_OAUTH2_MTLS_TOKEN_RESPONSE.get(
+                'token', {}).get('oauth2_credential', {}).get('x5t#S256')
+        )
+
+        auth_head = sess.get_auth_headers()
+        self.assertEqual(f'Bearer {oauth2_token}', auth_head['Authorization'])
+        self.assertEqual(oauth2_token, auth_head['X-Auth-Token'])
+
+    def test_oauth2_mtls_client_credential_method_without_v3(self):
+        base_https = self.TEST_URL.replace('http:', 'https:')
+        token_endpoint = f'{self.TEST_URL}/auth/tokens'
+        oauth2_endpoint = f'{base_https}/OS-OAUTH2/token'
+        oauth2_token = 'HW9bB6oYWJywz6mAN_KyIBXlof15Pk'
+        a = v3.OAuth2mTlsClientCredential(
+            self.TEST_URL.replace('v3', ''),
+            oauth2_endpoint=oauth2_endpoint,
+            oauth2_client_id=self.TEST_CLIENT_CRED_ID
+        )
+
+        oauth2_post_resp = {
+            'status_code': 200,
+            'json': {
+                'access_token': oauth2_token,
+                'expires_in': 3600,
+                'token_type': 'Bearer'
+            }
+        }
+        self.requests_mock.post(oauth2_endpoint, [oauth2_post_resp])
+        token_verify_resp = {
+            'status_code': 200,
+            'json': {
+                **self.TEST_OAUTH2_MTLS_TOKEN_RESPONSE
+            }
+        }
+        self.requests_mock.get(token_endpoint, [token_verify_resp])
+
+        sess = session.Session(auth=a)
+        auth_ref = a.get_auth_ref(sess)
+        self.assertEqual(auth_ref.auth_token, oauth2_token)
+        self.assertEqual(auth_ref._data,
+                         self.TEST_OAUTH2_MTLS_TOKEN_RESPONSE)
+        self.assertEqual(
+            auth_ref.oauth2_credential,
+            self.TEST_OAUTH2_MTLS_TOKEN_RESPONSE.get(
+                'token', {}).get('oauth2_credential'))
+        self.assertEqual(
+            auth_ref.oauth2_credential_thumbprint,
+            self.TEST_OAUTH2_MTLS_TOKEN_RESPONSE.get(
+                'token', {}).get('oauth2_credential', {}).get('x5t#S256')
+        )
+        auth_head = sess.get_auth_headers()
+        self.assertEqual(f'Bearer {oauth2_token}', auth_head['Authorization'])
+        self.assertEqual(oauth2_token, auth_head['X-Auth-Token'])
+
+    def test_oauth2_mtls_client_credential_method_resp_invalid_json(self):
+        base_https = self.TEST_URL.replace('http:', 'https:')
+        token_endpoint = f'{self.TEST_URL}/auth/tokens'
+        oauth2_endpoint = f'{base_https}/OS-OAUTH2/token'
+        oauth2_token = 'HW9bB6oYWJywz6mAN_KyIBXlof15Pk'
+        a = v3.OAuth2mTlsClientCredential(
+            self.TEST_URL,
+            oauth2_endpoint=oauth2_endpoint,
+            oauth2_client_id=self.TEST_CLIENT_CRED_ID
+        )
+
+        oauth2_post_resp = {
+            'status_code': 200,
+            'json': {
+                'access_token': oauth2_token,
+                'expires_in': 3600,
+                'token_type': 'Bearer'
+            }
+        }
+        self.requests_mock.post(oauth2_endpoint, [oauth2_post_resp])
+        token_verify_resp = {
+            'status_code': 200,
+            'text': 'invalid json'
+        }
+        self.requests_mock.get(token_endpoint, [token_verify_resp])
+
+        sess = session.Session(auth=a)
+        self.assertRaises(exceptions.InvalidResponse, a.get_auth_ref, sess)
+
+    def test_oauth2_mtls_client_credential_method_resp_without_token(self):
+        base_https = self.TEST_URL.replace('http:', 'https:')
+        token_endpoint = f'{self.TEST_URL}/auth/tokens'
+        oauth2_endpoint = f'{base_https}/OS-OAUTH2/token'
+        oauth2_token = 'HW9bB6oYWJywz6mAN_KyIBXlof15Pk'
+        a = v3.OAuth2mTlsClientCredential(
+            self.TEST_URL,
+            oauth2_endpoint=oauth2_endpoint,
+            oauth2_client_id=self.TEST_CLIENT_CRED_ID
+        )
+
+        oauth2_post_resp = {
+            'status_code': 200,
+            'json': {
+                'access_token': oauth2_token,
+                'expires_in': 3600,
+                'token_type': 'Bearer'
+            }
+        }
+        self.requests_mock.post(oauth2_endpoint, [oauth2_post_resp])
+        token_verify_resp = {
+            'status_code': 200,
+            'json': {
+                'without_token': {}
+            }
+        }
+        self.requests_mock.get(token_endpoint, [token_verify_resp])
+
+        sess = session.Session(auth=a)
+        self.assertRaises(exceptions.InvalidResponse, a.get_auth_ref, sess)
+
+    def test_oauth2_mtls_client_credential_method_client_exception(self):
+        base_https = self.TEST_URL.replace('http:', 'https:')
+        oauth2_endpoint = f'{base_https}/OS-OAUTH2/token'
+        a = v3.OAuth2mTlsClientCredential(
+            self.TEST_URL,
+            oauth2_endpoint=oauth2_endpoint,
+            oauth2_client_id=self.TEST_CLIENT_CRED_ID
+        )
+
+        oauth2_post_resp = {
+            'status_code': 400,
+            'json': {}
+        }
+        self.requests_mock.post(oauth2_endpoint, [oauth2_post_resp])
+
+        sess = session.Session(auth=a)
+        self.assertRaises(exceptions.ClientException, a.get_auth_ref, sess)
+
+    def test_oauth2_mtls_client_credential_method_base_header_none(self):
+        base_https = self.TEST_URL.replace('http:', 'https:')
+        token_endpoint = f'{self.TEST_URL}/auth/tokens'
+        oauth2_endpoint = f'{base_https}/OS-OAUTH2/token'
+        oauth2_token = 'HW9bB6oYWJywz6mAN_KyIBXlof15Pk'
+        a = v3.OAuth2mTlsClientCredential(
+            self.TEST_URL,
+            oauth2_endpoint=oauth2_endpoint,
+            oauth2_client_id=self.TEST_CLIENT_CRED_ID
+        )
+        oauth2_post_resp = {
+            'status_code': 200,
+            'json': {
+                'access_token': oauth2_token,
+                'expires_in': 3600,
+                'token_type': 'Bearer'
+            }
+        }
+        self.requests_mock.post(oauth2_endpoint,
+                                [oauth2_post_resp])
+        token_verify_resp = {
+            'status_code': 200,
+            'json': {
+                **self.TEST_OAUTH2_MTLS_TOKEN_RESPONSE
+            }
+        }
+        self.requests_mock.get(token_endpoint, [token_verify_resp])
+        sess = session.Session(auth=a)
+
+        with unittest.mock.patch(
+                'keystoneauth1.plugin.BaseAuthPlugin.'
+                'get_headers') as co_mock:
+            co_mock.return_value = None
+            auth_head = sess.get_auth_headers()
+            self.assertEqual('Bearer None', auth_head['Authorization'])
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_identity_v3_federation.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v3_federation.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import copy
 import uuid
 
-import six
-
 from keystoneauth1 import access
 from keystoneauth1 import exceptions
 from keystoneauth1 import fixture
 from keystoneauth1 import identity
 from keystoneauth1.identity import v3
 from keystoneauth1 import session
 from keystoneauth1.tests.unit import k2k_fixtures
@@ -75,14 +73,18 @@
         kwargs.setdefault('identity_provider', self.idp)
         return TesterFederationPlugin(**kwargs)
 
     def test_federated_url(self):
         plugin = self.get_plugin()
         self.assertEqual(self.token_url, plugin.federated_token_url)
 
+    def test_federated_url_unversioned(self):
+        plugin = self.get_plugin(auth_url="http://keystone/")
+        self.assertEqual(self.token_url, plugin.federated_token_url)
+
     def test_unscoped_behaviour(self):
         sess = session.Session(auth=self.get_plugin())
         self.assertEqual(self.unscoped_token_id, sess.get_token())
 
         self.assertTrue(self.unscoped_mock.called)
         self.assertFalse(self.scoped_mock.called)
 
@@ -140,23 +142,23 @@
             json={'version': fixture.V3Discovery(self.TEST_URL)},
             headers={'Content-Type': 'application/json'})
 
         # The IdP should return a ECP wrapped assertion when requested
         self.requests_mock.register_uri(
             'POST',
             self.REQUEST_ECP_URL,
-            content=six.b(k2k_fixtures.ECP_ENVELOPE),
+            content=bytes(k2k_fixtures.ECP_ENVELOPE, 'latin-1'),
             headers={'Content-Type': 'application/vnd.paos+xml'},
             status_code=200)
 
         # The SP should respond with a redirect (302 or 303)
         self.requests_mock.register_uri(
             'POST',
             self.SP_URL,
-            content=six.b(k2k_fixtures.TOKEN_BASED_ECP),
+            content=bytes(k2k_fixtures.TOKEN_BASED_ECP, 'latin-1'),
             headers={'Content-Type': 'application/vnd.paos+xml'},
             status_code=redirect_code)
 
         # Should not follow the redirect URL, but use the auth_url attribute
         self.requests_mock.register_uri(
             'GET',
             self.SP_AUTH_URL,
@@ -191,30 +193,30 @@
             self.TEST_URL,
             json={'version': fixture.V3Discovery(self.TEST_URL)},
             headers={'Content-Type': 'application/json'})
 
         self.requests_mock.register_uri(
             'POST', self.REQUEST_ECP_URL,
             headers={'Content-Type': 'application/vnd.paos+xml'},
-            content=six.b(''), status_code=200)
+            content=b'', status_code=200)
 
         self.assertRaises(exceptions.InvalidResponse,
                           self.k2kplugin._get_ecp_assertion,
                           self.session)
 
     def test_get_ecp_assertion_wrong_headers(self):
         self.requests_mock.get(
             self.TEST_URL,
             json={'version': fixture.V3Discovery(self.TEST_URL)},
             headers={'Content-Type': 'application/json'})
 
         self.requests_mock.register_uri(
             'POST', self.REQUEST_ECP_URL,
             headers={'Content-Type': uuid.uuid4().hex},
-            content=six.b(''), status_code=200)
+            content=b'', status_code=200)
 
         self.assertRaises(exceptions.InvalidResponse,
                           self.k2kplugin._get_ecp_assertion,
                           self.session)
 
     def test_send_ecp_authn_response(self):
         self._mock_k2k_flow_urls()
@@ -255,23 +257,23 @@
             json=fixture.DiscoveryList(self.TEST_ROOT_URL),
             headers={'Content-Type': 'application/json'})
 
         # The IdP should return a ECP wrapped assertion when requested
         self.requests_mock.register_uri(
             'POST',
             self.REQUEST_ECP_URL,
-            content=six.b(k2k_fixtures.ECP_ENVELOPE),
+            content=bytes(k2k_fixtures.ECP_ENVELOPE, 'latin-1'),
             headers={'Content-Type': 'application/vnd.paos+xml'},
             status_code=200)
 
         # The SP should respond with a redirect (302 or 303)
         self.requests_mock.register_uri(
             'POST',
             self.SP_URL,
-            content=six.b(k2k_fixtures.TOKEN_BASED_ECP),
+            content=bytes(k2k_fixtures.TOKEN_BASED_ECP, 'latin-1'),
             headers={'Content-Type': 'application/vnd.paos+xml'},
             status_code=302)
 
         # Should not follow the redirect URL, but use the auth_url attribute
         self.requests_mock.register_uri(
             'GET',
             self.SP_AUTH_URL,
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_identity_v3_oidc.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_identity_v3_oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
+import urllib
 import uuid
 import warnings
 
-from six.moves import urllib
-
 from keystoneauth1 import exceptions
 from keystoneauth1.identity.v3 import oidc
 from keystoneauth1 import session
 from keystoneauth1.tests.unit import oidc_fixtures
 from keystoneauth1.tests.unit import utils
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_password.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_password.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_token.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_token.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/test_tokenless_auth.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/test_tokenless_auth.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/identity/utils.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/identity/utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/k2k_fixtures.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/k2k_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/keystoneauth_fixtures.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/keystoneauth_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_adapter.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_adapter.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_cli.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_cli.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_conf.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_conf.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_entry_points.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_entry_points.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_fixtures.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_generic.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_generic.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_loading.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_loading.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_session.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_session.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/test_v3.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/test_v3.py`

 * *Files 8% similar despite different names*

```diff
@@ -291,14 +291,64 @@
                            protocol=protocol)
 
         self.assertEqual(identity_provider, oidc.identity_provider)
         self.assertEqual(protocol, oidc.protocol)
         self.assertEqual(access_token, oidc.access_token)
 
 
+class OpenIDConnectDeviceAuthorizationTests(utils.TestCase):
+
+    plugin_name = "v3oidcdeviceauthz"
+
+    def setUp(self):
+        super(OpenIDConnectDeviceAuthorizationTests, self).setUp()
+
+        self.auth_url = uuid.uuid4().hex
+
+    def create(self, **kwargs):
+        kwargs.setdefault('auth_url', self.auth_url)
+        loader = loading.get_plugin_loader(self.plugin_name)
+        return loader.load_from_options(**kwargs)
+
+    def test_options(self):
+        options = loading.get_plugin_loader(self.plugin_name).get_options()
+        self.assertTrue(
+            set(['client-id', 'client-secret', 'access-token-endpoint',
+                 'openid-scope', 'discovery-endpoint',
+                 'device-authorization-endpoint']).issubset(
+                set([o.name for o in options]))
+        )
+
+    def test_basic(self):
+        access_token_endpoint = uuid.uuid4().hex
+        device_authorization_endpoint = uuid.uuid4().hex
+        scope = uuid.uuid4().hex
+        identity_provider = uuid.uuid4().hex
+        protocol = uuid.uuid4().hex
+        client_id = uuid.uuid4().hex
+        client_secret = uuid.uuid4().hex
+
+        dev_authz_endpt = device_authorization_endpoint
+        oidc = self.create(identity_provider=identity_provider,
+                           protocol=protocol,
+                           access_token_endpoint=access_token_endpoint,
+                           device_authorization_endpoint=dev_authz_endpt,
+                           client_id=client_id,
+                           client_secret=client_secret,
+                           scope=scope)
+
+        self.assertEqual(dev_authz_endpt, oidc.device_authorization_endpoint)
+        self.assertEqual(identity_provider, oidc.identity_provider)
+        self.assertEqual(protocol, oidc.protocol)
+        self.assertEqual(access_token_endpoint, oidc.access_token_endpoint)
+        self.assertEqual(client_id, oidc.client_id)
+        self.assertEqual(client_secret, oidc.client_secret)
+        self.assertEqual(scope, oidc.scope)
+
+
 class V3TokenlessAuthTests(utils.TestCase):
 
     def setUp(self):
         super(V3TokenlessAuthTests, self).setUp()
 
         self.auth_url = uuid.uuid4().hex
 
@@ -535,7 +585,45 @@
 
     def test_without_secret(self):
         oauth2_endpoint = "https://localhost/token"
         self.assertRaises(exceptions.OptionError,
                           self.create,
                           oauth2_endpoint=oauth2_endpoint,
                           oauth2_client_id=uuid.uuid4().hex)
+
+
+class V3Oauth2mTlsClientCredentialTests(utils.TestCase):
+
+    def setUp(self):
+        super(V3Oauth2mTlsClientCredentialTests, self).setUp()
+
+        self.auth_url = uuid.uuid4().hex
+
+    def create(self, **kwargs):
+        kwargs.setdefault('auth_url', self.auth_url)
+        loader = loading.get_plugin_loader('v3oauth2mtlsclientcredential')
+        return loader.load_from_options(**kwargs)
+
+    def test_basic(self):
+        client_id = uuid.uuid4().hex
+        oauth2_endpoint = "https://localhost/token"
+
+        client_cred = self.create(oauth2_endpoint=oauth2_endpoint,
+                                  oauth2_client_id=client_id
+                                  )
+        self.assertEqual(self.auth_url, client_cred.auth_url)
+        self.assertEqual(client_id, client_cred.oauth2_client_id)
+        self.assertEqual(oauth2_endpoint, client_cred.oauth2_endpoint)
+
+    def test_without_oauth2_endpoint(self):
+        client_id = uuid.uuid4().hex
+        self.assertRaises(exceptions.OptionError,
+                          self.create,
+                          oauth2_client_id=client_id,
+                          )
+
+    def test_without_client_id(self):
+        oauth2_endpoint = "https://localhost/token"
+        self.assertRaises(exceptions.OptionError,
+                          self.create,
+                          oauth2_endpoint=oauth2_endpoint,
+                          oauth2_client_secret=uuid.uuid4().hex)
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/loading/utils.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/loading/utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/matchers.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/matchers.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/oidc_fixtures.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/oidc_fixtures.py`

 * *Files 18% similar despite different names*

```diff
@@ -73,25 +73,28 @@
         "phone_number",
         "phone_number_verified",
         "address"
     ],
     "grant_types_supported": [
         "authorization_code",
         "password",
+        "urn:ietf:params:oauth:grant-type:device_code",
     ],
     "introspection_endpoint": "https://localhost:8020/oidc/introspect",
     "issuer": "https://localhost:8020/oidc/",
     "jwks_uri": "https://localhost:8020/oidc/jwk",
     "op_policy_uri": "https://localhost:8020/oidc/about",
     "op_tos_uri": "https://localhost:8020/oidc/about",
     "registration_endpoint": "https://localhost:8020/oidc/register",
     "revocation_endpoint": "https://localhost:8020/oidc/revoke",
     "service_documentation": "https://localhost:8020/oidc/about",
     "token_endpoint": "https://localhost:8020/oidc/token",
     "userinfo_endpoint": "https://localhost:8020/oidc/userinfo",
+    "device_authorization_endpoint":
+        "https://localhost:8020/oidc/authorize/device",
     "token_endpoint_auth_methods_supported": [
         "client_secret_post",
         "client_secret_basic",
         "client_secret_jwt",
         "private_key_jwt",
         "none"
     ],
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_betamax_fixture.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_betamax_fixture.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_betamax_hooks.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_betamax_hooks.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_betamax_serializer.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_betamax_serializer.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_discovery.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_discovery.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_fair_sempahore.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_fair_sempahore.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
+import queue
 from threading import Thread
 from timeit import default_timer as timer
 from unittest import mock
 
-from six.moves import queue
 import testtools
 
 from keystoneauth1 import _fair_semaphore
 
 
 class SemaphoreTests(testtools.TestCase):
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_fixtures.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_fixtures.py`

 * *Files 5% similar despite different names*

```diff
@@ -342,7 +342,21 @@
         token.is_admin_project = False
         self.assertIs(False, token.is_admin_project)
         self.assertIs(False, token['token']['is_admin_project'])
 
         del token.is_admin_project
         self.assertIsNone(token.is_admin_project)
         self.assertNotIn('is_admin_project', token['token'])
+
+    def test_oauth2(self):
+        methods = ['oauth2_credential']
+        oauth2_thumbprint = uuid.uuid4().hex
+        token = fixture.V3Token(
+            methods=methods,
+            oauth2_thumbprint=oauth2_thumbprint,
+        )
+        oauth2_credential = {
+            'x5t#S256': oauth2_thumbprint,
+        }
+        self.assertEqual(methods, token.methods)
+        self.assertEqual(oauth2_credential, token.oauth2_credential)
+        self.assertEqual(oauth2_thumbprint, token.oauth2_thumbprint)
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_hacking_checks.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_hacking_checks.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_http_basic.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_http_basic.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_matchers.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_matchers.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_noauth.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_noauth.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_service_token.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_service_token.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_session.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import datetime
+import io
 import itertools
 import json
 import logging
 import sys
 from unittest import mock
 import uuid
 
 from oslo_utils import encodeutils
 import requests
 import requests.auth
-import six
 from testtools import matchers
 
 from keystoneauth1 import adapter
 from keystoneauth1 import discover
 from keystoneauth1 import exceptions
 from keystoneauth1 import plugin
 from keystoneauth1 import session as client_session
@@ -1254,30 +1254,30 @@
         self.assertEqual(auth.TEST_PROJECT_ID, sess.get_project_id())
 
     def test_logger_object_passed(self):
         logger = logging.getLogger(uuid.uuid4().hex)
         logger.setLevel(logging.DEBUG)
         logger.propagate = False
 
-        io = six.StringIO()
-        handler = logging.StreamHandler(io)
+        string_io = io.StringIO()
+        handler = logging.StreamHandler(string_io)
         logger.addHandler(handler)
 
         auth = AuthPlugin()
         sess = client_session.Session(auth=auth)
         response = {uuid.uuid4().hex: uuid.uuid4().hex}
 
         self.stub_url('GET',
                       json=response,
                       headers={'Content-Type': 'application/json'})
 
         resp = sess.get(self.TEST_URL, logger=logger)
 
         self.assertEqual(response, resp.json())
-        output = io.getvalue()
+        output = string_io.getvalue()
 
         self.assertIn(self.TEST_URL, output)
         self.assertIn(list(response.keys())[0], output)
         self.assertIn(list(response.values())[0], output)
 
         self.assertNotIn(list(response.keys())[0], self.logger.output)
         self.assertNotIn(list(response.values())[0], self.logger.output)
@@ -1285,22 +1285,22 @@
     def test_split_loggers(self):
 
         def get_logger_io(name):
             logger_name = 'keystoneauth.session.{name}'.format(name=name)
             logger = logging.getLogger(logger_name)
             logger.setLevel(logging.DEBUG)
 
-            io = six.StringIO()
-            handler = logging.StreamHandler(io)
+            string_io = io.StringIO()
+            handler = logging.StreamHandler(string_io)
             logger.addHandler(handler)
-            return io
+            return string_io
 
-        io = {}
+        io_dict = {}
         for name in ('request', 'body', 'response', 'request-id'):
-            io[name] = get_logger_io(name)
+            io_dict[name] = get_logger_io(name)
 
         auth = AuthPlugin()
         sess = client_session.Session(auth=auth, split_loggers=True)
         response_key = uuid.uuid4().hex
         response_val = uuid.uuid4().hex
         response = {response_key: response_val}
         request_id = uuid.uuid4().hex
@@ -1318,18 +1318,18 @@
             headers={
                 encodeutils.safe_encode('x-bytes-header'):
                 encodeutils.safe_encode('bytes-value')
             })
 
         self.assertEqual(response, resp.json())
 
-        request_output = io['request'].getvalue().strip()
-        response_output = io['response'].getvalue().strip()
-        body_output = io['body'].getvalue().strip()
-        id_output = io['request-id'].getvalue().strip()
+        request_output = io_dict['request'].getvalue().strip()
+        response_output = io_dict['response'].getvalue().strip()
+        body_output = io_dict['body'].getvalue().strip()
+        id_output = io_dict['request-id'].getvalue().strip()
 
         self.assertIn('curl -g -i -X GET {url}'.format(url=self.TEST_URL),
                       request_output)
         self.assertIn('-H "x-bytes-header: bytes-value"', request_output)
         self.assertEqual('[200] Content-Type: application/json '
                          'X-OpenStack-Request-ID: '
                          '{id}'.format(id=request_id), response_output)
@@ -1603,31 +1603,31 @@
         self.assertEqual(auth.TEST_PROJECT_ID, adpt.get_project_id())
 
     def test_logger_object_passed(self):
         logger = logging.getLogger(uuid.uuid4().hex)
         logger.setLevel(logging.DEBUG)
         logger.propagate = False
 
-        io = six.StringIO()
-        handler = logging.StreamHandler(io)
+        string_io = io.StringIO()
+        handler = logging.StreamHandler(string_io)
         logger.addHandler(handler)
 
         auth = AuthPlugin()
         sess = client_session.Session(auth=auth)
         adpt = adapter.Adapter(sess, auth=auth, logger=logger)
 
         response = {uuid.uuid4().hex: uuid.uuid4().hex}
 
         self.stub_url('GET', json=response,
                       headers={'Content-Type': 'application/json'})
 
         resp = adpt.get(self.TEST_URL, logger=logger)
 
         self.assertEqual(response, resp.json())
-        output = io.getvalue()
+        output = string_io.getvalue()
 
         self.assertIn(self.TEST_URL, output)
         self.assertIn(list(response.keys())[0], output)
         self.assertIn(list(response.values())[0], output)
 
         self.assertNotIn(list(response.keys())[0], self.logger.output)
         self.assertNotIn(list(response.values())[0], self.logger.output)
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_token_endpoint.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_token_endpoint.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/test_utils.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1/tests/unit/utils.py` & `keystoneauth1-5.2.0/keystoneauth1/tests/unit/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import json as jsonutils
 import logging
 import time
+import urllib.parse
 import uuid
 
 import fixtures
 import requests
 from requests_mock.contrib import fixture
-from six.moves.urllib import parse as urlparse
 import testtools
 
 
 class TestCase(testtools.TestCase):
 
     TEST_DOMAIN_ID = uuid.uuid4().hex
     TEST_DOMAIN_NAME = uuid.uuid4().hex
@@ -76,31 +76,33 @@
         self.assertEqual(last_request.headers['Content-Type'], content_type)
 
     def assertQueryStringIs(self, qs=''):
         r"""Verify the QueryString matches what is expected.
 
         The qs parameter should be of the format \'foo=bar&abc=xyz\'
         """
-        expected = urlparse.parse_qs(qs, keep_blank_values=True)
-        parts = urlparse.urlparse(self.requests_mock.last_request.url)
-        querystring = urlparse.parse_qs(parts.query, keep_blank_values=True)
+        expected = urllib.parse.parse_qs(qs, keep_blank_values=True)
+        parts = urllib.parse.urlparse(self.requests_mock.last_request.url)
+        querystring = urllib.parse.parse_qs(
+            parts.query, keep_blank_values=True,
+        )
         self.assertEqual(expected, querystring)
 
     def assertQueryStringContains(self, **kwargs):
         """Verify the query string contains the expected parameters.
 
         This method is used to verify that the query string for the most recent
         request made contains all the parameters provided as ``kwargs``, and
         that the value of each parameter contains the value for the kwarg. If
         the value for the kwarg is an empty string (''), then all that's
         verified is that the parameter is present.
 
         """
-        parts = urlparse.urlparse(self.requests_mock.last_request.url)
-        qs = urlparse.parse_qs(parts.query, keep_blank_values=True)
+        parts = urllib.parse.urlparse(self.requests_mock.last_request.url)
+        qs = urllib.parse.parse_qs(parts.query, keep_blank_values=True)
 
         for k, v in kwargs.items():
             self.assertIn(k, qs)
             self.assertIn(v, qs[k])
 
     def assertRequestHeaderEqual(self, name, val):
         """Verify that the last request made contains a header and its value.
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1/token_endpoint.py` & `keystoneauth1-5.2.0/keystoneauth1/token_endpoint.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/keystoneauth1.egg-info/PKG-INFO` & `keystoneauth1-5.2.0/keystoneauth1.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystoneauth1
-Version: 5.1.2
+Version: 5.2.0
 Summary: Authentication Library for OpenStack Identity
 Home-page: https://docs.openstack.org/keystoneauth/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -52,12 +52,13 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
 Provides-Extra: betamax
 Provides-Extra: kerberos
 Provides-Extra: oauth1
 Provides-Extra: saml2
 Provides-Extra: test
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1.egg-info/SOURCES.txt` & `keystoneauth1-5.2.0/keystoneauth1.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 keystoneauth1/identity/v3/__init__.py
 keystoneauth1/identity/v3/application_credential.py
 keystoneauth1/identity/v3/base.py
 keystoneauth1/identity/v3/federation.py
 keystoneauth1/identity/v3/k2k.py
 keystoneauth1/identity/v3/multi_factor.py
 keystoneauth1/identity/v3/oauth2_client_credential.py
+keystoneauth1/identity/v3/oauth2_mtls_client_credential.py
 keystoneauth1/identity/v3/oidc.py
 keystoneauth1/identity/v3/password.py
 keystoneauth1/identity/v3/receipt.py
 keystoneauth1/identity/v3/token.py
 keystoneauth1/identity/v3/tokenless_auth.py
 keystoneauth1/identity/v3/totp.py
 keystoneauth1/loading/__init__.py
@@ -211,25 +212,27 @@
 releasenotes/notes/add-totp-auth-plugin-0650d220899c25b7.yaml
 releasenotes/notes/additional-headers-f2d16f85f5abe942.yaml
 releasenotes/notes/allow_version_hack-flag-9b53b72d9b084c04.yaml
 releasenotes/notes/api-sig-error-guideline-handler.yaml
 releasenotes/notes/basic-http-auth-45bea4298209df75.yaml
 releasenotes/notes/bp-application-credentials-416a1f8bb2311e04.yaml
 releasenotes/notes/bp-oauth2-client-credentials-ext-06271700d4f33a7e.yaml
+releasenotes/notes/bp-support-oauth2-mtls-177cda05265ae65c.yaml
 releasenotes/notes/bp-system-scope-29e9c597039ddb1e.yaml
 releasenotes/notes/bug-1582774-49af731b6dfc6f2f.yaml
 releasenotes/notes/bug-1614688-c4a1bd54f4ba5644.yaml
 releasenotes/notes/bug-1616105-cc8b85eb056e99e2.yaml
 releasenotes/notes/bug-1654847-acdf9543158329ec.yaml
 releasenotes/notes/bug-1689424-set-adfspassword-endpointreference-f186d84a54007b09.yaml
 releasenotes/notes/bug-1733052-1b4af3b3fe1b05bb.yaml
 releasenotes/notes/bug-1766235wq-0de60d0f996c6bfb.yaml
 releasenotes/notes/bug-1839748-5d8dfc99c43aaefc.yaml
 releasenotes/notes/bug-1840235-ef2946d149ac329c.yaml
 releasenotes/notes/bug-1876317-1db97d1b12a3e4b4.yaml
+releasenotes/notes/bug-1998366-27cd486b46fb56b0.yaml
 releasenotes/notes/cache-trailing-slash-3663c86cd9754379.yaml
 releasenotes/notes/cleanup-session-on-delete-1ed6177d4c5c1f83.yaml
 releasenotes/notes/client-side-rate-limiting-dec43fc9b54f5b70.yaml
 releasenotes/notes/collect-timing-85f007f0d86c8b26.yaml
 releasenotes/notes/drop-py-2-7-f90c67a5db0dfeb8.yaml
 releasenotes/notes/drop-python-3-6-and-3-7-c407d5898c5eafec.yaml
 releasenotes/notes/drop-python-3.5-362bb9d47f830353.yaml
@@ -251,14 +254,15 @@
 releasenotes/notes/retry-authenticated-discovery-19c4354ff983f507.yaml
 releasenotes/notes/retry-delay-68d0c0a1dffcf2fd.yaml
 releasenotes/notes/serice-type-aliases-249454829c57f39a.yaml
 releasenotes/notes/status-code-retries-75052a43efa4edb2.yaml
 releasenotes/notes/support-api-wg-discovery-2cb4b0186619e124.yaml
 releasenotes/notes/user-agent-generation-b069100508c06177.yaml
 releasenotes/notes/version-between-b4b0bcf4cecfb9e4.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
@@ -267,9 +271,10 @@
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/ussuri.rst
 releasenotes/source/victoria.rst
 releasenotes/source/wallaby.rst
 releasenotes/source/xena.rst
 releasenotes/source/yoga.rst
+releasenotes/source/zed.rst
 releasenotes/source/_static/.placeholder
 releasenotes/source/_templates/.placeholder
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1.egg-info/entry_points.txt` & `keystoneauth1-5.2.0/keystoneauth1.egg-info/entry_points.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 v3adfspassword = keystoneauth1.extras._saml2._loading:ADFSPassword
 v3applicationcredential = keystoneauth1.loading._plugins.identity.v3:ApplicationCredential
 v3fedkerb = keystoneauth1.extras.kerberos._loading:MappedKerberos
 v3kerberos = keystoneauth1.extras.kerberos._loading:Kerberos
 v3multifactor = keystoneauth1.loading._plugins.identity.v3:MultiFactor
 v3oauth1 = keystoneauth1.extras.oauth1._loading:V3OAuth1
 v3oauth2clientcredential = keystoneauth1.loading._plugins.identity.v3:OAuth2ClientCredential
+v3oauth2mtlsclientcredential = keystoneauth1.loading._plugins.identity.v3:OAuth2mTlsClientCredential
 v3oidcaccesstoken = keystoneauth1.loading._plugins.identity.v3:OpenIDConnectAccessToken
 v3oidcauthcode = keystoneauth1.loading._plugins.identity.v3:OpenIDConnectAuthorizationCode
 v3oidcclientcredentials = keystoneauth1.loading._plugins.identity.v3:OpenIDConnectClientCredentials
+v3oidcdeviceauthz = keystoneauth1.loading._plugins.identity.v3:OpenIDConnectDeviceAuthorization
 v3oidcpassword = keystoneauth1.loading._plugins.identity.v3:OpenIDConnectPassword
 v3password = keystoneauth1.loading._plugins.identity.v3:Password
 v3samlpassword = keystoneauth1.extras._saml2._loading:Saml2Password
 v3token = keystoneauth1.loading._plugins.identity.v3:Token
 v3tokenlessauth = keystoneauth1.loading._plugins.identity.v3:TokenlessAuth
 v3totp = keystoneauth1.loading._plugins.identity.v3:TOTP
```

### Comparing `keystoneauth1-5.1.2/keystoneauth1.egg-info/requires.txt` & `keystoneauth1-5.2.0/keystoneauth1.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 iso8601>=0.1.11
 os-service-types>=1.2.0
 pbr!=2.1.0,>=2.0.0
 requests>=2.14.2
-six>=1.10.0
 stevedore>=1.20.0
 
 [betamax]
 betamax>=0.7.0
 fixtures>=3.0.0
 mock>=2.0.0
```

### Comparing `keystoneauth1-5.1.2/releasenotes/notes/add-totp-auth-plugin-0650d220899c25b7.yaml` & `keystoneauth1-5.2.0/releasenotes/notes/add-totp-auth-plugin-0650d220899c25b7.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/releasenotes/notes/bp-oauth2-client-credentials-ext-06271700d4f33a7e.yaml` & `keystoneauth1-5.2.0/releasenotes/notes/bp-oauth2-client-credentials-ext-06271700d4f33a7e.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/releasenotes/notes/bug-1840235-ef2946d149ac329c.yaml` & `keystoneauth1-5.2.0/releasenotes/notes/bug-1840235-ef2946d149ac329c.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/releasenotes/notes/retry-authenticated-discovery-19c4354ff983f507.yaml` & `keystoneauth1-5.2.0/releasenotes/notes/retry-authenticated-discovery-19c4354ff983f507.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/releasenotes/notes/user-agent-generation-b069100508c06177.yaml` & `keystoneauth1-5.2.0/releasenotes/notes/user-agent-generation-b069100508c06177.yaml`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/releasenotes/source/conf.py` & `keystoneauth1-5.2.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/requirements.txt` & `keystoneauth1-5.2.0/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 # Requirements lower bounds listed here are our best effort to keep them up to
 # date but we do not test them so no guarantee of having them all correct. If
 # you find any incorrect lower bounds, let us know or propose a fix.
 
-# The order of packages is significant, because pip processes them in the order
-# of appearance. Changing the order has an impact on the overall integration
-# process, which may cause wedges in the gate later.
-
 # All additions to this file must have significant justification.
 
 # NOTE(morgan) At no time may any oslo library be added to the keystoneauth
 # requirements. The requirements for keystoneauth are very tightly controlled
 # to ensure we are not pulling in a ton of transient dependencies. This is
 # important from the standpoint of ensuring keystoneauth can be used outside
 # of openstack-specific projects (allowing interaction with openstack APIs)
 # where oslo and associated transient dependencies are not desired.
 
 pbr!=2.1.0,>=2.0.0 # Apache-2.0
 iso8601>=0.1.11 # MIT
 requests>=2.14.2 # Apache-2.0
-six>=1.10.0 # MIT
 stevedore>=1.20.0 # Apache-2.0
 os-service-types>=1.2.0  # Apache-2.0
```

### Comparing `keystoneauth1-5.1.2/setup.cfg` & `keystoneauth1-5.2.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = keystoneauth1
 summary = Authentication Library for OpenStack Identity
 description_file = 
 	README.rst
 author = OpenStack
 author_email = openstack-discuss@lists.openstack.org
 home_page = https://docs.openstack.org/keystoneauth/latest/
-python_equires = >=3.8
+python_requires = >=3.8
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
@@ -45,24 +45,26 @@
 	admin_token = keystoneauth1.loading._plugins.admin_token:AdminToken
 	v2password = keystoneauth1.loading._plugins.identity.v2:Password
 	v2token = keystoneauth1.loading._plugins.identity.v2:Token
 	v3password = keystoneauth1.loading._plugins.identity.v3:Password
 	v3token = keystoneauth1.loading._plugins.identity.v3:Token
 	v3oidcclientcredentials = keystoneauth1.loading._plugins.identity.v3:OpenIDConnectClientCredentials
 	v3oidcpassword = keystoneauth1.loading._plugins.identity.v3:OpenIDConnectPassword
+	v3oidcdeviceauthz = keystoneauth1.loading._plugins.identity.v3:OpenIDConnectDeviceAuthorization
 	v3oidcauthcode = keystoneauth1.loading._plugins.identity.v3:OpenIDConnectAuthorizationCode
 	v3oidcaccesstoken = keystoneauth1.loading._plugins.identity.v3:OpenIDConnectAccessToken
 	v3oauth1 = keystoneauth1.extras.oauth1._loading:V3OAuth1
 	v3kerberos = keystoneauth1.extras.kerberos._loading:Kerberos
 	v3totp = keystoneauth1.loading._plugins.identity.v3:TOTP
 	v3fedkerb = keystoneauth1.extras.kerberos._loading:MappedKerberos
 	v3tokenlessauth = keystoneauth1.loading._plugins.identity.v3:TokenlessAuth
 	v3adfspassword = keystoneauth1.extras._saml2._loading:ADFSPassword
 	v3samlpassword = keystoneauth1.extras._saml2._loading:Saml2Password
 	v3applicationcredential = keystoneauth1.loading._plugins.identity.v3:ApplicationCredential
 	v3multifactor = keystoneauth1.loading._plugins.identity.v3:MultiFactor
 	v3oauth2clientcredential = keystoneauth1.loading._plugins.identity.v3:OAuth2ClientCredential
+	v3oauth2mtlsclientcredential = keystoneauth1.loading._plugins.identity.v3:OAuth2mTlsClientCredential
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `keystoneauth1-5.1.2/setup.py` & `keystoneauth1-5.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/test-requirements.txt` & `keystoneauth1-5.2.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `keystoneauth1-5.1.2/tox.ini` & `keystoneauth1-5.2.0/tox.ini`

 * *Files identical despite different names*

