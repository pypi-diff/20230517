# Comparing `tmp/dcspy-1.9.5.tar.gz` & `tmp/dcspy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcspy-1.9.5.tar", last modified: Mon Feb 13 15:50:25 2023, max compression
+gzip compressed data, was "dcspy-2.0.0.tar", last modified: Wed May 17 11:21:43 2023, max compression
```

## Comparing `dcspy-1.9.5.tar` & `dcspy-2.0.0.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:50:25.544875 dcspy-1.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-02-13 15:50:12.000000 dcspy-1.9.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-02-13 15:50:12.000000 dcspy-1.9.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-02-13 15:50:12.000000 dcspy-1.9.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-13 15:50:12.000000 dcspy-1.9.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-13 15:50:12.000000 dcspy-1.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15821 2023-02-13 15:50:25.544875 dcspy-1.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-02-13 15:50:12.000000 dcspy-1.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-13 15:50:12.000000 dcspy-1.9.5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:50:25.544875 dcspy-1.9.5/dcspy/
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/G13.png
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/G15v1.png
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/G15v2.png
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/G19.png
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/G510.png
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53899 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/aircraft.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/dcsbios.py
--rw-r--r--   0 runner    (1001) docker     (123)    23535 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/dcspy.ico
--rw-r--r--   0 runner    (1001) docker     (123)    35819 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/dcspy.png
--rw-r--r--   0 runner    (1001) docker     (123)    21792 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/dcspy_white.ico
--rw-r--r--   0 runner    (1001) docker     (123)    20420 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/falconded.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/logitech.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:50:25.544875 dcspy-1.9.5/dcspy/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/sdk/lcd_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/sdk/led_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/starter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32430 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/tk_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-02-13 15:50:12.000000 dcspy-1.9.5/dcspy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:50:25.544875 dcspy-1.9.5/dcspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15821 2023-02-13 15:50:25.000000 dcspy-1.9.5/dcspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-02-13 15:50:25.000000 dcspy-1.9.5/dcspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 15:50:25.000000 dcspy-1.9.5/dcspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-13 15:50:25.000000 dcspy-1.9.5/dcspy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-13 15:50:25.000000 dcspy-1.9.5/dcspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-13 15:50:25.000000 dcspy-1.9.5/dcspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-02-13 15:50:12.000000 dcspy-1.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-13 15:50:12.000000 dcspy-1.9.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-13 15:50:12.000000 dcspy-1.9.5/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-02-13 15:50:25.548875 dcspy-1.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-13 15:50:12.000000 dcspy-1.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:50:25.544875 dcspy-1.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23394 2023-02-13 15:50:12.000000 dcspy-1.9.5/tests/test_aircraft.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-13 15:50:12.000000 dcspy-1.9.5/tests/test_bios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-02-13 15:50:12.000000 dcspy-1.9.5/tests/test_dcsbios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-02-13 15:50:12.000000 dcspy-1.9.5/tests/test_lcd_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-02-13 15:50:12.000000 dcspy-1.9.5/tests/test_led_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-02-13 15:50:12.000000 dcspy-1.9.5/tests/test_logitech.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-02-13 15:50:12.000000 dcspy-1.9.5/tests/test_starter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-02-13 15:50:12.000000 dcspy-1.9.5/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:21:43.419128 dcspy-2.0.0/
+-rw-rw-rw-   0        0        0      708 2023-05-17 11:16:07.000000 dcspy-2.0.0/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     9538 2023-05-17 11:16:07.000000 dcspy-2.0.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5348 2023-05-17 11:16:07.000000 dcspy-2.0.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     4371 2023-05-17 11:16:07.000000 dcspy-2.0.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1092 2023-05-17 11:16:07.000000 dcspy-2.0.0/LICENSE.md
+-rw-rw-rw-   0        0        0       75 2023-05-17 11:16:07.000000 dcspy-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    16889 2023-05-17 11:21:43.419128 dcspy-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4776 2023-05-17 11:16:07.000000 dcspy-2.0.0/README.md
+-rw-rw-rw-   0        0        0      346 2023-05-17 11:16:07.000000 dcspy-2.0.0/SECURITY.md
+drwxrwxrwx   0        0        0        0 2023-05-17 11:21:43.403505 dcspy-2.0.0/dcspy/
+-rw-rw-rw-   0        0        0     7792 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/G13.png
+-rw-rw-rw-   0        0        0    11136 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/G15v1.png
+-rw-rw-rw-   0        0        0    11673 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/G15v2.png
+-rw-rw-rw-   0        0        0    13267 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/G19.png
+-rw-rw-rw-   0        0        0    10850 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/G510.png
+-rw-rw-rw-   0        0        0     4512 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/__init__.py
+-rw-rw-rw-   0        0        0    54681 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/aircraft.py
+-rw-rw-rw-   0        0        0      476 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/config.yaml
+-rw-rw-rw-   0        0        0     6160 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/dcsbios.py
+-rw-rw-rw-   0        0        0    23535 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/dcspy.ico
+-rw-rw-rw-   0        0        0    35819 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/dcspy.png
+-rw-rw-rw-   0        0        0    21792 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/dcspy_white.ico
+-rw-rw-rw-   0        0        0    20420 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/falconded.ttf
+-rw-rw-rw-   0        0        0      236 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/license.txt
+-rw-rw-rw-   0        0        0     1235 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/log.py
+-rw-rw-rw-   0        0        0     7433 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/logitech.py
+-rw-rw-rw-   0        0        0        0 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/py.typed
+-rw-rw-rw-   0        0        0     1312 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/run.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:21:43.403505 dcspy-2.0.0/dcspy/sdk/
+-rw-rw-rw-   0        0        0     1409 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/sdk/__init__.py
+-rw-rw-rw-   0        0        0     8629 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/sdk/lcd_sdk.py
+-rw-rw-rw-   0        0        0     8069 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/sdk/led_sdk.py
+-rw-rw-rw-   0        0        0     4318 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/starter.py
+-rw-rw-rw-   0        0        0    41669 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/tk_gui.py
+-rw-rw-rw-   0        0        0    12425 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:21:43.403505 dcspy-2.0.0/dcspy.egg-info/
+-rw-rw-rw-   0        0        0    16889 2023-05-17 11:21:43.000000 dcspy-2.0.0/dcspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2023-05-17 11:21:43.000000 dcspy-2.0.0/dcspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 11:21:43.000000 dcspy-2.0.0/dcspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-17 11:21:43.000000 dcspy-2.0.0/dcspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      221 2023-05-17 11:21:43.000000 dcspy-2.0.0/dcspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-17 11:21:43.000000 dcspy-2.0.0/dcspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1571 2023-05-17 11:21:42.000000 dcspy-2.0.0/file_version_info.txt
+-rw-rw-rw-   0        0        0      535 2023-05-17 11:16:07.000000 dcspy-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      150 2023-05-17 11:16:07.000000 dcspy-2.0.0/requirements.txt
+-rw-rw-rw-   0        0        0      298 2023-05-17 11:16:07.000000 dcspy-2.0.0/requirements_test.txt
+-rw-rw-rw-   0        0        0     3760 2023-05-17 11:21:43.419128 dcspy-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-05-17 11:16:07.000000 dcspy-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:21:43.419128 dcspy-2.0.0/tests/
+-rw-rw-rw-   0        0        0    23841 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_aircraft.py
+-rw-rw-rw-   0        0        0      971 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_bios.py
+-rw-rw-rw-   0        0        0     5193 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_dcsbios.py
+-rw-rw-rw-   0        0        0     5476 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_lcd_sdk.py
+-rw-rw-rw-   0        0        0     3905 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_led_sdk.py
+-rw-rw-rw-   0        0        0     5559 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_logitech.py
+-rw-rw-rw-   0        0        0     1321 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_starter.py
+-rw-rw-rw-   0        0        0     8472 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_utils.py
```

### Comparing `dcspy-1.9.5/CHANGELOG.md` & `dcspy-2.0.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,199 +1,213 @@
-## 1.9.5
-* Support for **Mi-8MTV2 Magnificent Eight**
-  * Autopilot Channels (Heading, Pitch/Bank and Altitude)
-  * Radios: R868, R828, YADRO1A information
-* Support for **Mi-24P Hind**
-  * Autopilot Channels (Yaw, Roll, Pitch and Altitude)
-  * Autopilot Modes (Hover, Route and Altitude)
-  * Radios: R868, R828, YADRO1I information
-* Add About tab with basic information
-* **F-16C Viper**:
-  * Add spacial font for DED (G19 only)
-  * Clean some extra characters from DED
-* Internal:
-  * force update customtkinter to at least 5.1.0
-
-## 1.8.1
-* Add support for **Ka-50 Black Shark III**
-* Update footer when checking DCS-BIOS version
-* Align with DCS 2.8.1.34667.2 and DCS-BIOS 0.7.47
-* Internal:
-  * add more unit tests
-  * mark some test as DCS-BIOS tests
-
-## 1.8.0
-* Major GUI redesign using `customtkinter` package, which provides new, modern widgets:
-  * Appearance system mode (`Light`, `Dark`)
-  * Three colort theme (`Green`, `Blue` and `Dark Blue`)
-  * All settings are configured from GUI vie widgets
-  * One window for all configuration and buttons
-  * Check version from GUI
-  * Add configuration flag to check for new version during start
-
-## 1.7.5
-* report DCS stable version correctly in logs during start
-* Internal:
-  * rename starting script
-  * remove usage of McCabe
-  * add unit tests
-
-## 1.7.4
-* **AH-64D Apache**
-  * add better support for G19 for PRE mode
-  * update name from `AH64D` to `AH64DBLKII`
-* Show DCS version in logs
-* Fix name of plane for **F-14 Tomcat** depending on model A or B
-* Toggle Start/Stop buttons
-* Do not show warning when plane's name is empty
-* Internal:
-  * improve checking DCS-BIOS data
-  * introduce enum values for parser state
-  * improve CI process - add Python 3.11
-  * force using Pillow 9.3.0
-
-## 1.7.3
-* Align **F-16C Viper** DED and **AH-64D Apache** EUFD with DCS-BIOS 0.7.46 changes
-* Basic support for **F-14A Tomcat**
-
-## 1.7.2
-* **AH-64D Apache**
-  * update name from `AH64DBLKII` to `AH64D`
-  * fix display PRE mode for G19
-  * fix handling buttons
-* Internal:
-  * update unit test for better coverage and more use-cases
-
-## 1.7.1
-* New config settings:
-  * `auto_start` - run DCSpy atomically after start
-  * `verbose` - show more logs in terminal/console window
-* Fixing handling of `dcsbios` settings from `config.yaml`
-* Start and stop buttons can be used several times without closing GUI
-* **F-16C Viper**
-  * replace `*` with inverse white circle character at DED
-  * Fix unhandled buttons for G19 (menu, ok and cancel)
-* G19 and **F/A-18C Hornet**
-  * Push **Menu** and **Cancel** toggle cockpit button down, push it again toggles button up (Integrated Fuel/Engine Indicator - IFEI).
-  * Add handling **Ok** as Attitude Selector Switch, INS/AUTO/STBY
-* Internal:
-  * use Pythonic way using temporary directory
-  * speed-up tests - cache json files instead of downloading from internet
-  * use Enum for LCD type
-  * use Enum for LCD buttons, add to LcdInfo dataclass
-
-## 1.7.0
-* Support for **AH-64D Apache** with 3 modes:
-  * `IDM` - Squeeze and shows radios frequencies (from Radio Area), IDM and RTS rocker are used to scroll down
-  * `WCA` - Enter button display warnings, cautions, and advisories, WCA rocker is used to scroll down
-  * `PRE` - Preset button displays the preset menu for the selected radio, WCA rocker is used to scroll down
-* **F-16C Viper** DED clean-up extra characters
-
-## 1.6.1
-* Update **F-16C Viper** for latest DSC-BIOS (0.7.45)
-* Fresh installation of DCS-BIOS is painless
-* Drop support for Python 3.6
-
-## 1.6.0
-* use fonts in dynamic way - you can customize fonts in `config.yaml` file (see [Configuration](https://github.com/emcek/dcspy#configuration))
-* usage for LCD SDK built-in LGS - no need additional package for usage
-* support for Python 3.10 (use `dataclasses` internally)
-* ability to stop DCSpy from GUI
-* supporters are printed in welcome screen - I'm thrilled with support and help of community!
-
-## 1.5.1
-* alignment for new DCS-BIOS [v0.7.43](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.43)
-
-## 1.5.0
-* Support for **AV-8B N/A Harrier** with:
-  * **UFC** - Up Front Controller
-  * **ODU** - Option Display Unit
-  * **decrease UFC Comm 1 Channel** - G13 1st button or G19 left button
-  * **increase UFC Comm 1 Channel** - G13 2nd button or G19 right button
-  * **decrease UFC Comm 2 Channel** - G13 3rd button or G19 down button
-  * **increase UFC Comm 2 Channel** - G13 4th button or G19 up button
-
-## 1.4.0
-* Configuration editor:
-  * **dcsbios** - set default Logitech keyboard: "G19", "G510", "G15 v1/v2", "G13"
-  * **show_gui** - showing or hiding GUI during start of DCSpy
-  * **dcsbios** - location of DCS-BIOS folder inside user's Saved Games
-* Check and update DCS-BIOS directly from DCSpy
-  * **Check DCS-BIOS** button in **Config** editor
-  * **dcsbios** needs to be set to correct value
-* Basic A-10C Warthog and A-10C II Tank Killer support
-
-## 1.3.0
-* **F-16C Viper** use 4 buttons for IFF
-  * **IFF MASTER Knob** - OFF/STBY/LOW/NORM/EMER
-  * **IFF ENABLE Switch** - M1/M3 /OFF/ M3/MS
-  * **IFF M-4 CODE Switch** - HOLD/ A/B /ZERO
-  * **IFF MODE 4 REPLY Switch** - OUT/A/B
-* Fix alignment of (DCS-BIOS [v0.7.41](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.41)) for **F-14B Tomcat**
-* Internally all data fetch form DCS-BIOS is check against its specification. Sometimes due to changes DCS-BIOS protocol DCSpy couldn't fetch all data i.e. F-16 DED. It shouldn't happened anymore.
-
-## 1.2.3
-* Fix alignment of DED (DCS-BIOS [v0.7.41](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.43)) for **F-16C Viper**
-
-## 1.2.2
-* Fix alignment of DED for **F-16C Viper**
-* Fix position of Integrated Fuel/Engine Indicator (IFEI) for **F/A-18C Hornet** (only G19)
-
-## 1.2.1
-* **F/A-18C Hornet** shows extra Total Internal Fuel (G19 only)
-* Internal refactoring
-
-## 1.2.0
-* Simple Tkinter GUI - to select your Logitech keyboard
-* Support for G19 - Big thanks for **BrotherBloat** who makes this release possible. He spent countless hours to share his G19 and let me troubleshoot remotely.
-* **F/A-18C Hornet** shows Total Fuel instead of Total Internal Fuel
-
-## 1.1.1
-* Basic support for **F-14B Tomcat** RIO CAP (Computer Address Panel):
-  * **CLEAR** - button 1
-  * **S-W** - button 2
-  * **N+E** - button 3
-  * **ENTER** - button 4
-
-## 1.1.0
-* dcspy use now UDP multicast connection do DCS-BIOS, since each TCP connection slightly increases the amount of work that is performed inside of DCS (blocking the rest of the simulation).
-* support for integer data to be fetch from DCS-BIOS - using IntegerBuffer()
-* bios_data in Airplanes instances allow both StringBuffer() and IntegerBuffer()
-* reformat waiting time before DCS connected
-* fix Data Entry Display for F-16C Viper - DCS-BIOS [v0.7.34](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.34) is required
-* **Ka-50 Black Shark** - Autopilot channels show up in LCD
-
-## 1.0.0
-* **Ka-50 Black Shark** data from PVI-800 shows (in similar boxes) on LCD
-* ProtocolParser for DCS-BIOS has new optimized state machine
-  * LCD SDK is re-written from scratch:
-  * low and high level API
-  * auto-loading C library during importing
-  * all API is type annotated and well documented
-  * move loading LCD C library from G13 handler
-*internal:
-  * refactoring and rename internals of G13 handler module
-  * add unit tests
-
-## 0.9.2
-* LCD prints current waiting time to connect to DCS
-* when DCS exit from plane/mission exception is catch and handle correctly
-* lots of internal changes, preparing for new features, most important:
-  * change structure of AircraftHandler, move subscription to DCS-BIOS changes out of planes
-  * update and clear methods move from G13 handler to LCD SDK
-
-## 0.9.1
-* G13 handler have display property to send text to LCD
-* rename starting script to dcspy.exe
-* starting script now show waiting time for DCS connection
-* minor code optimization and refactoring
-
-## 0.9.0
-* based on version [specelUFC v1.12.1](https://github.com/specel/specelUFC/releases/tag/v1.12.1)
-* added basic handling for Ka-50 PVI-800 data are received but not formatted properly
-* F-16C DED should working but not 4 buttons under LCD - I don't have it so it is hard to test
-* G13 handler detect 32/64 bit of Python and load correct version of LCD Logitech C library
-* adding basic logging for debugging - prints on console
-* all defined aircraft are detected and loaded on-the-fly during operation
-* define new plane should be easy just use AircraftHandler as base class
-* Python LCD SDK was clean-up
-* other refactorings and code duplication removal
+## 2.0.0
+* Allow use/update [live DCS-BIOS](https://github.com/emcek/dcspy/wiki/Information#live-dcs-bios) directly from GitHub (master branch)
+* Allow run DCSpy without console
+* Auto [screenshot of LCD](https://github.com/emcek/dcspy/wiki/Usage#advanced) during operation
+* Auto save change options from GUI
+* Fix problem when DCS-BIOS is empty or drive letter not exists
+* Generate [standalone version](https://github.com/emcek/dcspy/wiki/Installation#single-file-download-new-way) with PyInstaller
+* Save configuration in user local directory (preserved between updates)
+* Internal:
+  * improve type checking
+  * verbose setting will impact both console and file logs
+  * use pathlib for path manipulation
+  * improve CI/CD process
+
+## 1.9.5
+* Support for **Mi-8MTV2 Magnificent Eight**
+  * Autopilot Channels (Heading, Pitch/Bank and Altitude)
+  * Radios: R868, R828, YADRO1A information
+* Support for **Mi-24P Hind**
+  * Autopilot Channels (Yaw, Roll, Pitch and Altitude)
+  * Autopilot Modes (Hover, Route and Altitude)
+  * Radios: R868, R828, YADRO1I information
+* Add About tab with basic information
+* **F-16C Viper**:
+  * Add spacial font for DED (G19 only)
+  * Clean some extra characters from DED
+* Internal:
+  * force update customtkinter to at least 5.1.0
+
+## 1.8.1
+* Add support for **Ka-50 Black Shark III**
+* Update footer when checking DCS-BIOS version
+* Align with DCS 2.8.1.34667.2 and DCS-BIOS 0.7.47
+* Internal:
+  * add more unit tests
+  * mark some test as DCS-BIOS tests
+
+## 1.8.0
+* Major GUI redesign using `customtkinter` package, which provides new, modern widgets:
+  * Appearance system mode (`Light`, `Dark`)
+  * Three colort theme (`Green`, `Blue` and `Dark Blue`)
+  * All settings are configured from GUI vie widgets
+  * One window for all configuration and buttons
+  * Check version from GUI
+  * Add configuration flag to check for new version during start
+
+## 1.7.5
+* report DCS stable version correctly in logs during start
+* Internal:
+  * rename starting script
+  * remove usage of McCabe
+  * add unit tests
+
+## 1.7.4
+* **AH-64D Apache**
+  * add better support for G19 for PRE mode
+  * update name from `AH64D` to `AH64DBLKII`
+* Show DCS version in logs
+* Fix name of plane for **F-14 Tomcat** depending on model A or B
+* Toggle Start/Stop buttons
+* Do not show warning when plane's name is empty
+* Internal:
+  * improve checking DCS-BIOS data
+  * introduce enum values for parser state
+  * improve CI process - add Python 3.11
+  * force using Pillow 9.3.0
+
+## 1.7.3
+* Align **F-16C Viper** DED and **AH-64D Apache** EUFD with DCS-BIOS 0.7.46 changes
+* Basic support for **F-14A Tomcat**
+
+## 1.7.2
+* **AH-64D Apache**
+  * update name from `AH64DBLKII` to `AH64D`
+  * fix display PRE mode for G19
+  * fix handling buttons
+* Internal:
+  * update unit test for better coverage and more use-cases
+
+## 1.7.1
+* New config settings:
+  * `auto_start` - run DCSpy atomically after start
+  * `verbose` - show more logs in terminal/console window
+* Fixing handling of `dcsbios` settings from `config.yaml`
+* Start and stop buttons can be used several times without closing GUI
+* **F-16C Viper**
+  * replace `*` with inverse white circle character at DED
+  * Fix unhandled buttons for G19 (menu, ok and cancel)
+* G19 and **F/A-18C Hornet**
+  * Push **Menu** and **Cancel** toggle cockpit button down, push it again toggles button up (Integrated Fuel/Engine Indicator - IFEI).
+  * Add handling **Ok** as Attitude Selector Switch, INS/AUTO/STBY
+* Internal:
+  * use Pythonic way using temporary directory
+  * speed-up tests - cache json files instead of downloading from internet
+  * use Enum for LCD type
+  * use Enum for LCD buttons, add to LcdInfo dataclass
+
+## 1.7.0
+* Support for **AH-64D Apache** with 3 modes:
+  * `IDM` - Squeeze and shows radios frequencies (from Radio Area), IDM and RTS rocker are used to scroll down
+  * `WCA` - Enter button display warnings, cautions, and advisories, WCA rocker is used to scroll down
+  * `PRE` - Preset button displays the preset menu for the selected radio, WCA rocker is used to scroll down
+* **F-16C Viper** DED clean-up extra characters
+
+## 1.6.1
+* Update **F-16C Viper** for latest DSC-BIOS (0.7.45)
+* Fresh installation of DCS-BIOS is painless
+* Drop support for Python 3.6
+
+## 1.6.0
+* use fonts in dynamic way - you can customize fonts in `config.yaml` file (see [Configuration](https://github.com/emcek/dcspy#configuration))
+* usage for LCD SDK built-in LGS - no need additional package for usage
+* support for Python 3.10 (use `dataclasses` internally)
+* ability to stop DCSpy from GUI
+* supporters are printed in welcome screen - I'm thrilled with support and help of community!
+
+## 1.5.1
+* alignment for new DCS-BIOS [v0.7.43](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.43)
+
+## 1.5.0
+* Support for **AV-8B N/A Harrier** with:
+  * **UFC** - Up Front Controller
+  * **ODU** - Option Display Unit
+  * **decrease UFC Comm 1 Channel** - G13 1st button or G19 left button
+  * **increase UFC Comm 1 Channel** - G13 2nd button or G19 right button
+  * **decrease UFC Comm 2 Channel** - G13 3rd button or G19 down button
+  * **increase UFC Comm 2 Channel** - G13 4th button or G19 up button
+
+## 1.4.0
+* Configuration editor:
+  * **dcsbios** - set default Logitech keyboard: "G19", "G510", "G15 v1/v2", "G13"
+  * **show_gui** - showing or hiding GUI during start of DCSpy
+  * **dcsbios** - location of DCS-BIOS folder inside user's Saved Games
+* Check and update DCS-BIOS directly from DCSpy
+  * **Check DCS-BIOS** button in **Config** editor
+  * **dcsbios** needs to be set to correct value
+* Basic A-10C Warthog and A-10C II Tank Killer support
+
+## 1.3.0
+* **F-16C Viper** use 4 buttons for IFF
+  * **IFF MASTER Knob** - OFF/STBY/LOW/NORM/EMER
+  * **IFF ENABLE Switch** - M1/M3 /OFF/ M3/MS
+  * **IFF M-4 CODE Switch** - HOLD/ A/B /ZERO
+  * **IFF MODE 4 REPLY Switch** - OUT/A/B
+* Fix alignment of (DCS-BIOS [v0.7.41](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.41)) for **F-14B Tomcat**
+* Internally all data fetch form DCS-BIOS is check against its specification. Sometimes due to changes DCS-BIOS protocol DCSpy couldn't fetch all data i.e. F-16 DED. It shouldn't happened anymore.
+
+## 1.2.3
+* Fix alignment of DED (DCS-BIOS [v0.7.41](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.43)) for **F-16C Viper**
+
+## 1.2.2
+* Fix alignment of DED for **F-16C Viper**
+* Fix position of Integrated Fuel/Engine Indicator (IFEI) for **F/A-18C Hornet** (only G19)
+
+## 1.2.1
+* **F/A-18C Hornet** shows extra Total Internal Fuel (G19 only)
+* Internal refactoring
+
+## 1.2.0
+* Simple Tkinter GUI - to select your Logitech keyboard
+* Support for G19 - Big thanks for **BrotherBloat** who makes this release possible. He spent countless hours to share his G19 and let me troubleshoot remotely.
+* **F/A-18C Hornet** shows Total Fuel instead of Total Internal Fuel
+
+## 1.1.1
+* Basic support for **F-14B Tomcat** RIO CAP (Computer Address Panel):
+  * **CLEAR** - button 1
+  * **S-W** - button 2
+  * **N+E** - button 3
+  * **ENTER** - button 4
+
+## 1.1.0
+* dcspy use now UDP multicast connection do DCS-BIOS, since each TCP connection slightly increases the amount of work that is performed inside of DCS (blocking the rest of the simulation).
+* support for integer data to be fetch from DCS-BIOS - using IntegerBuffer()
+* bios_data in Airplanes instances allow both StringBuffer() and IntegerBuffer()
+* reformat waiting time before DCS connected
+* fix Data Entry Display for F-16C Viper - DCS-BIOS [v0.7.34](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.34) is required
+* **Ka-50 Black Shark** - Autopilot channels show up in LCD
+
+## 1.0.0
+* **Ka-50 Black Shark** data from PVI-800 shows (in similar boxes) on LCD
+* ProtocolParser for DCS-BIOS has new optimized state machine
+  * LCD SDK is re-written from scratch:
+  * low and high level API
+  * auto-loading C library during importing
+  * all API is type annotated and well documented
+  * move loading LCD C library from G13 handler
+*internal:
+  * refactoring and rename internals of G13 handler module
+  * add unit tests
+
+## 0.9.2
+* LCD prints current waiting time to connect to DCS
+* when DCS exit from plane/mission exception is catch and handle correctly
+* lots of internal changes, preparing for new features, most important:
+  * change structure of AircraftHandler, move subscription to DCS-BIOS changes out of planes
+  * update and clear methods move from G13 handler to LCD SDK
+
+## 0.9.1
+* G13 handler have display property to send text to LCD
+* rename starting script to dcspy.exe
+* starting script now show waiting time for DCS connection
+* minor code optimization and refactoring
+
+## 0.9.0
+* based on version [specelUFC v1.12.1](https://github.com/specel/specelUFC/releases/tag/v1.12.1)
+* added basic handling for Ka-50 PVI-800 data are received but not formatted properly
+* F-16C DED should working but not 4 buttons under LCD - I don't have it so it is hard to test
+* G13 handler detect 32/64 bit of Python and load correct version of LCD Logitech C library
+* adding basic logging for debugging - prints on console
+* all defined aircraft are detected and loaded on-the-fly during operation
+* define new plane should be easy just use AircraftHandler as base class
+* Python LCD SDK was clean-up
+* other refactorings and code duplication removal
```

### Comparing `dcspy-1.9.5/CODE_OF_CONDUCT.md` & `dcspy-2.0.0/CODE_OF_CONDUCT.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-# Contributor Covenant Code of Conduct
-
-## Our Pledge
-
-We as members, contributors, and leaders pledge to make participation in our
-community a harassment-free experience for everyone, regardless of age, body
-size, visible or invisible disability, ethnicity, sex characteristics, gender
-identity and expression, level of experience, education, socio-economic status,
-nationality, personal appearance, race, religion, or sexual identity
-and orientation.
-
-We pledge to act and interact in ways that contribute to an open, welcoming,
-diverse, inclusive, and healthy community.
-
-## Our Standards
-
-Examples of behavior that contributes to a positive environment for our
-community include:
-
-* Demonstrating empathy and kindness toward other people
-* Being respectful of differing opinions, viewpoints, and experiences
-* Giving and gracefully accepting constructive feedback
-* Accepting responsibility and apologizing to those affected by our mistakes,
-  and learning from the experience
-* Focusing on what is best not just for us as individuals, but for the
-  overall community
-
-Examples of unacceptable behavior include:
-
-* The use of sexualized language or imagery, and sexual attention or
-  advances of any kind
-* Trolling, insulting or derogatory comments, and personal or political attacks
-* Public or private harassment
-* Publishing others' private information, such as a physical or email
-  address, without their explicit permission
-* Other conduct which could reasonably be considered inappropriate in a
-  professional setting
-
-## Enforcement Responsibilities
-
-Community leaders are responsible for clarifying and enforcing our standards of
-acceptable behavior and will take appropriate and fair corrective action in
-response to any behavior that they deem inappropriate, threatening, offensive,
-or harmful.
-
-Community leaders have the right and responsibility to remove, edit, or reject
-comments, commits, code, wiki edits, issues, and other contributions that are
-not aligned to this Code of Conduct, and will communicate reasons for moderation
-decisions when appropriate.
-
-## Scope
-
-This Code of Conduct applies within all community spaces, and also applies when
-an individual is officially representing the community in public spaces.
-Examples of representing our community include using an official e-mail address,
-posting via an official social media account, or acting as an appointed
-representative at an online or offline event.
-
-## Enforcement
-
-Instances of abusive, harassing, or otherwise unacceptable behavior may be
-reported to the community leaders responsible for enforcement at
-mplichta@gmail.com.
-All complaints will be reviewed and investigated promptly and fairly.
-
-All community leaders are obligated to respect the privacy and security of the
-reporter of any incident.
-
-## Enforcement Guidelines
-
-Community leaders will follow these Community Impact Guidelines in determining
-the consequences for any action they deem in violation of this Code of Conduct:
-
-### 1. Correction
-
-**Community Impact**: Use of inappropriate language or other behavior deemed
-unprofessional or unwelcome in the community.
-
-**Consequence**: A private, written warning from community leaders, providing
-clarity around the nature of the violation and an explanation of why the
-behavior was inappropriate. A public apology may be requested.
-
-### 2. Warning
-
-**Community Impact**: A violation through a single incident or series
-of actions.
-
-**Consequence**: A warning with consequences for continued behavior. No
-interaction with the people involved, including unsolicited interaction with
-those enforcing the Code of Conduct, for a specified period of time. This
-includes avoiding interactions in community spaces as well as external channels
-like social media. Violating these terms may lead to a temporary or
-permanent ban.
-
-### 3. Temporary Ban
-
-**Community Impact**: A serious violation of community standards, including
-sustained inappropriate behavior.
-
-**Consequence**: A temporary ban from any sort of interaction or public
-communication with the community for a specified period of time. No public or
-private interaction with the people involved, including unsolicited interaction
-with those enforcing the Code of Conduct, is allowed during this period.
-Violating these terms may lead to a permanent ban.
-
-### 4. Permanent Ban
-
-**Community Impact**: Demonstrating a pattern of violation of community
-standards, including sustained inappropriate behavior,  harassment of an
-individual, or aggression toward or disparagement of classes of individuals.
-
-**Consequence**: A permanent ban from any sort of public interaction within
-the community.
-
-## Attribution
-
-This Code of Conduct is adapted from the [Contributor Covenant][homepage],
-version 2.0, available at
-https://www.contributor-covenant.org/version/2/0/code_of_conduct.html.
-
-Community Impact Guidelines were inspired by [Mozilla's code of conduct
-enforcement ladder](https://github.com/mozilla/diversity).
-
-For answers to common questions about this code of conduct, see the FAQ at
-https://www.contributor-covenant.org/faq. Translations are available at
-https://www.contributor-covenant.org/translations.
-
-[homepage]: https://www.contributor-covenant.org
+# Contributor Covenant Code of Conduct
+
+## Our Pledge
+
+We as members, contributors, and leaders pledge to make participation in our
+community a harassment-free experience for everyone, regardless of age, body
+size, visible or invisible disability, ethnicity, sex characteristics, gender
+identity and expression, level of experience, education, socio-economic status,
+nationality, personal appearance, race, religion, or sexual identity
+and orientation.
+
+We pledge to act and interact in ways that contribute to an open, welcoming,
+diverse, inclusive, and healthy community.
+
+## Our Standards
+
+Examples of behavior that contributes to a positive environment for our
+community include:
+
+* Demonstrating empathy and kindness toward other people
+* Being respectful of differing opinions, viewpoints, and experiences
+* Giving and gracefully accepting constructive feedback
+* Accepting responsibility and apologizing to those affected by our mistakes,
+  and learning from the experience
+* Focusing on what is best not just for us as individuals, but for the
+  overall community
+
+Examples of unacceptable behavior include:
+
+* The use of sexualized language or imagery, and sexual attention or
+  advances of any kind
+* Trolling, insulting or derogatory comments, and personal or political attacks
+* Public or private harassment
+* Publishing others' private information, such as a physical or email
+  address, without their explicit permission
+* Other conduct which could reasonably be considered inappropriate in a
+  professional setting
+
+## Enforcement Responsibilities
+
+Community leaders are responsible for clarifying and enforcing our standards of
+acceptable behavior and will take appropriate and fair corrective action in
+response to any behavior that they deem inappropriate, threatening, offensive,
+or harmful.
+
+Community leaders have the right and responsibility to remove, edit, or reject
+comments, commits, code, wiki edits, issues, and other contributions that are
+not aligned to this Code of Conduct, and will communicate reasons for moderation
+decisions when appropriate.
+
+## Scope
+
+This Code of Conduct applies within all community spaces, and also applies when
+an individual is officially representing the community in public spaces.
+Examples of representing our community include using an official e-mail address,
+posting via an official social media account, or acting as an appointed
+representative at an online or offline event.
+
+## Enforcement
+
+Instances of abusive, harassing, or otherwise unacceptable behavior may be
+reported to the community leaders responsible for enforcement at
+mplichta@gmail.com.
+All complaints will be reviewed and investigated promptly and fairly.
+
+All community leaders are obligated to respect the privacy and security of the
+reporter of any incident.
+
+## Enforcement Guidelines
+
+Community leaders will follow these Community Impact Guidelines in determining
+the consequences for any action they deem in violation of this Code of Conduct:
+
+### 1. Correction
+
+**Community Impact**: Use of inappropriate language or other behavior deemed
+unprofessional or unwelcome in the community.
+
+**Consequence**: A private, written warning from community leaders, providing
+clarity around the nature of the violation and an explanation of why the
+behavior was inappropriate. A public apology may be requested.
+
+### 2. Warning
+
+**Community Impact**: A violation through a single incident or series
+of actions.
+
+**Consequence**: A warning with consequences for continued behavior. No
+interaction with the people involved, including unsolicited interaction with
+those enforcing the Code of Conduct, for a specified period of time. This
+includes avoiding interactions in community spaces as well as external channels
+like social media. Violating these terms may lead to a temporary or
+permanent ban.
+
+### 3. Temporary Ban
+
+**Community Impact**: A serious violation of community standards, including
+sustained inappropriate behavior.
+
+**Consequence**: A temporary ban from any sort of interaction or public
+communication with the community for a specified period of time. No public or
+private interaction with the people involved, including unsolicited interaction
+with those enforcing the Code of Conduct, is allowed during this period.
+Violating these terms may lead to a permanent ban.
+
+### 4. Permanent Ban
+
+**Community Impact**: Demonstrating a pattern of violation of community
+standards, including sustained inappropriate behavior,  harassment of an
+individual, or aggression toward or disparagement of classes of individuals.
+
+**Consequence**: A permanent ban from any sort of public interaction within
+the community.
+
+## Attribution
+
+This Code of Conduct is adapted from the [Contributor Covenant][homepage],
+version 2.0, available at
+https://www.contributor-covenant.org/version/2/0/code_of_conduct.html.
+
+Community Impact Guidelines were inspired by [Mozilla's code of conduct
+enforcement ladder](https://github.com/mozilla/diversity).
+
+For answers to common questions about this code of conduct, see the FAQ at
+https://www.contributor-covenant.org/faq. Translations are available at
+https://www.contributor-covenant.org/translations.
+
+[homepage]: https://www.contributor-covenant.org
```

### Comparing `dcspy-1.9.5/CONTRIBUTING.md` & `dcspy-2.0.0/CONTRIBUTING.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,78 @@
-## Development
-DCSpy use multicast UDP to receive/send data from/to DCS-BIOS as describe [here](https://github.com/DCSFlightpanels/dcs-bios/blob/master/Scripts/DCS-BIOS/doc/developerguide.adoc).
-Main modules of DCSpy:
-* `run.py` main script - it starts GUI in tkinter
-* `starter.py` responsible for initialise DCS-BIOS parser, Logitech G13/G15/G510 Mono handler and G19 Color handler, as well as running connection to DCS.
-* `log.py` dumb simple logger configuration
-* `logitech.py` handling Logitech keyboards with LCD and buttons, loading dynamically current aircraft
-* `aircraft.py` are define all supported aircraft with details how and what and display from DCS, draws bitmap that will be passed to LCD keyboard handler and returns input data for buttons under LCD
-* `dcsbios.py` BIOS protocol parser and two buffers to fetching integer and string values `IntegerBuffer` and `StringBuffer` respectively.
-* `tk_gui.py` simple GUI with widgets, layouts and events. It allows configuring DCSpy as well.
-* `utils.py` various useful tools - load and save config, check online version or download file
-
-If you want to modify or write something by yourself, here's a quick walk-through:
-* Each plane has special dict:
-```python
-BIOS_VALUE = TypedDict('BIOS_VALUE', {'class': str, 'args': Dict[str, int], 'value': Union[int, str], 'max_value': int}, total=False)
-
-self.bios_data: Dict[str, BIOS_VALUE] = {
-    'PVI_LINE2_TEXT': {'class': 'StringBuffer',
-                       'args': {'address': 0x192a, 'max_length': 6},
-                       'value': str()},
-    'AP_ALT_HOLD_LED': {'class': 'IntegerBuffer',
-                        'args': {'address': 0x1936, 'mask': 0x8000, 'shift_by': 0xf},
-                        'value': int()},
-    'IFF_MASTER_KNB': {'class': 'IntegerBuffer',
-                       'args': {'address': 0x4450, 'mask': 0xe, 'shift_by': 0x1},
-                       'value': int(),
-                       'max_value': 4}}
-```
-which describe data to be fetched from DCS-BIOS with buffer class and its parameters. For required address and data max_length, look up in `C:\Users\xxx\Saved Games\DCS.openbeta\Scripts\DCS-BIOS\doc\control-reference.html`
-* Then after detecting current plane in DCS, `KeyboardMono` or `KeyboardColor` will load instance of aircraft as `plane`
-```python
-self.plane: Aircraft = getattr(import_module('dcspy.aircraft'), self.plane_name)(self.lcd)
-```
-* and "subscribe" for changes with callback for all fields defined in `plane` instance
-```python
-for field_name, proto_data in self.plane.bios_data.items():
-    buffer = getattr(import_module('dcspy.dcsbios'), proto_data['class'])
-    buffer(parser=self.parser, callback=partial(self.plane.set_bios, field_name), **proto_data['args'])
-```
-* when, receive bytes, parser will process data:
-```python
-dcs_bios_resp = sock.recv(2048)
-for int_byte in dcs_bios_resp:
-    parser.process_byte(int_byte)
-```
-and calls callback function `set_bios()` of current `plane` with received value and update display content, by creating bitmap and passing it through LCD SDK to device display.
-
-* You can also use 4 buttons below LCD (G13) and left, right, up and down buttons (G19), just check their state with `check_buttons()` of `KeyboardMono` which one is pressed and send request do DCS-BIOS.
-```python
-sock.sendto(bytes(self.plane.button_request(button), 'utf-8'), ('127.0.0.1', 7778))
-```
-* Correct action is define in aircraft instance `button_request()` method:
-```python
-action = {LcdButton.ONE: 'UFC_COMM1_CHANNEL_SELECT DEC\n',
-          LcdButton.TWO: 'UFC_COMM1_CHANNEL_SELECT INC\n',
-          LcdButton.THREE: 'UFC_COMM2_CHANNEL_SELECT DEC\n',
-          LcdButton.FOUR: 'UFC_COMM2_CHANNEL_SELECT INC\n',
-          LcdButton.LEFT: 'UFC_COMM1_CHANNEL_SELECT DEC\n',
-          LcdButton.RIGHT: 'UFC_COMM1_CHANNEL_SELECT INC\n',
-          LcdButton.DOWN: 'UFC_COMM2_CHANNEL_SELECT DEC\n',
-          LcdButton.UP: 'UFC_COMM2_CHANNEL_SELECT INC\n'}
-return super().button_request(button, action.get(button, '\n'))
-```
-Again, look it up in `control-reference.html`, in example above, COMM1 and COMM2 knobs of F/A-18C will rotate left and right.
+## Development
+DCSpy use multicast UDP to receive/send data from/to DCS-BIOS as describe [here](https://github.com/DCSFlightpanels/dcs-bios/blob/master/Scripts/DCS-BIOS/doc/developerguide.adoc).
+Main modules of DCSpy:
+* `run.py` main script - it starts GUI in tkinter
+* `starter.py` responsible for initialise DCS-BIOS parser, Logitech G13/G15/G510 Mono handler and G19 Color handler, as well as running connection to DCS.
+* `log.py` dumb simple logger configuration
+* `logitech.py` handling Logitech keyboards with LCD and buttons, loading dynamically current aircraft
+* `aircraft.py` are define all supported aircraft with details how and what and display from DCS, draws bitmap that will be passed to LCD keyboard handler and returns input data for buttons under LCD
+* `dcsbios.py` BIOS protocol parser and two buffers to fetching integer and string values `IntegerBuffer` and `StringBuffer` respectively.
+* `tk_gui.py` simple GUI with widgets, layouts and events. It allows configuring DCSpy as well.
+* `utils.py` various useful tools - load and save config, check online version or download file
+
+If you want to modify or write something by yourself, here's a quick walk-through:
+* Each plane has special dict:
+```python
+class IntBuffArgs(TypedDict):
+    address: int
+    mask: int
+    shift_by: int
+
+class StrBuffArgs(TypedDict):
+    address: int
+    max_length: int
+
+class BiosValue(TypedDict):
+    klass: str
+    args: Union[StrBuffArgs, IntBuffArgs]
+    value: Union[int, str]
+    max_value: NotRequired[int]
+
+self.bios_data: Dict[str, BiosValue] = {
+    'PVI_LINE2_TEXT': {'klass': 'StringBuffer',
+                       'args': {'address': 0x192a, 'max_length': 6},
+                       'value': str()},
+    'AP_ALT_HOLD_LED': {'klass': 'IntegerBuffer',
+                        'args': {'address': 0x1936, 'mask': 0x8000, 'shift_by': 0xf},
+                        'value': int()},
+    'IFF_MASTER_KNB': {'klass': 'IntegerBuffer',
+                       'args': {'address': 0x4450, 'mask': 0xe, 'shift_by': 0x1},
+                       'value': int(),
+                       'max_value': 4}}
+```
+which describe data to be fetched from DCS-BIOS with buffer class and its parameters. For required address and data max_length, look up in `C:\Users\xxx\Saved Games\DCS.openbeta\Scripts\DCS-BIOS\doc\control-reference.html`
+* Then after detecting current plane in DCS, `KeyboardMono` or `KeyboardColor` will load instance of aircraft as `plane`
+```python
+self.plane: Aircraft = getattr(import_module('dcspy.aircraft'), self.plane_name)(self.lcd)
+```
+* and "subscribe" for changes with callback for all fields defined in `plane` instance
+```python
+for field_name, proto_data in self.plane.bios_data.items():
+    buffer = getattr(import_module('dcspy.dcsbios'), proto_data['klass'])
+    buffer(parser=self.parser, callback=partial(self.plane.set_bios, field_name), **proto_data['args'])
+```
+* when, receive bytes, parser will process data:
+```python
+dcs_bios_resp = sock.recv(2048)
+for int_byte in dcs_bios_resp:
+    parser.process_byte(int_byte)
+```
+and calls callback function `set_bios()` of current `plane` with received value and update display content, by creating bitmap and passing it through LCD SDK to device display.
+
+* You can also use 4 buttons below LCD (G13) and left, right, up and down buttons (G19), just check their state with `check_buttons()` of `KeyboardMono` which one is pressed and send request do DCS-BIOS.
+```python
+sock.sendto(bytes(self.plane.button_request(button), 'utf-8'), ('127.0.0.1', 7778))
+```
+* Correct action is define in aircraft instance `button_request()` method:
+```python
+action = {LcdButton.ONE: 'UFC_COMM1_CHANNEL_SELECT DEC\n',
+          LcdButton.TWO: 'UFC_COMM1_CHANNEL_SELECT INC\n',
+          LcdButton.THREE: 'UFC_COMM2_CHANNEL_SELECT DEC\n',
+          LcdButton.FOUR: 'UFC_COMM2_CHANNEL_SELECT INC\n',
+          LcdButton.LEFT: 'UFC_COMM1_CHANNEL_SELECT DEC\n',
+          LcdButton.RIGHT: 'UFC_COMM1_CHANNEL_SELECT INC\n',
+          LcdButton.DOWN: 'UFC_COMM2_CHANNEL_SELECT DEC\n',
+          LcdButton.UP: 'UFC_COMM2_CHANNEL_SELECT INC\n'}
+return super().button_request(button, action.get(button, '\n'))
+```
+Again, look it up in `control-reference.html`, in example above, COMM1 and COMM2 knobs of F/A-18C will rotate left and right.
```

### Comparing `dcspy-1.9.5/PKG-INFO` & `dcspy-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,316 +1,330 @@
-Metadata-Version: 2.1
-Name: dcspy
-Version: 1.9.5
-Summary: Integrating DCS (Digital Combat Simulator) planes with Logitech G13/G15/G510/G19 LCD
-Home-page: https://github.com/emcek/dcspy
-Author: Michal Plichta
-Maintainer: Michal Plichta
-License: MIT
-Project-URL: Bug Reports, https://github.com/emcek/dcspy/issues
-Project-URL: Source, https://github.com/emcek/dcspy
-Keywords: logitech,logitech-sdk,logitech-keyboards,logitech-gaming,logitech-gaming-keyboard,dcs-world,dcs,g13,g15,g510,g19
-Platform: win32
-Platform: nt
-Platform: Windows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Games/Entertainment :: Simulation
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Hardware
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE.md
-
-[![image](https://img.shields.io/badge/pypi-v1.9.5-blue.svg)](https://pypi.org/project/dcspy/)
-[![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
-[![License](https://img.shields.io/badge/Licence-MIT-blue.svg)](./LICENSE.md)
-[![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
-[![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
-[![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
-[![Discord](https://img.shields.io/discord/672486999516774442?label=Discord&logo=discord&logoColor=lightblue)](https://discord.gg/SP5Yjx3)
-[![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://github.com/emcek/dcspy)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/emcek/dcspy/master.svg)](https://results.pre-commit.ci/latest/github/emcek/dcspy/master)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=emcek_dcspy&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=emcek_dcspy)
-[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6056/badge)](https://bestpractices.coreinfrastructure.org/projects/6056)
-[![Downloads](https://pepy.tech/badge/dcspy)](https://pepy.tech/project/dcspy)
-[![Rate this package](https://badges.openbase.com/python/rating/dcspy.svg?token=AZCVj1Hdbl6cC3I/gkVpgsigp22LtCOR0sB8lcODY9Y=)](https://openbase.com/python/dcspy?utm_source=embedded&amp;utm_medium=badge&amp;utm_campaign=rate-badge)
-
-![dcspylogo](https://i.imgur.com/eqqrPB8.jpg)
-## DCSpy
-DCSpy is able to pull information from DCS aircraft and display on Logitech G-series keyboards LCD.
-It supports:
-* Logitech device with 160x43 px (4 lines) monochrome LCD - **G13**, **G15 (v1 and v2)** and **G510**
-* Logitech device with 320x240 px (8 lines) full RGBA LCD - **G19**
-
-See more information on [Wiki](https://github.com/emcek/dcspy/wiki) page.
-
-## Sponsored by Jetbrains Open Source Support Program
-[![logo](https://resources.jetbrains.com/storage/products/company/brand/logos/PyCharm.svg)](https://jb.gg/OpenSourceSupport)
-[![logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.svg)](https://jb.gg/OpenSourceSupport)
-
-## Aircraft and instruments
-* F/A-18C Hornet UFC - Up Front Controller
-* F-16C Viper DED - Data Entry Display
-* Ka-50 Black Shark II and III - PVI-800 and autopilot channels
-* Mi-8MTV2 Hip - autopilot channels and Radios information
-* Mi-24P Hind - Autopilot channels and modes and Radios information
-* A-10C Warthog and A-10C II Tank Killer - Radio frequency information
-* F-14A and F-14B Tomcat - basic support for RIO CAP
-* AV-8B Night Attack Harrier - Up Front Controller and Option Display Unit
-* AH-64D Apache - Enhanced Up Front Display
-* more to come....
-
-## Requirements
-* [Python 3.11](https://www.python.org/downloads/) but 3.7+ (with tcl/tk support, see [installation](https://github.com/emcek/dcspy/wiki/installation)) should be fine, please choose Windows x86-64 version, file should be python-3.11.1-amd64.exe.
-* [Logitech Gaming Software 9.04.49](https://support.logitech.com/software/lgs)
-* [DCS-BIOS 0.7.47](https://github.com/DCSFlightpanels/dcs-bios/releases/latest) (or newer)
-* DCS World: [2.8.2.35759](https://www.digitalcombatsimulator.com/en/news/changelog/openbeta/2.8.2.35759/) Open Beta
-
-**Notes:**
-* If you upgrade DCSpy from 1.5.1 or older you can safely remove Logitech LCD SDK from `C:\Program Files\Logitech Gaming Software\LCDSDK_8.57.148`. Since DCSpy version 1.6.0 use built-in SDK in LGS (Logitech Gaming Software).
-
-## New ideas
-I have lots of plans and new ideas how to improve it internally and form user's perspective, but don't hesitate to contact me. Maybe it will motivate me to implement some new stuff. Please open issue if you find bug or have any crazy idea.
-You are welcome [dcspy Discord](https://discord.gg/SP5Yjx3) server.
-
-## Contributing
-You want contribute, perfect see: [contributing](./CONTRIBUTING.md) guide.
-
-## Credits
-More details [here](https://github.com/emcek/dcspy/wiki/Information#credits).
-
-## 1.9.5
-* Support for **Mi-8MTV2 Magnificent Eight**
-  * Autopilot Channels (Heading, Pitch/Bank and Altitude)
-  * Radios: R868, R828, YADRO1A information
-* Support for **Mi-24P Hind**
-  * Autopilot Channels (Yaw, Roll, Pitch and Altitude)
-  * Autopilot Modes (Hover, Route and Altitude)
-  * Radios: R868, R828, YADRO1I information
-* Add About tab with basic information
-* **F-16C Viper**:
-  * Add spacial font for DED (G19 only)
-  * Clean some extra characters from DED
-* Internal:
-  * force update customtkinter to at least 5.1.0
-
-## 1.8.1
-* Add support for **Ka-50 Black Shark III**
-* Update footer when checking DCS-BIOS version
-* Align with DCS 2.8.1.34667.2 and DCS-BIOS 0.7.47
-* Internal:
-  * add more unit tests
-  * mark some test as DCS-BIOS tests
-
-## 1.8.0
-* Major GUI redesign using `customtkinter` package, which provides new, modern widgets:
-  * Appearance system mode (`Light`, `Dark`)
-  * Three colort theme (`Green`, `Blue` and `Dark Blue`)
-  * All settings are configured from GUI vie widgets
-  * One window for all configuration and buttons
-  * Check version from GUI
-  * Add configuration flag to check for new version during start
-
-## 1.7.5
-* report DCS stable version correctly in logs during start
-* Internal:
-  * rename starting script
-  * remove usage of McCabe
-  * add unit tests
-
-## 1.7.4
-* **AH-64D Apache**
-  * add better support for G19 for PRE mode
-  * update name from `AH64D` to `AH64DBLKII`
-* Show DCS version in logs
-* Fix name of plane for **F-14 Tomcat** depending on model A or B
-* Toggle Start/Stop buttons
-* Do not show warning when plane's name is empty
-* Internal:
-  * improve checking DCS-BIOS data
-  * introduce enum values for parser state
-  * improve CI process - add Python 3.11
-  * force using Pillow 9.3.0
-
-## 1.7.3
-* Align **F-16C Viper** DED and **AH-64D Apache** EUFD with DCS-BIOS 0.7.46 changes
-* Basic support for **F-14A Tomcat**
-
-## 1.7.2
-* **AH-64D Apache**
-  * update name from `AH64DBLKII` to `AH64D`
-  * fix display PRE mode for G19
-  * fix handling buttons
-* Internal:
-  * update unit test for better coverage and more use-cases
-
-## 1.7.1
-* New config settings:
-  * `auto_start` - run DCSpy atomically after start
-  * `verbose` - show more logs in terminal/console window
-* Fixing handling of `dcsbios` settings from `config.yaml`
-* Start and stop buttons can be used several times without closing GUI
-* **F-16C Viper**
-  * replace `*` with inverse white circle character at DED
-  * Fix unhandled buttons for G19 (menu, ok and cancel)
-* G19 and **F/A-18C Hornet**
-  * Push **Menu** and **Cancel** toggle cockpit button down, push it again toggles button up (Integrated Fuel/Engine Indicator - IFEI).
-  * Add handling **Ok** as Attitude Selector Switch, INS/AUTO/STBY
-* Internal:
-  * use Pythonic way using temporary directory
-  * speed-up tests - cache json files instead of downloading from internet
-  * use Enum for LCD type
-  * use Enum for LCD buttons, add to LcdInfo dataclass
-
-## 1.7.0
-* Support for **AH-64D Apache** with 3 modes:
-  * `IDM` - Squeeze and shows radios frequencies (from Radio Area), IDM and RTS rocker are used to scroll down
-  * `WCA` - Enter button display warnings, cautions, and advisories, WCA rocker is used to scroll down
-  * `PRE` - Preset button displays the preset menu for the selected radio, WCA rocker is used to scroll down
-* **F-16C Viper** DED clean-up extra characters
-
-## 1.6.1
-* Update **F-16C Viper** for latest DSC-BIOS (0.7.45)
-* Fresh installation of DCS-BIOS is painless
-* Drop support for Python 3.6
-
-## 1.6.0
-* use fonts in dynamic way - you can customize fonts in `config.yaml` file (see [Configuration](https://github.com/emcek/dcspy#configuration))
-* usage for LCD SDK built-in LGS - no need additional package for usage
-* support for Python 3.10 (use `dataclasses` internally)
-* ability to stop DCSpy from GUI
-* supporters are printed in welcome screen - I'm thrilled with support and help of community!
-
-## 1.5.1
-* alignment for new DCS-BIOS [v0.7.43](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.43)
-
-## 1.5.0
-* Support for **AV-8B N/A Harrier** with:
-  * **UFC** - Up Front Controller
-  * **ODU** - Option Display Unit
-  * **decrease UFC Comm 1 Channel** - G13 1st button or G19 left button
-  * **increase UFC Comm 1 Channel** - G13 2nd button or G19 right button
-  * **decrease UFC Comm 2 Channel** - G13 3rd button or G19 down button
-  * **increase UFC Comm 2 Channel** - G13 4th button or G19 up button
-
-## 1.4.0
-* Configuration editor:
-  * **dcsbios** - set default Logitech keyboard: "G19", "G510", "G15 v1/v2", "G13"
-  * **show_gui** - showing or hiding GUI during start of DCSpy
-  * **dcsbios** - location of DCS-BIOS folder inside user's Saved Games
-* Check and update DCS-BIOS directly from DCSpy
-  * **Check DCS-BIOS** button in **Config** editor
-  * **dcsbios** needs to be set to correct value
-* Basic A-10C Warthog and A-10C II Tank Killer support
-
-## 1.3.0
-* **F-16C Viper** use 4 buttons for IFF
-  * **IFF MASTER Knob** - OFF/STBY/LOW/NORM/EMER
-  * **IFF ENABLE Switch** - M1/M3 /OFF/ M3/MS
-  * **IFF M-4 CODE Switch** - HOLD/ A/B /ZERO
-  * **IFF MODE 4 REPLY Switch** - OUT/A/B
-* Fix alignment of (DCS-BIOS [v0.7.41](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.41)) for **F-14B Tomcat**
-* Internally all data fetch form DCS-BIOS is check against its specification. Sometimes due to changes DCS-BIOS protocol DCSpy couldn't fetch all data i.e. F-16 DED. It shouldn't happened anymore.
-
-## 1.2.3
-* Fix alignment of DED (DCS-BIOS [v0.7.41](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.43)) for **F-16C Viper**
-
-## 1.2.2
-* Fix alignment of DED for **F-16C Viper**
-* Fix position of Integrated Fuel/Engine Indicator (IFEI) for **F/A-18C Hornet** (only G19)
-
-## 1.2.1
-* **F/A-18C Hornet** shows extra Total Internal Fuel (G19 only)
-* Internal refactoring
-
-## 1.2.0
-* Simple Tkinter GUI - to select your Logitech keyboard
-* Support for G19 - Big thanks for **BrotherBloat** who makes this release possible. He spent countless hours to share his G19 and let me troubleshoot remotely.
-* **F/A-18C Hornet** shows Total Fuel instead of Total Internal Fuel
-
-## 1.1.1
-* Basic support for **F-14B Tomcat** RIO CAP (Computer Address Panel):
-  * **CLEAR** - button 1
-  * **S-W** - button 2
-  * **N+E** - button 3
-  * **ENTER** - button 4
-
-## 1.1.0
-* dcspy use now UDP multicast connection do DCS-BIOS, since each TCP connection slightly increases the amount of work that is performed inside of DCS (blocking the rest of the simulation).
-* support for integer data to be fetch from DCS-BIOS - using IntegerBuffer()
-* bios_data in Airplanes instances allow both StringBuffer() and IntegerBuffer()
-* reformat waiting time before DCS connected
-* fix Data Entry Display for F-16C Viper - DCS-BIOS [v0.7.34](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.34) is required
-* **Ka-50 Black Shark** - Autopilot channels show up in LCD
-
-## 1.0.0
-* **Ka-50 Black Shark** data from PVI-800 shows (in similar boxes) on LCD
-* ProtocolParser for DCS-BIOS has new optimized state machine
-  * LCD SDK is re-written from scratch:
-  * low and high level API
-  * auto-loading C library during importing
-  * all API is type annotated and well documented
-  * move loading LCD C library from G13 handler
-*internal:
-  * refactoring and rename internals of G13 handler module
-  * add unit tests
-
-## 0.9.2
-* LCD prints current waiting time to connect to DCS
-* when DCS exit from plane/mission exception is catch and handle correctly
-* lots of internal changes, preparing for new features, most important:
-  * change structure of AircraftHandler, move subscription to DCS-BIOS changes out of planes
-  * update and clear methods move from G13 handler to LCD SDK
-
-## 0.9.1
-* G13 handler have display property to send text to LCD
-* rename starting script to dcspy.exe
-* starting script now show waiting time for DCS connection
-* minor code optimization and refactoring
-
-## 0.9.0
-* based on version [specelUFC v1.12.1](https://github.com/specel/specelUFC/releases/tag/v1.12.1)
-* added basic handling for Ka-50 PVI-800 data are received but not formatted properly
-* F-16C DED should working but not 4 buttons under LCD - I don't have it so it is hard to test
-* G13 handler detect 32/64 bit of Python and load correct version of LCD Logitech C library
-* adding basic logging for debugging - prints on console
-* all defined aircraft are detected and loaded on-the-fly during operation
-* define new plane should be easy just use AircraftHandler as base class
-* Python LCD SDK was clean-up
-* other refactorings and code duplication removal
-
-MIT License
-
-Copyright (c) 2020 Michal Plichta
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Metadata-Version: 2.1
+Name: dcspy
+Version: 2.0.0
+Summary: Integrating DCS (Digital Combat Simulator) planes with Logitech G13/G15/G510/G19 LCD
+Home-page: https://github.com/emcek/dcspy
+Author: Michal Plichta
+Maintainer: Michal Plichta
+License: MIT
+Project-URL: Bug Reports, https://github.com/emcek/dcspy/issues
+Project-URL: Source, https://github.com/emcek/dcspy
+Keywords: logitech,logitech-sdk,logitech-keyboards,logitech-gaming,logitech-gaming-keyboard,dcs-world,dcs,g13,g15,g510,g19
+Platform: win32
+Platform: nt
+Platform: Windows
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Games/Entertainment :: Simulation
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Hardware
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE.md
+
+[![image](https://img.shields.io/badge/pypi-v2.0.0-blue.svg)](https://pypi.org/project/dcspy/)
+[![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
+[![License](https://img.shields.io/badge/Licence-MIT-blue.svg)](./LICENSE.md)
+[![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
+[![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
+[![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
+[![Discord](https://img.shields.io/discord/672486999516774442?label=Discord&logo=discord&logoColor=lightblue)](https://discord.gg/SP5Yjx3)
+[![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://github.com/emcek/dcspy)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/emcek/dcspy/master.svg)](https://results.pre-commit.ci/latest/github/emcek/dcspy/master)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=emcek_dcspy&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=emcek_dcspy)
+[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6056/badge)](https://bestpractices.coreinfrastructure.org/projects/6056)
+[![Downloads](https://pepy.tech/badge/dcspy)](https://pepy.tech/project/dcspy)
+[![Rate this package](https://badges.openbase.com/python/rating/dcspy.svg?token=AZCVj1Hdbl6cC3I/gkVpgsigp22LtCOR0sB8lcODY9Y=)](https://openbase.com/python/dcspy?utm_source=embedded&amp;utm_medium=badge&amp;utm_campaign=rate-badge)
+
+![dcspylogo](https://i.imgur.com/eqqrPB8.jpg)
+## DCSpy
+DCSpy is able to pull information from DCS aircraft and display on Logitech G-series keyboards LCD.
+It supports:
+* Logitech device with 160x43 px (4 lines) monochrome LCD - **G13**, **G15 (v1 and v2)** and **G510**
+* Logitech device with 320x240 px (8 lines) full RGBA LCD - **G19**
+
+See more information on [Wiki](https://github.com/emcek/dcspy/wiki) page.
+
+## Sponsored by Jetbrains Open Source Support Program
+[![logo](https://resources.jetbrains.com/storage/products/company/brand/logos/PyCharm.svg)](https://jb.gg/OpenSourceSupport)
+[![logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.svg)](https://jb.gg/OpenSourceSupport)
+
+## Aircraft and instruments
+* F/A-18C Hornet UFC - Up Front Controller
+* F-16C Viper DED - Data Entry Display
+* Ka-50 Black Shark II and III - PVI-800 and autopilot channels
+* Mi-8MTV2 Hip - autopilot channels and Radios information
+* Mi-24P Hind - Autopilot channels and modes and Radios information
+* A-10C Warthog and A-10C II Tank Killer - Radio frequency information
+* F-14A and F-14B Tomcat - basic support for RIO CAP
+* AV-8B Night Attack Harrier - Up Front Controller and Option Display Unit
+* AH-64D Apache - Enhanced Up Front Display
+* more to come....
+
+## Requirements
+* [Logitech Gaming Software 9.04.49](https://support.logitech.com/software/lgs)
+* [DCS-BIOS 0.7.48](https://github.com/DCSFlightpanels/dcs-bios/releases/latest) or newer (can be installed directly from DCSpy)
+* DCS World: [2.8.4.39731](https://www.digitalcombatsimulator.com/en/news/changelog/openbeta/2.8.4.39731/) Open Beta (any release 2.8.* should work)
+* (optional) [Python 3.11](https://www.python.org/downloads/) but 3.7+ should be fine (with tcl/tk support, see [installation](https://github.com/emcek/dcspy/wiki/installation))
+
+**Notes:**
+* If you upgrade DCSpy from 1.5.1 or older you can safely remove Logitech LCD SDK from `C:\Program Files\Logitech Gaming Software\LCDSDK_8.57.148`. Since DCSpy version 1.6.0 use built-in SDK in LGS (Logitech Gaming Software).
+
+## New ideas
+I have lots of plans and new ideas how to improve it internally and form user's perspective, but don't hesitate to contact me. Maybe it will motivate me to implement some new stuff. Please open issue if you find bug or have any crazy idea.
+You are welcome [dcspy Discord](https://discord.gg/SP5Yjx3) server.
+
+## Contributing
+You want contribute, perfect see: [contributing](./CONTRIBUTING.md) guide.
+
+## Credits
+More details [here](https://github.com/emcek/dcspy/wiki/Information#credits).
+
+## 2.0.0
+* Allow use/update [live DCS-BIOS](https://github.com/emcek/dcspy/wiki/Information#live-dcs-bios) directly from GitHub (master branch)
+* Allow run DCSpy without console
+* Auto [screenshot of LCD](https://github.com/emcek/dcspy/wiki/Usage#advanced) during operation
+* Auto save change options from GUI
+* Fix problem when DCS-BIOS is empty or drive letter not exists
+* Generate [standalone version](https://github.com/emcek/dcspy/wiki/Installation#single-file-download-new-way) with PyInstaller
+* Save configuration in user local directory (preserved between updates)
+* Internal:
+  * improve type checking
+  * verbose setting will impact both console and file logs
+  * use pathlib for path manipulation
+  * improve CI/CD process
+
+## 1.9.5
+* Support for **Mi-8MTV2 Magnificent Eight**
+  * Autopilot Channels (Heading, Pitch/Bank and Altitude)
+  * Radios: R868, R828, YADRO1A information
+* Support for **Mi-24P Hind**
+  * Autopilot Channels (Yaw, Roll, Pitch and Altitude)
+  * Autopilot Modes (Hover, Route and Altitude)
+  * Radios: R868, R828, YADRO1I information
+* Add About tab with basic information
+* **F-16C Viper**:
+  * Add spacial font for DED (G19 only)
+  * Clean some extra characters from DED
+* Internal:
+  * force update customtkinter to at least 5.1.0
+
+## 1.8.1
+* Add support for **Ka-50 Black Shark III**
+* Update footer when checking DCS-BIOS version
+* Align with DCS 2.8.1.34667.2 and DCS-BIOS 0.7.47
+* Internal:
+  * add more unit tests
+  * mark some test as DCS-BIOS tests
+
+## 1.8.0
+* Major GUI redesign using `customtkinter` package, which provides new, modern widgets:
+  * Appearance system mode (`Light`, `Dark`)
+  * Three colort theme (`Green`, `Blue` and `Dark Blue`)
+  * All settings are configured from GUI vie widgets
+  * One window for all configuration and buttons
+  * Check version from GUI
+  * Add configuration flag to check for new version during start
+
+## 1.7.5
+* report DCS stable version correctly in logs during start
+* Internal:
+  * rename starting script
+  * remove usage of McCabe
+  * add unit tests
+
+## 1.7.4
+* **AH-64D Apache**
+  * add better support for G19 for PRE mode
+  * update name from `AH64D` to `AH64DBLKII`
+* Show DCS version in logs
+* Fix name of plane for **F-14 Tomcat** depending on model A or B
+* Toggle Start/Stop buttons
+* Do not show warning when plane's name is empty
+* Internal:
+  * improve checking DCS-BIOS data
+  * introduce enum values for parser state
+  * improve CI process - add Python 3.11
+  * force using Pillow 9.3.0
+
+## 1.7.3
+* Align **F-16C Viper** DED and **AH-64D Apache** EUFD with DCS-BIOS 0.7.46 changes
+* Basic support for **F-14A Tomcat**
+
+## 1.7.2
+* **AH-64D Apache**
+  * update name from `AH64DBLKII` to `AH64D`
+  * fix display PRE mode for G19
+  * fix handling buttons
+* Internal:
+  * update unit test for better coverage and more use-cases
+
+## 1.7.1
+* New config settings:
+  * `auto_start` - run DCSpy atomically after start
+  * `verbose` - show more logs in terminal/console window
+* Fixing handling of `dcsbios` settings from `config.yaml`
+* Start and stop buttons can be used several times without closing GUI
+* **F-16C Viper**
+  * replace `*` with inverse white circle character at DED
+  * Fix unhandled buttons for G19 (menu, ok and cancel)
+* G19 and **F/A-18C Hornet**
+  * Push **Menu** and **Cancel** toggle cockpit button down, push it again toggles button up (Integrated Fuel/Engine Indicator - IFEI).
+  * Add handling **Ok** as Attitude Selector Switch, INS/AUTO/STBY
+* Internal:
+  * use Pythonic way using temporary directory
+  * speed-up tests - cache json files instead of downloading from internet
+  * use Enum for LCD type
+  * use Enum for LCD buttons, add to LcdInfo dataclass
+
+## 1.7.0
+* Support for **AH-64D Apache** with 3 modes:
+  * `IDM` - Squeeze and shows radios frequencies (from Radio Area), IDM and RTS rocker are used to scroll down
+  * `WCA` - Enter button display warnings, cautions, and advisories, WCA rocker is used to scroll down
+  * `PRE` - Preset button displays the preset menu for the selected radio, WCA rocker is used to scroll down
+* **F-16C Viper** DED clean-up extra characters
+
+## 1.6.1
+* Update **F-16C Viper** for latest DSC-BIOS (0.7.45)
+* Fresh installation of DCS-BIOS is painless
+* Drop support for Python 3.6
+
+## 1.6.0
+* use fonts in dynamic way - you can customize fonts in `config.yaml` file (see [Configuration](https://github.com/emcek/dcspy#configuration))
+* usage for LCD SDK built-in LGS - no need additional package for usage
+* support for Python 3.10 (use `dataclasses` internally)
+* ability to stop DCSpy from GUI
+* supporters are printed in welcome screen - I'm thrilled with support and help of community!
+
+## 1.5.1
+* alignment for new DCS-BIOS [v0.7.43](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.43)
+
+## 1.5.0
+* Support for **AV-8B N/A Harrier** with:
+  * **UFC** - Up Front Controller
+  * **ODU** - Option Display Unit
+  * **decrease UFC Comm 1 Channel** - G13 1st button or G19 left button
+  * **increase UFC Comm 1 Channel** - G13 2nd button or G19 right button
+  * **decrease UFC Comm 2 Channel** - G13 3rd button or G19 down button
+  * **increase UFC Comm 2 Channel** - G13 4th button or G19 up button
+
+## 1.4.0
+* Configuration editor:
+  * **dcsbios** - set default Logitech keyboard: "G19", "G510", "G15 v1/v2", "G13"
+  * **show_gui** - showing or hiding GUI during start of DCSpy
+  * **dcsbios** - location of DCS-BIOS folder inside user's Saved Games
+* Check and update DCS-BIOS directly from DCSpy
+  * **Check DCS-BIOS** button in **Config** editor
+  * **dcsbios** needs to be set to correct value
+* Basic A-10C Warthog and A-10C II Tank Killer support
+
+## 1.3.0
+* **F-16C Viper** use 4 buttons for IFF
+  * **IFF MASTER Knob** - OFF/STBY/LOW/NORM/EMER
+  * **IFF ENABLE Switch** - M1/M3 /OFF/ M3/MS
+  * **IFF M-4 CODE Switch** - HOLD/ A/B /ZERO
+  * **IFF MODE 4 REPLY Switch** - OUT/A/B
+* Fix alignment of (DCS-BIOS [v0.7.41](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.41)) for **F-14B Tomcat**
+* Internally all data fetch form DCS-BIOS is check against its specification. Sometimes due to changes DCS-BIOS protocol DCSpy couldn't fetch all data i.e. F-16 DED. It shouldn't happened anymore.
+
+## 1.2.3
+* Fix alignment of DED (DCS-BIOS [v0.7.41](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.43)) for **F-16C Viper**
+
+## 1.2.2
+* Fix alignment of DED for **F-16C Viper**
+* Fix position of Integrated Fuel/Engine Indicator (IFEI) for **F/A-18C Hornet** (only G19)
+
+## 1.2.1
+* **F/A-18C Hornet** shows extra Total Internal Fuel (G19 only)
+* Internal refactoring
+
+## 1.2.0
+* Simple Tkinter GUI - to select your Logitech keyboard
+* Support for G19 - Big thanks for **BrotherBloat** who makes this release possible. He spent countless hours to share his G19 and let me troubleshoot remotely.
+* **F/A-18C Hornet** shows Total Fuel instead of Total Internal Fuel
+
+## 1.1.1
+* Basic support for **F-14B Tomcat** RIO CAP (Computer Address Panel):
+  * **CLEAR** - button 1
+  * **S-W** - button 2
+  * **N+E** - button 3
+  * **ENTER** - button 4
+
+## 1.1.0
+* dcspy use now UDP multicast connection do DCS-BIOS, since each TCP connection slightly increases the amount of work that is performed inside of DCS (blocking the rest of the simulation).
+* support for integer data to be fetch from DCS-BIOS - using IntegerBuffer()
+* bios_data in Airplanes instances allow both StringBuffer() and IntegerBuffer()
+* reformat waiting time before DCS connected
+* fix Data Entry Display for F-16C Viper - DCS-BIOS [v0.7.34](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.34) is required
+* **Ka-50 Black Shark** - Autopilot channels show up in LCD
+
+## 1.0.0
+* **Ka-50 Black Shark** data from PVI-800 shows (in similar boxes) on LCD
+* ProtocolParser for DCS-BIOS has new optimized state machine
+  * LCD SDK is re-written from scratch:
+  * low and high level API
+  * auto-loading C library during importing
+  * all API is type annotated and well documented
+  * move loading LCD C library from G13 handler
+*internal:
+  * refactoring and rename internals of G13 handler module
+  * add unit tests
+
+## 0.9.2
+* LCD prints current waiting time to connect to DCS
+* when DCS exit from plane/mission exception is catch and handle correctly
+* lots of internal changes, preparing for new features, most important:
+  * change structure of AircraftHandler, move subscription to DCS-BIOS changes out of planes
+  * update and clear methods move from G13 handler to LCD SDK
+
+## 0.9.1
+* G13 handler have display property to send text to LCD
+* rename starting script to dcspy.exe
+* starting script now show waiting time for DCS connection
+* minor code optimization and refactoring
+
+## 0.9.0
+* based on version [specelUFC v1.12.1](https://github.com/specel/specelUFC/releases/tag/v1.12.1)
+* added basic handling for Ka-50 PVI-800 data are received but not formatted properly
+* F-16C DED should working but not 4 buttons under LCD - I don't have it so it is hard to test
+* G13 handler detect 32/64 bit of Python and load correct version of LCD Logitech C library
+* adding basic logging for debugging - prints on console
+* all defined aircraft are detected and loaded on-the-fly during operation
+* define new plane should be easy just use AircraftHandler as base class
+* Python LCD SDK was clean-up
+* other refactorings and code duplication removal
+
+MIT License
+
+Copyright (c) 2020 Michal Plichta
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dcspy-1.9.5/README.md` & `dcspy-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-[![image](https://img.shields.io/badge/pypi-v1.9.5-blue.svg)](https://pypi.org/project/dcspy/)
-[![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
-[![License](https://img.shields.io/badge/Licence-MIT-blue.svg)](./LICENSE.md)
-[![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
-[![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
-[![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
-[![Discord](https://img.shields.io/discord/672486999516774442?label=Discord&logo=discord&logoColor=lightblue)](https://discord.gg/SP5Yjx3)
-[![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://github.com/emcek/dcspy)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/emcek/dcspy/master.svg)](https://results.pre-commit.ci/latest/github/emcek/dcspy/master)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=emcek_dcspy&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=emcek_dcspy)
-[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6056/badge)](https://bestpractices.coreinfrastructure.org/projects/6056)
-[![Downloads](https://pepy.tech/badge/dcspy)](https://pepy.tech/project/dcspy)
-[![Rate this package](https://badges.openbase.com/python/rating/dcspy.svg?token=AZCVj1Hdbl6cC3I/gkVpgsigp22LtCOR0sB8lcODY9Y=)](https://openbase.com/python/dcspy?utm_source=embedded&amp;utm_medium=badge&amp;utm_campaign=rate-badge)
-
-![dcspylogo](https://i.imgur.com/eqqrPB8.jpg)
-## DCSpy
-DCSpy is able to pull information from DCS aircraft and display on Logitech G-series keyboards LCD.
-It supports:
-* Logitech device with 160x43 px (4 lines) monochrome LCD - **G13**, **G15 (v1 and v2)** and **G510**
-* Logitech device with 320x240 px (8 lines) full RGBA LCD - **G19**
-
-See more information on [Wiki](https://github.com/emcek/dcspy/wiki) page.
-
-## Sponsored by Jetbrains Open Source Support Program
-[![logo](https://resources.jetbrains.com/storage/products/company/brand/logos/PyCharm.svg)](https://jb.gg/OpenSourceSupport)
-[![logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.svg)](https://jb.gg/OpenSourceSupport)
-
-## Aircraft and instruments
-* F/A-18C Hornet UFC - Up Front Controller
-* F-16C Viper DED - Data Entry Display
-* Ka-50 Black Shark II and III - PVI-800 and autopilot channels
-* Mi-8MTV2 Hip - autopilot channels and Radios information
-* Mi-24P Hind - Autopilot channels and modes and Radios information
-* A-10C Warthog and A-10C II Tank Killer - Radio frequency information
-* F-14A and F-14B Tomcat - basic support for RIO CAP
-* AV-8B Night Attack Harrier - Up Front Controller and Option Display Unit
-* AH-64D Apache - Enhanced Up Front Display
-* more to come....
-
-## Requirements
-* [Python 3.11](https://www.python.org/downloads/) but 3.7+ (with tcl/tk support, see [installation](https://github.com/emcek/dcspy/wiki/installation)) should be fine, please choose Windows x86-64 version, file should be python-3.11.1-amd64.exe.
-* [Logitech Gaming Software 9.04.49](https://support.logitech.com/software/lgs)
-* [DCS-BIOS 0.7.47](https://github.com/DCSFlightpanels/dcs-bios/releases/latest) (or newer)
-* DCS World: [2.8.2.35759](https://www.digitalcombatsimulator.com/en/news/changelog/openbeta/2.8.2.35759/) Open Beta
-
-**Notes:**
-* If you upgrade DCSpy from 1.5.1 or older you can safely remove Logitech LCD SDK from `C:\Program Files\Logitech Gaming Software\LCDSDK_8.57.148`. Since DCSpy version 1.6.0 use built-in SDK in LGS (Logitech Gaming Software).
-
-## New ideas
-I have lots of plans and new ideas how to improve it internally and form user's perspective, but don't hesitate to contact me. Maybe it will motivate me to implement some new stuff. Please open issue if you find bug or have any crazy idea.
-You are welcome [dcspy Discord](https://discord.gg/SP5Yjx3) server.
-
-## Contributing
-You want contribute, perfect see: [contributing](./CONTRIBUTING.md) guide.
-
-## Credits
-More details [here](https://github.com/emcek/dcspy/wiki/Information#credits).
+[![image](https://img.shields.io/badge/pypi-v2.0.0-blue.svg)](https://pypi.org/project/dcspy/)
+[![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
+[![License](https://img.shields.io/badge/Licence-MIT-blue.svg)](./LICENSE.md)
+[![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
+[![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
+[![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
+[![Discord](https://img.shields.io/discord/672486999516774442?label=Discord&logo=discord&logoColor=lightblue)](https://discord.gg/SP5Yjx3)
+[![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://github.com/emcek/dcspy)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/emcek/dcspy/master.svg)](https://results.pre-commit.ci/latest/github/emcek/dcspy/master)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=emcek_dcspy&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=emcek_dcspy)
+[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6056/badge)](https://bestpractices.coreinfrastructure.org/projects/6056)
+[![Downloads](https://pepy.tech/badge/dcspy)](https://pepy.tech/project/dcspy)
+[![Rate this package](https://badges.openbase.com/python/rating/dcspy.svg?token=AZCVj1Hdbl6cC3I/gkVpgsigp22LtCOR0sB8lcODY9Y=)](https://openbase.com/python/dcspy?utm_source=embedded&amp;utm_medium=badge&amp;utm_campaign=rate-badge)
+
+![dcspylogo](https://i.imgur.com/eqqrPB8.jpg)
+## DCSpy
+DCSpy is able to pull information from DCS aircraft and display on Logitech G-series keyboards LCD.
+It supports:
+* Logitech device with 160x43 px (4 lines) monochrome LCD - **G13**, **G15 (v1 and v2)** and **G510**
+* Logitech device with 320x240 px (8 lines) full RGBA LCD - **G19**
+
+See more information on [Wiki](https://github.com/emcek/dcspy/wiki) page.
+
+## Sponsored by Jetbrains Open Source Support Program
+[![logo](https://resources.jetbrains.com/storage/products/company/brand/logos/PyCharm.svg)](https://jb.gg/OpenSourceSupport)
+[![logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.svg)](https://jb.gg/OpenSourceSupport)
+
+## Aircraft and instruments
+* F/A-18C Hornet UFC - Up Front Controller
+* F-16C Viper DED - Data Entry Display
+* Ka-50 Black Shark II and III - PVI-800 and autopilot channels
+* Mi-8MTV2 Hip - autopilot channels and Radios information
+* Mi-24P Hind - Autopilot channels and modes and Radios information
+* A-10C Warthog and A-10C II Tank Killer - Radio frequency information
+* F-14A and F-14B Tomcat - basic support for RIO CAP
+* AV-8B Night Attack Harrier - Up Front Controller and Option Display Unit
+* AH-64D Apache - Enhanced Up Front Display
+* more to come....
+
+## Requirements
+* [Logitech Gaming Software 9.04.49](https://support.logitech.com/software/lgs)
+* [DCS-BIOS 0.7.48](https://github.com/DCSFlightpanels/dcs-bios/releases/latest) or newer (can be installed directly from DCSpy)
+* DCS World: [2.8.4.39731](https://www.digitalcombatsimulator.com/en/news/changelog/openbeta/2.8.4.39731/) Open Beta (any release 2.8.* should work)
+* (optional) [Python 3.11](https://www.python.org/downloads/) but 3.7+ should be fine (with tcl/tk support, see [installation](https://github.com/emcek/dcspy/wiki/installation))
+
+**Notes:**
+* If you upgrade DCSpy from 1.5.1 or older you can safely remove Logitech LCD SDK from `C:\Program Files\Logitech Gaming Software\LCDSDK_8.57.148`. Since DCSpy version 1.6.0 use built-in SDK in LGS (Logitech Gaming Software).
+
+## New ideas
+I have lots of plans and new ideas how to improve it internally and form user's perspective, but don't hesitate to contact me. Maybe it will motivate me to implement some new stuff. Please open issue if you find bug or have any crazy idea.
+You are welcome [dcspy Discord](https://discord.gg/SP5Yjx3) server.
+
+## Contributing
+You want contribute, perfect see: [contributing](./CONTRIBUTING.md) guide.
+
+## Credits
+More details [here](https://github.com/emcek/dcspy/wiki/Information#credits).
```

### Comparing `dcspy-1.9.5/dcspy/G13.png` & `dcspy-2.0.0/dcspy/G13.png`

 * *Files identical despite different names*

### Comparing `dcspy-1.9.5/dcspy/G15v1.png` & `dcspy-2.0.0/dcspy/G15v1.png`

 * *Files identical despite different names*

### Comparing `dcspy-1.9.5/dcspy/G15v2.png` & `dcspy-2.0.0/dcspy/G15v2.png`

 * *Files identical despite different names*

### Comparing `dcspy-1.9.5/dcspy/G19.png` & `dcspy-2.0.0/dcspy/G19.png`

 * *Files identical despite different names*

### Comparing `dcspy-1.9.5/dcspy/G510.png` & `dcspy-2.0.0/dcspy/G510.png`

 * *Files identical despite different names*

### Comparing `dcspy-1.9.5/dcspy/__init__.py` & `dcspy-2.0.0/dcspy/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,96 +1,126 @@
-from dataclasses import dataclass
-from enum import Enum
-from logging import getLogger
-from os import name, path
-from platform import architecture, uname, python_implementation, python_version
-from sys import platform
-from typing import Union, Sequence
-
-from PIL import ImageFont
-
-from dcspy.log import config_logger
-from dcspy.sdk import lcd_sdk
-from dcspy.utils import load_cfg, set_defaults, default_yaml
-
-SUPPORTED_CRAFTS = {'FA18Chornet': {'name': 'F/A-18C Hornet', 'bios': 'FA-18C_hornet'},
-                    'Ka50': {'name': 'Ka-50 Black Shark II', 'bios': 'Ka-50'},
-                    'Ka503': {'name': 'Ka-50 Black Shark III', 'bios': 'Ka-50'},
-                    'Mi8MT': {'name': 'Mi-8MTV2 Magnificent Eight', 'bios': 'Mi-8MT'},
-                    'Mi24P': {'name': 'Mi-24P Hind', 'bios': 'Mi-24P'},
-                    'F16C50': {'name': 'F-16C Viper', 'bios': 'F-16C_50'},
-                    'AH64DBLKII': {'name': 'AH-64D Apache', 'bios': 'AH-64D'},
-                    'A10C': {'name': 'A-10C Warthog', 'bios': 'A-10C'},
-                    'A10C2': {'name': 'A-10C II Tank Killer', 'bios': 'A-10C2'},
-                    'F14A135GR': {'name': 'F-14A Tomcat', 'bios': 'F14'},
-                    'F14B': {'name': 'F-14B Tomcat', 'bios': 'F-14'},
-                    'AV8BNA': {'name': 'AV-8B N/A Harrier', 'bios': 'AV8BNA'},
-                    }
-SEND_ADDR = ('127.0.0.1', 7778)
-RECV_ADDR = ('', 5010)
-MULTICAST_IP = '239.255.50.10'
-
-
-class LcdType(Enum):
-    """LCD Type."""
-    MONO = lcd_sdk.TYPE_MONO
-    COLOR = lcd_sdk.TYPE_COLOR
-
-
-class LcdButton(Enum):
-    """LCD Buttons."""
-    NONE = 0x0
-    ONE = 0x1
-    TWO = 0x2
-    THREE = 0x4
-    FOUR = 0x8
-    LEFT = 0x100
-    RIGHT = 0x200
-    OK = 0x400
-    CANCEL = 0x800
-    UP = 0x1000
-    DOWN = 0x2000
-    MENU = 0x4000
-
-
-@dataclass
-class LcdInfo:
-    """LCD info."""
-    width: int
-    height: int
-    type: LcdType
-    buttons: Sequence[LcdButton]
-    foreground: Union[int, Sequence[int]]
-    background: Union[int, Sequence[int]]
-    mode: str
-    font_xs: ImageFont.FreeTypeFont
-    font_s: ImageFont.FreeTypeFont
-    font_l: ImageFont.FreeTypeFont
-
-
-config = set_defaults(load_cfg())
-
-LcdMono = LcdInfo(width=lcd_sdk.MONO_WIDTH, height=lcd_sdk.MONO_HEIGHT, type=LcdType.MONO, foreground=255,
-                  buttons=(LcdButton.ONE, LcdButton.TWO, LcdButton.THREE, LcdButton.FOUR),
-                  background=0, mode='1', font_s=ImageFont.truetype(config['font_name'], config['font_mono_s']),
-                  font_l=ImageFont.truetype(config['font_name'], config['font_mono_l']),
-                  font_xs=ImageFont.truetype(config['font_name'], config['font_mono_xs']))
-LcdColor = LcdInfo(width=lcd_sdk.COLOR_WIDTH, height=lcd_sdk.COLOR_HEIGHT, type=LcdType.COLOR, foreground=(0, 255, 0, 255),
-                   buttons=(LcdButton.LEFT, LcdButton.RIGHT, LcdButton.UP, LcdButton.DOWN, LcdButton.OK, LcdButton.CANCEL, LcdButton.MENU),
-                   background=(0, 0, 0, 0), mode='RGBA', font_s=ImageFont.truetype(config['font_name'], config['font_color_s']),
-                   font_l=ImageFont.truetype(config['font_name'], config['font_color_l']),
-                   font_xs=ImageFont.truetype(config['font_name'], config['font_color_xs']))
-DED_FONT = ImageFont.truetype(f'{path.abspath(path.dirname(__file__))}/falconded.ttf', 25)
-LCD_TYPES = {
-    'G19': {'type': 'KeyboardColor', 'icon': 'G19.png'},
-    'G510': {'type': 'KeyboardMono', 'icon': 'G510.png'},
-    'G15 v1': {'type': 'KeyboardMono', 'icon': 'G15v1.png'},
-    'G15 v2': {'type': 'KeyboardMono', 'icon': 'G15v2.png'},
-    'G13': {'type': 'KeyboardMono', 'icon': 'G13.png'},
-}
-LOG = getLogger(__name__)
-config_logger(LOG, config['verbose'])
-
-LOG.debug(f'Arch: {name} / {platform} / {" / ".join(architecture())}')
-LOG.debug(f'Python: {python_implementation()}-{python_version()}')
-LOG.debug(f'{uname()}')
-LOG.info(f'Configuration: {config} from: {default_yaml}')
+from dataclasses import dataclass
+from enum import Enum
+from logging import getLogger
+from os import name
+from pathlib import Path
+from platform import architecture, uname, python_implementation, python_version
+from sys import platform
+from typing import Union, Sequence
+
+from PIL import ImageFont
+
+from dcspy.log import config_logger
+from dcspy.sdk import lcd_sdk
+from dcspy.utils import load_cfg, set_defaults, get_default_yaml
+try:
+    from typing import NotRequired
+except ImportError:
+    from typing_extensions import NotRequired
+try:
+    from typing import TypedDict
+except ImportError:
+    from typing_extensions import TypedDict
+
+
+SUPPORTED_CRAFTS = {
+    'FA18Chornet': {'name': 'F/A-18C Hornet', 'bios': 'FA-18C_hornet'},
+    'Ka50': {'name': 'Ka-50 Black Shark II', 'bios': 'Ka-50'},
+    'Ka503': {'name': 'Ka-50 Black Shark III', 'bios': 'Ka-50'},
+    'Mi8MT': {'name': 'Mi-8MTV2 Magnificent Eight', 'bios': 'Mi-8MT'},
+    'Mi24P': {'name': 'Mi-24P Hind', 'bios': 'Mi-24P'},
+    'F16C50': {'name': 'F-16C Viper', 'bios': 'F-16C_50'},
+    'AH64DBLKII': {'name': 'AH-64D Apache', 'bios': 'AH-64D'},
+    'A10C': {'name': 'A-10C Warthog', 'bios': 'A-10C'},
+    'A10C2': {'name': 'A-10C II Tank Killer', 'bios': 'A-10C2'},
+    'F14A135GR': {'name': 'F-14A Tomcat', 'bios': 'F14'},
+    'F14B': {'name': 'F-14B Tomcat', 'bios': 'F-14'},
+    'AV8BNA': {'name': 'AV-8B N/A Harrier', 'bios': 'AV8BNA'},
+}
+SEND_ADDR = ('127.0.0.1', 7778)
+RECV_ADDR = ('', 5010)
+MULTICAST_IP = '239.255.50.10'
+LOCAL_APPDATA = True
+
+
+class LcdType(Enum):
+    """LCD Type."""
+    MONO = lcd_sdk.TYPE_MONO
+    COLOR = lcd_sdk.TYPE_COLOR
+
+
+class LcdButton(Enum):
+    """LCD Buttons."""
+    NONE = 0x0
+    ONE = 0x1
+    TWO = 0x2
+    THREE = 0x4
+    FOUR = 0x8
+    LEFT = 0x100
+    RIGHT = 0x200
+    OK = 0x400
+    CANCEL = 0x800
+    UP = 0x1000
+    DOWN = 0x2000
+    MENU = 0x4000
+
+
+@dataclass
+class LcdInfo:
+    """LCD info."""
+    width: int
+    height: int
+    type: LcdType
+    buttons: Sequence[LcdButton]
+    foreground: Union[int, Sequence[int]]
+    background: Union[int, Sequence[int]]
+    mode: str
+    font_xs: ImageFont.FreeTypeFont
+    font_s: ImageFont.FreeTypeFont
+    font_l: ImageFont.FreeTypeFont
+
+
+default_yaml = get_default_yaml(local_appdata=LOCAL_APPDATA)
+config = set_defaults(load_cfg(filename=default_yaml), filename=default_yaml)
+LcdMono = LcdInfo(width=lcd_sdk.MONO_WIDTH, height=lcd_sdk.MONO_HEIGHT, type=LcdType.MONO, foreground=255,
+                  buttons=(LcdButton.ONE, LcdButton.TWO, LcdButton.THREE, LcdButton.FOUR),
+                  background=0, mode='1', font_s=ImageFont.truetype(config['font_name'], config['font_mono_s']),
+                  font_l=ImageFont.truetype(config['font_name'], config['font_mono_l']),
+                  font_xs=ImageFont.truetype(config['font_name'], config['font_mono_xs']))
+LcdColor = LcdInfo(width=lcd_sdk.COLOR_WIDTH, height=lcd_sdk.COLOR_HEIGHT, type=LcdType.COLOR, foreground=(0, 255, 0, 255),
+                   buttons=(LcdButton.LEFT, LcdButton.RIGHT, LcdButton.UP, LcdButton.DOWN, LcdButton.OK, LcdButton.CANCEL, LcdButton.MENU),
+                   background=(0, 0, 0, 0), mode='RGBA', font_s=ImageFont.truetype(config['font_name'], config['font_color_s']),
+                   font_l=ImageFont.truetype(config['font_name'], config['font_color_l']),
+                   font_xs=ImageFont.truetype(config['font_name'], config['font_color_xs']))
+DED_FONT = ImageFont.truetype(str(Path(__file__).resolve().with_name('falconded.ttf')), 25)
+LCD_TYPES = {
+    'G19': {'type': 'KeyboardColor', 'icon': 'G19.png'},
+    'G510': {'type': 'KeyboardMono', 'icon': 'G510.png'},
+    'G15 v1': {'type': 'KeyboardMono', 'icon': 'G15v1.png'},
+    'G15 v2': {'type': 'KeyboardMono', 'icon': 'G15v2.png'},
+    'G13': {'type': 'KeyboardMono', 'icon': 'G13.png'},
+}
+LOG = getLogger(__name__)
+config_logger(LOG, config['verbose'])
+
+LOG.debug(f'Arch: {name} / {platform} / {" / ".join(architecture())}')
+LOG.debug(f'Python: {python_implementation()}-{python_version()}')
+LOG.debug(f'{uname()}')
+LOG.info(f'Configuration: {config} from: {default_yaml}')
+
+
+class IntBuffArgs(TypedDict):
+    address: int
+    mask: int
+    shift_by: int
+
+
+class StrBuffArgs(TypedDict):
+    address: int
+    max_length: int
+
+
+class BiosValue(TypedDict):
+    klass: str
+    args: Union[StrBuffArgs, IntBuffArgs]
+    value: Union[int, str]
+    max_value: NotRequired[int]
```

### Comparing `dcspy-1.9.5/dcspy/aircraft.py` & `dcspy-2.0.0/dcspy/aircraft.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,1004 +1,999 @@
-from enum import Enum
-from functools import partial
-from itertools import chain, cycle
-from logging import getLogger
-from os import path
-from pprint import pformat
-from re import search, sub
-from string import whitespace
-from tempfile import gettempdir
-from typing import Dict, Union, Iterator, Sequence, List
-
-from PIL import Image, ImageDraw, ImageFont
-
-from dcspy import LcdInfo, LcdButton, LcdType, SUPPORTED_CRAFTS, DED_FONT, config
-from dcspy.sdk import lcd_sdk
-
-try:
-    from typing_extensions import TypedDict
-except ImportError:
-    from typing import TypedDict
-
-BIOS_VALUE = TypedDict('BIOS_VALUE', {'class': str, 'args': Dict[str, int], 'value': Union[int, str], 'max_value': int}, total=False)
-LOG = getLogger(__name__)
-
-
-class Aircraft:
-    """Common Aircraft."""
-    def __init__(self, lcd_type: LcdInfo) -> None:
-        """
-        Create common aircraft.
-
-        :param lcd_type: LCD type
-        """
-        self.lcd = lcd_type
-        self.bios_data: Dict[str, BIOS_VALUE] = {}
-        self.cycle_buttons: Dict[str, Iterator[int]] = {}
-        self._debug_img = cycle(chain([f'{x:02}' for x in range(10)], range(10, 99)))
-
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
-        """
-        Prepare aircraft specific DCS-BIOS request for button pressed.
-
-        For G13/G15/G510: 1-4
-        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
-
-        :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
-        :return: ready to send DCS-BIOS request
-        """
-        LOG.debug(f'{self.__class__.__name__} Button: {button}')
-        LOG.debug(f'Request: {request.replace(whitespace[2], " ")}')
-        return request
-
-    def prepare_image(self) -> Image.Image:
-        """
-        Prepare image to be sent to correct type of LCD.
-
-        :return: image instance ready display on LCD
-        """
-        img_for_lcd = {'mono': partial(Image.new, mode='1', size=(self.lcd.width, self.lcd.height), color=self.lcd.background),
-                       'color': partial(Image.new, mode='RGBA', size=(self.lcd.width, self.lcd.height), color=self.lcd.background)}
-
-        lcd_type = self.lcd.type.name.lower()
-        img = img_for_lcd[lcd_type]()
-        getattr(self, f'draw_for_lcd_{lcd_type}')(img)
-        img.save(path.join(gettempdir(), f'{self.__class__.__name__}_{next(self._debug_img)}.png'), 'PNG')
-        return img
-
-    def set_bios(self, selector: str, value: str) -> None:
-        """
-        Set value for DCS-BIOS selector.
-
-        :param selector:
-        :param value:
-        """
-        self.bios_data[selector]['value'] = value
-        LOG.debug(f'{self.__class__.__name__} {selector} value: "{value}"')
-        lcd_sdk.update_display(self.prepare_image())
-
-    def get_bios(self, selector: str) -> Union[str, int]:
-        """
-        Get value for DCS-BIOS selector.
-
-        :param selector:
-        """
-        try:
-            return self.bios_data[selector]['value']
-        except KeyError:
-            return ''
-
-    def draw_for_lcd_mono(self, img: Image.Image) -> None:
-        """Prepare image for Aircraft for Mono LCD."""
-        raise NotImplementedError
-
-    def draw_for_lcd_color(self, img: Image.Image) -> None:
-        """Prepare image for Aircraft for Color LCD."""
-        raise NotImplementedError
-
-    def get_next_value_for_button(self, btn_name: str) -> int:
-        """
-        Get next int value (cycle fore and back) for button name.
-
-        :param btn_name: BIOS button name
-        """
-        if not self.cycle_buttons[btn_name]:
-            curr_val = int(self.get_bios(btn_name))
-            max_val = self.bios_data[btn_name]['max_value']
-            full_seed = list(range(max_val + 1)) + list(range(max_val - 1, 0, -1)) + list(range(max_val + 1))
-            seed = full_seed[curr_val + 1:2 * max_val + curr_val + 1]
-            LOG.debug(f'{self.__class__.__name__} {btn_name} full_seed: {full_seed} seed: {seed} curr_val: {curr_val}')
-            self.cycle_buttons[btn_name] = cycle(chain(seed))
-        return next(self.cycle_buttons[btn_name])
-
-    def __repr__(self) -> str:
-        """
-        Show all details of Aircraft.
-
-        :return: string
-        """
-        return f'{super().__repr__()} with: {pformat(self.__dict__)}'
-
-
-class FA18Chornet(Aircraft):
-    """F/A-18C Hornet."""
-    def __init__(self, lcd_type: LcdInfo) -> None:
-        """
-        Create F/A-18C Hornet.
-
-        :param lcd_type: LCD type
-        """
-        super().__init__(lcd_type)
-        self.bios_data: Dict[str, BIOS_VALUE] = {
-            'UFC_SCRATCHPAD_STRING_1_DISPLAY': {'class': 'StringBuffer', 'args': {'address': 0x744e, 'max_length': 2}, 'value': ''},
-            'UFC_SCRATCHPAD_STRING_2_DISPLAY': {'class': 'StringBuffer', 'args': {'address': 0x7450, 'max_length': 2}, 'value': ''},
-            'UFC_SCRATCHPAD_NUMBER_DISPLAY': {'class': 'StringBuffer', 'args': {'address': 0x7446, 'max_length': 8}, 'value': ''},
-            'UFC_OPTION_DISPLAY_1': {'class': 'StringBuffer', 'args': {'address': 0x7432, 'max_length': 4}, 'value': ''},
-            'UFC_OPTION_DISPLAY_2': {'class': 'StringBuffer', 'args': {'address': 0x7436, 'max_length': 4}, 'value': ''},
-            'UFC_OPTION_DISPLAY_3': {'class': 'StringBuffer', 'args': {'address': 0x743a, 'max_length': 4}, 'value': ''},
-            'UFC_OPTION_DISPLAY_4': {'class': 'StringBuffer', 'args': {'address': 0x743e, 'max_length': 4}, 'value': ''},
-            'UFC_OPTION_DISPLAY_5': {'class': 'StringBuffer', 'args': {'address': 0x7442, 'max_length': 4}, 'value': ''},
-            'UFC_COMM1_DISPLAY': {'class': 'StringBuffer', 'args': {'address': 0x7424, 'max_length': 2}, 'value': ''},
-            'UFC_COMM2_DISPLAY': {'class': 'StringBuffer', 'args': {'address': 0x7426, 'max_length': 2}, 'value': ''},
-            'UFC_OPTION_CUEING_1': {'class': 'StringBuffer', 'args': {'address': 0x7428, 'max_length': 1}, 'value': ''},
-            'UFC_OPTION_CUEING_2': {'class': 'StringBuffer', 'args': {'address': 0x742a, 'max_length': 1}, 'value': ''},
-            'UFC_OPTION_CUEING_3': {'class': 'StringBuffer', 'args': {'address': 0x742c, 'max_length': 1}, 'value': ''},
-            'UFC_OPTION_CUEING_4': {'class': 'StringBuffer', 'args': {'address': 0x742e, 'max_length': 1}, 'value': ''},
-            'UFC_OPTION_CUEING_5': {'class': 'StringBuffer', 'args': {'address': 0x7430, 'max_length': 1}, 'value': ''},
-            'IFEI_FUEL_DOWN': {'class': 'StringBuffer', 'args': {'address': 0x748a, 'max_length': 6}, 'value': ''},
-            'IFEI_FUEL_UP': {'class': 'StringBuffer', 'args': {'address': 0x7490, 'max_length': 6}, 'value': ''},
-            'HUD_ATT_SW': {'class': 'IntegerBuffer', 'args': {'address': 0x742e, 'mask': 0x300, 'shift_by': 0x8}, 'value': int(), 'max_value': 2},
-            'IFEI_DWN_BTN': {'class': 'IntegerBuffer', 'args': {'address': 0x7466, 'mask': 0x10, 'shift_by': 0x4}, 'value': int(), 'max_value': 1},
-            'IFEI_UP_BTN': {'class': 'IntegerBuffer', 'args': {'address': 0x7466, 'mask': 0x8, 'shift_by': 0x3}, 'value': int(), 'max_value': 1}}
-        self.cycle_buttons = {'HUD_ATT_SW': '', 'IFEI_DWN_BTN': '', 'IFEI_UP_BTN': ''}  # type: ignore
-
-    def _draw_common_data(self, draw: ImageDraw, scale: int) -> ImageDraw:
-        """
-        Draw common part (based on scale) for Mono and Color LCD.
-
-        :param draw: ImageDraw instance
-        :param scale: scaling factor (Mono 1, Color 2)
-        :return: updated image to draw
-        """
-        scratch_1 = self.get_bios("UFC_SCRATCHPAD_STRING_1_DISPLAY")
-        scratch_2 = self.get_bios("UFC_SCRATCHPAD_STRING_2_DISPLAY")
-        scratch_num = self.get_bios("UFC_SCRATCHPAD_NUMBER_DISPLAY")
-        draw.text(xy=(0, 0), fill=self.lcd.foreground, font=self.lcd.font_l,
-                  text=f'{scratch_1}{scratch_2}{scratch_num}')
-        draw.line(xy=(0, 20 * scale, 115 * scale, 20 * scale), fill=self.lcd.foreground, width=1)
-
-        draw.rectangle(xy=(0, 29 * scale, 20 * scale, 42 * scale), fill=self.lcd.background, outline=self.lcd.foreground)
-        draw.text(xy=(2 * scale, 29 * scale), text=self.get_bios('UFC_COMM1_DISPLAY'), fill=self.lcd.foreground, font=self.lcd.font_l)
-
-        offset = 44 * scale
-        draw.rectangle(xy=(139 * scale - offset, 29 * scale, 159 * scale - offset, 42 * scale), fill=self.lcd.background, outline=self.lcd.foreground)
-        draw.text(xy=(140 * scale - offset, 29 * scale), text=self.get_bios('UFC_COMM2_DISPLAY'), fill=self.lcd.foreground, font=self.lcd.font_l)
-
-        for i in range(1, 6):
-            offset = (i - 1) * 8 * scale
-            draw.text(xy=(120 * scale, offset), fill=self.lcd.foreground, font=self.lcd.font_s,
-                      text=f'{i}{self.get_bios(f"UFC_OPTION_CUEING_{i}")}{self.get_bios(f"UFC_OPTION_DISPLAY_{i}")}')
-
-        draw.text(xy=(36 * scale, 29 * scale), text=self.get_bios('IFEI_FUEL_UP'), fill=self.lcd.foreground, font=self.lcd.font_l)
-        return draw
-
-    def draw_for_lcd_mono(self, img: Image.Image) -> None:
-        """Prepare image for F/A-18C Hornet for Mono LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
-
-    def draw_for_lcd_color(self, img: Image.Image) -> None:
-        """Prepare image for F/A-18C Hornet for Color LCD."""
-        draw = self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
-        draw.text(xy=(72, 100), text=self.get_bios('IFEI_FUEL_DOWN'), fill=self.lcd.foreground, font=self.lcd.font_l)
-
-    def set_bios(self, selector: str, value: str) -> None:
-        """
-        Set new data.
-
-        :param selector:
-        :param value:
-        """
-        if selector in ('UFC_SCRATCHPAD_STRING_1_DISPLAY', 'UFC_SCRATCHPAD_STRING_2_DISPLAY',
-                        'UFC_COMM1_DISPLAY', 'UFC_COMM2_DISPLAY'):
-            value = value.replace('`', '1').replace('~', '2')
-        super().set_bios(selector, value)
-
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
-        """
-        Prepare F/A-18 Hornet specific DCS-BIOS request for button pressed.
-
-        For G13/G15/G510: 1-4
-        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
-
-        :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
-        :return: ready to send DCS-BIOS request
-        """
-        button_map = {LcdButton.OK: 'HUD_ATT_SW', LcdButton.CANCEL: 'IFEI_UP_BTN', LcdButton.MENU: 'IFEI_DWN_BTN'}
-        settings = 0
-        button_bios_name = ''
-        if button in button_map:
-            button_bios_name = button_map[button]
-            settings = self.get_next_value_for_button(button_bios_name)
-        action = {LcdButton.ONE: 'UFC_COMM1_CHANNEL_SELECT DEC\n',
-                  LcdButton.TWO: 'UFC_COMM1_CHANNEL_SELECT INC\n',
-                  LcdButton.THREE: 'UFC_COMM2_CHANNEL_SELECT DEC\n',
-                  LcdButton.FOUR: 'UFC_COMM2_CHANNEL_SELECT INC\n',
-                  LcdButton.LEFT: 'UFC_COMM1_CHANNEL_SELECT DEC\n',
-                  LcdButton.RIGHT: 'UFC_COMM1_CHANNEL_SELECT INC\n',
-                  LcdButton.DOWN: 'UFC_COMM2_CHANNEL_SELECT DEC\n',
-                  LcdButton.UP: 'UFC_COMM2_CHANNEL_SELECT INC\n',
-                  LcdButton.MENU: f'{button_bios_name} {settings}\n',
-                  LcdButton.CANCEL: f'{button_bios_name} {settings}\n',
-                  LcdButton.OK: f'{button_bios_name} {settings}\n'}
-        return super().button_request(button, action.get(button, '\n'))
-
-
-class F16C50(Aircraft):
-    """F-16C Viper."""
-    def __init__(self, lcd_type: LcdInfo) -> None:
-        """
-        Create F-16C Viper.
-
-        :param lcd_type: LCD type
-        """
-        super().__init__(lcd_type)
-        self.font = self.lcd.font_s
-        self.ded_font = config['f16_ded_font']
-        if self.ded_font and self.lcd.type == LcdType.COLOR:
-            self.font = DED_FONT
-        self.bios_data: Dict[str, BIOS_VALUE] = {
-            'DED_LINE_1': {'class': 'StringBuffer', 'args': {'address': 0x450a, 'max_length': 29}, 'value': ''},
-            'DED_LINE_2': {'class': 'StringBuffer', 'args': {'address': 0x4528, 'max_length': 29}, 'value': ''},
-            'DED_LINE_3': {'class': 'StringBuffer', 'args': {'address': 0x4546, 'max_length': 29}, 'value': ''},
-            'DED_LINE_4': {'class': 'StringBuffer', 'args': {'address': 0x4564, 'max_length': 29}, 'value': ''},
-            'DED_LINE_5': {'class': 'StringBuffer', 'args': {'address': 0x4582, 'max_length': 29}, 'value': ''},
-            'IFF_MASTER_KNB': {'class': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0xe, 'shift_by': 0x1}, 'value': int(), 'max_value': 4},
-            'IFF_ENABLE_SW': {'class': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0x600, 'shift_by': 0x9}, 'value': int(), 'max_value': 2},
-            'IFF_M4_CODE_SW': {'class': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0x30, 'shift_by': 0x4}, 'value': int(), 'max_value': 2},
-            'IFF_M4_REPLY_SW': {'class': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0xc0, 'shift_by': 0x6}, 'value': int(), 'max_value': 2}}
-        self.cycle_buttons = {'IFF_MASTER_KNB': '', 'IFF_ENABLE_SW': '', 'IFF_M4_CODE_SW': '', 'IFF_M4_REPLY_SW': ''}  # type: ignore
-
-    def _draw_common_data(self, draw: ImageDraw, separation: int) -> None:
-        """
-        Draw common part (based on scale) for Mono and Color LCD.
-
-        :param draw: ImageDraw instance
-        :param separation: between lines in pixels
-        """
-        for i in range(1, 6):
-            offset = (i - 1) * separation
-            draw.text(xy=(0, offset), text=self.get_bios(f'DED_LINE_{i}'), fill=self.lcd.foreground, font=self.font)
-
-    def draw_for_lcd_mono(self, img: Image.Image) -> None:
-        """Prepare image for F-16C Viper for Mono LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img), separation=8)
-
-    def draw_for_lcd_color(self, img: Image.Image) -> None:
-        """Prepare image for F-16C Viper for Color LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img), separation=24)
-
-    def set_bios(self, selector: str, value: str) -> None:
-        """
-        Catch BIOS changes and remove garbage characters and replace with correct ones.
-
-        :param selector: selector name
-        :param value: value form DCS-BIOS
-        """
-        if 'DED_LINE_' in selector:
-            LOG.debug(f'{self.__class__.__name__} {selector} org  : "{value}"')
-            for character in ['A\x10\x04', '\x82', '\x03', '\x02', '\x80', '\x08', '\x10', '\x07', '\x0f', '\xfe', '\xfc', '\x03', '\xff', '\xc0']:
-                value = value.replace(character, '')  # List page
-            if value and value[-1] == '@':
-                value = value.replace('@', '')  # List - 6
-            if self.lcd.type == LcdType.MONO:
-                value = value.replace('o', '\u00b0')  # 'o' to degree sign
-                value = value.replace('a', '\u2666')  # 'a' to up-down arrow 2195 or black diamond 2666
-                value = value.replace('*', '\u25d9')  # INVERSE WHITE CIRCLE
-            elif self.ded_font and self.lcd.type == LcdType.COLOR:
-                value = value.replace('o', '\u005e')  # replace 'o' to degree sign
-                value = value.replace('a', '\u0040')  # fix up-down triangle arrow
-                value = value.replace('*', '\u00d7')  # fix to inverse star
-                value = sub(r'1DEST\s2BNGO\s3VIP\s{2}RINTG', '\u00c1DEST \u00c2BNGO \u00c3VIP  \u0072INTG', value)
-                value = sub(r'4NAV\s{2}5MAN\s{2}6INS\s{2}EDLNK', '\u00c4NAV  \u00c5MAN  \u00c6INS  \u0065DLNK', value)
-                value = sub(r'7CMDS\s8MODE\s9VRP\s{2}0MISC', '\u00c7CMDS \u00c8MODE \u00c9VRP  \u00c0MISC', value)
-                value = sub(r'1CORR\s2MAGV\s3OFP\s{2}RHMCS', '\u00c1CORR \u00c2MAGV \u00c3OFP  \u0072HMCS', value)
-                value = sub(r'4INSM\s5LASR\s6GPS\s{2}E', '\u00c4INSM \u00c5LASR \u00c6GPS  \u0065', value)
-                value = sub(r'7DRNG\s8BULL\s9\s{5}0', '\u00c7DRNG \u00c8BULL \u00c9     \u00c0', value)
-                value = sub(r'(M1\s:\d+\s+)M4(\s+\(\d\).*)', r'\1mÄ\2', value)
-                value = sub(r'M1(\s:\d+\s+)M4(\s+:\s+\(\d\).*)', r'mÁ\1mÄ\2', value)
-                value = sub(r'M3(\s+:\d+\s+×\s+\d×[A-Z]+\(\d\).*)', r'mÃ\1', value)
-                value = sub(r'(\s[\s|×])HUD BLNK([×|\s]\s+)', r'\1hud blnk\2', value)
-                value = sub(r'(\s[\s|×])CKPT BLNK([×|\s]\s+)', r'\1ckpt blnk\2', value)
-        super().set_bios(selector, value)
-
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
-        """
-        Prepare F-16C Viper specific DCS-BIOS request for button pressed.
-
-        For G13/G15/G510: 1-4
-        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
-
-        :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
-        :return: ready to send DCS-BIOS request
-        """
-        button_map = {LcdButton.ONE: 'IFF_MASTER_KNB',
-                      LcdButton.TWO: 'IFF_ENABLE_SW',
-                      LcdButton.THREE: 'IFF_M4_CODE_SW',
-                      LcdButton.FOUR: 'IFF_M4_REPLY_SW',
-                      LcdButton.LEFT: 'IFF_MASTER_KNB',
-                      LcdButton.RIGHT: 'IFF_ENABLE_SW',
-                      LcdButton.DOWN: 'IFF_M4_CODE_SW',
-                      LcdButton.UP: 'IFF_M4_REPLY_SW'}
-        settings = 0
-        button_bios_name = ''
-        if button in button_map:
-            button_bios_name = button_map[button]
-            settings = self.get_next_value_for_button(button_bios_name)
-        action = {LcdButton.ONE: f'{button_bios_name} {settings}\n',
-                  LcdButton.TWO: f'{button_bios_name} {settings}\n',
-                  LcdButton.THREE: f'{button_bios_name} {settings}\n',
-                  LcdButton.FOUR: f'{button_bios_name} {settings}\n',
-                  LcdButton.LEFT: f'{button_bios_name} {settings}\n',
-                  LcdButton.RIGHT: f'{button_bios_name} {settings}\n',
-                  LcdButton.DOWN: f'{button_bios_name} {settings}\n',
-                  LcdButton.UP: f'{button_bios_name} {settings}\n'}
-        return super().button_request(button, action.get(button, '\n'))
-
-
-class Ka50(Aircraft):
-    """Ka-50 Black Shark."""
-    def __init__(self, lcd_type: LcdInfo) -> None:
-        """
-        Create Ka-50 Black Shark.
-
-        :param lcd_type: LCD type
-        """
-        super().__init__(lcd_type)
-        self.bios_data: Dict[str, BIOS_VALUE] = {
-            'PVI_LINE1_APOSTROPHE1': {'class': 'StringBuffer', 'args': {'address': 0x1934, 'max_length': 1}, 'value': ''},
-            'PVI_LINE1_APOSTROPHE2': {'class': 'StringBuffer', 'args': {'address': 0x1936, 'max_length': 1}, 'value': ''},
-            'PVI_LINE1_POINT': {'class': 'StringBuffer', 'args': {'address': 0x1930, 'max_length': 1}, 'value': ''},
-            'PVI_LINE1_SIGN': {'class': 'StringBuffer', 'args': {'address': 0x1920, 'max_length': 1}, 'value': ''},
-            'PVI_LINE1_TEXT': {'class': 'StringBuffer', 'args': {'address': 0x1924, 'max_length': 6}, 'value': ''},
-            'PVI_LINE2_APOSTROPHE1': {'class': 'StringBuffer', 'args': {'address': 0x1938, 'max_length': 1}, 'value': ''},
-            'PVI_LINE2_APOSTROPHE2': {'class': 'StringBuffer', 'args': {'address': 0x193a, 'max_length': 1}, 'value': ''},
-            'PVI_LINE2_POINT': {'class': 'StringBuffer', 'args': {'address': 0x1932, 'max_length': 1}, 'value': ''},
-            'PVI_LINE2_SIGN': {'class': 'StringBuffer', 'args': {'address': 0x1922, 'max_length': 1}, 'value': ''},
-            'PVI_LINE2_TEXT': {'class': 'StringBuffer', 'args': {'address': 0x192a, 'max_length': 6}, 'value': ''},
-            'AP_ALT_HOLD_LED': {'class': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x8000, 'shift_by': 0xf}, 'value': int()},
-            'AP_BANK_HOLD_LED': {'class': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x200, 'shift_by': 0x9}, 'value': int()},
-            'AP_FD_LED': {'class': 'IntegerBuffer', 'args': {'address': 0x1938, 'mask': 0x200, 'shift_by': 0x9}, 'value': int()},
-            'AP_HDG_HOLD_LED': {'class': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x800, 'shift_by': 0xb}, 'value': int()},
-            'AP_PITCH_HOLD_LED': {'class': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x2000, 'shift_by': 0xd}, 'value': int()}}
-
-    def _draw_common_data(self, draw: ImageDraw, scale: int) -> None:
-        """
-        Draw common part (based on scale) for Mono and Color LCD.
-
-        :param draw: ImageDraw instance
-        :param scale: scaling factor (Mono 1, Color 2)
-        """
-        for rect_xy in [
-            (0 * scale, 1 * scale, 85 * scale, 18 * scale),
-            (0 * scale, 22 * scale, 85 * scale, 39 * scale),
-            (88 * scale, 1 * scale, 103 * scale, 18 * scale),
-            (88 * scale, 22 * scale, 103 * scale, 39 * scale),
-        ]:
-            draw.rectangle(xy=rect_xy, fill=self.lcd.background, outline=self.lcd.foreground)
-        line1, line2 = self._generate_pvi_lines()
-        draw.text(xy=(2 * scale, 3 * scale), text=line1, fill=self.lcd.foreground, font=self.lcd.font_l)
-        draw.text(xy=(2 * scale, 24 * scale), text=line2, fill=self.lcd.foreground, font=self.lcd.font_l)
-        self._auto_pilot_switch(draw, scale)
-
-    def _generate_pvi_lines(self) -> Sequence[str]:
-        """
-        Generate coordinate strings.
-
-        :return: tuple of string
-        """
-        text1, text2 = '', ''
-        line1_text = str(self.get_bios('PVI_LINE1_TEXT'))
-        line2_text = str(self.get_bios('PVI_LINE2_TEXT'))
-        if line1_text:
-            l1_apostr1 = self.get_bios("PVI_LINE1_APOSTROPHE1")
-            l1_apostr2 = self.get_bios("PVI_LINE1_APOSTROPHE2")
-            text1 = f'{line1_text[-6:-3]}{l1_apostr1}{line1_text[-3:-1]}{l1_apostr2}{line1_text[-1]}'
-        if line2_text:
-            l2_apostr1 = self.get_bios("PVI_LINE2_APOSTROPHE1")
-            l2_apostr2 = self.get_bios("PVI_LINE2_APOSTROPHE2")
-            text2 = f'{line2_text[-6:-3]}{l2_apostr1}{line2_text[-3:-1]}{l2_apostr2}{line2_text[-1]}'
-        line1 = f'{self.get_bios("PVI_LINE1_SIGN")}{text1} {self.get_bios("PVI_LINE1_POINT")}'
-        line2 = f'{self.get_bios("PVI_LINE2_SIGN")}{text2} {self.get_bios("PVI_LINE2_POINT")}'
-        return line1, line2
-
-    def _auto_pilot_switch(self, draw_obj: ImageDraw, scale: int) -> None:
-        """
-        Draw rectangle and add text for autopilot channels in correct coordinates.
-
-        :param draw_obj: ImageDraw object form PIL
-        :param scale: scaling factor (Mono 1, Color 2)
-        """
-        for c_rect, c_text, ap_channel, turn_on in (
-                ((111 * scale, 1 * scale, 124 * scale, 18 * scale), (113 * scale, 3 * scale), 'B', self.get_bios('AP_BANK_HOLD_LED')),
-                ((128 * scale, 1 * scale, 141 * scale, 18 * scale), (130 * scale, 3 * scale), 'P', self.get_bios('AP_PITCH_HOLD_LED')),
-                ((145 * scale, 1 * scale, 158 * scale, 18 * scale), (147 * scale, 3 * scale), 'F', self.get_bios('AP_FD_LED')),
-                ((111 * scale, 22 * scale, 124 * scale, 39 * scale), (113 * scale, 24 * scale), 'H', self.get_bios('AP_HDG_HOLD_LED')),
-                ((128 * scale, 22 * scale, 141 * scale, 39 * scale), (130 * scale, 24 * scale), 'A', self.get_bios('AP_ALT_HOLD_LED')),
-        ):
-            draw_autopilot_channels(self.lcd, ap_channel, c_rect, c_text, draw_obj, turn_on)
-
-    def draw_for_lcd_mono(self, img: Image.Image) -> None:
-        """Prepare image for Ka-50 Black Shark for Mono LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
-
-    def draw_for_lcd_color(self, img: Image.Image) -> None:
-        """Prepare image for Ka-50 Black Shark for Mono LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
-
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
-        """
-        Prepare Ka-50 Black Shark specific DCS-BIOS request for button pressed.
-
-        For G13/G15/G510: 1-4
-        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
-
-        :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
-        :return: ready to send DCS-BIOS request
-        """
-        action = {LcdButton.ONE: 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n',
-                  LcdButton.TWO: 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n',
-                  LcdButton.THREE: 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n',
-                  LcdButton.FOUR: 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n',
-                  LcdButton.LEFT: 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n',
-                  LcdButton.RIGHT: 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n',
-                  LcdButton.DOWN: 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n',
-                  LcdButton.UP: 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'}
-        return super().button_request(button, action.get(button, '\n'))
-
-
-class Ka503(Ka50):
-    """Ka-50 Black Shark III."""
-    pass
-
-
-class Mi8MT(Aircraft):
-    """Mi-8MTV2 Magnificent Eight."""
-
-    def __init__(self, lcd_type: LcdInfo) -> None:
-        """
-        Create Mi-8MTV2 Magnificent Eight.
-
-        :param lcd_type: LCD type
-        """
-        super().__init__(lcd_type)
-        self.bios_data: Dict[str, BIOS_VALUE] = {
-            'LMP_AP_HDG_ON': {'class': 'IntegerBuffer', 'args': {'address': 0x269e, 'mask': 0x20, 'shift_by': 0x5}, 'value': int()},
-            'LMP_AP_PITCH_ROLL_ON': {'class': 'IntegerBuffer', 'args': {'address': 0x269e, 'mask': 0x80, 'shift_by': 0x7}, 'value': int()},
-            'LMP_AP_HEIGHT_ON': {'class': 'IntegerBuffer', 'args': {'address': 0x269e, 'mask': 0x100, 'shift_by': 0x8}, 'value': int()},
-            'R863_CNL_SEL': {'class': 'IntegerBuffer', 'args': {'address': 0x268c, 'mask': 0x1f, 'shift_by': 0x0}, 'value': int()},
-            'R863_MOD': {'class': 'IntegerBuffer', 'args': {'address': 0x263a, 'mask': 0x1000, 'shift_by': 0xc}, 'value': int()},
-            'R863_FREQ': {'class': 'StringBuffer', 'args': {'address': 0x2804, 'max_length': 7}, 'value': ''},
-            'R828_PRST_CHAN_SEL': {'class': 'IntegerBuffer', 'args': {'address': 0x268e, 'mask': 0x780, 'shift_by': 0x7}, 'value': int()},
-            'YADRO1A_FREQ': {'class': 'StringBuffer', 'args': {'address': 0x2692, 'max_length': 7}, 'value': ''},
-        }
-
-    def _draw_common_data(self, draw: ImageDraw, scale: int) -> None:
-        """
-        Draw common part (based on scale) for Mono and Color LCD.
-
-        :param draw: ImageDraw instance
-        :param scale: scaling factor (Mono 1, Color 2)
-        """
-        for c_rect, c_text, ap_channel, turn_on in (
-                ((111 * scale, 1 * scale, 124 * scale, 18 * scale), (113 * scale, 3 * scale), 'H', self.get_bios('LMP_AP_HDG_ON')),
-                ((128 * scale, 1 * scale, 141 * scale, 18 * scale), (130 * scale, 3 * scale), 'P', self.get_bios('LMP_AP_PITCH_ROLL_ON')),
-                ((145 * scale, 1 * scale, 158 * scale, 18 * scale), (147 * scale, 3 * scale), 'A', self.get_bios('LMP_AP_HEIGHT_ON'))):
-            draw_autopilot_channels(self.lcd, ap_channel, c_rect, c_text, draw, turn_on)
-
-        r863, r828, yadro = self._generate_radio_values()
-        for i, line in enumerate([f'R828 {r828}', f'YADRO1 {yadro}', f'R863 {r863}'], 1):
-            offset = i * 10 * scale
-            draw.text(xy=(0, offset), text=line, fill=self.lcd.foreground, font=self.lcd.font_s)
-
-    def draw_for_lcd_mono(self, img: Image.Image) -> None:
-        """Prepare image for Mi-8MTV2 Magnificent Eight for Mono LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
-
-    def draw_for_lcd_color(self, img: Image.Image) -> None:
-        """Prepare image for Mi-8MTV2 Magnificent Eight for Color LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
-
-    def _generate_radio_values(self) -> Sequence[str]:
-        """
-        Generate string data about Hip R863, R828, YADRO1A radios settings.
-
-        :return: All 3 radios settings as strings
-        """
-        r863_mod = 'FM' if int(self.get_bios("R863_MOD")) else 'AM'
-        try:
-            r863_freq = float(self.get_bios("R863_FREQ"))
-        except ValueError:
-            r863_freq = 0.0
-        try:
-            yadro_freq = float(self.get_bios("YADRO1A_FREQ"))
-        except ValueError:
-            yadro_freq = 0.0
-        r863 = f'Ch:{int(self.get_bios("R863_CNL_SEL")) + 1:>2} {r863_mod} {r863_freq:.3f}'
-        r828 = f'Ch:{int(self.get_bios("R828_PRST_CHAN_SEL")) + 1:>2}'
-        yadro = f'{yadro_freq:>7.1f}'
-        return r863, r828, yadro
-
-
-class Mi24P(Aircraft):
-    """Mi-24P Hind."""
-    def __init__(self, lcd_type: LcdInfo) -> None:
-        """
-        Create Mi-24P Hind.
-
-        :param lcd_type: LCD type
-        """
-        super().__init__(lcd_type)
-        self.bios_data: Dict[str, BIOS_VALUE] = {
-            'PLT_R863_CHAN': {'class': 'IntegerBuffer', 'args': {'address': 0x69ec, 'mask': 0x3e0, 'shift_by': 0x5}, 'value': int()},
-            'PLT_R863_MODUL': {'class': 'IntegerBuffer', 'args': {'address': 0x69ec, 'mask': 0x2, 'shift_by': 0x1}, 'value': int()},
-            'PLT_R828_CHAN': {'class': 'IntegerBuffer', 'args': {'address': 0x69fe, 'mask': 0xf00, 'shift_by': 0x8}, 'value': int()},
-            'JADRO_FREQ': {'class': 'StringBuffer', 'args': {'address': 0x6a04, 'max_length': 7}, 'value': ''},
-            'PLT_SAU_HOVER_MODE_ON_L': {'class': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x8000, 'shift_by': 0xf}, 'value': int()},
-            'PLT_SAU_ROUTE_MODE_ON_L': {'class': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x2000, 'shift_by': 0xd}, 'value': int()},
-            'PLT_SAU_ALT_MODE_ON_L': {'class': 'IntegerBuffer', 'args': {'address': 0x6902, 'mask': 0x100, 'shift_by': 0x8}, 'value': int()},
-            'PLT_SAU_H_ON_L': {'class': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x80, 'shift_by': 0x7}, 'value': int()},
-            'PLT_SAU_K_ON_L': {'class': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x20, 'shift_by': 0x5}, 'value': int()},
-            'PLT_SAU_T_ON_L': {'class': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x800, 'shift_by': 0xb}, 'value': int()},
-            'PLT_SAU_B_ON_L': {'class': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x200, 'shift_by': 0x9}, 'value': int()},
-        }
-
-    def _draw_common_data(self, draw: ImageDraw, scale: int) -> None:
-        """
-        Draw common part (based on scale) for Mono and Color LCD.
-
-        :param draw: ImageDraw instance
-        :param scale: scaling factor (Mono 1, Color 2)
-        """
-        for c_rect, c_text, ap_channel, turn_on in (
-                ((111 * scale, 1 * scale, 124 * scale, 18 * scale), (113 * scale, 3 * scale), 'H', self.get_bios('PLT_SAU_HOVER_MODE_ON_L')),
-                ((128 * scale, 1 * scale, 141 * scale, 18 * scale), (130 * scale, 3 * scale), 'R', self.get_bios('PLT_SAU_ROUTE_MODE_ON_L')),
-                ((145 * scale, 1 * scale, 158 * scale, 18 * scale), (147 * scale, 3 * scale), 'A', self.get_bios('PLT_SAU_ALT_MODE_ON_L')),
-                ((94 * scale, 22 * scale, 107 * scale, 39 * scale), (96 * scale, 24 * scale), 'Y', self.get_bios('PLT_SAU_H_ON_L')),
-                ((111 * scale, 22 * scale, 124 * scale, 39 * scale), (113 * scale, 24 * scale), 'R', self.get_bios('PLT_SAU_K_ON_L')),
-                ((128 * scale, 22 * scale, 141 * scale, 39 * scale), (130 * scale, 24 * scale), 'P', self.get_bios('PLT_SAU_T_ON_L')),
-                ((145 * scale, 22 * scale, 158 * scale, 39 * scale), (147 * scale, 24 * scale), 'A', self.get_bios('PLT_SAU_B_ON_L')),
-        ):
-            draw_autopilot_channels(self.lcd, ap_channel, c_rect, c_text, draw, turn_on)
-
-        r863, r828, yadro = self._generate_radio_values()
-        for i, line in enumerate([f'R828 {r828}', f'R863 {r863}', f'YADRO1 {yadro}'], 1):
-            offset = i * 10 * scale
-            draw.text(xy=(0, offset), text=line, fill=self.lcd.foreground, font=self.lcd.font_s)
-
-    def draw_for_lcd_mono(self, img: Image.Image) -> None:
-        """Prepare image for Mi-24P Hind for Mono LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
-
-    def draw_for_lcd_color(self, img: Image.Image) -> None:
-        """Prepare image for Mi-24P Hind for Color LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
-
-    def _generate_radio_values(self) -> Sequence[str]:
-        """
-        Generate string data about Hind R863, R828, YADRO1I radios settings.
-
-        :return: All 3 radios settings as strings
-        """
-        r863_mod = 'FM' if int(self.get_bios("PLT_R863_MODUL")) else 'AM'
-        try:
-            yadro_freq = float(self.get_bios("JADRO_FREQ"))
-        except ValueError:
-            yadro_freq = 0.0
-        r863 = f'Ch:{int(self.get_bios("PLT_R863_CHAN")) + 1:>2} {r863_mod}'
-        r828 = f'Ch:{int(self.get_bios("PLT_R828_CHAN")) + 1:>2}'
-        yadro = f'{yadro_freq:>7.1f}'
-        return r863, r828, yadro
-
-
-class ApacheEufdMode(Enum):
-    """Apache EUFD Mode."""
-    IDM = 1
-    WCA = 2
-    PRE = 4
-
-
-class AH64DBLKII(Aircraft):
-    """AH-64D Apache."""
-    def __init__(self, lcd_type: LcdInfo) -> None:
-        """
-        Create AH-64D Apache.
-
-        :param lcd_type: LCD type
-        """
-        super().__init__(lcd_type)
-        self.mode = ApacheEufdMode.IDM
-        self.warning_line = 1
-        self.bios_data: Dict[str, BIOS_VALUE] = {
-            'PLT_EUFD_LINE1': {'class': 'StringBuffer', 'args': {'address': 0x80c2, 'max_length': 56}, 'value': ''},
-            'PLT_EUFD_LINE2': {'class': 'StringBuffer', 'args': {'address': 0x80fa, 'max_length': 56}, 'value': ''},
-            'PLT_EUFD_LINE3': {'class': 'StringBuffer', 'args': {'address': 0x8132, 'max_length': 56}, 'value': ''},
-            'PLT_EUFD_LINE4': {'class': 'StringBuffer', 'args': {'address': 0x816a, 'max_length': 56}, 'value': ''},
-            'PLT_EUFD_LINE5': {'class': 'StringBuffer', 'args': {'address': 0x81a2, 'max_length': 56}, 'value': ''},
-            'PLT_EUFD_LINE6': {'class': 'StringBuffer', 'args': {'address': 0x81da, 'max_length': 56}, 'value': ''},
-            'PLT_EUFD_LINE7': {'class': 'StringBuffer', 'args': {'address': 0x8212, 'max_length': 56}, 'value': ''},
-            'PLT_EUFD_LINE8': {'class': 'StringBuffer', 'args': {'address': 0x824a, 'max_length': 56}, 'value': ''},
-            'PLT_EUFD_LINE9': {'class': 'StringBuffer', 'args': {'address': 0x8282, 'max_length': 56}, 'value': ''},
-            'PLT_EUFD_LINE10': {'class': 'StringBuffer', 'args': {'address': 0x82ba, 'max_length': 56}, 'value': ''},
-            'PLT_EUFD_LINE11': {'class': 'StringBuffer', 'args': {'address': 0x82f2, 'max_length': 56}, 'value': ''},
-            'PLT_EUFD_LINE12': {'class': 'StringBuffer', 'args': {'address': 0x832a, 'max_length': 56}, 'value': ''},
-            'PLT_EUFD_LINE14': {'class': 'StringBuffer', 'args': {'address': 0x839a, 'max_length': 56}, 'value': ''},
-        }
-
-    def draw_for_lcd_mono(self, img: Image.Image) -> None:
-        """Prepare image for AH-64D Apache for Mono LCD."""
-        LOG.debug(f'Mode: {self.mode}')
-        kwargs = {'draw': ImageDraw.Draw(img), 'scale': 1}
-        mode = self.mode.name.lower()
-        if mode == 'pre':
-            kwargs['xcords'] = [0] * 5 + [80] * 5
-            kwargs['ycords'] = [j * 8 for j in range(0, 5)] * 2
-            kwargs['font'] = self.lcd.font_xs
-            del kwargs['scale']
-        getattr(self, f'_draw_for_{mode}')(**kwargs)
-
-    def draw_for_lcd_color(self, img: Image.Image) -> None:
-        """Prepare image for AH-64D Apache for Color LCD."""
-        LOG.debug(f'Mode: {self.mode}')
-        kwargs = {'draw': ImageDraw.Draw(img), 'scale': 2}
-        mode = self.mode.name.lower()
-        if mode == 'pre':
-            kwargs['xcords'] = [0] * 10
-            kwargs['ycords'] = [j * 24 for j in range(0, 10)]
-            kwargs['font'] = self.lcd.font_l
-            del kwargs['scale']
-        getattr(self, f'_draw_for_{mode}')(**kwargs)
-
-    def _draw_for_idm(self, draw: ImageDraw.Draw, scale: int):
-        """
-        Draw image for IDM mode.
-
-        :param draw: ImageDraw instance
-        :param scale: scaling factor (Mono 1, Color 2)
-        """
-        for i in range(8, 13):
-            offset = (i - 8) * 8 * scale
-            mat = search(r'(.*\*)\s+(\d+)([\.\dULCA]+)[-\sA-Z]*(\d+)([\.\dULCA]+)[\s-]+', str(self.get_bios(f'PLT_EUFD_LINE{i}')))
-            if mat:
-                spacer = ' ' * (6 - len(mat.group(3)))
-                text = f'{mat.group(1):>7}{mat.group(2):>4}{mat.group(3):5<}{spacer}{mat.group(4):>4}{mat.group(5):5<}'
-                draw.text(xy=(0, offset), text=text, fill=self.lcd.foreground, font=self.lcd.font_xs)
-
-    def _draw_for_wca(self, draw: ImageDraw.Draw, scale: int):
-        """
-        Draw image for WCA mode.
-
-        :param draw: ImageDraw instance
-        :param scale: scaling factor (Mono 1, Color 2)
-        """
-        warnings = self._fetch_warning_list()
-        LOG.debug(f'Warnings: {warnings}')
-        try:
-            for idx, warn_no in enumerate(range(self.warning_line - 1, self.warning_line + 4)):
-                line = idx * 8 * scale
-                draw.text(xy=(0, line), text=f'{idx + self.warning_line:2} {warnings[warn_no]}', fill=self.lcd.foreground, font=self.lcd.font_s)
-                if self.warning_line >= len(warnings) - 3:
-                    self.warning_line = 1
-        except IndexError:
-            self.warning_line = 1
-
-    def _fetch_warning_list(self) -> List[str]:
-        """
-        Fetch all warnings and return as list.
-
-        :return: list of warnings (as strings)
-        """
-        warn = []
-        for i in range(1, 8):
-            mat = search(r'(.*)\|(.*)\|(.*)', str(self.get_bios(f'PLT_EUFD_LINE{i}')))
-            if mat:
-                warn.extend([w for w in [mat.group(1).strip(), mat.group(2).strip(), mat.group(3).strip()] if w])
-        return warn
-
-    def _draw_for_pre(self, draw: ImageDraw.Draw, xcords: List[int], ycords: List[int], font: ImageFont.FreeTypeFont):
-        """
-        Draw image for PRE mode.
-
-        :param draw: ImageDraw instance
-        :param xcords: list of X coordinates
-        :param ycords: list of Y coordinates
-        :param font: font instance
-        :param scale: scaling factor (Mono 1, Color 2)
-        """
-        match_dict = {2: r'.*\|.*\|([\u2192\s]CO CMD)\s*([\d\.]*)\s+',
-                      3: r'.*\|.*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
-                      4: r'.*\|.*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
-                      5: r'.*\|.*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
-                      6: r'\s*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
-                      7: r'\s*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
-                      8: r'\s*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
-                      9: r'\s*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
-                      10: r'\s*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
-                      11: r'\s*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+'}
-        for i, xcord, ycord in zip(range(2, 12), xcords, ycords):
-            mat = search(match_dict[i], str(self.get_bios(f'PLT_EUFD_LINE{i}')))
-            if mat:
-                draw.text(xy=(xcord, ycord), text=f'{mat.group(1):<9}{mat.group(2):>7}',
-                          fill=self.lcd.foreground, font=font)
-
-    def set_bios(self, selector: str, value: str) -> None:
-        """
-        Set new data.
-
-        :param selector:
-        :param value:
-        """
-        if selector == 'PLT_EUFD_LINE1':
-            match = search(r'.*\|.*\|(PRESET TUNE)\s\w+', value)
-            self.mode = ApacheEufdMode.IDM
-            if match:
-                self.mode = ApacheEufdMode.PRE
-        if selector in ('PLT_EUFD_LINE8', 'PLT_EUFD_LINE9', 'PLT_EUFD_LINE10', 'PLT_EUFD_LINE11', 'PLT_EUFD_LINE12'):
-            LOG.debug(f'{self.__class__.__name__} {selector} original: "{value}"')
-            value = value.replace(']', '\u2666').replace('[', '\u25ca').replace('~', '\u25a0').\
-                replace('>', '\u25b8').replace('<', '\u25c2').replace('=', '\u2219')
-        if 'PLT_EUFD_LINE' in selector:
-            LOG.debug(f'{self.__class__.__name__} {selector} original: "{value}"')
-            value = value.replace('!', '\u2192')  # replace ! with ->
-        super().set_bios(selector, value)
-
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
-        """
-        Prepare AH-64D Apache specific DCS-BIOS request for button pressed.
-
-        For G13/G15/G510: 1-4
-        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
-
-        :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
-        :return: ready to send DCS-BIOS request
-        """
-        wca_or_idm = 'PLT_EUFD_WCA 0\nPLT_EUFD_WCA 1\n'
-        if self.mode == ApacheEufdMode.IDM:
-            wca_or_idm = 'PLT_EUFD_IDM 0\nPLT_EUFD_IDM 1\n'
-
-        if button in (LcdButton.FOUR, LcdButton.UP) and self.mode == ApacheEufdMode.IDM:
-            self.mode = ApacheEufdMode.WCA
-        elif button in (LcdButton.FOUR, LcdButton.UP) and self.mode != ApacheEufdMode.IDM:
-            self.mode = ApacheEufdMode.IDM
-
-        if button in (LcdButton.ONE, LcdButton.LEFT) and self.mode == ApacheEufdMode.WCA:
-            self.warning_line += 1
-
-        action = {LcdButton.ONE: wca_or_idm,
-                  LcdButton.TWO: 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n',
-                  LcdButton.THREE: 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n',
-                  LcdButton.FOUR: 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n',
-                  LcdButton.LEFT: wca_or_idm,
-                  LcdButton.RIGHT: 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n',
-                  LcdButton.DOWN: 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n',
-                  LcdButton.UP: 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n'}
-        return super().button_request(button, action.get(button, '\n'))
-
-
-class A10C(Aircraft):
-    """A-10C Warthog."""
-    def __init__(self, lcd_type: LcdInfo) -> None:
-        """
-        Create A-10C Warthog or A-10C II Tank Killer.
-
-        :param lcd_type: LCD type
-        """
-        super().__init__(lcd_type)
-        self.bios_data: Dict[str, BIOS_VALUE] = {
-            'VHFAM_FREQ1': {'class': 'StringBuffer', 'args': {'address': 0x1190, 'max_length': 2}, 'value': ''},
-            'VHFAM_FREQ2': {'class': 'IntegerBuffer', 'args': {'address': 0x118e, 'mask': 0xf0, 'shift_by': 0x4}, 'value': int()},
-            'VHFAM_FREQ3': {'class': 'IntegerBuffer', 'args': {'address': 0x118e, 'mask': 0xf00, 'shift_by': 0x8}, 'value': int()},
-            'VHFAM_FREQ4': {'class': 'StringBuffer', 'args': {'address': 0x1192, 'max_length': 2}, 'value': ''},
-            'VHFFM_FREQ1': {'class': 'StringBuffer', 'args': {'address': 0x119a, 'max_length': 2}, 'value': ''},
-            'VHFFM_FREQ2': {'class': 'IntegerBuffer', 'args': {'address': 0x119c, 'mask': 0xf, 'shift_by': 0x0}, 'value': int()},
-            'VHFFM_FREQ3': {'class': 'IntegerBuffer', 'args': {'address': 0x119c, 'mask': 0xf0, 'shift_by': 0x4}, 'value': int()},
-            'VHFFM_FREQ4': {'class': 'StringBuffer', 'args': {'address': 0x119e, 'max_length': 2}, 'value': ''},
-            'UHF_100MHZ_SEL': {'class': 'StringBuffer', 'args': {'address': 0x1178, 'max_length': 1}, 'value': ''},
-            'UHF_10MHZ_SEL': {'class': 'IntegerBuffer', 'args': {'address': 0x1170, 'mask': 0x3c00, 'shift_by': 0xa}, 'value': int()},
-            'UHF_1MHZ_SEL': {'class': 'IntegerBuffer', 'args': {'address': 0x1178, 'mask': 0xf00, 'shift_by': 0x8}, 'value': int()},
-            'UHF_POINT1MHZ_SEL': {'class': 'IntegerBuffer', 'args': {'address': 0x1178, 'mask': 0xf000, 'shift_by': 0xc}, 'value': int()},
-            'UHF_POINT25_SEL': {'class': 'StringBuffer', 'args': {'address': 0x117a, 'max_length': 2}, 'value': ''}}
-
-    def _generate_freq_values(self) -> Sequence[str]:
-        """
-        Generate frequency for all 3 radios (VHF AM, VHF FM and UHF).
-
-        :return: All 3 frequency settings as strings
-        """
-        vhfam = f'{self.get_bios("VHFAM_FREQ1")}{self.get_bios("VHFAM_FREQ2")}.' \
-                f'{self.get_bios("VHFAM_FREQ3")}{self.get_bios("VHFAM_FREQ4")}'
-        vhffm = f'{self.get_bios("VHFFM_FREQ1")}{self.get_bios("VHFFM_FREQ2")}.' \
-                f'{self.get_bios("VHFFM_FREQ3")}{self.get_bios("VHFFM_FREQ4")}'
-        uhf = f'{self.get_bios("UHF_100MHZ_SEL")}{self.get_bios("UHF_10MHZ_SEL")}{self.get_bios("UHF_1MHZ_SEL")}.' \
-              f'{self.get_bios("UHF_POINT1MHZ_SEL")}{self.get_bios("UHF_POINT25_SEL")}'
-        return uhf, vhfam, vhffm
-
-    def draw_for_lcd_mono(self, img: Image.Image) -> None:
-        """Prepare image for A-10C Warthog or A-10C II Tank Killer for Mono LCD."""
-        draw = ImageDraw.Draw(img)
-        uhf, vhfam, vhffm = self._generate_freq_values()
-        for i, line in enumerate(['      *** RADIOS ***', f'VHF AM: {vhfam} MHz',
-                                  f'VHF FM: {vhffm} MHz', f'   UHF: {uhf} MHz']):
-            offset = i * 10
-            draw.text(xy=(0, offset), text=line, fill=self.lcd.foreground, font=self.lcd.font_s)
-
-    def draw_for_lcd_color(self, img: Image.Image) -> None:
-        """Prepare image for A-10C Warthog or A-10C II Tank Killer for Color LCD."""
-        draw = ImageDraw.Draw(img)
-        uhf, vhfam, vhffm = self._generate_freq_values()
-        for i, line in enumerate(['      *** RADIOS ***', f'VHF AM: {vhfam} MHz',
-                                  f'VHF FM: {vhffm} MHz', f'   UHF: {uhf} MHz']):
-            offset = i * 20
-            draw.text(xy=(0, offset), text=line, fill=self.lcd.foreground, font=self.lcd.font_s)
-
-
-class A10C2(A10C):
-    """A-10C II Tank Killer."""
-    pass
-
-
-class F14B(Aircraft):
-    """F-14B Tomcat."""
-    def __init__(self, lcd_type: LcdInfo) -> None:
-        """
-        Create F-14B Tomcat.
-
-        :param lcd_type: LCD type
-        """
-        super().__init__(lcd_type)
-        self.bios_data: Dict[str, BIOS_VALUE] = {
-            'RIO_CAP_CLEAR': {'class': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x4000, 'shift_by': 0xe}, 'value': int()},
-            'RIO_CAP_SW': {'class': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x2000, 'shift_by': 0xd}, 'value': int()},
-            'RIO_CAP_NE': {'class': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x1000, 'shift_by': 0xc}, 'value': int()},
-            'RIO_CAP_ENTER': {'class': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x8000, 'shift_by': 0xf}, 'value': int()}}
-
-    def _draw_common_data(self, draw: ImageDraw) -> None:
-        """
-        Draw common part for Mono and Color LCD.
-
-        :param draw: ImageDraw instance
-        """
-        draw.text(xy=(2, 3), text=f'{SUPPORTED_CRAFTS[self.__class__.__name__]["name"]}', fill=self.lcd.foreground, font=self.lcd.font_l)
-
-    def draw_for_lcd_mono(self, img: Image.Image) -> None:
-        """Prepare image for F-14B Tomcat for Mono LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img))
-
-    def draw_for_lcd_color(self, img: Image.Image) -> None:
-        """Prepare image for F-14B Tomcat for Color LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img))
-
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
-        """
-        Prepare F-14B Tomcat specific DCS-BIOS request for button pressed.
-
-        For G13/G15/G510: 1-4
-        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
-
-        :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
-        :return: ready to send DCS-BIOS request
-        """
-        action = {LcdButton.ONE: 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n',
-                  LcdButton.TWO: 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n',
-                  LcdButton.THREE: 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n',
-                  LcdButton.FOUR: 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n',
-                  LcdButton.LEFT: 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n',
-                  LcdButton.RIGHT: 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n',
-                  LcdButton.DOWN: 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n',
-                  LcdButton.UP: 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'}
-        return super().button_request(button, action.get(button, '\n'))
-
-
-class F14A135GR(F14B):
-    """F-14A-135-GR Tomcat."""
-    pass
-
-
-class AV8BNA(Aircraft):
-    """AV-8B Night Attack."""
-    def __init__(self, lcd_type: LcdInfo) -> None:
-        """
-        Create AV-8B Night Attack.
-
-        :param lcd_type: LCD type
-        """
-        super().__init__(lcd_type)
-        self.bios_data: Dict[str, BIOS_VALUE] = {
-            'UFC_SCRATCHPAD': {'class': 'StringBuffer', 'args': {'address': 0x7984, 'max_length': 12}, 'value': ''},
-            'UFC_COMM1_DISPLAY': {'class': 'StringBuffer', 'args': {'address': 0x7954, 'max_length': 2}, 'value': ''},
-            'UFC_COMM2_DISPLAY': {'class': 'StringBuffer', 'args': {'address': 0x7956, 'max_length': 2}, 'value': ''},
-            'AV8BNA_ODU_1_SELECT': {'class': 'StringBuffer', 'args': {'address': 0x7966, 'max_length': 1}, 'value': ''},
-            'AV8BNA_ODU_1_Text': {'class': 'StringBuffer', 'args': {'address': 0x7968, 'max_length': 4}, 'value': ''},
-            'AV8BNA_ODU_2_SELECT': {'class': 'StringBuffer', 'args': {'address': 0x796c, 'max_length': 1}, 'value': ''},
-            'AV8BNA_ODU_2_Text': {'class': 'StringBuffer', 'args': {'address': 0x796e, 'max_length': 4}, 'value': ''},
-            'AV8BNA_ODU_3_SELECT': {'class': 'StringBuffer', 'args': {'address': 0x7972, 'max_length': 1}, 'value': ''},
-            'AV8BNA_ODU_3_Text': {'class': 'StringBuffer', 'args': {'address': 0x7974, 'max_length': 4}, 'value': ''},
-            'AV8BNA_ODU_4_SELECT': {'class': 'StringBuffer', 'args': {'address': 0x7978, 'max_length': 1}, 'value': ''},
-            'AV8BNA_ODU_4_Text': {'class': 'StringBuffer', 'args': {'address': 0x797a, 'max_length': 4}, 'value': ''},
-            'AV8BNA_ODU_5_SELECT': {'class': 'StringBuffer', 'args': {'address': 0x797e, 'max_length': 1}, 'value': ''},
-            'AV8BNA_ODU_5_Text': {'class': 'StringBuffer', 'args': {'address': 0x7980, 'max_length': 4}, 'value': ''}}
-
-    def _draw_common_data(self, draw: ImageDraw, scale: int) -> ImageDraw:
-        """
-        Draw common part (based on scale) for Mono and Color LCD.
-
-        :param draw: ImageDraw instance
-        :param scale: scaling factor (Mono 1, Color 2)
-        :return: updated image to draw
-        """
-        draw.text(xy=(50 * scale, 0), fill=self.lcd.foreground, font=self.lcd.font_l, text=f'{self.get_bios("UFC_SCRATCHPAD")}')
-        draw.line(xy=(50 * scale, 20 * scale, 160 * scale, 20 * scale), fill=self.lcd.foreground, width=1)
-
-        draw.rectangle(xy=(50 * scale, 29 * scale, 70 * scale, 42 * scale), fill=self.lcd.background, outline=self.lcd.foreground)
-        draw.text(xy=(52 * scale, 29 * scale), text=self.get_bios('UFC_COMM1_DISPLAY'), fill=self.lcd.foreground, font=self.lcd.font_l)
-
-        draw.rectangle(xy=(139 * scale, 29 * scale, 159 * scale, 42 * scale), fill=self.lcd.background, outline=self.lcd.foreground)
-        draw.text(xy=(140 * scale, 29 * scale), text=self.get_bios('UFC_COMM2_DISPLAY'), fill=self.lcd.foreground, font=self.lcd.font_l)
-
-        for i in range(1, 6):
-            offset = (i - 1) * 8 * scale
-            draw.text(xy=(0 * scale, offset), fill=self.lcd.foreground, font=self.lcd.font_s,
-                      text=f'{i}{self.get_bios(f"AV8BNA_ODU_{i}_SELECT")}{self.get_bios(f"AV8BNA_ODU_{i}_Text")}')
-        return draw
-
-    def draw_for_lcd_mono(self, img: Image.Image) -> None:
-        """Prepare image for AV-8B N/A for Mono LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
-
-    def draw_for_lcd_color(self, img: Image.Image) -> None:
-        """Prepare image for AV-8B N/A for Color LCD."""
-        self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
-
-    def button_request(self, button: LcdButton, request: str = '\n') -> str:
-        """
-        Prepare AV-8B N/A specific DCS-BIOS request for button pressed.
-
-        For G13/G15/G510: 1-4
-        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
-
-        :param button: LcdButton Enum
-        :param request: valid DCS-BIOS command as string
-        :return: ready to send DCS-BIOS request
-        """
-        action = {LcdButton.ONE: 'UFC_COM1_SEL -3200\n',
-                  LcdButton.TWO: 'UFC_COM1_SEL 3200\n',
-                  LcdButton.THREE: 'UFC_COM2_SEL -3200\n',
-                  LcdButton.FOUR: 'UFC_COM2_SEL 3200\n',
-                  LcdButton.LEFT: 'UFC_COM1_SEL -3200\n',
-                  LcdButton.RIGHT: 'UFC_COM1_SEL 3200\n',
-                  LcdButton.DOWN: 'UFC_COM2_SEL -3200\n',
-                  LcdButton.UP: 'UFC_COM2_SEL 3200\n'}
-        return super().button_request(button, action.get(button, '\n'))
-
-
-def draw_autopilot_channels(lcd: LcdInfo, ap_channel: str, c_rect: Sequence[int], c_text: Sequence[int], draw_obj: ImageDraw, turn_on: Union[str, int]) -> None:
-    """
-    Draw rectangles with background for autopilot channels.
-
-    :param lcd: instance of LCD
-    :param ap_channel: channel name
-    :param c_rect: coordinates for rectangle
-    :param c_text: coordinates for name
-    :param draw_obj: ImageDraw instance
-    :param turn_on: channel on/off, fill on/off
-    """
-    if turn_on:
-        draw_obj.rectangle(c_rect, fill=lcd.foreground, outline=lcd.foreground)
-        draw_obj.text(xy=c_text, text=ap_channel, fill=lcd.background, font=lcd.font_l)
-    else:
-        draw_obj.rectangle(xy=c_rect, fill=lcd.background, outline=lcd.foreground)
-        draw_obj.text(xy=c_text, text=ap_channel, fill=lcd.foreground, font=lcd.font_l)
+from enum import Enum
+from functools import partial
+from itertools import chain, cycle
+from logging import getLogger
+from pathlib import Path
+from pprint import pformat
+from re import search, sub
+from string import whitespace
+from tempfile import gettempdir
+from typing import Dict, Union, Iterator, Sequence, List
+
+from PIL import Image, ImageDraw, ImageFont
+
+from dcspy import LcdInfo, LcdButton, LcdType, SUPPORTED_CRAFTS, DED_FONT, config, BiosValue
+from dcspy.sdk import lcd_sdk
+
+
+LOG = getLogger(__name__)
+
+
+class Aircraft:
+    """Common Aircraft."""
+    def __init__(self, lcd_type: LcdInfo) -> None:
+        """
+        Create common aircraft.
+
+        :param lcd_type: LCD type
+        """
+        self.lcd = lcd_type
+        self.bios_data: Dict[str, BiosValue] = {}
+        self.cycle_buttons: Dict[str, Iterator[int]] = {}
+        self._debug_img = cycle(chain([f'{x:02}' for x in range(10)], range(10, 99)))
+
+    def button_request(self, button: LcdButton, request: str = '\n') -> str:
+        """
+        Prepare aircraft specific DCS-BIOS request for button pressed.
+
+        For G13/G15/G510: 1-4
+        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
+
+        :param button: LcdButton Enum
+        :param request: valid DCS-BIOS command as string
+        :return: ready to send DCS-BIOS request
+        """
+        LOG.debug(f'{self.__class__.__name__} Button: {button}')
+        LOG.debug(f'Request: {request.replace(whitespace[2], " ")}')
+        return request
+
+    def prepare_image(self) -> Image.Image:
+        """
+        Prepare image to be sent to correct type of LCD.
+
+        :return: image instance ready display on LCD
+        """
+        img_for_lcd = {'mono': partial(Image.new, mode='1', size=(self.lcd.width, self.lcd.height), color=self.lcd.background),
+                       'color': partial(Image.new, mode='RGBA', size=(self.lcd.width, self.lcd.height), color=self.lcd.background)}
+
+        lcd_type = self.lcd.type.name.lower()
+        img = img_for_lcd[lcd_type]()
+        getattr(self, f'draw_for_lcd_{lcd_type}')(img)
+        if config.get('save_lcd', False):
+            img.save(Path(gettempdir()) / f'{self.__class__.__name__}_{next(self._debug_img)}.png', 'PNG')
+        return img
+
+    def set_bios(self, selector: str, value: Union[str, int]) -> None:
+        """
+        Set value for DCS-BIOS selector.
+
+        :param selector:
+        :param value:
+        """
+        self.bios_data[selector]['value'] = value
+        LOG.debug(f'{self.__class__.__name__} {selector} value: "{value}"')
+        lcd_sdk.update_display(self.prepare_image())
+
+    def get_bios(self, selector: str) -> Union[str, int]:
+        """
+        Get value for DCS-BIOS selector.
+
+        :param selector:
+        """
+        try:
+            return self.bios_data[selector]['value']
+        except KeyError:
+            return ''
+
+    def draw_for_lcd_mono(self, img: Image.Image) -> None:
+        """Prepare image for Aircraft for Mono LCD."""
+        raise NotImplementedError
+
+    def draw_for_lcd_color(self, img: Image.Image) -> None:
+        """Prepare image for Aircraft for Color LCD."""
+        raise NotImplementedError
+
+    def get_next_value_for_button(self, btn_name: str) -> int:
+        """
+        Get next int value (cycle fore and back) for button name.
+
+        :param btn_name: BIOS button name
+        """
+        if not isinstance(self.cycle_buttons[btn_name], cycle):
+            curr_val = int(self.get_bios(btn_name))
+            max_val = self.bios_data[btn_name]['max_value']
+            full_seed = list(range(max_val + 1)) + list(range(max_val - 1, 0, -1)) + list(range(max_val + 1))
+            seed = full_seed[curr_val + 1:2 * max_val + curr_val + 1]
+            LOG.debug(f'{self.__class__.__name__} {btn_name} full_seed: {full_seed} seed: {seed} curr_val: {curr_val}')
+            self.cycle_buttons[btn_name] = cycle(chain(seed))
+        return next(self.cycle_buttons[btn_name])
+
+    def __repr__(self) -> str:
+        """
+        Show all details of Aircraft.
+
+        :return: string
+        """
+        return f'{super().__repr__()} with: {pformat(self.__dict__)}'
+
+
+class FA18Chornet(Aircraft):
+    """F/A-18C Hornet."""
+    def __init__(self, lcd_type: LcdInfo) -> None:
+        """
+        Create F/A-18C Hornet.
+
+        :param lcd_type: LCD type
+        """
+        super().__init__(lcd_type)
+        self.bios_data: Dict[str, BiosValue] = {
+            'UFC_SCRATCHPAD_STRING_1_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x744e, 'max_length': 2}, 'value': ''},
+            'UFC_SCRATCHPAD_STRING_2_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x7450, 'max_length': 2}, 'value': ''},
+            'UFC_SCRATCHPAD_NUMBER_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x7446, 'max_length': 8}, 'value': ''},
+            'UFC_OPTION_DISPLAY_1': {'klass': 'StringBuffer', 'args': {'address': 0x7432, 'max_length': 4}, 'value': ''},
+            'UFC_OPTION_DISPLAY_2': {'klass': 'StringBuffer', 'args': {'address': 0x7436, 'max_length': 4}, 'value': ''},
+            'UFC_OPTION_DISPLAY_3': {'klass': 'StringBuffer', 'args': {'address': 0x743a, 'max_length': 4}, 'value': ''},
+            'UFC_OPTION_DISPLAY_4': {'klass': 'StringBuffer', 'args': {'address': 0x743e, 'max_length': 4}, 'value': ''},
+            'UFC_OPTION_DISPLAY_5': {'klass': 'StringBuffer', 'args': {'address': 0x7442, 'max_length': 4}, 'value': ''},
+            'UFC_COMM1_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x7424, 'max_length': 2}, 'value': ''},
+            'UFC_COMM2_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x7426, 'max_length': 2}, 'value': ''},
+            'UFC_OPTION_CUEING_1': {'klass': 'StringBuffer', 'args': {'address': 0x7428, 'max_length': 1}, 'value': ''},
+            'UFC_OPTION_CUEING_2': {'klass': 'StringBuffer', 'args': {'address': 0x742a, 'max_length': 1}, 'value': ''},
+            'UFC_OPTION_CUEING_3': {'klass': 'StringBuffer', 'args': {'address': 0x742c, 'max_length': 1}, 'value': ''},
+            'UFC_OPTION_CUEING_4': {'klass': 'StringBuffer', 'args': {'address': 0x742e, 'max_length': 1}, 'value': ''},
+            'UFC_OPTION_CUEING_5': {'klass': 'StringBuffer', 'args': {'address': 0x7430, 'max_length': 1}, 'value': ''},
+            'IFEI_FUEL_DOWN': {'klass': 'StringBuffer', 'args': {'address': 0x748a, 'max_length': 6}, 'value': ''},
+            'IFEI_FUEL_UP': {'klass': 'StringBuffer', 'args': {'address': 0x7490, 'max_length': 6}, 'value': ''},
+            'HUD_ATT_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x742e, 'mask': 0x300, 'shift_by': 0x8}, 'value': int(), 'max_value': 2},
+            'IFEI_DWN_BTN': {'klass': 'IntegerBuffer', 'args': {'address': 0x7466, 'mask': 0x10, 'shift_by': 0x4}, 'value': int(), 'max_value': 1},
+            'IFEI_UP_BTN': {'klass': 'IntegerBuffer', 'args': {'address': 0x7466, 'mask': 0x8, 'shift_by': 0x3}, 'value': int(), 'max_value': 1}}
+        self.cycle_buttons = {'HUD_ATT_SW': iter([0]), 'IFEI_DWN_BTN': iter([0]), 'IFEI_UP_BTN': iter([0])}
+
+    def _draw_common_data(self, draw: ImageDraw, scale: int) -> ImageDraw:
+        """
+        Draw common part (based on scale) for Mono and Color LCD.
+
+        :param draw: ImageDraw instance
+        :param scale: scaling factor (Mono 1, Color 2)
+        :return: updated image to draw
+        """
+        scratch_1 = self.get_bios("UFC_SCRATCHPAD_STRING_1_DISPLAY")
+        scratch_2 = self.get_bios("UFC_SCRATCHPAD_STRING_2_DISPLAY")
+        scratch_num = self.get_bios("UFC_SCRATCHPAD_NUMBER_DISPLAY")
+        draw.text(xy=(0, 0), fill=self.lcd.foreground, font=self.lcd.font_l,
+                  text=f'{scratch_1}{scratch_2}{scratch_num}')
+        draw.line(xy=(0, 20 * scale, 115 * scale, 20 * scale), fill=self.lcd.foreground, width=1)
+
+        draw.rectangle(xy=(0, 29 * scale, 20 * scale, 42 * scale), fill=self.lcd.background, outline=self.lcd.foreground)
+        draw.text(xy=(2 * scale, 29 * scale), text=self.get_bios('UFC_COMM1_DISPLAY'), fill=self.lcd.foreground, font=self.lcd.font_l)
+
+        offset = 44 * scale
+        draw.rectangle(xy=(139 * scale - offset, 29 * scale, 159 * scale - offset, 42 * scale), fill=self.lcd.background, outline=self.lcd.foreground)
+        draw.text(xy=(140 * scale - offset, 29 * scale), text=self.get_bios('UFC_COMM2_DISPLAY'), fill=self.lcd.foreground, font=self.lcd.font_l)
+
+        for i in range(1, 6):
+            offset = (i - 1) * 8 * scale
+            draw.text(xy=(120 * scale, offset), fill=self.lcd.foreground, font=self.lcd.font_s,
+                      text=f'{i}{self.get_bios(f"UFC_OPTION_CUEING_{i}")}{self.get_bios(f"UFC_OPTION_DISPLAY_{i}")}')
+
+        draw.text(xy=(36 * scale, 29 * scale), text=self.get_bios('IFEI_FUEL_UP'), fill=self.lcd.foreground, font=self.lcd.font_l)
+        return draw
+
+    def draw_for_lcd_mono(self, img: Image.Image) -> None:
+        """Prepare image for F/A-18C Hornet for Mono LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
+
+    def draw_for_lcd_color(self, img: Image.Image) -> None:
+        """Prepare image for F/A-18C Hornet for Color LCD."""
+        draw = self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
+        draw.text(xy=(72, 100), text=self.get_bios('IFEI_FUEL_DOWN'), fill=self.lcd.foreground, font=self.lcd.font_l)
+
+    def set_bios(self, selector: str, value: Union[str, int]) -> None:
+        """
+        Set new data.
+
+        :param selector:
+        :param value:
+        """
+        if selector in ('UFC_SCRATCHPAD_STRING_1_DISPLAY', 'UFC_SCRATCHPAD_STRING_2_DISPLAY',
+                        'UFC_COMM1_DISPLAY', 'UFC_COMM2_DISPLAY'):
+            value = str(value).replace('`', '1').replace('~', '2')
+        super().set_bios(selector, value)
+
+    def button_request(self, button: LcdButton, request: str = '\n') -> str:
+        """
+        Prepare F/A-18 Hornet specific DCS-BIOS request for button pressed.
+
+        For G13/G15/G510: 1-4
+        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
+
+        :param button: LcdButton Enum
+        :param request: valid DCS-BIOS command as string
+        :return: ready to send DCS-BIOS request
+        """
+        button_map = {LcdButton.OK: 'HUD_ATT_SW', LcdButton.CANCEL: 'IFEI_UP_BTN', LcdButton.MENU: 'IFEI_DWN_BTN'}
+        settings = 0
+        button_bios_name = ''
+        if button in button_map:
+            button_bios_name = button_map[button]
+            settings = self.get_next_value_for_button(button_bios_name)
+        action = {LcdButton.ONE: 'UFC_COMM1_CHANNEL_SELECT DEC\n',
+                  LcdButton.TWO: 'UFC_COMM1_CHANNEL_SELECT INC\n',
+                  LcdButton.THREE: 'UFC_COMM2_CHANNEL_SELECT DEC\n',
+                  LcdButton.FOUR: 'UFC_COMM2_CHANNEL_SELECT INC\n',
+                  LcdButton.LEFT: 'UFC_COMM1_CHANNEL_SELECT DEC\n',
+                  LcdButton.RIGHT: 'UFC_COMM1_CHANNEL_SELECT INC\n',
+                  LcdButton.DOWN: 'UFC_COMM2_CHANNEL_SELECT DEC\n',
+                  LcdButton.UP: 'UFC_COMM2_CHANNEL_SELECT INC\n',
+                  LcdButton.MENU: f'{button_bios_name} {settings}\n',
+                  LcdButton.CANCEL: f'{button_bios_name} {settings}\n',
+                  LcdButton.OK: f'{button_bios_name} {settings}\n'}
+        return super().button_request(button, action.get(button, '\n'))
+
+
+class F16C50(Aircraft):
+    """F-16C Viper."""
+    def __init__(self, lcd_type: LcdInfo) -> None:
+        """
+        Create F-16C Viper.
+
+        :param lcd_type: LCD type
+        """
+        super().__init__(lcd_type)
+        self.font = self.lcd.font_s
+        self.ded_font = config.get('f16_ded_font', True)
+        if self.ded_font and self.lcd.type == LcdType.COLOR:
+            self.font = DED_FONT
+        self.bios_data: Dict[str, BiosValue] = {
+            'DED_LINE_1': {'klass': 'StringBuffer', 'args': {'address': 0x450a, 'max_length': 29}, 'value': ''},
+            'DED_LINE_2': {'klass': 'StringBuffer', 'args': {'address': 0x4528, 'max_length': 29}, 'value': ''},
+            'DED_LINE_3': {'klass': 'StringBuffer', 'args': {'address': 0x4546, 'max_length': 29}, 'value': ''},
+            'DED_LINE_4': {'klass': 'StringBuffer', 'args': {'address': 0x4564, 'max_length': 29}, 'value': ''},
+            'DED_LINE_5': {'klass': 'StringBuffer', 'args': {'address': 0x4582, 'max_length': 29}, 'value': ''},
+            'IFF_MASTER_KNB': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0xe, 'shift_by': 0x1}, 'value': int(), 'max_value': 4},
+            'IFF_ENABLE_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0x600, 'shift_by': 0x9}, 'value': int(), 'max_value': 2},
+            'IFF_M4_CODE_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0x30, 'shift_by': 0x4}, 'value': int(), 'max_value': 2},
+            'IFF_M4_REPLY_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0xc0, 'shift_by': 0x6}, 'value': int(), 'max_value': 2}}
+        self.cycle_buttons = {'IFF_MASTER_KNB': iter([0]), 'IFF_ENABLE_SW': iter([0]), 'IFF_M4_CODE_SW': iter([0]), 'IFF_M4_REPLY_SW': iter([0])}
+
+    def _draw_common_data(self, draw: ImageDraw, separation: int) -> None:
+        """
+        Draw common part (based on scale) for Mono and Color LCD.
+
+        :param draw: ImageDraw instance
+        :param separation: between lines in pixels
+        """
+        for i in range(1, 6):
+            offset = (i - 1) * separation
+            draw.text(xy=(0, offset), text=self.get_bios(f'DED_LINE_{i}'), fill=self.lcd.foreground, font=self.font)
+
+    def draw_for_lcd_mono(self, img: Image.Image) -> None:
+        """Prepare image for F-16C Viper for Mono LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img), separation=8)
+
+    def draw_for_lcd_color(self, img: Image.Image) -> None:
+        """Prepare image for F-16C Viper for Color LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img), separation=24)
+
+    def set_bios(self, selector: str, value: Union[str, int]) -> None:
+        """
+        Catch BIOS changes and remove garbage characters and replace with correct ones.
+
+        :param selector: selector name
+        :param value: value form DCS-BIOS
+        """
+        if 'DED_LINE_' in selector:
+            value = str(value)
+            LOG.debug(f'{self.__class__.__name__} {selector} org  : "{value}"')
+            for character in ['A\x10\x04', '\x82', '\x03', '\x02', '\x80', '\x08', '\x10', '\x07', '\x0f', '\xfe', '\xfc', '\x03', '\xff', '\xc0']:
+                value = value.replace(character, '')  # List page
+            if value and value[-1] == '@':
+                value = value.replace('@', '')  # List - 6
+            if self.lcd.type == LcdType.MONO:
+                value = value.replace('o', '\u00b0')  # 'o' to degree sign
+                value = value.replace('a', '\u2666')  # 'a' to up-down arrow 2195 or black diamond 2666
+                value = value.replace('*', '\u25d9')  # INVERSE WHITE CIRCLE
+            elif self.ded_font and self.lcd.type == LcdType.COLOR:
+                value = value.replace('o', '\u005e')  # replace 'o' to degree sign
+                value = value.replace('a', '\u0040')  # fix up-down triangle arrow
+                value = value.replace('*', '\u00d7')  # fix to inverse star
+                value = sub(r'1DEST\s2BNGO\s3VIP\s{2}RINTG', '\u00c1DEST \u00c2BNGO \u00c3VIP  \u0072INTG', value)
+                value = sub(r'4NAV\s{2}5MAN\s{2}6INS\s{2}EDLNK', '\u00c4NAV  \u00c5MAN  \u00c6INS  \u0065DLNK', value)
+                value = sub(r'7CMDS\s8MODE\s9VRP\s{2}0MISC', '\u00c7CMDS \u00c8MODE \u00c9VRP  \u00c0MISC', value)
+                value = sub(r'1CORR\s2MAGV\s3OFP\s{2}RHMCS', '\u00c1CORR \u00c2MAGV \u00c3OFP  \u0072HMCS', value)
+                value = sub(r'4INSM\s5LASR\s6GPS\s{2}E', '\u00c4INSM \u00c5LASR \u00c6GPS  \u0065', value)
+                value = sub(r'7DRNG\s8BULL\s9\s{5}0', '\u00c7DRNG \u00c8BULL \u00c9     \u00c0', value)
+                value = sub(r'(M1\s:\d+\s+)M4(\s+\(\d\).*)', r'\1mÄ\2', value)
+                value = sub(r'M1(\s:\d+\s+)M4(\s+:\s+\(\d\).*)', r'mÁ\1mÄ\2', value)
+                value = sub(r'M3(\s+:\d+\s+×\s+\d×[A-Z]+\(\d\).*)', r'mÃ\1', value)
+                value = sub(r'(\s[\s|×])HUD BLNK([×|\s]\s+)', r'\1hud blnk\2', value)
+                value = sub(r'(\s[\s|×])CKPT BLNK([×|\s]\s+)', r'\1ckpt blnk\2', value)
+        super().set_bios(selector, value)
+
+    def button_request(self, button: LcdButton, request: str = '\n') -> str:
+        """
+        Prepare F-16C Viper specific DCS-BIOS request for button pressed.
+
+        For G13/G15/G510: 1-4
+        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
+
+        :param button: LcdButton Enum
+        :param request: valid DCS-BIOS command as string
+        :return: ready to send DCS-BIOS request
+        """
+        button_map = {LcdButton.ONE: 'IFF_MASTER_KNB',
+                      LcdButton.TWO: 'IFF_ENABLE_SW',
+                      LcdButton.THREE: 'IFF_M4_CODE_SW',
+                      LcdButton.FOUR: 'IFF_M4_REPLY_SW',
+                      LcdButton.LEFT: 'IFF_MASTER_KNB',
+                      LcdButton.RIGHT: 'IFF_ENABLE_SW',
+                      LcdButton.DOWN: 'IFF_M4_CODE_SW',
+                      LcdButton.UP: 'IFF_M4_REPLY_SW'}
+        settings = 0
+        button_bios_name = ''
+        if button in button_map:
+            button_bios_name = button_map[button]
+            settings = self.get_next_value_for_button(button_bios_name)
+        action = {LcdButton.ONE: f'{button_bios_name} {settings}\n',
+                  LcdButton.TWO: f'{button_bios_name} {settings}\n',
+                  LcdButton.THREE: f'{button_bios_name} {settings}\n',
+                  LcdButton.FOUR: f'{button_bios_name} {settings}\n',
+                  LcdButton.LEFT: f'{button_bios_name} {settings}\n',
+                  LcdButton.RIGHT: f'{button_bios_name} {settings}\n',
+                  LcdButton.DOWN: f'{button_bios_name} {settings}\n',
+                  LcdButton.UP: f'{button_bios_name} {settings}\n'}
+        return super().button_request(button, action.get(button, '\n'))
+
+
+class Ka50(Aircraft):
+    """Ka-50 Black Shark."""
+    def __init__(self, lcd_type: LcdInfo) -> None:
+        """
+        Create Ka-50 Black Shark.
+
+        :param lcd_type: LCD type
+        """
+        super().__init__(lcd_type)
+        self.bios_data: Dict[str, BiosValue] = {
+            'PVI_LINE1_APOSTROPHE1': {'klass': 'StringBuffer', 'args': {'address': 0x1934, 'max_length': 1}, 'value': ''},
+            'PVI_LINE1_APOSTROPHE2': {'klass': 'StringBuffer', 'args': {'address': 0x1936, 'max_length': 1}, 'value': ''},
+            'PVI_LINE1_POINT': {'klass': 'StringBuffer', 'args': {'address': 0x1930, 'max_length': 1}, 'value': ''},
+            'PVI_LINE1_SIGN': {'klass': 'StringBuffer', 'args': {'address': 0x1920, 'max_length': 1}, 'value': ''},
+            'PVI_LINE1_TEXT': {'klass': 'StringBuffer', 'args': {'address': 0x1924, 'max_length': 6}, 'value': ''},
+            'PVI_LINE2_APOSTROPHE1': {'klass': 'StringBuffer', 'args': {'address': 0x1938, 'max_length': 1}, 'value': ''},
+            'PVI_LINE2_APOSTROPHE2': {'klass': 'StringBuffer', 'args': {'address': 0x193a, 'max_length': 1}, 'value': ''},
+            'PVI_LINE2_POINT': {'klass': 'StringBuffer', 'args': {'address': 0x1932, 'max_length': 1}, 'value': ''},
+            'PVI_LINE2_SIGN': {'klass': 'StringBuffer', 'args': {'address': 0x1922, 'max_length': 1}, 'value': ''},
+            'PVI_LINE2_TEXT': {'klass': 'StringBuffer', 'args': {'address': 0x192a, 'max_length': 6}, 'value': ''},
+            'AP_ALT_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x8000, 'shift_by': 0xf}, 'value': int()},
+            'AP_BANK_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x200, 'shift_by': 0x9}, 'value': int()},
+            'AP_FD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1938, 'mask': 0x200, 'shift_by': 0x9}, 'value': int()},
+            'AP_HDG_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x800, 'shift_by': 0xb}, 'value': int()},
+            'AP_PITCH_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x2000, 'shift_by': 0xd}, 'value': int()}}
+
+    def _draw_common_data(self, draw: ImageDraw, scale: int) -> None:
+        """
+        Draw common part (based on scale) for Mono and Color LCD.
+
+        :param draw: ImageDraw instance
+        :param scale: scaling factor (Mono 1, Color 2)
+        """
+        for rect_xy in [
+            (0 * scale, 1 * scale, 85 * scale, 18 * scale),
+            (0 * scale, 22 * scale, 85 * scale, 39 * scale),
+            (88 * scale, 1 * scale, 103 * scale, 18 * scale),
+            (88 * scale, 22 * scale, 103 * scale, 39 * scale),
+        ]:
+            draw.rectangle(xy=rect_xy, fill=self.lcd.background, outline=self.lcd.foreground)
+        line1, line2 = self._generate_pvi_lines()
+        draw.text(xy=(2 * scale, 3 * scale), text=line1, fill=self.lcd.foreground, font=self.lcd.font_l)
+        draw.text(xy=(2 * scale, 24 * scale), text=line2, fill=self.lcd.foreground, font=self.lcd.font_l)
+        self._auto_pilot_switch(draw, scale)
+
+    def _generate_pvi_lines(self) -> Sequence[str]:
+        """
+        Generate coordinate strings.
+
+        :return: tuple of string
+        """
+        text1, text2 = '', ''
+        line1_text = str(self.get_bios('PVI_LINE1_TEXT'))
+        line2_text = str(self.get_bios('PVI_LINE2_TEXT'))
+        if line1_text:
+            l1_apostr1 = self.get_bios("PVI_LINE1_APOSTROPHE1")
+            l1_apostr2 = self.get_bios("PVI_LINE1_APOSTROPHE2")
+            text1 = f'{line1_text[-6:-3]}{l1_apostr1}{line1_text[-3:-1]}{l1_apostr2}{line1_text[-1]}'
+        if line2_text:
+            l2_apostr1 = self.get_bios("PVI_LINE2_APOSTROPHE1")
+            l2_apostr2 = self.get_bios("PVI_LINE2_APOSTROPHE2")
+            text2 = f'{line2_text[-6:-3]}{l2_apostr1}{line2_text[-3:-1]}{l2_apostr2}{line2_text[-1]}'
+        line1 = f'{self.get_bios("PVI_LINE1_SIGN")}{text1} {self.get_bios("PVI_LINE1_POINT")}'
+        line2 = f'{self.get_bios("PVI_LINE2_SIGN")}{text2} {self.get_bios("PVI_LINE2_POINT")}'
+        return line1, line2
+
+    def _auto_pilot_switch(self, draw_obj: ImageDraw, scale: int) -> None:
+        """
+        Draw rectangle and add text for autopilot channels in correct coordinates.
+
+        :param draw_obj: ImageDraw object form PIL
+        :param scale: scaling factor (Mono 1, Color 2)
+        """
+        for c_rect, c_text, ap_channel, turn_on in (
+                ((111 * scale, 1 * scale, 124 * scale, 18 * scale), (113 * scale, 3 * scale), 'B', self.get_bios('AP_BANK_HOLD_LED')),
+                ((128 * scale, 1 * scale, 141 * scale, 18 * scale), (130 * scale, 3 * scale), 'P', self.get_bios('AP_PITCH_HOLD_LED')),
+                ((145 * scale, 1 * scale, 158 * scale, 18 * scale), (147 * scale, 3 * scale), 'F', self.get_bios('AP_FD_LED')),
+                ((111 * scale, 22 * scale, 124 * scale, 39 * scale), (113 * scale, 24 * scale), 'H', self.get_bios('AP_HDG_HOLD_LED')),
+                ((128 * scale, 22 * scale, 141 * scale, 39 * scale), (130 * scale, 24 * scale), 'A', self.get_bios('AP_ALT_HOLD_LED')),
+        ):
+            draw_autopilot_channels(self.lcd, ap_channel, c_rect, c_text, draw_obj, turn_on)
+
+    def draw_for_lcd_mono(self, img: Image.Image) -> None:
+        """Prepare image for Ka-50 Black Shark for Mono LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
+
+    def draw_for_lcd_color(self, img: Image.Image) -> None:
+        """Prepare image for Ka-50 Black Shark for Mono LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
+
+    def button_request(self, button: LcdButton, request: str = '\n') -> str:
+        """
+        Prepare Ka-50 Black Shark specific DCS-BIOS request for button pressed.
+
+        For G13/G15/G510: 1-4
+        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
+
+        :param button: LcdButton Enum
+        :param request: valid DCS-BIOS command as string
+        :return: ready to send DCS-BIOS request
+        """
+        action = {LcdButton.ONE: 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n',
+                  LcdButton.TWO: 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n',
+                  LcdButton.THREE: 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n',
+                  LcdButton.FOUR: 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n',
+                  LcdButton.LEFT: 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n',
+                  LcdButton.RIGHT: 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n',
+                  LcdButton.DOWN: 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n',
+                  LcdButton.UP: 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'}
+        return super().button_request(button, action.get(button, '\n'))
+
+
+class Ka503(Ka50):
+    """Ka-50 Black Shark III."""
+    pass
+
+
+class Mi8MT(Aircraft):
+    """Mi-8MTV2 Magnificent Eight."""
+
+    def __init__(self, lcd_type: LcdInfo) -> None:
+        """
+        Create Mi-8MTV2 Magnificent Eight.
+
+        :param lcd_type: LCD type
+        """
+        super().__init__(lcd_type)
+        self.bios_data: Dict[str, BiosValue] = {
+            'LMP_AP_HDG_ON': {'klass': 'IntegerBuffer', 'args': {'address': 0x269e, 'mask': 0x20, 'shift_by': 0x5}, 'value': int()},
+            'LMP_AP_PITCH_ROLL_ON': {'klass': 'IntegerBuffer', 'args': {'address': 0x269e, 'mask': 0x80, 'shift_by': 0x7}, 'value': int()},
+            'LMP_AP_HEIGHT_ON': {'klass': 'IntegerBuffer', 'args': {'address': 0x269e, 'mask': 0x100, 'shift_by': 0x8}, 'value': int()},
+            'R863_CNL_SEL': {'klass': 'IntegerBuffer', 'args': {'address': 0x268c, 'mask': 0x1f, 'shift_by': 0x0}, 'value': int()},
+            'R863_MOD': {'klass': 'IntegerBuffer', 'args': {'address': 0x263a, 'mask': 0x1000, 'shift_by': 0xc}, 'value': int()},
+            'R863_FREQ': {'klass': 'StringBuffer', 'args': {'address': 0x2804, 'max_length': 7}, 'value': ''},
+            'R828_PRST_CHAN_SEL': {'klass': 'IntegerBuffer', 'args': {'address': 0x268e, 'mask': 0x780, 'shift_by': 0x7}, 'value': int()},
+            'YADRO1A_FREQ': {'klass': 'StringBuffer', 'args': {'address': 0x2692, 'max_length': 7}, 'value': ''},
+        }
+
+    def _draw_common_data(self, draw: ImageDraw, scale: int) -> None:
+        """
+        Draw common part (based on scale) for Mono and Color LCD.
+
+        :param draw: ImageDraw instance
+        :param scale: scaling factor (Mono 1, Color 2)
+        """
+        for c_rect, c_text, ap_channel, turn_on in (
+                ((111 * scale, 1 * scale, 124 * scale, 18 * scale), (113 * scale, 3 * scale), 'H', self.get_bios('LMP_AP_HDG_ON')),
+                ((128 * scale, 1 * scale, 141 * scale, 18 * scale), (130 * scale, 3 * scale), 'P', self.get_bios('LMP_AP_PITCH_ROLL_ON')),
+                ((145 * scale, 1 * scale, 158 * scale, 18 * scale), (147 * scale, 3 * scale), 'A', self.get_bios('LMP_AP_HEIGHT_ON'))):
+            draw_autopilot_channels(self.lcd, ap_channel, c_rect, c_text, draw, turn_on)
+
+        r863, r828, yadro = self._generate_radio_values()
+        for i, line in enumerate([f'R828 {r828}', f'YADRO1 {yadro}', f'R863 {r863}'], 1):
+            offset = i * 10 * scale
+            draw.text(xy=(0, offset), text=line, fill=self.lcd.foreground, font=self.lcd.font_s)
+
+    def draw_for_lcd_mono(self, img: Image.Image) -> None:
+        """Prepare image for Mi-8MTV2 Magnificent Eight for Mono LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
+
+    def draw_for_lcd_color(self, img: Image.Image) -> None:
+        """Prepare image for Mi-8MTV2 Magnificent Eight for Color LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
+
+    def _generate_radio_values(self) -> Sequence[str]:
+        """
+        Generate string data about Hip R863, R828, YADRO1A radios settings.
+
+        :return: All 3 radios settings as strings
+        """
+        r863_mod = 'FM' if int(self.get_bios("R863_MOD")) else 'AM'
+        try:
+            r863_freq = float(self.get_bios("R863_FREQ"))
+        except ValueError:
+            r863_freq = 0.0
+        try:
+            yadro_freq = float(self.get_bios("YADRO1A_FREQ"))
+        except ValueError:
+            yadro_freq = 0.0
+        r863 = f'Ch:{int(self.get_bios("R863_CNL_SEL")) + 1:>2} {r863_mod} {r863_freq:.3f}'
+        r828 = f'Ch:{int(self.get_bios("R828_PRST_CHAN_SEL")) + 1:>2}'
+        yadro = f'{yadro_freq:>7.1f}'
+        return r863, r828, yadro
+
+
+class Mi24P(Aircraft):
+    """Mi-24P Hind."""
+    def __init__(self, lcd_type: LcdInfo) -> None:
+        """
+        Create Mi-24P Hind.
+
+        :param lcd_type: LCD type
+        """
+        super().__init__(lcd_type)
+        self.bios_data: Dict[str, BiosValue] = {
+            'PLT_R863_CHAN': {'klass': 'IntegerBuffer', 'args': {'address': 0x69ec, 'mask': 0x3e0, 'shift_by': 0x5}, 'value': int()},
+            'PLT_R863_MODUL': {'klass': 'IntegerBuffer', 'args': {'address': 0x69ec, 'mask': 0x2, 'shift_by': 0x1}, 'value': int()},
+            'PLT_R828_CHAN': {'klass': 'IntegerBuffer', 'args': {'address': 0x69fe, 'mask': 0xf00, 'shift_by': 0x8}, 'value': int()},
+            'JADRO_FREQ': {'klass': 'StringBuffer', 'args': {'address': 0x6a04, 'max_length': 7}, 'value': ''},
+            'PLT_SAU_HOVER_MODE_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x8000, 'shift_by': 0xf}, 'value': int()},
+            'PLT_SAU_ROUTE_MODE_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x2000, 'shift_by': 0xd}, 'value': int()},
+            'PLT_SAU_ALT_MODE_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x6902, 'mask': 0x100, 'shift_by': 0x8}, 'value': int()},
+            'PLT_SAU_H_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x80, 'shift_by': 0x7}, 'value': int()},
+            'PLT_SAU_K_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x20, 'shift_by': 0x5}, 'value': int()},
+            'PLT_SAU_T_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x800, 'shift_by': 0xb}, 'value': int()},
+            'PLT_SAU_B_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x200, 'shift_by': 0x9}, 'value': int()},
+        }
+
+    def _draw_common_data(self, draw: ImageDraw, scale: int) -> None:
+        """
+        Draw common part (based on scale) for Mono and Color LCD.
+
+        :param draw: ImageDraw instance
+        :param scale: scaling factor (Mono 1, Color 2)
+        """
+        for c_rect, c_text, ap_channel, turn_on in (
+                ((111 * scale, 1 * scale, 124 * scale, 18 * scale), (113 * scale, 3 * scale), 'H', self.get_bios('PLT_SAU_HOVER_MODE_ON_L')),
+                ((128 * scale, 1 * scale, 141 * scale, 18 * scale), (130 * scale, 3 * scale), 'R', self.get_bios('PLT_SAU_ROUTE_MODE_ON_L')),
+                ((145 * scale, 1 * scale, 158 * scale, 18 * scale), (147 * scale, 3 * scale), 'A', self.get_bios('PLT_SAU_ALT_MODE_ON_L')),
+                ((94 * scale, 22 * scale, 107 * scale, 39 * scale), (96 * scale, 24 * scale), 'Y', self.get_bios('PLT_SAU_H_ON_L')),
+                ((111 * scale, 22 * scale, 124 * scale, 39 * scale), (113 * scale, 24 * scale), 'R', self.get_bios('PLT_SAU_K_ON_L')),
+                ((128 * scale, 22 * scale, 141 * scale, 39 * scale), (130 * scale, 24 * scale), 'P', self.get_bios('PLT_SAU_T_ON_L')),
+                ((145 * scale, 22 * scale, 158 * scale, 39 * scale), (147 * scale, 24 * scale), 'A', self.get_bios('PLT_SAU_B_ON_L')),
+        ):
+            draw_autopilot_channels(self.lcd, ap_channel, c_rect, c_text, draw, turn_on)
+
+        r863, r828, yadro = self._generate_radio_values()
+        for i, line in enumerate([f'R828 {r828}', f'R863 {r863}', f'YADRO1 {yadro}'], 1):
+            offset = i * 10 * scale
+            draw.text(xy=(0, offset), text=line, fill=self.lcd.foreground, font=self.lcd.font_s)
+
+    def draw_for_lcd_mono(self, img: Image.Image) -> None:
+        """Prepare image for Mi-24P Hind for Mono LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
+
+    def draw_for_lcd_color(self, img: Image.Image) -> None:
+        """Prepare image for Mi-24P Hind for Color LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
+
+    def _generate_radio_values(self) -> Sequence[str]:
+        """
+        Generate string data about Hind R863, R828, YADRO1I radios settings.
+
+        :return: All 3 radios settings as strings
+        """
+        r863_mod = 'FM' if int(self.get_bios("PLT_R863_MODUL")) else 'AM'
+        try:
+            yadro_freq = float(self.get_bios("JADRO_FREQ"))
+        except ValueError:
+            yadro_freq = 0.0
+        r863 = f'Ch:{int(self.get_bios("PLT_R863_CHAN")) + 1:>2} {r863_mod}'
+        r828 = f'Ch:{int(self.get_bios("PLT_R828_CHAN")) + 1:>2}'
+        yadro = f'{yadro_freq:>7.1f}'
+        return r863, r828, yadro
+
+
+class ApacheEufdMode(Enum):
+    """Apache EUFD Mode."""
+    IDM = 1
+    WCA = 2
+    PRE = 4
+
+
+class AH64DBLKII(Aircraft):
+    """AH-64D Apache."""
+    def __init__(self, lcd_type: LcdInfo) -> None:
+        """
+        Create AH-64D Apache.
+
+        :param lcd_type: LCD type
+        """
+        super().__init__(lcd_type)
+        self.mode = ApacheEufdMode.IDM
+        self.warning_line = 1
+        self.bios_data: Dict[str, BiosValue] = {
+            'PLT_EUFD_LINE1': {'klass': 'StringBuffer', 'args': {'address': 0x80c2, 'max_length': 56}, 'value': ''},
+            'PLT_EUFD_LINE2': {'klass': 'StringBuffer', 'args': {'address': 0x80fa, 'max_length': 56}, 'value': ''},
+            'PLT_EUFD_LINE3': {'klass': 'StringBuffer', 'args': {'address': 0x8132, 'max_length': 56}, 'value': ''},
+            'PLT_EUFD_LINE4': {'klass': 'StringBuffer', 'args': {'address': 0x816a, 'max_length': 56}, 'value': ''},
+            'PLT_EUFD_LINE5': {'klass': 'StringBuffer', 'args': {'address': 0x81a2, 'max_length': 56}, 'value': ''},
+            'PLT_EUFD_LINE6': {'klass': 'StringBuffer', 'args': {'address': 0x81da, 'max_length': 56}, 'value': ''},
+            'PLT_EUFD_LINE7': {'klass': 'StringBuffer', 'args': {'address': 0x8212, 'max_length': 56}, 'value': ''},
+            'PLT_EUFD_LINE8': {'klass': 'StringBuffer', 'args': {'address': 0x824a, 'max_length': 56}, 'value': ''},
+            'PLT_EUFD_LINE9': {'klass': 'StringBuffer', 'args': {'address': 0x8282, 'max_length': 56}, 'value': ''},
+            'PLT_EUFD_LINE10': {'klass': 'StringBuffer', 'args': {'address': 0x82ba, 'max_length': 56}, 'value': ''},
+            'PLT_EUFD_LINE11': {'klass': 'StringBuffer', 'args': {'address': 0x82f2, 'max_length': 56}, 'value': ''},
+            'PLT_EUFD_LINE12': {'klass': 'StringBuffer', 'args': {'address': 0x832a, 'max_length': 56}, 'value': ''},
+        }
+
+    def draw_for_lcd_mono(self, img: Image.Image) -> None:
+        """Prepare image for AH-64D Apache for Mono LCD."""
+        LOG.debug(f'Mode: {self.mode}')
+        kwargs = {'draw': ImageDraw.Draw(img), 'scale': 1}
+        mode = self.mode.name.lower()
+        if mode == 'pre':
+            kwargs['xcords'] = [0] * 5 + [80] * 5
+            kwargs['ycords'] = [j * 8 for j in range(0, 5)] * 2
+            kwargs['font'] = self.lcd.font_xs
+            del kwargs['scale']
+        getattr(self, f'_draw_for_{mode}')(**kwargs)
+
+    def draw_for_lcd_color(self, img: Image.Image) -> None:
+        """Prepare image for AH-64D Apache for Color LCD."""
+        LOG.debug(f'Mode: {self.mode}')
+        kwargs = {'draw': ImageDraw.Draw(img), 'scale': 2}
+        mode = self.mode.name.lower()
+        if mode == 'pre':
+            kwargs['xcords'] = [0] * 10
+            kwargs['ycords'] = [j * 24 for j in range(0, 10)]
+            kwargs['font'] = self.lcd.font_l
+            del kwargs['scale']
+        getattr(self, f'_draw_for_{mode}')(**kwargs)
+
+    def _draw_for_idm(self, draw: ImageDraw.Draw, scale: int):
+        """
+        Draw image for IDM mode.
+
+        :param draw: ImageDraw instance
+        :param scale: scaling factor (Mono 1, Color 2)
+        """
+        for i in range(8, 13):
+            offset = (i - 8) * 8 * scale
+            mat = search(r'(.*\*)\s+(\d+)([.\dULCA]+)[-\sA-Z]*(\d+)([.\dULCA]+)[\s-]+', str(self.get_bios(f'PLT_EUFD_LINE{i}')))
+            if mat:
+                spacer = ' ' * (6 - len(mat.group(3)))
+                text = f'{mat.group(1):>7}{mat.group(2):>4}{mat.group(3):5<}{spacer}{mat.group(4):>4}{mat.group(5):5<}'
+                draw.text(xy=(0, offset), text=text, fill=self.lcd.foreground, font=self.lcd.font_xs)
+
+    def _draw_for_wca(self, draw: ImageDraw.Draw, scale: int):
+        """
+        Draw image for WCA mode.
+
+        :param draw: ImageDraw instance
+        :param scale: scaling factor (Mono 1, Color 2)
+        """
+        warnings = self._fetch_warning_list()
+        LOG.debug(f'Warnings: {warnings}')
+        try:
+            for idx, warn_no in enumerate(range(self.warning_line - 1, self.warning_line + 4)):
+                line = idx * 8 * scale
+                draw.text(xy=(0, line), text=f'{idx + self.warning_line:2} {warnings[warn_no]}', fill=self.lcd.foreground, font=self.lcd.font_s)
+                if self.warning_line >= len(warnings) - 3:
+                    self.warning_line = 1
+        except IndexError:
+            self.warning_line = 1
+
+    def _fetch_warning_list(self) -> List[str]:
+        """
+        Fetch all warnings and return as list.
+
+        :return: list of warnings (as strings)
+        """
+        warn = []
+        for i in range(1, 8):
+            mat = search(r'(.*)\|(.*)\|(.*)', str(self.get_bios(f'PLT_EUFD_LINE{i}')))
+            if mat:
+                warn.extend([w for w in [mat.group(1).strip(), mat.group(2).strip(), mat.group(3).strip()] if w])
+        return warn
+
+    def _draw_for_pre(self, draw: ImageDraw.Draw, xcords: List[int], ycords: List[int], font: ImageFont.FreeTypeFont):
+        """
+        Draw image for PRE mode.
+
+        :param draw: ImageDraw instance
+        :param xcords: list of X coordinates
+        :param ycords: list of Y coordinates
+        :param font: font instance
+        """
+        match_dict = {2: r'.*\|.*\|([\u2192\s]CO CMD)\s*([\d\.]*)\s+',
+                      3: r'.*\|.*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
+                      4: r'.*\|.*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
+                      5: r'.*\|.*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
+                      6: r'\s*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
+                      7: r'\s*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
+                      8: r'\s*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
+                      9: r'\s*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
+                      10: r'\s*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+',
+                      11: r'\s*\|([\u2192\s][A-Z\d\/]*)\s*([\d\.]*)\s+'}
+        for i, xcord, ycord in zip(range(2, 12), xcords, ycords):
+            mat = search(match_dict[i], str(self.get_bios(f'PLT_EUFD_LINE{i}')))
+            if mat:
+                draw.text(xy=(xcord, ycord), text=f'{mat.group(1):<9}{mat.group(2):>7}',
+                          fill=self.lcd.foreground, font=font)
+
+    def set_bios(self, selector: str, value: Union[str, int]) -> None:
+        """
+        Set new data.
+
+        :param selector:
+        :param value:
+        """
+        if selector == 'PLT_EUFD_LINE1':
+            match = search(r'.*\|.*\|(PRESET TUNE)\s\w+', str(value))
+            self.mode = ApacheEufdMode.IDM
+            if match:
+                self.mode = ApacheEufdMode.PRE
+        if selector in ('PLT_EUFD_LINE8', 'PLT_EUFD_LINE9', 'PLT_EUFD_LINE10', 'PLT_EUFD_LINE11', 'PLT_EUFD_LINE12'):
+            LOG.debug(f'{self.__class__.__name__} {selector} original: "{value}"')
+            value = str(value).replace(']', '\u2666').replace('[', '\u25ca').replace('~', '\u25a0'). \
+                replace('>', '\u25b8').replace('<', '\u25c2').replace('=', '\u2219')
+        if 'PLT_EUFD_LINE' in selector:
+            LOG.debug(f'{self.__class__.__name__} {selector} original: "{value}"')
+            value = str(value).replace('!', '\u2192')  # replace ! with ->
+        super().set_bios(selector, value)
+
+    def button_request(self, button: LcdButton, request: str = '\n') -> str:
+        """
+        Prepare AH-64D Apache specific DCS-BIOS request for button pressed.
+
+        For G13/G15/G510: 1-4
+        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
+
+        :param button: LcdButton Enum
+        :param request: valid DCS-BIOS command as string
+        :return: ready to send DCS-BIOS request
+        """
+        wca_or_idm = 'PLT_EUFD_WCA 0\nPLT_EUFD_WCA 1\n'
+        if self.mode == ApacheEufdMode.IDM:
+            wca_or_idm = 'PLT_EUFD_IDM 0\nPLT_EUFD_IDM 1\n'
+
+        if button in (LcdButton.FOUR, LcdButton.UP) and self.mode == ApacheEufdMode.IDM:
+            self.mode = ApacheEufdMode.WCA
+        elif button in (LcdButton.FOUR, LcdButton.UP) and self.mode != ApacheEufdMode.IDM:
+            self.mode = ApacheEufdMode.IDM
+
+        if button in (LcdButton.ONE, LcdButton.LEFT) and self.mode == ApacheEufdMode.WCA:
+            self.warning_line += 1
+
+        action = {LcdButton.ONE: wca_or_idm,
+                  LcdButton.TWO: 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n',
+                  LcdButton.THREE: 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n',
+                  LcdButton.FOUR: 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n',
+                  LcdButton.LEFT: wca_or_idm,
+                  LcdButton.RIGHT: 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n',
+                  LcdButton.DOWN: 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n',
+                  LcdButton.UP: 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n'}
+        return super().button_request(button, action.get(button, '\n'))
+
+
+class A10C(Aircraft):
+    """A-10C Warthog."""
+    def __init__(self, lcd_type: LcdInfo) -> None:
+        """
+        Create A-10C Warthog or A-10C II Tank Killer.
+
+        :param lcd_type: LCD type
+        """
+        super().__init__(lcd_type)
+        self.bios_data: Dict[str, BiosValue] = {
+            'VHFAM_FREQ1': {'klass': 'StringBuffer', 'args': {'address': 0x1190, 'max_length': 2}, 'value': ''},
+            'VHFAM_FREQ2': {'klass': 'IntegerBuffer', 'args': {'address': 0x118e, 'mask': 0xf0, 'shift_by': 0x4}, 'value': int()},
+            'VHFAM_FREQ3': {'klass': 'IntegerBuffer', 'args': {'address': 0x118e, 'mask': 0xf00, 'shift_by': 0x8}, 'value': int()},
+            'VHFAM_FREQ4': {'klass': 'StringBuffer', 'args': {'address': 0x1192, 'max_length': 2}, 'value': ''},
+            'VHFFM_FREQ1': {'klass': 'StringBuffer', 'args': {'address': 0x119a, 'max_length': 2}, 'value': ''},
+            'VHFFM_FREQ2': {'klass': 'IntegerBuffer', 'args': {'address': 0x119c, 'mask': 0xf, 'shift_by': 0x0}, 'value': int()},
+            'VHFFM_FREQ3': {'klass': 'IntegerBuffer', 'args': {'address': 0x119c, 'mask': 0xf0, 'shift_by': 0x4}, 'value': int()},
+            'VHFFM_FREQ4': {'klass': 'StringBuffer', 'args': {'address': 0x119e, 'max_length': 2}, 'value': ''},
+            'UHF_100MHZ_SEL': {'klass': 'StringBuffer', 'args': {'address': 0x1178, 'max_length': 1}, 'value': ''},
+            'UHF_10MHZ_SEL': {'klass': 'IntegerBuffer', 'args': {'address': 0x1170, 'mask': 0x3c00, 'shift_by': 0xa}, 'value': int()},
+            'UHF_1MHZ_SEL': {'klass': 'IntegerBuffer', 'args': {'address': 0x1178, 'mask': 0xf00, 'shift_by': 0x8}, 'value': int()},
+            'UHF_POINT1MHZ_SEL': {'klass': 'IntegerBuffer', 'args': {'address': 0x1178, 'mask': 0xf000, 'shift_by': 0xc}, 'value': int()},
+            'UHF_POINT25_SEL': {'klass': 'StringBuffer', 'args': {'address': 0x117a, 'max_length': 2}, 'value': ''}}
+
+    def _generate_freq_values(self) -> Sequence[str]:
+        """
+        Generate frequency for all 3 radios (VHF AM, VHF FM and UHF).
+
+        :return: All 3 frequency settings as strings
+        """
+        vhfam = f'{self.get_bios("VHFAM_FREQ1")}{self.get_bios("VHFAM_FREQ2")}.' \
+                f'{self.get_bios("VHFAM_FREQ3")}{self.get_bios("VHFAM_FREQ4")}'
+        vhffm = f'{self.get_bios("VHFFM_FREQ1")}{self.get_bios("VHFFM_FREQ2")}.' \
+                f'{self.get_bios("VHFFM_FREQ3")}{self.get_bios("VHFFM_FREQ4")}'
+        uhf = f'{self.get_bios("UHF_100MHZ_SEL")}{self.get_bios("UHF_10MHZ_SEL")}{self.get_bios("UHF_1MHZ_SEL")}.' \
+              f'{self.get_bios("UHF_POINT1MHZ_SEL")}{self.get_bios("UHF_POINT25_SEL")}'
+        return uhf, vhfam, vhffm
+
+    def draw_for_lcd_mono(self, img: Image.Image) -> None:
+        """Prepare image for A-10C Warthog or A-10C II Tank Killer for Mono LCD."""
+        draw = ImageDraw.Draw(img)
+        uhf, vhfam, vhffm = self._generate_freq_values()
+        for i, line in enumerate(['      *** RADIOS ***', f'VHF AM: {vhfam} MHz',
+                                  f'VHF FM: {vhffm} MHz', f'   UHF: {uhf} MHz']):
+            offset = i * 10
+            draw.text(xy=(0, offset), text=line, fill=self.lcd.foreground, font=self.lcd.font_s)
+
+    def draw_for_lcd_color(self, img: Image.Image) -> None:
+        """Prepare image for A-10C Warthog or A-10C II Tank Killer for Color LCD."""
+        draw = ImageDraw.Draw(img)
+        uhf, vhfam, vhffm = self._generate_freq_values()
+        for i, line in enumerate(['      *** RADIOS ***', f'VHF AM: {vhfam} MHz',
+                                  f'VHF FM: {vhffm} MHz', f'   UHF: {uhf} MHz']):
+            offset = i * 20
+            draw.text(xy=(0, offset), text=line, fill=self.lcd.foreground, font=self.lcd.font_s)
+
+
+class A10C2(A10C):
+    """A-10C II Tank Killer."""
+    pass
+
+
+class F14B(Aircraft):
+    """F-14B Tomcat."""
+    def __init__(self, lcd_type: LcdInfo) -> None:
+        """
+        Create F-14B Tomcat.
+
+        :param lcd_type: LCD type
+        """
+        super().__init__(lcd_type)
+        self.bios_data: Dict[str, BiosValue] = {
+            'RIO_CAP_CLEAR': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x4000, 'shift_by': 0xe}, 'value': int()},
+            'RIO_CAP_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x2000, 'shift_by': 0xd}, 'value': int()},
+            'RIO_CAP_NE': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x1000, 'shift_by': 0xc}, 'value': int()},
+            'RIO_CAP_ENTER': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x8000, 'shift_by': 0xf}, 'value': int()}}
+
+    def _draw_common_data(self, draw: ImageDraw) -> None:
+        """
+        Draw common part for Mono and Color LCD.
+
+        :param draw: ImageDraw instance
+        """
+        draw.text(xy=(2, 3), text=f'{SUPPORTED_CRAFTS[self.__class__.__name__]["name"]}', fill=self.lcd.foreground, font=self.lcd.font_l)
+
+    def draw_for_lcd_mono(self, img: Image.Image) -> None:
+        """Prepare image for F-14B Tomcat for Mono LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img))
+
+    def draw_for_lcd_color(self, img: Image.Image) -> None:
+        """Prepare image for F-14B Tomcat for Color LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img))
+
+    def button_request(self, button: LcdButton, request: str = '\n') -> str:
+        """
+        Prepare F-14B Tomcat specific DCS-BIOS request for button pressed.
+
+        For G13/G15/G510: 1-4
+        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
+
+        :param button: LcdButton Enum
+        :param request: valid DCS-BIOS command as string
+        :return: ready to send DCS-BIOS request
+        """
+        action = {LcdButton.ONE: 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n',
+                  LcdButton.TWO: 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n',
+                  LcdButton.THREE: 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n',
+                  LcdButton.FOUR: 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n',
+                  LcdButton.LEFT: 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n',
+                  LcdButton.RIGHT: 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n',
+                  LcdButton.DOWN: 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n',
+                  LcdButton.UP: 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'}
+        return super().button_request(button, action.get(button, '\n'))
+
+
+class F14A135GR(F14B):
+    """F-14A-135-GR Tomcat."""
+    pass
+
+
+class AV8BNA(Aircraft):
+    """AV-8B Night Attack."""
+    def __init__(self, lcd_type: LcdInfo) -> None:
+        """
+        Create AV-8B Night Attack.
+
+        :param lcd_type: LCD type
+        """
+        super().__init__(lcd_type)
+        self.bios_data: Dict[str, BiosValue] = {
+            'UFC_SCRATCHPAD': {'klass': 'StringBuffer', 'args': {'address': 0x7984, 'max_length': 12}, 'value': ''},
+            'UFC_COMM1_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x7954, 'max_length': 2}, 'value': ''},
+            'UFC_COMM2_DISPLAY': {'klass': 'StringBuffer', 'args': {'address': 0x7956, 'max_length': 2}, 'value': ''},
+            'AV8BNA_ODU_1_SELECT': {'klass': 'StringBuffer', 'args': {'address': 0x7966, 'max_length': 1}, 'value': ''},
+            'AV8BNA_ODU_1_Text': {'klass': 'StringBuffer', 'args': {'address': 0x7968, 'max_length': 4}, 'value': ''},
+            'AV8BNA_ODU_2_SELECT': {'klass': 'StringBuffer', 'args': {'address': 0x796c, 'max_length': 1}, 'value': ''},
+            'AV8BNA_ODU_2_Text': {'klass': 'StringBuffer', 'args': {'address': 0x796e, 'max_length': 4}, 'value': ''},
+            'AV8BNA_ODU_3_SELECT': {'klass': 'StringBuffer', 'args': {'address': 0x7972, 'max_length': 1}, 'value': ''},
+            'AV8BNA_ODU_3_Text': {'klass': 'StringBuffer', 'args': {'address': 0x7974, 'max_length': 4}, 'value': ''},
+            'AV8BNA_ODU_4_SELECT': {'klass': 'StringBuffer', 'args': {'address': 0x7978, 'max_length': 1}, 'value': ''},
+            'AV8BNA_ODU_4_Text': {'klass': 'StringBuffer', 'args': {'address': 0x797a, 'max_length': 4}, 'value': ''},
+            'AV8BNA_ODU_5_SELECT': {'klass': 'StringBuffer', 'args': {'address': 0x797e, 'max_length': 1}, 'value': ''},
+            'AV8BNA_ODU_5_Text': {'klass': 'StringBuffer', 'args': {'address': 0x7980, 'max_length': 4}, 'value': ''}}
+
+    def _draw_common_data(self, draw: ImageDraw, scale: int) -> ImageDraw:
+        """
+        Draw common part (based on scale) for Mono and Color LCD.
+
+        :param draw: ImageDraw instance
+        :param scale: scaling factor (Mono 1, Color 2)
+        :return: updated image to draw
+        """
+        draw.text(xy=(50 * scale, 0), fill=self.lcd.foreground, font=self.lcd.font_l, text=f'{self.get_bios("UFC_SCRATCHPAD")}')
+        draw.line(xy=(50 * scale, 20 * scale, 160 * scale, 20 * scale), fill=self.lcd.foreground, width=1)
+
+        draw.rectangle(xy=(50 * scale, 29 * scale, 70 * scale, 42 * scale), fill=self.lcd.background, outline=self.lcd.foreground)
+        draw.text(xy=(52 * scale, 29 * scale), text=self.get_bios('UFC_COMM1_DISPLAY'), fill=self.lcd.foreground, font=self.lcd.font_l)
+
+        draw.rectangle(xy=(139 * scale, 29 * scale, 159 * scale, 42 * scale), fill=self.lcd.background, outline=self.lcd.foreground)
+        draw.text(xy=(140 * scale, 29 * scale), text=self.get_bios('UFC_COMM2_DISPLAY'), fill=self.lcd.foreground, font=self.lcd.font_l)
+
+        for i in range(1, 6):
+            offset = (i - 1) * 8 * scale
+            draw.text(xy=(0 * scale, offset), fill=self.lcd.foreground, font=self.lcd.font_s,
+                      text=f'{i}{self.get_bios(f"AV8BNA_ODU_{i}_SELECT")}{self.get_bios(f"AV8BNA_ODU_{i}_Text")}')
+        return draw
+
+    def draw_for_lcd_mono(self, img: Image.Image) -> None:
+        """Prepare image for AV-8B N/A for Mono LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
+
+    def draw_for_lcd_color(self, img: Image.Image) -> None:
+        """Prepare image for AV-8B N/A for Color LCD."""
+        self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
+
+    def button_request(self, button: LcdButton, request: str = '\n') -> str:
+        """
+        Prepare AV-8B N/A specific DCS-BIOS request for button pressed.
+
+        For G13/G15/G510: 1-4
+        For G19 9-15: LEFT = 9, RIGHT = 10, OK = 11, CANCEL = 12, UP = 13, DOWN = 14, MENU = 15
+
+        :param button: LcdButton Enum
+        :param request: valid DCS-BIOS command as string
+        :return: ready to send DCS-BIOS request
+        """
+        action = {LcdButton.ONE: 'UFC_COM1_SEL -3200\n',
+                  LcdButton.TWO: 'UFC_COM1_SEL 3200\n',
+                  LcdButton.THREE: 'UFC_COM2_SEL -3200\n',
+                  LcdButton.FOUR: 'UFC_COM2_SEL 3200\n',
+                  LcdButton.LEFT: 'UFC_COM1_SEL -3200\n',
+                  LcdButton.RIGHT: 'UFC_COM1_SEL 3200\n',
+                  LcdButton.DOWN: 'UFC_COM2_SEL -3200\n',
+                  LcdButton.UP: 'UFC_COM2_SEL 3200\n'}
+        return super().button_request(button, action.get(button, '\n'))
+
+
+def draw_autopilot_channels(lcd: LcdInfo, ap_channel: str, c_rect: Sequence[int], c_text: Sequence[int], draw_obj: ImageDraw, turn_on: Union[str, int]) -> None:
+    """
+    Draw rectangles with background for autopilot channels.
+
+    :param lcd: instance of LCD
+    :param ap_channel: channel name
+    :param c_rect: coordinates for rectangle
+    :param c_text: coordinates for name
+    :param draw_obj: ImageDraw instance
+    :param turn_on: channel on/off, fill on/off
+    """
+    if turn_on:
+        draw_obj.rectangle(c_rect, fill=lcd.foreground, outline=lcd.foreground)
+        draw_obj.text(xy=c_text, text=ap_channel, fill=lcd.background, font=lcd.font_l)
+    else:
+        draw_obj.rectangle(xy=c_rect, fill=lcd.background, outline=lcd.foreground)
+        draw_obj.text(xy=c_text, text=ap_channel, fill=lcd.foreground, font=lcd.font_l)
```

### Comparing `dcspy-1.9.5/dcspy/dcsbios.py` & `dcspy-2.0.0/dcspy/dcsbios.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-from enum import Enum, auto
-from functools import partial
-from struct import pack
-from typing import Callable, Set
-
-
-class ParserState(Enum):
-    """Protocol parser states."""
-    ADDRESS_LOW = auto()
-    ADDRESS_HIGH = auto()
-    COUNT_LOW = auto()
-    COUNT_HIGH = auto()
-    DATA_LOW = auto()
-    DATA_HIGH = auto()
-    WAIT_FOR_SYNC = auto()
-
-
-class ProtocolParser:
-    """DCS_BIOS protocol parser."""
-    def __init__(self) -> None:
-        """Basic constructor."""
-        self.state = ParserState.WAIT_FOR_SYNC
-        self.sync_byte_count = 0
-        self.address = 0
-        self.count = 0
-        self.data = 0
-        self.write_callbacks: Set[Callable] = set()
-        self.frame_sync_callbacks: Set[Callable] = set()
-
-    def process_byte(self, int_byte: int) -> None:
-        """
-        State machine - processing of byte.
-
-        Allowed states are: ParserState
-        :param int_byte:
-        """
-        state_handling = getattr(self, f'_{self.state.name.lower()}')
-        if self.state == ParserState.WAIT_FOR_SYNC:
-            state_handling()
-        else:
-            state_handling(int_byte)
-
-        if int_byte == 0x55:
-            self.sync_byte_count += 1
-        else:
-            self.sync_byte_count = 0
-
-        self._wait_for_sync()
-
-    def _address_low(self, int_byte: int) -> None:
-        """
-        Handling of ADDRESS_LOW state.
-
-        :param int_byte: data to process
-        """
-        self.address = int_byte
-        self.state = ParserState.ADDRESS_HIGH
-
-    def _address_high(self, int_byte: int) -> None:
-        """
-        Handling of ADDRESS_HIGH state.
-
-        :param int_byte: data to process
-        """
-        self.address += int_byte * 256
-        if self.address != 0x5555:
-            self.state = ParserState.COUNT_LOW
-        else:
-            self.state = ParserState.WAIT_FOR_SYNC
-
-    def _count_low(self, int_byte: int) -> None:
-        """
-        Handling of COUNT_LOW state.
-
-        :param int_byte: data to process
-        """
-        self.count = int_byte
-        self.state = ParserState.COUNT_HIGH
-
-    def _count_high(self, int_byte: int) -> None:
-        """
-        Handling of COUNT_HIGH state.
-
-        :param int_byte: data to process
-        """
-        self.count += 256 * int_byte
-        self.state = ParserState.DATA_LOW
-
-    def _data_low(self, int_byte: int) -> None:
-        """
-        Handling of DATA_LOW state.
-
-        :param int_byte: data to process
-        """
-        self.data = int_byte
-        self.count -= 1
-        self.state = ParserState.DATA_HIGH
-
-    def _data_high(self, int_byte: int) -> None:
-        """
-        Handling of DATA_HIGH state.
-
-        :param int_byte: data to process
-        """
-        self.data += 256 * int_byte
-        self.count -= 1
-        for callback in self.write_callbacks:
-            callback(self.address, self.data)
-        self.address += 2
-        if self.count == 0:
-            self.state = ParserState.ADDRESS_LOW
-        else:
-            self.state = ParserState.DATA_LOW
-
-    def _wait_for_sync(self) -> None:
-        """Handling of WAIT_FOR_SYNC state."""
-        if self.sync_byte_count == 4:
-            self.state = ParserState.ADDRESS_LOW
-            self.sync_byte_count = 0
-            for callback in self.frame_sync_callbacks:
-                callback()
-
-
-class StringBuffer:
-    """String buffer for DCS-BIOS protocol."""
-    def __init__(self, parser: ProtocolParser, address: int, max_length: int, callback: Callable) -> None:
-        """
-        Basic constructor.
-
-        :param parser:
-        :param address:
-        :param max_length:
-        :param callback:
-        """
-        self.__address = address
-        self.__length = max_length
-        self.__dirty = False
-        self.buffer = bytearray(max_length)
-        self.callbacks: Set[Callable] = set()
-        self.callbacks.add(callback)
-        parser.write_callbacks.add(partial(self.on_dcsbios_write))
-
-    def set_char(self, index, char) -> None:
-        """
-        Set char.
-
-        :param index:
-        :param char:
-        """
-        if self.buffer[index] != char:
-            self.buffer[index] = char
-            self.__dirty = True
-
-    def on_dcsbios_write(self, address: int, data: int) -> None:
-        """
-        Callback function.
-
-        :param address:
-        :param data:
-        """
-        if self.__address <= address < self.__address + self.__length:
-            data_bytes = pack('<H', data)
-            self.set_char(address - self.__address, data_bytes[0])
-            if self.__address + self.__length > (address + 1):
-                self.set_char(address - self.__address + 1, data_bytes[1])
-
-        if address == 0xfffe and self.__dirty:
-            self.__dirty = False
-            str_buff = self.buffer.split(sep=b'\x00', maxsplit=1)[0].decode('latin-1')
-            for callback in self.callbacks:
-                callback(str_buff)
-
-
-class IntegerBuffer:
-    """Integer buffer for DCS-BIOS protocol."""
-    def __init__(self, parser: ProtocolParser, address: int, mask: int, shift_by: int, callback: Callable) -> None:
-        """
-        Basic constructor.
-
-        :param parser:
-        :param address:
-        :param mask:
-        :param shift_by:
-        :param callback:
-        """
-        self.__address = address
-        self.__mask = mask
-        self.__shift_by = shift_by
-        self.__value = int()
-        self.callbacks: Set[Callable] = set()
-        self.callbacks.add(callback)
-        parser.write_callbacks.add(partial(self.on_dcsbios_write))
-
-    def on_dcsbios_write(self, address: int, data: int) -> None:
-        """
-        Callback function.
-
-        :param address:
-        :param data:
-        """
-        if address == self.__address:
-            value = (data & self.__mask) >> self.__shift_by
-            if self.__value != value:
-                self.__value = value
-                for callback in self.callbacks:
-                    callback(value)
+from enum import Enum, auto
+from functools import partial
+from struct import pack
+from typing import Callable, Set
+
+
+class ParserState(Enum):
+    """Protocol parser states."""
+    ADDRESS_LOW = auto()
+    ADDRESS_HIGH = auto()
+    COUNT_LOW = auto()
+    COUNT_HIGH = auto()
+    DATA_LOW = auto()
+    DATA_HIGH = auto()
+    WAIT_FOR_SYNC = auto()
+
+
+class ProtocolParser:
+    """DCS_BIOS protocol parser."""
+    def __init__(self) -> None:
+        """Basic constructor."""
+        self.state = ParserState.WAIT_FOR_SYNC
+        self.sync_byte_count = 0
+        self.address = 0
+        self.count = 0
+        self.data = 0
+        self.write_callbacks: Set[Callable] = set()
+        self.frame_sync_callbacks: Set[Callable] = set()
+
+    def process_byte(self, int_byte: int) -> None:
+        """
+        State machine - processing of byte.
+
+        Allowed states are: ParserState
+        :param int_byte:
+        """
+        state_handling = getattr(self, f'_{self.state.name.lower()}')
+        if self.state == ParserState.WAIT_FOR_SYNC:
+            state_handling()
+        else:
+            state_handling(int_byte)
+
+        if int_byte == 0x55:
+            self.sync_byte_count += 1
+        else:
+            self.sync_byte_count = 0
+
+        self._wait_for_sync()
+
+    def _address_low(self, int_byte: int) -> None:
+        """
+        Handling of ADDRESS_LOW state.
+
+        :param int_byte: data to process
+        """
+        self.address = int_byte
+        self.state = ParserState.ADDRESS_HIGH
+
+    def _address_high(self, int_byte: int) -> None:
+        """
+        Handling of ADDRESS_HIGH state.
+
+        :param int_byte: data to process
+        """
+        self.address += int_byte * 256
+        if self.address != 0x5555:
+            self.state = ParserState.COUNT_LOW
+        else:
+            self.state = ParserState.WAIT_FOR_SYNC
+
+    def _count_low(self, int_byte: int) -> None:
+        """
+        Handling of COUNT_LOW state.
+
+        :param int_byte: data to process
+        """
+        self.count = int_byte
+        self.state = ParserState.COUNT_HIGH
+
+    def _count_high(self, int_byte: int) -> None:
+        """
+        Handling of COUNT_HIGH state.
+
+        :param int_byte: data to process
+        """
+        self.count += 256 * int_byte
+        self.state = ParserState.DATA_LOW
+
+    def _data_low(self, int_byte: int) -> None:
+        """
+        Handling of DATA_LOW state.
+
+        :param int_byte: data to process
+        """
+        self.data = int_byte
+        self.count -= 1
+        self.state = ParserState.DATA_HIGH
+
+    def _data_high(self, int_byte: int) -> None:
+        """
+        Handling of DATA_HIGH state.
+
+        :param int_byte: data to process
+        """
+        self.data += 256 * int_byte
+        self.count -= 1
+        for callback in self.write_callbacks:
+            callback(self.address, self.data)
+        self.address += 2
+        if self.count == 0:
+            self.state = ParserState.ADDRESS_LOW
+        else:
+            self.state = ParserState.DATA_LOW
+
+    def _wait_for_sync(self) -> None:
+        """Handling of WAIT_FOR_SYNC state."""
+        if self.sync_byte_count == 4:
+            self.state = ParserState.ADDRESS_LOW
+            self.sync_byte_count = 0
+            for callback in self.frame_sync_callbacks:
+                callback()
+
+
+class StringBuffer:
+    """String buffer for DCS-BIOS protocol."""
+    def __init__(self, parser: ProtocolParser, address: int, max_length: int, callback: Callable) -> None:
+        """
+        Basic constructor.
+
+        :param parser:
+        :param address:
+        :param max_length:
+        :param callback:
+        """
+        self.__address = address
+        self.__length = max_length
+        self.__dirty = False
+        self.buffer = bytearray(max_length)
+        self.callbacks: Set[Callable] = set()
+        self.callbacks.add(callback)
+        parser.write_callbacks.add(partial(self.on_dcsbios_write))
+
+    def set_char(self, index, char) -> None:
+        """
+        Set char.
+
+        :param index:
+        :param char:
+        """
+        if self.buffer[index] != char:
+            self.buffer[index] = char
+            self.__dirty = True
+
+    def on_dcsbios_write(self, address: int, data: int) -> None:
+        """
+        Callback function.
+
+        :param address:
+        :param data:
+        """
+        if self.__address <= address < self.__address + self.__length:
+            data_bytes = pack('<H', data)
+            self.set_char(address - self.__address, data_bytes[0])
+            if self.__address + self.__length > (address + 1):
+                self.set_char(address - self.__address + 1, data_bytes[1])
+
+        if address == 0xfffe and self.__dirty:
+            self.__dirty = False
+            str_buff = self.buffer.split(sep=b'\x00', maxsplit=1)[0].decode('latin-1')
+            for callback in self.callbacks:
+                callback(str_buff)
+
+
+class IntegerBuffer:
+    """Integer buffer for DCS-BIOS protocol."""
+    def __init__(self, parser: ProtocolParser, address: int, mask: int, shift_by: int, callback: Callable) -> None:
+        """
+        Basic constructor.
+
+        :param parser:
+        :param address:
+        :param mask:
+        :param shift_by:
+        :param callback:
+        """
+        self.__address = address
+        self.__mask = mask
+        self.__shift_by = shift_by
+        self.__value = int()
+        self.callbacks: Set[Callable] = set()
+        self.callbacks.add(callback)
+        parser.write_callbacks.add(partial(self.on_dcsbios_write))
+
+    def on_dcsbios_write(self, address: int, data: int) -> None:
+        """
+        Callback function.
+
+        :param address:
+        :param data:
+        """
+        if address == self.__address:
+            value = (data & self.__mask) >> self.__shift_by
+            if self.__value != value:
+                self.__value = value
+                for callback in self.callbacks:
+                    callback(value)
```

### Comparing `dcspy-1.9.5/dcspy/dcspy.ico` & `dcspy-2.0.0/dcspy/dcspy.ico`

 * *Files identical despite different names*

### Comparing `dcspy-1.9.5/dcspy/dcspy.png` & `dcspy-2.0.0/dcspy/dcspy.png`

 * *Files identical despite different names*

### Comparing `dcspy-1.9.5/dcspy/dcspy_white.ico` & `dcspy-2.0.0/dcspy/dcspy_white.ico`

 * *Files identical despite different names*

### Comparing `dcspy-1.9.5/dcspy/falconded.ttf` & `dcspy-2.0.0/dcspy/falconded.ttf`

 * *Files identical despite different names*

### Comparing `dcspy-1.9.5/dcspy/log.py` & `dcspy-2.0.0/dcspy/log.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from datetime import datetime
-from logging import DEBUG, StreamHandler, INFO, Formatter, Logger
-from logging.handlers import RotatingFileHandler
-from os import path
-from tempfile import gettempdir
-
-
-def config_logger(logger: Logger, verbose=False) -> None:
-    """
-    Configure global logger add handlers and set formatters.
-
-    :param logger:
-    :param verbose: turn on/off verbose mode
-    """
-    logger.setLevel(DEBUG)
-    file_hand = RotatingFileHandler(filename=path.join(gettempdir(), 'dcspy.log'), mode='a', encoding='utf-8', maxBytes=5 * 1024 * 1024, backupCount=1)
-    file_hand.setLevel(DEBUG)
-    file_hand.setFormatter(Formatter('%(asctime)s | %(name)-17s | %(levelname)-7s | %(threadName)-10s | %(message)s / %(funcName)s:%(lineno)d'))
-    stream_hand = StreamHandler()
-    stream_hand.setLevel(INFO)
-    if verbose:
-        stream_hand.setLevel(DEBUG)
-    stream_hand.setFormatter(Formatter('%(levelname)-7s | %(message)s'))
-    logger.addHandler(stream_hand)
-    logger.addHandler(file_hand)
-    header = '#' * 60
-    logger.debug(f'\n{header}\nStart session: {datetime.now()}\n{header}')
-    logger.info(f'Log file store at: {file_hand.baseFilename}')
+from datetime import datetime
+from logging import DEBUG, StreamHandler, INFO, Formatter, Logger
+from logging.handlers import RotatingFileHandler
+from pathlib import Path
+from tempfile import gettempdir
+
+
+def config_logger(logger: Logger, verbose=False) -> None:
+    """
+    Configure global logger add handlers and set formatters.
+
+    :param logger:
+    :param verbose: turn on/off verbose mode
+    """
+    logger.setLevel(DEBUG)
+    file_hand = RotatingFileHandler(filename=Path(gettempdir()) / 'dcspy.log', mode='a', encoding='utf-8', maxBytes=5 * 1024 * 1024, backupCount=1)
+    file_hand.setFormatter(Formatter('%(asctime)s | %(name)-17s | %(levelname)-7s | %(threadName)-10s | %(message)s / %(funcName)s:%(lineno)d'))
+    file_hand.setLevel(INFO)
+    stream_hand = StreamHandler()
+    stream_hand.setLevel(INFO)
+    if verbose:
+        file_hand.setLevel(DEBUG)
+        stream_hand.setLevel(DEBUG)
+    stream_hand.setFormatter(Formatter('%(levelname)-7s | %(message)s'))
+    logger.addHandler(stream_hand)
+    logger.addHandler(file_hand)
+    header = '#' * 60
+    logger.debug(f'\n{header}\nStart session: {datetime.now()}\n{header}')
+    logger.info(f'Log file store at: {file_hand.baseFilename}')
```

### Comparing `dcspy-1.9.5/dcspy/logitech.py` & `dcspy-2.0.0/dcspy/logitech.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-from functools import partial
-from importlib import import_module
-from logging import getLogger
-from pprint import pformat
-from socket import socket
-from typing import List
-
-from PIL import Image, ImageDraw
-
-from dcspy import LcdColor, LcdMono, SUPPORTED_CRAFTS, SEND_ADDR, LcdButton
-from dcspy.aircraft import Aircraft
-from dcspy.dcsbios import ProtocolParser
-from dcspy.sdk import lcd_sdk
-
-LOG = getLogger(__name__)
-
-
-class LogitechKeyboard:
-    """General keyboard with LCD from Logitech."""
-    def __init__(self, parser: ProtocolParser, **kwargs) -> None:
-        """
-        General keyboard with LCD from Logitech.
-
-        It can be easily extended for any of:
-        - Mono LCD: G13, G15 (v1 and v2) and G510
-        - RGB LCD: G19
-
-        However, it defines a bunch of functionally to be used be child class:
-        - DCS-BIOS callback for currently used aircraft in DCS
-        - auto-detecting aircraft and load its handling class
-        - send button request to DCS-BIOS
-
-        Child class needs redefine:
-        - pass lcd_type argument as LcdInfo to super constructor
-
-        :param parser: DCS-BIOS parser instance
-        """
-        detect_plane = {'parser': parser, 'address': 0x0, 'max_length': 0x10, 'callback': partial(self.detecting_plane)}
-        getattr(import_module('dcspy.dcsbios'), 'StringBuffer')(**detect_plane)
-        self.parser = parser
-        self.plane_name = ''
-        self.plane_detected = False
-        self.already_pressed = False
-        self._display: List[str] = []
-        self.lcd = kwargs.get('lcd_type', LcdMono)
-        lcd_sdk.logi_lcd_init('DCS World', self.lcd.type.value)
-        self.plane = Aircraft(self.lcd)
-        self.vert_space = 0
-
-    @property
-    def display(self) -> List[str]:
-        """
-        Get the latest text from LCD.
-
-        :return: list of strings with data, row by row
-        """
-        return self._display
-
-    @display.setter
-    def display(self, message: List[str]) -> None:
-        """
-        Display message as image at LCD.
-
-        For G13/G15/G510 takes first 4 or fewer elements of list and display as 4 rows.
-        For G19 takes first 8 or fewer elements of list and display as 8 rows.
-        :param message: List of strings to display, row by row.
-        """
-        self._display = message
-        lcd_sdk.update_display(self._prepare_image())
-
-    @staticmethod
-    def text(message: List[str]) -> None:
-        """
-        Display message at LCD.
-
-        For G13/G15/G510 takes first 4 or fewer elements of list and display as 4 rows.
-        For G19 takes first 8 or fewer elements of list and display as 8 rows.
-        :param message: List of strings to display, row by row.
-        """
-        lcd_sdk.update_text(message)
-
-    def detecting_plane(self, value: str) -> None:
-        """
-        Try to detect airplane base on value received from DCS-BIOS.
-
-        :param value: data from DCS-BIOS
-        """
-        short_name = value.replace('-', '').replace('_', '')
-        if self.plane_name != short_name:
-            self.plane_name = short_name
-            if self.plane_name in SUPPORTED_CRAFTS:
-                LOG.info(f'Detected Aircraft: {value}')
-                self.display = ['Detected aircraft:', SUPPORTED_CRAFTS[self.plane_name]['name']]
-                self.plane_detected = True
-            elif self.plane_name not in SUPPORTED_CRAFTS and self.plane_name:
-                LOG.warning(f'Not supported aircraft: {value}')
-                self.display = ['Detected aircraft:', self.plane_name, 'Not supported yet!']
-
-    def load_new_plane(self) -> None:
-        """
-        Dynamic load of new detected aircraft.
-
-        Setup callbacks for detected plane inside DCS-BIOS parser.
-        """
-        self.plane_detected = False
-        self.plane = getattr(import_module('dcspy.aircraft'), self.plane_name)(self.lcd)
-        LOG.debug(f'Dynamic load of: {self.plane_name} as {SUPPORTED_CRAFTS[self.plane_name]["name"]}')
-        LOG.debug(f'{repr(self)}')
-        for field_name, proto_data in self.plane.bios_data.items():
-            dcsbios_buffer = getattr(import_module('dcspy.dcsbios'), proto_data['class'])
-            dcsbios_buffer(parser=self.parser, callback=partial(self.plane.set_bios, field_name), **proto_data['args'])
-
-    def check_buttons(self) -> LcdButton:
-        """
-        Check if button was pressed and return it`s enum.
-
-        :return: LcdButton enum of pressed button
-        """
-        for btn in self.lcd.buttons:
-            if lcd_sdk.logi_lcd_is_button_pressed(btn.value):
-                if not self.already_pressed:
-                    self.already_pressed = True
-                    return LcdButton(btn)
-                return LcdButton.NONE
-        self.already_pressed = False
-        return LcdButton.NONE
-
-    def button_handle(self, sock: socket) -> None:
-        """
-        Button handler.
-
-        * detect if button was pressed
-        * fetch DCS-BIOS request from current plane
-        * sent action to DCS-BIOS via. network socket
-        :param sock: network socket
-        """
-        button = self.check_buttons()
-        if button.value:
-            sock.sendto(bytes(self.plane.button_request(button), 'utf-8'), SEND_ADDR)
-
-    def clear(self, true_clear=False):
-        """
-        Clear LCD.
-
-        :param true_clear:
-        """
-        LOG.debug(f'Clear LCD type: {self.lcd.type}')
-        lcd_sdk.clear_display(true_clear)
-
-    def _prepare_image(self) -> Image.Image:
-        """
-        Prepare image for base of LCD type.
-
-        For G13/G15/G510 takes first 4 or fewer elements of list and display as 4 rows.
-        For G19 takes first 8 or fewer elements of list and display as 8 rows.
-        :return: image instance ready display on LCD
-        """
-        img = Image.new(mode=self.lcd.mode, size=(self.lcd.width, self.lcd.height), color=self.lcd.background)
-        draw = ImageDraw.Draw(img)
-        for line_no, line in enumerate(self._display):
-            draw.text(xy=(0, self.vert_space * line_no), text=line, fill=self.lcd.foreground, font=self.lcd.font_s)
-        return img
-
-    def __str__(self) -> str:
-        """
-        Show basic info of LCD.
-
-        :return: string
-        """
-        return f'{self.__class__.__name__}: {self.lcd.width}x{self.lcd.height}'
-
-    def __repr__(self) -> str:
-        """
-        Show all details of LCD.
-
-        :return: string
-        """
-        return f'{super().__repr__()} with: {pformat(self.__dict__)}'
-
-
-class KeyboardMono(LogitechKeyboard):
-    """Logitech`s keyboard with mono LCD."""
-    def __init__(self, parser: ProtocolParser) -> None:
-        """
-        Logitech`s keyboard with mono LCD.
-
-        Support for: G510, G13, G15 (v1 and v2)
-        :param parser: DCS-BIOS parser instance
-        """
-        super().__init__(parser, lcd_type=LcdMono)
-        self.vert_space = 10
-
-
-class KeyboardColor(LogitechKeyboard):
-    """Logitech`s keyboard with color LCD."""
-    def __init__(self, parser: ProtocolParser) -> None:
-        """
-        Logitech`s keyboard with color LCD.
-
-        Support for: G19
-        :param parser: DCS-BIOS parser instance
-        """
-        super().__init__(parser, lcd_type=LcdColor)
-        self.vert_space = 40
+from functools import partial
+from importlib import import_module
+from logging import getLogger
+from pprint import pformat
+from socket import socket
+from typing import List
+
+from PIL import Image, ImageDraw
+
+from dcspy import LcdColor, LcdMono, SUPPORTED_CRAFTS, SEND_ADDR, LcdButton
+from dcspy.aircraft import Aircraft
+from dcspy.dcsbios import ProtocolParser
+from dcspy.sdk import lcd_sdk
+
+LOG = getLogger(__name__)
+
+
+class LogitechKeyboard:
+    """General keyboard with LCD from Logitech."""
+    def __init__(self, parser: ProtocolParser, **kwargs) -> None:
+        """
+        General keyboard with LCD from Logitech.
+
+        It can be easily extended for any of:
+        - Mono LCD: G13, G15 (v1 and v2) and G510
+        - RGB LCD: G19
+
+        However, it defines a bunch of functionally to be used be child class:
+        - DCS-BIOS callback for currently used aircraft in DCS
+        - auto-detecting aircraft and load its handling class
+        - send button request to DCS-BIOS
+
+        Child class needs redefine:
+        - pass lcd_type argument as LcdInfo to super constructor
+
+        :param parser: DCS-BIOS parser instance
+        """
+        detect_plane = {'parser': parser, 'address': 0x0, 'max_length': 0x10, 'callback': partial(self.detecting_plane)}
+        getattr(import_module('dcspy.dcsbios'), 'StringBuffer')(**detect_plane)
+        self.parser = parser
+        self.plane_name = ''
+        self.plane_detected = False
+        self.already_pressed = False
+        self._display: List[str] = []
+        self.lcd = kwargs.get('lcd_type', LcdMono)
+        lcd_sdk.logi_lcd_init('DCS World', self.lcd.type.value)
+        self.plane = Aircraft(self.lcd)
+        self.vert_space = 0
+
+    @property
+    def display(self) -> List[str]:
+        """
+        Get the latest text from LCD.
+
+        :return: list of strings with data, row by row
+        """
+        return self._display
+
+    @display.setter
+    def display(self, message: List[str]) -> None:
+        """
+        Display message as image at LCD.
+
+        For G13/G15/G510 takes first 4 or fewer elements of list and display as 4 rows.
+        For G19 takes first 8 or fewer elements of list and display as 8 rows.
+        :param message: List of strings to display, row by row.
+        """
+        self._display = message
+        lcd_sdk.update_display(self._prepare_image())
+
+    @staticmethod
+    def text(message: List[str]) -> None:
+        """
+        Display message at LCD.
+
+        For G13/G15/G510 takes first 4 or fewer elements of list and display as 4 rows.
+        For G19 takes first 8 or fewer elements of list and display as 8 rows.
+        :param message: List of strings to display, row by row.
+        """
+        lcd_sdk.update_text(message)
+
+    def detecting_plane(self, value: str) -> None:
+        """
+        Try to detect airplane base on value received from DCS-BIOS.
+
+        :param value: data from DCS-BIOS
+        """
+        short_name = value.replace('-', '').replace('_', '')
+        if self.plane_name != short_name:
+            self.plane_name = short_name
+            if self.plane_name in SUPPORTED_CRAFTS:
+                LOG.info(f'Detected Aircraft: {value}')
+                self.display = ['Detected aircraft:', SUPPORTED_CRAFTS[self.plane_name]['name']]
+                self.plane_detected = True
+            elif self.plane_name not in SUPPORTED_CRAFTS and self.plane_name:
+                LOG.warning(f'Not supported aircraft: {value}')
+                self.display = ['Detected aircraft:', self.plane_name, 'Not supported yet!']
+
+    def load_new_plane(self) -> None:
+        """
+        Dynamic load of new detected aircraft.
+
+        Setup callbacks for detected plane inside DCS-BIOS parser.
+        """
+        self.plane_detected = False
+        self.plane = getattr(import_module('dcspy.aircraft'), self.plane_name)(self.lcd)
+        LOG.debug(f'Dynamic load of: {self.plane_name} as {SUPPORTED_CRAFTS[self.plane_name]["name"]}')
+        LOG.debug(f'{repr(self)}')
+        for field_name, proto_data in self.plane.bios_data.items():
+            dcsbios_buffer = getattr(import_module('dcspy.dcsbios'), proto_data['klass'])
+            dcsbios_buffer(parser=self.parser, callback=partial(self.plane.set_bios, field_name), **proto_data['args'])
+
+    def check_buttons(self) -> LcdButton:
+        """
+        Check if button was pressed and return it`s enum.
+
+        :return: LcdButton enum of pressed button
+        """
+        for btn in self.lcd.buttons:
+            if lcd_sdk.logi_lcd_is_button_pressed(btn.value):
+                if not self.already_pressed:
+                    self.already_pressed = True
+                    return LcdButton(btn)
+                return LcdButton.NONE
+        self.already_pressed = False
+        return LcdButton.NONE
+
+    def button_handle(self, sock: socket) -> None:
+        """
+        Button handler.
+
+        * detect if button was pressed
+        * fetch DCS-BIOS request from current plane
+        * sent action to DCS-BIOS via. network socket
+        :param sock: network socket
+        """
+        button = self.check_buttons()
+        if button.value:
+            sock.sendto(bytes(self.plane.button_request(button), 'utf-8'), SEND_ADDR)
+
+    def clear(self, true_clear=False):
+        """
+        Clear LCD.
+
+        :param true_clear:
+        """
+        LOG.debug(f'Clear LCD type: {self.lcd.type}')
+        lcd_sdk.clear_display(true_clear)
+
+    def _prepare_image(self) -> Image.Image:
+        """
+        Prepare image for base of LCD type.
+
+        For G13/G15/G510 takes first 4 or fewer elements of list and display as 4 rows.
+        For G19 takes first 8 or fewer elements of list and display as 8 rows.
+        :return: image instance ready display on LCD
+        """
+        img = Image.new(mode=self.lcd.mode, size=(self.lcd.width, self.lcd.height), color=self.lcd.background)
+        draw = ImageDraw.Draw(img)
+        for line_no, line in enumerate(self._display):
+            draw.text(xy=(0, self.vert_space * line_no), text=line, fill=self.lcd.foreground, font=self.lcd.font_s)
+        return img
+
+    def __str__(self) -> str:
+        """
+        Show basic info of LCD.
+
+        :return: string
+        """
+        return f'{self.__class__.__name__}: {self.lcd.width}x{self.lcd.height}'
+
+    def __repr__(self) -> str:
+        """
+        Show all details of LCD.
+
+        :return: string
+        """
+        return f'{super().__repr__()} with: {pformat(self.__dict__)}'
+
+
+class KeyboardMono(LogitechKeyboard):
+    """Logitech`s keyboard with mono LCD."""
+    def __init__(self, parser: ProtocolParser) -> None:
+        """
+        Logitech`s keyboard with mono LCD.
+
+        Support for: G510, G13, G15 (v1 and v2)
+        :param parser: DCS-BIOS parser instance
+        """
+        super().__init__(parser, lcd_type=LcdMono)
+        self.vert_space = 10
+
+
+class KeyboardColor(LogitechKeyboard):
+    """Logitech`s keyboard with color LCD."""
+    def __init__(self, parser: ProtocolParser) -> None:
+        """
+        Logitech`s keyboard with color LCD.
+
+        Support for: G19
+        :param parser: DCS-BIOS parser instance
+        """
+        super().__init__(parser, lcd_type=LcdColor)
+        self.vert_space = 40
```

### Comparing `dcspy-1.9.5/dcspy/run.py` & `dcspy-2.0.0/dcspy/run.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-from logging import getLogger
-from os import path
-from threading import Event
-
-import customtkinter
-
-from dcspy import config, LCD_TYPES
-from dcspy.starter import dcspy_run
-from dcspy.tk_gui import DcspyGui
-from dcspy.utils import check_dcs_ver
-
-LOG = getLogger(__name__)
-__version__ = '1.9.5'
-
-
-def run():
-    """Function to start DCSpy GUI."""
-    if config['show_gui']:
-        customtkinter.set_appearance_mode(config['theme_mode'])
-        customtkinter.set_default_color_theme(config['theme_color'])
-        LOG.info(f'dcspy {__version__} https://github.com/emcek/dcspy')
-        dcs_type, dcs_ver = check_dcs_ver(config["dcs"])
-        LOG.info(f'DCS {dcs_type} ver: {dcs_ver}')
-        root = customtkinter.CTk()
-        width, height = 770, 500
-        root.geometry(f'{width}x{height}')
-        root.minsize(width=width, height=height)
-        here = path.abspath(path.dirname(__file__))
-        root.iconbitmap(path.join(here, 'dcspy.ico'))
-        if config['theme_mode'] == 'dark':
-            root.iconbitmap(path.join(here, 'dcspy_white.ico'))
-        root.title('DCSpy')
-        DcspyGui(master=root, config_file=path.join(here, 'config.yaml'))
-        root.mainloop()
-    else:
-        dcspy_run(lcd_type=LCD_TYPES[config['keyboard']]['type'], event=Event())
-
-
-if __name__ == '__main__':
-    run()
+from logging import getLogger
+from pathlib import Path
+from threading import Event
+
+import customtkinter
+
+from dcspy import config, LCD_TYPES
+from dcspy.starter import dcspy_run
+from dcspy.tk_gui import DcspyGui
+from dcspy.utils import check_dcs_ver
+
+LOG = getLogger(__name__)
+__version__ = '2.0.0'
+
+
+def run():
+    """Function to start DCSpy GUI."""
+    if config['show_gui']:
+        customtkinter.set_appearance_mode(config['theme_mode'])
+        customtkinter.set_default_color_theme(config['theme_color'])
+        LOG.info(f'dcspy {__version__} https://github.com/emcek/dcspy')
+        dcs_type, dcs_ver = check_dcs_ver(Path(str(config["dcs"])))
+        LOG.info(f'DCS {dcs_type} ver: {dcs_ver}')
+        root = customtkinter.CTk()
+        width, height = 770, 500
+        root.geometry(f'{width}x{height}')
+        root.minsize(width=width, height=height)
+        root.iconbitmap(Path(__file__).resolve().with_name('dcspy.ico'))
+        if config['theme_mode'] == 'dark':
+            root.iconbitmap(Path(__file__).resolve().with_name('dcspy_white.ico'))
+        root.title('DCSpy')
+        DcspyGui(master=root)
+        root.mainloop()
+    else:
+        dcspy_run(lcd_type=LCD_TYPES[config['keyboard']]['type'], event=Event())
+
+
+if __name__ == '__main__':
+    run()
```

### Comparing `dcspy-1.9.5/dcspy/sdk/__init__.py` & `dcspy-2.0.0/dcspy/sdk/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from ctypes import CDLL, sizeof, c_void_p
-from logging import getLogger
-from os import environ
-from platform import architecture
-from sys import maxsize
-from typing import Optional
-
-LOG = getLogger(__name__)
-
-
-def _init_dll(lib_type: str) -> CDLL:
-    """
-    Initialization of C dynamic linking library.
-
-    :param lib_type: LCD or LED
-    :return: C DLL instance
-    """
-    arch = 'x64' if all([architecture()[0] == '64bit', maxsize > 2 ** 32, sizeof(c_void_p) > 4]) else 'x86'
-    try:
-        prog_files = environ['PROGRAMW6432']
-    except KeyError:
-        prog_files = environ['PROGRAMFILES']
-    return CDLL(f"{prog_files}\\Logitech Gaming Software\\SDK\\{lib_type}\\{arch}\\Logitech{lib_type.capitalize()}.dll")
-
-
-def load_dll(lib_type: str) -> Optional[CDLL]:
-    """
-    Initialization and loading of C dynamic linking library.
-
-    :param lib_type: library to load: LCD or LED
-    :return: C DLL instance
-    """
-    try:
-        dll = _init_dll(lib_type)
-        LOG.info(f'Loading of {lib_type} SDK success')
-        return dll
-    except (KeyError, FileNotFoundError) as err:
-        header = '*' * 40
-        space = ' ' * 15
-        LOG.error(f'\n{header}\n*{space}ERROR!!!{space}*\n{header}\n'
-                  f'Loading of {lib_type} SDK failed: {err.__class__.__name__}', exc_info=True)
-        LOG.error(f'\n{header}')
-        return None
+from ctypes import CDLL, sizeof, c_void_p
+from logging import getLogger
+from os import environ
+from platform import architecture
+from sys import maxsize
+from typing import Optional
+
+LOG = getLogger(__name__)
+
+
+def _init_dll(lib_type: str) -> CDLL:
+    """
+    Initialization of C dynamic linking library.
+
+    :param lib_type: LCD or LED
+    :return: C DLL instance
+    """
+    arch = 'x64' if all([architecture()[0] == '64bit', maxsize > 2 ** 32, sizeof(c_void_p) > 4]) else 'x86'
+    try:
+        prog_files = environ['PROGRAMW6432']
+    except KeyError:
+        prog_files = environ['PROGRAMFILES']
+    return CDLL(f"{prog_files}\\Logitech Gaming Software\\SDK\\{lib_type}\\{arch}\\Logitech{lib_type.capitalize()}.dll")
+
+
+def load_dll(lib_type: str) -> Optional[CDLL]:
+    """
+    Initialization and loading of C dynamic linking library.
+
+    :param lib_type: library to load: LCD or LED
+    :return: C DLL instance
+    """
+    try:
+        dll = _init_dll(lib_type)
+        LOG.info(f'Loading of {lib_type} SDK success')
+        return dll
+    except (KeyError, FileNotFoundError) as err:
+        header = '*' * 44
+        error_string = 'ERROR!!!'
+        LOG.error(f'\n{header}\n*{error_string:^42}*\n{header}\n'
+                  f'Loading of {lib_type} SDK failed: {err.__class__.__name__}', exc_info=True)
+        LOG.error(f'{header}')
+        return None
```

### Comparing `dcspy-1.9.5/dcspy/sdk/lcd_sdk.py` & `dcspy-2.0.0/dcspy/sdk/lcd_sdk.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,253 +1,253 @@
-from ctypes import c_bool, c_wchar_p, c_int, c_ubyte
-from logging import getLogger
-from typing import List, Tuple
-
-from PIL import Image
-
-from dcspy.sdk import load_dll
-
-LOG = getLogger(__name__)
-
-# LCD types
-TYPE_MONO = 1
-TYPE_COLOR = 2
-
-# LCD Monochrome size
-MONO_WIDTH = 160
-MONO_HEIGHT = 43
-
-# LCD Color size
-COLOR_WIDTH = 320
-COLOR_HEIGHT = 240
-
-LCD_DLL = load_dll('LCD')
-
-
-def logi_lcd_init(name: str, lcd_type: int) -> bool:
-    """
-    Function makes necessary initializations.
-
-    You must call this function prior to any other function in the library.
-    :param name: the name of your applet, you can't change it after initialization
-    :param lcd_type: defines the type of your applet lcd target
-    :return: result
-    """
-    if LCD_DLL:
-        logilcdinit = LCD_DLL['LogiLcdInit']
-        logilcdinit.restype = c_bool
-        logilcdinit.argtypes = (c_wchar_p, c_int)
-        return logilcdinit(name, lcd_type)
-    return False
-
-
-def logi_lcd_is_connected(lcd_type: int) -> bool:
-    """
-    Function checks if a device of the type specified by the parameter is connected.
-
-    :param lcd_type: defines the type of your applet lcd target
-    :return: result
-    """
-    if LCD_DLL:
-        logilcdisconnected = LCD_DLL['LogiLcdIsConnected']
-        logilcdisconnected.restype = c_bool
-        logilcdisconnected.argtypes = [c_int]
-        return logilcdisconnected(lcd_type)
-    return False
-
-
-def logi_lcd_is_button_pressed(button: int) -> bool:
-    """
-    Function checks if the button specified by the parameter is being pressed.
-
-    :param button: defines the button to check on
-    :return: result
-    """
-    if LCD_DLL:
-        logilcdisbuttonpressed = LCD_DLL['LogiLcdIsButtonPressed']
-        logilcdisbuttonpressed.restype = c_bool
-        logilcdisbuttonpressed.argtypes = [c_int]
-        return logilcdisbuttonpressed(button)
-    return False
-
-
-def logi_lcd_update() -> None:
-    """Function updates the LCD."""
-    if LCD_DLL:
-        logilcdupdate = LCD_DLL['LogiLcdUpdate']
-        logilcdupdate.restype = None
-        logilcdupdate()
-
-
-def logi_lcd_shutdown() -> None:
-    """Function kills the applet and frees memory used by the SDK."""
-    if LCD_DLL:
-        logilcdshutdown = LCD_DLL['LogiLcdShutdown']
-        logilcdshutdown.restype = None
-        logilcdshutdown()
-
-
-def logi_lcd_mono_set_background(pixels: List[int]) -> bool:
-    """
-    The array of pixels is organized as a rectangular area, 160 bytes wide and 43 bytes high.
-
-    Despite the display being monochrome, 8 bits per pixel are used here for simple
-    manipulation of individual pixels.
-
-    Note: The image size must be 160x43 in order to use this function. The SDK will turn on
-    the pixel on the screen if the value assigned to that byte is >= 128, it will remain off
-    if the  value is < 128.
-    :param pixels: list of 6880 (160x43) pixels as int
-    :return: result
-    """
-    if LCD_DLL:
-        logilcdmonosetbackground = LCD_DLL['LogiLcdMonoSetBackground']
-        logilcdmonosetbackground.restype = c_bool
-        logilcdmonosetbackground.argtypes = [c_ubyte * (MONO_WIDTH * MONO_HEIGHT)]
-        img_bytes = [pixel * 128 for pixel in pixels]
-        return logilcdmonosetbackground((c_ubyte * (MONO_WIDTH * MONO_HEIGHT))(*img_bytes))
-    return False
-
-
-def logi_lcd_mono_set_text(line_no: int, text: str):
-    """
-    Function sets the specified text in the requested line on the monochrome lcd device connected.
-
-    :param line_no: The monochrome LCD has 4 lines, so this parameter can be any number from 0 to 3
-    :param text: defines the text you want to display
-    :return: result
-    """
-    if LCD_DLL:
-        logilcdmonosettext = LCD_DLL['LogiLcdMonoSetText']
-        logilcdmonosettext.restype = c_bool
-        logilcdmonosettext.argtypes = (c_int, c_wchar_p)
-        return logilcdmonosettext(line_no, text)
-    return False
-
-
-def logi_lcd_color_set_background(pixels: List[Tuple[int, int, int, int]]) -> bool:
-    """
-    The array of pixels is organized as a rectangular area, 320 bytes wide and 240 bytes high.
-
-    Since the color lcd can display the full RGB gamma, 32 bits per pixel (4 bytes) are used.
-    The size of the colorBitmap array has to be 320x240x4 = 307200 therefore.
-    Note: The image size must be 320x240 in order to use this function.
-    :param pixels: list of 307200 (320x240x4) pixels as int
-    :return: result
-    """
-    if LCD_DLL:
-        logilcdcolorsetbackground = LCD_DLL['LogiLcdColorSetBackground']
-        logilcdcolorsetbackground.restype = c_bool
-        logilcdcolorsetbackground.argtypes = [c_ubyte * (4 * COLOR_WIDTH * COLOR_HEIGHT)]
-        img_bytes = [byte for pixel in pixels for byte in pixel]
-        return logilcdcolorsetbackground((c_ubyte * (4 * COLOR_WIDTH * COLOR_HEIGHT))(*img_bytes))
-    return False
-
-
-def logi_lcd_color_set_title(text: str, rgb: Tuple[int, int, int] = (255, 255, 255)):
-    """
-    Function sets the specified text in the first line on the color lcd device connected.
-
-    The font size that will be displayed is bigger than the one used in the other lines,
-    so you can use this function to set the title of your applet/page.
-    If you don't specify any color, your title will be white.
-    :param text: defines the text you want to display as title
-    :param rgb: tuple with integer values between 0 and 255 as red, green, blue
-    :return: result
-    """
-    if LCD_DLL:
-        logilcdcolorsettitle = LCD_DLL['LogiLcdColorSetTitle']
-        logilcdcolorsettitle.restype = c_bool
-        logilcdcolorsettitle.argtypes = (c_wchar_p, c_int, c_int, c_int)
-        return logilcdcolorsettitle(text, *rgb)
-    return False
-
-
-def logi_lcd_color_set_text(line_no: int, text: str, rgb: Tuple[int, int, int] = (255, 255, 255)):
-    """
-    Function sets the specified text in the requested line on the color lcd device connected.
-
-    If you don't specify any color, your title will be white.
-    :param line_no: The color LCD has 8 lines for standard text, so this parameter can be any number from 0 to 7
-    :param text: defines the text you want to display
-    :param rgb: tuple with integer values between 0 and 255 as red, green, blue
-    :return: result
-    """
-    if LCD_DLL:
-        logilcdcolorsettext = LCD_DLL['LogiLcdColorSetText']
-        logilcdcolorsettext.restype = c_bool
-        logilcdcolorsettext.argtypes = (c_int, c_wchar_p, c_int, c_int, c_int)
-        return logilcdcolorsettext(line_no, text, *rgb)
-    return False
-
-
-def update_text(txt: List[str]) -> None:
-    """
-    Update display LCD with list of text.
-
-    For mono LCD it takes 4 elements of list and display as 4 rows.
-    For color LCD  takes 8 elements of list and display as 8 rows.
-    :param txt: List of strings to display, row by row
-    """
-    if logi_lcd_is_connected(TYPE_MONO):
-        for line_no, line in enumerate(txt):
-            logi_lcd_mono_set_text(line_no, line)
-        logi_lcd_update()
-    elif logi_lcd_is_connected(TYPE_COLOR):
-        for line_no, line in enumerate(txt):
-            logi_lcd_color_set_text(line_no, line)
-        logi_lcd_update()
-    else:
-        LOG.warning('LCD is not connected')
-
-
-def update_display(image: Image) -> None:
-    """
-    Update display LCD with image.
-
-    :param image: image object from pillow library
-    """
-    if logi_lcd_is_connected(TYPE_MONO):
-        logi_lcd_mono_set_background(list(image.getdata()))
-        logi_lcd_update()
-    elif logi_lcd_is_connected(TYPE_COLOR):
-        logi_lcd_color_set_background(list(image.getdata()))
-        logi_lcd_update()
-    else:
-        LOG.warning('LCD is not connected')
-
-
-def clear_display(true_clear=False) -> None:
-    """
-    Clear display.
-
-    :param true_clear:
-    """
-    if logi_lcd_is_connected(TYPE_MONO):
-        _clear_mono(true_clear)
-    elif logi_lcd_is_connected(TYPE_COLOR):
-        _clear_color(true_clear)
-    logi_lcd_update()
-
-
-def _clear_mono(true_clear):
-    """
-    Clear mono display.
-
-    :param true_clear:
-    """
-    logi_lcd_mono_set_background([0] * MONO_WIDTH * MONO_HEIGHT)
-    if true_clear:
-        for i in range(4):
-            logi_lcd_mono_set_text(i, '')
-
-
-def _clear_color(true_clear):
-    """
-    Clear color display.
-
-    :param true_clear:
-    """
-    logi_lcd_color_set_background([(0,) * 4] * COLOR_WIDTH * COLOR_HEIGHT)
-    if true_clear:
-        for i in range(8):
-            logi_lcd_color_set_text(i, '')
+from ctypes import c_bool, c_wchar_p, c_int, c_ubyte
+from logging import getLogger
+from typing import List, Tuple
+
+from PIL import Image
+
+from dcspy.sdk import load_dll
+
+LOG = getLogger(__name__)
+
+# LCD types
+TYPE_MONO = 1
+TYPE_COLOR = 2
+
+# LCD Monochrome size
+MONO_WIDTH = 160
+MONO_HEIGHT = 43
+
+# LCD Color size
+COLOR_WIDTH = 320
+COLOR_HEIGHT = 240
+
+LCD_DLL = load_dll('LCD')
+
+
+def logi_lcd_init(name: str, lcd_type: int) -> bool:
+    """
+    Function makes necessary initializations.
+
+    You must call this function prior to any other function in the library.
+    :param name: the name of your applet, you can't change it after initialization
+    :param lcd_type: defines the type of your applet lcd target
+    :return: result
+    """
+    if LCD_DLL:
+        logilcdinit = LCD_DLL['LogiLcdInit']
+        logilcdinit.restype = c_bool
+        logilcdinit.argtypes = (c_wchar_p, c_int)
+        return logilcdinit(name, lcd_type)
+    return False
+
+
+def logi_lcd_is_connected(lcd_type: int) -> bool:
+    """
+    Function checks if a device of the type specified by the parameter is connected.
+
+    :param lcd_type: defines the type of your applet lcd target
+    :return: result
+    """
+    if LCD_DLL:
+        logilcdisconnected = LCD_DLL['LogiLcdIsConnected']
+        logilcdisconnected.restype = c_bool
+        logilcdisconnected.argtypes = [c_int]
+        return logilcdisconnected(lcd_type)
+    return False
+
+
+def logi_lcd_is_button_pressed(button: int) -> bool:
+    """
+    Function checks if the button specified by the parameter is being pressed.
+
+    :param button: defines the button to check on
+    :return: result
+    """
+    if LCD_DLL:
+        logilcdisbuttonpressed = LCD_DLL['LogiLcdIsButtonPressed']
+        logilcdisbuttonpressed.restype = c_bool
+        logilcdisbuttonpressed.argtypes = [c_int]
+        return logilcdisbuttonpressed(button)
+    return False
+
+
+def logi_lcd_update() -> None:
+    """Function updates the LCD."""
+    if LCD_DLL:
+        logilcdupdate = LCD_DLL['LogiLcdUpdate']
+        logilcdupdate.restype = None
+        logilcdupdate()
+
+
+def logi_lcd_shutdown() -> None:
+    """Function kills the applet and frees memory used by the SDK."""
+    if LCD_DLL:
+        logilcdshutdown = LCD_DLL['LogiLcdShutdown']
+        logilcdshutdown.restype = None
+        logilcdshutdown()
+
+
+def logi_lcd_mono_set_background(pixels: List[int]) -> bool:
+    """
+    The array of pixels is organized as a rectangular area, 160 bytes wide and 43 bytes high.
+
+    Despite the display being monochrome, 8 bits per pixel are used here for simple
+    manipulation of individual pixels.
+
+    Note: The image size must be 160x43 in order to use this function. The SDK will turn on
+    the pixel on the screen if the value assigned to that byte is >= 128, it will remain off
+    if the  value is < 128.
+    :param pixels: list of 6880 (160x43) pixels as int
+    :return: result
+    """
+    if LCD_DLL:
+        logilcdmonosetbackground = LCD_DLL['LogiLcdMonoSetBackground']
+        logilcdmonosetbackground.restype = c_bool
+        logilcdmonosetbackground.argtypes = [c_ubyte * (MONO_WIDTH * MONO_HEIGHT)]
+        img_bytes = [pixel * 128 for pixel in pixels]
+        return logilcdmonosetbackground((c_ubyte * (MONO_WIDTH * MONO_HEIGHT))(*img_bytes))
+    return False
+
+
+def logi_lcd_mono_set_text(line_no: int, text: str):
+    """
+    Function sets the specified text in the requested line on the monochrome lcd device connected.
+
+    :param line_no: The monochrome LCD has 4 lines, so this parameter can be any number from 0 to 3
+    :param text: defines the text you want to display
+    :return: result
+    """
+    if LCD_DLL:
+        logilcdmonosettext = LCD_DLL['LogiLcdMonoSetText']
+        logilcdmonosettext.restype = c_bool
+        logilcdmonosettext.argtypes = (c_int, c_wchar_p)
+        return logilcdmonosettext(line_no, text)
+    return False
+
+
+def logi_lcd_color_set_background(pixels: List[Tuple[int, int, int, int]]) -> bool:
+    """
+    The array of pixels is organized as a rectangular area, 320 bytes wide and 240 bytes high.
+
+    Since the color lcd can display the full RGB gamma, 32 bits per pixel (4 bytes) are used.
+    The size of the colorBitmap array has to be 320x240x4 = 307200 therefore.
+    Note: The image size must be 320x240 in order to use this function.
+    :param pixels: list of 307200 (320x240x4) pixels as int
+    :return: result
+    """
+    if LCD_DLL:
+        logilcdcolorsetbackground = LCD_DLL['LogiLcdColorSetBackground']
+        logilcdcolorsetbackground.restype = c_bool
+        logilcdcolorsetbackground.argtypes = [c_ubyte * (4 * COLOR_WIDTH * COLOR_HEIGHT)]
+        img_bytes = [byte for pixel in pixels for byte in pixel]
+        return logilcdcolorsetbackground((c_ubyte * (4 * COLOR_WIDTH * COLOR_HEIGHT))(*img_bytes))
+    return False
+
+
+def logi_lcd_color_set_title(text: str, rgb: Tuple[int, int, int] = (255, 255, 255)):
+    """
+    Function sets the specified text in the first line on the color lcd device connected.
+
+    The font size that will be displayed is bigger than the one used in the other lines,
+    so you can use this function to set the title of your applet/page.
+    If you don't specify any color, your title will be white.
+    :param text: defines the text you want to display as title
+    :param rgb: tuple with integer values between 0 and 255 as red, green, blue
+    :return: result
+    """
+    if LCD_DLL:
+        logilcdcolorsettitle = LCD_DLL['LogiLcdColorSetTitle']
+        logilcdcolorsettitle.restype = c_bool
+        logilcdcolorsettitle.argtypes = (c_wchar_p, c_int, c_int, c_int)
+        return logilcdcolorsettitle(text, *rgb)
+    return False
+
+
+def logi_lcd_color_set_text(line_no: int, text: str, rgb: Tuple[int, int, int] = (255, 255, 255)):
+    """
+    Function sets the specified text in the requested line on the color lcd device connected.
+
+    If you don't specify any color, your title will be white.
+    :param line_no: The color LCD has 8 lines for standard text, so this parameter can be any number from 0 to 7
+    :param text: defines the text you want to display
+    :param rgb: tuple with integer values between 0 and 255 as red, green, blue
+    :return: result
+    """
+    if LCD_DLL:
+        logilcdcolorsettext = LCD_DLL['LogiLcdColorSetText']
+        logilcdcolorsettext.restype = c_bool
+        logilcdcolorsettext.argtypes = (c_int, c_wchar_p, c_int, c_int, c_int)
+        return logilcdcolorsettext(line_no, text, *rgb)
+    return False
+
+
+def update_text(txt: List[str]) -> None:
+    """
+    Update display LCD with list of text.
+
+    For mono LCD it takes 4 elements of list and display as 4 rows.
+    For color LCD  takes 8 elements of list and display as 8 rows.
+    :param txt: List of strings to display, row by row
+    """
+    if logi_lcd_is_connected(TYPE_MONO):
+        for line_no, line in enumerate(txt):
+            logi_lcd_mono_set_text(line_no, line)
+        logi_lcd_update()
+    elif logi_lcd_is_connected(TYPE_COLOR):
+        for line_no, line in enumerate(txt):
+            logi_lcd_color_set_text(line_no, line)
+        logi_lcd_update()
+    else:
+        LOG.warning('LCD is not connected')
+
+
+def update_display(image: Image) -> None:
+    """
+    Update display LCD with image.
+
+    :param image: image object from pillow library
+    """
+    if logi_lcd_is_connected(TYPE_MONO):
+        logi_lcd_mono_set_background(list(image.getdata()))
+        logi_lcd_update()
+    elif logi_lcd_is_connected(TYPE_COLOR):
+        logi_lcd_color_set_background(list(image.getdata()))
+        logi_lcd_update()
+    else:
+        LOG.warning('LCD is not connected')
+
+
+def clear_display(true_clear=False) -> None:
+    """
+    Clear display.
+
+    :param true_clear:
+    """
+    if logi_lcd_is_connected(TYPE_MONO):
+        _clear_mono(true_clear)
+    elif logi_lcd_is_connected(TYPE_COLOR):
+        _clear_color(true_clear)
+    logi_lcd_update()
+
+
+def _clear_mono(true_clear):
+    """
+    Clear mono display.
+
+    :param true_clear:
+    """
+    logi_lcd_mono_set_background([0] * MONO_WIDTH * MONO_HEIGHT)
+    if true_clear:
+        for i in range(4):
+            logi_lcd_mono_set_text(i, '')
+
+
+def _clear_color(true_clear):
+    """
+    Clear color display.
+
+    :param true_clear:
+    """
+    logi_lcd_color_set_background([(0,) * 4] * COLOR_WIDTH * COLOR_HEIGHT)
+    if true_clear:
+        for i in range(8):
+            logi_lcd_color_set_text(i, '')
```

### Comparing `dcspy-1.9.5/dcspy/sdk/led_sdk.py` & `dcspy-2.0.0/dcspy/sdk/led_sdk.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-from ctypes import c_bool, c_wchar_p, c_int
-from logging import getLogger
-from threading import Event
-from time import sleep
-from typing import Tuple
-
-from dcspy.sdk import load_dll
-
-LOG = getLogger(__name__)
-
-LOGI_LED_DURATION_INFINITE = 0
-LOGI_DEVICETYPE_MONOCHROME = 1
-LOGI_DEVICETYPE_RGB = 2
-LOGI_DEVICETYPE_ALL = LOGI_DEVICETYPE_MONOCHROME | LOGI_DEVICETYPE_RGB
-
-LED_DLL = load_dll('LED')
-
-
-def logi_led_init() -> bool:
-    """
-    The function makes sure there isn't already another instance running and then makes necessary initializations.
-
-    It saves the current lighting for all connected and supported devices. This function will also stop any effect
-    currently going on the connected devices.
-    :return: result
-    """
-    if LED_DLL:
-        logiledinit = LED_DLL['LogiLedInit']
-        logiledinit.restype = c_bool
-        return logiledinit()
-    return False
-
-
-def logi_led_init_with_name(name: str) -> bool:
-    """
-    The function makes sure there isn't already another instance running and then makes necessary initializations.
-
-    It saves the current lighting for all connected and supported devices.
-    This function will also stop any effect currently going on the connected devices. Passing a name into this
-    function will make the integration show up with a given custom name. The name is set only once, the first
-    time this function or logi_led_init() is called.
-    :param name: The referred name for this integration to show u as
-    :return: result
-    """
-    if LED_DLL:
-        logiledinitwithname = LED_DLL['LogiLedInitWithName']
-        logiledinitwithname.restype = c_bool
-        logiledinitwithname.argtypes = (c_wchar_p,)
-        return logiledinitwithname(name)
-    return False
-
-
-def logi_led_set_target_device(target_device: int) -> bool:
-    """
-    The function sets the target device type for future calls.
-
-    The default target device is LOGI_DEVICETYPE_ALL, therefore, if no call is made to LogiLedSetTargetDevice
-    the SDK will apply any function to all the connected devices.
-    :param target_device: one or a combination of the following values:
-                          LOGI_DEVICETYPE_MONOCHROME, LOGI_DEVICETYPE_RGB, LOGI_DEVICETYPE_ALL
-    :return: result
-    """
-    if LED_DLL:
-        logiledsettargetdevice = LED_DLL['LogiLedSetTargetDevice']
-        logiledsettargetdevice.restype = c_bool
-        logiledsettargetdevice.argtypes = (c_int,)
-        return logiledsettargetdevice(target_device)
-    return False
-
-
-def logi_led_save_current_lighting() -> bool:
-    """
-    The function saves the current lighting so that it can be restored after a temporary effect is finished.
-
-    For example if flashing a red warning sign for a few seconds, you would call the logi_led_save_current_lighting()
-    function just before starting the warning effect.
-    :return: result
-    """
-    if LED_DLL:
-        logiledsavecurrentlighting = LED_DLL['LogiLedSaveCurrentLighting']
-        logiledsavecurrentlighting.restype = c_bool
-        return logiledsavecurrentlighting()
-    return False
-
-
-def logi_led_restore_lighting() -> bool:
-    """
-    The function restores the last saved lighting.
-
-    It should be called after a temporary effect is finished.
-    For example if flashing a red warning sign for a few seconds, you would call this function right
-    after the warning effect is finished.
-    :return: result
-    """
-    if LED_DLL:
-        logiledrestorecurrentlighting = LED_DLL['LogiLedRestoreLighting']
-        logiledrestorecurrentlighting.restype = c_bool
-        return logiledrestorecurrentlighting()
-    return False
-
-
-def logi_led_set_lighting(rgb: Tuple[int, int, int]) -> bool:
-    """
-    The function sets the lighting on connected and supported devices.
-
-    Do not call this function immediately after logi_led_init(). Instead of leave a little of time after logi_led_init().
-    For devices that only support a single color, the highest percentage value given of the three colors will
-    define the intensity. For monochrome device, Logitech Gaming Software will reduce
-    proportionally the value of the highest color, according to the user hardware brightness setting.
-
-    :param rgb: tuple with integer values range 0 to 100 as amount of red, green, blue
-    :return: result
-    """
-    if LED_DLL:
-        logiledsetlighting = LED_DLL['LogiLedSetLighting']
-        logiledsetlighting.restype = c_bool
-        logiledsetlighting.argtypes = (c_int, c_int, c_int)
-        return logiledsetlighting(*rgb)
-    return False
-
-
-def logi_led_flash_lighting(rgb: Tuple[int, int, int], duration: int, interval: int) -> bool:
-    """
-    The function saves the current lighting, plays the flashing effect on the targeted devices.
-
-    Finally, restores the saved lighting.
-    :param rgb: tuple with integer values range 0 to 100 as amount of red, green, blue
-    :param duration: duration of the effect in milliseconds this parameter can be set to LOGI_LED_DURATION_INFINITE
-                     to make the effect run until sto ed through logi_led_stop_effects()
-    :param interval: duration of the flashing interval in milliseconds
-    :return: result
-    """
-    if LED_DLL:
-        logiledflashlighting = LED_DLL['LogiLedFlashLighting']
-        logiledflashlighting.restype = c_bool
-        logiledflashlighting.argtypes = (c_int, c_int, c_int, c_int, c_int)
-        return logiledflashlighting(*rgb, duration, interval)
-    return False
-
-
-def logi_led_pulse_lighting(rgb: Tuple[int, int, int], duration: int, interval: int) -> bool:
-    """
-    The function saves the current lighting, plays the pulsing effect on the targeted devices.
-
-    Finally, restores the saved lighting.
-    :param rgb: tuple with integer values range 0 to 100 as amount of red, green, blue
-    :param duration: duration of the effect in milliseconds this parameter can be set to LOGI_LED_DURATION_INFINITE
-                     to make the effect run until sto ed through logi_led_stop_effects()
-    :param interval: duration of the flashing interval in milliseconds
-    :return: result
-    """
-    if LED_DLL:
-        logiledpulselighting = LED_DLL['LogiLedPulseLighting']
-        logiledpulselighting.restype = c_bool
-        logiledpulselighting.argtypes = (c_int, c_int, c_int, c_int, c_int)
-        return logiledpulselighting(*rgb, duration, interval)
-    return False
-
-
-def logi_led_stop_effects() -> bool:
-    """
-    The function stops any of the presets effects.
-
-    Started from logi_led_flash_lighting() or logi_led_pulse_lighting().
-    :return: result
-    """
-    if LED_DLL:
-        logiledstopeffects = LED_DLL['LogiLedStopEffects']
-        logiledstopeffects.restype = c_bool
-        return logiledstopeffects()
-    return False
-
-
-def logi_led_shutdown() -> None:
-    """The function restores the last saved lighting and frees memory used by the SDK."""
-    if LED_DLL:
-        logiledshutdown = LED_DLL['LogiLedShutdown']
-        logiledshutdown.restype = c_bool
-        logiledshutdown()
-
-
-def start_led_pulse(rgb: Tuple[int, int, int], duration: int, interval: int, event: Event):
-    """
-    The function start the pulsing red effect in thread on the keyboard.
-
-    :param rgb: tuple with integer values range 0 to 100 as amount of red, green, blue
-    :param duration: duration of the effect in milliseconds this parameter can be set to 0 (zero)
-                     to make the effect run until event is set
-    :param interval: duration of the flashing interval in milliseconds
-    :param event: stop event for infinite loop
-    """
-    LOG.debug('Start LED thread')
-    logi_led_init()
-    sleep(0.05)
-    logi_led_set_target_device(LOGI_DEVICETYPE_ALL)
-    sleep_time = duration + 0.2
-    logi_led_pulse_lighting(rgb, duration, interval)
-    sleep(sleep_time)
-    while not event.is_set():
-        sleep(0.2)
-    logi_led_shutdown()
-    LOG.debug('Stop LED thread')
+from ctypes import c_bool, c_wchar_p, c_int
+from logging import getLogger
+from threading import Event
+from time import sleep
+from typing import Tuple
+
+from dcspy.sdk import load_dll
+
+LOG = getLogger(__name__)
+
+LOGI_LED_DURATION_INFINITE = 0
+LOGI_DEVICETYPE_MONOCHROME = 1
+LOGI_DEVICETYPE_RGB = 2
+LOGI_DEVICETYPE_ALL = LOGI_DEVICETYPE_MONOCHROME | LOGI_DEVICETYPE_RGB
+
+LED_DLL = load_dll('LED')
+
+
+def logi_led_init() -> bool:
+    """
+    The function makes sure there isn't already another instance running and then makes necessary initializations.
+
+    It saves the current lighting for all connected and supported devices. This function will also stop any effect
+    currently going on the connected devices.
+    :return: result
+    """
+    if LED_DLL:
+        logiledinit = LED_DLL['LogiLedInit']
+        logiledinit.restype = c_bool
+        return logiledinit()
+    return False
+
+
+def logi_led_init_with_name(name: str) -> bool:
+    """
+    The function makes sure there isn't already another instance running and then makes necessary initializations.
+
+    It saves the current lighting for all connected and supported devices.
+    This function will also stop any effect currently going on the connected devices. Passing a name into this
+    function will make the integration show up with a given custom name. The name is set only once, the first
+    time this function or logi_led_init() is called.
+    :param name: The referred name for this integration to show u as
+    :return: result
+    """
+    if LED_DLL:
+        logiledinitwithname = LED_DLL['LogiLedInitWithName']
+        logiledinitwithname.restype = c_bool
+        logiledinitwithname.argtypes = (c_wchar_p,)
+        return logiledinitwithname(name)
+    return False
+
+
+def logi_led_set_target_device(target_device: int) -> bool:
+    """
+    The function sets the target device type for future calls.
+
+    The default target device is LOGI_DEVICETYPE_ALL, therefore, if no call is made to LogiLedSetTargetDevice
+    the SDK will apply any function to all the connected devices.
+    :param target_device: one or a combination of the following values:
+                          LOGI_DEVICETYPE_MONOCHROME, LOGI_DEVICETYPE_RGB, LOGI_DEVICETYPE_ALL
+    :return: result
+    """
+    if LED_DLL:
+        logiledsettargetdevice = LED_DLL['LogiLedSetTargetDevice']
+        logiledsettargetdevice.restype = c_bool
+        logiledsettargetdevice.argtypes = (c_int,)
+        return logiledsettargetdevice(target_device)
+    return False
+
+
+def logi_led_save_current_lighting() -> bool:
+    """
+    The function saves the current lighting so that it can be restored after a temporary effect is finished.
+
+    For example if flashing a red warning sign for a few seconds, you would call the logi_led_save_current_lighting()
+    function just before starting the warning effect.
+    :return: result
+    """
+    if LED_DLL:
+        logiledsavecurrentlighting = LED_DLL['LogiLedSaveCurrentLighting']
+        logiledsavecurrentlighting.restype = c_bool
+        return logiledsavecurrentlighting()
+    return False
+
+
+def logi_led_restore_lighting() -> bool:
+    """
+    The function restores the last saved lighting.
+
+    It should be called after a temporary effect is finished.
+    For example if flashing a red warning sign for a few seconds, you would call this function right
+    after the warning effect is finished.
+    :return: result
+    """
+    if LED_DLL:
+        logiledrestorecurrentlighting = LED_DLL['LogiLedRestoreLighting']
+        logiledrestorecurrentlighting.restype = c_bool
+        return logiledrestorecurrentlighting()
+    return False
+
+
+def logi_led_set_lighting(rgb: Tuple[int, int, int]) -> bool:
+    """
+    The function sets the lighting on connected and supported devices.
+
+    Do not call this function immediately after logi_led_init(). Instead of leave a little of time after logi_led_init().
+    For devices that only support a single color, the highest percentage value given of the three colors will
+    define the intensity. For monochrome device, Logitech Gaming Software will reduce
+    proportionally the value of the highest color, according to the user hardware brightness setting.
+
+    :param rgb: tuple with integer values range 0 to 100 as amount of red, green, blue
+    :return: result
+    """
+    if LED_DLL:
+        logiledsetlighting = LED_DLL['LogiLedSetLighting']
+        logiledsetlighting.restype = c_bool
+        logiledsetlighting.argtypes = (c_int, c_int, c_int)
+        return logiledsetlighting(*rgb)
+    return False
+
+
+def logi_led_flash_lighting(rgb: Tuple[int, int, int], duration: int, interval: int) -> bool:
+    """
+    The function saves the current lighting, plays the flashing effect on the targeted devices.
+
+    Finally, restores the saved lighting.
+    :param rgb: tuple with integer values range 0 to 100 as amount of red, green, blue
+    :param duration: duration of the effect in milliseconds this parameter can be set to LOGI_LED_DURATION_INFINITE
+                     to make the effect run until sto ed through logi_led_stop_effects()
+    :param interval: duration of the flashing interval in milliseconds
+    :return: result
+    """
+    if LED_DLL:
+        logiledflashlighting = LED_DLL['LogiLedFlashLighting']
+        logiledflashlighting.restype = c_bool
+        logiledflashlighting.argtypes = (c_int, c_int, c_int, c_int, c_int)
+        return logiledflashlighting(*rgb, duration, interval)
+    return False
+
+
+def logi_led_pulse_lighting(rgb: Tuple[int, int, int], duration: int, interval: int) -> bool:
+    """
+    The function saves the current lighting, plays the pulsing effect on the targeted devices.
+
+    Finally, restores the saved lighting.
+    :param rgb: tuple with integer values range 0 to 100 as amount of red, green, blue
+    :param duration: duration of the effect in milliseconds this parameter can be set to LOGI_LED_DURATION_INFINITE
+                     to make the effect run until sto ed through logi_led_stop_effects()
+    :param interval: duration of the flashing interval in milliseconds
+    :return: result
+    """
+    if LED_DLL:
+        logiledpulselighting = LED_DLL['LogiLedPulseLighting']
+        logiledpulselighting.restype = c_bool
+        logiledpulselighting.argtypes = (c_int, c_int, c_int, c_int, c_int)
+        return logiledpulselighting(*rgb, duration, interval)
+    return False
+
+
+def logi_led_stop_effects() -> bool:
+    """
+    The function stops any of the presets effects.
+
+    Started from logi_led_flash_lighting() or logi_led_pulse_lighting().
+    :return: result
+    """
+    if LED_DLL:
+        logiledstopeffects = LED_DLL['LogiLedStopEffects']
+        logiledstopeffects.restype = c_bool
+        return logiledstopeffects()
+    return False
+
+
+def logi_led_shutdown() -> None:
+    """The function restores the last saved lighting and frees memory used by the SDK."""
+    if LED_DLL:
+        logiledshutdown = LED_DLL['LogiLedShutdown']
+        logiledshutdown.restype = c_bool
+        logiledshutdown()
+
+
+def start_led_pulse(rgb: Tuple[int, int, int], duration: int, interval: int, event: Event):
+    """
+    The function start the pulsing red effect in thread on the keyboard.
+
+    :param rgb: tuple with integer values range 0 to 100 as amount of red, green, blue
+    :param duration: duration of the effect in milliseconds this parameter can be set to 0 (zero)
+                     to make the effect run until event is set
+    :param interval: duration of the flashing interval in milliseconds
+    :param event: stop event for infinite loop
+    """
+    LOG.debug('Start LED thread')
+    logi_led_init()
+    sleep(0.05)
+    logi_led_set_target_device(LOGI_DEVICETYPE_ALL)
+    sleep_time = duration + 0.2
+    logi_led_pulse_lighting(rgb, duration, interval)
+    sleep(sleep_time)
+    while not event.is_set():
+        sleep(0.2)
+    logi_led_shutdown()
+    LOG.debug('Stop LED thread')
```

### Comparing `dcspy-1.9.5/dcspy/starter.py` & `dcspy-2.0.0/dcspy/starter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import socket
-import struct
-from collections import deque
-from importlib import import_module
-from logging import getLogger
-from threading import Event
-from time import time, gmtime
-from typing import Iterator
-
-from dcspy import RECV_ADDR, MULTICAST_IP, config
-from dcspy.dcsbios import ProtocolParser
-from dcspy.logitech import LogitechKeyboard
-from dcspy.utils import get_version_string
-
-LOG = getLogger(__name__)
-LOOP_FLAG = True
-__version__ = '1.9.5'
-
-
-def _handle_connection(logi_keyboard: LogitechKeyboard, parser: ProtocolParser, sock: socket.socket, event: Event) -> None:
-    """
-    Main loop where all the magic is happened.
-
-    :param logi_keyboard: type of Logitech keyboard with LCD
-    :param parser: DCS protocol parser
-    :param sock: multi-cast UDP socket
-    :param event: stop event for main loop
-    """
-    start_time = time()
-    ver_string = get_version_string(repo='emcek/dcspy', current_ver=__version__, check=config['check_ver'])
-    LOG.info('Waiting for DCS connection...')
-    support_banner = _supporters(text='Huge thanks to: Sireyn, Nick Thain, BrotherBloat and others! For support and help! ', width=26)
-    while not event.is_set():
-        try:
-            dcs_bios_resp = sock.recv(2048)
-            for int_byte in dcs_bios_resp:
-                parser.process_byte(int_byte)
-            start_time = time()
-            _load_new_plane_if_detected(logi_keyboard)
-            logi_keyboard.button_handle(sock)
-        except OSError as exp:
-            _sock_err_handler(logi_keyboard, start_time, ver_string, support_banner, exp)
-
-
-def _load_new_plane_if_detected(logi_keyboard: LogitechKeyboard) -> None:
-    """
-    Load instance when new plane detected.
-
-    :param logi_keyboard: type of Logitech keyboard with LCD
-    """
-    global LOOP_FLAG
-    if logi_keyboard.plane_detected:
-        logi_keyboard.load_new_plane()
-        LOOP_FLAG = True
-
-
-def _supporters(text: str, width: int) -> Iterator[str]:
-    """
-    Scroll text with widow width.
-
-    :param text: text to scroll
-    :param width: width of window
-    """
-    queue = deque(text)
-    while True:
-        yield ''.join(queue)[:width]
-        queue.rotate(-1)
-
-
-def _sock_err_handler(logi_keyboard: LogitechKeyboard, start_time: float, ver_string: str, support_iter: Iterator[str], exp: Exception) -> None:
-    """
-    Show basic data when DCS is disconnected.
-
-    :param logi_keyboard: type of Logitech keyboard with LCD
-    :param start_time: time when connection to DCS was lost
-    :param ver_string: current version to show
-    :param support_iter: iterator for banner supporters
-    :param exp: caught exception instance
-    """
-    global LOOP_FLAG
-    if LOOP_FLAG:
-        LOG.debug(f'Main loop socket error: {exp}')
-        LOOP_FLAG = False
-    wait_time = gmtime(time() - start_time)
-    logi_keyboard.display = ['Logitech LCD OK',
-                             f'No data from DCS:   {wait_time.tm_min:02d}:{wait_time.tm_sec:02d}',
-                             f'{next(support_iter)}',
-                             ver_string]
-
-
-def _prepare_socket() -> socket.socket:
-    """
-    Preparing multi-cast UDP socket for DCS-BIOS communication.
-
-    :return: socket object
-    """
-    sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
-    sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-    sock.bind(RECV_ADDR)
-    mreq = struct.pack('=4sl', socket.inet_aton(MULTICAST_IP), socket.INADDR_ANY)
-    sock.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, mreq)
-    sock.settimeout(0.5)
-    return sock
-
-
-def dcspy_run(lcd_type: str, event: Event) -> None:
-    """
-    Real starting point of DCSpy.
-
-    :param lcd_type: LCD handling class as string
-    :param event: stop event for main loop
-    """
-    parser = ProtocolParser()
-    logi_keyboard = getattr(import_module('dcspy.logitech'), lcd_type)(parser)
-    LOG.info(f'Loading: {str(logi_keyboard)}')
-    LOG.debug(f'Loading: {repr(logi_keyboard)}')
-    dcs_sock = _prepare_socket()
-    _handle_connection(logi_keyboard, parser, dcs_sock, event)
-    dcs_sock.close()
-    LOG.info('DCSpy stopped.')
-    logi_keyboard.display = ['Logitech LCD OK', 'DCSpy stopped', '', f'v{__version__}']
+import socket
+import struct
+from collections import deque
+from importlib import import_module
+from logging import getLogger
+from threading import Event
+from time import time, gmtime
+from typing import Iterator
+
+from dcspy import RECV_ADDR, MULTICAST_IP, config
+from dcspy.dcsbios import ProtocolParser
+from dcspy.logitech import LogitechKeyboard
+from dcspy.utils import get_version_string
+
+LOG = getLogger(__name__)
+LOOP_FLAG = True
+__version__ = '2.0.0'
+
+
+def _handle_connection(logi_keyboard: LogitechKeyboard, parser: ProtocolParser, sock: socket.socket, event: Event) -> None:
+    """
+    Main loop where all the magic is happened.
+
+    :param logi_keyboard: type of Logitech keyboard with LCD
+    :param parser: DCS protocol parser
+    :param sock: multi-cast UDP socket
+    :param event: stop event for main loop
+    """
+    start_time = time()
+    ver_string = get_version_string(repo='emcek/dcspy', current_ver=__version__, check=config['check_ver'])
+    LOG.info('Waiting for DCS connection...')
+    support_banner = _supporters(text='Huge thanks to: Sireyn, Nick Thain, BrotherBloat and others! For support and help! ', width=26)
+    while not event.is_set():
+        try:
+            dcs_bios_resp = sock.recv(2048)
+            for int_byte in dcs_bios_resp:
+                parser.process_byte(int_byte)
+            start_time = time()
+            _load_new_plane_if_detected(logi_keyboard)
+            logi_keyboard.button_handle(sock)
+        except OSError as exp:
+            _sock_err_handler(logi_keyboard, start_time, ver_string, support_banner, exp)
+
+
+def _load_new_plane_if_detected(logi_keyboard: LogitechKeyboard) -> None:
+    """
+    Load instance when new plane detected.
+
+    :param logi_keyboard: type of Logitech keyboard with LCD
+    """
+    global LOOP_FLAG
+    if logi_keyboard.plane_detected:
+        logi_keyboard.load_new_plane()
+        LOOP_FLAG = True
+
+
+def _supporters(text: str, width: int) -> Iterator[str]:
+    """
+    Scroll text with widow width.
+
+    :param text: text to scroll
+    :param width: width of window
+    """
+    queue = deque(text)
+    while True:
+        yield ''.join(queue)[:width]
+        queue.rotate(-1)
+
+
+def _sock_err_handler(logi_keyboard: LogitechKeyboard, start_time: float, ver_string: str, support_iter: Iterator[str], exp: Exception) -> None:
+    """
+    Show basic data when DCS is disconnected.
+
+    :param logi_keyboard: type of Logitech keyboard with LCD
+    :param start_time: time when connection to DCS was lost
+    :param ver_string: current version to show
+    :param support_iter: iterator for banner supporters
+    :param exp: caught exception instance
+    """
+    global LOOP_FLAG
+    if LOOP_FLAG:
+        LOG.debug(f'Main loop socket error: {exp}')
+        LOOP_FLAG = False
+    wait_time = gmtime(time() - start_time)
+    logi_keyboard.display = ['Logitech LCD OK',
+                             f'No data from DCS:   {wait_time.tm_min:02d}:{wait_time.tm_sec:02d}',
+                             f'{next(support_iter)}',
+                             ver_string]
+
+
+def _prepare_socket() -> socket.socket:
+    """
+    Preparing multi-cast UDP socket for DCS-BIOS communication.
+
+    :return: socket object
+    """
+    sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
+    sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+    sock.bind(RECV_ADDR)
+    mreq = struct.pack('=4sl', socket.inet_aton(MULTICAST_IP), socket.INADDR_ANY)
+    sock.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, mreq)
+    sock.settimeout(0.5)
+    return sock
+
+
+def dcspy_run(lcd_type: str, event: Event) -> None:
+    """
+    Real starting point of DCSpy.
+
+    :param lcd_type: LCD handling class as string
+    :param event: stop event for main loop
+    """
+    parser = ProtocolParser()
+    logi_keyboard = getattr(import_module('dcspy.logitech'), lcd_type)(parser)
+    LOG.info(f'Loading: {str(logi_keyboard)}')
+    LOG.debug(f'Loading: {repr(logi_keyboard)}')
+    dcs_sock = _prepare_socket()
+    _handle_connection(logi_keyboard, parser, dcs_sock, event)
+    dcs_sock.close()
+    LOG.info('DCSpy stopped.')
+    logi_keyboard.display = ['Logitech LCD OK', 'DCSpy stopped', '', f'v{__version__}']
```

### Comparing `dcspy-1.9.5/dcspy.egg-info/PKG-INFO` & `dcspy-2.0.0/dcspy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,316 +1,330 @@
-Metadata-Version: 2.1
-Name: dcspy
-Version: 1.9.5
-Summary: Integrating DCS (Digital Combat Simulator) planes with Logitech G13/G15/G510/G19 LCD
-Home-page: https://github.com/emcek/dcspy
-Author: Michal Plichta
-Maintainer: Michal Plichta
-License: MIT
-Project-URL: Bug Reports, https://github.com/emcek/dcspy/issues
-Project-URL: Source, https://github.com/emcek/dcspy
-Keywords: logitech,logitech-sdk,logitech-keyboards,logitech-gaming,logitech-gaming-keyboard,dcs-world,dcs,g13,g15,g510,g19
-Platform: win32
-Platform: nt
-Platform: Windows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Games/Entertainment :: Simulation
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Hardware
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE.md
-
-[![image](https://img.shields.io/badge/pypi-v1.9.5-blue.svg)](https://pypi.org/project/dcspy/)
-[![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
-[![License](https://img.shields.io/badge/Licence-MIT-blue.svg)](./LICENSE.md)
-[![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
-[![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
-[![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
-[![Discord](https://img.shields.io/discord/672486999516774442?label=Discord&logo=discord&logoColor=lightblue)](https://discord.gg/SP5Yjx3)
-[![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://github.com/emcek/dcspy)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/emcek/dcspy/master.svg)](https://results.pre-commit.ci/latest/github/emcek/dcspy/master)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=emcek_dcspy&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=emcek_dcspy)
-[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6056/badge)](https://bestpractices.coreinfrastructure.org/projects/6056)
-[![Downloads](https://pepy.tech/badge/dcspy)](https://pepy.tech/project/dcspy)
-[![Rate this package](https://badges.openbase.com/python/rating/dcspy.svg?token=AZCVj1Hdbl6cC3I/gkVpgsigp22LtCOR0sB8lcODY9Y=)](https://openbase.com/python/dcspy?utm_source=embedded&amp;utm_medium=badge&amp;utm_campaign=rate-badge)
-
-![dcspylogo](https://i.imgur.com/eqqrPB8.jpg)
-## DCSpy
-DCSpy is able to pull information from DCS aircraft and display on Logitech G-series keyboards LCD.
-It supports:
-* Logitech device with 160x43 px (4 lines) monochrome LCD - **G13**, **G15 (v1 and v2)** and **G510**
-* Logitech device with 320x240 px (8 lines) full RGBA LCD - **G19**
-
-See more information on [Wiki](https://github.com/emcek/dcspy/wiki) page.
-
-## Sponsored by Jetbrains Open Source Support Program
-[![logo](https://resources.jetbrains.com/storage/products/company/brand/logos/PyCharm.svg)](https://jb.gg/OpenSourceSupport)
-[![logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.svg)](https://jb.gg/OpenSourceSupport)
-
-## Aircraft and instruments
-* F/A-18C Hornet UFC - Up Front Controller
-* F-16C Viper DED - Data Entry Display
-* Ka-50 Black Shark II and III - PVI-800 and autopilot channels
-* Mi-8MTV2 Hip - autopilot channels and Radios information
-* Mi-24P Hind - Autopilot channels and modes and Radios information
-* A-10C Warthog and A-10C II Tank Killer - Radio frequency information
-* F-14A and F-14B Tomcat - basic support for RIO CAP
-* AV-8B Night Attack Harrier - Up Front Controller and Option Display Unit
-* AH-64D Apache - Enhanced Up Front Display
-* more to come....
-
-## Requirements
-* [Python 3.11](https://www.python.org/downloads/) but 3.7+ (with tcl/tk support, see [installation](https://github.com/emcek/dcspy/wiki/installation)) should be fine, please choose Windows x86-64 version, file should be python-3.11.1-amd64.exe.
-* [Logitech Gaming Software 9.04.49](https://support.logitech.com/software/lgs)
-* [DCS-BIOS 0.7.47](https://github.com/DCSFlightpanels/dcs-bios/releases/latest) (or newer)
-* DCS World: [2.8.2.35759](https://www.digitalcombatsimulator.com/en/news/changelog/openbeta/2.8.2.35759/) Open Beta
-
-**Notes:**
-* If you upgrade DCSpy from 1.5.1 or older you can safely remove Logitech LCD SDK from `C:\Program Files\Logitech Gaming Software\LCDSDK_8.57.148`. Since DCSpy version 1.6.0 use built-in SDK in LGS (Logitech Gaming Software).
-
-## New ideas
-I have lots of plans and new ideas how to improve it internally and form user's perspective, but don't hesitate to contact me. Maybe it will motivate me to implement some new stuff. Please open issue if you find bug or have any crazy idea.
-You are welcome [dcspy Discord](https://discord.gg/SP5Yjx3) server.
-
-## Contributing
-You want contribute, perfect see: [contributing](./CONTRIBUTING.md) guide.
-
-## Credits
-More details [here](https://github.com/emcek/dcspy/wiki/Information#credits).
-
-## 1.9.5
-* Support for **Mi-8MTV2 Magnificent Eight**
-  * Autopilot Channels (Heading, Pitch/Bank and Altitude)
-  * Radios: R868, R828, YADRO1A information
-* Support for **Mi-24P Hind**
-  * Autopilot Channels (Yaw, Roll, Pitch and Altitude)
-  * Autopilot Modes (Hover, Route and Altitude)
-  * Radios: R868, R828, YADRO1I information
-* Add About tab with basic information
-* **F-16C Viper**:
-  * Add spacial font for DED (G19 only)
-  * Clean some extra characters from DED
-* Internal:
-  * force update customtkinter to at least 5.1.0
-
-## 1.8.1
-* Add support for **Ka-50 Black Shark III**
-* Update footer when checking DCS-BIOS version
-* Align with DCS 2.8.1.34667.2 and DCS-BIOS 0.7.47
-* Internal:
-  * add more unit tests
-  * mark some test as DCS-BIOS tests
-
-## 1.8.0
-* Major GUI redesign using `customtkinter` package, which provides new, modern widgets:
-  * Appearance system mode (`Light`, `Dark`)
-  * Three colort theme (`Green`, `Blue` and `Dark Blue`)
-  * All settings are configured from GUI vie widgets
-  * One window for all configuration and buttons
-  * Check version from GUI
-  * Add configuration flag to check for new version during start
-
-## 1.7.5
-* report DCS stable version correctly in logs during start
-* Internal:
-  * rename starting script
-  * remove usage of McCabe
-  * add unit tests
-
-## 1.7.4
-* **AH-64D Apache**
-  * add better support for G19 for PRE mode
-  * update name from `AH64D` to `AH64DBLKII`
-* Show DCS version in logs
-* Fix name of plane for **F-14 Tomcat** depending on model A or B
-* Toggle Start/Stop buttons
-* Do not show warning when plane's name is empty
-* Internal:
-  * improve checking DCS-BIOS data
-  * introduce enum values for parser state
-  * improve CI process - add Python 3.11
-  * force using Pillow 9.3.0
-
-## 1.7.3
-* Align **F-16C Viper** DED and **AH-64D Apache** EUFD with DCS-BIOS 0.7.46 changes
-* Basic support for **F-14A Tomcat**
-
-## 1.7.2
-* **AH-64D Apache**
-  * update name from `AH64DBLKII` to `AH64D`
-  * fix display PRE mode for G19
-  * fix handling buttons
-* Internal:
-  * update unit test for better coverage and more use-cases
-
-## 1.7.1
-* New config settings:
-  * `auto_start` - run DCSpy atomically after start
-  * `verbose` - show more logs in terminal/console window
-* Fixing handling of `dcsbios` settings from `config.yaml`
-* Start and stop buttons can be used several times without closing GUI
-* **F-16C Viper**
-  * replace `*` with inverse white circle character at DED
-  * Fix unhandled buttons for G19 (menu, ok and cancel)
-* G19 and **F/A-18C Hornet**
-  * Push **Menu** and **Cancel** toggle cockpit button down, push it again toggles button up (Integrated Fuel/Engine Indicator - IFEI).
-  * Add handling **Ok** as Attitude Selector Switch, INS/AUTO/STBY
-* Internal:
-  * use Pythonic way using temporary directory
-  * speed-up tests - cache json files instead of downloading from internet
-  * use Enum for LCD type
-  * use Enum for LCD buttons, add to LcdInfo dataclass
-
-## 1.7.0
-* Support for **AH-64D Apache** with 3 modes:
-  * `IDM` - Squeeze and shows radios frequencies (from Radio Area), IDM and RTS rocker are used to scroll down
-  * `WCA` - Enter button display warnings, cautions, and advisories, WCA rocker is used to scroll down
-  * `PRE` - Preset button displays the preset menu for the selected radio, WCA rocker is used to scroll down
-* **F-16C Viper** DED clean-up extra characters
-
-## 1.6.1
-* Update **F-16C Viper** for latest DSC-BIOS (0.7.45)
-* Fresh installation of DCS-BIOS is painless
-* Drop support for Python 3.6
-
-## 1.6.0
-* use fonts in dynamic way - you can customize fonts in `config.yaml` file (see [Configuration](https://github.com/emcek/dcspy#configuration))
-* usage for LCD SDK built-in LGS - no need additional package for usage
-* support for Python 3.10 (use `dataclasses` internally)
-* ability to stop DCSpy from GUI
-* supporters are printed in welcome screen - I'm thrilled with support and help of community!
-
-## 1.5.1
-* alignment for new DCS-BIOS [v0.7.43](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.43)
-
-## 1.5.0
-* Support for **AV-8B N/A Harrier** with:
-  * **UFC** - Up Front Controller
-  * **ODU** - Option Display Unit
-  * **decrease UFC Comm 1 Channel** - G13 1st button or G19 left button
-  * **increase UFC Comm 1 Channel** - G13 2nd button or G19 right button
-  * **decrease UFC Comm 2 Channel** - G13 3rd button or G19 down button
-  * **increase UFC Comm 2 Channel** - G13 4th button or G19 up button
-
-## 1.4.0
-* Configuration editor:
-  * **dcsbios** - set default Logitech keyboard: "G19", "G510", "G15 v1/v2", "G13"
-  * **show_gui** - showing or hiding GUI during start of DCSpy
-  * **dcsbios** - location of DCS-BIOS folder inside user's Saved Games
-* Check and update DCS-BIOS directly from DCSpy
-  * **Check DCS-BIOS** button in **Config** editor
-  * **dcsbios** needs to be set to correct value
-* Basic A-10C Warthog and A-10C II Tank Killer support
-
-## 1.3.0
-* **F-16C Viper** use 4 buttons for IFF
-  * **IFF MASTER Knob** - OFF/STBY/LOW/NORM/EMER
-  * **IFF ENABLE Switch** - M1/M3 /OFF/ M3/MS
-  * **IFF M-4 CODE Switch** - HOLD/ A/B /ZERO
-  * **IFF MODE 4 REPLY Switch** - OUT/A/B
-* Fix alignment of (DCS-BIOS [v0.7.41](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.41)) for **F-14B Tomcat**
-* Internally all data fetch form DCS-BIOS is check against its specification. Sometimes due to changes DCS-BIOS protocol DCSpy couldn't fetch all data i.e. F-16 DED. It shouldn't happened anymore.
-
-## 1.2.3
-* Fix alignment of DED (DCS-BIOS [v0.7.41](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.43)) for **F-16C Viper**
-
-## 1.2.2
-* Fix alignment of DED for **F-16C Viper**
-* Fix position of Integrated Fuel/Engine Indicator (IFEI) for **F/A-18C Hornet** (only G19)
-
-## 1.2.1
-* **F/A-18C Hornet** shows extra Total Internal Fuel (G19 only)
-* Internal refactoring
-
-## 1.2.0
-* Simple Tkinter GUI - to select your Logitech keyboard
-* Support for G19 - Big thanks for **BrotherBloat** who makes this release possible. He spent countless hours to share his G19 and let me troubleshoot remotely.
-* **F/A-18C Hornet** shows Total Fuel instead of Total Internal Fuel
-
-## 1.1.1
-* Basic support for **F-14B Tomcat** RIO CAP (Computer Address Panel):
-  * **CLEAR** - button 1
-  * **S-W** - button 2
-  * **N+E** - button 3
-  * **ENTER** - button 4
-
-## 1.1.0
-* dcspy use now UDP multicast connection do DCS-BIOS, since each TCP connection slightly increases the amount of work that is performed inside of DCS (blocking the rest of the simulation).
-* support for integer data to be fetch from DCS-BIOS - using IntegerBuffer()
-* bios_data in Airplanes instances allow both StringBuffer() and IntegerBuffer()
-* reformat waiting time before DCS connected
-* fix Data Entry Display for F-16C Viper - DCS-BIOS [v0.7.34](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.34) is required
-* **Ka-50 Black Shark** - Autopilot channels show up in LCD
-
-## 1.0.0
-* **Ka-50 Black Shark** data from PVI-800 shows (in similar boxes) on LCD
-* ProtocolParser for DCS-BIOS has new optimized state machine
-  * LCD SDK is re-written from scratch:
-  * low and high level API
-  * auto-loading C library during importing
-  * all API is type annotated and well documented
-  * move loading LCD C library from G13 handler
-*internal:
-  * refactoring and rename internals of G13 handler module
-  * add unit tests
-
-## 0.9.2
-* LCD prints current waiting time to connect to DCS
-* when DCS exit from plane/mission exception is catch and handle correctly
-* lots of internal changes, preparing for new features, most important:
-  * change structure of AircraftHandler, move subscription to DCS-BIOS changes out of planes
-  * update and clear methods move from G13 handler to LCD SDK
-
-## 0.9.1
-* G13 handler have display property to send text to LCD
-* rename starting script to dcspy.exe
-* starting script now show waiting time for DCS connection
-* minor code optimization and refactoring
-
-## 0.9.0
-* based on version [specelUFC v1.12.1](https://github.com/specel/specelUFC/releases/tag/v1.12.1)
-* added basic handling for Ka-50 PVI-800 data are received but not formatted properly
-* F-16C DED should working but not 4 buttons under LCD - I don't have it so it is hard to test
-* G13 handler detect 32/64 bit of Python and load correct version of LCD Logitech C library
-* adding basic logging for debugging - prints on console
-* all defined aircraft are detected and loaded on-the-fly during operation
-* define new plane should be easy just use AircraftHandler as base class
-* Python LCD SDK was clean-up
-* other refactorings and code duplication removal
-
-MIT License
-
-Copyright (c) 2020 Michal Plichta
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Metadata-Version: 2.1
+Name: dcspy
+Version: 2.0.0
+Summary: Integrating DCS (Digital Combat Simulator) planes with Logitech G13/G15/G510/G19 LCD
+Home-page: https://github.com/emcek/dcspy
+Author: Michal Plichta
+Maintainer: Michal Plichta
+License: MIT
+Project-URL: Bug Reports, https://github.com/emcek/dcspy/issues
+Project-URL: Source, https://github.com/emcek/dcspy
+Keywords: logitech,logitech-sdk,logitech-keyboards,logitech-gaming,logitech-gaming-keyboard,dcs-world,dcs,g13,g15,g510,g19
+Platform: win32
+Platform: nt
+Platform: Windows
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Games/Entertainment :: Simulation
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Hardware
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE.md
+
+[![image](https://img.shields.io/badge/pypi-v2.0.0-blue.svg)](https://pypi.org/project/dcspy/)
+[![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
+[![License](https://img.shields.io/badge/Licence-MIT-blue.svg)](./LICENSE.md)
+[![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
+[![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
+[![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
+[![Discord](https://img.shields.io/discord/672486999516774442?label=Discord&logo=discord&logoColor=lightblue)](https://discord.gg/SP5Yjx3)
+[![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://github.com/emcek/dcspy)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/emcek/dcspy/master.svg)](https://results.pre-commit.ci/latest/github/emcek/dcspy/master)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=emcek_dcspy&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=emcek_dcspy)
+[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6056/badge)](https://bestpractices.coreinfrastructure.org/projects/6056)
+[![Downloads](https://pepy.tech/badge/dcspy)](https://pepy.tech/project/dcspy)
+[![Rate this package](https://badges.openbase.com/python/rating/dcspy.svg?token=AZCVj1Hdbl6cC3I/gkVpgsigp22LtCOR0sB8lcODY9Y=)](https://openbase.com/python/dcspy?utm_source=embedded&amp;utm_medium=badge&amp;utm_campaign=rate-badge)
+
+![dcspylogo](https://i.imgur.com/eqqrPB8.jpg)
+## DCSpy
+DCSpy is able to pull information from DCS aircraft and display on Logitech G-series keyboards LCD.
+It supports:
+* Logitech device with 160x43 px (4 lines) monochrome LCD - **G13**, **G15 (v1 and v2)** and **G510**
+* Logitech device with 320x240 px (8 lines) full RGBA LCD - **G19**
+
+See more information on [Wiki](https://github.com/emcek/dcspy/wiki) page.
+
+## Sponsored by Jetbrains Open Source Support Program
+[![logo](https://resources.jetbrains.com/storage/products/company/brand/logos/PyCharm.svg)](https://jb.gg/OpenSourceSupport)
+[![logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.svg)](https://jb.gg/OpenSourceSupport)
+
+## Aircraft and instruments
+* F/A-18C Hornet UFC - Up Front Controller
+* F-16C Viper DED - Data Entry Display
+* Ka-50 Black Shark II and III - PVI-800 and autopilot channels
+* Mi-8MTV2 Hip - autopilot channels and Radios information
+* Mi-24P Hind - Autopilot channels and modes and Radios information
+* A-10C Warthog and A-10C II Tank Killer - Radio frequency information
+* F-14A and F-14B Tomcat - basic support for RIO CAP
+* AV-8B Night Attack Harrier - Up Front Controller and Option Display Unit
+* AH-64D Apache - Enhanced Up Front Display
+* more to come....
+
+## Requirements
+* [Logitech Gaming Software 9.04.49](https://support.logitech.com/software/lgs)
+* [DCS-BIOS 0.7.48](https://github.com/DCSFlightpanels/dcs-bios/releases/latest) or newer (can be installed directly from DCSpy)
+* DCS World: [2.8.4.39731](https://www.digitalcombatsimulator.com/en/news/changelog/openbeta/2.8.4.39731/) Open Beta (any release 2.8.* should work)
+* (optional) [Python 3.11](https://www.python.org/downloads/) but 3.7+ should be fine (with tcl/tk support, see [installation](https://github.com/emcek/dcspy/wiki/installation))
+
+**Notes:**
+* If you upgrade DCSpy from 1.5.1 or older you can safely remove Logitech LCD SDK from `C:\Program Files\Logitech Gaming Software\LCDSDK_8.57.148`. Since DCSpy version 1.6.0 use built-in SDK in LGS (Logitech Gaming Software).
+
+## New ideas
+I have lots of plans and new ideas how to improve it internally and form user's perspective, but don't hesitate to contact me. Maybe it will motivate me to implement some new stuff. Please open issue if you find bug or have any crazy idea.
+You are welcome [dcspy Discord](https://discord.gg/SP5Yjx3) server.
+
+## Contributing
+You want contribute, perfect see: [contributing](./CONTRIBUTING.md) guide.
+
+## Credits
+More details [here](https://github.com/emcek/dcspy/wiki/Information#credits).
+
+## 2.0.0
+* Allow use/update [live DCS-BIOS](https://github.com/emcek/dcspy/wiki/Information#live-dcs-bios) directly from GitHub (master branch)
+* Allow run DCSpy without console
+* Auto [screenshot of LCD](https://github.com/emcek/dcspy/wiki/Usage#advanced) during operation
+* Auto save change options from GUI
+* Fix problem when DCS-BIOS is empty or drive letter not exists
+* Generate [standalone version](https://github.com/emcek/dcspy/wiki/Installation#single-file-download-new-way) with PyInstaller
+* Save configuration in user local directory (preserved between updates)
+* Internal:
+  * improve type checking
+  * verbose setting will impact both console and file logs
+  * use pathlib for path manipulation
+  * improve CI/CD process
+
+## 1.9.5
+* Support for **Mi-8MTV2 Magnificent Eight**
+  * Autopilot Channels (Heading, Pitch/Bank and Altitude)
+  * Radios: R868, R828, YADRO1A information
+* Support for **Mi-24P Hind**
+  * Autopilot Channels (Yaw, Roll, Pitch and Altitude)
+  * Autopilot Modes (Hover, Route and Altitude)
+  * Radios: R868, R828, YADRO1I information
+* Add About tab with basic information
+* **F-16C Viper**:
+  * Add spacial font for DED (G19 only)
+  * Clean some extra characters from DED
+* Internal:
+  * force update customtkinter to at least 5.1.0
+
+## 1.8.1
+* Add support for **Ka-50 Black Shark III**
+* Update footer when checking DCS-BIOS version
+* Align with DCS 2.8.1.34667.2 and DCS-BIOS 0.7.47
+* Internal:
+  * add more unit tests
+  * mark some test as DCS-BIOS tests
+
+## 1.8.0
+* Major GUI redesign using `customtkinter` package, which provides new, modern widgets:
+  * Appearance system mode (`Light`, `Dark`)
+  * Three colort theme (`Green`, `Blue` and `Dark Blue`)
+  * All settings are configured from GUI vie widgets
+  * One window for all configuration and buttons
+  * Check version from GUI
+  * Add configuration flag to check for new version during start
+
+## 1.7.5
+* report DCS stable version correctly in logs during start
+* Internal:
+  * rename starting script
+  * remove usage of McCabe
+  * add unit tests
+
+## 1.7.4
+* **AH-64D Apache**
+  * add better support for G19 for PRE mode
+  * update name from `AH64D` to `AH64DBLKII`
+* Show DCS version in logs
+* Fix name of plane for **F-14 Tomcat** depending on model A or B
+* Toggle Start/Stop buttons
+* Do not show warning when plane's name is empty
+* Internal:
+  * improve checking DCS-BIOS data
+  * introduce enum values for parser state
+  * improve CI process - add Python 3.11
+  * force using Pillow 9.3.0
+
+## 1.7.3
+* Align **F-16C Viper** DED and **AH-64D Apache** EUFD with DCS-BIOS 0.7.46 changes
+* Basic support for **F-14A Tomcat**
+
+## 1.7.2
+* **AH-64D Apache**
+  * update name from `AH64DBLKII` to `AH64D`
+  * fix display PRE mode for G19
+  * fix handling buttons
+* Internal:
+  * update unit test for better coverage and more use-cases
+
+## 1.7.1
+* New config settings:
+  * `auto_start` - run DCSpy atomically after start
+  * `verbose` - show more logs in terminal/console window
+* Fixing handling of `dcsbios` settings from `config.yaml`
+* Start and stop buttons can be used several times without closing GUI
+* **F-16C Viper**
+  * replace `*` with inverse white circle character at DED
+  * Fix unhandled buttons for G19 (menu, ok and cancel)
+* G19 and **F/A-18C Hornet**
+  * Push **Menu** and **Cancel** toggle cockpit button down, push it again toggles button up (Integrated Fuel/Engine Indicator - IFEI).
+  * Add handling **Ok** as Attitude Selector Switch, INS/AUTO/STBY
+* Internal:
+  * use Pythonic way using temporary directory
+  * speed-up tests - cache json files instead of downloading from internet
+  * use Enum for LCD type
+  * use Enum for LCD buttons, add to LcdInfo dataclass
+
+## 1.7.0
+* Support for **AH-64D Apache** with 3 modes:
+  * `IDM` - Squeeze and shows radios frequencies (from Radio Area), IDM and RTS rocker are used to scroll down
+  * `WCA` - Enter button display warnings, cautions, and advisories, WCA rocker is used to scroll down
+  * `PRE` - Preset button displays the preset menu for the selected radio, WCA rocker is used to scroll down
+* **F-16C Viper** DED clean-up extra characters
+
+## 1.6.1
+* Update **F-16C Viper** for latest DSC-BIOS (0.7.45)
+* Fresh installation of DCS-BIOS is painless
+* Drop support for Python 3.6
+
+## 1.6.0
+* use fonts in dynamic way - you can customize fonts in `config.yaml` file (see [Configuration](https://github.com/emcek/dcspy#configuration))
+* usage for LCD SDK built-in LGS - no need additional package for usage
+* support for Python 3.10 (use `dataclasses` internally)
+* ability to stop DCSpy from GUI
+* supporters are printed in welcome screen - I'm thrilled with support and help of community!
+
+## 1.5.1
+* alignment for new DCS-BIOS [v0.7.43](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.43)
+
+## 1.5.0
+* Support for **AV-8B N/A Harrier** with:
+  * **UFC** - Up Front Controller
+  * **ODU** - Option Display Unit
+  * **decrease UFC Comm 1 Channel** - G13 1st button or G19 left button
+  * **increase UFC Comm 1 Channel** - G13 2nd button or G19 right button
+  * **decrease UFC Comm 2 Channel** - G13 3rd button or G19 down button
+  * **increase UFC Comm 2 Channel** - G13 4th button or G19 up button
+
+## 1.4.0
+* Configuration editor:
+  * **dcsbios** - set default Logitech keyboard: "G19", "G510", "G15 v1/v2", "G13"
+  * **show_gui** - showing or hiding GUI during start of DCSpy
+  * **dcsbios** - location of DCS-BIOS folder inside user's Saved Games
+* Check and update DCS-BIOS directly from DCSpy
+  * **Check DCS-BIOS** button in **Config** editor
+  * **dcsbios** needs to be set to correct value
+* Basic A-10C Warthog and A-10C II Tank Killer support
+
+## 1.3.0
+* **F-16C Viper** use 4 buttons for IFF
+  * **IFF MASTER Knob** - OFF/STBY/LOW/NORM/EMER
+  * **IFF ENABLE Switch** - M1/M3 /OFF/ M3/MS
+  * **IFF M-4 CODE Switch** - HOLD/ A/B /ZERO
+  * **IFF MODE 4 REPLY Switch** - OUT/A/B
+* Fix alignment of (DCS-BIOS [v0.7.41](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.41)) for **F-14B Tomcat**
+* Internally all data fetch form DCS-BIOS is check against its specification. Sometimes due to changes DCS-BIOS protocol DCSpy couldn't fetch all data i.e. F-16 DED. It shouldn't happened anymore.
+
+## 1.2.3
+* Fix alignment of DED (DCS-BIOS [v0.7.41](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.43)) for **F-16C Viper**
+
+## 1.2.2
+* Fix alignment of DED for **F-16C Viper**
+* Fix position of Integrated Fuel/Engine Indicator (IFEI) for **F/A-18C Hornet** (only G19)
+
+## 1.2.1
+* **F/A-18C Hornet** shows extra Total Internal Fuel (G19 only)
+* Internal refactoring
+
+## 1.2.0
+* Simple Tkinter GUI - to select your Logitech keyboard
+* Support for G19 - Big thanks for **BrotherBloat** who makes this release possible. He spent countless hours to share his G19 and let me troubleshoot remotely.
+* **F/A-18C Hornet** shows Total Fuel instead of Total Internal Fuel
+
+## 1.1.1
+* Basic support for **F-14B Tomcat** RIO CAP (Computer Address Panel):
+  * **CLEAR** - button 1
+  * **S-W** - button 2
+  * **N+E** - button 3
+  * **ENTER** - button 4
+
+## 1.1.0
+* dcspy use now UDP multicast connection do DCS-BIOS, since each TCP connection slightly increases the amount of work that is performed inside of DCS (blocking the rest of the simulation).
+* support for integer data to be fetch from DCS-BIOS - using IntegerBuffer()
+* bios_data in Airplanes instances allow both StringBuffer() and IntegerBuffer()
+* reformat waiting time before DCS connected
+* fix Data Entry Display for F-16C Viper - DCS-BIOS [v0.7.34](https://github.com/DCSFlightpanels/dcs-bios/releases/tag/v0.7.34) is required
+* **Ka-50 Black Shark** - Autopilot channels show up in LCD
+
+## 1.0.0
+* **Ka-50 Black Shark** data from PVI-800 shows (in similar boxes) on LCD
+* ProtocolParser for DCS-BIOS has new optimized state machine
+  * LCD SDK is re-written from scratch:
+  * low and high level API
+  * auto-loading C library during importing
+  * all API is type annotated and well documented
+  * move loading LCD C library from G13 handler
+*internal:
+  * refactoring and rename internals of G13 handler module
+  * add unit tests
+
+## 0.9.2
+* LCD prints current waiting time to connect to DCS
+* when DCS exit from plane/mission exception is catch and handle correctly
+* lots of internal changes, preparing for new features, most important:
+  * change structure of AircraftHandler, move subscription to DCS-BIOS changes out of planes
+  * update and clear methods move from G13 handler to LCD SDK
+
+## 0.9.1
+* G13 handler have display property to send text to LCD
+* rename starting script to dcspy.exe
+* starting script now show waiting time for DCS connection
+* minor code optimization and refactoring
+
+## 0.9.0
+* based on version [specelUFC v1.12.1](https://github.com/specel/specelUFC/releases/tag/v1.12.1)
+* added basic handling for Ka-50 PVI-800 data are received but not formatted properly
+* F-16C DED should working but not 4 buttons under LCD - I don't have it so it is hard to test
+* G13 handler detect 32/64 bit of Python and load correct version of LCD Logitech C library
+* adding basic logging for debugging - prints on console
+* all defined aircraft are detected and loaded on-the-fly during operation
+* define new plane should be easy just use AircraftHandler as base class
+* Python LCD SDK was clean-up
+* other refactorings and code duplication removal
+
+MIT License
+
+Copyright (c) 2020 Michal Plichta
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dcspy-1.9.5/dcspy.egg-info/SOURCES.txt` & `dcspy-2.0.0/dcspy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+.pre-commit-config.yaml
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE.md
 MANIFEST.in
 README.md
 SECURITY.md
+file_version_info.txt
 pyproject.toml
 requirements.txt
 requirements_test.txt
 setup.cfg
 setup.py
 dcspy/G13.png
 dcspy/G15v1.png
```

### Comparing `dcspy-1.9.5/tests/test_aircraft.py` & `dcspy-2.0.0/tests/test_aircraft.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,472 +1,472 @@
-from os import path
-from sys import platform
-from unittest.mock import patch
-
-import PIL
-from PIL import ImageChops
-from pytest import mark, raises
-
-from dcspy import LcdColor, LcdMono, LcdButton
-from tests.helpers import all_plane_list, set_bios_during_test
-
-resources = path.join(path.dirname(path.abspath(__file__)), 'resources')
-
-
-# <=><=><=><=><=> Base Class <=><=><=><=><=>
-@mark.parametrize('model', all_plane_list)
-def test_check_all_aircraft_inherit_from_correct_base_class(model, lcd_mono):
-    from dcspy import aircraft
-    airplane = getattr(aircraft, model)
-    aircraft_model = airplane(lcd_mono)
-    assert isinstance(aircraft_model, aircraft.Aircraft)
-    assert issubclass(airplane, aircraft.Aircraft)
-
-
-@mark.parametrize('selector, data, value, c_func, effect, lcd', [
-    ('field1', {'addr': 0xdeadbeef, 'len': 16, 'value': ''}, 'val1', 'logi_lcd_mono_set_background', [True], LcdMono),
-    ('field2', {'addr': 0xdeadbeef, 'len': 16, 'value': ''}, 'val2', 'logi_lcd_color_set_background', [False, True], LcdColor),
-])
-def test_aircraft_base_class_set_bios_with_mono_color_lcd(selector, data, value, c_func, effect, lcd, aircraft):
-    from dcspy.sdk import lcd_sdk
-    assert aircraft.bios_data == {}
-    aircraft.bios_data = {selector: data}
-    aircraft.lcd = lcd
-    with patch.object(lcd_sdk, 'logi_lcd_is_connected', side_effect=effect), \
-            patch.object(lcd_sdk, c_func, return_value=True), \
-            patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
-        assert aircraft.bios_data[selector]['value'] == ''
-        assert aircraft.get_bios('none') == ''
-        with raises(NotImplementedError):
-            aircraft.set_bios(selector, value)
-
-
-@mark.parametrize('mode, c_func, lcd', [('1', 'logi_lcd_mono_set_background', LcdMono),
-                                        ('RGBA', 'logi_lcd_color_set_background', LcdColor)])
-def test_aircraft_base_class_prepare_img_with_mono_color_lcd(mode, c_func, lcd, aircraft):
-    from dcspy.sdk import lcd_sdk
-    aircraft.lcd = lcd
-    with patch.object(lcd_sdk, 'logi_lcd_is_connected', return_value=True), \
-            patch.object(lcd_sdk, c_func, return_value=True), \
-            patch.object(lcd_sdk, 'logi_lcd_update', return_value=True), \
-            raises(NotImplementedError):
-        aircraft.prepare_image()
-
-
-# <=><=><=><=><=> Button Requests <=><=><=><=><=>
-@mark.parametrize('plane, button, result', [
-    ('hornet_mono', LcdButton.NONE, '\n'),
-    ('hornet_mono', LcdButton.ONE, 'UFC_COMM1_CHANNEL_SELECT DEC\n'),
-    ('hornet_mono', LcdButton.TWO, 'UFC_COMM1_CHANNEL_SELECT INC\n'),
-    ('hornet_mono', LcdButton.THREE, 'UFC_COMM2_CHANNEL_SELECT DEC\n'),
-    ('hornet_mono', LcdButton.FOUR, 'UFC_COMM2_CHANNEL_SELECT INC\n'),
-    ('hornet_color', LcdButton.NONE, '\n'),
-    ('hornet_color', LcdButton.LEFT, 'UFC_COMM1_CHANNEL_SELECT DEC\n'),
-    ('hornet_color', LcdButton.RIGHT, 'UFC_COMM1_CHANNEL_SELECT INC\n'),
-    ('hornet_color', LcdButton.DOWN, 'UFC_COMM2_CHANNEL_SELECT DEC\n'),
-    ('hornet_color', LcdButton.UP, 'UFC_COMM2_CHANNEL_SELECT INC\n'),
-    ('hornet_color', LcdButton.MENU, 'IFEI_DWN_BTN 1\n'),
-    ('hornet_color', LcdButton.CANCEL, 'IFEI_UP_BTN 1\n'),
-    ('hornet_color', LcdButton.OK, 'HUD_ATT_SW 1\n'),
-    ('harrier_mono', LcdButton.NONE, '\n'),
-    ('harrier_mono', LcdButton.ONE, 'UFC_COM1_SEL -3200\n'),
-    ('harrier_mono', LcdButton.TWO, 'UFC_COM1_SEL 3200\n'),
-    ('harrier_mono', LcdButton.THREE, 'UFC_COM2_SEL -3200\n'),
-    ('harrier_mono', LcdButton.FOUR, 'UFC_COM2_SEL 3200\n'),
-    ('harrier_color', LcdButton.NONE, '\n'),
-    ('harrier_color', LcdButton.LEFT, 'UFC_COM1_SEL -3200\n'),
-    ('harrier_color', LcdButton.RIGHT, 'UFC_COM1_SEL 3200\n'),
-    ('harrier_color', LcdButton.DOWN, 'UFC_COM2_SEL -3200\n'),
-    ('harrier_color', LcdButton.UP, 'UFC_COM2_SEL 3200\n'),
-    ('harrier_color', LcdButton.MENU, '\n'),
-    ('harrier_color', LcdButton.CANCEL, '\n'),
-    ('harrier_color', LcdButton.OK, '\n'),
-    ('shark_mono', LcdButton.NONE, '\n'),
-    ('shark_mono', LcdButton.ONE, 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n'),
-    ('shark_mono', LcdButton.TWO, 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n'),
-    ('shark_mono', LcdButton.THREE, 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n'),
-    ('shark_mono', LcdButton.FOUR, 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'),
-    ('shark_color', LcdButton.NONE, '\n'),
-    ('shark_color', LcdButton.LEFT, 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n'),
-    ('shark_color', LcdButton.RIGHT, 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n'),
-    ('shark_color', LcdButton.DOWN, 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n'),
-    ('shark_color', LcdButton.UP, 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'),
-    ('shark_color', LcdButton.MENU, '\n'),
-    ('shark_color', LcdButton.CANCEL, '\n'),
-    ('shark_color', LcdButton.OK, '\n'),
-    ('shark3_mono', LcdButton.NONE, '\n'),
-    ('shark3_mono', LcdButton.ONE, 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n'),
-    ('shark3_mono', LcdButton.TWO, 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n'),
-    ('shark3_mono', LcdButton.THREE, 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n'),
-    ('shark3_mono', LcdButton.FOUR, 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'),
-    ('shark3_color', LcdButton.NONE, '\n'),
-    ('shark3_color', LcdButton.LEFT, 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n'),
-    ('shark3_color', LcdButton.RIGHT, 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n'),
-    ('shark3_color', LcdButton.DOWN, 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n'),
-    ('shark3_color', LcdButton.UP, 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'),
-    ('shark3_color', LcdButton.MENU, '\n'),
-    ('shark3_color', LcdButton.CANCEL, '\n'),
-    ('shark3_color', LcdButton.OK, '\n'),
-    ('tomcata_mono', LcdButton.NONE, '\n'),
-    ('tomcata_mono', LcdButton.ONE, 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n'),
-    ('tomcata_mono', LcdButton.TWO, 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n'),
-    ('tomcata_mono', LcdButton.THREE, 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n'),
-    ('tomcata_mono', LcdButton.FOUR, 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'),
-    ('tomcata_color', LcdButton.NONE, '\n'),
-    ('tomcata_color', LcdButton.LEFT, 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n'),
-    ('tomcata_color', LcdButton.RIGHT, 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n'),
-    ('tomcata_color', LcdButton.DOWN, 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n'),
-    ('tomcata_color', LcdButton.UP, 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'),
-    ('tomcata_color', LcdButton.MENU, '\n'),
-    ('tomcata_color', LcdButton.CANCEL, '\n'),
-    ('tomcata_color', LcdButton.OK, '\n'),
-    ('tomcatb_mono', LcdButton.NONE, '\n'),
-    ('tomcatb_mono', LcdButton.ONE, 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n'),
-    ('tomcatb_mono', LcdButton.TWO, 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n'),
-    ('tomcatb_mono', LcdButton.THREE, 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n'),
-    ('tomcatb_mono', LcdButton.FOUR, 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'),
-    ('tomcatb_color', LcdButton.NONE, '\n'),
-    ('tomcatb_color', LcdButton.LEFT, 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n'),
-    ('tomcatb_color', LcdButton.RIGHT, 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n'),
-    ('tomcatb_color', LcdButton.DOWN, 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n'),
-    ('tomcatb_color', LcdButton.UP, 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'),
-    ('tomcatb_color', LcdButton.MENU, '\n'),
-    ('tomcatb_color', LcdButton.CANCEL, '\n'),
-    ('tomcatb_color', LcdButton.OK, '\n'),
-    ('viper_mono', LcdButton.NONE, '\n'),
-    ('viper_mono', LcdButton.ONE, 'IFF_MASTER_KNB 1\n'),
-    ('viper_mono', LcdButton.TWO, 'IFF_ENABLE_SW 1\n'),
-    ('viper_mono', LcdButton.THREE, 'IFF_M4_CODE_SW 1\n'),
-    ('viper_mono', LcdButton.FOUR, 'IFF_M4_REPLY_SW 1\n'),
-    ('viper_color', LcdButton.NONE, '\n'),
-    ('viper_color', LcdButton.LEFT, 'IFF_MASTER_KNB 1\n'),
-    ('viper_color', LcdButton.RIGHT, 'IFF_ENABLE_SW 1\n'),
-    ('viper_color', LcdButton.DOWN, 'IFF_M4_CODE_SW 1\n'),
-    ('viper_color', LcdButton.UP, 'IFF_M4_REPLY_SW 1\n'),
-    ('viper_color', LcdButton.MENU, '\n'),
-    ('viper_color', LcdButton.CANCEL, '\n'),
-    ('viper_color', LcdButton.OK, '\n'),
-    ('apache_mono', LcdButton.NONE, '\n'),
-    ('apache_mono', LcdButton.ONE, 'PLT_EUFD_IDM 0\nPLT_EUFD_IDM 1\n'),
-    ('apache_mono', LcdButton.TWO, 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n'),
-    ('apache_mono', LcdButton.THREE, 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n'),
-    ('apache_mono', LcdButton.FOUR, 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n'),
-])
-def test_button_pressed_for_plane(plane, button, result, request):
-    plane = request.getfixturevalue(plane)
-    assert plane.button_request(button) == result
-
-
-@mark.parametrize('button, result', [
-    (LcdButton.NONE, '\n'),
-    (LcdButton.LEFT, 'PLT_EUFD_WCA 0\nPLT_EUFD_WCA 1\n'),
-    (LcdButton.RIGHT, 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n'),
-    (LcdButton.DOWN, 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n'),
-    (LcdButton.UP, 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n'),
-    (LcdButton.MENU, '\n'),
-    (LcdButton.CANCEL, '\n'),
-    (LcdButton.OK, '\n'),
-])
-def test_button_pressed_for_apache_color(button, result, apache_color):
-    from dcspy.aircraft import ApacheEufdMode
-    apache_color.mode = ApacheEufdMode.WCA
-    assert apache_color.button_request(button) == result
-
-
-@mark.parametrize('plane, btn_name, btn, values', [
-    ('viper_mono', 'IFF_MASTER_KNB', LcdButton.ONE, (1, 2, 3, 4, 3, 2, 1, 0, 1)),
-    ('viper_mono', 'IFF_ENABLE_SW', LcdButton.TWO, (1, 2, 1, 0, 1)),
-    ('viper_mono', 'IFF_M4_CODE_SW', LcdButton.THREE, (1, 2, 1, 0, 1)),
-    ('viper_mono', 'IFF_M4_REPLY_SW', LcdButton.FOUR, (1, 2, 1, 0, 1)),
-    ('viper_color', 'IFF_MASTER_KNB', LcdButton.LEFT, (1, 2, 3, 4, 3, 2, 1, 0, 1)),
-    ('viper_color', 'IFF_ENABLE_SW', LcdButton.RIGHT, (1, 2, 1, 0, 1)),
-    ('viper_color', 'IFF_M4_CODE_SW', LcdButton.DOWN, (1, 2, 1, 0, 1)),
-    ('viper_color', 'IFF_M4_REPLY_SW', LcdButton.UP, (1, 2, 1, 0, 1)),
-    ('hornet_color', 'HUD_ATT_SW', LcdButton.OK, (1, 2, 1, 0, 1)),
-    ('hornet_color', 'IFEI_DWN_BTN', LcdButton.MENU, (1, 0, 1)),
-    ('hornet_color', 'IFEI_UP_BTN', LcdButton.CANCEL, (1, 0, 1)),
-])
-def test_get_next_value_for_cycle_buttons(plane, btn_name, btn, values, request):
-    from itertools import cycle
-    plane = request.getfixturevalue(plane)
-    assert not all([cyc_btn for cyc_btn in plane.cycle_buttons.values()])
-    for val in values:
-        assert plane.button_request(btn) == f'{btn_name} {val}\n'
-    assert isinstance(plane.cycle_buttons[btn_name], cycle)
-
-
-# <=><=><=><=><=> Set BIOS <=><=><=><=><=>
-@mark.parametrize('plane, bios_pairs, result', [
-    ('hornet_mono', [('UFC_SCRATCHPAD_STRING_2_DISPLAY', '~~')], '22'),
-    ('hornet_mono', [('UFC_COMM1_DISPLAY', '``')], '11'),
-    ('hornet_mono', [('IFEI_FUEL_UP', '104T')], '104T'),
-    ('hornet_color', [('UFC_SCRATCHPAD_STRING_1_DISPLAY', '~~')], '22'),
-    ('hornet_color', [('UFC_COMM1_DISPLAY', '``')], '11'),
-    ('hornet_color', [('IFEI_FUEL_UP', '1000T')], '1000T'),
-    ('viper_mono', [('DED_LINE_1', 'a')], '\u2666'),
-    ('viper_mono', [('DED_LINE_2', 'o')], '\u00b0'),
-    ('viper_mono', [('DED_LINE_3', '*')], '\u25d9'),
-    ('viper_mono', [('DED_LINE_5', '\x07')], ''),
-    ('viper_mono', [('DED_LINE_4', '\x10')], ''),
-    ('viper_mono', [('DED_LINE_2', '   @')], '   '),
-    ('viper_color', [('DED_LINE_3', 'a')], '\u0040'),
-    ('viper_color', [('DED_LINE_4', 'o')], '\u005e'),
-    ('viper_color', [('DED_LINE_3', '*')], '\u00d7'),
-    ('viper_color', [('DED_LINE_5', '\xfe')], ''),
-    ('viper_color', [('DED_LINE_1', '\xfc')], ''),
-    ('viper_color', [('DED_LINE_2', '   @')], '   '),
-    ('viper_color', [('DED_LINE_2', '1DEST 2BNGO 3VIP  RINTG  A\x10\x04')], "ÁDEST ÂBNGO ÃVIP  rINTG  "),
-    ('viper_color', [('DED_LINE_3', '4NAV  5MAN  6INS  EDLNK  A\x10\x04')], "ÄNAV  ÅMAN  ÆINS  eDLNK  "),
-    ('viper_color', [('DED_LINE_4', '7CMDS 8MODE 9VRP  0MISC  A\x10\x04')], "ÇCMDS ÈMODE ÉVRP  ÀMISC  "),
-    ('viper_mono', [('DED_LINE_1', '       *      *CMD STRG  \x80@')], '       \u25d9      \u25d9CMD STRG  '),
-    ('viper_mono', [('DED_LINE_2', '1DEST 2BNGO 3VIP  RINTG  A\x10\x04')], '1DEST 2BNGO 3VIP  RINTG  '),
-    ('viper_mono', [('DED_LINE_1', ' MARK *HUD *    26a      @')], ' MARK \u25d9HUD \u25d9    26\u2666      '),
-    ('viper_mono', [('DED_LINE_5', 'M3 :7000 *     *DCPL(9)  \x03\x82')], 'M3 :7000 \u25d9     \u25d9DCPL(9)  '),
-    ('apache_mono', [('PLT_EUFD_LINE8', '~=>VHF*  121.000   -----              121.500   -----   ')], '\u25a0\u2219\u25b8VHF*  121.000   -----              121.500   -----   '),
-    ('apache_mono', [('PLT_EUFD_LINE9', ' <=UHF*  305.000   -----              305.000   -----   ')], ' \u25c2\u2219UHF*  305.000   -----              305.000   -----   '),
-    ('apache_mono', [('PLT_EUFD_LINE10', ' <>FM1*   30.000   -----    NORM       30.000   -----   ')], ' \u25c2\u25b8FM1*   30.000   -----    NORM       30.000   -----   '),
-    ('apache_color', [('PLT_EUFD_LINE11', '[==FM2*   30.000   -----               30.000   -----   ')], '\u25ca\u2219\u2219FM2*   30.000   -----               30.000   -----   '),
-    ('apache_color', [('PLT_EUFD_LINE12', ' ==HF *    2.0000A -----    LOW         2.0000A -----   ')], ' \u2219\u2219HF *    2.0000A -----    LOW         2.0000A -----   '),
-    ('apache_color', [('PLT_EUFD_LINE12', ']==HF *    2.0000A -----    LOW         2.0000A -----   ')], '\u2666\u2219\u2219HF *    2.0000A -----    LOW         2.0000A -----   '),
-])
-def test_set_bios_for_airplane(plane, bios_pairs, result, request):
-    plane = request.getfixturevalue(plane)
-    set_bios_during_test(plane, bios_pairs)
-    assert plane.bios_data[bios_pairs[0][0]]['value'] == result
-
-
-@mark.parametrize('plane, bios_pairs, mode', [
-    ('apache_mono', [('PLT_EUFD_LINE1', 'ENGINE 1 OUT      |AFT FUEL LOW      |TAIL WHL LOCK SEL ')], 'IDM'),
-    ('apache_mono', [('PLT_EUFD_LINE1', '                  |AFT FUEL LOW      |PRESET TUNE VHS ')], 'PRE'),
-    ('apache_color', [('PLT_EUFD_LINE1', '                  |                  |TAIL WHL LOCK SEL ')], 'IDM'),
-    ('apache_color', [('PLT_EUFD_LINE1', '                  |AFT FUEL LOW      |TAIL WHL LOCK SEL ')], 'IDM'),
-    ('apache_color', [('PLT_EUFD_LINE1', 'ENGINE 1 OUT      |AFT FUEL LOW      |PRESET TUNE FM1 ')], 'PRE'),
-])
-def test_mode_switch_idm_pre_for_apache(plane, bios_pairs, mode, request):
-    plane = request.getfixturevalue(plane)
-    set_bios_during_test(plane, bios_pairs)
-    assert plane.mode.name == mode
-
-
-# <=><=><=><=><=> Prepare Image <=><=><=><=><=>
-hornet_bios = [
-    ('UFC_SCRATCHPAD_STRING_1_DISPLAY', '11'),
-    ('UFC_SCRATCHPAD_STRING_2_DISPLAY', '22'),
-    ('UFC_SCRATCHPAD_NUMBER_DISPLAY', '1234567890'),
-    ('UFC_OPTION_DISPLAY_1', '1234'),
-    ('UFC_OPTION_DISPLAY_2', '2345'),
-    ('UFC_OPTION_DISPLAY_3', '3456'),
-    ('UFC_OPTION_DISPLAY_4', '4567'),
-    ('UFC_OPTION_DISPLAY_5', '5678'),
-    ('UFC_COMM1_DISPLAY', '11'),
-    ('UFC_COMM2_DISPLAY', '22'),
-    ('UFC_OPTION_CUEING_1', '1'),
-    ('UFC_OPTION_CUEING_2', '2'),
-    ('UFC_OPTION_CUEING_3', '3'),
-    ('UFC_OPTION_CUEING_4', '4'),
-    ('UFC_OPTION_CUEING_5', '5'),
-    ('IFEI_FUEL_DOWN', '123456'),
-    ('IFEI_FUEL_UP', '234567')
-]
-viper_bios = [
-    ('DED_LINE_1', "  INS  08.0/ 6        1a "),
-    ('DED_LINE_2', "  LAT *N 43o06.2'*       @"),
-    ('DED_LINE_3', "  LNG  E040o34.2'        "),
-    ('DED_LINE_4', " SALT      74FT          "),
-    ('DED_LINE_5', " THDG   25.0o   G/S    0 "),
-]
-shark_bios = [
-    ('PVI_LINE1_APOSTROPHE1', '`'),
-    ('PVI_LINE1_APOSTROPHE2', '`'),
-    ('PVI_LINE1_POINT', '1'),
-    ('PVI_LINE1_SIGN', '-'),
-    ('PVI_LINE1_TEXT', '123456'),
-    ('PVI_LINE2_APOSTROPHE1', '`'),
-    ('PVI_LINE2_APOSTROPHE2', '`'),
-    ('PVI_LINE2_POINT', '2'),
-    ('PVI_LINE2_SIGN', ' '),
-    ('PVI_LINE2_TEXT', '654321'),
-    ('AP_ALT_HOLD_LED', 1),
-    ('AP_BANK_HOLD_LED', 0),
-    ('AP_FD_LED', 1),
-    ('AP_HDG_HOLD_LED', 0),
-    ('AP_PITCH_HOLD_LED', 1)
-]
-hip_bios = [
-    ('LMP_AP_HDG_ON', 1),
-    ('LMP_AP_PITCH_ROLL_ON', 0),
-    ('LMP_AP_HEIGHT_ON', 1),
-    ('R863_CNL_SEL', 9),
-    ('R863_MOD', 1),
-    ('R863_FREQ', "123.525"),
-    ('R828_PRST_CHAN_SEL', 9),
-    ('YADRO1A_FREQ', "09091.9"),
-]
-hind_bios = [
-    ('PLT_R863_CHAN', 9),
-    ('PLT_R863_MODUL', 1),
-    ('PLT_R828_CHAN', 9),
-    ('JADRO_FREQ', "08082.8"),
-    ('PLT_SAU_HOVER_MODE_ON_L', 1),
-    ('PLT_SAU_ROUTE_MODE_ON_L', 0),
-    ('PLT_SAU_ALT_MODE_ON_L', 1),
-    ('PLT_SAU_H_ON_L', 0),
-    ('PLT_SAU_K_ON_L', 0),
-    ('PLT_SAU_T_ON_L', 0),
-    ('PLT_SAU_B_ON_L', 1),
-]
-apache_bios = [
-    ('PLT_EUFD_LINE8', '~<>VHF*  121.000   -----              121.500   -----   '),
-    ('PLT_EUFD_LINE9', ' ==UHF*  305.000   -----              305.000   -----   '),
-    ('PLT_EUFD_LINE10', ' ==FM1*   30.000   -----    NORM       30.000   -----   '),
-    ('PLT_EUFD_LINE11', ' ==FM2*   30.000   -----               30.000   -----   '),
-    ('PLT_EUFD_LINE12', ' ==HF *    2.0000A -----    LOW         2.0000A -----   ')
-]
-warthog_bios = [
-    ('VHFAM_FREQ1', '20'),
-    ('VHFAM_FREQ2', 1),
-    ('VHFAM_FREQ3', 1),
-    ('VHFAM_FREQ4', '30'),
-    ('VHFFM_FREQ1', '40'),
-    ('VHFFM_FREQ2', 2),
-    ('VHFFM_FREQ3', 2),
-    ('VHFFM_FREQ4', '50'),
-    ('UHF_100MHZ_SEL', '5'),
-    ('UHF_10MHZ_SEL', 3),
-    ('UHF_1MHZ_SEL', 2),
-    ('UHF_POINT1MHZ_SEL', 1),
-    ('UHF_POINT25_SEL', '25')
-]
-harrier_bios = [
-    ('UFC_SCRATCHPAD', '123456789012'),
-    ('UFC_COMM1_DISPLAY', '11'),
-    ('UFC_COMM2_DISPLAY', '22'),
-    ('AV8BNA_ODU_1_SELECT', '1'),
-    ('AV8BNA_ODU_1_Text', '1234'),
-    ('AV8BNA_ODU_2_SELECT', '2'),
-    ('AV8BNA_ODU_2_Text', '2345'),
-    ('AV8BNA_ODU_3_SELECT', '3'),
-    ('AV8BNA_ODU_3_Text', '3456'),
-    ('AV8BNA_ODU_4_SELECT', '4'),
-    ('AV8BNA_ODU_4_Text', '4567'),
-    ('AV8BNA_ODU_5_SELECT', '5'),
-    ('AV8BNA_ODU_5_Text', '5678')
-]
-
-
-@mark.parametrize('model, bios_pairs', [
-    ('hornet_mono', hornet_bios),
-    ('hornet_color', hornet_bios),
-    ('viper_mono', viper_bios),
-    ('viper_color', viper_bios),
-    ('shark_mono', shark_bios),
-    ('shark_color', shark_bios),
-    ('shark3_mono', shark_bios),
-    ('shark3_color', shark_bios),
-    ('hip_mono', hip_bios),
-    ('hip_color', hip_bios),
-    ('hind_mono', hind_bios),
-    ('hind_color', hind_bios),
-    ('apache_mono', apache_bios),
-    ('apache_color', apache_bios),
-    ('warthog_mono', warthog_bios),
-    ('warthog_color', warthog_bios),
-    ('warthog2_mono', warthog_bios),
-    ('warthog2_color', warthog_bios),
-    ('tomcata_mono', []),
-    ('tomcata_color', []),
-    ('tomcatb_mono', []),
-    ('tomcatb_color', []),
-    ('harrier_mono', harrier_bios),
-    ('harrier_color', harrier_bios),
-])
-def test_prepare_image_for_all_planes(model, bios_pairs, request):
-    aircraft_model = request.getfixturevalue(model)
-    set_bios_during_test(aircraft_model, bios_pairs)
-    img = aircraft_model.prepare_image()
-    assert isinstance(img, PIL.Image.Image)
-    ref_img = PIL.Image.open(path.join(resources, platform, f'{model}_{aircraft_model.__class__.__name__}.png'))
-    assert img.tobytes() == ref_img.tobytes()
-    assert not ImageChops.difference(img, ref_img).getbbox()
-
-
-def test_prepare_image_for_apache_mono_wca_mode(apache_mono):
-    from dcspy.aircraft import ApacheEufdMode
-    bios_pairs = [
-        ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |CHARGER           '),
-        ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |TAIL WHL LOCK SEL '),
-        ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      |                  '),
-        ('PLT_EUFD_LINE4', '                  |FORWARD FUEL LOW  |                  '),
-        ('PLT_EUFD_LINE5', '                  |                  |                  ')
-    ]
-    set_bios_during_test(apache_mono, bios_pairs)
-    apache_mono.mode = ApacheEufdMode.WCA
-    img = apache_mono.prepare_image()
-    assert isinstance(img, PIL.Image.Image)
-    ref_img = PIL.Image.open(path.join(resources, platform, 'apache_mono_wca_mode.png'))
-    assert img.tobytes() == ref_img.tobytes()
-    assert not ImageChops.difference(img, ref_img).getbbox()
-
-
-# <=><=><=><=><=> Apache special <=><=><=><=><=>
-def test_apache_mono_wca_more_then_one_screen(apache_mono):
-    from dcspy.aircraft import ApacheEufdMode
-    bios_pairs = [
-        ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |CHARGER           '),
-        ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |TAIL WHL LOCK SEL '),
-        ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      |                  ')
-    ]
-    set_bios_during_test(apache_mono, bios_pairs)
-    apache_mono.mode = ApacheEufdMode.WCA
-
-    for i in range(1, 5):
-        assert apache_mono.warning_line == i
-        apache_mono.warning_line += 1
-        apache_mono.prepare_image()
-    assert apache_mono.warning_line == 1
-    img = apache_mono.prepare_image()
-    assert isinstance(img, PIL.Image.Image)
-    ref_img = PIL.Image.open(path.join(resources, platform, 'apache_mono_wca_mode.png'))
-    assert img.tobytes() == ref_img.tobytes()
-    assert not ImageChops.difference(img, ref_img).getbbox()
-
-
-apache_pre_mono_bios = [
-    ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |PRESET TUNE VHF   '),
-    ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |!CO CMD   127.000 '),
-    ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      | D/1/227  135.000 '),
-    ('PLT_EUFD_LINE4', '                  |FORWARD FUEL LOW  | JAAT     136.000 '),
-    ('PLT_EUFD_LINE5', '                  |                  | BDE/HIG  127.000 '),
-    ('PLT_EUFD_LINE6', '                                     | FAAD     125.000 '),
-    ('PLT_EUFD_LINE7', '                                     | JTAC     121.000 '),
-    ('PLT_EUFD_LINE8', '~<>VHF*  127.000   -----             | AWACS    141.000 '),
-    ('PLT_EUFD_LINE9', ' ==UHF*  305.000   -----             | FLIGHT   128.000 '),
-    ('PLT_EUFD_LINE10', ' ==FM1*   30.000   -----    NORM     | BATUMI   126.000 '),
-    ('PLT_EUFD_LINE11', ' ==FM2*   30.000   -----             | COMMAND  137.000 ')
-]
-apache_pre_color_bios = [
-    ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |PRESET TUNE VHF   '),
-    ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |!CO CMD   127.000 '),
-    ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      | D/1/227  135.000 '),
-    ('PLT_EUFD_LINE4', '                  |FORWARD FUEL LOW  | JAAT     136.000 '),
-    ('PLT_EUFD_LINE5', '                  |                  | BDE/HIG  127.000 '),
-    ('PLT_EUFD_LINE6', '                                     | FAAD     125.000 '),
-    ('PLT_EUFD_LINE7', '                                     | JTAC     121.000 '),
-    ('PLT_EUFD_LINE8', '~<>VHF*  127.000   -----             | AWACS    141.000 '),
-    ('PLT_EUFD_LINE9', ' ==UHF*  305.000   -----             | FLIGHT   128.000 '),
-    ('PLT_EUFD_LINE10', ' ==FM1*   30.000   -----    NORM     | BATUMI   126.000 '),
-    ('PLT_EUFD_LINE11', ' ==FM2*   30.000   -----             | COMMAND  137.000 ')
-]
-
-
-@mark.parametrize('model, bios_pairs, filename', [
-    ('apache_mono', apache_pre_mono_bios, 'apache_mono_pre_mode.png'),
-    ('apache_color', apache_pre_color_bios, 'apache_color_pre_mode.png')
-])
-def test_apache_pre_mode(model, bios_pairs, filename, request):
-    aircraft_model = request.getfixturevalue(model)
-    set_bios_during_test(aircraft_model, bios_pairs)
-    img = aircraft_model.prepare_image()
-    assert isinstance(img, PIL.Image.Image)
-    ref_img = PIL.Image.open(path.join(resources, platform, filename))
-    assert img.tobytes() == ref_img.tobytes()
-    assert not ImageChops.difference(img, ref_img).getbbox()
+from pathlib import Path
+from sys import platform
+from unittest.mock import patch
+
+import PIL
+from PIL import ImageChops
+from pytest import mark, raises
+
+from dcspy import LcdColor, LcdMono, LcdButton
+from tests.helpers import all_plane_list, set_bios_during_test
+
+resources = Path(__file__).resolve().with_name('resources')
+
+
+# <=><=><=><=><=> Base Class <=><=><=><=><=>
+@mark.parametrize('model', all_plane_list)
+def test_check_all_aircraft_inherit_from_correct_base_class(model, lcd_mono):
+    from dcspy import aircraft
+    airplane = getattr(aircraft, model)
+    aircraft_model = airplane(lcd_mono)
+    assert isinstance(aircraft_model, aircraft.Aircraft)
+    assert issubclass(airplane, aircraft.Aircraft)
+
+
+@mark.parametrize('selector, data, value, c_func, effect, lcd', [
+    ('field1', {'addr': 0xdeadbeef, 'len': 16, 'value': ''}, 'val1', 'logi_lcd_mono_set_background', [True], LcdMono),
+    ('field2', {'addr': 0xdeadbeef, 'len': 16, 'value': ''}, 'val2', 'logi_lcd_color_set_background', [False, True], LcdColor),
+])
+def test_aircraft_base_class_set_bios_with_mono_color_lcd(selector, data, value, c_func, effect, lcd, aircraft):
+    from dcspy.sdk import lcd_sdk
+    assert aircraft.bios_data == {}
+    aircraft.bios_data = {selector: data}
+    aircraft.lcd = lcd
+    with patch.object(lcd_sdk, 'logi_lcd_is_connected', side_effect=effect), \
+            patch.object(lcd_sdk, c_func, return_value=True), \
+            patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
+        assert aircraft.bios_data[selector]['value'] == ''
+        assert aircraft.get_bios('none') == ''
+        with raises(NotImplementedError):
+            aircraft.set_bios(selector, value)
+
+
+@mark.parametrize('mode, c_func, lcd', [('1', 'logi_lcd_mono_set_background', LcdMono),
+                                        ('RGBA', 'logi_lcd_color_set_background', LcdColor)])
+def test_aircraft_base_class_prepare_img_with_mono_color_lcd(mode, c_func, lcd, aircraft):
+    from dcspy.sdk import lcd_sdk
+    aircraft.lcd = lcd
+    with patch.object(lcd_sdk, 'logi_lcd_is_connected', return_value=True), \
+            patch.object(lcd_sdk, c_func, return_value=True), \
+            patch.object(lcd_sdk, 'logi_lcd_update', return_value=True), \
+            raises(NotImplementedError):
+        aircraft.prepare_image()
+
+
+# <=><=><=><=><=> Button Requests <=><=><=><=><=>
+@mark.parametrize('plane, button, result', [
+    ('hornet_mono', LcdButton.NONE, '\n'),
+    ('hornet_mono', LcdButton.ONE, 'UFC_COMM1_CHANNEL_SELECT DEC\n'),
+    ('hornet_mono', LcdButton.TWO, 'UFC_COMM1_CHANNEL_SELECT INC\n'),
+    ('hornet_mono', LcdButton.THREE, 'UFC_COMM2_CHANNEL_SELECT DEC\n'),
+    ('hornet_mono', LcdButton.FOUR, 'UFC_COMM2_CHANNEL_SELECT INC\n'),
+    ('hornet_color', LcdButton.NONE, '\n'),
+    ('hornet_color', LcdButton.LEFT, 'UFC_COMM1_CHANNEL_SELECT DEC\n'),
+    ('hornet_color', LcdButton.RIGHT, 'UFC_COMM1_CHANNEL_SELECT INC\n'),
+    ('hornet_color', LcdButton.DOWN, 'UFC_COMM2_CHANNEL_SELECT DEC\n'),
+    ('hornet_color', LcdButton.UP, 'UFC_COMM2_CHANNEL_SELECT INC\n'),
+    ('hornet_color', LcdButton.MENU, 'IFEI_DWN_BTN 1\n'),
+    ('hornet_color', LcdButton.CANCEL, 'IFEI_UP_BTN 1\n'),
+    ('hornet_color', LcdButton.OK, 'HUD_ATT_SW 1\n'),
+    ('harrier_mono', LcdButton.NONE, '\n'),
+    ('harrier_mono', LcdButton.ONE, 'UFC_COM1_SEL -3200\n'),
+    ('harrier_mono', LcdButton.TWO, 'UFC_COM1_SEL 3200\n'),
+    ('harrier_mono', LcdButton.THREE, 'UFC_COM2_SEL -3200\n'),
+    ('harrier_mono', LcdButton.FOUR, 'UFC_COM2_SEL 3200\n'),
+    ('harrier_color', LcdButton.NONE, '\n'),
+    ('harrier_color', LcdButton.LEFT, 'UFC_COM1_SEL -3200\n'),
+    ('harrier_color', LcdButton.RIGHT, 'UFC_COM1_SEL 3200\n'),
+    ('harrier_color', LcdButton.DOWN, 'UFC_COM2_SEL -3200\n'),
+    ('harrier_color', LcdButton.UP, 'UFC_COM2_SEL 3200\n'),
+    ('harrier_color', LcdButton.MENU, '\n'),
+    ('harrier_color', LcdButton.CANCEL, '\n'),
+    ('harrier_color', LcdButton.OK, '\n'),
+    ('shark_mono', LcdButton.NONE, '\n'),
+    ('shark_mono', LcdButton.ONE, 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n'),
+    ('shark_mono', LcdButton.TWO, 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n'),
+    ('shark_mono', LcdButton.THREE, 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n'),
+    ('shark_mono', LcdButton.FOUR, 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'),
+    ('shark_color', LcdButton.NONE, '\n'),
+    ('shark_color', LcdButton.LEFT, 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n'),
+    ('shark_color', LcdButton.RIGHT, 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n'),
+    ('shark_color', LcdButton.DOWN, 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n'),
+    ('shark_color', LcdButton.UP, 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'),
+    ('shark_color', LcdButton.MENU, '\n'),
+    ('shark_color', LcdButton.CANCEL, '\n'),
+    ('shark_color', LcdButton.OK, '\n'),
+    ('shark3_mono', LcdButton.NONE, '\n'),
+    ('shark3_mono', LcdButton.ONE, 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n'),
+    ('shark3_mono', LcdButton.TWO, 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n'),
+    ('shark3_mono', LcdButton.THREE, 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n'),
+    ('shark3_mono', LcdButton.FOUR, 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'),
+    ('shark3_color', LcdButton.NONE, '\n'),
+    ('shark3_color', LcdButton.LEFT, 'PVI_WAYPOINTS_BTN 1\nPVI_WAYPOINTS_BTN 0\n'),
+    ('shark3_color', LcdButton.RIGHT, 'PVI_FIXPOINTS_BTN 1\nPVI_FIXPOINTS_BTN 0\n'),
+    ('shark3_color', LcdButton.DOWN, 'PVI_AIRFIELDS_BTN 1\nPVI_AIRFIELDS_BTN 0\n'),
+    ('shark3_color', LcdButton.UP, 'PVI_TARGETS_BTN 1\nPVI_TARGETS_BTN 0\n'),
+    ('shark3_color', LcdButton.MENU, '\n'),
+    ('shark3_color', LcdButton.CANCEL, '\n'),
+    ('shark3_color', LcdButton.OK, '\n'),
+    ('tomcata_mono', LcdButton.NONE, '\n'),
+    ('tomcata_mono', LcdButton.ONE, 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n'),
+    ('tomcata_mono', LcdButton.TWO, 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n'),
+    ('tomcata_mono', LcdButton.THREE, 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n'),
+    ('tomcata_mono', LcdButton.FOUR, 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'),
+    ('tomcata_color', LcdButton.NONE, '\n'),
+    ('tomcata_color', LcdButton.LEFT, 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n'),
+    ('tomcata_color', LcdButton.RIGHT, 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n'),
+    ('tomcata_color', LcdButton.DOWN, 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n'),
+    ('tomcata_color', LcdButton.UP, 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'),
+    ('tomcata_color', LcdButton.MENU, '\n'),
+    ('tomcata_color', LcdButton.CANCEL, '\n'),
+    ('tomcata_color', LcdButton.OK, '\n'),
+    ('tomcatb_mono', LcdButton.NONE, '\n'),
+    ('tomcatb_mono', LcdButton.ONE, 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n'),
+    ('tomcatb_mono', LcdButton.TWO, 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n'),
+    ('tomcatb_mono', LcdButton.THREE, 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n'),
+    ('tomcatb_mono', LcdButton.FOUR, 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'),
+    ('tomcatb_color', LcdButton.NONE, '\n'),
+    ('tomcatb_color', LcdButton.LEFT, 'RIO_CAP_CLEAR 1\nRIO_CAP_CLEAR 0\n'),
+    ('tomcatb_color', LcdButton.RIGHT, 'RIO_CAP_SW 1\nRIO_CAP_SW 0\n'),
+    ('tomcatb_color', LcdButton.DOWN, 'RIO_CAP_NE 1\nRIO_CAP_NE 0\n'),
+    ('tomcatb_color', LcdButton.UP, 'RIO_CAP_ENTER 1\nRIO_CAP_ENTER 0\n'),
+    ('tomcatb_color', LcdButton.MENU, '\n'),
+    ('tomcatb_color', LcdButton.CANCEL, '\n'),
+    ('tomcatb_color', LcdButton.OK, '\n'),
+    ('viper_mono', LcdButton.NONE, '\n'),
+    ('viper_mono', LcdButton.ONE, 'IFF_MASTER_KNB 1\n'),
+    ('viper_mono', LcdButton.TWO, 'IFF_ENABLE_SW 1\n'),
+    ('viper_mono', LcdButton.THREE, 'IFF_M4_CODE_SW 1\n'),
+    ('viper_mono', LcdButton.FOUR, 'IFF_M4_REPLY_SW 1\n'),
+    ('viper_color', LcdButton.NONE, '\n'),
+    ('viper_color', LcdButton.LEFT, 'IFF_MASTER_KNB 1\n'),
+    ('viper_color', LcdButton.RIGHT, 'IFF_ENABLE_SW 1\n'),
+    ('viper_color', LcdButton.DOWN, 'IFF_M4_CODE_SW 1\n'),
+    ('viper_color', LcdButton.UP, 'IFF_M4_REPLY_SW 1\n'),
+    ('viper_color', LcdButton.MENU, '\n'),
+    ('viper_color', LcdButton.CANCEL, '\n'),
+    ('viper_color', LcdButton.OK, '\n'),
+    ('apache_mono', LcdButton.NONE, '\n'),
+    ('apache_mono', LcdButton.ONE, 'PLT_EUFD_IDM 0\nPLT_EUFD_IDM 1\n'),
+    ('apache_mono', LcdButton.TWO, 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n'),
+    ('apache_mono', LcdButton.THREE, 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n'),
+    ('apache_mono', LcdButton.FOUR, 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n'),
+])
+def test_button_pressed_for_plane(plane, button, result, request):
+    plane = request.getfixturevalue(plane)
+    assert plane.button_request(button) == result
+
+
+@mark.parametrize('button, result', [
+    (LcdButton.NONE, '\n'),
+    (LcdButton.LEFT, 'PLT_EUFD_WCA 0\nPLT_EUFD_WCA 1\n'),
+    (LcdButton.RIGHT, 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n'),
+    (LcdButton.DOWN, 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n'),
+    (LcdButton.UP, 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n'),
+    (LcdButton.MENU, '\n'),
+    (LcdButton.CANCEL, '\n'),
+    (LcdButton.OK, '\n'),
+])
+def test_button_pressed_for_apache_color(button, result, apache_color):
+    from dcspy.aircraft import ApacheEufdMode
+    apache_color.mode = ApacheEufdMode.WCA
+    assert apache_color.button_request(button) == result
+
+
+@mark.parametrize('plane, btn_name, btn, values', [
+    ('viper_mono', 'IFF_MASTER_KNB', LcdButton.ONE, (1, 2, 3, 4, 3, 2, 1, 0, 1)),
+    ('viper_mono', 'IFF_ENABLE_SW', LcdButton.TWO, (1, 2, 1, 0, 1)),
+    ('viper_mono', 'IFF_M4_CODE_SW', LcdButton.THREE, (1, 2, 1, 0, 1)),
+    ('viper_mono', 'IFF_M4_REPLY_SW', LcdButton.FOUR, (1, 2, 1, 0, 1)),
+    ('viper_color', 'IFF_MASTER_KNB', LcdButton.LEFT, (1, 2, 3, 4, 3, 2, 1, 0, 1)),
+    ('viper_color', 'IFF_ENABLE_SW', LcdButton.RIGHT, (1, 2, 1, 0, 1)),
+    ('viper_color', 'IFF_M4_CODE_SW', LcdButton.DOWN, (1, 2, 1, 0, 1)),
+    ('viper_color', 'IFF_M4_REPLY_SW', LcdButton.UP, (1, 2, 1, 0, 1)),
+    ('hornet_color', 'HUD_ATT_SW', LcdButton.OK, (1, 2, 1, 0, 1)),
+    ('hornet_color', 'IFEI_DWN_BTN', LcdButton.MENU, (1, 0, 1)),
+    ('hornet_color', 'IFEI_UP_BTN', LcdButton.CANCEL, (1, 0, 1)),
+])
+def test_get_next_value_for_cycle_buttons(plane, btn_name, btn, values, request):
+    from itertools import cycle
+    plane = request.getfixturevalue(plane)
+    assert not all([isinstance(cyc_btn, cycle) for cyc_btn in plane.cycle_buttons.values()])
+    for val in values:
+        assert plane.button_request(btn) == f'{btn_name} {val}\n'
+    assert isinstance(plane.cycle_buttons[btn_name], cycle)
+
+
+# <=><=><=><=><=> Set BIOS <=><=><=><=><=>
+@mark.parametrize('plane, bios_pairs, result', [
+    ('hornet_mono', [('UFC_SCRATCHPAD_STRING_2_DISPLAY', '~~')], '22'),
+    ('hornet_mono', [('UFC_COMM1_DISPLAY', '``')], '11'),
+    ('hornet_mono', [('IFEI_FUEL_UP', '104T')], '104T'),
+    ('hornet_color', [('UFC_SCRATCHPAD_STRING_1_DISPLAY', '~~')], '22'),
+    ('hornet_color', [('UFC_COMM1_DISPLAY', '``')], '11'),
+    ('hornet_color', [('IFEI_FUEL_UP', '1000T')], '1000T'),
+    ('viper_mono', [('DED_LINE_1', 'a')], '\u2666'),
+    ('viper_mono', [('DED_LINE_2', 'o')], '\u00b0'),
+    ('viper_mono', [('DED_LINE_3', '*')], '\u25d9'),
+    ('viper_mono', [('DED_LINE_5', '\x07')], ''),
+    ('viper_mono', [('DED_LINE_4', '\x10')], ''),
+    ('viper_mono', [('DED_LINE_2', '   @')], '   '),
+    ('viper_color', [('DED_LINE_3', 'a')], '\u0040'),
+    ('viper_color', [('DED_LINE_4', 'o')], '\u005e'),
+    ('viper_color', [('DED_LINE_3', '*')], '\u00d7'),
+    ('viper_color', [('DED_LINE_5', '\xfe')], ''),
+    ('viper_color', [('DED_LINE_1', '\xfc')], ''),
+    ('viper_color', [('DED_LINE_2', '   @')], '   '),
+    ('viper_color', [('DED_LINE_2', '1DEST 2BNGO 3VIP  RINTG  A\x10\x04')], "ÁDEST ÂBNGO ÃVIP  rINTG  "),
+    ('viper_color', [('DED_LINE_3', '4NAV  5MAN  6INS  EDLNK  A\x10\x04')], "ÄNAV  ÅMAN  ÆINS  eDLNK  "),
+    ('viper_color', [('DED_LINE_4', '7CMDS 8MODE 9VRP  0MISC  A\x10\x04')], "ÇCMDS ÈMODE ÉVRP  ÀMISC  "),
+    ('viper_mono', [('DED_LINE_1', '       *      *CMD STRG  \x80@')], '       \u25d9      \u25d9CMD STRG  '),
+    ('viper_mono', [('DED_LINE_2', '1DEST 2BNGO 3VIP  RINTG  A\x10\x04')], '1DEST 2BNGO 3VIP  RINTG  '),
+    ('viper_mono', [('DED_LINE_1', ' MARK *HUD *    26a      @')], ' MARK \u25d9HUD \u25d9    26\u2666      '),
+    ('viper_mono', [('DED_LINE_5', 'M3 :7000 *     *DCPL(9)  \x03\x82')], 'M3 :7000 \u25d9     \u25d9DCPL(9)  '),
+    ('apache_mono', [('PLT_EUFD_LINE8', '~=>VHF*  121.000   -----              121.500   -----   ')], '\u25a0\u2219\u25b8VHF*  121.000   -----              121.500   -----   '),
+    ('apache_mono', [('PLT_EUFD_LINE9', ' <=UHF*  305.000   -----              305.000   -----   ')], ' \u25c2\u2219UHF*  305.000   -----              305.000   -----   '),
+    ('apache_mono', [('PLT_EUFD_LINE10', ' <>FM1*   30.000   -----    NORM       30.000   -----   ')], ' \u25c2\u25b8FM1*   30.000   -----    NORM       30.000   -----   '),
+    ('apache_color', [('PLT_EUFD_LINE11', '[==FM2*   30.000   -----               30.000   -----   ')], '\u25ca\u2219\u2219FM2*   30.000   -----               30.000   -----   '),
+    ('apache_color', [('PLT_EUFD_LINE12', ' ==HF *    2.0000A -----    LOW         2.0000A -----   ')], ' \u2219\u2219HF *    2.0000A -----    LOW         2.0000A -----   '),
+    ('apache_color', [('PLT_EUFD_LINE12', ']==HF *    2.0000A -----    LOW         2.0000A -----   ')], '\u2666\u2219\u2219HF *    2.0000A -----    LOW         2.0000A -----   '),
+])
+def test_set_bios_for_airplane(plane, bios_pairs, result, request):
+    plane = request.getfixturevalue(plane)
+    set_bios_during_test(plane, bios_pairs)
+    assert plane.bios_data[bios_pairs[0][0]]['value'] == result
+
+
+@mark.parametrize('plane, bios_pairs, mode', [
+    ('apache_mono', [('PLT_EUFD_LINE1', 'ENGINE 1 OUT      |AFT FUEL LOW      |TAIL WHL LOCK SEL ')], 'IDM'),
+    ('apache_mono', [('PLT_EUFD_LINE1', '                  |AFT FUEL LOW      |PRESET TUNE VHS ')], 'PRE'),
+    ('apache_color', [('PLT_EUFD_LINE1', '                  |                  |TAIL WHL LOCK SEL ')], 'IDM'),
+    ('apache_color', [('PLT_EUFD_LINE1', '                  |AFT FUEL LOW      |TAIL WHL LOCK SEL ')], 'IDM'),
+    ('apache_color', [('PLT_EUFD_LINE1', 'ENGINE 1 OUT      |AFT FUEL LOW      |PRESET TUNE FM1 ')], 'PRE'),
+])
+def test_mode_switch_idm_pre_for_apache(plane, bios_pairs, mode, request):
+    plane = request.getfixturevalue(plane)
+    set_bios_during_test(plane, bios_pairs)
+    assert plane.mode.name == mode
+
+
+# <=><=><=><=><=> Prepare Image <=><=><=><=><=>
+hornet_bios = [
+    ('UFC_SCRATCHPAD_STRING_1_DISPLAY', '11'),
+    ('UFC_SCRATCHPAD_STRING_2_DISPLAY', '22'),
+    ('UFC_SCRATCHPAD_NUMBER_DISPLAY', '1234567890'),
+    ('UFC_OPTION_DISPLAY_1', '1234'),
+    ('UFC_OPTION_DISPLAY_2', '2345'),
+    ('UFC_OPTION_DISPLAY_3', '3456'),
+    ('UFC_OPTION_DISPLAY_4', '4567'),
+    ('UFC_OPTION_DISPLAY_5', '5678'),
+    ('UFC_COMM1_DISPLAY', '11'),
+    ('UFC_COMM2_DISPLAY', '22'),
+    ('UFC_OPTION_CUEING_1', '1'),
+    ('UFC_OPTION_CUEING_2', '2'),
+    ('UFC_OPTION_CUEING_3', '3'),
+    ('UFC_OPTION_CUEING_4', '4'),
+    ('UFC_OPTION_CUEING_5', '5'),
+    ('IFEI_FUEL_DOWN', '123456'),
+    ('IFEI_FUEL_UP', '234567')
+]
+viper_bios = [
+    ('DED_LINE_1', "  INS  08.0/ 6        1a "),
+    ('DED_LINE_2', "  LAT *N 43o06.2'*       @"),
+    ('DED_LINE_3', "  LNG  E040o34.2'        "),
+    ('DED_LINE_4', " SALT      74FT          "),
+    ('DED_LINE_5', " THDG   25.0o   G/S    0 "),
+]
+shark_bios = [
+    ('PVI_LINE1_APOSTROPHE1', '`'),
+    ('PVI_LINE1_APOSTROPHE2', '`'),
+    ('PVI_LINE1_POINT', '1'),
+    ('PVI_LINE1_SIGN', '-'),
+    ('PVI_LINE1_TEXT', '123456'),
+    ('PVI_LINE2_APOSTROPHE1', '`'),
+    ('PVI_LINE2_APOSTROPHE2', '`'),
+    ('PVI_LINE2_POINT', '2'),
+    ('PVI_LINE2_SIGN', ' '),
+    ('PVI_LINE2_TEXT', '654321'),
+    ('AP_ALT_HOLD_LED', 1),
+    ('AP_BANK_HOLD_LED', 0),
+    ('AP_FD_LED', 1),
+    ('AP_HDG_HOLD_LED', 0),
+    ('AP_PITCH_HOLD_LED', 1)
+]
+hip_bios = [
+    ('LMP_AP_HDG_ON', 1),
+    ('LMP_AP_PITCH_ROLL_ON', 0),
+    ('LMP_AP_HEIGHT_ON', 1),
+    ('R863_CNL_SEL', 9),
+    ('R863_MOD', 1),
+    ('R863_FREQ', "123.525"),
+    ('R828_PRST_CHAN_SEL', 9),
+    ('YADRO1A_FREQ', "09091.9"),
+]
+hind_bios = [
+    ('PLT_R863_CHAN', 9),
+    ('PLT_R863_MODUL', 1),
+    ('PLT_R828_CHAN', 9),
+    ('JADRO_FREQ', "08082.8"),
+    ('PLT_SAU_HOVER_MODE_ON_L', 1),
+    ('PLT_SAU_ROUTE_MODE_ON_L', 0),
+    ('PLT_SAU_ALT_MODE_ON_L', 1),
+    ('PLT_SAU_H_ON_L', 0),
+    ('PLT_SAU_K_ON_L', 0),
+    ('PLT_SAU_T_ON_L', 0),
+    ('PLT_SAU_B_ON_L', 1),
+]
+apache_bios = [
+    ('PLT_EUFD_LINE8', '~<>VHF*  121.000   -----              121.500   -----   '),
+    ('PLT_EUFD_LINE9', ' ==UHF*  305.000   -----              305.000   -----   '),
+    ('PLT_EUFD_LINE10', ' ==FM1*   30.000   -----    NORM       30.000   -----   '),
+    ('PLT_EUFD_LINE11', ' ==FM2*   30.000   -----               30.000   -----   '),
+    ('PLT_EUFD_LINE12', ' ==HF *    2.0000A -----    LOW         2.0000A -----   ')
+]
+warthog_bios = [
+    ('VHFAM_FREQ1', '20'),
+    ('VHFAM_FREQ2', 1),
+    ('VHFAM_FREQ3', 1),
+    ('VHFAM_FREQ4', '30'),
+    ('VHFFM_FREQ1', '40'),
+    ('VHFFM_FREQ2', 2),
+    ('VHFFM_FREQ3', 2),
+    ('VHFFM_FREQ4', '50'),
+    ('UHF_100MHZ_SEL', '5'),
+    ('UHF_10MHZ_SEL', 3),
+    ('UHF_1MHZ_SEL', 2),
+    ('UHF_POINT1MHZ_SEL', 1),
+    ('UHF_POINT25_SEL', '25')
+]
+harrier_bios = [
+    ('UFC_SCRATCHPAD', '123456789012'),
+    ('UFC_COMM1_DISPLAY', '11'),
+    ('UFC_COMM2_DISPLAY', '22'),
+    ('AV8BNA_ODU_1_SELECT', '1'),
+    ('AV8BNA_ODU_1_Text', '1234'),
+    ('AV8BNA_ODU_2_SELECT', '2'),
+    ('AV8BNA_ODU_2_Text', '2345'),
+    ('AV8BNA_ODU_3_SELECT', '3'),
+    ('AV8BNA_ODU_3_Text', '3456'),
+    ('AV8BNA_ODU_4_SELECT', '4'),
+    ('AV8BNA_ODU_4_Text', '4567'),
+    ('AV8BNA_ODU_5_SELECT', '5'),
+    ('AV8BNA_ODU_5_Text', '5678')
+]
+
+
+@mark.parametrize('model, bios_pairs', [
+    ('hornet_mono', hornet_bios),
+    ('hornet_color', hornet_bios),
+    ('viper_mono', viper_bios),
+    ('viper_color', viper_bios),
+    ('shark_mono', shark_bios),
+    ('shark_color', shark_bios),
+    ('shark3_mono', shark_bios),
+    ('shark3_color', shark_bios),
+    ('hip_mono', hip_bios),
+    ('hip_color', hip_bios),
+    ('hind_mono', hind_bios),
+    ('hind_color', hind_bios),
+    ('apache_mono', apache_bios),
+    ('apache_color', apache_bios),
+    ('warthog_mono', warthog_bios),
+    ('warthog_color', warthog_bios),
+    ('warthog2_mono', warthog_bios),
+    ('warthog2_color', warthog_bios),
+    ('tomcata_mono', []),
+    ('tomcata_color', []),
+    ('tomcatb_mono', []),
+    ('tomcatb_color', []),
+    ('harrier_mono', harrier_bios),
+    ('harrier_color', harrier_bios),
+])
+def test_prepare_image_for_all_planes(model, bios_pairs, request):
+    aircraft_model = request.getfixturevalue(model)
+    set_bios_during_test(aircraft_model, bios_pairs)
+    img = aircraft_model.prepare_image()
+    assert isinstance(img, PIL.Image.Image)
+    ref_img = PIL.Image.open(resources / platform / f'{model}_{aircraft_model.__class__.__name__}.png')
+    assert img.tobytes() == ref_img.tobytes()
+    assert not ImageChops.difference(img, ref_img).getbbox()
+
+
+def test_prepare_image_for_apache_mono_wca_mode(apache_mono):
+    from dcspy.aircraft import ApacheEufdMode
+    bios_pairs = [
+        ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |CHARGER           '),
+        ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |TAIL WHL LOCK SEL '),
+        ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      |                  '),
+        ('PLT_EUFD_LINE4', '                  |FORWARD FUEL LOW  |                  '),
+        ('PLT_EUFD_LINE5', '                  |                  |                  ')
+    ]
+    set_bios_during_test(apache_mono, bios_pairs)
+    apache_mono.mode = ApacheEufdMode.WCA
+    img = apache_mono.prepare_image()
+    assert isinstance(img, PIL.Image.Image)
+    ref_img = PIL.Image.open(resources / platform / 'apache_mono_wca_mode.png')
+    assert img.tobytes() == ref_img.tobytes()
+    assert not ImageChops.difference(img, ref_img).getbbox()
+
+
+# <=><=><=><=><=> Apache special <=><=><=><=><=>
+def test_apache_mono_wca_more_then_one_screen(apache_mono):
+    from dcspy.aircraft import ApacheEufdMode
+    bios_pairs = [
+        ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |CHARGER           '),
+        ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |TAIL WHL LOCK SEL '),
+        ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      |                  ')
+    ]
+    set_bios_during_test(apache_mono, bios_pairs)
+    apache_mono.mode = ApacheEufdMode.WCA
+
+    for i in range(1, 5):
+        assert apache_mono.warning_line == i
+        apache_mono.warning_line += 1
+        apache_mono.prepare_image()
+    assert apache_mono.warning_line == 1
+    img = apache_mono.prepare_image()
+    assert isinstance(img, PIL.Image.Image)
+    ref_img = PIL.Image.open(resources / platform / 'apache_mono_wca_mode.png')
+    assert img.tobytes() == ref_img.tobytes()
+    assert not ImageChops.difference(img, ref_img).getbbox()
+
+
+apache_pre_mono_bios = [
+    ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |PRESET TUNE VHF   '),
+    ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |!CO CMD   127.000 '),
+    ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      | D/1/227  135.000 '),
+    ('PLT_EUFD_LINE4', '                  |FORWARD FUEL LOW  | JAAT     136.000 '),
+    ('PLT_EUFD_LINE5', '                  |                  | BDE/HIG  127.000 '),
+    ('PLT_EUFD_LINE6', '                                     | FAAD     125.000 '),
+    ('PLT_EUFD_LINE7', '                                     | JTAC     121.000 '),
+    ('PLT_EUFD_LINE8', '~<>VHF*  127.000   -----             | AWACS    141.000 '),
+    ('PLT_EUFD_LINE9', ' ==UHF*  305.000   -----             | FLIGHT   128.000 '),
+    ('PLT_EUFD_LINE10', ' ==FM1*   30.000   -----    NORM     | BATUMI   126.000 '),
+    ('PLT_EUFD_LINE11', ' ==FM2*   30.000   -----             | COMMAND  137.000 ')
+]
+apache_pre_color_bios = [
+    ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |PRESET TUNE VHF   '),
+    ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |!CO CMD   127.000 '),
+    ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      | D/1/227  135.000 '),
+    ('PLT_EUFD_LINE4', '                  |FORWARD FUEL LOW  | JAAT     136.000 '),
+    ('PLT_EUFD_LINE5', '                  |                  | BDE/HIG  127.000 '),
+    ('PLT_EUFD_LINE6', '                                     | FAAD     125.000 '),
+    ('PLT_EUFD_LINE7', '                                     | JTAC     121.000 '),
+    ('PLT_EUFD_LINE8', '~<>VHF*  127.000   -----             | AWACS    141.000 '),
+    ('PLT_EUFD_LINE9', ' ==UHF*  305.000   -----             | FLIGHT   128.000 '),
+    ('PLT_EUFD_LINE10', ' ==FM1*   30.000   -----    NORM     | BATUMI   126.000 '),
+    ('PLT_EUFD_LINE11', ' ==FM2*   30.000   -----             | COMMAND  137.000 ')
+]
+
+
+@mark.parametrize('model, bios_pairs, filename', [
+    ('apache_mono', apache_pre_mono_bios, 'apache_mono_pre_mode.png'),
+    ('apache_color', apache_pre_color_bios, 'apache_color_pre_mode.png')
+])
+def test_apache_pre_mode(model, bios_pairs, filename, request):
+    aircraft_model = request.getfixturevalue(model)
+    set_bios_during_test(aircraft_model, bios_pairs)
+    img = aircraft_model.prepare_image()
+    assert isinstance(img, PIL.Image.Image)
+    ref_img = PIL.Image.open(resources / platform / filename)
+    assert img.tobytes() == ref_img.tobytes()
+    assert not ImageChops.difference(img, ref_img).getbbox()
```

### Comparing `dcspy-1.9.5/tests/test_logitech.py` & `dcspy-2.0.0/tests/test_logitech.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-from unittest.mock import call, patch
-
-from pytest import mark
-
-from dcspy import LcdType, LcdButton
-from dcspy.logitech import KeyboardColor, KeyboardMono
-from tests.helpers import all_plane_list
-
-
-def test_keyboard_base_basic_check(keyboard_base):
-    from dcspy.sdk import lcd_sdk
-
-    assert str(keyboard_base) == 'LogitechKeyboard: 160x43'
-    logitech_repr = repr(keyboard_base)
-    data = ('parser', 'ProtocolParser', 'plane_name', 'plane_detected', 'already_pressed', 'buttons',
-            '_display', 'plane', 'Aircraft', 'vert_space', 'lcd')
-    for test_string in data:
-        assert test_string in logitech_repr
-
-    with patch.object(lcd_sdk, 'clear_display', return_value=True):
-        keyboard_base.clear()
-
-
-@mark.parametrize('pressed1, effect, chk_btn, calls, pressed2', [
-    (False, [False, False, False, True], LcdButton.FOUR, [call(1), call(2), call(4), call(8)], True),
-    (True, [True, False, False, False], LcdButton.NONE, [call(1)], True),
-    (False, [False, False, False, False], LcdButton.NONE, [call(1), call(2), call(4), call(8)], False),
-])
-def test_keyboard_mono_check_buttons(pressed1, effect, chk_btn, calls, pressed2, keyboard_mono):
-    from dcspy.sdk import lcd_sdk
-    keyboard_mono.already_pressed = pressed1
-    with patch.object(lcd_sdk, 'logi_lcd_is_button_pressed', side_effect=effect) as lcd_btn_pressed:
-        assert keyboard_mono.check_buttons() == chk_btn
-    lcd_btn_pressed.assert_has_calls(calls)
-    assert keyboard_mono.already_pressed is pressed2
-
-
-def test_keyboard_color_button_handle(keyboard_color, sock):
-    from dcspy.sdk import lcd_sdk
-    with patch.object(lcd_sdk, 'logi_lcd_is_button_pressed', side_effect=[True]):
-        keyboard_color.button_handle(sock)
-    sock.sendto.assert_called_once_with(b'\n', ('127.0.0.1', 7778))
-
-
-@mark.parametrize('plane_str, plane, display, detect', [
-    ('FA-18C_hornet', 'FA18Chornet', ['Detected aircraft:', 'F/A-18C Hornet'], True),
-    ('F-16C_50', 'F16C50', ['Detected aircraft:', 'F-16C Viper'], True),
-    ('Ka-50', 'Ka50', ['Detected aircraft:', 'Ka-50 Black Shark II'], True),
-    ('Ka-503', 'Ka503', ['Detected aircraft:', 'Ka-50 Black Shark III'], True),
-    ('Mi-8MT', 'Mi8MT', ['Detected aircraft:', 'Mi-8MTV2 Magnificent Eight'], True),
-    ('Mi-24P', 'Mi24P', ['Detected aircraft:', 'Mi-24P Hind'], True),
-    ('AH-64D_BLKII', 'AH64DBLKII', ['Detected aircraft:', 'AH-64D Apache'], True),
-    ('A-10C', 'A10C', ['Detected aircraft:', 'A-10C Warthog'], True),
-    ('A-10C_2', 'A10C2', ['Detected aircraft:', 'A-10C II Tank Killer'], True),
-    ('F-14B', 'F14B', ['Detected aircraft:', 'F-14B Tomcat'], True),
-    ('F14A135GR', 'F14A135GR', ['Detected aircraft:', 'F-14A Tomcat'], True),
-    ('AV8BNA', 'AV8BNA', ['Detected aircraft:', 'AV-8B N/A Harrier'], True),
-    ('F-117_Nighthawk', 'F117Nighthawk', ['Detected aircraft:', 'F117Nighthawk', 'Not supported yet!'], False),
-    ('', '', [], False),
-])
-def test_keyboard_mono_detecting_plane(plane_str, plane, display, detect, keyboard_mono):
-    from dcspy.sdk import lcd_sdk
-    with patch.object(lcd_sdk, 'logi_lcd_is_connected', return_value=True), \
-            patch.object(lcd_sdk, 'logi_lcd_mono_set_background', return_value=True), \
-            patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
-        keyboard_mono.detecting_plane(plane_str)
-    assert keyboard_mono.plane_name == plane
-    assert keyboard_mono._display == display
-    assert keyboard_mono.plane_detected is detect
-
-
-@mark.parametrize('mode, size,  lcd_type, keyboard', [('1', (160, 43), LcdType.MONO, KeyboardMono),
-                                                      ('RGBA', (320, 240), LcdType.COLOR, KeyboardColor)])
-def test_check_keyboard_display_and_prepare_image(mode, size, lcd_type, keyboard, protocol_parser):
-    from dcspy.aircraft import Aircraft
-    from dcspy.sdk import lcd_sdk
-    from dcspy import LcdInfo
-
-    with patch.object(lcd_sdk, 'logi_lcd_init', return_value=True):
-        keyboard = keyboard(protocol_parser)
-    assert isinstance(keyboard.plane, Aircraft)
-    assert isinstance(keyboard.lcd, LcdInfo)
-    assert keyboard.lcd.type == lcd_type
-    assert isinstance(keyboard.display, list)
-    with patch.object(lcd_sdk, 'update_display', return_value=True):
-        keyboard.display = ['1', '2']
-        assert len(keyboard.display) == 2
-
-    img = keyboard._prepare_image()
-    assert img.mode == mode
-    assert img.size == size
-
-
-@mark.parametrize('keyboard', [KeyboardMono, KeyboardColor])
-def test_check_keyboard_text(keyboard, protocol_parser):
-    from dcspy.sdk import lcd_sdk
-
-    with patch.object(lcd_sdk, 'logi_lcd_init', return_value=True):
-        keyboard = keyboard(protocol_parser)
-
-    with patch.object(lcd_sdk, 'update_text', return_value=True) as upd_txt:
-        keyboard.text(['1', '2'])
-        upd_txt.assert_called()
-
-
-@mark.parametrize('model', all_plane_list)
-def test_keyboard_mono_load_plane(model, keyboard_mono):
-    from dcspy.sdk import lcd_sdk
-    from dcspy.aircraft import Aircraft
-    with patch.object(lcd_sdk, 'logi_lcd_is_connected', return_value=True), \
-            patch.object(lcd_sdk, 'logi_lcd_mono_set_background', return_value=True), \
-            patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
-        keyboard_mono.plane_name = model
-        keyboard_mono.load_new_plane()
-    assert isinstance(keyboard_mono.plane, Aircraft)
-    assert model in keyboard_mono.plane.__class__.__name__
+from unittest.mock import call, patch
+
+from pytest import mark
+
+from dcspy import LcdType, LcdButton
+from dcspy.logitech import KeyboardColor, KeyboardMono
+from tests.helpers import all_plane_list
+
+
+def test_keyboard_base_basic_check(keyboard_base):
+    from dcspy.sdk import lcd_sdk
+
+    assert str(keyboard_base) == 'LogitechKeyboard: 160x43'
+    logitech_repr = repr(keyboard_base)
+    data = ('parser', 'ProtocolParser', 'plane_name', 'plane_detected', 'already_pressed', 'buttons',
+            '_display', 'plane', 'Aircraft', 'vert_space', 'lcd')
+    for test_string in data:
+        assert test_string in logitech_repr
+
+    with patch.object(lcd_sdk, 'clear_display', return_value=True):
+        keyboard_base.clear()
+
+
+@mark.parametrize('pressed1, effect, chk_btn, calls, pressed2', [
+    (False, [False, False, False, True], LcdButton.FOUR, [call(1), call(2), call(4), call(8)], True),
+    (True, [True, False, False, False], LcdButton.NONE, [call(1)], True),
+    (False, [False, False, False, False], LcdButton.NONE, [call(1), call(2), call(4), call(8)], False),
+])
+def test_keyboard_mono_check_buttons(pressed1, effect, chk_btn, calls, pressed2, keyboard_mono):
+    from dcspy.sdk import lcd_sdk
+    keyboard_mono.already_pressed = pressed1
+    with patch.object(lcd_sdk, 'logi_lcd_is_button_pressed', side_effect=effect) as lcd_btn_pressed:
+        assert keyboard_mono.check_buttons() == chk_btn
+    lcd_btn_pressed.assert_has_calls(calls)
+    assert keyboard_mono.already_pressed is pressed2
+
+
+def test_keyboard_color_button_handle(keyboard_color, sock):
+    from dcspy.sdk import lcd_sdk
+    with patch.object(lcd_sdk, 'logi_lcd_is_button_pressed', side_effect=[True]):
+        keyboard_color.button_handle(sock)
+    sock.sendto.assert_called_once_with(b'\n', ('127.0.0.1', 7778))
+
+
+@mark.parametrize('plane_str, plane, display, detect', [
+    ('FA-18C_hornet', 'FA18Chornet', ['Detected aircraft:', 'F/A-18C Hornet'], True),
+    ('F-16C_50', 'F16C50', ['Detected aircraft:', 'F-16C Viper'], True),
+    ('Ka-50', 'Ka50', ['Detected aircraft:', 'Ka-50 Black Shark II'], True),
+    ('Ka-503', 'Ka503', ['Detected aircraft:', 'Ka-50 Black Shark III'], True),
+    ('Mi-8MT', 'Mi8MT', ['Detected aircraft:', 'Mi-8MTV2 Magnificent Eight'], True),
+    ('Mi-24P', 'Mi24P', ['Detected aircraft:', 'Mi-24P Hind'], True),
+    ('AH-64D_BLKII', 'AH64DBLKII', ['Detected aircraft:', 'AH-64D Apache'], True),
+    ('A-10C', 'A10C', ['Detected aircraft:', 'A-10C Warthog'], True),
+    ('A-10C_2', 'A10C2', ['Detected aircraft:', 'A-10C II Tank Killer'], True),
+    ('F-14B', 'F14B', ['Detected aircraft:', 'F-14B Tomcat'], True),
+    ('F14A135GR', 'F14A135GR', ['Detected aircraft:', 'F-14A Tomcat'], True),
+    ('AV8BNA', 'AV8BNA', ['Detected aircraft:', 'AV-8B N/A Harrier'], True),
+    ('F-117_Nighthawk', 'F117Nighthawk', ['Detected aircraft:', 'F117Nighthawk', 'Not supported yet!'], False),
+    ('', '', [], False),
+])
+def test_keyboard_mono_detecting_plane(plane_str, plane, display, detect, keyboard_mono):
+    from dcspy.sdk import lcd_sdk
+    with patch.object(lcd_sdk, 'logi_lcd_is_connected', return_value=True), \
+            patch.object(lcd_sdk, 'logi_lcd_mono_set_background', return_value=True), \
+            patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
+        keyboard_mono.detecting_plane(plane_str)
+    assert keyboard_mono.plane_name == plane
+    assert keyboard_mono._display == display
+    assert keyboard_mono.plane_detected is detect
+
+
+@mark.parametrize('mode, size,  lcd_type, keyboard', [('1', (160, 43), LcdType.MONO, KeyboardMono),
+                                                      ('RGBA', (320, 240), LcdType.COLOR, KeyboardColor)])
+def test_check_keyboard_display_and_prepare_image(mode, size, lcd_type, keyboard, protocol_parser):
+    from dcspy.aircraft import Aircraft
+    from dcspy.sdk import lcd_sdk
+    from dcspy import LcdInfo
+
+    with patch.object(lcd_sdk, 'logi_lcd_init', return_value=True):
+        keyboard = keyboard(protocol_parser)
+    assert isinstance(keyboard.plane, Aircraft)
+    assert isinstance(keyboard.lcd, LcdInfo)
+    assert keyboard.lcd.type == lcd_type
+    assert isinstance(keyboard.display, list)
+    with patch.object(lcd_sdk, 'update_display', return_value=True):
+        keyboard.display = ['1', '2']
+        assert len(keyboard.display) == 2
+
+    img = keyboard._prepare_image()
+    assert img.mode == mode
+    assert img.size == size
+
+
+@mark.parametrize('keyboard', [KeyboardMono, KeyboardColor])
+def test_check_keyboard_text(keyboard, protocol_parser):
+    from dcspy.sdk import lcd_sdk
+
+    with patch.object(lcd_sdk, 'logi_lcd_init', return_value=True):
+        keyboard = keyboard(protocol_parser)
+
+    with patch.object(lcd_sdk, 'update_text', return_value=True) as upd_txt:
+        keyboard.text(['1', '2'])
+        upd_txt.assert_called()
+
+
+@mark.parametrize('model', all_plane_list)
+def test_keyboard_mono_load_plane(model, keyboard_mono):
+    from dcspy.sdk import lcd_sdk
+    from dcspy.aircraft import Aircraft
+    with patch.object(lcd_sdk, 'logi_lcd_is_connected', return_value=True), \
+            patch.object(lcd_sdk, 'logi_lcd_mono_set_background', return_value=True), \
+            patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
+        keyboard_mono.plane_name = model
+        keyboard_mono.load_new_plane()
+    assert isinstance(keyboard_mono.plane, Aircraft)
+    assert model in keyboard_mono.plane.__class__.__name__
```

