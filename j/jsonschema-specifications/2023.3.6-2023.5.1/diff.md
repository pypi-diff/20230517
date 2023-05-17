# Comparing `tmp/jsonschema_specifications-2023.3.6.tar.gz` & `tmp/jsonschema_specifications-2023.5.1.tar.gz`

## Comparing `jsonschema_specifications-2023.3.6.tar` & `jsonschema_specifications-2023.5.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/.coveragerc
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/.flake8
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/.readthedocs.yml
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/.github/FUNDING.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/.github/dependabot.yml
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/docs/Makefile
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/docs/api.rst
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/docs/conf.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/docs/index.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/docs/requirements.in
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/docs/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/__init__.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/_core.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft201909/metaschema.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft201909/vocabularies/applicator
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft201909/vocabularies/content
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft201909/vocabularies/core
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft201909/vocabularies/meta-data
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft201909/vocabularies/validation
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/metaschema.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/applicator
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/content
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/core
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/format
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/format-annotation
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/format-assertion
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/meta-data
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/unevaluated
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/validation
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft3/metaschema.json
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft4/metaschema.json
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft6/metaschema.json
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft7/metaschema.json
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/jsonschema_specifications/tests/test_jsonschema_specifications.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/COPYING
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/README.rst
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/pyproject.toml
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.3.6/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.coveragerc
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.flake8
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.readthedocs.yml
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.github/release.yml
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/Makefile
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/api.rst
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/conf.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/index.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/requirements.in
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/__init__.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/_core.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/metaschema.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/applicator
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/content
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/core
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/meta-data
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/validation
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/metaschema.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/applicator
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/content
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/core
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/format
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/format-annotation
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/format-assertion
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/meta-data
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/unevaluated
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/validation
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft3/metaschema.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft4/metaschema.json
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft6/metaschema.json
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft7/metaschema.json
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/tests/test_jsonschema_specifications.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/COPYING
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/README.rst
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/PKG-INFO
```

### Comparing `jsonschema_specifications-2023.3.6/.pre-commit-config.yaml` & `jsonschema_specifications-2023.5.1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -23,20 +23,20 @@
     hooks:
       - id: flake8
   - repo: https://github.com/asottile/yesqa
     rev: v1.4.0
     hooks:
       - id: yesqa
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.3.2
     hooks:
       - id: pyupgrade
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - name: black
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.6"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
```

### Comparing `jsonschema_specifications-2023.3.6/noxfile.py` & `jsonschema_specifications-2023.5.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/.github/SECURITY.md` & `jsonschema_specifications-2023.5.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/.github/workflows/ci.yml` & `jsonschema_specifications-2023.5.1/.github/workflows/ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -8,34 +8,33 @@
   schedule:
     # Daily at 6:43
     - cron: "43 6 * * *"
 
 env:
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_NO_PYTHON_VERSION_WARNING: "1"
-  PYTHON_LATEST: "3.11"
 
 jobs:
   pre-commit:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: ${{ env.PYTHON_LATEST }}
+          python-version: "3.x"
       - uses: pre-commit/action@v3.0.0
 
   list:
     runs-on: ubuntu-latest
     outputs:
       noxenvs: ${{ steps.noxenvs-matrix.outputs.noxenvs }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
       - id: noxenvs-matrix
         run: |
           echo >>$GITHUB_OUTPUT noxenvs=$(
             nox --list-sessions |
             grep '^* ' |
             cut -d ' ' -f 2- |
             jq --raw-input --slurp 'split("\n") | map(select(. != ""))'
@@ -52,54 +51,50 @@
 
     steps:
       - uses: actions/checkout@v3
       - name: Install dependencies
         run: >
           sudo apt-get update &&
           sudo apt-get install -y libenchant-2-dev
-        if: runner.os == 'Linux'
+        if: runner.os == 'Linux' && startsWith(matrix.noxenv, 'docs')
       - name: Install dependencies
         run: brew install enchant
-        if: runner.os == 'macOS'
+        if: runner.os == 'macOS' && startsWith(matrix.noxenv, 'docs')
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ env.PYTHON_LATEST }}
+          python-version: "3.x"
       - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
       - name: Run nox
         run: nox -s "${{ matrix.noxenv }}"
 
   packaging:
     needs: ci
     runs-on: ubuntu-latest
