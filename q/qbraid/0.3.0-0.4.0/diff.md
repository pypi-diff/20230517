# Comparing `tmp/qbraid-0.3.0.tar.gz` & `tmp/qbraid-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-0.3.0.tar", last modified: Thu May 11 19:29:31 2023, max compression
+gzip compressed data, was "qbraid-0.4.0.tar", last modified: Tue May 16 22:30:19 2023, max compression
```

## Comparing `qbraid-0.3.0.tar` & `qbraid-0.4.0.tar`

### file list

```diff
@@ -1,261 +1,272 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.483199 qbraid-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 19:29:20.000000 qbraid-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 19:29:20.000000 qbraid-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-05-11 19:29:31.483199 qbraid-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-05-11 19:29:20.000000 qbraid-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.447199 qbraid-0.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.447199 qbraid-0.3.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.447199 qbraid-0.3.0/docs/_static/account/
--rw-r--r--   0 runner    (1001) docker     (123)    80371 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/account/account_access_key.png
--rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/account/account_profile_details.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.447199 qbraid-0.3.0/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.455199 qbraid-0.3.0/docs/_static/environments/
--rw-r--r--   0 runner    (1001) docker     (123)   358114 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/environments/env_add.png
--rw-r--r--   0 runner    (1001) docker     (123)   236606 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/environments/env_add_package.png
--rw-r--r--   0 runner    (1001) docker     (123)   112288 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/environments/env_create.png
--rw-r--r--   0 runner    (1001) docker     (123)    41898 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/environments/env_custom_installing.png
--rw-r--r--   0 runner    (1001) docker     (123)    40671 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/environments/env_custom_pkgs.png
--rw-r--r--   0 runner    (1001) docker     (123)   497786 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/environments/env_install.png
--rw-r--r--   0 runner    (1001) docker     (123)   450900 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/environments/env_installing.png
--rw-r--r--   0 runner    (1001) docker     (123)   394044 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/environments/env_more.png
--rw-r--r--   0 runner    (1001) docker     (123)   545265 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/environments/env_new.png
--rw-r--r--   0 runner    (1001) docker     (123)   148896 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/environments/env_pkg_install.png
--rw-r--r--   0 runner    (1001) docker     (123)    47510 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/environments/env_share.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.455199 qbraid-0.3.0/docs/_static/errors/
--rw-r--r--   0 runner    (1001) docker     (123)   108308 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/errors/sidebar_glitch.png
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.455199 qbraid-0.3.0/docs/_static/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/integrations/0_file_control_panel.png
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/integrations/1_top_bar_token.png
--rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/integrations/2_request_token.png
--rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/integrations/3_copy_token.png
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/integrations/4_jupyter_server.png
--rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/integrations/5_existing_uri.png
--rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/integrations/6_example_user.png
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/integrations/7_notebook_kernel.png
--rw-r--r--   0 runner    (1001) docker     (123)    34868 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/integrations/8_select_kernel.png
--rw-r--r--   0 runner    (1001) docker     (123)    85020 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/integrations/os.png
--rw-r--r--   0 runner    (1001) docker     (123)    34944 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/integrations/vscode_graphic.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.459199 qbraid-0.3.0/docs/_static/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)   411673 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/jobs/jobs_ionq.png
--rw-r--r--   0 runner    (1001) docker     (123)   592257 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/jobs/jobs_sdk.png
--rw-r--r--   0 runner    (1001) docker     (123)    85873 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/jobs/jobs_tag.png
--rw-r--r--   0 runner    (1001) docker     (123)   154811 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.459199 qbraid-0.3.0/docs/_static/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/notebooks/file_browser.png
--rw-r--r--   0 runner    (1001) docker     (123)   451731 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/notebooks/kernel_activate.png
--rw-r--r--   0 runner    (1001) docker     (123)   510341 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/notebooks/kernel_deactivate.png
--rw-r--r--   0 runner    (1001) docker     (123)   290430 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/notebooks/kernel_nb.png
--rw-r--r--   0 runner    (1001) docker     (123)   346617 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/notebooks/kernel_switch.png
--rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/notebooks/share_notebook.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.463199 qbraid-0.3.0/docs/_static/pkg-logos/
--rw-r--r--   0 runner    (1001) docker     (123)    36600 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/pkg-logos/braket.png
--rw-r--r--   0 runner    (1001) docker     (123)    53519 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/pkg-logos/cirq.png
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/pkg-logos/pyquil.png
--rw-r--r--   0 runner    (1001) docker     (123)    28492 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/pkg-logos/pytket.png
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/pkg-logos/qiskit.png
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/pkg-logos/xanadu.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.463199 qbraid-0.3.0/docs/_static/sdk-files/
--rw-r--r--   0 runner    (1001) docker     (123)   447304 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/sdk-files/get_devices.png
--rw-r--r--   0 runner    (1001) docker     (123)    53194 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/_static/sdk-files/plot_counts.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.463199 qbraid-0.3.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/api/qbraid.api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/api/qbraid.devices.aws.rst
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/api/qbraid.devices.ibm.rst
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/api/qbraid.devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/api/qbraid.interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/api/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/api/qbraid.transpiler.cirq_braket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/api/qbraid.transpiler.cirq_pyquil.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/api/qbraid.transpiler.cirq_pytket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/api/qbraid.transpiler.cirq_qiskit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/api/qbraid.transpiler.cirq_utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/api/qbraid.transpiler.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.467199 qbraid-0.3.0/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/cli/envs-activate.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/cli/envs-list.rst
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/cli/envs-uninstall.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/cli/envs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/cli/jobs-add.rst
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/cli/jobs-disable.rst
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/cli/jobs-enable.rst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/cli/jobs-get-credits.rst
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/cli/jobs-list.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/cli/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/cli/kernels.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/cli/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.467199 qbraid-0.3.0/docs/lab/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/lab/account.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/lab/environments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/lab/files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/lab/integrations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/lab/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/lab/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/lab/quantumjobs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/lab/system.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/lab/troubleshoot.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.471199 qbraid-0.3.0/docs/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/sdk/circuits.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/sdk/devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/sdk/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/sdk/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-11 19:29:20.000000 qbraid-0.3.0/docs/sdk/results.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-11 19:29:20.000000 qbraid-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.471199 qbraid-0.3.0/qbraid/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/_qprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.471199 qbraid-0.3.0/qbraid/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/api/job_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/api/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/api/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.471199 qbraid-0.3.0/qbraid/api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/api/tests/test_api_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/api/tests/test_api_thirdparty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.471199 qbraid-0.3.0/qbraid/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.475199 qbraid-0.3.0/qbraid/devices/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/aws/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/aws/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/aws/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.475199 qbraid-0.3.0/qbraid/devices/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/ibm/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/ibm/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/ibm/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/ibm/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.475199 qbraid-0.3.0/qbraid/devices/ibm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/ibm/tests/test_ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/status_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.475199 qbraid-0.3.0/qbraid/devices/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/devices/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/display_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/get_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.475199 qbraid-0.3.0/qbraid/interface/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/calculate_unitary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/convert_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/draw_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/programs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.475199 qbraid-0.3.0/qbraid/interface/qbraid_braket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_braket/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_braket/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.475199 qbraid-0.3.0/qbraid/interface/qbraid_cirq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_cirq/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_cirq/circuits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.475199 qbraid-0.3.0/qbraid/interface/qbraid_cirq/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_cirq/tests/test_cirq_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_cirq/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.475199 qbraid-0.3.0/qbraid/interface/qbraid_pyquil/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_pyquil/programs.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_pyquil/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.479200 qbraid-0.3.0/qbraid/interface/qbraid_pytket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_pytket/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_pytket/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.479200 qbraid-0.3.0/qbraid/interface/qbraid_qiskit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_qiskit/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/qbraid_qiskit/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.479200 qbraid-0.3.0/qbraid/interface/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/tests/test_calculate_unitary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/tests/test_convert_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/interface/tests/test_programs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.479200 qbraid-0.3.0/qbraid/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/tests/test_top_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.479200 qbraid-0.3.0/qbraid/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.479200 qbraid-0.3.0/qbraid/transpiler/cirq_braket/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_braket/convert_from_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_braket/convert_from_braket_qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_braket/convert_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_braket/custom_gates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.479200 qbraid-0.3.0/qbraid/transpiler/cirq_braket/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_braket/tests/_gate_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_braket/tests/test_from_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_braket/tests/test_from_braket_qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_braket/tests/test_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_braket/tests/test_to_braket_measure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.479200 qbraid-0.3.0/qbraid/transpiler/cirq_pyquil/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_pyquil/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.479200 qbraid-0.3.0/qbraid/transpiler/cirq_pyquil/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_pyquil/tests/test_conversions_pyquil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.479200 qbraid-0.3.0/qbraid/transpiler/cirq_pytket/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_pytket/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.479200 qbraid-0.3.0/qbraid/transpiler/cirq_pytket/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_pytket/tests/test_conversions_pytket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_pytket/tests/test_from_pytket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_pytket/tests/test_to_pytket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.483199 qbraid-0.3.0/qbraid/transpiler/cirq_qasm/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qasm/qasm_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qasm/qasm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qasm/qasm_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.483199 qbraid-0.3.0/qbraid/transpiler/cirq_qasm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qasm/tests/_gate_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qasm/tests/test_qasm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qasm/tests/test_qasm_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.483199 qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.483199 qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/tests/_gate_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/tests/test_conversions_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/tests/test_from_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/tests/test_to_qiskit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.483199 qbraid-0.3.0/qbraid/transpiler/code/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/code/qasm_to_braket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.483199 qbraid-0.3.0/qbraid/transpiler/code/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/code/tests/test_qasm_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/custom_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.483199 qbraid-0.3.0/qbraid/transpiler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/tests/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.483199 qbraid-0.3.0/qbraid/transpiler/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/wrappers/abc_qprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/wrappers/braket_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/wrappers/cirq_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/wrappers/pyquil_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/wrappers/pytket_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/transpiler/wrappers/qiskit_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-11 19:29:20.000000 qbraid-0.3.0/qbraid/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:29:31.471199 qbraid-0.3.0/qbraid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-05-11 19:29:31.000000 qbraid-0.3.0/qbraid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-05-11 19:29:31.000000 qbraid-0.3.0/qbraid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:29:31.000000 qbraid-0.3.0/qbraid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-11 19:29:31.000000 qbraid-0.3.0/qbraid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-11 19:29:31.000000 qbraid-0.3.0/qbraid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 19:29:31.000000 qbraid-0.3.0/qbraid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-11 19:29:20.000000 qbraid-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-11 19:29:20.000000 qbraid-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-11 19:29:31.487200 qbraid-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-11 19:29:20.000000 qbraid-0.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-11 19:29:20.000000 qbraid-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.753776 qbraid-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-16 22:30:06.000000 qbraid-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 22:30:06.000000 qbraid-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-16 22:30:06.000000 qbraid-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-16 22:30:19.753776 qbraid-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-05-16 22:30:06.000000 qbraid-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.713776 qbraid-0.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.713776 qbraid-0.4.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.713776 qbraid-0.4.0/docs/_static/account/
+-rw-r--r--   0 runner    (1001) docker     (123)    80371 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/account/account_access_key.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27399 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/account/account_profile_details.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.713776 qbraid-0.4.0/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.721776 qbraid-0.4.0/docs/_static/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)   358114 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_add.png
+-rw-r--r--   0 runner    (1001) docker     (123)   236606 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_add_package.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112288 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_create.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41898 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_custom_installing.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40671 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_custom_pkgs.png
+-rw-r--r--   0 runner    (1001) docker     (123)   497786 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_install.png
+-rw-r--r--   0 runner    (1001) docker     (123)   450900 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_installing.png
+-rw-r--r--   0 runner    (1001) docker     (123)   394044 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_more.png
+-rw-r--r--   0 runner    (1001) docker     (123)   545265 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_new.png
+-rw-r--r--   0 runner    (1001) docker     (123)   148896 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_pkg_install.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47510 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/environments/env_share.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.721776 qbraid-0.4.0/docs/_static/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)   108308 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/errors/sidebar_glitch.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.721776 qbraid-0.4.0/docs/_static/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/0_file_control_panel.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/1_top_bar_token.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/2_request_token.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/3_copy_token.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/4_jupyter_server.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/5_existing_uri.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/6_example_user.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/7_notebook_kernel.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34868 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/8_select_kernel.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85020 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/os.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34944 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/integrations/vscode_graphic.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.721776 qbraid-0.4.0/docs/_static/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)   411673 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/jobs/jobs_ionq.png
+-rw-r--r--   0 runner    (1001) docker     (123)   592257 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/jobs/jobs_sdk.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85873 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/jobs/jobs_tag.png
+-rw-r--r--   0 runner    (1001) docker     (123)   154811 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.725776 qbraid-0.4.0/docs/_static/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/notebooks/file_browser.png
+-rw-r--r--   0 runner    (1001) docker     (123)   451731 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/notebooks/kernel_activate.png
+-rw-r--r--   0 runner    (1001) docker     (123)   510341 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/notebooks/kernel_deactivate.png
+-rw-r--r--   0 runner    (1001) docker     (123)   290430 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/notebooks/kernel_nb.png
+-rw-r--r--   0 runner    (1001) docker     (123)   346617 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/notebooks/kernel_switch.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/notebooks/share_notebook.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.725776 qbraid-0.4.0/docs/_static/pkg-logos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36600 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/braket.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53519 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/cirq.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/pyquil.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28492 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/pytket.png
+-rw-r--r--   0 runner    (1001) docker     (123)   125852 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/qasm.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/qiskit.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/pkg-logos/xanadu.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.729776 qbraid-0.4.0/docs/_static/sdk-files/
+-rw-r--r--   0 runner    (1001) docker     (123)   447304 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/sdk-files/get_devices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53194 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/_static/sdk-files/plot_counts.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.729776 qbraid-0.4.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.devices.aws.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.devices.ibm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_braket.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_pyquil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_pytket.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_qiskit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/api/qbraid.transpiler.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.733776 qbraid-0.4.0/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/envs-activate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/envs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/envs-uninstall.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/envs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/jobs-add.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/jobs-disable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/jobs-enable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/jobs-get-credits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/jobs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/kernels.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/cli/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.733776 qbraid-0.4.0/docs/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/account.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/environments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/integrations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/quantumjobs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/system.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/lab/troubleshoot.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.733776 qbraid-0.4.0/docs/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/sdk/circuits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/sdk/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/sdk/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/sdk/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-16 22:30:06.000000 qbraid-0.4.0/docs/sdk/results.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-16 22:30:06.000000 qbraid-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.737776 qbraid-0.4.0/qbraid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/_qprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.737776 qbraid-0.4.0/qbraid/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/job_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.737776 qbraid-0.4.0/qbraid/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/tests/test_api_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/api/tests/test_api_thirdparty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.737776 qbraid-0.4.0/qbraid/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/devices/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/aws/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/aws/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/aws/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/devices/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/ibm/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/ibm/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/ibm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/ibm/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/devices/ibm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/ibm/tests/test_ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/status_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/devices/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/devices/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/display_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/get_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/calculate_unitary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/convert_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/programs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/interface/qbraid_braket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_braket/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_braket/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/interface/qbraid_cirq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_cirq/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_cirq/circuits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.741776 qbraid-0.4.0/qbraid/interface/qbraid_cirq/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_cirq/tests/test_cirq_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_cirq/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/interface/qbraid_pyquil/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_pyquil/programs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_pyquil/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/interface/qbraid_pytket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_pytket/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_pytket/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/interface/qbraid_qasm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qasm/circuits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/interface/qbraid_qasm/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qasm/test/test_qasm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qasm/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/interface/qbraid_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qiskit/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/qbraid_qiskit/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/interface/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/tests/test_calculate_unitary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/tests/test_convert_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/interface/tests/test_programs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/tests/test_top_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/transpiler/cirq_braket/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/convert_from_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/convert_from_braket_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/convert_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/custom_gates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.745776 qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/_gate_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_from_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_from_braket_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_to_braket_measure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/tests/test_conversions_pyquil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/test_conversions_pytket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/test_from_pytket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/test_to_pytket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/qasm_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/qasm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/qasm_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/_gate_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/test_qasm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/test_qasm_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/_gate_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/test_conversions_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/test_from_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/test_to_qiskit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/code/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/code/qasm_to_braket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/code/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/code/tests/test_qasm_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/custom_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/tests/test_transpiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.749776 qbraid-0.4.0/qbraid/transpiler/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/abc_qprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/braket_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/cirq_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/pyquil_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/pytket_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/qasm_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/transpiler/wrappers/qiskit_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-16 22:30:06.000000 qbraid-0.4.0/qbraid/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.737776 qbraid-0.4.0/qbraid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-16 22:30:19.000000 qbraid-0.4.0/qbraid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-16 22:30:19.000000 qbraid-0.4.0/qbraid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:30:19.000000 qbraid-0.4.0/qbraid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-16 22:30:19.000000 qbraid-0.4.0/qbraid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-16 22:30:19.000000 qbraid-0.4.0/qbraid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 22:30:19.000000 qbraid-0.4.0/qbraid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-16 22:30:06.000000 qbraid-0.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-16 22:30:06.000000 qbraid-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-16 22:30:19.753776 qbraid-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-16 22:30:06.000000 qbraid-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:30:19.753776 qbraid-0.4.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-16 22:30:06.000000 qbraid-0.4.0/tools/verify_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-16 22:30:06.000000 qbraid-0.4.0/tox.ini
```

### Comparing `qbraid-0.3.0/LICENSE` & `qbraid-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/PKG-INFO` & `qbraid-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,97 @@
-Metadata-Version: 2.1
-Name: qbraid
-Version: 0.3.0
-Summary: A Python toolkit for cross-framework abstraction of quantum programs.
-Home-page: https://github.com/qBraid/qBraid/
-Author: qBraid Development Team
-Author-email: contact@qbraid.com
-License: Restricted
-Keywords: qbraid,quantum
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-License-File: LICENSE
-
 <img width=full alt="qbraid-sdk-header" src="https://user-images.githubusercontent.com/46977852/224456452-605e51f2-193d-4789-863e-e51cdd4b0a54.png">
 
