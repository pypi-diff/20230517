# Comparing `tmp/gpt_review-0.9.2rc796.post1.tar.gz` & `tmp/gpt_review-0.9.2rc812.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_review-0.9.2rc796.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gpt_review-0.9.2rc812.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gpt_review-0.9.2rc796.post1.tar` & `gpt_review-0.9.2rc812.post1.tar`

### file list

```diff
@@ -1,56 +1,59 @@
--rw-r--r--   0        0        0      336 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1995 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4181 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1776 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1862 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.pypirc
--rw-r--r--   0        0        0      450 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1125 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/LICENSE
--rw-r--r--   0        0        0     3556 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/README.md
--rw-r--r--   0        0        0     2308 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/action.yml
--rw-r--r--   0        0        0      307 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/azure.yaml.template
--rw-r--r--   0        0        0      218 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/config.summary.template.yml
--rw-r--r--   0        0        0      362 2023-05-16 16:42:22.656174 gpt_review-0.9.2rc796.post1/prompt.template.yml
--rw-r--r--   0        0        0     8500 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-16 16:42:33.972341 gpt_review-0.9.2rc796.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      170 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-16 16:42:33.972341 gpt_review-0.9.2rc796.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      170 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0     9453 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     3520 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5998 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     6437 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0     4241 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/_openai.py
--rw-r--r--   0        0        0      788 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     8558 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      955 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0     3227 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/context.py
--rw-r--r--   0        0        0      924 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0       33 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/prompts/__init__.py
--rw-r--r--   0        0        0     1246 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/prompts/_prompt.py
--rw-r--r--   0        0        0      349 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/prompts/prompt_bug.yaml
--rw-r--r--   0        0        0      362 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/prompts/prompt_coverage.yaml
--rw-r--r--   0        0        0      327 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/prompts/prompt_summary.yaml
--rw-r--r--   0        0        0      863 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/src/gpt_review/utils.py
--rw-r--r--   0        0        0      218 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     5573 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/tests/mock.diff
--rw-r--r--   0        0        0      375 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/tests/test_context.py
--rw-r--r--   0        0        0      716 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/tests/test_git.py
--rw-r--r--   0        0        0     1443 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/tests/test_github.py
--rw-r--r--   0        0        0     5427 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      684 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1449 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/tests/test_openai.py
--rw-r--r--   0        0        0     1015 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/tests/test_report.py
--rw-r--r--   0        0        0      797 2023-05-16 16:42:22.660174 gpt_review-0.9.2rc796.post1/tests/test_review.py
--rw-r--r--   0        0        0     5729 1970-01-01 00:00:00.000000 gpt_review-0.9.2rc796.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1977 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4160 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1776 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     2041 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.pypirc
+-rw-r--r--   0        0        0       96 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.vscode/extensions.json
+-rw-r--r--   0        0        0      530 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1125 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      905 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/.vscode/tasks.json
+-rw-r--r--   0        0        0     1070 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/LICENSE
+-rw-r--r--   0        0        0     3556 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/README.md
+-rw-r--r--   0        0        0     2307 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/action.yml
+-rw-r--r--   0        0        0      308 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/azure.yaml.template
+-rw-r--r--   0        0        0      218 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/config.summary.template.yml
+-rw-r--r--   0        0        0      362 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/prompt.template.yml
+-rw-r--r--   0        0        0     8686 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 05:30:19.357215 gpt_review-0.9.2rc812.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-17 05:30:19.357215 gpt_review-0.9.2rc812.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0     9452 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     3520 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     1453 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     6437 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0     4242 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/_openai.py
+-rw-r--r--   0        0        0     8575 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      955 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0     3227 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/context.py
+-rw-r--r--   0        0        0      924 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0       33 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/prompts/__init__.py
+-rw-r--r--   0        0        0     1246 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/prompts/_prompt.py
+-rw-r--r--   0        0        0      349 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/prompts/prompt_bug.yaml
+-rw-r--r--   0        0        0      362 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/prompts/prompt_coverage.yaml
+-rw-r--r--   0        0        0      327 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/prompts/prompt_summary.yaml
+-rw-r--r--   0        0        0        1 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/repositories/__init__.py
+-rw-r--r--   0        0        0      779 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/repositories/_repository.py
+-rw-r--r--   0        0        0     6368 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/repositories/github.py
+-rw-r--r--   0        0        0      863 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/src/gpt_review/utils.py
+-rw-r--r--   0        0        0      218 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     5573 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/tests/mock.diff
+-rw-r--r--   0        0        0      375 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/tests/test_context.py
+-rw-r--r--   0        0        0      716 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1452 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5427 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      684 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1449 2023-05-17 05:30:09.805115 gpt_review-0.9.2rc812.post1/tests/test_openai.py
+-rw-r--r--   0        0        0     1015 2023-05-17 05:30:09.809115 gpt_review-0.9.2rc812.post1/tests/test_report.py
+-rw-r--r--   0        0        0      807 2023-05-17 05:30:09.809115 gpt_review-0.9.2rc812.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5943 1970-01-01 00:00:00.000000 gpt_review-0.9.2rc812.post1/PKG-INFO
```

