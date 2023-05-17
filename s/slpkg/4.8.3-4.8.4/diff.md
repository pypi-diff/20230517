# Comparing `tmp/slpkg-4.8.3.tar.gz` & `tmp/slpkg-4.8.4.tar.gz`

## Comparing `slpkg-4.8.3.tar` & `slpkg-4.8.4.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:21:35.000000 slpkg-4.8.3/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/multilib/
--rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/multilib/README.ERIC
--rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/multilib/glibc_packages.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/multilib/README
--rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/multilib/compat32.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/README
--rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-05-14 17:18:17.000000 slpkg-4.8.3/repositories.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-05-14 17:18:17.000000 slpkg-4.8.3/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-05-14 17:18:17.000000 slpkg-4.8.3/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-05-14 17:18:17.000000 slpkg-4.8.3/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     4195 2023-05-14 17:18:17.000000 slpkg-4.8.3/slackbuild/slpkg.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-05-14 17:18:17.000000 slpkg-4.8.3/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-05-14 17:18:17.000000 slpkg-4.8.3/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/configs/
--rw-r--r--   0 dslackw   (1000) users      (100)     8822 2023-05-14 17:18:17.000000 slpkg-4.8.3/configs/repositories.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-05-14 17:18:17.000000 slpkg-4.8.3/configs/blacklist.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     3813 2023-05-14 17:18:17.000000 slpkg-4.8.3/configs/slpkg.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      753 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_sbo_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/check_updates_test.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_bin_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-05-14 17:18:17.000000 slpkg-4.8.3/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-05-14 17:18:17.000000 slpkg-4.8.3/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)    46097 2023-05-14 17:18:17.000000 slpkg-4.8.3/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/man/
--rw-r--r--   0 dslackw   (1000) users      (100)     9164 2023-05-14 17:18:17.000000 slpkg-4.8.3/man/slpkg.1
--rw-r--r--   0 dslackw   (1000) users      (100)     9919 2023-05-14 17:18:17.000000 slpkg-4.8.3/man/slpkg-fr.1
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/completion/
--rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-05-14 17:18:17.000000 slpkg-4.8.3/completion/slpkg
--rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-05-14 17:18:17.000000 slpkg-4.8.3/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/
--rw-r--r--   0 dslackw   (1000) users      (100)     4208 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/dialog_configs.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/binaries/
--rw-r--r--   0 dslackw   (1000) users      (100)     1901 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/binaries/required.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/binaries/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/binaries/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7477 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/binaries/install.py
--rw-r--r--   0 dslackw   (1000) users      (100)    65522 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/install_data.py
--rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/repositories.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4370 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/repo_info.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/sbos/
--rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/sbos/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)    11741 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/sbos/slackbuild.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1160 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/sbos/dependencies.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/sbos/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4483 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/sbos/sbo_generate.py
--rw-r--r--   0 dslackw   (1000) users      (100)    34064 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/update_repository.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2066 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/progress_bar.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3156 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/downloader.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/models/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/models/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/models/models.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/
--rw-r--r--   0 dslackw   (1000) users      (100)     5945 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/view_package.py
--rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/version.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6212 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/cli_menu.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4898 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/asciibox.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3801 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/help_commands.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     9651 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/views.py
--rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/error_messages.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3649 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1334 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/logging_deps.py
--rw-r--r--   0 dslackw   (1000) users      (100)    11666 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/new_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1819 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/multi_process.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3256 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/cleanings.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/checksum.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/dialog_box.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4460 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7274 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3715 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/dependees.py
--rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/toml_error_message.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6020 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/check_updates.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6025 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/remove_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)      939 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3339 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/download_only.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3965 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/tracking.py
--rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/logging_config.py
--rw-r--r--   0 dslackw   (1000) users      (100)    29842 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1262 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/find_installed.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3609 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2731 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/search.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1471 2023-05-14 17:18:17.000000 slpkg-4.8.3/setup.cfg
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/entry_points.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1286 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1262 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)     8493 2023-05-14 17:18:17.000000 slpkg-4.8.3/README.md
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/tools/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-05-14 17:18:17.000000 slpkg-4.8.3/tools/gen_sbo_txt.sh
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:57:00.000000 slpkg-4.8.4/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/multilib/
+-rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/multilib/README.ERIC
+-rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/multilib/glibc_packages.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/multilib/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/multilib/compat32.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-05-17 17:49:35.000000 slpkg-4.8.4/repositories.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-05-17 17:49:35.000000 slpkg-4.8.4/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-05-17 17:49:35.000000 slpkg-4.8.4/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-05-17 17:49:35.000000 slpkg-4.8.4/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     4195 2023-05-17 17:49:35.000000 slpkg-4.8.4/slackbuild/slpkg.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-05-17 17:49:35.000000 slpkg-4.8.4/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1520 2023-05-17 17:49:35.000000 slpkg-4.8.4/.pyproject.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-05-17 17:49:35.000000 slpkg-4.8.4/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/configs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8822 2023-05-17 17:49:35.000000 slpkg-4.8.4/configs/repositories.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-05-17 17:49:35.000000 slpkg-4.8.4/configs/blacklist.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     4129 2023-05-17 17:49:35.000000 slpkg-4.8.4/configs/slpkg.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      754 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_sbo_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/check_updates_test.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_bin_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-05-17 17:49:35.000000 slpkg-4.8.4/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-05-17 17:49:35.000000 slpkg-4.8.4/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)    46324 2023-05-17 17:49:35.000000 slpkg-4.8.4/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/man/
+-rw-r--r--   0 dslackw   (1000) users      (100)     9644 2023-05-17 17:49:35.000000 slpkg-4.8.4/man/slpkg.1
+-rw-r--r--   0 dslackw   (1000) users      (100)     9919 2023-05-17 17:49:35.000000 slpkg-4.8.4/man/slpkg-fr.1
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/completion/
+-rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-05-17 17:49:35.000000 slpkg-4.8.4/completion/slpkg
+-rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-05-17 17:49:35.000000 slpkg-4.8.4/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/
+-rw-r--r--   0 dslackw   (1000) users      (100)     4289 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/dialog_configs.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/binaries/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1901 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/binaries/required.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/binaries/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/binaries/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7464 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/binaries/install.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    65522 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/install_data.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/repositories.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4370 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/repo_info.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/sbos/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/sbos/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11497 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/sbos/slackbuild.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1160 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/sbos/dependencies.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/sbos/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4483 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    34008 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/update_repository.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2437 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/progress_bar.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3156 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/downloader.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/models/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/models/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/models/models.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/
+-rw-r--r--   0 dslackw   (1000) users      (100)     5945 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/view_package.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/version.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6335 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/cli_menu.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5928 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/asciibox.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3801 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/help_commands.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     9691 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/views.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/error_messages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3445 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1334 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/logging_deps.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11666 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/new_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2002 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/multi_process.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3256 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/cleanings.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/checksum.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/dialog_box.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4812 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7847 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3864 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/dependees.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/toml_error_message.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6051 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/check_updates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6654 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/remove_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      939 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3339 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/download_only.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3965 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/tracking.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/logging_config.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    32240 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1518 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/find_installed.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3609 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3089 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/search.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1466 2023-05-17 17:49:35.000000 slpkg-4.8.4/setup.cfg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/entry_points.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1286 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1257 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/PKG-INFO
+-rw-r--r--   0 dslackw   (1000) users      (100)     8561 2023-05-17 17:49:35.000000 slpkg-4.8.4/README.md
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/tools/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-05-17 17:49:35.000000 slpkg-4.8.4/tools/gen_sbo_txt.sh
```

### Comparing `slpkg-4.8.3/filelists/multilib/README.ERIC` & `slpkg-4.8.4/filelists/multilib/README.ERIC`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/filelists/multilib/README` & `slpkg-4.8.4/filelists/multilib/README`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/filelists/multilib/compat32.pkgs` & `slpkg-4.8.4/filelists/multilib/compat32.pkgs`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/repositories.txt` & `slpkg-4.8.4/repositories.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slackbuild/slack-desc` & `slpkg-4.8.4/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slackbuild/slpkg.SlackBuild` & `slpkg-4.8.4/slackbuild/slpkg.SlackBuild`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/configs/repositories.toml` & `slpkg-4.8.4/configs/repositories.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This is the general repositories configuration file of slpkg:
 # /etc/slpkg/repositories.toml
-# Date: 26/04/2023, Version: 4.8.2
+# Date: 26/04/2023, Version: 4.8.3
 
 # Set 'true' to the variable {NAME}_REPO to enable a repository.
 
 # If you are going to use a local repository, set the repository:
 # as the example bellow:
 # ALIEN_REPO_LOCAL = ["file:///path/to/alien/repository/" ,"15.0/", "x86_64/"]
 # A binary local repository will must contain the files:
```

### Comparing `slpkg-4.8.3/configs/slpkg.toml` & `slpkg-4.8.4/configs/slpkg.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This is the general configuration file of slpkg:
 # /etc/slpkg/slpkg.toml
-# Date: 24/04/2023, Version: 4.8.2
+# Date: 24/04/2023, Version: 4.8.3
 
 [CONFIGS]
 
 # OS architecture by default.
 OS_ARCH = "x86_64"
 
 # Where the packages download.