-[![CI](https://github.com/qBraid/qBraid/actions/workflows/main.yml/badge.svg)](https://github.com/qBraid/qBraid/actions/workflows/main.yml)
+[![CI](https://github.com/qBraid/qBraid/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/qBraid/qBraid/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/qBraid/qBraid/branch/main/graph/badge.svg?token=1UTM0XZB7A)](https://codecov.io/gh/qBraid/qBraid)
 [![Documentation Status](https://readthedocs.com/projects/qbraid-qbraid/badge/?version=latest)](https://docs.qbraid.com/en/latest/?badge=latest)
+[![PyPI version](https://img.shields.io/pypi/v/qbraid.svg?color=blue)](https://pypi.org/project/qbraid/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-The qBraid-SDK is a Python toolkit for cross-framework abstraction, transpilation, and execution of quantum programs.
+The qBraid-SDK is a Python toolkit for cross-framework abstraction,
+transpilation, and execution of quantum programs.
 
 [<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png" width="150">](https://account.qbraid.com?gitHubUrl=https://github.com/qBraid/qBraid.git)
 
-
 ## Features
 
-- Unified quantum frontend interface. **Transpile** quantum circuits between supported packages. Leverage the capabilities of multiple frontends through **simple, consistent protocols**.
-- Build once, target many. **Create** quantum programs using your preferred circuit-building package, and **execute** on any backend that interfaces with a supported frontend.
-- Benchmark, compare, interpret results. Built-in **compatible** post-processing enables comparing results between runs and **across backends**.
-
-
-## Installation
+- Unified quantum frontend interface. **Transpile** quantum circuits between
+  supported packages. Leverage the capabilities of multiple frontends through
+  **simple, consistent protocols**.
+- Build once, target many. **Create** quantum programs using your preferred
+  circuit-building package, and **execute** on any backend that interfaces with
+  a supported frontend.
+- Benchmark, compare, interpret results. Built-in **compatible** post-processing
+  enables comparing results between runs and **across backends**.
+
+## Installation & Setup
+
+<img align="right" width="300" alt="qbraid-sdk-env" src="https://github.com/qBraid/qBraid/assets/46977852/669bd6f3-bbef-428c-9b59-b421c940262e">
+
+For the best experience, install the qBraid-SDK environment on
+[lab.qbraid.com](https://lab.qbraid.com). Login (or
+[create an account](https://account.qbraid.com)) and follow the steps to
+[install an environment](https://docs.qbraid.com/en/latest/lab/environments.html#install-environment).
+
+Using the SDK on qBraid Lab means direct, pre-configured access to all
+[Amazon Braket supported devices](https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html)
+and [IBM Quantum open systems](https://www.ibm.com/quantum/access-plans) with no
+additional access keys or API tokens required. See
+[qBraid Quantum Jobs](https://docs.qbraid.com/en/latest/lab/quantumjobs.html)
+for more.
 
-For the best experience, install the qBraid-SDK environment on [qBraid Lab](https://lab.qbraid.com). Login (or create an account) and then follow the steps to [install an environment](https://docs.qbraid.com/en/latest/lab/environments.html#install-environment).
+### Local install
 
 The qBraid-SDK, and all of its dependencies, can also be installed using pip:
 
 ```bash
 pip install qbraid
 ```
 
-## Quickstart
+If using locally, follow linked instructions to configure your
+[qBraid](#local-account-setup),
+[AWS](https://github.com/aws/amazon-braket-sdk-python#boto3-and-setting-up-aws-credentials),
+and [IBMQ](https://github.com/Qiskit/qiskit-ibm-provider#provider-setup)
+credentials.
+
+## Documentation & Tutorials
+
+qBraid documentation is available at
+[docs.qbraid.com](https://docs.qbraid.com/en/latest/).
+
+See also:
+
+- [API Reference](https://docs.qbraid.com/en/latest/api/qbraid.html)
+- [User Guide](https://docs.qbraid.com/en/latest/sdk/overview.html)
+- [Example Notebooks](https://github.com/qBraid/qbraid-lab-demo)
 
-For more in-depth examples, see [user guide](https://docs.qbraid.com/en/latest/sdk/overview.html) and [demo notebooks](https://github.com/qBraid/qbraid-lab-demo).
+## Quickstart
 
 ### Transpiler
 
-Construct a quantum program of any supported program type, 
+Construct a quantum program of any supported program type,
 
 ```python
 >>> from qbraid import QPROGRAM_LIBS
 >>> QPROGRAM_LIBS
-['braket', 'cirq', 'qiskit', 'pyquil', 'pytket']
+['braket', 'cirq', 'qiskit', 'pyquil', 'pytket', 'qasm']
 ```
 
 and use the `circuit_wrapper()` to convert to any other supported program type:
 
 ```python
 >>> from qbraid import circuit_wrapper
 >>> from qbraid.interface import random_circuit
 >>> qiskit_circuit = random_circuit("qiskit")
 >>> cirq_circuit = circuit_wrapper(qiskit_circuit).transpile("cirq")
 >>> print(qiskit_circuit)
           ┌────────────┐
 q_0: ──■──┤ Rx(3.0353) ├
      ┌─┴─┐└───┬────┬───┘
 q_1: ┤ H ├────┤ √X ├────
-     └───┘    └────┘    
+     └───┘    └────┘
 >>> print(cirq_circuit)
 0: ───H───X^0.5────────
       │
 1: ───@───Rx(0.966π)───
 ```
 
 ### Devices & Jobs
@@ -99,15 +109,16 @@
 aws_rigetti_aspen_m2                OFFLINE
 aws_rigetti_aspen_m3                ONLINE
 ibm_q_perth                         ONLINE
 ...
 
 ```
 
-Apply the `device_wrapper()`, and send quantum jobs to any supported backend, from any supported program type:
+Apply the `device_wrapper()`, and send quantum jobs to any supported backend,
+from any supported program type:
 
 ```python
 >>> from qbraid import device_wrapper, get_jobs
 >>> aws_device = device_wrapper("aws_oqc_lucy")
 >>> ibm_device = device_wrapper("ibm_q_perth")
 >>> aws_job = aws_device.run(qiskit_circuit, shots=1000)
 >>> ibm_job = ibm_device.run(cirq_circuit, shots=1000)
@@ -128,114 +139,92 @@
 >>> ibm_result = ibm_job.result()
 >>> aws_result.measurement_counts()
 {'00': 483, '01': 14, '10': 486, '11': 17}
 >>> ibm_result.measurement_counts()
 {'00': 496, '01': 12, '10': 479, '11': 13}
 ```
 
-## Local Setup
+## Local account setup
+<img mg align="right" width="350" alt="api_key" src="https://github.com/qBraid/qBraid/assets/32727721/d087c404-e9c7-4a0b-b2a5-a58f2e483cce">
+
+
+To use the qBraid-SDK locally (outside of qBraid Lab), you must add your account
+credentials:
 
-To use the qBraid-SDK locally (outside of qBraid Lab), you must add your account credentials:
+1. Create a qBraid account or log in to your existing account by visiting
+   [account.qbraid.com](https://account.qbraid.com/v2)
+2. Copy your API Key token from the left side of
+    your [account page](https://account.qbraid.com/v2):
 
-1. Create a qBraid account or log in to your existing account by visiting https://account.qbraid.com
-2. Copy your API (refresh) token from your qBraid account page:
-- Login to your account and open DevTools / inspector window (MacOS: Option-Command-I)
-- Go to Application -> Storage -> Cookies -> https://account.qbraid.com
-- The value corresponding to `REFRESH` is your API refresh token.
-  Note, this token is updated monthly.
-3. Take your account email and refresh token from step 2, and save it by calling `QbraidSession.save_config()`:
+3. Save your API key from step 2 by calling
+   `QbraidSession.save_config()`:
 
 ```python
 from qbraid.api import QbraidSession
 
-session = QbraidSession(user_email='USER_EMAIL', refresh_token='REFRESH_TOKEN')
+session = QbraidSession(api_key='API_KEY')
 session.save_config()
 ```
 
-The command above stores your credentials locally in a configuration file called `qbraidrc` in `$HOME/.qbraid`, where `$HOME` is your home directory. Once saved you can then connect to the qBraid API and leverage functions such as `get_devices()` and `get_jobs()`.
+The command above stores your credentials locally in a configuration file `~/.qbraid/qbraidrc`,
+where `~` corresponds to your home (`$HOME`) directory. Once saved, you can then connect to the
+qBraid API and leverage functions such as `get_devices()` and `get_jobs()`.
 
 ### Load Account from Environment Variables
 
-Alternatively, the qBraid-SDK can discover credentials from environment variables:
+Alternatively, the qBraid-SDK can discover credentials from environment
+variables:
 
 ```bash
 export JUPYTERHUB_USER='USER_EMAIL'
-export REFRESH='REFRESH_TOKEN'
+export QBRAID_API_KEY='QBRAID_API_KEY'
 ```
 
 Then instantiate the session without any arguments
 
 ```python
 from qbraid.api import QbraidSession
 
 session = QbraidSession()
 ```
 
-## Documentation
-
-The API reference can be found on [Read the Docs](https://docs.qbraid.com/en/latest/api/qbraid.html).
-
-To generate the API reference documentation locally:
-
-```bash
-pip install tox<4
-tox -e docs
-```
-
-Alternatively:
-```bash
-pip install -e ".[docs]"
-cd docs
-make html
-```
+## Launch on qBraid
 
-Both methods will run Sphinx in your shell. If the build results in an `InvocationError` due to a 
-duplicate object description, try `rm docs/stubs/*` to empty the old stubs directory, and then 
-re-start the build. If the build succeeds, it will say `The HTML pages are in build/html`. You can 
-view the generated documentation in your browser (on OS X) using:
+The "Launch on qBraid" button (below) can be added to any public GitHub
+repository. Clicking on it automaically opens qBraid Lab, and performs a
+`git clone` of the project repo into your account's home directory. Copy the
+code below, and replace `YOUR-USERNAME` and `YOUR-REPOSITORY` with your GitHub
+info.
 
-```bash
-open build/html/index.html
-```
+[<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png" width="150">](https://account.qbraid.com?gitHubUrl=https://github.com/qBraid/qBraid.git)
 
-You can also view it by running a web server in that directory:
+Use the badge in your project's `README.md`:
 
-```bash
-cd build/html
-python3 -m http.server
 ```
-Then open your browser to http://localhost:8000. If you make changes to the docs that aren't
-reflected in subsequent builds, run `make clean html`, which will force a full rebuild.
-
-## Testing
-
-To run all unit tests:
-
-```bash
-pip install tox<4
-tox -e unit-tests
+[<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png" width="150">](https://account.qbraid.com?gitHubUrl=https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git)
 ```
 
-You can also pass in various pytest arguments to run selected tests:
+Use the badge in your project's `README.rst`:
 
-```bash
-tox -e unit-tests -- {your-arguments}
 ```
-
-Alternatively:
-
-```bash
-pip install -e ".[test]"
-pytest {path-to-test}
+.. image:: https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png
+    :target: https://account.qbraid.com?gitHubUrl=https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
+    :width: 150px
 ```
 
-Running unit tests with tox will automatically generate a coverage report, which can be viewed by
-opening `tests/_coverage/index.html` in your browser.
+## Contributing
 
-To run linters and doc generators and unit tests:
-```bash
-tox
-```
+- Interested in contributing code, or making a PR? See
+  [CONTRIBUTING.md](CONTRIBUTING.md)
+- For feature requests and bug reports:
+  [Submit an issue](https://github.com/qBraid/qBraid/issues)
+- For discussions, and specific questions about the qBraid SDK, qBraid Lab, or
+  other topics, [join our discord community](https://discord.gg/gwBebaBZZX)
+- For questions that are more suited for a forum, use the `qbraid` tag on
+  [Stack Exchange](https://quantumcomputing.stackexchange.com/)
+- Want your open-source project featured as its own runtime environment on
+  qBraid Lab? Fill out our
+  [New Environment Request Form](https://forms.gle/a4v7Kdn7G7bs9jYD8)
 
 ## License
 
 [GNU General Public License v3.0](LICENSE)
```

### Comparing `qbraid-0.3.0/docs/_static/account/account_access_key.png` & `qbraid-0.4.0/docs/_static/account/account_access_key.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/account/account_profile_details.png` & `qbraid-0.4.0/docs/_static/account/account_profile_details.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/cards/jupyter.png` & `qbraid-0.4.0/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/cards/python.png` & `qbraid-0.4.0/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/cards/terminal.png` & `qbraid-0.4.0/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/environments/env_add.png` & `qbraid-0.4.0/docs/_static/environments/env_add.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/environments/env_add_package.png` & `qbraid-0.4.0/docs/_static/environments/env_add_package.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/environments/env_create.png` & `qbraid-0.4.0/docs/_static/environments/env_create.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/environments/env_custom_installing.png` & `qbraid-0.4.0/docs/_static/environments/env_custom_installing.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/environments/env_custom_pkgs.png` & `qbraid-0.4.0/docs/_static/environments/env_custom_pkgs.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/environments/env_install.png` & `qbraid-0.4.0/docs/_static/environments/env_install.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/environments/env_installing.png` & `qbraid-0.4.0/docs/_static/environments/env_installing.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/environments/env_more.png` & `qbraid-0.4.0/docs/_static/environments/env_more.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/environments/env_new.png` & `qbraid-0.4.0/docs/_static/environments/env_new.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/environments/env_pkg_install.png` & `qbraid-0.4.0/docs/_static/environments/env_pkg_install.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/environments/env_share.png` & `qbraid-0.4.0/docs/_static/environments/env_share.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/errors/sidebar_glitch.png` & `qbraid-0.4.0/docs/_static/errors/sidebar_glitch.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/favicon.ico` & `qbraid-0.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/integrations/0_file_control_panel.png` & `qbraid-0.4.0/docs/_static/integrations/0_file_control_panel.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/integrations/1_top_bar_token.png` & `qbraid-0.4.0/docs/_static/integrations/1_top_bar_token.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/integrations/2_request_token.png` & `qbraid-0.4.0/docs/_static/integrations/2_request_token.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/integrations/3_copy_token.png` & `qbraid-0.4.0/docs/_static/integrations/3_copy_token.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/integrations/4_jupyter_server.png` & `qbraid-0.4.0/docs/_static/integrations/4_jupyter_server.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/integrations/5_existing_uri.png` & `qbraid-0.4.0/docs/_static/integrations/5_existing_uri.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/integrations/6_example_user.png` & `qbraid-0.4.0/docs/_static/integrations/6_example_user.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/integrations/7_notebook_kernel.png` & `qbraid-0.4.0/docs/_static/integrations/7_notebook_kernel.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/integrations/8_select_kernel.png` & `qbraid-0.4.0/docs/_static/integrations/8_select_kernel.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/integrations/os.png` & `qbraid-0.4.0/docs/_static/integrations/os.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/integrations/vscode_graphic.png` & `qbraid-0.4.0/docs/_static/integrations/vscode_graphic.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/jobs/jobs_ionq.png` & `qbraid-0.4.0/docs/_static/jobs/jobs_ionq.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/jobs/jobs_sdk.png` & `qbraid-0.4.0/docs/_static/jobs/jobs_sdk.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/jobs/jobs_tag.png` & `qbraid-0.4.0/docs/_static/jobs/jobs_tag.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/logo.png` & `qbraid-0.4.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/notebooks/file_browser.png` & `qbraid-0.4.0/docs/_static/notebooks/file_browser.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/notebooks/kernel_activate.png` & `qbraid-0.4.0/docs/_static/notebooks/kernel_activate.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/notebooks/kernel_deactivate.png` & `qbraid-0.4.0/docs/_static/notebooks/kernel_deactivate.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/notebooks/kernel_nb.png` & `qbraid-0.4.0/docs/_static/notebooks/kernel_nb.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/notebooks/kernel_switch.png` & `qbraid-0.4.0/docs/_static/notebooks/kernel_switch.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/notebooks/share_notebook.png` & `qbraid-0.4.0/docs/_static/notebooks/share_notebook.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/pkg-logos/braket.png` & `qbraid-0.4.0/docs/_static/pkg-logos/braket.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/pkg-logos/cirq.png` & `qbraid-0.4.0/docs/_static/pkg-logos/cirq.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/pkg-logos/pyquil.png` & `qbraid-0.4.0/docs/_static/pkg-logos/pyquil.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/pkg-logos/pytket.png` & `qbraid-0.4.0/docs/_static/pkg-logos/pytket.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/pkg-logos/qiskit.png` & `qbraid-0.4.0/docs/_static/pkg-logos/qiskit.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/pkg-logos/xanadu.png` & `qbraid-0.4.0/docs/_static/pkg-logos/xanadu.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/sdk-files/get_devices.png` & `qbraid-0.4.0/docs/_static/sdk-files/get_devices.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/_static/sdk-files/plot_counts.png` & `qbraid-0.4.0/docs/_static/sdk-files/plot_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/api/qbraid.devices.aws.rst` & `qbraid-0.4.0/docs/api/qbraid.devices.aws.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/api/qbraid.devices.ibm.rst` & `qbraid-0.4.0/docs/api/qbraid.devices.ibm.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/api/qbraid.interface.rst` & `qbraid-0.4.0/docs/api/qbraid.interface.rst`

 * *Files 1% similar despite different names*

```diff
@@ -21,7 +21,12 @@
    :undoc-members:
    :show-inheritance:
 
 .. automodule:: qbraid.interface.qbraid_qiskit
    :members:
    :undoc-members:
    :show-inheritance:
+
+.. automodule:: qbraid.interface.qbraid_qasm
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `qbraid-0.3.0/docs/api/qbraid.transpiler.cirq_braket.rst` & `qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_braket.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/api/qbraid.transpiler.cirq_utils.rst` & `qbraid-0.4.0/docs/api/qbraid.transpiler.cirq_utils.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/api/qbraid.transpiler.rst` & `qbraid-0.4.0/docs/api/qbraid.transpiler.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/cli/envs-activate.rst` & `qbraid-0.4.0/docs/cli/envs-activate.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/cli/envs-list.rst` & `qbraid-0.4.0/docs/cli/envs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/cli/envs-uninstall.rst` & `qbraid-0.4.0/docs/cli/envs-uninstall.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/cli/envs.rst` & `qbraid-0.4.0/docs/cli/envs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/cli/jobs-add.rst` & `qbraid-0.4.0/docs/cli/jobs-add.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/cli/jobs-disable.rst` & `qbraid-0.4.0/docs/cli/jobs-disable.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/cli/jobs-enable.rst` & `qbraid-0.4.0/docs/cli/jobs-enable.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/cli/jobs-list.rst` & `qbraid-0.4.0/docs/cli/jobs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/cli/jobs.rst` & `qbraid-0.4.0/docs/cli/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/cli/kernels.rst` & `qbraid-0.4.0/docs/cli/kernels.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/cli/qbraid.rst` & `qbraid-0.4.0/docs/cli/qbraid.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/conf.py` & `qbraid-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/index.rst` & `qbraid-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/lab/account.rst` & `qbraid-0.4.0/docs/lab/account.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/lab/environments.rst` & `qbraid-0.4.0/docs/lab/environments.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/lab/files.rst` & `qbraid-0.4.0/docs/lab/files.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/lab/integrations.rst` & `qbraid-0.4.0/docs/lab/integrations.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/lab/notebooks.rst` & `qbraid-0.4.0/docs/lab/notebooks.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/lab/overview.rst` & `qbraid-0.4.0/docs/lab/overview.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/lab/quantumjobs.rst` & `qbraid-0.4.0/docs/lab/quantumjobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/lab/system.rst` & `qbraid-0.4.0/docs/lab/system.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/lab/troubleshoot.rst` & `qbraid-0.4.0/docs/lab/troubleshoot.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/sdk/circuits.rst` & `qbraid-0.4.0/docs/sdk/circuits.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,36 +7,38 @@
 quantum circuit objects accross various frontends. We will demonstrate how to
 use the transpiler to convert circuits between packages, and highlight a few
 other circuit-based convenience features.
 
 Program Types
 --------------
 
-Supported frontend program types include `Qiskit QuantumCircuit <QiskitQuantumCircuit>`_,
-`Braket Circuit <BraketCircuit>`_, `Cirq Circuit <CirqCircuit>`_, `PyQuil Program <PyQuilProgram>`_
-and `PyTKET Circuit <PyTKETCircuit>`_:
+Supported frontend program types include `Qiskit <QiskitQuantumCircuit>`_,
+`Amazon Braket <BraketCircuit>`_, `Cirq <CirqCircuit>`_, `PyQuil <PyQuilProgram>`_,
+`PyTKET <PyTKETCircuit>`_, and `OpenQASM <OpenQASMString>`_:
 
 .. code-block:: python
     
     >>> from qbraid import QPROGRAM_TYPES
     >>> for k in QPROGRAM_TYPES:
     ...     print(k)
     ...
     braket.circuits.circuit.Circuit
     cirq.circuits.circuit.Circuit
     qiskit.circuit.quantumcircuit.QuantumCircuit
     pyquil.quil.Program
     pytket._tket.circuit.Circuit
+    qasm
 
 
 .. _QiskitQuantumCircuit: https://qiskit.org/documentation/stubs/qiskit.circuit.QuantumCircuit.html
 .. _BraketCircuit: https://docs.aws.amazon.com/braket/latest/developerguide/braket-constructing-circuit.html
 .. _CirqCircuit: https://quantumai.google/reference/python/cirq/circuits/Circuit
 .. _PyQuilProgram: https://pyquil-docs.rigetti.com/en/stable/basics.html
 .. _PyTKETCircuit: https://cqcl.github.io/tket/pytket/api/circuit_class.html
+.. _OpenQASMString: https://openqasm.com/language/index.html
 
 
 Circuit Wrapper
 ----------------
 
 We'll start with a simple qiskit circuit that creates the bell state.
```

### Comparing `qbraid-0.3.0/docs/sdk/devices.rst` & `qbraid-0.4.0/docs/sdk/devices.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/sdk/jobs.rst` & `qbraid-0.4.0/docs/sdk/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/docs/sdk/overview.rst` & `qbraid-0.4.0/docs/sdk/overview.rst`

 * *Files 16% similar despite different names*

```diff
@@ -29,30 +29,45 @@
 
 - *Benchmark, compare, interpret results*. Built-in **compatible** post-processing enables comparing results between runs and **across backends**.
 
 
 Installation
 -------------
 
-The qBraid SDK is available exclusively through `qBraid Lab <https://lab.qbraid.com>`_.
-Login (or create an account) and then follow the steps in `Install environment <../lab/environments.html#install-environment>`_
-to get started using the SDK.
+For the best experience, install the qBraid SDK on `lab.qbraid.com <https://lab.qbraid.com>`_.
+Login (or create an account) on `account.qbraid.com <https://account.qbraid.com/v2>`_ and then
+follow the steps to `install an environment <../lab/environments.html#install-environment>`_.
+Using the SDK on qBraid Lab means direct, pre-configured access to all
+`Amazon Braket supported devices <https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html>`_
+and `IBM Quantum open systems <https://www.ibm.com/quantum/access-plans>`_
+with *no additional access keys or API tokens required*. See `qBraid Quantum Jobs <../lab/quantumjobs.html>`_ for more.
+
+The qBraid-SDK, and all of its dependencies, can also be installed using `pip <https://pypi.org/project/qbraid/>`_:
+
+.. code-block:: bash
+
+   pip install qbraid
+
+
+If using locally, follow linked instructions to configure your `qBraid <https://github.com/qBraid/qBraid#local-account-setup>`_,
+`AWS <https://github.com/aws/amazon-braket-sdk-python#boto3-and-setting-up-aws-credentials>`_,
+and `IBMQ <https://github.com/Qiskit/qiskit-ibm-provider#provider-setup>`_ credentials.
 
 
 Usage
 ------
 
 Construct a quantum program of any supported program type:
 
 .. code-block:: python
    
    >>> from qbraid import QPROGRAM_LIBS
    >>> from qbraid.interface import random_circuit
    >>> QPROGRAM_LIBS
-   ['braket', 'cirq', 'qiskit', 'pyquil', 'pytket']
+   ['braket', 'cirq', 'qiskit', 'pyquil', 'pytket', 'qasm']
    >>> circuit = random_circuit("qiskit", num_qubits=1, measure=True)
 
 Search for quantum backend(s) on which to execute your program:
 
 .. code-block:: python
 
    >>> from qbraid import get_devices
@@ -107,19 +122,19 @@
    aws_oqc_lucy         {'0': 477, '1': 547}
    ibm_q_perth          {'0': 550, '1': 474}
 
 
 Supported Frontends
 ^^^^^^^^^^^^^^^^^^^^
 
-+-------------+-------------+------------+-------------+-------------+
-|  Cirq_      |  Braket_    |  Qiskit_   |  PyQuil_    |  PyTKET_    |
-+=============+=============+============+=============+=============+
-| |cirq|      | |braket|    | |qiskit|   | |pyquil|    | |pytket|    |
-+-------------+-------------+------------+-------------+-------------+
++-------------+-------------+------------+-------------+-------------+-------------+
+|  Cirq_      |  Braket_    |  Qiskit_   |  PyQuil_    |  PyTKET_    |  QASM_      |
++=============+=============+============+=============+=============+=============+
+| |cirq|      | |braket|    | |qiskit|   | |pyquil|    | |pytket|    | |qasm|      |
++-------------+-------------+------------+-------------+-------------+-------------+
 
 
 .. |cirq| image:: ../_static/pkg-logos/cirq.png
    :align: middle
    :width: 70%
    :target: Cirq_
 
@@ -139,19 +154,24 @@
    :target: PyQuil_
 
 .. |pytket| image:: ../_static/pkg-logos/pytket.png
    :align: middle
    :width: 70%
    :target: PyTKET_
 
+.. |qasm| image:: ../_static/pkg-logos/qasm.png
+   :align: middle
+   :width: 70%
+   :target: QASM_
+
 .. .. |pennylane| image:: ../_static/pkg-logos/xanadu.png
 ..    :align: middle
 ..    :width: 90%
 ..    :target: Pennylane_
 
 .. _Cirq: https://quantumai.google/cirq
 .. _Braket: https://aws.amazon.com/braket
 .. _Qiskit: https://qiskit.org
 .. _PyQuil: https://www.rigetti.com/applications/pyquil
 .. _PyTKET: https://cqcl.github.io/tket/pytket/api/
-.. _Pennylane: https://pennylane.ai
-.. _qBraid: https://qbraid.com/
+.. _QASM: https://openqasm.com/
+.. _Pennylane: https://pennylane.ai
```

### Comparing `qbraid-0.3.0/docs/sdk/results.rst` & `qbraid-0.4.0/docs/sdk/results.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/pyproject.toml` & `qbraid-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/__init__.py` & `qbraid-0.4.0/qbraid/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/_qprogram.py` & `qbraid-0.4.0/qbraid/_qprogram.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 from braket.circuits import Circuit as _BraketCircuit
 from cirq import Circuit as _CirqCircuit
 from pyquil import Program as _pyQuilProgram
 from pytket.circuit import Circuit as _PytketCircuit
 from qiskit import QuantumCircuit as _QiskitCircuit
 
 # Supported quantum programs.
+QASMType = str
 QPROGRAM = Union[_BraketCircuit, _CirqCircuit, _QiskitCircuit, _pyQuilProgram, _PytketCircuit]
 
 _PROGRAMS = [_BraketCircuit, _CirqCircuit, _QiskitCircuit, _pyQuilProgram, _PytketCircuit]
 
 # pylint: disable-next=bad-str-strip-call
 QPROGRAM_TYPES = [str(x).strip("<class").strip(">").strip(" ").strip("'") for x in _PROGRAMS]
+QPROGRAM_TYPES.append("qasm")
 
 QPROGRAM_LIBS = [x.split(".")[0] for x in QPROGRAM_TYPES]
```

### Comparing `qbraid-0.3.0/qbraid/_version.py` & `qbraid-0.4.0/qbraid/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
 """
 Module containing version information
 
 Version number (major.minor.patch[-label])
 
 """
-__version__ = "0.3.0"
+__version__ = "0.4.0"
```

### Comparing `qbraid-0.3.0/qbraid/_warnings.py` & `qbraid-0.4.0/qbraid/_warnings.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 
 warnings.filterwarnings("ignore", category=SyntaxWarning)
 warnings.filterwarnings("ignore", category=UserWarning, message="Setuptools is replacing distutils")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 warnings.filterwarnings("ignore", category=PendingDeprecationWarning)
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-_check_version()
+# _check_version()
```

### Comparing `qbraid-0.3.0/qbraid/api/__init__.py` & `qbraid-0.4.0/qbraid/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
    .. rubric:: Attributes
 
    .. autosummary::
 
       ~QbraidSession.base_url
       ~QbraidSession.user_email
+      ~QbraidSession.api_key
       ~QbraidSession.refresh_token
 
 """
 from .exceptions import ApiError, AuthError, ConfigError, RequestsApiError
 from .job_api import get_job_data, init_job
 from .retry import PostForcelistRetry
 from .session import QbraidSession
```

### Comparing `qbraid-0.3.0/qbraid/api/exceptions.py` & `qbraid-0.4.0/qbraid/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/api/job_api.py` & `qbraid-0.4.0/qbraid/api/job_api.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/api/retry.py` & `qbraid-0.4.0/qbraid/api/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/api/session.py` & `qbraid-0.4.0/qbraid/api/session.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,37 +35,40 @@
 
     This is a child class of :py:class:`requests.Session`. It handles qbraid
     authentication with custom headers, has SSL verification disabled
     for compatibility with lab, and returns all responses as jsons for
     convenience in the sdk.
 
     Args:
-        base_url: Base URL for the session's requests.
         user_email: qBraid / JupyterHub User.
+        api_key: Authenticated qBraid API key.
         refresh_token: Authenticated qBraid refresh-token.
+        base_url: Base URL for the session's requests.
         retries_total: Number of total retries for the requests.
         retries_connect: Number of connect retries for the requests.
         backoff_factor: Backoff factor between retry attempts.
 
     """
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        base_url: Optional[str] = None,
         user_email: Optional[str] = None,
+        api_key: Optional[str] = None,
         refresh_token: Optional[str] = None,
+        base_url: Optional[str] = None,
         retries_total: int = 5,
         retries_connect: int = 3,
         backoff_factor: float = 0.5,
     ) -> None:
         super().__init__()
 
-        self.base_url = base_url
         self.user_email = user_email
+        self.api_key = api_key
         self.refresh_token = refresh_token
+        self.base_url = base_url
         self.verify = False
 
         self._initialize_retry(retries_total, retries_connect, backoff_factor)
 
     def __del__(self) -> None:
         """qbraid session destructor. Closes the session."""
         self.close()
@@ -74,40 +77,53 @@
     def base_url(self) -> Optional[str]:
         """Return the qbraid api url."""
         return self._base_url
 
     @base_url.setter
     def base_url(self, value: Optional[str]) -> None:
         """Set the qbraid api url."""
-        url = value if value else self.get_config_variable("url")
-        self._base_url = url if url else DEFAULT_ENDPOINT_URL
+        url = value or self.get_config_variable("url")
+        self._base_url = url or DEFAULT_ENDPOINT_URL
 
     @property
     def user_email(self) -> Optional[str]:
         """Return the session user email."""
         return self._user_email
 
     @user_email.setter
     def user_email(self, value: Optional[str]) -> None:
         """Set the session user email."""
-        user_email = value if value else self.get_config_variable("email")
-        self._user_email = user_email if user_email else os.getenv("JUPYTERHUB_USER")
+        user_email = value or self.get_config_variable("email")
+        self._user_email = user_email or os.getenv("JUPYTERHUB_USER")
         if user_email:
             self.headers.update({"email": user_email})  # type: ignore[attr-defined]
 
     @property
+    def api_key(self) -> Optional[str]:
+        """Return the api key."""
+        return self._api_key
+
+    @api_key.setter
+    def api_key(self, value: Optional[str]) -> None:
+        """Set the api key."""
+        api_key = value or self.get_config_variable("api-key")
+        self._api_key = api_key or os.getenv("QBRAID_API_KEY")
+        if api_key:
+            self.headers.update({"api-key": api_key})  # type: ignore[attr-defined]
+
+    @property
     def refresh_token(self) -> Optional[str]:
         """Return the session refresh token."""
         return self._refresh_token
 
     @refresh_token.setter
     def refresh_token(self, value: Optional[str]) -> None:
         """Set the session refresh token."""
-        refresh_token = value if value else self.get_config_variable("refresh-token")
-        self._refresh_token = refresh_token if refresh_token else os.getenv("REFRESH")
+        refresh_token = value or self.get_config_variable("refresh-token")
+        self._refresh_token = refresh_token or os.getenv("REFRESH")
         if refresh_token:
             self.headers.update({"refresh-token": refresh_token})  # type: ignore[attr-defined]
 
     def get_config_variable(self, config_name: str) -> Optional[str]:
         """Returns the config value of specified config.
 
         Args:
@@ -122,45 +138,69 @@
                 if config_name in config[section]:
                     return config[section][config_name]
         return None
 
     def save_config(
         self,
         user_email: Optional[str] = None,
+        api_key: Optional[str] = None,
         refresh_token: Optional[str] = None,
         base_url: Optional[str] = None,
     ) -> None:
         """Create qbraidrc file. In qBraid Lab, qbraidrc is automatically present in filesystem.
 
         Args:
             user_email:  JupyterHub User.
+            api_key: Authenticated qBraid api-key.
             refresh_token: Authenticated qBraid refresh-token.
             base_url: Base URL for the session's requests.
         """
-        self.user_email = user_email if user_email else self.user_email
-        self.refresh_token = refresh_token if refresh_token else self.refresh_token
-        self.base_url = base_url if base_url else self.base_url
-
-        res = self.get("/identity")
+        self.user_email = user_email or self.user_email
+        self.api_key = api_key or self.api_key
+        self.refresh_token = refresh_token or self.refresh_token
+        self.base_url = base_url or self.base_url
 
-        if res.status_code != 200 or self.user_email != res.json()["email"]:
-            raise AuthError("Invalid qBraid API credentials")
+        try:
+            res = self.get("/identity")
+        except RequestsApiError as err:
+            raise AuthError from err
+
+        res_json = res.json()
+
+        if res.status_code != 200:
+            raise AuthError(f"{res.status_code} Client Error: Invalid qBraid API credentials")
+
+        res_email = res_json.get("email")
+
+        if self.user_email:
+            if self.user_email != res_email:
+                raise AuthError(
+                    f"Credential mismatch: Session initialized for '{self.user_email}', \
+                        but API key corresponds to '{res_email}'."
+                )
+        else:
+            self.user_email = res_email
 
         try:
             filepath = DEFAULT_CONFIG_PATH
+
             if not os.path.isfile(filepath):
                 os.makedirs(os.path.dirname(filepath), exist_ok=True)
             config = configparser.ConfigParser()
-            config.read(filepath)
             section = DEFAULT_CONFIG_SECTION
             if section not in config.sections():
                 config.add_section(section)
-            config.set(section, "email", self.user_email)
-            config.set(section, "refresh-token", self.refresh_token)
-            config.set(section, "url", self.base_url)
+            if self.user_email:
+                config.set(section, "email", self.user_email)
+            if self.api_key:
+                config.set(section, "api-key", self.api_key)
+            if self.refresh_token:
+                config.set(section, "refresh-token", self.refresh_token)
+            if self.base_url:
+                config.set(section, "url", self.base_url)
             with open(filepath, "w", encoding="utf-8") as cfgfile:
                 config.write(cfgfile)
         except Exception as err:
             raise ConfigError from err
 
     def _email_converter(self) -> Optional[str]:
         """Convert email to compatible string format"""
```

### Comparing `qbraid-0.3.0/qbraid/api/tests/test_api_config.py` & `qbraid-0.4.0/qbraid/api/tests/test_api_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 """
 import configparser
 import os
 
 import pytest
 from qiskit_ibm_provider import IBMProvider
 
-from qbraid.api.exceptions import RequestsApiError
+from qbraid.api.exceptions import AuthError, RequestsApiError
 from qbraid.api.session import QbraidSession
 
 aws_cred_path = os.path.join(os.path.expanduser("~"), ".aws", "credentials")
 aws_config_path = os.path.join(os.path.expanduser("~"), ".aws", "config")
 qiskitrc_path = os.path.join(os.path.expanduser("~"), ".qiskit", "qiskitrc")
 qbraidrc_path = os.path.join(os.path.expanduser("~"), ".qbraid", "qbraidrc")
 
 # These environment variables don't actually exist in qBraid Lab, but instead
 # are set and used for convenience for local development and testing.
 aws_access_key_id = os.getenv("AWS_ACCESS_KEY_ID")
 aws_secret_access_key = os.getenv("AWS_SECRET_ACCESS_KEY")
 ibmq_token = os.getenv("QISKIT_IBM_TOKEN")
-qbraid_token = os.getenv("REFRESH")
+qbraid_refresh_token = os.getenv("REFRESH")
+qbraid_api_key = os.getenv("QBRAID_API_KEY")
 
 # This is the only environment variable that actually exists in qBraid Lab
 qbraid_user = os.getenv("JUPYTERHUB_USER")
 
 config_lst = [
     # (config_name, config_value, section, filepath)
     ["aws_access_key_id", aws_access_key_id, "default", aws_cred_path],
@@ -93,13 +94,27 @@
     """Test initializing QbraidSession with attributes set from user-provided values."""
     refresh_token = "test123"
     session = QbraidSession(refresh_token=refresh_token)
     assert session.refresh_token == refresh_token
     del session
 
 
+def test_qbraid_session_api_key():
+    """Test initializing QbraidSession without args and then saving config."""
+    session = QbraidSession()
+    session.save_config(api_key=qbraid_api_key, user_email=qbraid_user)
+    assert session.get_config_variable("api-key") == qbraid_api_key
+
+
 def test_qbraid_session_save_config():
     """Test initializing QbraidSession without args and then saving config."""
     session = QbraidSession()
-    session.save_config(user_email=qbraid_user, refresh_token=qbraid_token)
+    session.save_config(user_email=qbraid_user, refresh_token=qbraid_refresh_token)
     assert session.get_config_variable("email") == qbraid_user
-    assert session.get_config_variable("refresh-token") == qbraid_token
+    assert session.get_config_variable("refresh-token") == qbraid_refresh_token
+
+
+def test_qbraid_session_credential_mismatch_error():
+    """Test initializing QbraidSession with mismatched email and apiKey."""
+    session = QbraidSession(api_key=qbraid_api_key, user_email="fakeuser@email.com")
+    with pytest.raises(AuthError):
+        session.save_config()
```

### Comparing `qbraid-0.3.0/qbraid/api/tests/test_api_thirdparty.py` & `qbraid-0.4.0/qbraid/api/tests/test_api_thirdparty.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/__init__.py` & `qbraid-0.4.0/qbraid/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/aws/__init__.py` & `qbraid-0.4.0/qbraid/devices/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/aws/device.py` & `qbraid-0.4.0/qbraid/devices/aws/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/aws/job.py` & `qbraid-0.4.0/qbraid/devices/aws/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/aws/result.py` & `qbraid-0.4.0/qbraid/devices/aws/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/device.py` & `qbraid-0.4.0/qbraid/devices/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/enums.py` & `qbraid-0.4.0/qbraid/devices/enums.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/exceptions.py` & `qbraid-0.4.0/qbraid/devices/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/ibm/__init__.py` & `qbraid-0.4.0/qbraid/devices/ibm/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/ibm/device.py` & `qbraid-0.4.0/qbraid/devices/ibm/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/ibm/job.py` & `qbraid-0.4.0/qbraid/devices/ibm/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/ibm/provider.py` & `qbraid-0.4.0/qbraid/devices/ibm/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/ibm/result.py` & `qbraid-0.4.0/qbraid/devices/ibm/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/ibm/tests/test_ibm_provider.py` & `qbraid-0.4.0/qbraid/devices/ibm/tests/test_ibm_provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/job.py` & `qbraid-0.4.0/qbraid/devices/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/result.py` & `qbraid-0.4.0/qbraid/devices/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/status_maps.py` & `qbraid-0.4.0/qbraid/devices/status_maps.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/tests/test_devices.py` & `qbraid-0.4.0/qbraid/devices/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/tests/test_enums.py` & `qbraid-0.4.0/qbraid/devices/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/devices/tests/test_results.py` & `qbraid-0.4.0/qbraid/devices/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/display_utils.py` & `qbraid-0.4.0/qbraid/display_utils.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/exceptions.py` & `qbraid-0.4.0/qbraid/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,7 +33,11 @@
 
 class ProgramTypeError(QbraidError):
     """Class for errors raised when processing unsupported quantum programs"""
 
     def __init__(self, program):
         msg = f"Quantum program of type {type(program)} is not supported."
         super().__init__(msg)
+
+
+class VisualizationError(QbraidError):
+    """Class for errors raised when using visualization features."""
```

### Comparing `qbraid-0.3.0/qbraid/get_devices.py` & `qbraid-0.4.0/qbraid/get_devices.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/get_jobs.py` & `qbraid-0.4.0/qbraid/get_jobs.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/__init__.py` & `qbraid-0.4.0/qbraid/interface/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,21 @@
    :toctree: ../stubs/
 
    to_unitary
    unitary_to_little_endian
    convert_to_contiguous
    circuits_allclose
    random_circuit
-   draw
+   circuit_drawer
    ContiguousConversionError
    UnitaryCalculationError
 
 """
 from .calculate_unitary import (
     UnitaryCalculationError,
     circuits_allclose,
     to_unitary,
     unitary_to_little_endian,
 )
 from .convert_to_contiguous import ContiguousConversionError, convert_to_contiguous
-from .draw_circuit import draw
+from .draw import circuit_drawer
 from .programs import random_circuit
```

### Comparing `qbraid-0.3.0/qbraid/interface/calculate_unitary.py` & `qbraid-0.4.0/qbraid/interface/calculate_unitary.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,21 @@
         UnitaryCalculationError: If the programs unitary could not be calculated.
 
     Returns:
         Matrix representation of the input quantum program.
     """
     to_unitary_function: Callable[[Any], np.ndarray]
 
-    try:
-        package = program.__module__
-    except AttributeError as err:
-        raise ProgramTypeError(program) from err
+    if isinstance(program, str):
+        package = "qasm"
+    else:
+        try:
+            package = program.__module__
+        except AttributeError as err:
+            raise ProgramTypeError(program) from err
 
     # pylint: disable=import-outside-toplevel
 
     if "qiskit" in package:
         from qbraid.interface.qbraid_qiskit.tools import _unitary_from_qiskit
 
         to_unitary_function = _unitary_from_qiskit
@@ -68,14 +71,18 @@
         from qbraid.interface.qbraid_pyquil.tools import _unitary_from_pyquil
 
         to_unitary_function = _unitary_from_pyquil
     elif "pytket" in package:
         from qbraid.interface.qbraid_pytket.tools import _unitary_from_pytket
 
         to_unitary_function = _unitary_from_pytket
+    elif "qasm" in package:
+        from qbraid.interface.qbraid_qasm.tools import _unitary_from_qasm
+
+        to_unitary_function = _unitary_from_qasm
     else:
         raise ProgramTypeError(program)
 
     program_input = convert_to_contiguous(program) if ensure_contiguous else program
 
     try:
         unitary = to_unitary_function(program_input)
```

### Comparing `qbraid-0.3.0/qbraid/interface/convert_to_contiguous.py` & `qbraid-0.4.0/qbraid/interface/convert_to_contiguous.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,18 +40,21 @@
 
     Returns:
         :data:`~qbraid.QPROGRAM`: Program of the same type as the input quantum program.
 
     """
     conversion_function: Callable[[Any], QPROGRAM]
 
-    try:
-        package = program.__module__
-    except AttributeError as err:
-        raise ProgramTypeError(program) from err
+    if isinstance(program, str):
+        package = "qasm"
+    else:
+        try:
+            package = program.__module__
+        except AttributeError as err:
+            raise ProgramTypeError(program) from err
 
     # pylint: disable=import-outside-toplevel
 
     if "pyquil" in package:
         return program
 
     if "qiskit" in package:
@@ -66,14 +69,18 @@
         from qbraid.interface.qbraid_braket.tools import _convert_to_contiguous_braket
 
         conversion_function = _convert_to_contiguous_braket
     elif "pytket" in package:
         from qbraid.interface.qbraid_pytket.tools import _convert_to_contiguous_pytket
 
         conversion_function = _convert_to_contiguous_pytket
+    elif "qasm" in package:
+        from qbraid.interface.qbraid_qasm.tools import _convert_to_contiguous_qasm
+
+        conversion_function = _convert_to_contiguous_qasm
     else:
         raise ProgramTypeError(program)
 
     try:
         compat_program = conversion_function(program, **kwargs)
     except Exception as err:
         raise ContiguousConversionError(
```

### Comparing `qbraid-0.3.0/qbraid/interface/draw_circuit.py` & `qbraid-0.4.0/qbraid/transpiler/wrappers/pyquil_program.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,41 +5,32 @@
 # The qBraid-SDK is free software released under the GNU General Public License v3
 # or later. You can redistribute and/or modify it under the terms of the GPL v3.
 # See the LICENSE file in the project root or <https://www.gnu.org/licenses/gpl-3.0.html>.
 #
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
-Module for drawing quantum circuit diagrams
+Module defining PyQuilProgramWrapper Class
 
 """
-from typing import TYPE_CHECKING
+from pyquil import Program
 
-from qbraid.exceptions import ProgramTypeError
+from qbraid.transpiler.wrappers.abc_qprogram import QuantumProgramWrapper
 
-if TYPE_CHECKING:
-    import qbraid
 
+class PyQuilProgramWrapper(QuantumProgramWrapper):
+    """Wrapper class for pyQuil ``Program`` objects."""
 
-def draw(program: "qbraid.QPROGRAM") -> None:
-    """Draws circuit diagram.
+    def __init__(self, program: Program):
+        """Create a PyQuilProgramWrapper
 
-    Args:
-        :data:`~.qbraid.QPROGRAM`: Supported quantum program
+        Args:
+            program: the program object to be wrapped
 
-    Raises:
-        ProgramTypeError: If quantum program is not of a supported type
-    """
-    # todo: visualization from supportive framework
-    try:
-        package = program.__module__
-    except AttributeError as err:
-        raise ProgramTypeError(program) from err
+        """
+        super().__init__(program)
 
-    if "qiskit" in package:
-        print(program.draw())
-
-    elif "braket" in package or "cirq" in package or "pyquil" in package:
-        print(program)
-
-    else:
-        raise ProgramTypeError(program)
+        self._qubits = program.get_qubits()
+        self._num_qubits = len(self.qubits)
+        self._depth = len(program)
+        self._package = "pyquil"
+        self._program_type = "Program"
```

### Comparing `qbraid-0.3.0/qbraid/interface/programs.py` & `qbraid-0.4.0/qbraid/interface/programs.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,43 +31,47 @@
 
 def bell_data() -> QROGRAM_TEST_TYPE:
     """Returns bell circuit/program in each supported package."""
     from qbraid.interface.qbraid_braket.circuits import braket_bell
     from qbraid.interface.qbraid_cirq.circuits import cirq_bell
     from qbraid.interface.qbraid_pyquil.programs import pyquil_bell
     from qbraid.interface.qbraid_pytket.circuits import pytket_bell
+    from qbraid.interface.qbraid_qasm.circuits import qasm_bell
     from qbraid.interface.qbraid_qiskit.circuits import qiskit_bell
 
     unitary = to_unitary(cirq_bell())
 
     circuits = {
         "braket": braket_bell,
         "cirq": cirq_bell,
         "pyquil": pyquil_bell,
         "qiskit": qiskit_bell,
         "pytket": pytket_bell,
+        "qasm": qasm_bell,
     }
 
     return circuits, unitary
 
 
 def shared15_data() -> QROGRAM_TEST_TYPE:
     """Returns shared gates circuit/program in each supported package."""
     from qbraid.interface.qbraid_braket.circuits import braket_shared15
     from qbraid.interface.qbraid_cirq.circuits import cirq_shared15
     from qbraid.interface.qbraid_pytket.circuits import pytket_shared15
+    from qbraid.interface.qbraid_qasm.circuits import qasm_shared15
     from qbraid.interface.qbraid_qiskit.circuits import qiskit_shared15
 
     unitary = to_unitary(cirq_shared15())
 
     circuits = {
         "braket": braket_shared15,
         "cirq": cirq_shared15,
         "qiskit": qiskit_shared15,
         "pytket": pytket_shared15,
+        "qasm": qasm_shared15,
     }
 
     return circuits, unitary
 
 
 def random_circuit(
     package: str, num_qubits: Optional[int] = None, depth: Optional[int] = None, **kwargs
```

### Comparing `qbraid-0.3.0/qbraid/interface/qbraid_braket/circuits.py` & `qbraid-0.4.0/qbraid/interface/qbraid_braket/circuits.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/qbraid_braket/tools.py` & `qbraid-0.4.0/qbraid/interface/qbraid_braket/tools.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/qbraid_cirq/_utils.py` & `qbraid-0.4.0/qbraid/interface/qbraid_cirq/_utils.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/qbraid_cirq/circuits.py` & `qbraid-0.4.0/qbraid/interface/qbraid_cirq/circuits.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/qbraid_cirq/tests/test_cirq_utils.py` & `qbraid-0.4.0/qbraid/interface/qbraid_cirq/tests/test_cirq_utils.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/qbraid_cirq/tools.py` & `qbraid-0.4.0/qbraid/interface/qbraid_cirq/tools.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/qbraid_pyquil/programs.py` & `qbraid-0.4.0/qbraid/interface/qbraid_pyquil/programs.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/qbraid_pyquil/tools.py` & `qbraid-0.4.0/qbraid/interface/qbraid_pyquil/tools.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/qbraid_pytket/circuits.py` & `qbraid-0.4.0/qbraid/interface/qbraid_pytket/circuits.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/qbraid_pytket/tools.py` & `qbraid-0.4.0/qbraid/interface/qbraid_pytket/tools.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/qbraid_qiskit/circuits.py` & `qbraid-0.4.0/qbraid/interface/qbraid_qiskit/circuits.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/qbraid_qiskit/tools.py` & `qbraid-0.4.0/qbraid/interface/qbraid_qiskit/tools.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/interface/tests/test_calculate_unitary.py` & `qbraid-0.4.0/qbraid/interface/tests/test_calculate_unitary.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import numpy as np
 import pytest
 from braket.circuits import Circuit, Instruction, gates
 from pytket.circuit import Circuit as TKCircuit
 from pytket.circuit import OpType
 
+from qbraid.exceptions import ProgramTypeError
 from qbraid.interface.calculate_unitary import to_unitary, unitary_to_little_endian
 from qbraid.interface.convert_to_contiguous import convert_to_contiguous
 
 
 def get_subsets(nqubits):
     """Return list of all combinations up to number nqubits"""
     qubits = list(range(0, nqubits))
@@ -106,7 +107,20 @@
     c_unitary = _gate_to_matrix_pytket(
         gates=c.get_commands()[0] if list_type else c.get_commands(), flat=flat
     )
     if flat:
         assert c_unitary.shape[0] == 2**2
     else:
         assert c_unitary.shape[0] == 2**4
+
+
+def test_qasm_depth():
+    from qbraid.interface.qbraid_qasm.circuits import qasm_bell, qasm_shared15
+    from qbraid.interface.qbraid_qasm.tools import qasm_depth
+
+    assert qasm_depth(qasm_bell()) == 2
+    assert qasm_depth(qasm_shared15()) == 22
+
+
+def test_unitary_raises():
+    with pytest.raises(ProgramTypeError):
+        to_unitary(None)
```

### Comparing `qbraid-0.3.0/qbraid/interface/tests/test_convert_to_contiguous.py` & `qbraid-0.4.0/qbraid/interface/tests/test_convert_to_contiguous.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 # THERE IS NO WARRANTY for the qBraid-SDK, as per Section 15 of the GPL v3.
 
 """
 Unit tests for the qbraid convert_to_contiguous interfacing
 
 """
 import numpy as np
+import pytest
 from braket.circuits import Circuit as BKCircuit
 from cirq import Circuit, LineQubit, X, Y, Z
 from pytket.circuit import Circuit as TKCircuit
 from qiskit import QuantumCircuit
 
+from qbraid.exceptions import ProgramTypeError
 from qbraid.interface.calculate_unitary import circuits_allclose
 from qbraid.interface.convert_to_contiguous import convert_to_contiguous
 
 
 def test_remove_idle_qubits_qiskit():
     """Test convert_to_contigious on qiskit circuit"""
     circuit = QuantumCircuit(3)
@@ -77,7 +79,12 @@
 
 def test_remove_blank_wires_pytket():
     circuit = TKCircuit(3)
     circuit.H(0)
     circuit.CX(0, 1)
     contig_circuit = convert_to_contiguous(circuit)
     assert contig_circuit.n_qubits == 2
+
+
+def test_unitary_raises():
+    with pytest.raises(ProgramTypeError):
+        convert_to_contiguous(None)
```

### Comparing `qbraid-0.3.0/qbraid/tests/test_top_level.py` & `qbraid-0.4.0/qbraid/tests/test_top_level.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/__init__.py` & `qbraid-0.4.0/qbraid/transpiler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,21 @@
    convert_to_cirq
    QuantumProgramWrapper
    BraketCircuitWrapper
    CirqCircuitWrapper
    PyQuilProgramWrapper
    QiskitCircuitWrapper
    PytketCircuitWrapper
+   QasmCircuitWrapper
    CircuitConversionError
    QasmError
 
 """
 from qbraid.transpiler.conversions import convert_from_cirq, convert_to_cirq
 from qbraid.transpiler.exceptions import CircuitConversionError, QasmError
 from qbraid.transpiler.wrappers.abc_qprogram import QuantumProgramWrapper
 from qbraid.transpiler.wrappers.braket_circuit import BraketCircuitWrapper
 from qbraid.transpiler.wrappers.cirq_circuit import CirqCircuitWrapper
 from qbraid.transpiler.wrappers.pyquil_program import PyQuilProgramWrapper
 from qbraid.transpiler.wrappers.pytket_circuit import PytketCircuitWrapper
+from qbraid.transpiler.wrappers.qasm_str import QasmCircuitWrapper
 from qbraid.transpiler.wrappers.qiskit_circuit import QiskitCircuitWrapper
```

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_braket/__init__.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_braket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_braket/convert_from_braket.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_braket/convert_from_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_braket/convert_from_braket_qasm.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_braket/convert_from_braket_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_braket/convert_to_braket.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_braket/convert_to_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_braket/custom_gates.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_braket/custom_gates.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_braket/tests/_gate_archive.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/_gate_archive.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_braket/tests/test_from_braket.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_from_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_braket/tests/test_from_braket_qasm.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_from_braket_qasm.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_braket/tests/test_to_braket.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_to_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_braket/tests/test_to_braket_measure.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_braket/tests/test_to_braket_measure.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_pyquil/__init__.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_pyquil/conversions.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_pyquil/tests/test_conversions_pyquil.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_pyquil/tests/test_conversions_pyquil.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_pytket/__init__.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_pytket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_pytket/conversions.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_pytket/conversions.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 """
 from cirq import Circuit
 from pytket.circuit import Circuit as TKCircuit
 from pytket.qasm import circuit_from_qasm_str, circuit_to_qasm_str
 
 from qbraid.interface import convert_to_contiguous
-from qbraid.interface.qbraid_cirq.tools import _convert_to_line_qubits
 from qbraid.transpiler.cirq_qasm import from_qasm, to_qasm
 from qbraid.transpiler.custom_gates import _map_zpow_and_unroll
 from qbraid.transpiler.exceptions import CircuitConversionError
 
 
 def to_pytket(circuit: Circuit) -> TKCircuit:
     """Returns a pytket circuit equivalent to the input Cirq circuit. Note
@@ -39,22 +38,24 @@
         contig_circuit = convert_to_contiguous(circuit, rev_qubits=False)
         compat_circuit = _map_zpow_and_unroll(contig_circuit)
         return circuit_from_qasm_str(to_qasm(compat_circuit))
     except ValueError as err:
         raise CircuitConversionError("Cirq qasm converter doesn't yet support qasm3.") from err
 
 
-def from_pytket(circuit: TKCircuit) -> Circuit:
+def from_pytket(circuit: TKCircuit, compat=False) -> Circuit:
     """Returns a Cirq circuit equivalent to the input pytket circuit.
 
     Args:
         circuit: pytket circuit to convert to a Cirq circuit.
 
     Returns:
         Cirq circuit representation equivalent to the input pytket circuit.
     """
     try:
         qasm_str = circuit_to_qasm_str(circuit)
         cirq_circuit = from_qasm(qasm_str)
-        return _convert_to_line_qubits(cirq_circuit, rev_qubits=False)
+        if compat:
+            cirq_circuit = convert_to_contiguous(cirq_circuit, rev_qubits=True)
+        return cirq_circuit
     except Exception as err:
         raise CircuitConversionError("Cirq qasm converter doesn't yet support qasm3.") from err
```

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_pytket/tests/test_conversions_pytket.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/test_conversions_pytket.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pytket.circuit import Circuit as TKCircuit
 from pytket.qasm import circuit_to_qasm_str
 
 from qbraid.interface import circuits_allclose
 from qbraid.interface.qbraid_cirq._utils import _equal
 from qbraid.transpiler.cirq_pytket.conversions import from_pytket, to_pytket
 from qbraid.transpiler.cirq_qasm import from_qasm
+from qbraid.transpiler.exceptions import CircuitConversionError
 
 
 def test_bell_state_to_from_circuits():
     """Tests cirq.Circuit --> pytket.circuit.Circuit --> cirq.Circuit
     with a Bell state circuit.
     """
     qreg = LineQubit.range(2)
```

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_pytket/tests/test_from_pytket.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/test_from_pytket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_pytket/tests/test_to_pytket.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_pytket/tests/test_to_pytket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qasm/__init__.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qasm/qasm_conversions.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/qasm_conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qasm/qasm_parser.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/qasm_parser.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qasm/qasm_preprocess.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/qasm_preprocess.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qasm/tests/_gate_archive.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/_gate_archive.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qasm/tests/test_qasm_parser.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/test_qasm_parser.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qasm/tests/test_qasm_preprocess.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qasm/tests/test_qasm_preprocess.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/__init__.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/conversions.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/tests/_gate_archive.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/_gate_archive.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/tests/test_conversions_qiskit.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/test_conversions_qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/tests/test_from_qiskit.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/test_from_qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/cirq_qiskit/tests/test_to_qiskit.py` & `qbraid-0.4.0/qbraid/transpiler/cirq_qiskit/tests/test_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/code/__init__.py` & `qbraid-0.4.0/qbraid/transpiler/code/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/code/qasm_to_braket.py` & `qbraid-0.4.0/qbraid/transpiler/code/qasm_to_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/code/tests/test_qasm_to_braket.py` & `qbraid-0.4.0/qbraid/transpiler/code/tests/test_qasm_to_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/conversions.py` & `qbraid-0.4.0/qbraid/transpiler/conversions.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,19 +14,22 @@
 Module containing functions for converting to/from Cirq's circuit representation.
 
 """
 from typing import TYPE_CHECKING, Tuple
 
 from cirq import Circuit
 from cirq.contrib.qasm_import import circuit_from_qasm
+from cirq.contrib.qasm_import.exception import QasmException
 
 from qbraid.exceptions import PackageValueError, ProgramTypeError
 from qbraid.transpiler.cirq_braket import from_braket, to_braket
 from qbraid.transpiler.cirq_pyquil import from_pyquil, to_pyquil
 from qbraid.transpiler.cirq_pytket import from_pytket, to_pytket
+from qbraid.transpiler.cirq_qasm import from_qasm, to_qasm
+from qbraid.transpiler.cirq_qasm.qasm_parser import QasmParser
 from qbraid.transpiler.cirq_qiskit import from_qiskit, to_qiskit
 from qbraid.transpiler.exceptions import CircuitConversionError
 
 if TYPE_CHECKING:
     import qbraid
 
 
@@ -40,33 +43,42 @@
         ProgramTypeError: If the input quantum program is not supported.
         CircuitConversionError: If the input quantum program could not be converted.
 
     Returns:
         A Tuple containing the Cirq circuit equivalent to input circuit and the
             input quantum program type.
     """
-
-    try:
-        package = program.__module__
-    except AttributeError as err:
-        raise ProgramTypeError(program) from err
+    if isinstance(program, str):
+        try:
+            QasmParser().parse(program)
+            package = "qasm"
+        except QasmException as err:
+            raise CircuitConversionError("Qbraid only support qasm string.") from err
+    else:
+        try:
+            package = program.__module__
+        except AttributeError as err:
+            raise ProgramTypeError(program) from err
 
     try:
         if "qiskit" in package:
             return from_qiskit(program), "qiskit"
 
         if "pyquil" in package:
             return from_pyquil(program), "pyquil"
 
         if "braket" in package:
             return from_braket(program), "braket"
 
         if "pytket" in package:
             return from_pytket(program), "pytket"
 
+        if "qasm" in package:
+            return from_qasm(program), "qasm"
+
         if isinstance(program, Circuit):
             return program, "cirq"
 
     except Exception as err:
         raise CircuitConversionError(
             "Quantum program could not be converted to a Cirq circuit."
         ) from err
@@ -97,14 +109,17 @@
 
         if frontend == "braket":
             return to_braket(circuit)
 
         if frontend == "pytket":
             return to_pytket(circuit)
 
+        if frontend == "qasm":
+            return to_qasm(circuit)
+
         if frontend == "cirq":
             return circuit
 
     except Exception as err:
         raise CircuitConversionError(
             f"Cirq Circuit could not be converted to a " f"quantum program of type {frontend}."
         ) from err
```

### Comparing `qbraid-0.3.0/qbraid/transpiler/custom_gates.py` & `qbraid-0.4.0/qbraid/transpiler/custom_gates.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/exceptions.py` & `qbraid-0.4.0/qbraid/transpiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/tests/test_conversions.py` & `qbraid-0.4.0/qbraid/transpiler/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/tests/test_transpiler.py` & `qbraid-0.4.0/qbraid/transpiler/tests/test_transpiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,20 +86,26 @@
 )
 def test_to_cirq(circuit):
     converted_circuit, input_type = convert_to_cirq(circuit)
     assert _equal(converted_circuit, cirq_circuit) or _equal(converted_circuit, cirq_circuit_rev)
     assert input_type in circuit.__module__
 
 
-@pytest.mark.parametrize("item", ["circuit", 1, None])
+@pytest.mark.parametrize("item", [1, None])
 def test_to_cirq_bad_types(item):
     with pytest.raises(ProgramTypeError):
         convert_to_cirq(item)
 
 
+@pytest.mark.parametrize("item", ["DECLARE ro BIT[1]", "circuit"])
+def test_to_cirq_bad_string(item):
+    with pytest.raises(CircuitConversionError):
+        convert_to_cirq(item)
+
+
 @pytest.mark.parametrize("to_type", QPROGRAM_LIBS)
 def test_from_cirq(to_type):
     converted_circuit = convert_from_cirq(cirq_circuit, to_type)
     circuit, input_type = convert_to_cirq(converted_circuit)
     assert _equal(circuit, cirq_circuit)
     assert input_type == to_type
 
@@ -112,14 +118,20 @@
 
 def test_circuit_wrapper_error():
     """Test raising circuit wrapper error"""
     with pytest.raises(QbraidError):
         circuit_wrapper("Not a circuit")
 
 
+def test_circuit_wrapper_error():
+    """Test raising circuit wrapper error"""
+    with pytest.raises(QbraidError):
+        circuit_wrapper(None)
+
+
 def test_transpile_package_error():
     """Test raising circuit wrapper error"""
     circuit = TEST_BELL["braket"]()
     wrapped = circuit_wrapper(circuit)
     with pytest.raises(PackageValueError):
         wrapped.transpile("Not a package")
```

### Comparing `qbraid-0.3.0/qbraid/transpiler/wrappers/abc_qprogram.py` & `qbraid-0.4.0/qbraid/transpiler/wrappers/abc_qprogram.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 Module defining QuantumProgramWrapper Class
 
 """
 from typing import TYPE_CHECKING, List, Optional
 
 from qbraid._qprogram import QPROGRAM_LIBS, QPROGRAM_TYPES
 from qbraid.exceptions import PackageValueError
+from qbraid.interface.draw import circuit_drawer
 from qbraid.transpiler.conversions import convert_from_cirq, convert_to_cirq
 from qbraid.transpiler.exceptions import CircuitConversionError
 
 if TYPE_CHECKING:
     import qbraid
 
 
@@ -121,7 +122,11 @@
                     f"Circuit could not be converted from a Cirq type to a "
                     f"circuit of type {conversion_type}."
                 ) from err
 
             return converted_program
 
         raise PackageValueError(conversion_type)
+
+    def draw(self, package: str = "cirq", output: Optional[str] = None, **kwrags):
+        """draw circuit"""
+        return circuit_drawer(self.transpile(package), output, **kwrags)
```

### Comparing `qbraid-0.3.0/qbraid/transpiler/wrappers/braket_circuit.py` & `qbraid-0.4.0/qbraid/transpiler/wrappers/braket_circuit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/wrappers/cirq_circuit.py` & `qbraid-0.4.0/qbraid/transpiler/wrappers/cirq_circuit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/wrappers/pytket_circuit.py` & `qbraid-0.4.0/qbraid/transpiler/wrappers/pytket_circuit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/transpiler/wrappers/qiskit_circuit.py` & `qbraid-0.4.0/qbraid/transpiler/wrappers/qiskit_circuit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/qbraid/wrappers.py` & `qbraid-0.4.0/qbraid/wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 """
 Module containing top-level qbraid wrapper functionality. Each of these
 functions utilize entrypoints via ``pkg_resources``.
 
 """
 import pkg_resources
+from cirq.contrib.qasm_import.exception import QasmException
+
+from qbraid.transpiler.cirq_qasm.qasm_parser import QasmParser
 
 from ._qprogram import QPROGRAM
 from .api import QbraidSession
 from .exceptions import QbraidError
 
 
 def _get_entrypoints(group: str):
@@ -48,21 +51,28 @@
     Returns:
         :class:`~qbraid.transpiler.QuantumProgramWrapper`: A wrapped quantum circuit-like object
 
     Raises:
         :class:`~qbraid.QbraidError`: If the input circuit is not a supported quantum program.
 
     """
-    try:
-        package = program.__module__.split(".")[0]
-    except AttributeError as err:
-        raise QbraidError(
-            f"Error applying circuit wrapper to quantum program \
-            of type {type(program)}"
-        ) from err
+    if isinstance(program, str):
+        try:
+            QasmParser().parse(program)
+            package = "qasm"
+        except QasmException as err:
+            raise QbraidError("Qbraid currently only support qasm string.") from err
+    else:
+        try:
+            package = program.__module__.split(".")[0]
+        except AttributeError as err:
+            raise QbraidError(
+                f"Error applying circuit wrapper to quantum program \
+                of type {type(program)}"
+            ) from err
 
     ep = package.lower()
 
     transpiler_entrypoints = _get_entrypoints("qbraid.transpiler")
 
     if package in transpiler_entrypoints:
         circuit_wrapper_class = transpiler_entrypoints[ep].load()
```

### Comparing `qbraid-0.3.0/qbraid.egg-info/PKG-INFO` & `qbraid-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python toolkit for cross-framework abstraction of quantum programs.
 Home-page: https://github.com/qBraid/qBraid/
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
 License: Restricted
 Keywords: qbraid,quantum
 Classifier: Intended Audience :: Developers
@@ -20,68 +20,102 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 <img width=full alt="qbraid-sdk-header" src="https://user-images.githubusercontent.com/46977852/224456452-605e51f2-193d-4789-863e-e51cdd4b0a54.png">
 
-[![CI](https://github.com/qBraid/qBraid/actions/workflows/main.yml/badge.svg)](https://github.com/qBraid/qBraid/actions/workflows/main.yml)
+[![CI](https://github.com/qBraid/qBraid/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/qBraid/qBraid/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/qBraid/qBraid/branch/main/graph/badge.svg?token=1UTM0XZB7A)](https://codecov.io/gh/qBraid/qBraid)
 [![Documentation Status](https://readthedocs.com/projects/qbraid-qbraid/badge/?version=latest)](https://docs.qbraid.com/en/latest/?badge=latest)
+[![PyPI version](https://img.shields.io/pypi/v/qbraid.svg?color=blue)](https://pypi.org/project/qbraid/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-The qBraid-SDK is a Python toolkit for cross-framework abstraction, transpilation, and execution of quantum programs.
+The qBraid-SDK is a Python toolkit for cross-framework abstraction,
+transpilation, and execution of quantum programs.
 
 [<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png" width="150">](https://account.qbraid.com?gitHubUrl=https://github.com/qBraid/qBraid.git)
 
-
 ## Features
 
-- Unified quantum frontend interface. **Transpile** quantum circuits between supported packages. Leverage the capabilities of multiple frontends through **simple, consistent protocols**.
-- Build once, target many. **Create** quantum programs using your preferred circuit-building package, and **execute** on any backend that interfaces with a supported frontend.
-- Benchmark, compare, interpret results. Built-in **compatible** post-processing enables comparing results between runs and **across backends**.
-
+- Unified quantum frontend interface. **Transpile** quantum circuits between
+  supported packages. Leverage the capabilities of multiple frontends through
+  **simple, consistent protocols**.
+- Build once, target many. **Create** quantum programs using your preferred
+  circuit-building package, and **execute** on any backend that interfaces with
+  a supported frontend.
+- Benchmark, compare, interpret results. Built-in **compatible** post-processing
+  enables comparing results between runs and **across backends**.
+
+## Installation & Setup
+
+<img align="right" width="300" alt="qbraid-sdk-env" src="https://github.com/qBraid/qBraid/assets/46977852/669bd6f3-bbef-428c-9b59-b421c940262e">
+
+For the best experience, install the qBraid-SDK environment on
+[lab.qbraid.com](https://lab.qbraid.com). Login (or
+[create an account](https://account.qbraid.com)) and follow the steps to
+[install an environment](https://docs.qbraid.com/en/latest/lab/environments.html#install-environment).
+
+Using the SDK on qBraid Lab means direct, pre-configured access to all
+[Amazon Braket supported devices](https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html)
+and [IBM Quantum open systems](https://www.ibm.com/quantum/access-plans) with no
+additional access keys or API tokens required. See
+[qBraid Quantum Jobs](https://docs.qbraid.com/en/latest/lab/quantumjobs.html)
+for more.
 
-## Installation
-
-For the best experience, install the qBraid-SDK environment on [qBraid Lab](https://lab.qbraid.com). Login (or create an account) and then follow the steps to [install an environment](https://docs.qbraid.com/en/latest/lab/environments.html#install-environment).
+### Local install
 
 The qBraid-SDK, and all of its dependencies, can also be installed using pip:
 
 ```bash
 pip install qbraid
 ```
 
-## Quickstart
+If using locally, follow linked instructions to configure your
+[qBraid](#local-account-setup),
+[AWS](https://github.com/aws/amazon-braket-sdk-python#boto3-and-setting-up-aws-credentials),
+and [IBMQ](https://github.com/Qiskit/qiskit-ibm-provider#provider-setup)
+credentials.
+
+## Documentation & Tutorials
+
+qBraid documentation is available at
+[docs.qbraid.com](https://docs.qbraid.com/en/latest/).
+
+See also:
+
+- [API Reference](https://docs.qbraid.com/en/latest/api/qbraid.html)
+- [User Guide](https://docs.qbraid.com/en/latest/sdk/overview.html)
+- [Example Notebooks](https://github.com/qBraid/qbraid-lab-demo)
 
-For more in-depth examples, see [user guide](https://docs.qbraid.com/en/latest/sdk/overview.html) and [demo notebooks](https://github.com/qBraid/qbraid-lab-demo).
+## Quickstart
 
 ### Transpiler
 
-Construct a quantum program of any supported program type, 
+Construct a quantum program of any supported program type,
 
 ```python
 >>> from qbraid import QPROGRAM_LIBS
 >>> QPROGRAM_LIBS
-['braket', 'cirq', 'qiskit', 'pyquil', 'pytket']
+['braket', 'cirq', 'qiskit', 'pyquil', 'pytket', 'qasm']
 ```
 
 and use the `circuit_wrapper()` to convert to any other supported program type:
 
 ```python
 >>> from qbraid import circuit_wrapper
 >>> from qbraid.interface import random_circuit
 >>> qiskit_circuit = random_circuit("qiskit")
 >>> cirq_circuit = circuit_wrapper(qiskit_circuit).transpile("cirq")
 >>> print(qiskit_circuit)
           ┌────────────┐
 q_0: ──■──┤ Rx(3.0353) ├
      ┌─┴─┐└───┬────┬───┘
 q_1: ┤ H ├────┤ √X ├────
-     └───┘    └────┘    
+     └───┘    └────┘
 >>> print(cirq_circuit)
 0: ───H───X^0.5────────
       │
 1: ───@───Rx(0.966π)───
 ```
 
 ### Devices & Jobs
@@ -99,15 +133,16 @@
 aws_rigetti_aspen_m2                OFFLINE
 aws_rigetti_aspen_m3                ONLINE
 ibm_q_perth                         ONLINE
 ...
 
 ```
 
-Apply the `device_wrapper()`, and send quantum jobs to any supported backend, from any supported program type:
+Apply the `device_wrapper()`, and send quantum jobs to any supported backend,
+from any supported program type:
 
 ```python
 >>> from qbraid import device_wrapper, get_jobs
 >>> aws_device = device_wrapper("aws_oqc_lucy")
 >>> ibm_device = device_wrapper("ibm_q_perth")
 >>> aws_job = aws_device.run(qiskit_circuit, shots=1000)
 >>> ibm_job = ibm_device.run(cirq_circuit, shots=1000)
@@ -128,114 +163,92 @@
 >>> ibm_result = ibm_job.result()
 >>> aws_result.measurement_counts()
 {'00': 483, '01': 14, '10': 486, '11': 17}
 >>> ibm_result.measurement_counts()
 {'00': 496, '01': 12, '10': 479, '11': 13}
 ```
 
-## Local Setup
+## Local account setup
+<img mg align="right" width="350" alt="api_key" src="https://github.com/qBraid/qBraid/assets/32727721/d087c404-e9c7-4a0b-b2a5-a58f2e483cce">
+
 
-To use the qBraid-SDK locally (outside of qBraid Lab), you must add your account credentials:
+To use the qBraid-SDK locally (outside of qBraid Lab), you must add your account
+credentials:
 
-1. Create a qBraid account or log in to your existing account by visiting https://account.qbraid.com
-2. Copy your API (refresh) token from your qBraid account page:
-- Login to your account and open DevTools / inspector window (MacOS: Option-Command-I)
-- Go to Application -> Storage -> Cookies -> https://account.qbraid.com
-- The value corresponding to `REFRESH` is your API refresh token.
-  Note, this token is updated monthly.
-3. Take your account email and refresh token from step 2, and save it by calling `QbraidSession.save_config()`:
+1. Create a qBraid account or log in to your existing account by visiting
+   [account.qbraid.com](https://account.qbraid.com/v2)
+2. Copy your API Key token from the left side of
+    your [account page](https://account.qbraid.com/v2):
+
+3. Save your API key from step 2 by calling
+   `QbraidSession.save_config()`:
 
 ```python
 from qbraid.api import QbraidSession
 
-session = QbraidSession(user_email='USER_EMAIL', refresh_token='REFRESH_TOKEN')
+session = QbraidSession(api_key='API_KEY')
 session.save_config()
 ```
 
-The command above stores your credentials locally in a configuration file called `qbraidrc` in `$HOME/.qbraid`, where `$HOME` is your home directory. Once saved you can then connect to the qBraid API and leverage functions such as `get_devices()` and `get_jobs()`.
+The command above stores your credentials locally in a configuration file `~/.qbraid/qbraidrc`,
+where `~` corresponds to your home (`$HOME`) directory. Once saved, you can then connect to the
+qBraid API and leverage functions such as `get_devices()` and `get_jobs()`.
 
 ### Load Account from Environment Variables
 
-Alternatively, the qBraid-SDK can discover credentials from environment variables:
+Alternatively, the qBraid-SDK can discover credentials from environment
+variables:
 
 ```bash
 export JUPYTERHUB_USER='USER_EMAIL'
-export REFRESH='REFRESH_TOKEN'
+export QBRAID_API_KEY='QBRAID_API_KEY'
 ```
 
 Then instantiate the session without any arguments
 
 ```python
 from qbraid.api import QbraidSession
 
 session = QbraidSession()
 ```
 
-## Documentation
-
-The API reference can be found on [Read the Docs](https://docs.qbraid.com/en/latest/api/qbraid.html).
-
-To generate the API reference documentation locally:
-
-```bash
-pip install tox<4
-tox -e docs
-```
-
-Alternatively:
-```bash
-pip install -e ".[docs]"
-cd docs
-make html
-```
+## Launch on qBraid
 
-Both methods will run Sphinx in your shell. If the build results in an `InvocationError` due to a 
-duplicate object description, try `rm docs/stubs/*` to empty the old stubs directory, and then 
-re-start the build. If the build succeeds, it will say `The HTML pages are in build/html`. You can 
-view the generated documentation in your browser (on OS X) using:
+The "Launch on qBraid" button (below) can be added to any public GitHub
+repository. Clicking on it automaically opens qBraid Lab, and performs a
+`git clone` of the project repo into your account's home directory. Copy the
+code below, and replace `YOUR-USERNAME` and `YOUR-REPOSITORY` with your GitHub
+info.
 
-```bash
-open build/html/index.html
-```
+[<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png" width="150">](https://account.qbraid.com?gitHubUrl=https://github.com/qBraid/qBraid.git)
 
-You can also view it by running a web server in that directory:
+Use the badge in your project's `README.md`:
 
-```bash
-cd build/html
-python3 -m http.server
 ```
-Then open your browser to http://localhost:8000. If you make changes to the docs that aren't
-reflected in subsequent builds, run `make clean html`, which will force a full rebuild.
-
-## Testing
-
-To run all unit tests:
-
-```bash
-pip install tox<4
-tox -e unit-tests
+[<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png" width="150">](https://account.qbraid.com?gitHubUrl=https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git)
 ```
 
-You can also pass in various pytest arguments to run selected tests:
+Use the badge in your project's `README.rst`:
 
-```bash
-tox -e unit-tests -- {your-arguments}
 ```
-
-Alternatively:
-
-```bash
-pip install -e ".[test]"
-pytest {path-to-test}
+.. image:: https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png
+    :target: https://account.qbraid.com?gitHubUrl=https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
+    :width: 150px
 ```
 
-Running unit tests with tox will automatically generate a coverage report, which can be viewed by
-opening `tests/_coverage/index.html` in your browser.
+## Contributing
 
-To run linters and doc generators and unit tests:
-```bash
-tox
-```
+- Interested in contributing code, or making a PR? See
+  [CONTRIBUTING.md](CONTRIBUTING.md)
+- For feature requests and bug reports:
+  [Submit an issue](https://github.com/qBraid/qBraid/issues)
+- For discussions, and specific questions about the qBraid SDK, qBraid Lab, or
+  other topics, [join our discord community](https://discord.gg/gwBebaBZZX)
+- For questions that are more suited for a forum, use the `qbraid` tag on
+  [Stack Exchange](https://quantumcomputing.stackexchange.com/)
+- Want your open-source project featured as its own runtime environment on
+  qBraid Lab? Fill out our
+  [New Environment Request Form](https://forms.gle/a4v7Kdn7G7bs9jYD8)
 
 ## License
 
 [GNU General Public License v3.0](LICENSE)
```

### Comparing `qbraid-0.3.0/qbraid.egg-info/SOURCES.txt` & `qbraid-0.4.0/qbraid.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
@@ -48,14 +49,15 @@
 docs/_static/notebooks/kernel_nb.png
 docs/_static/notebooks/kernel_switch.png
 docs/_static/notebooks/share_notebook.png
 docs/_static/pkg-logos/braket.png
 docs/_static/pkg-logos/cirq.png
 docs/_static/pkg-logos/pyquil.png
 docs/_static/pkg-logos/pytket.png
+docs/_static/pkg-logos/qasm.png
 docs/_static/pkg-logos/qiskit.png
 docs/_static/pkg-logos/xanadu.png
 docs/_static/sdk-files/get_devices.png
 docs/_static/sdk-files/plot_counts.png
 docs/api/qbraid.api.rst
 docs/api/qbraid.devices.aws.rst
 docs/api/qbraid.devices.ibm.rst
@@ -135,15 +137,15 @@
 qbraid/devices/ibm/tests/test_ibm_provider.py
 qbraid/devices/tests/test_devices.py
 qbraid/devices/tests/test_enums.py
 qbraid/devices/tests/test_results.py
 qbraid/interface/__init__.py
 qbraid/interface/calculate_unitary.py
 qbraid/interface/convert_to_contiguous.py
-qbraid/interface/draw_circuit.py
+qbraid/interface/draw.py
 qbraid/interface/programs.py
 qbraid/interface/qbraid_braket/__init__.py
 qbraid/interface/qbraid_braket/circuits.py
 qbraid/interface/qbraid_braket/tools.py
 qbraid/interface/qbraid_cirq/__init__.py
 qbraid/interface/qbraid_cirq/_utils.py
 qbraid/interface/qbraid_cirq/circuits.py
@@ -151,14 +153,18 @@
 qbraid/interface/qbraid_cirq/tests/test_cirq_utils.py
 qbraid/interface/qbraid_pyquil/__init__.py
 qbraid/interface/qbraid_pyquil/programs.py
 qbraid/interface/qbraid_pyquil/tools.py
 qbraid/interface/qbraid_pytket/__init__.py
 qbraid/interface/qbraid_pytket/circuits.py
 qbraid/interface/qbraid_pytket/tools.py
+qbraid/interface/qbraid_qasm/__init__.py
+qbraid/interface/qbraid_qasm/circuits.py
+qbraid/interface/qbraid_qasm/tools.py
+qbraid/interface/qbraid_qasm/test/test_qasm_utils.py
 qbraid/interface/qbraid_qiskit/__init__.py
 qbraid/interface/qbraid_qiskit/circuits.py
 qbraid/interface/qbraid_qiskit/tools.py
 qbraid/interface/tests/test_calculate_unitary.py
 qbraid/interface/tests/test_convert_to_contiguous.py
 qbraid/interface/tests/test_programs.py
 qbraid/tests/test_top_level.py
@@ -204,8 +210,10 @@
 qbraid/transpiler/tests/test_transpiler.py
 qbraid/transpiler/wrappers/__init__.py
 qbraid/transpiler/wrappers/abc_qprogram.py
 qbraid/transpiler/wrappers/braket_circuit.py
 qbraid/transpiler/wrappers/cirq_circuit.py
 qbraid/transpiler/wrappers/pyquil_program.py
 qbraid/transpiler/wrappers/pytket_circuit.py
-qbraid/transpiler/wrappers/qiskit_circuit.py
+qbraid/transpiler/wrappers/qasm_str.py
+qbraid/transpiler/wrappers/qiskit_circuit.py
+tools/verify_headers.py
```

### Comparing `qbraid-0.3.0/setup.cfg` & `qbraid-0.4.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 packages = find:
 python_requires = >=3.9
 install_requires = 
-	amazon-braket-sdk~=1.38.0
+	amazon-braket-sdk~=1.38.1
 	cirq~=1.1.0
 	numpy>=1.17,<1.24
 	pyquil~=3.4.1
 	pytket<1.13.2
 	qiskit<0.43.0
 	qiskit-ibm-provider<0.5.3
 	requests~=2.30.0
@@ -47,14 +47,15 @@
 [options.entry_points]
 qbraid.transpiler = 
 	braket = qbraid.transpiler:BraketCircuitWrapper
 	cirq = qbraid.transpiler:CirqCircuitWrapper
 	pyquil = qbraid.transpiler:PyQuilProgramWrapper
 	qiskit = qbraid.transpiler:QiskitCircuitWrapper
 	pytket = qbraid.transpiler:PytketCircuitWrapper
+	qasm = qbraid.transpiler:QasmCircuitWrapper
 qbraid.devices = 
 	aws.device = qbraid.devices.aws:AwsDeviceWrapper
 	aws.job = qbraid.devices.aws:AwsQuantumTaskWrapper
 	ibm.device = qbraid.devices.ibm:IBMBackendWrapper
 	ibm.job = qbraid.devices.ibm:IBMJobWrapper
 
 [egg_info]
```

### Comparing `qbraid-0.3.0/setup.py` & `qbraid-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.3.0/tox.ini` & `qbraid-0.4.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tox]
-envlist = unit-tests, docs, linters
+envlist = unit-tests, docs, linters, format-check
 skip_missing_interpreter = true
 skipsdist = True
 
 [testenv]
 usedevelop = True
 basepython = python3
 deps = -r{toxinidir}/requirements.txt
 passenv =
     JUPYTERHUB_USER
     REFRESH
+    QBRAID_API_KEY
     AWS_ACCESS_KEY_ID
     AWS_SECRET_ACCESS_KEY
     QISKIT_IBM_TOKEN
 
 [testenv:unit-tests]
 description = Run pytests and generate coverage report.
 extras = 
@@ -44,15 +45,16 @@
 envdir = .tox/linters
 skip_install = true
 deps = isort
 commands = 
     isort . {posargs} qbraid/api \               
                       qbraid/interface \
                       qbraid/transpiler \
-                      qbraid/devices
+                      qbraid/devices \
+                      tools
 
 [testenv:pylint]
 envdir = .tox/linters
 skip_install = true
 deps = pylint
 commands = 
     pylint {posargs} qbraid/__init__.py \
@@ -64,30 +66,47 @@
                      qbraid/get_devices.py \
                      qbraid/get_jobs.py \
                      qbraid/tests \
                      qbraid/api \
                      qbraid/interface \
                      qbraid/transpiler \
                      qbraid/devices \
-                     --exit-zero \
+                     tools \
                      --disable=C0103,E0401,R0801,R0902,R0903,R0911,R0912,R0914,W0212,W0511
                     
-
 [testenv:black]
 envdir = .tox/linters
 skip_install = true
 deps = black
 commands = 
-    black {posargs} qbraid --exclude /(qbraid/transpiler/cirq_pytket/tests/test_from_pytket.py|qbraid/transpiler/cirq_qasm)/
+    black qbraid tools --exclude /(qbraid/transpiler/cirq_pytket/tests/test_from_pytket.py|qbraid/transpiler/cirq_qasm)/ {posargs}
+
+[testenv:headers]
+envdir = .tox/linters
+skip_install = true
+deps =
+commands = 
+    python tools/verify_headers.py qbraid tools {posargs}
 
 [testenv:linters]
 envdir = .tox/linters
 skip_install = true
 deps =
     {[testenv:isort]deps}
-    {[testenv:pylint]deps}
     {[testenv:black]deps}
 commands =
     {[testenv:isort]commands}
-    {[testenv:pylint]commands}
     {[testenv:black]commands}
-    python tools/verify_headers.py qbraid
+    {[testenv:headers]commands} {posargs:--fix}
+
+[testenv:format-check]
+envdir = .tox/linters
+skip_install = true
+deps =
+    {[testenv:pylint]deps}
+    {[testenv:isort]deps}
+    {[testenv:black]deps}
+commands =
+    {[testenv:pylint]commands}
+    {[testenv:isort]commands} {posargs:--check-only}
+    {[testenv:black]commands} {posargs:--check}
+    {[testenv:headers]commands}
```