### Comparing `gpt_review-0.9.2rc796.post1/.devcontainer/devcontainer.json` & `gpt_review-0.9.2rc812.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt_review-0.9.2rc812.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/.github/dependabot.yml` & `gpt_review-0.9.2rc812.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/.github/pull_request_template.md` & `gpt_review-0.9.2rc812.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/.github/workflows/codeql.yml` & `gpt_review-0.9.2rc812.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/.github/workflows/dependency-review.yml` & `gpt_review-0.9.2rc812.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt_review-0.9.2rc812.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   CreateRelease:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout repository
         uses: actions/checkout@v2
         with:
           token: ${{ secrets.PAT }}
-        
+
       - name: Bump version and push tag
         id: tag_version
         uses: mathieudutour/github-tag-action@v6.0
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           dry_run: true
           tag_prefix: 'v'
@@ -46,15 +46,15 @@
 
       - if: steps.tag_version.outputs.release_type
         run: |
           python -m pip install --upgrade pip
           python -m pip install flit
 
           python -m flit build
-          
+
       - if: steps.tag_version.outputs.release_type
         run: |
           gh release delete $TAG || echo "no tag existed"
 
           gh release create \
             -d \
             --target main \
```

### Comparing `gpt_review-0.9.2rc796.post1/.github/workflows/python.yml` & `gpt_review-0.9.2rc812.post1/.github/workflows/python.yml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         tools: ['black', 'bandit', 'pylint', 'flake8']
     steps:
       - uses: actions/checkout@v2
         with:
           ref: ${{ github.event.pull_request.head.sha }}
 
       - name: ${{ matrix.tools }}
-        uses: microsoft/action-python@0.6.3
+        uses: microsoft/action-python@0.6.4
         with:
           ${{ matrix.tools }}: true
           workdir: '.'
           testdir: 'tests'
           python_version: '3.11.3'
 
   tests:
@@ -52,16 +52,16 @@
       - uses: actions/checkout@v2
         with:
           ref: ${{ github.event.pull_request.head.sha }}
       - uses: Azure/login@v1.4.6
         if: ${{ matrix.flags == 'integration' }}
         with:
           creds: ${{ secrets.AZURE_CREDENTIALS }}
-      - name: ${{ matrix.flags }}-${{ matrix.python }}
-        uses: microsoft/action-python@0.6.3
+      - name: ${{ matrix.tools }}
+        uses: microsoft/action-python@0.6.4
         with:
           pytest: true
           args: ${{ matrix.args }}
           workdir: '.'
           testdir: 'tests'
           python_version: ${{ matrix.python }}
           flags: ${{ matrix.flags }}-${{ matrix.python }}
```

### Comparing `gpt_review-0.9.2rc796.post1/.github/workflows/test-action.yml` & `gpt_review-0.9.2rc812.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/.gitignore` & `gpt_review-0.9.2rc812.post1/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -127,7 +127,21 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # Default Directory for llama index files
 storage/