@@ -48,21 +48,31 @@
 SPINNING_BAR = true
 
 # There are 5 predefined spinners for the progress bar.
 # Default is pixel. [spinner/pie/moon/line/pixel]
 PROGRESS_SPINNER = "pixel"
 
 # Choose color for the progress bar spinner.
-# Default is green. [green/violet/yellow/blue/cyan/grey/red]
+# Default is green. [white/green/violet/yellow/blue/cyan/grey/red]
 SPINNER_COLOR = "green"
 
+# Choose color for the border box.
+# Bold colors: [bold_green/bold_cyan/bold_yellow/bold_red/bold_blue]
+# Colors: [white/green/cyan/yellow/red/blue]
+# Default is bold_green.
+BORDER_COLOR = "bold_green"
+
+# Enable or disable case-sensitive pattern matching.
+# Default is true. [true/false]
+CASE_SENSITIVE = true
+
 # Slackware command for install packages, instead, you can use 'installpkg'.
 # Normally upgradepkg only upgrades packages that are already installed
 # on the system, and will skip any packages that do not already have a
-# version installed. If --install- new is specified, the behavior is
+# version installed. If --install-new is specified, the behavior is
 # modified to install new packages in addition to upgrading existing ones.
 # See manpage of the upgradepkg.
 INSTALLPKG = "upgradepkg --install-new"
 
 # Slackware command to reinstall packages.
 # Upgradepkg usually skips packages if the exact same package (matching name,
 # version, arch, and build number) is already installed on the system. Use
```

### Comparing `slpkg-4.8.3/tests/test_configs.py` & `slpkg-4.8.4/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/tests/test_checks.py` & `slpkg-4.8.4/tests/test_checks.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class TestPkgInstalled(unittest.TestCase):
 
     def setUp(self):
         self.bin_queries = SBoQueries('sbo')
         self.data = self.bin_queries.repository_data()
         self.check = Check('sbo', self.data)
-        self.packages = ['audacity', 'Flask', 'awscli']
+        self.packages = ['colored', 'sbo-create', 'sun']
 
     def test_check_exists(self):
         self.assertIsNone(self.check.package_exists_in_the_database(self.packages))
 
     def test_check_unsupported(self):
         self.assertIsNone(self.check.is_package_unsupported(self.packages))
```

### Comparing `slpkg-4.8.3/tests/test_utilities.py` & `slpkg-4.8.4/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/tests/test_sbo_queries.py` & `slpkg-4.8.4/tests/test_sbo_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/tests/test_colors.py` & `slpkg-4.8.4/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/tests/check_updates_test.py` & `slpkg-4.8.4/tests/check_updates_test.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/tests/test_upgrade.py` & `slpkg-4.8.4/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/tests/test_bin_queries.py` & `slpkg-4.8.4/tests/test_bin_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/LICENSE` & `slpkg-4.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/install.sh` & `slpkg-4.8.4/install.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/ChangeLog.txt` & `slpkg-4.8.4/ChangeLog.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+4.8.4 - 14/05/2023
+Added:
+- Case-insensitive pattern matching, --no-case option
+- Choose border color via configuration file
+- New processing status view for build, install, upgrade, remove
+Fixed:
+- Remove chosen dependencies
+
 4.8.3 - 29/04/2023
 Updated:
 - For synchronization with the local repository (Thanks to Christopher Schrauben) #166
 - Renamed the option --bin-repo with --repository
 Added:
 - Options --install-data to install only data into the database
 - Column for package installed version (Thanks to tpiszcze)
```

### Comparing `slpkg-4.8.3/man/slpkg.1` & `slpkg-4.8.4/man/slpkg.1`

 * *Files 6% similar despite different names*

```diff
@@ -176,14 +176,20 @@
 .P
 .B -P, --parallel
 .RS
 Download files in parallel to speed up the process.
 (to be used with: -u, update, -U, upgrade, -b, build, -i, install, -d, download)
 .RE
 .P
+.B -m, --no-case
+.RS
+Case-sensitive pattern matching packages.
+(to be used with: -b, build, -i, install, -d, download, -s, search, -f, find, -w, view, -t, tracking, -e, dependees)
+.RE
+.P
 .BI "-o," "" " \-\--repository=" NAME "
 .RS
 Switches the default repository and set the repository you want to work with.
 Make sure that you have been enabling the repository in the file '/etc/slpkg/repositories.toml'.
 Repo pattern '*' supported only with: '-s, search' option.
 (to be used with: -u, update, -U, upgrade, -c, check-updates, -I, repo-info, -b, build, -i, install, -d, download, -s, search,
 -t, tracking, -e, dependees, -w, view)
@@ -245,14 +251,25 @@
 .P
 0 Successful slpkg execution.
 .P
 1 Something wrong happened.
 .P
 20 No package found to be  downloaded,  installed,  reinstalled,  upgraded, or removed.
 .RE
+.SH EXPLANATION CHARACTERS
+.P
+[•] Processing status: Red is still processing, Green is done.
+.P
+[✔️] Done character: Appear when the processing is done.
+.P
+[X] Failed character: Appear when the processing is failed.
+.P
+[↪] Skipped character: Appear when the processing skipped.
+.P
+.RE
 .SH CONFIGURATION FILES
 .P
 Configuration file in the /etc/slpkg/slpkg.toml file.
 .P
 Repositories file in the /etc/slpkg/repositories.toml file.
 .P
 Blacklist file in the /etc/slpkg/blacklist.toml file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `slpkg-4.8.3/man/slpkg-fr.1` & `slpkg-4.8.4/man/slpkg-fr.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/completion/slpkg` & `slpkg-4.8.4/completion/slpkg`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/dialog_configs.py` & `slpkg-4.8.4/slpkg/dialog_configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             self.errors.raise_error_message(f"You should enable the dialog in the "
                                             f"'{self.etc_path}/{self.prog_name}.toml' file", exit_status=1)
 
     def edit(self) -> None:
         """ Read and write the configuration file. """
         self.is_dialog_enabled()
         elements: list = []
-        height: int = 30
+        height: int = 35
         width: int = 74
         text: str = f'Edit the configuration file: {self.config_file}'
         title: str = ' Configuration File '
 
         # Creating the elements for the dialog form.
         for i, (key, value) in enumerate(self.configs['CONFIGS'].items(), start=1):
             if value is True:
@@ -72,15 +72,16 @@
         keys: list = [
             'COLORS',
             'DIALOG',
             'SILENT_MODE',
             'ASCII_CHARACTERS',
             'ASK_QUESTION',
             'PARALLEL_DOWNLOADS',
-            'SPINNING_BAR'
+            'SPINNING_BAR',
+            'CASE_INSENSITIVE'
         ]
         values: list = ['true', 'false']
 
         for key, value in zip(self.configs['CONFIGS'].keys(), tags):
 
             if key in keys and value not in values:
                 self.dialogbox.msgbox(f"\nError: Value for '{key}', it must be 'true' or 'false.'\n",
@@ -114,12 +115,13 @@
 
                             ('COLORS =',
                              'DIALOG =',
                              'SILENT_MODE =',
                              'ASCII_CHARACTERS =',
                              'ASK_QUESTION =',
                              'PARALLEL_DOWNLOADS =',
-                             'SPINNING_BAR =')
+                             'SPINNING_BAR =',
+                             'CASE_SENSITIVE =')
                     ):
                         line: str = line.replace('"', '')
 
                 patch_toml.write(line)
```

### Comparing `slpkg-4.8.3/slpkg/binaries/required.py` & `slpkg-4.8.4/slpkg/binaries/required.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/binaries/queries.py` & `slpkg-4.8.4/slpkg/binaries/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/binaries/install.py` & `slpkg-4.8.4/slpkg/binaries/install.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         self.upgrade = Upgrade(repository, data)
         self.view_message = ViewMessage(flags, repository, data)
         self.check_md5 = Md5sum(flags)
 
         self.dependencies: list = []
         self.install_order: list = []
         self.binary_packages: list = []
+        self.slackware_command: str = self.installpkg
+        self.progress_message: str = f'{self.cyan}Installing{self.endc}'
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ['-r', '--reinstall'], flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
             ['-k', '--skip-installed'], flags)
 
@@ -63,14 +65,16 @@
 
         self.view_message.install_upgrade_packages(self.packages, self.dependencies, self.mode)
         self.view_message.question()
 
         start: float = time.time()
         self.crating_the_package_urls_list()
         self.checksum_binary_packages()
+        self.set_slackware_command()
+        self.set_progress_message()
         self.install_packages()
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
     def creating_dependencies_list(self) -> None:
         if not self.option_for_resolve_off:
@@ -110,16 +114,15 @@
 
                 package_urls.append(f'{mirror}{location}/{package}')
 
                 self.binary_packages.append(package)
                 self.utils.remove_file_if_exists(self.tmp_slpkg, package)
             else:
                 installed_package: str = self.utils.is_package_installed(pkg)
-                installed_version: str = self.utils.split_package(installed_package)['version']
-                self.view_message.view_skipping_packages(pkg, installed_version)
+                self.view_message.view_skipping_packages(installed_package)
 
         self.download_the_binary_packages(package_urls)
 
     def download_the_binary_packages(self, package_urls: list) -> None:
         if package_urls:
             down = Downloader(self.tmp_slpkg, package_urls, self.flags)
             down.download()