+    environment:
+      name: PyPI
+      url: https://pypi.org/p/jsonschema-specifications
+    permissions:
+      contents: write
+      id-token: write
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ env.PYTHON_LATEST }}
+          python-version: "3.x"
       - name: Install dependencies
         run: python -m pip install build
       - name: Create packages
         run: python -m build .
-      - uses: actions/upload-artifact@v3
-        with:
-          name: dist
-          path: dist
-      - name: Publish the package
+      - name: Publish to PyPI
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.pypi_password }}
       - name: Create a Release
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
-        uses: actions/github-script@v6
+        uses: softprops/action-gh-release@v1
         with:
-          github-token: ${{ secrets.GITHUB_TOKEN }}
-
-          script: |
-            await github.request(`POST /repos/${{ github.repository }}/releases`, {
-              tag_name: "${{ github.ref }}",
-              generate_release_notes: true
-            });
+          files: |
+            dist/*
+          generate_release_notes: true
```

### Comparing `jsonschema_specifications-2023.3.6/docs/Makefile` & `jsonschema_specifications-2023.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/docs/conf.py` & `jsonschema_specifications-2023.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/docs/index.rst` & `jsonschema_specifications-2023.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/docs/requirements.txt` & `jsonschema_specifications-2023.5.1/docs/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --resolver=backtracking docs/requirements.in
 #
 alabaster==0.7.13
     # via sphinx
-attrs==22.2.0
+attrs==23.1.0
     # via referencing
 babel==2.12.1
     # via sphinx
-beautifulsoup4==4.12.0
+beautifulsoup4==4.12.2
     # via furo
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 contourpy==1.0.7
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 docutils==0.19
     # via sphinx
-fonttools==4.39.2
+fonttools==4.39.4
     # via matplotlib
-furo==2022.12.7
+furo==2023.3.27
     # via -r docs/requirements.in
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.2
     # via sphinx
@@ -36,60 +36,60 @@
     # via -r docs/requirements.in
 kiwisolver==1.4.4
     # via matplotlib
 markupsafe==2.1.2
     # via jinja2
 matplotlib==3.7.1
     # via sphinxext-opengraph
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   contourpy
     #   matplotlib
-packaging==23.0
+packaging==23.1
     # via
     #   matplotlib
     #   sphinx
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pyenchant==3.2.2
     # via sphinxcontrib-spelling
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   furo
     #   pygments-github-lexers
     #   sphinx
 pygments-github-lexers==0.0.5
     # via -r docs/requirements.in
 pyparsing==3.0.9
     # via matplotlib
 python-dateutil==2.8.2
     # via matplotlib
-referencing==0.25.0
+referencing==0.28.1
     # via jsonschema-specifications
-requests==2.28.2
+requests==2.30.0
     # via sphinx
-rpds-py==0.7.0
+rpds-py==0.7.1
     # via referencing
 six==1.16.0
     # via python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
-soupsieve==2.4
+soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==6.1.3
+sphinx==6.2.1
     # via
     #   -r docs/requirements.in
     #   furo
     #   sphinx-basic-ng
     #   sphinx-copybutton
     #   sphinxcontrib-spelling
     #   sphinxext-opengraph
 sphinx-basic-ng==1.0.0b1
     # via furo
-sphinx-copybutton==0.5.1
+sphinx-copybutton==0.5.2
     # via -r docs/requirements.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
@@ -97,11 +97,11 @@
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via -r docs/requirements.in
-sphinxext-opengraph==0.8.1
+sphinxext-opengraph==0.8.2
     # via -r docs/requirements.in
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
```

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/_core.py` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/_core.py`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft201909/metaschema.json` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft201909/vocabularies/applicator` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/applicator`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft201909/vocabularies/content` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/content`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft201909/vocabularies/core` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/core`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft201909/vocabularies/meta-data` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/meta-data`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft201909/vocabularies/validation` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/validation`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/metaschema.json` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/applicator` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/applicator`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/content` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/content`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/core` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/core`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/meta-data` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/meta-data`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft202012/vocabularies/validation` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/validation`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft3/metaschema.json` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft3/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft4/metaschema.json` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft4/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft6/metaschema.json` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft6/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/jsonschema_specifications/schemas/draft7/metaschema.json` & `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft7/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/COPYING` & `jsonschema_specifications-2023.5.1/COPYING`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/README.rst` & `jsonschema_specifications-2023.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.3.6/pyproject.toml` & `jsonschema_specifications-2023.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,56 +7,64 @@
 
 [project]
 name = "jsonschema-specifications"
 description = "The JSON Schema meta-schemas and vocabularies, exposed as a Registry"
 readme = "README.rst"
 license = {text = "MIT"}
 requires-python = ">=3.8"
-keywords = ["jsonschema", "json", "data", "validation"]
+keywords = [
+    "validation",
+    "data validation",
+    "jsonschema",
+    "json",
+    "json schema",
+]
 authors = [
   {email = "Julian+jsonschema-specifications@GrayVines.com"},
   {name = "Julian Berman"},
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
+  "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
-  "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
+  "Topic :: File Formats :: JSON :: JSON Schema",
 ]
 dynamic = ["version"]
 
 dependencies = [
-  "referencing>=0.25.0",
+  "referencing>=0.28.0",
   "importlib_resources>=1.4.0;python_version<'3.9'",
 ]
 
 [project.urls]
 Documentation = "https://jsonschema-specifications.readthedocs.io/"
 Homepage = "https://github.com/python-jsonschema/jsonschema-specifications"
 Issues = "https://github.com/python-jsonschema/jsonschema-specifications/issues/"
 Funding = "https://github.com/sponsors/Julian"
 Source = "https://github.com/python-jsonschema/jsonschema-specifications"
 
 [tool.coverage.run]
 branch = true
-source = ["referencing"]
+source = ["jsonschema-specifications"]
 dynamic_context = "test_function"
 
 [tool.coverage.report]
 fail_under = 100
 
 [tool.doc8]
 ignore = [
     "D001",  # one sentence per line, so max length doesn't make sense
 ]
 
 [tool.isort]
 combine_as_imports = true
+ensure_newline_before_comments = true
 from_first = true
 include_trailing_comma = true
 multi_line_output = 3
```

### Comparing `jsonschema_specifications-2023.3.6/PKG-INFO` & `jsonschema_specifications-2023.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: jsonschema-specifications
-Version: 2023.3.6
+Version: 2023.5.1
 Summary: The JSON Schema meta-schemas and vocabularies, exposed as a Registry
 Project-URL: Documentation, https://jsonschema-specifications.readthedocs.io/
 Project-URL: Homepage, https://github.com/python-jsonschema/jsonschema-specifications
 Project-URL: Issues, https://github.com/python-jsonschema/jsonschema-specifications/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/python-jsonschema/jsonschema-specifications
 Author: Julian Berman
 Author-email: Julian+jsonschema-specifications@GrayVines.com
 License: MIT
 License-File: COPYING
-Keywords: data,json,jsonschema,validation
+Keywords: data validation,json,json schema,jsonschema,validation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: File Formats :: JSON :: JSON Schema
 Requires-Python: >=3.8
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
-Requires-Dist: referencing>=0.25.0
+Requires-Dist: referencing>=0.28.0
 Description-Content-Type: text/x-rst
 
 =============================
 ``jsonschema-specifications``
 =============================
 
 |PyPI| |Pythons| |CI| |ReadTheDocs|
```