+
+# Azure Functions artifacts
+bin
+obj
+appsettings.json
+local.settings.json
+*.deb
+.venvs
+
+# Azurite artifacts
+__blobstorage__
+__queuestorage__
+__azurite_db*__.json
+.python_packages
```

### Comparing `gpt_review-0.9.2rc796.post1/.vscode/settings.json` & `gpt_review-0.9.2rc812.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/LICENSE` & `gpt_review-0.9.2rc812.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/README.md` & `gpt_review-0.9.2rc812.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/action.yml` & `gpt_review-0.9.2rc812.post1/action.yml`

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,7 @@
           PATCH_REPO: ${{ github.repository }}
           FULL_SUMMARY: true
           FILE_SUMMARY: false
           TEST_SUMMARY: false
           BUG_SUMMARY: false
           RISK_SUMMARY: false
           RISK_BREAKING: false
-
```

### Comparing `gpt_review-0.9.2rc796.post1/pyproject.toml` & `gpt_review-0.9.2rc812.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 requires-python = ">=3.8.1"
 dynamic = ["version"]
 dependencies = [
+  'azure-devops',
+  'azure-functions; python_version <= "3.10"',
   'azure-identity',
   'azure-keyvault-secrets',
   'llama-index>=0.6.0,<=0.6.8',
   'httpx',
   'GitPython',
   'knack',
   'openai',
@@ -35,14 +37,16 @@
   'transformers; python_version <= "3.8"'
 ]
 
 [project.optional-dependencies]
 test = [
     "bandit[toml]==1.7.5",
     "black==23.3.0",
+    "cattrs",
+    "docx2txt",
     "check-manifest==0.49",
     "flake8-bugbear==23.5.9",
     "flake8-docstrings",
     "flake8-formatter_junit_xml",
     "flake8",
     "flake8-pyproject",
     "pre-commit==3.3.1",
@@ -50,15 +54,16 @@
     "pylint_junit",
     "pytest-cov>=3.0.0",
     "pytest-mock",
     "pytest-runner",
     "pytest-xdist",
     "pytest>=7.2.2",
     "pytest-github-actions-annotate-failures",
-    "shellcheck-py==0.9.0.2"
+    "shellcheck-py==0.9.0.2",
+    "requests_mock"
 ]
 
 [project.scripts]
 gpt = "gpt_review.main:__main__"
 
 [project.urls]
 Documentation = "https://github.com/dciborow/action-gpt/tree/main#readme"
@@ -113,14 +118,18 @@
     # Covered by Ruff
     "F401",
     "F501",
     "F821",
     "W391", # Covered by Pylint trailing-newlines
 ]
 
+[tool.isort]
+profile = "black"
+src_paths = ["src", "tests", "azure"]
+
 [tool.pyright]
 include = ["src"]
 exclude = [
     "**/node_modules",
     "**/__pycache__",
 ]
 venv = "env37"
```

### Comparing `gpt_review-0.9.2rc796.post1/src/gpt_review/_ask.py` & `gpt_review-0.9.2rc812.post1/src/gpt_review/_ask.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         repository (Optional[str], optional): The repository to search. Defaults to None.
 
     Returns:
             Dict[str, str]: The response from GPT.
     """
     _load_azure_openai_context()
 
-    prompt = " ".join(question)
+    prompt = "".join(question)
 
     if files or directory or repository:
         response = _query_index(
             prompt,
             files,
             input_dir=directory,
             reset=reset,
```

### Comparing `gpt_review-0.9.2rc796.post1/src/gpt_review/_git.py` & `gpt_review-0.9.2rc812.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/src/gpt_review/_github.py` & `gpt_review-0.9.2rc812.post1/src/gpt_review/repositories/github.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 import requests
 from knack import CLICommandsLoader
 from knack.arguments import ArgumentsContext
 from knack.commands import CommandGroup
 
 from gpt_review._command import GPTCommandGroup
-from gpt_review._repository import _RepositoryClient
 from gpt_review._review import _summarize_files
+from gpt_review.repositories._repository import _RepositoryClient
 
 
-class _GitHubClient(_RepositoryClient):
+class GitHubClient(_RepositoryClient):
     """GitHub client."""
 
     @staticmethod
     def get_pr_diff(patch_repo=None, patch_pr=None, access_token=None) -> str:
         """
         Get the diff of a PR.
 