@@ -145,30 +148,29 @@
         for package in self.binary_packages:
             name: str = self.utils.split_package(Path(package).stem)['name']
             pkg_checksum: str = self.data[name]['checksum']
             self.check_md5.md5sum(self.tmp_slpkg, package, pkg_checksum)
 
     def install_packages(self) -> None:
         for package in self.binary_packages:
-            progress_message: str = f'{self.cyan}Installing{self.endc}'
-            slack_command: str = self.installpkg
-
-            if (self.option_for_reinstall or self.utils.is_package_installed(package)
-                    or self.mode == 'upgrade'):
-                progress_message: str = f'{self.cyan}Upgrading{self.endc}'
-                slack_command: str = self.reinstall
-
-            command: str = f'{slack_command} {self.tmp_slpkg}/{package}'
-            process_message: str = f"package '{package}' to install"
-            self.multi_proc.process(command, package, process_message, progress_message)
+            command: str = f'{self.slackware_command} {self.tmp_slpkg}/{package}'
+            self.multi_proc.process(command, package, self.progress_message)
 
             if not self.option_for_resolve_off:
                 name: str = self.utils.split_package(Path(package).stem)['name']
                 self.logs_deps.logging(name)
 
+    def set_progress_message(self):
+        if self.mode == 'upgrade' or self.option_for_reinstall:
+            self.progress_message: str = f'{self.cyan}Upgrading{self.endc}'
+
+    def set_slackware_command(self) -> None:
+        if self.mode == 'upgrade' or self.option_for_reinstall:
+            self.slackware_command: str = self.reinstall
+
     def choose_package_dependencies(self) -> None:
         if self.dependencies:
             height: int = 10
             width: int = 70
             list_height: int = 0
             choices: list = []
             title: str = ' Choose dependencies you want to install '
```

### Comparing `slpkg-4.8.3/slpkg/install_data.py` & `slpkg-4.8.4/slpkg/install_data.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/repositories.py` & `slpkg-4.8.4/slpkg/repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/repo_info.py` & `slpkg-4.8.4/slpkg/repo_info.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/sbos/queries.py` & `slpkg-4.8.4/slpkg/sbos/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/sbos/slackbuild.py` & `slpkg-4.8.4/slpkg/sbos/slackbuild.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         self.view_message = ViewMessage(flags, repository, data)
         self.check_md5 = Md5sum(self.flags)
 
         self.sources: dict = {}
         self.install_order: list = []
         self.dependencies: list = []
         self.slackware_command: str = str()
+        self.slackware_command: str = self.installpkg
+        self.progress_message: str = f'{self.cyan}Installing{self.endc}'
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ['-r', '--reinstall'], flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
             ['-k', '--skip-installed'], flags)
 
@@ -83,14 +85,16 @@
         self.clean_the_main_slackbuilds()
         self.add_main_packages_to_install_order()
         self.view_slackbuilds_before_build()
 
         start: float = time.time()
         self.prepare_slackbuilds_for_build()
         self.download_the_sources()
+        self.set_slackware_command()
+        self.set_progress_message()
         self.build_and_install_the_slackbuilds()
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
     def creating_dependencies_list(self) -> None:
         if not self.option_for_resolve_off:
@@ -197,47 +201,31 @@
                 if self.mode in ('install', 'upgrade'):
                     self.install_package(sbo)
 
                     if not self.option_for_resolve_off:
                         self.logs_deps.logging(sbo)
             else:
                 installed_package: str = self.utils.is_package_installed(sbo)
-                installed_version: str = self.utils.split_package(installed_package)['version']
-                self.view_message.view_skipping_packages(sbo, installed_version)
+                self.view_message.view_skipping_packages(installed_package)
 
     def patch_slackbuild_tag(self, sbo: str) -> None:
         sbo_script: Path = Path(self.build_path, sbo, f'{sbo}.SlackBuild')
         if sbo_script.is_file() and self.repo_tag:
             lines: list = self.utils.read_text_file(sbo_script)
 
             with open(sbo_script, 'w') as script:
                 for line in lines:
                     if line.startswith('TAG=$'):
                         line: str = f'TAG=${{TAG:-{self.repo_tag}}}\n'
                     script.write(line)
 
     def install_package(self, name: str) -> None:
         package: str = self.find_package_for_install(name)
-        self.set_slackware_command(name)
-
-        progress_message: str = f'{self.cyan}Installing{self.endc}'
-        process_message: str = f"package '{name}' to install"
-
-        if self.mode == 'upgrade':
-            progress_message: str = f'{self.cyan}Upgrading{self.endc}'
-            process_message: str = f"package '{name}' to upgrade"
-
         command: str = f'{self.slackware_command} {self.tmp_path}/{package}'
-
-        self.multi_proc.process(command, package, process_message, progress_message)
-
-    def set_slackware_command(self, name: str) -> None:
-        self.slackware_command: str = self.installpkg
-        if self.option_for_reinstall and self.utils.is_package_installed(name):
-            self.slackware_command: str = self.reinstall
+        self.multi_proc.process(command, package, self.progress_message)
 
     def find_package_for_install(self, name: str) -> str:
         version: str = self.data[name]['version']
         pattern: str = f'{name}-{version}*{self.repo_tag}*'
         packages: list = [file.name for file in self.tmp_path.glob(pattern)]
         try:
             return max(packages)
@@ -248,21 +236,25 @@
             self.errors.raise_error_message(f"Package '{name}' not found for install", exit_status=20)
 
     def build_the_script(self, path: Path, name: str) -> None:
         self.set_makeflags()
         folder: Path = Path(path, name)
         filename: str = f'{name}.SlackBuild'
         command: str = f'{folder}/./{filename}'
-
         self.utils.change_owner_privileges(folder)
-
         progress_message: str = f'{self.red}Build{self.endc}'
-        process_message: str = f"package '{name}' to build"
+        self.multi_proc.process(command, filename, progress_message)
+
+    def set_progress_message(self):
+        if self.mode == 'upgrade' or self.option_for_reinstall:
+            self.progress_message: str = f'{self.cyan}Upgrading{self.endc}'
 
-        self.multi_proc.process(command, filename, process_message, progress_message)
+    def set_slackware_command(self) -> None:
+        if self.mode == 'upgrade' or self.option_for_reinstall:
+            self.slackware_command: str = self.reinstall
 
     def set_makeflags(self) -> None:
         if self.option_for_jobs:
             os.environ['MAKEFLAGS'] = f'-j {cpu_count()}'
 
     def choose_package_dependencies(self) -> None:
         if self.dependencies:
```

### Comparing `slpkg-4.8.3/slpkg/sbos/dependencies.py` & `slpkg-4.8.4/slpkg/sbos/dependencies.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/sbos/sbo_generate.py` & `slpkg-4.8.4/slpkg/sbos/sbo_generate.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/update_repository.py` & `slpkg-4.8.4/slpkg/update_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -608,33 +608,30 @@
 
         if not any(list(compare.values())):
             print(f'\n{self.endc}{self.yellow}No changes in ChangeLog.txt between your '
                   f'last update and now.{self.endc}')
 
     def repositories(self) -> None:
         queue = Queue()
-        message = f'Checking for news, please wait...'
+        message: str = 'Checking for news, please wait...'
 
         # Starting multiprocessing
         p1 = Process(target=self.check_for_updates, args=(queue,))
-        p2 = Process(target=self.progress.progress_bar, args=(message, ''))
+        p2 = Process(target=self.progress.progress_bar, args=(message,))
 
         p1.start()
         p2.start()
 
         # Wait until process 1 finish
         p1.join()
 
         # Terminate process 2 if process 1 finished
         if not p1.is_alive():
             p2.terminate()
 
-        # Wait until process 2 finish
-        p2.join()
-
         # Restore the terminal cursor
         print('\x1b[?25h', self.endc, end='')
 
         self.repos_for_update: dict = queue.get()
         self.update_the_repositories()
 
     def delete_sbo_database_data(self) -> None:
```

### Comparing `slpkg-4.8.3/slpkg/progress_bar.py` & `slpkg-4.8.4/slpkg/progress_bar.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,43 +2,52 @@
 # -*- coding: utf-8 -*-
 
 import time
 from progress.spinner import (PixelSpinner, LineSpinner,
                               MoonSpinner, PieSpinner, Spinner)
 
 from slpkg.configs import Configs
+from slpkg.views.asciibox import AsciiBox
 
 
 class ProgressBar(Configs):
 
     def __init__(self):
         super(Configs, self).__init__()
         self.spinner = PixelSpinner
+        self.ascii = AsciiBox()
+
         self.color: str = self.endc
         self.spinners: dict = {}
         self.spinners_color: dict = {}
 
-    def progress_bar(self, message: str, filename: str) -> None:
+    def progress_bar(self, message: str, filename=None) -> None:
         """ Creating progress bar. """
         self.assign_spinners()
         self.assign_spinner_colors()
         self.set_spinner()
         self.set_color()
 
+        bar_message: str = f"{self.endc}{message} "
+        if filename:
+            bar_message: str = (f"{'':>2}{self.red}{self.ascii.bullet}{self.endc} {filename}: "
+                                f"{message}... ")
+
         if self.spinning_bar:
-            bar_spinner = self.spinner(f'{self.endc}{message} {filename} {self.color}')
+            bar_spinner = self.spinner(f'{bar_message}{self.color}')
             # print('\033[F', end='', flush=True)
             try:
                 while True:
                     time.sleep(0.1)
                     bar_spinner.next()
             except KeyboardInterrupt:
                 raise SystemExit(1)
         else:
-            print(f'{message} ', end='', flush=True)
+            print(f"{'':>2}{self.red}{self.ascii.bullet}{self.endc} {filename}: "
+                  f"{message}... {self.color}", end='')
 
     def assign_spinners(self) -> None:
         self.spinners: dict[str] = {
             'pixel': PixelSpinner,
             'line': LineSpinner,
             'moon': MoonSpinner,
             'pie': PieSpinner,
@@ -50,20 +59,20 @@
             'green': self.green,
             'violet': self.violet,
             'yellow': self.yellow,
             'blue': self.blue,
             'cyan': self.cyan,
             'grey': self.grey,
             'red': self.red,
-            '': self.endc
+            'white': self.endc
         }
 
     def set_spinner(self) -> None:
         try:
-            self.spinner = self.spinners[self.progress_spinner]
+            self.spinner: str = self.spinners[self.progress_spinner]
         except KeyError:
             self.spinner = PixelSpinner
 
     def set_color(self) -> None:
         try:
             self.color: str = self.spinners_color[self.spinner_color]
         except KeyError:
```

### Comparing `slpkg-4.8.3/slpkg/downloader.py` & `slpkg-4.8.4/slpkg/downloader.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/models/models.py` & `slpkg-4.8.4/slpkg/models/models.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/views/view_package.py` & `slpkg-4.8.4/slpkg/views/view_package.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/views/version.py` & `slpkg-4.8.4/slpkg/views/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 8, 3)
+        self.version_info: tuple = (4, 8, 4)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.8.3/slpkg/views/cli_menu.py` & `slpkg-4.8.4/slpkg/views/cli_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-g, configs, -L, clean-logs, -T, clean-data, -D, clean-tmp]\n'
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-b, build, -i, install, -R, remove [PACKAGES...]]\n'
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-d, download, -f, find, -w, view [PACKAGES...]]\n'
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-s, search, -e, dependees, -t, tracking  [PACKAGES...]]\n'
             f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-y, --yes, -j, --jobs, -O, --resolve-off, -r, --reinstall]\n'
             f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-k, --skip-installed, -a, --install-data]\n'
             f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-E, --full-reverse, -S, --search, -n, --no-silent]\n'
-            f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-p, --pkg-version, -P, --parallel]\n'
+            f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-p, --pkg-version, -P, --parallel, -m, --no-case]\n'
             f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-o, --repository=NAME, -z, --directory=PATH]\n'
             "  \nIf you need more information please try 'slpkg --help'.")
 
         print(args)
         raise SystemExit(status)
 
     def help(self, status: int) -> NoReturn:
@@ -75,14 +75,15 @@
             f'  {self.yellow}-k, --skip-installed{self.endc}          Skip installed packages.\n'
             f'  {self.yellow}-a, --install-data{self.endc}            Install data into the database only.\n'
             f'  {self.yellow}-E, --full-reverse{self.endc}            Full reverse dependency.\n'
             f'  {self.yellow}-S, --search{self.endc}                  Search packages from the repository.\n'
             f'  {self.yellow}-n, --no-silent{self.endc}               Disable silent mode.\n'
             f'  {self.yellow}-p, --pkg-version{self.endc}             Print the repository package version.\n'
             f'  {self.yellow}-P, --parallel{self.endc}                Download files in parallel.\n'
+            f'  {self.yellow}-m, --no-case{self.endc}                 Case-insensitive pattern matching.\n'
             f'  {self.yellow}-o, --repository={self.endc}NAME         Change repository you want to work.\n'
             f'  {self.yellow}-z, --directory={self.endc}PATH          Download files to a specific path.\n'
             '\n  -h, --help                    Show this message and exit.\n'
             '  -v, --version                 Print version and exit.\n'
             "\nIf you need more information try to use slpkg manpage.\n"
             "Extra help for the commands, use: 'slpkg help [COMMAND]'.\n"
             "Edit the config file in the /etc/slpkg/slpkg.toml or 'slpkg configs'.")
```

### Comparing `slpkg-4.8.3/slpkg/views/asciibox.py` & `slpkg-4.8.4/slpkg/views/asciibox.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,71 +15,103 @@
         self.version_alignment: int = 29
         self.size_alignment: int = 14
         self.repo_alignment: int = 14
 
         if self.package_alignment < 1:
             self.package_alignment = 1
 
+        self.bd_color: str = self.endc
+        self.border_colors: dict = {}
+        self.assign_border_color()
+
+        self.bullet: str = '-'
+        self.done: str = 'Done'
+        self.failed: str = 'Failed'
+        self.skipped: str = 'Skipped'
+
         self.vertical_line: str = '|'
         self.horizontal_line: str = '='
         self.horizontal_vertical: str = '+'
         self.upper_right_corner: str = '+'
         self.lower_left_corner: str = '+'
         self.lower_right_corner: str = '+'
         self.upper_left_corner: str = '+'
         self.horizontal_and_up: str = '+'
         self.horizontal_and_down: str = '+'
         self.vertical_and_right: str = '+'
         self.vertical_and_left: str = '+'
 
         if self.ascii_characters:
+            self.bullet: str = '•'
+            self.done: str = '✔️'
+            self.failed: str = 'X'
+            self.skipped: str = '↪'
             self.vertical_line: str = '│'
             self.horizontal_line: str = '─'
             self.horizontal_vertical: str = '┼'
             self.upper_right_corner: str = '┐'
             self.lower_left_corner: str = '└'
             self.lower_right_corner: str = '┘'
             self.upper_left_corner: str = '┌'
             self.horizontal_and_up: str = '┴'
             self.horizontal_and_down: str = '┬'
             self.vertical_and_right: str = '├'
             self.vertical_and_left: str = '┤'
 
+    def assign_border_color(self):
+        self.border_colors: dict[str] = {
+            'red': self.red,
+            'blue': self.blue,
+            'cyan': self.cyan,
+            'white': self.endc,
+            'green': self.green,
+            'yellow': self.yellow,
+            'bold_red': self.bred,
+            'bold_blue': self.bblue,
+            'bold_cyan': self.bcyan,
+            'bold_green': self.bgreen,
+            'bold_yellow': self.byellow
+        }
+        try:
+            self.bd_color: str = self.border_colors[self.border_color]
+        except KeyError:
+            self.bd_color: str = self.endc
+
     def draw_package_title(self, message: str, title: str) -> None:
         title = title.title()
-        print(f"{self.bgreen}{self.upper_left_corner}{self.horizontal_line * (self.columns - 2)}"
+        print(f"{self.bd_color}{self.upper_left_corner}{self.horizontal_line * (self.columns - 2)}"
               f"{self.upper_right_corner}")
         print(f"{self.vertical_line}{title.center(self.columns - 2, ' ')}{self.vertical_line}")
         self.draw_middle_line()
         print(f"{self.vertical_line} {self.endc}{message.ljust(self.columns - 3, ' ')}"
-              f"{self.bgreen}{self.vertical_line}")
+              f"{self.bd_color}{self.vertical_line}")
         self.draw_middle_line()
-        print(f"{self.bgreen}{self.vertical_line}{self.endc} {'Package:':<{self.package_alignment}}"
+        print(f"{self.bd_color}{self.vertical_line}{self.endc} {'Package:':<{self.package_alignment}}"
               f"{'Version:':<{self.version_alignment}}{'Size:':<{self.size_alignment}}{'Repo:':>{self.repo_alignment}} "
-              f"{self.bgreen}{self.vertical_line}{self.endc}")
+              f"{self.bd_color}{self.vertical_line}{self.endc}")
 
     def draw_package_line(self, package: str, version: str, size: str, color: str, repo: str) -> None:
         if len(version) >= 20 and self.columns <= 80:
             version: str = f'{version[:self.version_alignment - 5]}...'
         if len(package) >= 15 and self.columns <= 80:
             package: str = f'{package[:self.package_alignment - 5]}...'
-        print(f"{self.bgreen}{self.vertical_line} {self.bold}{color}{package:<{self.package_alignment}}{self.endc}"
-              f"{self.bgreen}{version:<{self.version_alignment}}{self.endc}{size:<{self.size_alignment}}{self.blue}"
-              f"{repo:>{self.repo_alignment}}{self.bgreen} {self.vertical_line}{self.endc}")
+        print(f"{self.bd_color}{self.vertical_line} {self.bold}{color}{package:<{self.package_alignment}}{self.endc}"
+              f"{self.bd_color}{version:<{self.version_alignment}}{self.endc}{size:<{self.size_alignment}}{self.blue}"
+              f"{repo:>{self.repo_alignment}}{self.bd_color} {self.vertical_line}{self.endc}")
 
     def draw_middle_line(self) -> None:
-        print(f"{self.bgreen}{self.vertical_and_right}{self.horizontal_line * (self.columns - 2)}"
+        print(f"{self.bd_color}{self.vertical_and_right}{self.horizontal_line * (self.columns - 2)}"
               f"{self.vertical_and_left}")
 
     def draw_dependency_line(self) -> None:
-        print(f"{self.bgreen}{self.vertical_line}{self.endc} Dependencies:{' ' * (self.columns - 16)}"
-              f"{self.bgreen}{self.vertical_line}{self.endc}")
+        print(f"{self.bd_color}{self.vertical_line}{self.endc} Dependencies:{' ' * (self.columns - 16)}"
+              f"{self.bd_color}{self.vertical_line}{self.endc}")
 
     def draw_bottom_line(self) -> None:
-        print(f"{self.bold}{self.green}{self.lower_left_corner}{self.horizontal_line * (self.columns - 2)}"
+        print(f"{self.bd_color}{self.lower_left_corner}{self.horizontal_line * (self.columns - 2)}"
               f"{self.lower_right_corner}{self.endc}")
 
     def draw_checksum_error_box(self, name: str, checksum: str, file_check: str) -> None:
         print(f"{self.bred}{self.upper_left_corner}{self.horizontal_line * (self.columns - 2)}"
               f"{self.upper_right_corner}")
         print(f"{self.bred}{self.vertical_line}{self.bred} FAILED:{self.endc} MD5SUM check for "
               f"'{self.cyan}{name}'{' ' * (self.columns - len(name) - 30)}{self.red}{self.vertical_line}")
```

### Comparing `slpkg-4.8.3/slpkg/views/help_commands.py` & `slpkg-4.8.4/slpkg/views/help_commands.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/views/views.py` & `slpkg-4.8.4/slpkg/views/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,16 +227,17 @@
         print(summary_message)
 
     def build_package_and_version(self, package: str) -> str:
         installed_package: str = self.utils.is_package_installed(package)
         version: str = self.utils.split_package(installed_package)['version']
         return f'{package}-{version}'
 
-    def view_skipping_packages(self, package: str, version: str) -> None:
-        print(f'{self.yellow}Skipping{self.endc}: {package}-{version} {self.red}(already installed){self.endc}')
+    def view_skipping_packages(self, filename: str) -> None:
+        failed: str = f'{self.red}{self.ascii.skipped}{self.endc}'
+        print(f"\r{'':>2}{self.bred}{self.ascii.bullet}{self.endc} {filename} {failed}{' ' * 17}")
 
     def question(self) -> None:
         if not self.option_for_yes and self.ask_question:
             answer: str = input('\nDo you want to continue? [y/N] ')
             if answer not in ['Y', 'y']:
                 raise SystemExit()
         print()
```

### Comparing `slpkg-4.8.3/slpkg/checks.py` & `slpkg-4.8.4/slpkg/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,16 @@
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
     def package_exists_in_the_database(self, packages: list) -> None:
         not_packages: list = []
 
         for pkg in packages:
-            if self.is_binary:
-                if not self.data.get(pkg) and pkg != '*':
-                    not_packages.append(pkg)
-            else:
-                if not self.data.get(pkg) and pkg != '*':
-                    not_packages.append(pkg)
+            if not self.data.get(pkg) and pkg != '*':
+                not_packages.append(pkg)
 
         if not_packages:
             self.errors.raise_error_message(f"Packages '{', '.join(not_packages)}' does not exists",
                                             exit_status=1)
 
     def is_package_unsupported(self, slackbuilds: list) -> None:
         """ Checking for unsupported slackbuilds. """
@@ -86,9 +82,8 @@
             if self.is_binary:
                 count: int = self.session.query(BinariesTable.id).where(BinariesTable.repo == self.repository).count()
             else:
                 count: int = self.session.query(sbo_table[self.repository].id).count()
 
         if count == 0:
             self.errors.raise_error_message("You need to update the package lists first, run:\n\n"
-                                            "              $ slpkg update",
-                                            exit_status=1)
+                                            "              $ slpkg update", exit_status=1)
```

### Comparing `slpkg-4.8.3/slpkg/logging_deps.py` & `slpkg-4.8.4/slpkg/logging_deps.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/new_configs.py` & `slpkg-4.8.4/slpkg/new_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/cleanings.py` & `slpkg-4.8.4/slpkg/cleanings.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/checksum.py` & `slpkg-4.8.4/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/dialog_box.py` & `slpkg-4.8.4/slpkg/dialog_box.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/configs.py` & `slpkg-4.8.4/slpkg/configs.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,29 +31,31 @@
     installpkg: str = 'upgradepkg --install-new'
     reinstall: str = 'upgradepkg --reinstall'
     removepkg: str = 'removepkg'
     colors: bool = True
     dialog: bool = True
     downloader: str = 'wget'
     wget_options: str = '--c -q --progress=bar:force:noscroll --show-progress'
-    curl_options: str = ''
+    curl_options: str = str()
     lftp_get_options: str = '-c get -e'
     lftp_mirror_options: str = '-c mirror --parallel=100 --only-newer'
     silent_mode: bool = True
     ascii_characters: bool = True
     ask_question: bool = True
     parallel_downloads: bool = False
     file_pattern: str = '*'
     spinning_bar: str = True
     progress_spinner: str = 'pixel'
     spinner_color: str = 'green'
+    border_color: str = 'bgreen'
+    case_sensitive: bool = True
 
-    proxy_address: str = ''
-    proxy_username: str = ''
-    proxy_password: str = ''
+    proxy_address: str = str()
+    proxy_username: str = str()
+    proxy_password: str = str()
 
     try:
         # Load user configuration.
         config_path_file = Path(etc_path, f'{prog_name}.toml')
         if config_path_file.exists():
             with open(config_path_file, 'rb') as conf:
                 configs = tomli.load(conf)
@@ -78,46 +80,52 @@
             ascii_characters: bool = config['ASCII_CHARACTERS']
             file_list_suffix: str = config['FILE_LIST_SUFFIX']
             parallel_downloads: bool = config['PARALLEL_DOWNLOADS']
             file_pattern_conf: str = config['FILE_PATTERN']
             spinning_bar: str = config['SPINNING_BAR']
             progress_spinner: str = config['PROGRESS_SPINNER']
             spinner_color: str = config['SPINNER_COLOR']
+            border_color: str = config['BORDER_COLOR']
+            case_sensitive: bool = config['CASE_SENSITIVE']
             proxy_address: str = config['PROXY_ADDRESS']
             proxy_username: str = config['PROXY_USERNAME']
             proxy_password: str = config['PROXY_PASSWORD']
 
     except (KeyError, tomli.TOMLDecodeError) as error:
         errors.raise_toml_error_message(error, toml_file='/etc/slpkg/slpkg.toml')
 
-    blink: str = ''
-    bold: str = ''
-    red: str = ''
-    bred: str = ''
-    green: str = ''
-    bgreen: str = ''
-    yellow: str = ''
-    byellow: str = ''
-    cyan: str = ''
-    blue: str = ''
-    grey: str = ''
-    violet: str = ''
-    endc: str = ''
+    blink: str = str()
+    bold: str = str()
+    red: str = str()
+    bred: str = str()
+    green: str = str()
+    bgreen: str = str()
+    yellow: str = str()
+    byellow: str = str()
+    cyan: str = str()
+    bcyan: str = str()
+    blue: str = str()
+    bblue: str = str()
+    grey: str = str()
+    violet: str = str()
+    endc: str = str()
 
     if colors:
         blink: str = '\033[32;5m'
         bold: str = '\033[1m'
         red: str = '\x1b[91m'
         bred: str = f'{bold}{red}'
         green: str = '\x1b[32m'
         bgreen: str = f'{bold}{green}'
         yellow: str = '\x1b[93m'
         byellow: str = f'{bold}{yellow}'
         cyan: str = '\x1b[96m'
-        blue: str = '\x1b[94m'
+        bcyan: str = f'{bold}{cyan}'
+        blue: str = f'\x1b[94m'
+        bblue: str = f'{bold}{blue}'
         grey: str = '\x1b[38;5;247m'
         violet: str = '\x1b[35m'
         endc: str = '\x1b[0m'
 
     # Creating the paths if not exists
     paths = [
         db_path,
```

### Comparing `slpkg-4.8.3/slpkg/utilities.py` & `slpkg-4.8.4/slpkg/utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -139,24 +139,28 @@
             logger = logging.getLogger(LoggingConfig.date_time)
             logger.exception(f'{self.__class__.__name__}: '
                              f'{self.__class__.read_text_file.__name__}')
             self.errors.raise_error_message(f"No such file or directory: '{file}'", exit_status=20)
 
     def process(self, command: str, stderr=None, stdout=None) -> None:
         """ Handle the processes. """
+        output: int = 0
         try:
-            subprocess.call(command, shell=True, stderr=stderr, stdout=stdout)
+            output: int = subprocess.call(command, shell=True, stderr=stderr, stdout=stdout)
         except subprocess.CalledProcessError as error:
             logger = logging.getLogger(LoggingConfig.date_time)
             logger.exception(f'{self.__class__.__name__}'
                              f'{self.__class__.process.__name__}')
             self.errors.raise_error_message(str(error), exit_status=20)
         except KeyboardInterrupt:
             raise SystemExit(1)
 
+        if output != 0:
+            raise SystemExit(1)
+
     def get_file_size(self, file: Path) -> str:
         """ Get the local file size and converted to units. """
         size: int = file.stat().st_size
         return self.convert_file_sizes(size)
 
     @staticmethod
     def convert_file_sizes(size: int) -> str:
@@ -186,10 +190,22 @@
     def is_binary_repo(self, repo: str) -> bool:
         """ Checks if the repository is binary. """
         if repo in tuple(self.repos.repositories.keys())[2:]:
             return True
 
     @staticmethod
     def change_owner_privileges(folder: Path):
+        """ Changes thw owner privileges. """
         os.chown(folder, 0, 0)
         for file in os.listdir(folder):
             os.chown(Path(folder, file), 0, 0)
+
+    @staticmethod
+    def case_insensitive_pattern_matching(packages: list, data: dict) -> list:
+        """ Case-insensitive pattern matching packages. """
+        repo_packages: tuple = tuple(data.keys())
+        for package in packages:
+            for pkg in repo_packages:
+                if package == pkg.lower():
+                    packages.append(pkg)
+                    packages.remove(package)
+        return packages
```

### Comparing `slpkg-4.8.3/slpkg/dependees.py` & `slpkg-4.8.4/slpkg/dependees.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         for package in self.packages:
             dependees: dict = dict(self.find_requires(package))
             self.view_the_main_package(package)
             self.view_no_dependees(dependees)
             self.view_dependees(dependees)
             self.view_summary_of_dependees(dependees, package)
 
-    def set_the_package_version(self, package: str):
+    def set_the_package_version(self, package: str) -> None:
         self.package_version: str = self.data[package]['version']
 
     def find_requires(self, package: str) -> Generator:
         """ Find requires that package dependees. """
         for name, data in self.data.items():
             if package in data['requires'].split():
                 yield name, data['requires']
@@ -68,19 +68,22 @@
     def view_dependency_line(n: int, dependency: str) -> None:
         str_dependency: str = f"{'':>4}{dependency}"
         if n == 1:
             str_dependency: str = f"{'':>1}{dependency}"
         print(str_dependency)
 
     def view_dependees(self, dependees: dict) -> None:
+        name_length: int = 0
+        if dependees:
+            name_length: int = max(len(name) for name in dependees.keys())
         for n, (name, requires) in enumerate(dependees.items(), start=1):
             dependency: str = f'{self.cyan}{name}{self.endc}'
             if self.option_for_pkg_version:
                 self.set_the_package_version(name)
-                dependency: str = (f'{self.cyan}{name}{self.endc} {self.yellow}'
+                dependency: str = (f'{self.cyan}{name:<{name_length}}{self.endc} {self.yellow}'
                                    f'{self.package_version}{self.endc}')
 
             self.view_dependency_line(n, dependency)
 
             if self.option_for_full_reverse:
                 self.view_full_reverse(n, dependees, requires)
```

### Comparing `slpkg-4.8.3/slpkg/toml_error_message.py` & `slpkg-4.8.4/slpkg/toml_error_message.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/check_updates.py` & `slpkg-4.8.4/slpkg/check_updates.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,17 +93,20 @@
 
         if self.proxy_address.startswith('http'):
             self.set_http_proxy_server()
 
         if self.proxy_address.startswith('socks'):
             self.set_socks_proxy_server()
 
-        repo = self.http.request('GET', repo_chg_txt)
-        if local_chg_txt.is_file():
-            local_size: int = int(os.stat(local_chg_txt).st_size)
+        try:
+            repo = self.http.request('GET', repo_chg_txt)
+            if local_chg_txt.is_file():
+                local_size: int = int(os.stat(local_chg_txt).st_size)
+        except KeyboardInterrupt:
+            raise SystemExit(1)
 
         repo_size: int = int(repo.headers['Content-Length'])
 
         logger = logging.getLogger(LoggingConfig.date_time)
         logger.info(f'{self.__class__.__name__}: '
                     f'{self.__class__.compare_the_changelogs.__name__}: '
                     f'{local_chg_txt=}, {local_size=}, '
@@ -138,24 +141,21 @@
             print(f'\n{self.endc}{self.yellow}No updated packages since the last check.{self.endc}')
 
     def updates(self) -> None:
         message: str = 'Checking for news, please wait...'
 
         # Starting multiprocessing
         p1 = Process(target=self.check_for_updates)
-        p2 = Process(target=self.progress.progress_bar, args=(message, ''))
+        p2 = Process(target=self.progress.progress_bar, args=(message,))
 
         p1.start()
         p2.start()
 
         # Wait until process 1 finish
         p1.join()
 
         # Terminate process 2 if process 1 finished
         if not p1.is_alive():
             p2.terminate()
 
-        # Wait until process 2 finish
-        p2.join()
-
         # Restore the terminal cursor
         print('\x1b[?25h', self.endc)
```

### Comparing `slpkg-4.8.3/slpkg/remove_packages.py` & `slpkg-4.8.4/slpkg/remove_packages.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,149 +4,162 @@
 import os
 import time
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.views.views import ViewMessage
+from slpkg.views.asciibox import AsciiBox
 from slpkg.multi_process import MultiProcess
 from slpkg.models.models import LogsDependencies
 from slpkg.models.models import session as Session
 
 
 class RemovePackages(Configs):
     """ Removes installed packages with dependencies if they installed with
         slpkg install command.
     """
 
     def __init__(self, packages: list, flags: list):
         super(Configs, self).__init__()
         self.packages: list = packages
-        self.flags: list = flags
 
         self.session = Session
         self.dialogbox = DialogBox()
         self.utils = Utilities()
+        self.ascii = AsciiBox()
         self.multi_proc = MultiProcess(flags)
         self.view = ViewMessage(flags)
 
         self.logs_dependencies: dict = {}
-        self.installed_packages: list = []
+        self.packages_for_remove: list = []
         self.installed_dependencies: list = []
         self.dependencies: list = []
+        self.llc: str = self.ascii.lower_left_corner
+        self.hl: str = self.ascii.horizontal_line
 
         self.option_for_resolve_off: bool = self.utils.is_option(
             ['-O', '--resolve-off'], flags)
 
         self.option_for_yes: bool = self.utils.is_option(
             ['-y', '--yes'], flags)
 
     def remove(self) -> None:
         self.query_logs_dependencies()
+        self.add_packages_for_remove()
         self.save_dependencies_for_remove()
         self.remove_doubles_dependencies()
         self.remove_doubles_installed_dependencies()
-        self.add_dependencies_to_remove()
         self.choose_dependencies_for_remove()
-        self.save_packages_for_remove()
+        self.update_installed_dependencies_for_remove()
+        self.add_installed_dependencies_to_remove()
 
         self.view.remove_packages(self.packages, self.dependencies)
         self.view.question()
 
         start: float = time.time()
         self.remove_packages()
         elapsed_time: float = time.time() - start
         self.utils.finished_time(elapsed_time)
 
+    def add_packages_for_remove(self) -> None:
+        for package in self.packages:
+            installed: str = self.utils.is_package_installed(package)
+            if installed:
+                self.packages_for_remove.append(installed)
+
     def save_dependencies_for_remove(self) -> None:
         if not self.option_for_resolve_off:
             for package in self.packages:
                 if self.logs_dependencies.get(package):
                     requires: tuple = self.logs_dependencies[package]
 
                     for require in requires:
                         installed: str = self.utils.is_package_installed(require)
                         if installed and require not in self.packages:
                             self.dependencies.append(require)
-                            self.installed_dependencies.append(installed)
 
     def remove_doubles_dependencies(self) -> None:
         self.dependencies: list = list(set(self.dependencies))
 
     def remove_doubles_installed_dependencies(self):
         self.installed_dependencies: list = list(set(self.installed_dependencies))
 
-    def add_dependencies_to_remove(self) -> None:
-        self.installed_packages.extend(self.installed_dependencies)
+    def update_installed_dependencies_for_remove(self):
+        for dependency in self.dependencies:
+            installed: str = self.utils.is_package_installed(dependency)
+            if installed and dependency not in self.packages:
+                self.installed_dependencies.append(installed)
 
-    def save_packages_for_remove(self) -> None:
-        for package in self.packages:
-            installed: str = self.utils.is_package_installed(package)
-            if installed:
-                self.installed_packages.append(installed)
+    def add_installed_dependencies_to_remove(self) -> None:
+        self.packages_for_remove.extend(self.installed_dependencies)
 
     def remove_packages(self) -> None:
-        for package in self.installed_packages:
+        for package in self.packages_for_remove:
             command: str = f'{self.removepkg} {package}'
             name: str = self.utils.split_package(package)['name']
-            process_message: str = f"package '{name}' to remove"
-            progress_message: str = f'{self.bold}{self.red}Remove{self.endc}'
+            progress_message: str = f'{self.bold}{self.red}Removing{self.endc}'
 
             dependencies: list = self.is_dependency(name)
             if dependencies:
                 self.view_warning_message(dependencies, name)
                 if not self.question_to_remove():
                     continue
 
-            self.multi_proc.process(command, package, process_message, progress_message)
+            self.multi_proc.process(command, package, progress_message)
             self.delete_package_from_logs(name)
 
     def is_dependency(self, name: str) -> list:
         dependencies: list = []
         for package, requires in self.logs_dependencies.items():
             if name in requires and package not in self.packages:
                 dependencies.append(package)
 
         if dependencies:
             return dependencies
 
     def question_to_remove(self) -> bool:
         if not self.option_for_yes and self.ask_question:
-            answer: str = input('\nDo you want to remove? [y/N] ')
+            answer: str = input(f'\nDo you want to remove? [y/N] ')
             if answer in ['Y', 'y']:
+                print()
                 return True
             print()
 
     def view_warning_message(self, dependencies: list, name: str) -> None:
-        print(f"\n{self.bold}{self.violet}WARNING!{self.endc}: The package '{self.red}{name}{self.endc}' "
-              f"is a dependency for the packages:")
-        for dependency in dependencies:
-            print(f"{self.cyan:>16}-> {dependency}{self.endc}")
+        print(f"\n{'':>2}{self.bold}{self.bred}{self.ascii.bullet} {name}{self.endc}: is a dependency in the packages:")
+        print(f"{'':>5}{self.llc}{self.hl}", end='')
+        for i, dependency in enumerate(dependencies, start=1):
+            if i == 1:
+                print(f"{'':>1}{self.cyan}{dependency}{self.endc}")
+            if i > 1:
+                print(f"{'':>8}{self.cyan}{dependency}{self.endc}")
 
     def query_logs_dependencies(self) -> None:
         package_requires: tuple = self.session.query(
             LogsDependencies.name, LogsDependencies.requires).all()
         for package in package_requires:
             self.logs_dependencies[package[0]] = package[1].split()
 
     def delete_package_from_logs(self, package) -> None:
         if not self.option_for_resolve_off:
             self.session.query(LogsDependencies).filter(
                 LogsDependencies.name == package).delete()
             self.session.commit()
 
     def choose_dependencies_for_remove(self) -> None:
-        height: int = 10
-        width: int = 70
-        list_height: int = 0
-        choices: list = []
-        title: str = " Choose dependencies you want to remove "
-
-        for package in self.dependencies:
-            installed_package: str = self.utils.is_package_installed(package)
-            installed_version: str = self.utils.split_package(installed_package)['version']
-            choices.extend([(package, installed_version, True, f'Package: {installed_package}')])
-
-        text: str = f'There are {len(choices)} dependencies:'
-        code, self.dependencies = self.dialogbox.checklist(text, self.dependencies, title, height,
-                                                           width, list_height, choices)
-        os.system('clear')
+        if self.dependencies:
+            height: int = 10
+            width: int = 70
+            list_height: int = 0
+            choices: list = []
+            title: str = " Choose dependencies you want to remove "
+
+            for package in self.dependencies:
+                installed_package: str = self.utils.is_package_installed(package)
+                installed_version: str = self.utils.split_package(installed_package)['version']
+                choices.extend([(package, installed_version, True, f'Package: {installed_package}')])
+
+            text: str = f'There are {len(choices)} dependencies:'
+            code, self.dependencies = self.dialogbox.checklist(text, self.dependencies, title, height,
+                                                               width, list_height, choices)
+            os.system('clear')
```

### Comparing `slpkg-4.8.3/slpkg/blacklist.py` & `slpkg-4.8.4/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/download_only.py` & `slpkg-4.8.4/slpkg/download_only.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/tracking.py` & `slpkg-4.8.4/slpkg/tracking.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/logging_config.py` & `slpkg-4.8.4/slpkg/logging_config.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/main.py` & `slpkg-4.8.4/slpkg/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,24 +72,31 @@
         self.flag_short_search: str = '-S'
         self.flag_no_silent: str = '--no-silent'
         self.flag_short_no_silent: str = '-n'
         self.flag_pkg_version: str = '--pkg-version'
         self.flag_short_pkg_version: str = '-p'
         self.flag_parallel: str = '--parallel'
         self.flag_short_parallel: str = '-P'
+        self.flag_no_case: str = '--no-case'
+        self.flag_short_no_case: str = '-m'
         self.flag_repository: str = '--repository='
         self.flag_short_repository: str = '-o'
         self.flag_directory: str = '--directory='
         self.flag_short_directory: str = '-z'
 
         self.flag_searches: list = [
             self.flag_short_search,
             self.flag_search
         ]
 
+        self.flag_no_cases: list = [
+            self.flag_no_case,
+            self.flag_short_no_case
+        ]
+
         self.options: list = [
             self.flag_yes,
             self.flag_short_yes,
             self.flag_jobs,
             self.flag_short_jobs,
             self.flag_resolve_off,
             self.flag_short_resolve_off,
@@ -105,14 +112,16 @@
             self.flag_short_search,
             self.flag_no_silent,
             self.flag_short_no_silent,
             self.flag_pkg_version,
             self.flag_short_pkg_version,
             self.flag_parallel,
             self.flag_short_parallel,
+            self.flag_no_case,
+            self.flag_short_no_case,
             self.flag_repository,
             self.flag_short_repository,
             self.flag_directory,
             self.flag_short_directory,
         ]
 
         self.commands: dict = {
@@ -173,15 +182,17 @@
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_no_silent,
                 self.flag_short_no_silent,
                 self.flag_repository,
                 self.flag_short_repository,
                 self.flag_parallel,
-                self.flag_short_parallel
+                self.flag_short_parallel,
+                self.flag_no_case,
+                self.flag_short_no_case
             ],
             'install': [
                 self.flag_yes,
                 self.flag_short_yes,
                 self.flag_jobs,
                 self.flag_short_jobs,
                 self.flag_resolve_off,
@@ -193,73 +204,87 @@
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_no_silent,
                 self.flag_short_no_silent,
                 self.flag_repository,
                 self.flag_short_repository,
                 self.flag_parallel,
-                self.flag_short_parallel
+                self.flag_short_parallel,
+                self.flag_no_case,
+                self.flag_short_no_case
             ],
             'download': [
                 self.flag_yes,
                 self.flag_short_yes,
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_directory,
                 self.flag_short_directory,
                 self.flag_repository,
                 self.flag_short_repository,
                 self.flag_parallel,
-                self.flag_short_parallel
+                self.flag_short_parallel,
+                self.flag_no_case,
+                self.flag_short_no_case
             ],
             'remove': [
                 self.flag_yes,
                 self.flag_short_yes,
                 self.flag_resolve_off,
                 self.flag_short_resolve_off,
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_no_silent,
                 self.flag_short_no_silent,
             ],
             'find': [
                 self.flag_search,
                 self.flag_short_search,
+                self.flag_no_case,
+                self.flag_short_no_case
             ],
             'view': [
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_repository,
                 self.flag_short_repository,
                 self.flag_pkg_version,
-                self.flag_short_pkg_version
+                self.flag_short_pkg_version,
+                self.flag_no_case,
+                self.flag_short_no_case
             ],
             'search': [
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_repository,
-                self.flag_short_repository
+                self.flag_short_repository,
+                self.flag_no_case,
+                self.flag_short_no_case
             ],
             'dependees': [
                 self.flag_full_reverse,
                 self.flag_short_full_reverse,
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_repository,
                 self.flag_short_repository,
                 self.flag_pkg_version,
-                self.flag_short_pkg_version
+                self.flag_short_pkg_version,
+                self.flag_no_case,
+                self.flag_short_no_case
             ],
             'tracking': [
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_pkg_version,
                 self.flag_short_pkg_version,
                 self.flag_repository,
-                self.flag_short_repository
+                self.flag_short_repository,
+                self.flag_no_case,
+                self.flag_short_no_case
             ]
         }
 
         self.commands['-h'] = self.commands['--help']
         self.commands['-v'] = self.commands['--version']
         self.commands['-u'] = self.commands['update']
         self.commands['-U'] = self.commands['upgrade']
@@ -587,14 +612,17 @@
     def build(self) -> None:
         command: str = Argparse.build.__name__
 
         if len(self.args) >= 2:
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
+            if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
+                packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
+
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             self.check.package_exists_in_the_database(packages)
             self.check.is_package_unsupported(packages)
 
             if self.repository in list(self.repos.repositories.keys())[:2]:
@@ -611,38 +639,42 @@
     def install(self) -> None:
         command: str = Argparse.install.__name__
 
         if len(self.args) >= 2:
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
+            if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
+                packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
+
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            if self.is_binary:
-                self.check.package_exists_in_the_database(packages)
+            self.check.package_exists_in_the_database(packages)
 
+            if self.is_binary:
                 install = Packages(self.repository, self.data, packages, self.flags, mode=command)
                 install.execute()
             else:
-                self.check.package_exists_in_the_database(packages)
                 self.check.is_package_unsupported(packages)
-
                 install = Slackbuilds(self.repository, self.data, packages, self.flags, mode=command)
                 install.execute()
             raise SystemExit()
         self.usage.help_short(1)
 
     def download(self) -> None:
         command: str = Argparse.download.__name__
 
         if len(self.args) >= 2:
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
+            if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
+                packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
+
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             self.check.package_exists_in_the_database(packages)
             down_only = DownloadOnly(self.directory, self.flags, self.data, self.repository)
             down_only.packages(packages)
             raise SystemExit()
@@ -667,29 +699,35 @@
     def find(self) -> None:
         command: str = Argparse.find.__name__
 
         if len(self.args) >= 2:
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
+            if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
+                packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
+
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            find = FindInstalled(packages)
+            find = FindInstalled(self.flags, packages)
             find.find()
             raise SystemExit()
         self.usage.help_short(1)
 
     def view(self) -> None:
         command: str = Argparse.view.__name__
 
         if len(self.args) >= 2:
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
+            if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
+                packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
+
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             self.check.package_exists_in_the_database(packages)
 
             view = ViewPackage(self.flags, self.repository)
 
@@ -703,29 +741,35 @@
     def search(self) -> None:
         command: str = Argparse.search.__name__
 
         if len(self.args) >= 2:
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
+            if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
+                packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
+
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            pkgs = SearchPackage(self.data, packages, self.repository)
+            pkgs = SearchPackage(self.flags, self.data, packages, self.repository)
             pkgs.search()
             raise SystemExit()
         self.usage.help_short(1)
 
     def dependees(self) -> None:
         command: str = Argparse.dependees.__name__
 
         if len(self.args) >= 2:
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
+            if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
+                packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
+
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             self.check.package_exists_in_the_database(packages)
 
             dependees = Dependees(self.data, packages, self.flags, self.repository)
             dependees.find()
@@ -735,14 +779,17 @@
     def tracking(self) -> None:
         command: str = Argparse.tracking.__name__
 
         if len(self.args) >= 2:
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
+            if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
+                packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
+
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             self.check.package_exists_in_the_database(packages)
 
             tracking = Tracking(self.data, packages, self.flags, self.repository)
             tracking.package()
```

### Comparing `slpkg-4.8.3/slpkg/find_installed.py` & `slpkg-4.8.4/slpkg/find_installed.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,33 @@
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 
 
 class FindInstalled(Configs):
     """ Find installed packages. """
 
-    def __init__(self, packages: list):
+    def __init__(self, flags: list, packages: list):
         super(Configs, self).__init__()
         self.packages: list = packages
 
         self.utils = Utilities()
         self.matching: list = []
 
+        self.option_for_no_case: bool = self.utils.is_option(
+            ['-m', '--no-case'], flags)
+
     def find(self) -> None:
         self.view_title()
         for pkg in self.packages:
             for package in self.utils.installed_packages.values():
+
+                if self.option_for_no_case:
+                    pkg: str = pkg.lower()
+                    package: str = package.lower()
+
                 if pkg in package or pkg == '*':
                     self.matching.append(package)
         self.matched()
 
     def view_title(self):
         print(f'The list below shows the installed packages '
               f'that contains \'{", ".join([p for p in self.packages])}\' files:\n')
```

### Comparing `slpkg-4.8.3/slpkg/upgrade.py` & `slpkg-4.8.4/slpkg/upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg/search.py` & `slpkg-4.8.4/slpkg/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,31 @@
 from slpkg.repositories import Repositories
 from slpkg.binaries.queries import BinQueries
 
 
 class SearchPackage(Configs):
     """ Search packages from the repositories. """
 
-    def __init__(self, data: dict, packages: list, repository: str):
+    def __init__(self, flags: list, data: dict, packages: list, repository: str):
         super(Configs, self).__init__()
         self.data: dict = data
         self.packages: list = packages
         self.repository: str = repository
 
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.matching: int = 0
         self.data_dict: dict = {}
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
+        self.option_for_no_case: bool = self.utils.is_option(
+            ['-m', '--no-case'], flags)
+
     def search(self) -> None:
         print(f'The list below shows the repo '
               f'packages that contains \'{", ".join([p for p in self.packages])}\':\n')
 
         if self.repository == '*':
             self.search_to_all_repositories()
         else:
@@ -52,25 +55,30 @@
             data: dict = SBoQueries(self.repository).repository_data()
         self.search_for_the_packages(data, self.repository)
 
     def search_for_the_packages(self, data: dict, repo: str) -> None:
         for package in self.packages:
             for name, data_pkg in data.items():
 
+                if self.option_for_no_case:
+                    package: str = package.lower()
+                    name: str = name.lower()
+
                 if package in name or package == '*':
                     self.matching += 1
 
                     self.data_dict[self.matching] = {
                         'repository': repo,
                         'name': name,
                         'version': data_pkg['version']
                     }
 
     def summary_of_searching(self) -> None:
+        name_length: int = max(len(name['name']) for name in self.data_dict.values())
         if self.matching:
             for item in self.data_dict.values():
-                print(f"{item['repository']}: {self.cyan}{item['name']}{self.endc} "
+                print(f"{item['repository']}: {self.cyan}{item['name']:<{name_length}}{self.endc} "
                       f"{self.yellow}{item['version']}{self.endc}")
 
             print(f'\n{self.grey}Total found {self.matching} packages.{self.endc}')
         else:
             print('\nDoes not match any package.\n')
```

### Comparing `slpkg-4.8.3/setup.cfg` & `slpkg-4.8.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = slpkg
-version = 4.8.3
+version = 4.8.4
 license_file = LICENSE
 author = Dimitris Zlatanidis
-author_email = d.zlatanidis@gmail.com
+author_email = dslackw@gmail.com
 description = Package manager utility for Slackware Linux.
 long_description = file:README.rst
 url = https://dslackw.gitlab.io/slpkg/
 project_urls = 
 	Source = https://dslackw.gitlab.io/slpkg/
 	Documentation = https://dslackw.gitlab.io/slpkg/
 classifiers =
```

### Comparing `slpkg-4.8.3/slpkg.egg-info/SOURCES.txt` & `slpkg-4.8.4/slpkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.3/slpkg.egg-info/PKG-INFO` & `slpkg-4.8.4/slpkg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 4.8.3
+Version: 4.8.4
 Summary: Package manager utility for Slackware Linux.
 Home-page: https://dslackw.gitlab.io/slpkg/
 Author: Dimitris Zlatanidis
-Author-email: d.zlatanidis@gmail.com
+Author-email: dslackw@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://dslackw.gitlab.io/slpkg/
 Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
```

### Comparing `slpkg-4.8.3/README.md` & `slpkg-4.8.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 $ slpkg tracking --pkg-version Flask awscli pychess
 ```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_tracking.png" width="900">
 
 ### Installation
 
 ```
-$ tar xvf slpkg-4.8.3.tar.gz
-$ cd slpkg-4.8.3
+$ tar xvf slpkg-4.8.4.tar.gz
+$ cd slpkg-4.8.4
 $ ./install.sh
 ```
 
 ### Requirements
 
 ```
 SQLAlchemy >= 1.4.46
@@ -82,15 +82,15 @@
 
 The majority of trials have been made in Slackware x86_64 'stable' environment.
 
 
 ### Command Line Tool Usage
 
 ```
-slpkg - version 4.8.3
+slpkg - version 4.8.4
 
 USAGE:
   slpkg [COMMAND] [OPTIONS] [FILELIST|PACKAGES...]
 
 DESCRIPTION:
   Package manager utility for Slackware.
 
@@ -99,41 +99,43 @@
   -U, upgrade                   Upgrade all the packages.
   -c, check-updates             Check for news on ChangeLog.txt.
   -I, repo-info                 Prints the repositories information.
   -g, configs                   Edit the configuration file.
   -L, clean-logs                Clean dependencies log tracking.
   -T, clean-data                Clean all the repositories data.
   -D, clean-tmp                 Delete all the downloaded sources.
-  -b, build [packages...]       Build only the packages.
-  -i, install [packages...]     Build and install the packages.
-  -R, remove [packages...]      Remove installed packages.
-  -d, download [packages...]    Download only the scripts and sources.
-  -f, find [packages...]        Find installed packages.
-  -w, view [packages...]        View packages from the repository.
-  -s, search [packages...]      Search packages from the repository.
-  -e, dependees [packages...]   Show which packages depend on.
-  -t, tracking [packages...]    Tracking the packages dependencies.
+  -b, build [PACKAGES...]       Build only the packages.
+  -i, install [PACKAGES...]     Build and install the packages.
+  -R, remove [PACKAGES...]      Remove installed packages.
+  -d, download [PACKAGES...]    Download only the scripts and sources.
+  -f, find [PACKAGES...]        Find installed packages.
+  -w, view [PACKAGES...]        View packages from the repository.
+  -s, search [PACKAGES...]      Search packages from the repository.
+  -e, dependees [PACKAGES...]   Show which packages depend on.
+  -t, tracking [PACKAGES...]    Tracking the packages dependencies.
 
 OPTIONS:
   -y, --yes                     Answer Yes to all questions.
   -j, --jobs                    Set it for multicore systems.
   -O, --resolve-off             Turns off dependency resolving.
   -r, --reinstall               Upgrade packages of the same version.
   -k, --skip-installed          Skip installed packages.
   -a, --install-data            Install data into the database only.
   -E, --full-reverse            Full reverse dependency.
   -S, --search                  Search packages from the repository.
   -n, --no-silent               Disable silent mode.
   -p, --pkg-version             Print the repository package version.
   -P, --parallel                Download files in parallel.
+  -m, --no-case                 Case-insensitive pattern matching.
   -o, --repository=NAME         Change repository you want to work.
   -z, --directory=PATH          Download files to a specific path.
 
   -h, --help                    Show this message and exit.
   -v, --version                 Print version and exit.
+
 ```
 
 
 ### How to start
 
 If you are going to use only the [SlackBuilds.org](https://slackbuilds.org) repository, you don't need to edit
 the `/etc/slpkg/repositories.toml` file, otherwise edit the file and set `true` the repositories you want.
```

### Comparing `slpkg-4.8.3/tools/gen_sbo_txt.sh` & `slpkg-4.8.4/tools/gen_sbo_txt.sh`

 * *Files identical despite different names*