@@ -100,64 +100,74 @@
                 data=data,
                 timeout=10,
             )
         logging.debug(response.json())
         return response
 
     @staticmethod
-    def post_pr_summary(pr_patch) -> Dict[str, str]:
+    def post_pr_summary(diff) -> Dict[str, str]:
         """
         Get a review of a PR.
 
+        Requires the following environment variables:
+            - LINK: The link to the PR.
+            - GIT_COMMIT_HASH: The git commit hash.
+            - GITHUB_TOKEN: The GitHub access token.
+
         Args:
-            pr_patch (str): The patch of the PR.
+            diff (str): The patch of the PR.
 
         Returns:
             Dict[str, str]: The review.
         """
-        review = _summarize_files(pr_patch)
+        review = _summarize_files(diff)
         logging.debug(review)
 
         link = os.getenv("LINK")
         git_commit_hash = os.getenv("GIT_COMMIT_HASH")
         access_token = os.getenv("GITHUB_TOKEN")
 
         if link and git_commit_hash and access_token:
-            _GitHubClient._post_pr_comment(
+            GitHubClient._post_pr_comment(
                 review=review, git_commit_hash=git_commit_hash, link=link, access_token=access_token
             )
             return {"response": "PR posted"}
 
         logging.warning("No PR to post too")
         return {"response": "No PR to post too"}
 
 
-def _github_review(repository=None, pull_request=None, access_token=None) -> Dict[str, str]:
+def _review(repository=None, pull_request=None, access_token=None) -> Dict[str, str]:
     """Review GitHub PR with Open AI, and post response as a comment.
 
     Args:
         repository (str): The repo of the PR.
         pull_request (str): The PR number.
         access_token (str): The GitHub access token.
 
     Returns:
         Dict[str, str]: The response.
     """
-    diff = _GitHubClient.get_pr_diff(repository, pull_request, access_token)
-    _GitHubClient.post_pr_summary(diff)
+    diff = GitHubClient.get_pr_diff(repository, pull_request, access_token)
+    GitHubClient.post_pr_summary(diff)
     return {"response": "Review posted as a comment."}
 
 
+def _comment(question: str, comment_id: int, diff: str = ".diff", link=None, access_token=None) -> Dict[str, str]:
+    """"""
+    raise NotImplementedError
+
+
 class GitHubCommandGroup(GPTCommandGroup):
     """Ask Command Group."""
 
     @staticmethod
     def load_command_table(loader: CLICommandsLoader) -> None:
-        with CommandGroup(loader, "github", "gpt_review._github#{}") as group:
-            group.command("review", "_github_review", is_preview=True)
+        with CommandGroup(loader, "github", "gpt_review.repositories.github#{}", is_preview=True) as group:
+            group.command("review", "_review", is_preview=True)
 
     @staticmethod
     def load_arguments(loader: CLICommandsLoader) -> None:
         """Add patch_repo, patch_pr, and access_token arguments."""
         with ArgumentsContext(loader, "github") as args:
             args.argument(
                 "access_token",
```

### Comparing `gpt_review-0.9.2rc796.post1/src/gpt_review/_gpt_cli.py` & `gpt_review-0.9.2rc812.post1/src/gpt_review/_gpt_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from collections import OrderedDict
 
 from knack import CLI, CLICommandsLoader
 
 from gpt_review import __version__
 from gpt_review._ask import AskCommandGroup
 from gpt_review._git import GitCommandGroup
-from gpt_review._github import GitHubCommandGroup
 from gpt_review._review import ReviewCommandGroup
+from gpt_review.repositories.github import GitHubCommandGroup
 
 CLI_NAME = "gpt"
 
 
 class GPTCLI(CLI):
     """Custom CLI implemntation to set version for the GPT CLI."""
```

### Comparing `gpt_review-0.9.2rc796.post1/src/gpt_review/_llama_index.py` & `gpt_review-0.9.2rc812.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/src/gpt_review/_openai.py` & `gpt_review-0.9.2rc812.post1/src/gpt_review/_openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Open AI API Call Wrapper."""
-import os
 import logging
+import os
 
 import openai
 from openai.error import RateLimitError
 
 import gpt_review.constants as C
-from gpt_review.utils import _retry_with_exponential_backoff
 from gpt_review.context import _load_azure_openai_context
+from gpt_review.utils import _retry_with_exponential_backoff
 
 
 def _count_tokens(prompt) -> int:
     """
     Determine number of tokens in prompt.
 
     Args:
@@ -80,15 +80,15 @@
         str: The response from GPT.
     """
     messages = messages or [{"role": "user", "content": prompt}]
     logging.debug("Prompt sent to GPT: %s\n", prompt)
 
     try:
         model = _get_model(prompt, max_tokens=max_tokens, fast=fast, large=large)
-        logging.debug(f"Model Selected based on prompt size: {model}")
+        logging.debug("Model Selected based on prompt size: %s", model)
 
         if os.environ["OPENAI_API_TYPE"] == C.AZURE_API_TYPE:
             logging.debug("Using Azure Open AI.")
             completion = openai.ChatCompletion.create(
                 deployment_id=model,
                 messages=messages,
                 max_tokens=max_tokens,
```

### Comparing `gpt_review-0.9.2rc796.post1/src/gpt_review/_review.py` & `gpt_review-0.9.2rc812.post1/src/gpt_review/_review.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 import yaml
 from knack import CLICommandsLoader
 from knack.arguments import ArgumentsContext
 from knack.commands import CommandGroup
 
 from gpt_review._ask import _ask
 from gpt_review._command import GPTCommandGroup
-from gpt_review.prompts._prompt import load_bug_yaml, load_coverage_yaml, load_summary_yaml
+from gpt_review.prompts._prompt import (
+    load_bug_yaml,
+    load_coverage_yaml,
+    load_summary_yaml,
+)
 
 _CHECKS = {
     "SUMMARY_CHECKS": [
         {
             "flag": "SUMMARY_SUGGEST",
             "header": "Suggestions",
             "goal": "Any suggestions for improving the changes in this PR?",
```

### Comparing `gpt_review-0.9.2rc796.post1/src/gpt_review/constants.py` & `gpt_review-0.9.2rc812.post1/src/gpt_review/constants.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/src/gpt_review/context.py` & `gpt_review-0.9.2rc812.post1/src/gpt_review/context.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/src/gpt_review/main.py` & `gpt_review-0.9.2rc812.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/src/gpt_review/prompts/_prompt.py` & `gpt_review-0.9.2rc812.post1/src/gpt_review/prompts/_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/src/gpt_review/utils.py` & `gpt_review-0.9.2rc812.post1/src/gpt_review/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/tests/conftest.py` & `gpt_review-0.9.2rc812.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/tests/mock.diff` & `gpt_review-0.9.2rc812.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/tests/test_git.py` & `gpt_review-0.9.2rc812.post1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/tests/test_github.py` & `gpt_review-0.9.2rc812.post1/tests/test_github.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pytest
 
-from gpt_review._github import _GitHubClient
+from gpt_review.repositories.github import GitHubClient
 
 
 def get_pr_diff_test(starts_with, patch_repo=None, patch_pr=None) -> None:
     """Test the GitHub API call."""
-    diff = _GitHubClient.get_pr_diff(patch_repo=patch_repo, patch_pr=patch_pr)
+    diff = GitHubClient.get_pr_diff(patch_repo=patch_repo, patch_pr=patch_pr)
     assert diff.startswith(starts_with)
 
 
 def post_pr_comment_test() -> None:
     """Test the GitHub API call."""
-    response = _GitHubClient.post_pr_summary("test")
+    response = GitHubClient.post_pr_summary("test")
     assert response
 
 
 @pytest.mark.integration
 def test_int_pr_diff(mock_github) -> None:
     """Integration Test for GitHub API diff call."""
     get_pr_diff_test("diff --git a/README.md b/README.md", "microsoft/gpt-review", 1)
```

### Comparing `gpt_review-0.9.2rc796.post1/tests/test_gpt_cli.py` & `gpt_review-0.9.2rc812.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/tests/test_llama_index.py` & `gpt_review-0.9.2rc812.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/tests/test_openai.py` & `gpt_review-0.9.2rc812.post1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/tests/test_report.py` & `gpt_review-0.9.2rc812.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.2rc796.post1/tests/test_review.py` & `gpt_review-0.9.2rc812.post1/tests/test_review.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from gpt_review._github import _GitHubClient
+from gpt_review.repositories.github import GitHubClient
 
 
 def test_get_review(mock_openai) -> None:
     get_review_test()
 
 
 @pytest.mark.integration
@@ -14,15 +14,15 @@
 
 def get_review_test() -> None:
     """Test get_review."""
     # Load test data from moock.diff
     with open("tests/mock.diff", "r") as f:
         diff = f.read()
 
-        _GitHubClient.post_pr_summary(diff)
+        GitHubClient.post_pr_summary(diff)
 
 
 def test_empty_summary(empty_summary, mock_openai) -> None:
     get_review_test()
 
 
 @pytest.mark.integration
```

### Comparing `gpt_review-0.9.2rc796.post1/PKG-INFO` & `gpt_review-0.9.2rc812.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.9.2rc796.post1
+Version: 0.9.2rc812.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: azure-devops
+Requires-Dist: azure-functions; python_version <= "3.10"
 Requires-Dist: azure-identity
 Requires-Dist: azure-keyvault-secrets
 Requires-Dist: llama-index>=0.6.0,<=0.6.8
 Requires-Dist: httpx
 Requires-Dist: GitPython
 Requires-Dist: knack
 Requires-Dist: openai
 Requires-Dist: requests
 Requires-Dist: pyyaml
 Requires-Dist: typing_extensions; python_version <= "3.10"
 Requires-Dist: transformers; python_version <= "3.8"
 Requires-Dist: bandit[toml]==1.7.5 ; extra == "test"
 Requires-Dist: black==23.3.0 ; extra == "test"
+Requires-Dist: cattrs ; extra == "test"
+Requires-Dist: docx2txt ; extra == "test"
 Requires-Dist: check-manifest==0.49 ; extra == "test"
 Requires-Dist: flake8-bugbear==23.5.9 ; extra == "test"
 Requires-Dist: flake8-docstrings ; extra == "test"
 Requires-Dist: flake8-formatter_junit_xml ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
 Requires-Dist: flake8-pyproject ; extra == "test"
 Requires-Dist: pre-commit==3.3.1 ; extra == "test"
@@ -38,14 +42,15 @@
 Requires-Dist: pytest-cov>=3.0.0 ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
 Requires-Dist: pytest-runner ; extra == "test"
 Requires-Dist: pytest-xdist ; extra == "test"
 Requires-Dist: pytest>=7.2.2 ; extra == "test"
 Requires-Dist: pytest-github-actions-annotate-failures ; extra == "test"
 Requires-Dist: shellcheck-py==0.9.0.2 ; extra == "test"
+Requires-Dist: requests_mock ; extra == "test"
 Project-URL: Documentation, https://github.com/dciborow/action-gpt/tree/main#readme
 Project-URL: Source, https://github.com/dciborow/action-gpt
 Project-URL: Tracker, https://github.com/dciborow/action-gpt/issues
 Provides-Extra: test
 
 # gpt-review
```

#### html2text {}

```diff
@@ -1,34 +1,37 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.9.2rc796.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.9.2rc812.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: azure-identity Requires-Dist: azure-keyvault-
-secrets Requires-Dist: llama-index>=0.6.0,<=0.6.8 Requires-Dist: httpx
+Python :: 3.11 Requires-Dist: azure-devops Requires-Dist: azure-functions;
+python_version <= "3.10" Requires-Dist: azure-identity Requires-Dist: azure-
+keyvault-secrets Requires-Dist: llama-index>=0.6.0,<=0.6.8 Requires-Dist: httpx
 Requires-Dist: GitPython Requires-Dist: knack Requires-Dist: openai Requires-
 Dist: requests Requires-Dist: pyyaml Requires-Dist: typing_extensions;
 python_version <= "3.10" Requires-Dist: transformers; python_version <= "3.8"
 Requires-Dist: bandit[toml]==1.7.5 ; extra == "test" Requires-Dist:
-black==23.3.0 ; extra == "test" Requires-Dist: check-manifest==0.49 ; extra ==
-"test" Requires-Dist: flake8-bugbear==23.5.9 ; extra == "test" Requires-Dist:
-flake8-docstrings ; extra == "test" Requires-Dist: flake8-formatter_junit_xml ;
-extra == "test" Requires-Dist: flake8 ; extra == "test" Requires-Dist: flake8-
-pyproject ; extra == "test" Requires-Dist: pre-commit==3.3.1 ; extra == "test"
-Requires-Dist: pylint==2.17.4 ; extra == "test" Requires-Dist: pylint_junit ;
-extra == "test" Requires-Dist: pytest-cov>=3.0.0 ; extra == "test" Requires-
-Dist: pytest-mock ; extra == "test" Requires-Dist: pytest-runner ; extra ==
-"test" Requires-Dist: pytest-xdist ; extra == "test" Requires-Dist:
-pytest>=7.2.2 ; extra == "test" Requires-Dist: pytest-github-actions-annotate-
-failures ; extra == "test" Requires-Dist: shellcheck-py==0.9.0.2 ; extra ==
-"test" Project-URL: Documentation, https://github.com/dciborow/action-gpt/tree/
+black==23.3.0 ; extra == "test" Requires-Dist: cattrs ; extra == "test"
+Requires-Dist: docx2txt ; extra == "test" Requires-Dist: check-manifest==0.49 ;
+extra == "test" Requires-Dist: flake8-bugbear==23.5.9 ; extra == "test"
+Requires-Dist: flake8-docstrings ; extra == "test" Requires-Dist: flake8-
+formatter_junit_xml ; extra == "test" Requires-Dist: flake8 ; extra == "test"
+Requires-Dist: flake8-pyproject ; extra == "test" Requires-Dist: pre-
+commit==3.3.1 ; extra == "test" Requires-Dist: pylint==2.17.4 ; extra == "test"
+Requires-Dist: pylint_junit ; extra == "test" Requires-Dist: pytest-cov>=3.0.0
+; extra == "test" Requires-Dist: pytest-mock ; extra == "test" Requires-Dist:
+pytest-runner ; extra == "test" Requires-Dist: pytest-xdist ; extra == "test"
+Requires-Dist: pytest>=7.2.2 ; extra == "test" Requires-Dist: pytest-github-
+actions-annotate-failures ; extra == "test" Requires-Dist: shellcheck-
+py==0.9.0.2 ; extra == "test" Requires-Dist: requests_mock ; extra == "test"
+Project-URL: Documentation, https://github.com/dciborow/action-gpt/tree/
 main#readme Project-URL: Source, https://github.com/dciborow/action-gpt
 Project-URL: Tracker, https://github.com/dciborow/action-gpt/issues Provides-
 Extra: test # gpt-review
   [Actions_Status] [Coverage_Status] [License:_MIT] [PyPI] [Downloads] [Code
                                  style:_black]
 A Python based CLI and GitHub Action to use Open AI or Azure Open AI models to
 review contents of pull requests. ## How to install CLI First, install the
```

