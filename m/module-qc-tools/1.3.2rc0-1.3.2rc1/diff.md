# Comparing `tmp/module_qc_tools-1.3.2rc0.tar.gz` & `tmp/module_qc_tools-1.3.2rc1.tar.gz`

## Comparing `module_qc_tools-1.3.2rc0.tar` & `module_qc_tools-1.3.2rc1.tar`

### file list

```diff
@@ -1,49 +1,55 @@
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/.flake8
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/.gitmodules
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/tbump.toml
--rw-r--r--   0        0        0    40218 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/Measurements/ADC_CALIBRATION/2023-04-27_204040/20UPGXM1234567.json
--rw-r--r--   0        0        0   311634 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/Measurements/ANALOG_READBACK/2023-04-27_204048/20UPGXM1234567.json
--rw-r--r--   0        0        0    22346 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/Measurements/INJECTION_CAPACITANCE/2023-04-27_204052/20UPGXM1234567.json
--rw-r--r--   0        0        0    75478 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/Measurements/SLDO/2023-04-27_204051/20UPGXM1234567.json
--rw-r--r--   0        0        0   140202 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/Measurements/VCAL_CALIBRATION/2023-04-27_204053/20UPGXM1234567.json
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/emulator/README.md
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/_version.py
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    21893 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/SLDO.py
--rw-r--r--   0        0        0    12063 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0    17257 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/hardware_emulator.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/main.py
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/upload_localdb.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/configs/emulator_merged_vmux.json
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/configs/example_merged_vmux.json
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/configs/example_separate_vmux.json
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/module_state_template.json
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json
--rw-r--r--   0        0        0  1905867 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json
--rw-r--r--   0        0        0  1905871 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json
--rw-r--r--   0        0        0  1905885 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json
--rw-r--r--   0        0        0  1905869 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/ADC_CALIBRATION.json
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/ANALOG_READBACK.json
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/SLDO.json
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json
--rw-r--r--   0        0        0    26090 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/common.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/__init__.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/hardware_control_base.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/misc.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/multimeter.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/ntc.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/power_supply.py
--rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/yarr.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/tests/test_package.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/LICENSE
--rw-r--r--   0        0        0    23808 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/README.md
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/pyproject.toml
--rw-r--r--   0        0        0    25933 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc0/PKG-INFO
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/.gitmodules
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/tbump.toml
+-rw-r--r--   0        0        0    40218 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/ADC_CALIBRATION/2023-05-16_222258/20UPGXM1234567.json
+-rw-r--r--   0        0        0   311634 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/ANALOG_READBACK/2023-05-16_222258/20UPGXM1234567.json
+-rw-r--r--   0        0        0    22346 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/INJECTION_CAPACITANCE/2023-05-16_222259/20UPGXM1234567.json
+-rw-r--r--   0        0        0    27194 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/LP_MODE/2023-05-16_222257/20UPGXM1234567.json
+-rw-r--r--   0        0        0    23798 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/OVERVOLTAGE_PROTECTION/2023-05-16_222254/20UPGXM1234567.json
+-rw-r--r--   0        0        0    75478 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/SLDO/2023-05-16_222255/20UPGXM1234567.json
+-rw-r--r--   0        0        0   140202 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/VCAL_CALIBRATION/2023-05-16_222245/20UPGXM1234567.json
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/emulator/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/_version.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0    10519 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/LP_MODE.py
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    12449 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0    17516 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/hardware_emulator.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/main.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/upload_localdb.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/configs/emulator_merged_vmux.json
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/configs/example_merged_vmux.json
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/configs/example_separate_vmux.json
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/module_state_template.json
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json
+-rw-r--r--   0        0        0  1905867 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json
+-rw-r--r--   0        0        0  1905871 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json
+-rw-r--r--   0        0        0  1905885 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json
+-rw-r--r--   0        0        0  1905869 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/ADC_CALIBRATION.json
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/ANALOG_READBACK.json
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/LP_MODE.json
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/SLDO.json
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json
+-rw-r--r--   0        0        0    26090 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/common.json
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/config.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/__init__.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/hardware_control_base.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/misc.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/multimeter.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/ntc.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/power_supply.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/yarr.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/tests/test_package.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/LICENSE
+-rw-r--r--   0        0        0    28359 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/README.md
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/pyproject.toml
+-rw-r--r--   0        0        0    30484 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/PKG-INFO
```

### Comparing `module_qc_tools-1.3.2rc0/.gitlab-ci.yml` & `module_qc_tools-1.3.2rc1/.gitlab-ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -41,92 +41,129 @@
 SLDO:
   stage: test
   script:
     - python3 -m pip install .
     - echo "Running SLDO with toy emulator..."
     - measurement-SLDO -c $(module-qc-tools
       --prefix)/configs/emulator_merged_vmux.json -o ./
-    - for file in Measurements/SLDO/*/*; do echo $file; jsonschema --instance
-      $file $(module-qc-tools --prefix)/schema/common.json; done
-    - for file in Measurements/SLDO/*/*; do echo $file; jsonschema --instance
-      $file $(module-qc-tools --prefix)/schema/SLDO.json; done
+    - for file in Measurements/SLDO/*/*.json; do echo $file; jsonschema
+      --instance $file $(module-qc-tools --prefix)/schema/common.json; done
+    - for file in Measurements/SLDO/*/*.json; do echo $file; jsonschema
+      --instance $file $(module-qc-tools --prefix)/schema/SLDO.json; done
   artifacts:
     paths:
       - Measurements/SLDO/*/*.json
     expire_in: 1 day
 
 VCAL_CALIBRATION:
   stage: test
   script:
     - python3 -m pip install .
     - echo "Running VCAL_CALIBRATION with the toy emulator..."
     - measurement-VCAL-CALIBRATION -c $(module-qc-tools
       --prefix)/configs/emulator_merged_vmux.json -o ./
-    - for file in Measurements/VCAL_CALIBRATION/*/*; do echo $file; jsonschema
-      --instance $file $(module-qc-tools --prefix)/schema/common.json; done
-    - for file in Measurements/VCAL_CALIBRATION/*/*; do echo $file; jsonschema
-      --instance $file $(module-qc-tools --prefix)/schema/VCAL_CALIBRATION.json;
-      done
+    - for file in Measurements/VCAL_CALIBRATION/*/*.json; do echo $file;
+      jsonschema --instance $file $(module-qc-tools
+      --prefix)/schema/common.json; done
+    - for file in Measurements/VCAL_CALIBRATION/*/*.json; do echo $file;
+      jsonschema --instance $file $(module-qc-tools
+      --prefix)/schema/VCAL_CALIBRATION.json; done
   artifacts:
     paths:
       - Measurements/VCAL_CALIBRATION/*/*.json
     expire_in: 1 day
 
 ANALOG_READBACK:
   stage: test
   script:
     - python3 -m pip install .
     - echo "Running ANALOG_READBACK with toy emulator..."
     - measurement-ANALOG-READBACK -c $(module-qc-tools
       --prefix)/configs/emulator_merged_vmux.json -o ./
-    - for file in Measurements/ANALOG_READBACK/*/*; do echo $file; jsonschema
-      --instance $file $(module-qc-tools --prefix)/schema/common.json; done
-    - for file in Measurements/ANALOG_READBACK/*/*; do echo $file; jsonschema
-      --instance $file $(module-qc-tools --prefix)/schema/ANALOG_READBACK.json;
-      done
+    - for file in Measurements/ANALOG_READBACK/*/*.json; do echo $file;
+      jsonschema --instance $file $(module-qc-tools
+      --prefix)/schema/common.json; done
+    - for file in Measurements/ANALOG_READBACK/*/*.json; do echo $file;
+      jsonschema --instance $file $(module-qc-tools
+      --prefix)/schema/ANALOG_READBACK.json; done
   artifacts:
     paths:
       - Measurements/ANALOG_READBACK/*/*.json
     expire_in: 1 day
 
 ADC_CALIBRATION:
   stage: test
   script:
     - python3 -m pip install . --no-cache-dir
     - echo "Running ADC_CALIBRATION with the toy emulator..."
     - measurement-ADC-CALIBRATION -c $(module-qc-tools
       --prefix)/configs/emulator_merged_vmux.json -o ./
-    - for file in Measurements/ADC_CALIBRATION/*/*; do echo $file; jsonschema
-      --instance $file $(module-qc-tools --prefix)/schema/common.json; done
-    - for file in Measurements/ADC_CALIBRATION/*/*; do echo $file; jsonschema
-      --instance $file $(module-qc-tools --prefix)/schema/ADC_CALIBRATION.json;
-      done
+    - for file in Measurements/ADC_CALIBRATION/*/*.json; do echo $file;
+      jsonschema --instance $file $(module-qc-tools
+      --prefix)/schema/common.json; done
+    - for file in Measurements/ADC_CALIBRATION/*/*.json; do echo $file;
+      jsonschema --instance $file $(module-qc-tools
+      --prefix)/schema/ADC_CALIBRATION.json; done
   artifacts:
     paths:
       - Measurements/ADC_CALIBRATION/*/*.json
     expire_in: 1 day
 
 INJECTION_CAPACITANCE:
   stage: test
   script:
     - python3 -m pip install . --no-cache-dir
     - echo "Running INJECTION-CAPACITANCE with the toy emulator..."
     - measurement-INJECTION-CAPACITANCE -c $(module-qc-tools
       --prefix)/configs/emulator_merged_vmux.json -o ./
-    - for file in Measurements/INJECTION_CAPACITANCE/*/*; do echo $file;
+    - for file in Measurements/INJECTION_CAPACITANCE/*/*.json; do echo $file;
       jsonschema --instance $file $(module-qc-tools
       --prefix)/schema/common.json; done
-    - for file in Measurements/INJECTION_CAPACITANCE/*/*; do echo $file;
+    - for file in Measurements/INJECTION_CAPACITANCE/*/*.json; do echo $file;
       jsonschema --instance $file $(module-qc-tools
       --prefix)/schema/INJECTION_CAPACITANCE.json; done
   artifacts:
     paths:
       - Measurements/INJECTION_CAPACITANCE/*/*.json
     expire_in: 1 day
 
+LP_MODE:
+  stage: test
+  script:
+    - python3 -m pip install .
+    - echo "Running LP_MODE with toy emulator..."
+    - measurement-LP-MODE -c $(module-qc-tools
+      --prefix)/configs/emulator_merged_vmux.json -o ./
+    - for file in Measurements/LP_MODE/*/*.json; do echo $file; jsonschema
+      --instance $file $(module-qc-tools --prefix)/schema/common.json; done
+    - for file in Measurements/LP_MODE/*/*.json; do echo $file; jsonschema
+      --instance $file $(module-qc-tools --prefix)/schema/LP_MODE.json; done
+  artifacts:
+    paths:
+      - Measurements/LP_MODE/*/*.json
+    expire_in: 1 day
+
+OVERVOLTAGE_PROTECTION:
+  stage: test
+  script:
+    - python3 -m pip install .
+    - echo "Running OVERVOLTAGE_PROTECTION with toy emulator..."
+    - measurement-OVERVOLTAGE-PROTECTION -c $(module-qc-tools
+      --prefix)/configs/emulator_merged_vmux.json -o ./
+    - for file in Measurements/OVERVOLTAGE_PROTECTION/*/*.json; do echo $file;
+      jsonschema --instance $file $(module-qc-tools
+      --prefix)/schema/common.json; done
+    - for file in Measurements/OVERVOLTAGE_PROTECTION/*/*.json; do echo $file;
+      jsonschema --instance $file $(module-qc-tools
+      --prefix)/schema/OVERVOLTAGE_PROTECTION.json; done
+  artifacts:
+    paths:
+      - Measurements/OVERVOLTAGE_PROTECTION/*/*.json
+    expire_in: 1 day
+
 package:
   stage: build
   variables:
     GIT_STRATEGY: clone
   script:
     - pipx run hatch run build-check
   artifacts:
```

### Comparing `module_qc_tools-1.3.2rc0/.pre-commit-config.yaml` & `module_qc_tools-1.3.2rc1/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,19 @@
+ci:
+  autoupdate_commit_msg: "chore: update pre-commit hooks"
+  autofix_commit_msg: "style: pre-commit fixes"
+
 repos:
+  - repo: https://github.com/psf/black
+    rev: "23.3.0"
+    hooks:
+      - id: black-jupyter
+
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: check-json
       - id: trailing-whitespace
       # broken in old git from 2013
       # - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
@@ -22,99 +31,50 @@
         args: ["--pytest-test-first"]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.0.1
     hooks:
       - id: check-added-large-files
 
-  - repo: https://github.com/MarcoGorelli/absolufy-imports
-    rev: v0.3.1
-    hooks:
-      - id: absolufy-imports
-
-  - repo: https://github.com/psf/black
-    rev: 22.10.0
+  - repo: https://github.com/pre-commit/pygrep-hooks
+    rev: "v1.10.0"
     hooks:
-      - id: black-jupyter
-
-  # -   repo: https://github.com/pre-commit/mirrors-mypy
-  #     rev: v0.971  # Use the sha / tag you want to point at
-  #     hooks:
-  #     -   id: mypy
+      - id: rst-backticks
+      - id: rst-directive-colons
+      - id: rst-inline-touching-normal
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
         files: ^.*\.(py|md|rst)$
         args: ["-w", "-L", "hist,gaus"]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0-alpha.3"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript] #, json]
         args: [--prose-wrap=always]
         language_version: 16.14.2
 
-  - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
-    hooks:
-      - id: python-check-blanket-noqa
-      - id: python-check-blanket-type-ignore
-      - id: python-no-eval
-      - id: python-use-type-annotations
-      - id: rst-backticks
-      - id: rst-directive-colons
-      - id: rst-inline-touching-normal
-
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.13.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.3.0]
 
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.11.5
-    hooks:
-      - id: isort
-        # args: ["-a", "from __future__ import annotations"] # Python 3.7+
-
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.1.0
-    hooks:
-      - id: pyupgrade
-        args: ["--py36-plus"]
-
-  - repo: https://github.com/hadialqattan/pycln
-    rev: v2.1.1
-    hooks:
-      - id: pycln
-        additional_dependencies: [click<8.1]
-        args: [--all]
-        stages: [manual]
-
-  - repo: https://github.com/asottile/yesqa
-    rev: v1.4.0
-    hooks:
-      - id: yesqa
-        exclude: docs/conf.py
-        additional_dependencies: &flake8_dependencies
-          - flake8-bugbear
-          - flake8-print
-
-  - repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: v0.0.261
     hooks:
-      - id: flake8
-        exclude: docs/conf.py
-        additional_dependencies: *flake8_dependencies
+      - id: ruff
+        args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.8.0.4
+    rev: v0.9.0.2
     hooks:
       - id: shellcheck
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
```

### Comparing `module_qc_tools-1.3.2rc0/tbump.toml` & `module_qc_tools-1.3.2rc1/tbump.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e33 2e32 7263 3022 0a0a  t = "1.3.2rc0"..
+00000010: 7420 3d20 2231 2e33 2e32 7263 3122 0a0a  t = "1.3.2rc1"..
 00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
 00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
 00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
 00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
 00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
 00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
 00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
@@ -15,15 +15,15 @@
 000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
 000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
 00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
 00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
 00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
 00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
 00000140: 2242 756d 7020 7665 7273 696f 6e3a 2031  "Bump version: 1
-00000150: 2e33 2e32 7263 3020 e286 9220 7b6e 6577  .3.2rc0 ... {new
+00000150: 2e33 2e32 7263 3120 e286 9220 7b6e 6577  .3.2rc1 ... {new
 00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
 00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
 00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
 00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
 000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
 000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
 000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
```

### Comparing `module_qc_tools-1.3.2rc0/Measurements/ADC_CALIBRATION/2023-04-27_204040/20UPGXM1234567.json` & `module_qc_tools-1.3.2rc1/Measurements/ADC_CALIBRATION/2023-05-16_222258/20UPGXM1234567.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666666%*

 * *Differences: {'0': "{0: {'results': {'property': {'ADC_CALIBRATION_MEASUREMENT_VERSION': '1.3.2rc1'}, "*

 * *      "'Metadata': {'TimeStart': 1684275780, 'TimeEnd': 1684275961}}}}",*

 * * '1': "{0: {'results': {'property': {'ADC_CALIBRATION_MEASUREMENT_VERSION': '1.3.2rc1'}, "*

 * *      "'Metadata': {'TimeStart': 1684275780, 'TimeEnd': 1684275961}}}}",*

 * * '2': "{0: {'results': {'property': {'ADC_CALIBRATION_MEASUREMENT_VERSION': '1.3.2rc1'}, "*

 * *      "'Metadata': {'TimeStart': 1684275780, 'TimeEnd': 1684275961}}}}",*

 * * '3': "{0: {'results […]*

```diff
@@ -246,20 +246,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628225,
-                    "TimeStart": 1682628042
+                    "TimeEnd": 1684275961,
+                    "TimeStart": 1684275780
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "ADC_CALIBRATION"
         }
     ],
@@ -510,20 +510,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628225,
-                    "TimeStart": 1682628042
+                    "TimeEnd": 1684275961,
+                    "TimeStart": 1684275780
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "ADC_CALIBRATION"
         }
     ],
@@ -774,20 +774,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628225,
-                    "TimeStart": 1682628042
+                    "TimeEnd": 1684275961,
+                    "TimeStart": 1684275780
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "ADC_CALIBRATION"
         }
     ],
@@ -1038,20 +1038,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628225,
-                    "TimeStart": 1682628042
+                    "TimeEnd": 1684275961,
+                    "TimeStart": 1684275780
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "ADC_CALIBRATION"
         }
     ]
```

### Comparing `module_qc_tools-1.3.2rc0/Measurements/ANALOG_READBACK/2023-04-27_204048/20UPGXM1234567.json` & `module_qc_tools-1.3.2rc1/Measurements/ANALOG_READBACK/2023-05-16_222258/20UPGXM1234567.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666666%*

 * *Differences: {'0': "{0: {'results': {'property': {'ANALOG_READBACK_MEASUREMENT_VERSION': '1.3.2rc1'}, "*

 * *      "'Metadata': {'TimeStart': 1684275781, 'TimeEnd': 1684276264}}}, 1: {'results': {'property': "*

 * *      "{'ANALOG_READBACK_MEASUREMENT_VERSION': '1.3.2rc1'}, 'Metadata': {'TimeStart': 1684275858, "*

 * *      "'TimeEnd': 1684276264}}}, 2: {'results': {'property': "*

 * *      "{'ANALOG_READBACK_MEASUREMENT_VERSION': '1.3.2rc1'}, 'Metadata': {'TimeStart': 1684276196, "*

 * *      "'TimeEnd': 1684276264}}}}",*

 * * '1': "{0: {'results': […]*

```diff
@@ -450,20 +450,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628562,
-                    "TimeStart": 1682628051
+                    "TimeEnd": 1684276264,
+                    "TimeStart": 1684275781
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -1063,20 +1063,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628562,
-                    "TimeStart": 1682628131
+                    "TimeEnd": 1684276264,
+                    "TimeStart": 1684275858
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -2178,20 +2178,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628562,
-                    "TimeStart": 1682628490
+                    "TimeEnd": 1684276264,
+                    "TimeStart": 1684276196
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
@@ -2646,20 +2646,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628562,
-                    "TimeStart": 1682628051
+                    "TimeEnd": 1684276264,
+                    "TimeStart": 1684275781
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -3259,20 +3259,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628562,
-                    "TimeStart": 1682628131
+                    "TimeEnd": 1684276264,
+                    "TimeStart": 1684275858
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -4374,20 +4374,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628562,
-                    "TimeStart": 1682628490
+                    "TimeEnd": 1684276264,
+                    "TimeStart": 1684276196
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
@@ -4842,20 +4842,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628562,
-                    "TimeStart": 1682628051
+                    "TimeEnd": 1684276264,
+                    "TimeStart": 1684275781
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -5455,20 +5455,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628562,
-                    "TimeStart": 1682628131
+                    "TimeEnd": 1684276264,
+                    "TimeStart": 1684275858
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -6570,20 +6570,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628562,
-                    "TimeStart": 1682628490
+                    "TimeEnd": 1684276264,
+                    "TimeStart": 1684276196
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
@@ -7038,20 +7038,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628562,
-                    "TimeStart": 1682628051
+                    "TimeEnd": 1684276264,
+                    "TimeStart": 1684275781
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -7651,20 +7651,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628562,
-                    "TimeStart": 1682628131
+                    "TimeEnd": 1684276264,
+                    "TimeStart": 1684275858
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -8766,20 +8766,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628562,
-                    "TimeStart": 1682628490
+                    "TimeEnd": 1684276264,
+                    "TimeStart": 1684276196
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ]
```

### Comparing `module_qc_tools-1.3.2rc0/Measurements/INJECTION_CAPACITANCE/2023-04-27_204052/20UPGXM1234567.json` & `module_qc_tools-1.3.2rc1/Measurements/INJECTION_CAPACITANCE/2023-05-16_222259/20UPGXM1234567.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666666%*

 * *Differences: {'0': "{0: {'results': {'property': {'INJECTION_CAPACITANCE_MEASUREMENT_VERSION': '1.3.2rc1'}, "*

 * *      "'Metadata': {'TimeStart': 1684275781, 'TimeEnd': 1684275844}}}}",*

 * * '1': "{0: {'results': {'property': {'INJECTION_CAPACITANCE_MEASUREMENT_VERSION': '1.3.2rc1'}, "*

 * *      "'Metadata': {'TimeStart': 1684275781, 'TimeEnd': 1684275844}}}}",*

 * * '2': "{0: {'results': {'property': {'INJECTION_CAPACITANCE_MEASUREMENT_VERSION': '1.3.2rc1'}, "*

 * *      "'Metadata': {'TimeStart': 1684275781, 'TimeEnd': 1684275844}}}}",*

 * * ' […]*

```diff
@@ -120,20 +120,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628115,
-                    "TimeStart": 1682628054
+                    "TimeEnd": 1684275844,
+                    "TimeStart": 1684275781
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ],
@@ -258,20 +258,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628115,
-                    "TimeStart": 1682628054
+                    "TimeEnd": 1684275844,
+                    "TimeStart": 1684275781
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ],
@@ -396,20 +396,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628115,
-                    "TimeStart": 1682628054
+                    "TimeEnd": 1684275844,
+                    "TimeStart": 1684275781
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ],
@@ -534,20 +534,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628115,
-                    "TimeStart": 1682628055
+                    "TimeEnd": 1684275844,
+                    "TimeStart": 1684275781
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ]
```

### Comparing `module_qc_tools-1.3.2rc0/Measurements/SLDO/2023-04-27_204051/20UPGXM1234567.json` & `module_qc_tools-1.3.2rc1/Measurements/SLDO/2023-05-16_222255/20UPGXM1234567.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9909855769230769%*

 * *Differences: {'0': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION': '1.3.2rc1'}, 'Metadata': "*

 * *      "{'TimeStart': 1684275776, 'TimeEnd': 1684276226}}}}",*

 * * '1': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION': '1.3.2rc1'}, 'Metadata': "*

 * *      "{'TimeStart': 1684275776, 'TimeEnd': 1684276226}}}}",*

 * * '2': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION': '1.3.2rc1'}, 'Metadata': "*

 * *      "{'TimeStart': 1684275776, 'TimeEnd': 1684276226}}}}",*

 * * '3': "{0: {'results': {'property': {'SLDO_MEASUREMEN […]*

```diff
@@ -466,20 +466,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628486,
-                    "TimeStart": 1682628051
+                    "TimeEnd": 1684276226,
+                    "TimeStart": 1684275776
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "SLDO"
         }
     ],
@@ -950,20 +950,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628486,
-                    "TimeStart": 1682628052
+                    "TimeEnd": 1684276226,
+                    "TimeStart": 1684275776
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "SLDO"
         }
     ],
@@ -1434,20 +1434,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628486,
-                    "TimeStart": 1682628052
+                    "TimeEnd": 1684276226,
+                    "TimeStart": 1684275776
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "SLDO"
         }
     ],
@@ -1918,20 +1918,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628486,
-                    "TimeStart": 1682628052
+                    "TimeEnd": 1684276226,
+                    "TimeStart": 1684275776
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "SLDO"
         }
     ]
```

### Comparing `module_qc_tools-1.3.2rc0/Measurements/VCAL_CALIBRATION/2023-04-27_204053/20UPGXM1234567.json` & `module_qc_tools-1.3.2rc1/Measurements/VCAL_CALIBRATION/2023-05-16_222245/20UPGXM1234567.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666666%*

 * *Differences: {'0': "{0: {'results': {'property': {'VCAL_CALIBRATION_MEASUREMENT_VERSION': '1.3.2rc1'}, "*

 * *      "'Metadata': {'TimeStart': 1684275769, 'TimeEnd': 1684275780}}}, 1: {'results': {'property': "*

 * *      "{'VCAL_CALIBRATION_MEASUREMENT_VERSION': '1.3.2rc1'}, 'Metadata': {'TimeStart': 1684275780, "*

 * *      "'TimeEnd': 1684275791}}}, 2: {'results': {'property': "*

 * *      "{'VCAL_CALIBRATION_MEASUREMENT_VERSION': '1.3.2rc1'}, 'Metadata': {'TimeStart': 1684275791, "*

 * *      "'TimeEnd': 1684275802}}}, 3: {'results': {'prop […]*

```diff
@@ -202,20 +202,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628074,
-                    "TimeStart": 1682628057
+                    "TimeEnd": 1684275780,
+                    "TimeStart": 1684275769
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "VCAL_MED",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -420,20 +420,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628090,
-                    "TimeStart": 1682628074
+                    "TimeEnd": 1684275791,
+                    "TimeStart": 1684275780
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "VCAL_MED_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -638,20 +638,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628107,
-                    "TimeStart": 1682628090
+                    "TimeEnd": 1684275802,
+                    "TimeStart": 1684275791
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "VCAL_HIGH",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -856,20 +856,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628123,
-                    "TimeStart": 1682628107
+                    "TimeEnd": 1684275813,
+                    "TimeStart": 1684275802
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "VCAL_HIGH_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         }
     ],
@@ -1076,20 +1076,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628140,
-                    "TimeStart": 1682628123
+                    "TimeEnd": 1684275824,
+                    "TimeStart": 1684275813
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "VCAL_MED",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -1294,20 +1294,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628156,
-                    "TimeStart": 1682628140
+                    "TimeEnd": 1684275834,
+                    "TimeStart": 1684275824
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "VCAL_MED_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -1512,20 +1512,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628173,
-                    "TimeStart": 1682628156
+                    "TimeEnd": 1684275845,
+                    "TimeStart": 1684275834
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "VCAL_HIGH",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -1730,20 +1730,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628189,
-                    "TimeStart": 1682628173
+                    "TimeEnd": 1684275855,
+                    "TimeStart": 1684275845
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "VCAL_HIGH_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         }
     ],
@@ -1950,20 +1950,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628206,
-                    "TimeStart": 1682628189
+                    "TimeEnd": 1684275866,
+                    "TimeStart": 1684275855
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "VCAL_MED",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -2168,20 +2168,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628222,
-                    "TimeStart": 1682628206
+                    "TimeEnd": 1684275877,
+                    "TimeStart": 1684275866
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "VCAL_MED_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -2386,20 +2386,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628239,
-                    "TimeStart": 1682628222
+                    "TimeEnd": 1684275887,
+                    "TimeStart": 1684275877
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "VCAL_HIGH",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -2604,20 +2604,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628256,
-                    "TimeStart": 1682628239
+                    "TimeEnd": 1684275898,
+                    "TimeStart": 1684275887
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "VCAL_HIGH_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         }
     ],
@@ -2824,20 +2824,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628273,
-                    "TimeStart": 1682628256
+                    "TimeEnd": 1684275909,
+                    "TimeStart": 1684275898
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "VCAL_MED",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -3042,20 +3042,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628290,
-                    "TimeStart": 1682628273
+                    "TimeEnd": 1684275919,
+                    "TimeStart": 1684275909
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "VCAL_MED_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -3260,20 +3260,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628307,
-                    "TimeStart": 1682628290
+                    "TimeEnd": 1684275931,
+                    "TimeStart": 1684275919
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "VCAL_HIGH",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -3478,20 +3478,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1682628323,
-                    "TimeStart": 1682628307
+                    "TimeEnd": 1684275942,
+                    "TimeStart": 1684275931
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc0"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "VCAL_HIGH_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         }
     ]
```

### Comparing `module_qc_tools-1.3.2rc0/emulator/README.md` & `module_qc_tools-1.3.2rc1/emulator/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -81,7 +81,33 @@
   -r CONTROLLER, --controller CONTROLLER
                         Controller
   -c CONNECTIVITY, --connectivity CONNECTIVITY
                         Connectivity
   -i CHIPPOSITION, --chipPosition CHIPPOSITION
                         chip position
 ```
+
+## `emulator-switch-lpm`
+
+`emulator-switch-lpm` emulates the effect when toggling low power mode
+
+```
+
+TBD
+$ emulator-write-register --help
+usage: write-register [-h] [-r CONTROLLER] [-c CONNECTIVITY] [-i CHIPPOSITION]
+                      [--skip-reset]
+                      name value
+
+positional arguments:
+  name                  Name
+  value                 Value
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -r CONTROLLER, --controller CONTROLLER
+                        Controller
+  -c CONNECTIVITY, --connectivity CONNECTIVITY
+                        Connectivity
+  -i CHIPPOSITION, --chipPosition CHIPPOSITION
+                        chip position
+```
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/ADC_CALIBRATION.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/ADC_CALIBRATION.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import json
 import logging
-import os
 import sys
 from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import pkg_resources
 from module_qc_data_tools import (
     get_env,
     get_layer_from_sn,
     get_sn_from_connectivity,
-    load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
 from module_qc_tools import data
-from module_qc_tools.utils.misc import get_identifiers, get_meta_data
+from module_qc_tools.utils.misc import check_meas_config, get_identifiers, get_meta_data
 from module_qc_tools.utils.multimeter import multimeter
 from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
-logging.basicConfig(level=logging.DEBUG)
-log = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO)
+log = logging.getLogger("measurement")
 
 parser = ArgumentParser()
 parser.add_argument(
     "-c",
     "--config",
     action="store",
     default=data / "configs/example_merged_vmux.json",
     help="Config file",
 )
 parser.add_argument(
-    "-i", "--input-file", action="store", nargs="*", help="input file if exists"
-)
-parser.add_argument(
     "-o",
     "--output-dir",
     action="store",
     default="outputs",
     help="output directory",
 )
 parser.add_argument(
     "-m",
     "--module-connectivity",
     action="store",
     help="path to the module connectivity. Used also to identify the module SN, and to set the default output directory",
 )
-parser.add_argument("--verbose", action="store_true", help="verbose mode")
+parser.add_argument(
+    "-v",
+    "--verbosity",
+    action="store",
+    default="INFO",
+    help="Log level [options: DEBUG, INFO (default) WARNING, ERROR]",
+)
 parser.add_argument(
     "--perchip",
     action="store_true",
     help="Store results in one file per chip (default: one file per module)",
 )
 args = parser.parse_args()
 
@@ -126,67 +127,76 @@
     if yr.running_emulator():
         ps.off()
 
 
 def main():
     """main() creates the qcDataFrame and pass it to the run() where the measurements are stored in the qcDataFrame."""
 
+    log.setLevel(args.verbosity)
+
     log.info("[run_ADC_calib] Start ADC calibration!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     log.info(f"[run_ADC_calib] TimeStart: {timestart}")
 
     with resources.as_file(Path(args.config)) as path:
         config = json.loads(path.read_text())
 
+    check_meas_config(config, args.config)
+
     if args.module_connectivity:
         config["yarr"]["connectivity"] = args.module_connectivity
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
     if "emulator" not in args.config and not args.module_connectivity:
-        raise RuntimeError(
-            "must supply path to connectivity file [-m --module-connectivity]"
-        )
+        msg = "must supply path to connectivity file [-m --module-connectivity]"
+        raise RuntimeError(msg)
 
     adc_calib_config = config["tasks"]["GENERAL"]
     adc_calib_config.update(config["tasks"]["ADC_CALIBRATION"])
 
-    ps = power_supply(config["power_supply"], verbose=args.verbose)
-    yr = yarr(config["yarr"], verbose=args.verbose)
-    meter = multimeter(config["multimeter"], verbose=args.verbose)
+    ps = power_supply(config["power_supply"])
+    yr = yarr(config["yarr"])
+    meter = multimeter(config["multimeter"])
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
     layer = get_layer_from_sn(module_serial)
-    test_type = os.path.basename(__file__).split(".py")[0]
+    test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
     if institution is None:
         institution = ""
 
     ps.set(v=adc_calib_config["v_max"], i=adc_calib_config["i_config"][layer])
 
     # if -o option used, overwrite the default output directory
     if args.module_connectivity:
         output_dir = args.module_connectivity.rsplit("/", 1)[0]
     else:
         output_dir = args.output_dir
 
-    if "outputs" != args.output_dir:
+    if args.output_dir != "outputs":
         output_dir = args.output_dir
 
+    # Make output directory and start log file
+    Path(f"{output_dir}/Measurements/{test_type}/{timestart}").mkdir(
+        parents=True, exist_ok=True
+    )
+    log.addHandler(
+        logging.FileHandler(
+            f"{output_dir}/Measurements/{test_type}/{timestart}/output.log"
+        )
+    )
+
     InjVcalRange = adc_calib_config["InjVcalRange"]
 
-    input_files = (
-        [None] * yr._number_of_chips if not args.input_file else args.input_file
-    )
+    input_files = [None] * yr._number_of_chips
     data = [
-        load_json(input_file)
-        if input_file
-        else qcDataFrame(
+        qcDataFrame(
             columns=["DACs_input"]
             + [f"Vmux{v_mux}" for v_mux in adc_calib_config["MonitorV"]]
             + [f"ADC_Vmux{v_mux}" for v_mux in adc_calib_config["MonitorV"]],
             units=["Count"]
             + ["V" for v_mux in adc_calib_config["MonitorV"]]
             + ["Count" for v_mux in adc_calib_config["MonitorV"]],
         )
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/ANALOG_READBACK.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/ANALOG_READBACK.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 #!/usr/bin/env python
 from __future__ import annotations
 
 import json
 import logging
-import os
 import sys
 from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
 
 import pkg_resources
 from module_qc_data_tools import (
     get_env,
     get_layer_from_sn,
     get_sn_from_connectivity,
-    load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 from tabulate import tabulate
 
 from module_qc_tools import data
-from module_qc_tools.utils.misc import get_identifiers, get_meta_data
+from module_qc_tools.utils.misc import check_meas_config, get_identifiers, get_meta_data
 from module_qc_tools.utils.multimeter import multimeter
 from module_qc_tools.utils.ntc import ntc
 from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
-logging.basicConfig(level=logging.DEBUG)
-log = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO)
+log = logging.getLogger("measurement")
 
 parser = ArgumentParser()
 parser.add_argument(
     "-c",
     "--config",
     action="store",
     default=data / "configs/example_merged_vmux.json",
     help="Config file",
 )
 parser.add_argument(
-    "-i", "--input-file", action="store", nargs="*", help="input file if exists"
-)
-parser.add_argument(
     "-o",
     "--output-dir",
     action="store",
     default="outputs",
     help="output directory",
 )
 parser.add_argument(
     "-m",
     "--module-connectivity",
     action="store",
     help="path to the module connectivity. Used also to identify the module SN, and to set the default output directory",
 )
-parser.add_argument("--verbose", action="store_true", help="verbose mode")
+parser.add_argument(
+    "-v",
+    "--verbosity",
+    action="store",
+    default="INFO",
+    help="Log level [options: DEBUG, INFO (default) WARNING, ERROR]",
+)
 parser.add_argument(
     "--perchip",
     action="store_true",
     help="Store results in one file per chip (default: one file per module)",
 )
 args = parser.parse_args()
 
@@ -290,15 +291,15 @@
 
     i_mea = [{} for _ in range(yr._number_of_chips)]
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
 
         # Measure VDDA/VDDD vs SldoTrimA/SldoTrimD
-        for v_mux in trim_maps.keys():
+        for v_mux in trim_maps:
             yr.set_mux(chip_position=chip, v_mux=v_mux, reset_other_chips=reset)
             for trim in analog_readback_config[trim_maps[v_mux]]:
                 yr.set_trim(
                     chip_position=chip,
                     v_mux=v_mux,
                     trim=trim,
                     reset_other_chips=reset,
@@ -368,44 +369,47 @@
 
 
 def main():
     """
     main() creates the qcDataFrame and pass it to the run() where the measurements are stored in the qcDataFrame.
     """
 
+    log.setLevel(args.verbosity)
+
     log.info("[run_AnalogReadBack] Starting analog readback!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     log.info(f"[run_AnalogReadBack] TimeStart: {timestart}")
 
     with resources.as_file(Path(args.config)) as path:
         config = json.loads(path.read_text())
 
+    check_meas_config(config, args.config)
+
     if args.module_connectivity:
         config["yarr"]["connectivity"] = args.module_connectivity
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
     if "emulator" not in args.config and not args.module_connectivity:
-        raise RuntimeError(
-            "must supply path to connectivity file [-m --module-connectivity]"
-        )
+        msg = "must supply path to connectivity file [-m --module-connectivity]"
+        raise RuntimeError(msg)
 
     analog_readback_config = config["tasks"]["GENERAL"]
     analog_readback_config.update(config["tasks"]["ANALOG_READBACK"])
 
-    ps = power_supply(config["power_supply"], verbose=args.verbose)
-    yr = yarr(config["yarr"], verbose=args.verbose)
-    meter = multimeter(config["multimeter"], verbose=args.verbose)
-    nt = ntc(config["ntc"], verbose=args.verbose)
+    ps = power_supply(config["power_supply"])
+    yr = yarr(config["yarr"])
+    meter = multimeter(config["multimeter"])
+    nt = ntc(config["ntc"])
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
     layer = get_layer_from_sn(module_serial)
-    test_type = os.path.basename(__file__).split(".py")[0]
+    test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
     if institution is None:
         institution = ""
 
     ps.set(
         v=analog_readback_config["v_max"], i=analog_readback_config["i_config"][layer]
     )
@@ -413,37 +417,41 @@
 
     # if -o option used, overwrite the default output directory
     if args.module_connectivity:
         output_dir = args.module_connectivity.rsplit("/", 1)[0]
     else:
         output_dir = args.output_dir
 
-    if "outputs" != args.output_dir:
+    if args.output_dir != "outputs":
         output_dir = args.output_dir
 
-    input_files = (
-        [None] * yr._number_of_chips if not args.input_file else args.input_file
+    # Make output directory and start log file
+    Path(f"{output_dir}/Measurements/{test_type}/{timestart}").mkdir(
+        parents=True, exist_ok=True
     )
+    log.addHandler(
+        logging.FileHandler(
+            f"{output_dir}/Measurements/{test_type}/{timestart}/output.log"
+        )
+    )
+
+    input_files = [None] * yr._number_of_chips
 
     data = [
-        load_json(input_file)
-        if input_file
-        else qcDataFrame(
+        qcDataFrame(
             columns=[f"Vmux{v_mux}" for v_mux in analog_readback_config["v_mux"]]
             + [f"Imux{i_mux}" for i_mux in analog_readback_config["i_mux"]],
             units=["V" for v_mux in analog_readback_config["v_mux"]]
             + ["V" for i_mux in analog_readback_config["i_mux"]],
         )
         for input_file in input_files
     ]
 
     data_tempmeas = [
-        load_json(input_file)
-        if input_file
-        else qcDataFrame(
+        qcDataFrame(
             columns=[f"Vmux{v_mux}" for v_mux in analog_readback_config["v_mux_ntc"]]
             + [f"Imux{i_mux}" for i_mux in analog_readback_config["i_mux_ntc"]]
             + [f"Vmux{v_mux}" for v_mux in analog_readback_config["v_mux_tempsens"]]
             + ["MonSensSldoAnaSelBias"]
             + ["MonSensSldoDigSelBias"]
             + ["MonSensAcbSelBias"]
             + ["MonSensSldoAnaDem"]
@@ -461,17 +469,15 @@
             + ["-"]
             + ["C"],
         )
         for input_file in input_files
     ]
 
     data_vdda_vddd_vs_trim = [
-        load_json(input_file)
-        if input_file
-        else qcDataFrame(
+        qcDataFrame(
             columns=["Vmux34"]
             + ["Vmux38"]
             + ["Vmux30"]
             + ["SldoTrimA"]
             + ["SldoTrimD"]
             + [f"ROSC{i}" for i in range(42)],
             units=["V"] + ["V"] + ["V"] + ["-"] + ["-"] + ["MHz" for i in range(42)],
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import json
 import logging
-import os
 import sys
 from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
 
 import pkg_resources
 from module_qc_data_tools import (
     get_env,
     get_layer_from_sn,
     get_sn_from_connectivity,
-    load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
 from module_qc_tools import data
-from module_qc_tools.utils.misc import get_identifiers, get_meta_data
+from module_qc_tools.utils.misc import check_meas_config, get_identifiers, get_meta_data
 from module_qc_tools.utils.multimeter import multimeter
 from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
-logging.basicConfig(level=logging.DEBUG)
-log = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO)
+log = logging.getLogger("measurement")
 
 parser = ArgumentParser()
 parser.add_argument(
     "-c",
     "--config",
     action="store",
     default=data / "configs/example_merged_vmux.json",
     help="Config file",
 )
 parser.add_argument(
-    "-i", "--input-file", action="store", nargs="*", help="input file if exists"
-)
-parser.add_argument(
     "-o",
     "--output-dir",
     action="store",
     default="outputs",
     help="output directory",
 )
 parser.add_argument(
     "-m",
     "--module-connectivity",
     action="store",
     help="path to the module connectivity. Used also to identify the module SN, and to set the default output directory",
 )
-parser.add_argument("--verbose", action="store_true", help="verbose mode")
+parser.add_argument(
+    "-v",
+    "--verbosity",
+    action="store",
+    default="INFO",
+    help="Log level [options: DEBUG, INFO (default) WARNING, ERROR]",
+)
 parser.add_argument(
     "--perchip",
     action="store_true",
     help="Store results in one file per chip (default: one file per module)",
 )
 args = parser.parse_args()
 
@@ -136,65 +137,74 @@
     if yr.running_emulator():
         ps.off()
 
 
 def main():
     """main() creates the qcDataFrame and pass it to the run() where the measurements are stored in the qcDataFrame."""
 
+    log.setLevel(args.verbosity)
+
     log.info("[run_inj_capacitance] Start injection capacitance measurement!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     log.info(f"[run_inj_capacitance] TimeStart: {timestart}")
 
     with resources.as_file(Path(args.config)) as path:
         config = json.loads(path.read_text())
 
+    check_meas_config(config, args.config)
+
     if args.module_connectivity:
         config["yarr"]["connectivity"] = args.module_connectivity
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
     if "emulator" not in args.config and not args.module_connectivity:
-        raise RuntimeError(
-            "must supply path to connectivity file [-m --module-connectivity]"
-        )
+        msg = "must supply path to connectivity file [-m --module-connectivity]"
+        raise RuntimeError(msg)
 
     inj_cap_config = config["tasks"]["GENERAL"]
     inj_cap_config.update(config["tasks"]["INJECTION_CAPACITANCE"])
 
-    ps = power_supply(config["power_supply"], verbose=args.verbose)
-    yr = yarr(config["yarr"], verbose=args.verbose)
-    meter = multimeter(config["multimeter"], verbose=args.verbose)
+    ps = power_supply(config["power_supply"])
+    yr = yarr(config["yarr"])
+    meter = multimeter(config["multimeter"])
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
     layer = get_layer_from_sn(module_serial)
-    test_type = os.path.basename(__file__).split(".py")[0]
+    test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
     if institution is None:
         institution = ""
 
     ps.set(v=inj_cap_config["v_max"], i=inj_cap_config["i_config"][layer])
 
     # if -o option used, overwrite the default output directory
     if args.module_connectivity:
         output_dir = args.module_connectivity.rsplit("/", 1)[0]
     else:
         output_dir = args.output_dir
 
-    if "outputs" != args.output_dir:
+    if args.output_dir != "outputs":
         output_dir = args.output_dir
 
-    input_files = (
-        [None] * yr._number_of_chips if not args.input_file else args.input_file
+    # Make output directory and start log file
+    Path(f"{output_dir}/Measurements/{test_type}/{timestart}").mkdir(
+        parents=True, exist_ok=True
     )
+    log.addHandler(
+        logging.FileHandler(
+            f"{output_dir}/Measurements/{test_type}/{timestart}/output.log"
+        )
+    )
+
+    input_files = [None] * yr._number_of_chips
     data = [
-        load_json(input_file)
-        if input_file
-        else qcDataFrame(
+        qcDataFrame(
             columns=[f"Vmux{v_mux}" for v_mux in inj_cap_config["v_mux"]]
             + [f"Imux{i_mux}" for i_mux in inj_cap_config["i_mux"]],
             units=["V" for v_mux in inj_cap_config["v_mux"]]
             + ["V" for i_mux in inj_cap_config["i_mux"]],
         )
         for input_file in input_files
     ]
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/SLDO.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/SLDO.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,53 @@
 #!/usr/bin/env python
 from __future__ import annotations
 
 import json
 import logging
-import os
 import sys
 from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import pkg_resources
 from module_qc_data_tools import (
     get_env,
     get_layer_from_sn,
     get_sn_from_connectivity,
-    load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 from tabulate import tabulate
 
 from module_qc_tools import data
-from module_qc_tools.utils.misc import get_identifiers, get_meta_data
+from module_qc_tools.utils.misc import check_meas_config, get_identifiers, get_meta_data
 from module_qc_tools.utils.multimeter import multimeter
 from module_qc_tools.utils.ntc import ntc
 from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
-logging.basicConfig(level=logging.DEBUG)
-log = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO)
+log = logging.getLogger("measurement")
 
 parser = ArgumentParser()
 parser.add_argument(
     "-c",
     "--config",
     action="store",
     default=data / "configs/example_merged_vmux.json",
     help="Config file",
 )
 parser.add_argument(
-    "-i", "--input-file", action="store", nargs="*", help="input file if exists"
-)
-parser.add_argument(
     "-o",
     "--output-dir",
     action="store",
     default="outputs",
     help="output directory",
 )
 parser.add_argument(
@@ -62,15 +57,21 @@
     help="path to the module connectivity. Used also to identify the module SN, and to set the default output directory",
 )
 parser.add_argument(
     "--perchip",
     action="store_true",
     help="Store results in one file per chip (default: one file per module)",
 )
-parser.add_argument("--verbose", action="store_true", help="verbose mode")
+parser.add_argument(
+    "-v",
+    "--verbosity",
+    action="store",
+    default="INFO",
+    help="Log level [options: DEBUG, INFO (default) WARNING, ERROR]",
+)
 args = parser.parse_args()
 
 
 def run(data, SLDOVI_config, ps, yr, meter, nt, layer):
     # turn on power supply and configure all chips
     ps.set(v=SLDOVI_config["v_max"], i=SLDOVI_config["i_config"][layer])
     status = yr.configure()
@@ -131,66 +132,74 @@
             log.info(tabulate(i_mea[chip], headers="keys", floatfmt=".3f"))
 
     # Return to initial state
     ps.set(v=SLDOVI_config["v_max"], i=SLDOVI_config["i_config"][layer])
 
 
 def main():
+    log.setLevel(args.verbosity)
 
     log.info("[run_SLDOVI] Start VI scan!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     log.info(f"[run_SLDOVI] TimeStart: {timestart}")
 
     with resources.as_file(Path(args.config)) as path:
         config = json.loads(path.read_text())
 
+    check_meas_config(config, args.config)
+
     # Need to pass module connectivity path to yarr class (except in case we are running the emulator)
     if args.module_connectivity:
         config["yarr"]["connectivity"] = args.module_connectivity
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
     if "emulator" not in args.config and not args.module_connectivity:
-        raise RuntimeError(
-            "must supply path to connectivity file [-m --module-connectivity]"
-        )
+        msg = "must supply path to connectivity file [-m --module-connectivity]"
+        raise RuntimeError(msg)
 
     SLDOVI_config = config["tasks"]["GENERAL"]
     SLDOVI_config.update(config["tasks"]["SLDO"])
-    ps = power_supply(config["power_supply"], verbose=args.verbose)
-    yr = yarr(config["yarr"], verbose=args.verbose)
+    ps = power_supply(config["power_supply"])
+    yr = yarr(config["yarr"])
 
-    meter = multimeter(config["multimeter"], verbose=args.verbose)
-    nt = ntc(config["ntc"], verbose=args.verbose)
+    meter = multimeter(config["multimeter"])
+    nt = ntc(config["ntc"])
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
     layer = get_layer_from_sn(module_serial)
-    test_type = os.path.basename(__file__).split(".py")[0]
+    test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
     if institution is None:
         institution = ""
 
     # if -o option used, overwrite the default output directory
     if args.module_connectivity:
         output_dir = args.module_connectivity.rsplit("/", 1)[0]
     else:
         output_dir = args.output_dir
 
-    if "outputs" != args.output_dir:
+    if args.output_dir != "outputs":
         output_dir = args.output_dir
 
-    input_files = (
-        [None] * yr._number_of_chips if not args.input_file else args.input_file
+    # Make output directory and start log file
+    Path(f"{output_dir}/Measurements/{test_type}/{timestart}").mkdir(
+        parents=True, exist_ok=True
     )
+    log.addHandler(
+        logging.FileHandler(
+            f"{output_dir}/Measurements/{test_type}/{timestart}/output.log"
+        )
+    )
+
+    input_files = [None] * yr._number_of_chips
     data = [
-        load_json(input_file)
-        if input_file
-        else qcDataFrame(
+        qcDataFrame(
             columns=["Temperature", "SetCurrent", "Current"]
             + [f"Vmux{v_mux}" for v_mux in SLDOVI_config["v_mux"]]
             + [f"Imux{i_mux}" for i_mux in SLDOVI_config["i_mux"]],
             units=["C", "A", "A"]
             + ["V" for v_mux in SLDOVI_config["v_mux"]]
             + ["V" for i_mux in SLDOVI_config["i_mux"]],
         )
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/VCAL_CALIBRATION.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/VCAL_CALIBRATION.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import json
 import logging
-import os
 import sys
 from argparse import ArgumentParser
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 import pkg_resources
@@ -17,26 +16,26 @@
     get_sn_from_connectivity,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
 from module_qc_tools import data
-from module_qc_tools.utils.misc import get_identifiers, get_meta_data
+from module_qc_tools.utils.misc import check_meas_config, get_identifiers, get_meta_data
 from module_qc_tools.utils.multimeter import multimeter
 from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
-logging.basicConfig(level=logging.DEBUG)
-log = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO)
+log = logging.getLogger("measurement")
 
 
 parser = ArgumentParser()
 parser.add_argument(
     "-c",
     "--config",
     action="store",
@@ -52,15 +51,21 @@
 )
 parser.add_argument(
     "-m",
     "--module-connectivity",
     action="store",
     help="path to the module connectivity. Used also to identify the module SN, and to set the default output directory",
 )
-parser.add_argument("--verbose", action="store_true", help="verbose mode")
+parser.add_argument(
+    "-v",
+    "--verbosity",
+    action="store",
+    default="INFO",
+    help="Log level [options: DEBUG, INFO (default) WARNING, ERROR]",
+)
 parser.add_argument(
     "--perchip",
     action="store_true",
     help="Store results in one file per chip (default: one file per module)",
 )
 args = parser.parse_args()
 
@@ -172,43 +177,46 @@
     if yr.running_emulator():
         ps.off()
 
 
 def main():
     """main() creates the qcDataFrame and pass it to the run() where the measurements are stored in the qcDataFrame."""
 
+    log.setLevel(args.verbosity)
+
     log.info("[run_VCal_calib] Start VCal calibration!")
     timestart = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     log.info(f"[run_VCal_calib] TimeStart: {timestart}")
 
     with resources.as_file(Path(args.config)) as path:
         config = json.loads(path.read_text())
 
+    check_meas_config(config, args.config)
+
     if args.module_connectivity:
         config["yarr"]["connectivity"] = args.module_connectivity
 
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
     if "emulator" not in args.config and not args.module_connectivity:
-        raise RuntimeError(
-            "must supply path to connectivity file [-m --module-connectivity]"
-        )
+        msg = "must supply path to connectivity file [-m --module-connectivity]"
+        raise RuntimeError(msg)
 
     vcal_calib_config = config["tasks"]["GENERAL"]
     vcal_calib_config.update(config["tasks"]["VCAL_CALIBRATION"])
 
-    ps = power_supply(config["power_supply"], verbose=args.verbose)
-    yr = yarr(config["yarr"], verbose=args.verbose)
-    meter = multimeter(config["multimeter"], verbose=args.verbose)
+    ps = power_supply(config["power_supply"])
+    yr = yarr(config["yarr"])
+    meter = multimeter(config["multimeter"])
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
     layer = get_layer_from_sn(module_serial)
-    test_type = os.path.basename(__file__).split(".py")[0]
+    test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
     if institution is None:
         institution = ""
 
     ps.set(v=vcal_calib_config["v_max"], i=vcal_calib_config["i_config"][layer])
 
     MonitorV = vcal_calib_config["MonitorV"]
@@ -217,17 +225,27 @@
 
     # if -o option used, overwrite the default output directory
     if args.module_connectivity:
         output_dir = args.module_connectivity.rsplit("/", 1)[0]
     else:
         output_dir = args.output_dir
 
-    if "outputs" != args.output_dir:
+    if args.output_dir != "outputs":
         output_dir = args.output_dir
 
+    # Make output directory and start log file
+    Path(f"{output_dir}/Measurements/{test_type}/{timestart}").mkdir(
+        parents=True, exist_ok=True
+    )
+    log.addHandler(
+        logging.FileHandler(
+            f"{output_dir}/Measurements/{test_type}/{timestart}/output.log"
+        )
+    )
+
     chip_data = []
     for chip in range(yr._number_of_chips):
         # if chip in yr._disabled_chip_positions:
         # continue
         qcdata_list = []
         for i, _vmux_value in enumerate(MonitorV):
             for _j, vcalrange in enumerate(InjVcalRange):
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/hardware_emulator.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/hardware_emulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import argparse
 import json
 import logging
-import os
 import shutil
 import sys
+from pathlib import Path
 
 import numpy as np
 
 from module_qc_tools import data
 
 if sys.version_info >= (3, 9):
     from importlib import resources
@@ -27,25 +27,23 @@
 def initialize_module_state():
     with resources.as_file(data / "emulator/module_state_template.json") as path:
         shutil.copyfile(path, _MODULE_STATE_FILE)
 
 
 def get_module_state():
     # Copy module state from template if not existing
-    if not os.path.isfile(_MODULE_STATE_FILE):
+    if not _MODULE_STATE_FILE.is_file():
         initialize_module_state()
 
-    with open(_MODULE_STATE_FILE) as serialized:
-        module_state = json.load(serialized)
-
-    return module_state
+    with _MODULE_STATE_FILE.open() as serialized:
+        return json.load(serialized)
 
 
 def update_module_state(state):
-    with open(_MODULE_STATE_FILE, "w") as serialized:
+    with _MODULE_STATE_FILE.open("w") as serialized:
         json.dump(state, serialized, indent=4)
 
 
 def update_Vmux(chip_state):
     """
     This function updates the Vmux voltage values to the corresponding channel.
     Currently emulates MonitorV = 1, 30, 33, 37, 34, 38, 36, 32, and
@@ -151,29 +149,31 @@
     )
     parser.add_argument(
         "-c",
         "--connectivity",
         default=_MODULE_CONNECTIVITY_FILE,
         help="Connectivity",
     )
+    parser.add_argument("-s", "--scan", default=None, help="Scan config")
     parser.add_argument("-n", "--nThreads", type=int, help="Number of threads")
+    parser.add_argument("-o", "--output", default="./", help="Output directory")
     parser.add_argument("--skip-reset", action="store_true", help="skip reset")
     args = parser.parse_args()
 
     module_state = get_module_state()
 
-    with open(args.connectivity) as path:
+    with Path(args.connectivity).open() as path:
         spec_connectivity = json.load(path)
 
     nChips = len(spec_connectivity["chips"])
 
     for chip in range(nChips):
         config_path = spec_connectivity["chips"][chip]["config"]
         abs_path = args.connectivity.rsplit("/", 1)[0] + "/" + config_path
-        with open(abs_path) as path:
+        with Path(abs_path).open() as path:
             spec = json.load(path)
         GlobalConfig = spec["RD53B"]["GlobalConfig"]
         Parameter = spec["RD53B"]["Parameter"]
         # VDDA/D should be trimmed to 1.2 after chip configuring
         module_state[f"Chip{chip+1}"]["VDDA"] = min(1.2, module_state["Vin"])
         module_state[f"Chip{chip+1}"]["VDDD"] = min(1.2, module_state["Vin"])
         # MonitorI and V set according to chip configs
@@ -195,14 +195,17 @@
         module_state[f"Chip{chip+1}"]["ADCcalSlope"] = ADCcalPar[1] * 0.001
 
         # Update Vmux
         module_state[f"Chip{chip+1}"] = update_Vmux(module_state[f"Chip{chip+1}"])
 
     update_module_state(module_state)
 
+    # YARR returns 0 when scan is run
+    if args.scan is not None:
+        return 0
     return 1
 
 
 def write_register():
     """
     This function emulates the effect of running YARR write-register
     Currently only emulates register MonitorI, MonitorV. One needs to add a new if statement for a new register name.
@@ -223,15 +226,15 @@
         help="Connectivity",
     )
     parser.add_argument("-i", "--chipPosition", type=int, help="chip position")
     args = parser.parse_args()
 
     module_state = get_module_state()
 
-    with open(args.connectivity) as path:
+    with Path(args.connectivity).open() as path:
         spec_connectivity = json.load(path)
 
     nChips = len(spec_connectivity["chips"])
 
     log.info(args.name, args.value)
 
     for chip in range(nChips):
@@ -280,19 +283,18 @@
     if args.action == "getI":
         # measure Iin
         i = module_state["Iin"]
         sys.stdout.write(f"{i}")
         sys.exit(0)
 
     if args.action == "on":
-
         nChips = module_state["nChips"]
 
         # check if the module has already been powered on
-        already_power = True if module_state["Vin"] > 0 else False
+        already_power = module_state["Vin"] > 0
 
         # Calculate Vin based on the prediction (slope and offset), as well as the voltage and the current set to the power supply
         module_state["Vin"] = min(
             0.348293 / nChips * args.current + 1, args.voltage, 2.0
         )
         # Calculate Iin from the calculated Vin
         module_state["Iin"] = (module_state["Vin"] - 1) * nChips / 0.348293
@@ -442,15 +444,15 @@
         "--connectivity",
         default=data / "emulator" / _MODULE_CONNECTIVITY_FILE,
         help="Connectivity",
     )
     parser.add_argument("-i", "--chip_position", type=int, help="chip position")
     args = parser.parse_args()
 
-    with open(args.connectivity) as path:
+    with Path(args.connectivity).open() as path:
         spec_connectivity = json.load(path)
 
     nChips = len(spec_connectivity["chips"])
 
     for chip in range(nChips):
         if args.chip_position is not None and chip is not args.chip_position:
             continue
@@ -465,7 +467,11 @@
     This function emulates the effect of NTC (measure module temperature)
     """
     module_state = get_module_state()
 
     T = module_state["temperature"]
     sys.stdout.write(f"{T}")
     sys.exit(0)
+
+
+def switchLPM():
+    sys.exit(0)
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/main.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     default=False,
     help="display prefix",
 )
 args = parser.parse_args()
 
 
 def main():
-
     if args.prefix:
         print(data)  # noqa: T201
         sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/cli/upload_localdb.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/upload_localdb.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 
     log.info(f"Extracted {len(pack)} tests from {len(flist)} input files.")
     log.info("==> Submitting RAW results pack...")
 
     protocol = "http" if args.port != "443" else "https"
 
     if not args.dry_run:
-
         try:
             response = requests.post(
                 f"{protocol}://{args.host}:{args.port}/localdb/qc_uploader_post",
                 json=pack,
             )
             response.raise_for_status()
 
@@ -101,27 +100,24 @@
                 continue
 
             log.info(
                 f'SerialNumber: {testRun["serialNumber"]}, Stage: {testRun["stage"]}, TestType: {testRun["testType"]}, QC-passed: {testRun["passed"]}'
             )
 
         try:
-
-            with open(args.out, "w") as f:
+            with Path(args.out).open("w") as f:
                 json.dump(data, f, indent=4)
                 log.info(f"Saved the output TestRun to {args.out}")
 
         except Exception:
-
             log.warning(f"Failed to saved the output TestRun to {args.out}")
             altFilePath = f"/var/tmp/module-qc-tools-record-{int(time.time())}.json"
 
             try:
-
-                with open(altFilePath, "w") as f:
+                with Path(altFilePath).open("w") as f:
                     json.dump(data, f, indent=4)
                 log.info(f"Saved the output TestRun to {altFilePath}")
 
             except Exception:
                 log.warning(f"Failed to saved the output TestRun to {altFilePath}")
                 pass
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/configs/emulator_merged_vmux.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/configs/emulator_merged_vmux.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9527777777777778%*

 * *Differences: {"'tasks'": "{'LP_MODE': OrderedDict([('v_max', 2.0), ('i_config', OrderedDict([('L0', 2.1), "*

 * *            "('L1', 2.1), ('L2', 2.1)])), ('v_mux', [30, 33, 36, 37]), ('i_mux', [0, 28, 29, 30, "*

 * *            "31, 63])]), 'OVERVOLTAGE_PROTECTION': OrderedDict([('v_max', 2.0), ('i_config', "*

 * *            "OrderedDict([('L0', 2.1), ('L1', 2.1), ('L2', 2.1)])), ('i_ovp', OrderedDict([('L0', "*

 * *            "5.0), ('L1', 7.0), ('L2', 7.0)])), ('v_mux', [30, 32, 33, 37]), ('i_mux', [28, 30, "*

 * *            '63])])}',*

 * * " […]*

```diff
@@ -229,14 +229,60 @@
             ],
             "n_meas": 5,
             "v_mux": [
                 4,
                 30
             ]
         },
+        "LP_MODE": {
+            "i_config": {
+                "L0": 2.1,
+                "L1": 2.1,
+                "L2": 2.1
+            },
+            "i_mux": [
+                0,
+                28,
+                29,
+                30,
+                31,
+                63
+            ],
+            "v_max": 2.0,
+            "v_mux": [
+                30,
+                33,
+                36,
+                37
+            ]
+        },
+        "OVERVOLTAGE_PROTECTION": {
+            "i_config": {
+                "L0": 2.1,
+                "L1": 2.1,
+                "L2": 2.1
+            },
+            "i_mux": [
+                28,
+                30,
+                63
+            ],
+            "i_ovp": {
+                "L0": 5.0,
+                "L1": 7.0,
+                "L2": 7.0
+            },
+            "v_max": 2.0,
+            "v_mux": [
+                30,
+                32,
+                33,
+                37
+            ]
+        },
         "SLDO": {
             "extra_i": [],
             "i_max": {
                 "L0": 9.75,
                 "L1": 10.6,
                 "L2": 9.48
             },
@@ -289,14 +335,16 @@
                 "stop": 4000
             }
         }
     },
     "yarr": {
         "connectivity": "src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json",
         "controller": "configs/controller/emuCfg_rd53a.json",
+        "lpm_digitalscan": "configs/scans/rd53b/lpm_digitalscan.json",
         "read_adc_exe": "emulator-read-adc",
         "read_ringosc_exe": "emulator-read-ringosc",
         "run_dir": "emulator",
         "scanConsole_exe": "emulator-scanConsole",
+        "switchLPM_exe": "emulator-switch-lpm",
         "write_register_exe": "emulator-write-register"
     }
 }
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/configs/example_merged_vmux.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/configs/example_merged_vmux.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'tasks'": "{'LP_MODE': OrderedDict([('v_max', 2.0), ('i_config', OrderedDict([('L0', 2.1), "*

 * *            "('L1', 2.1), ('L2', 2.1)])), ('v_mux', [30, 33, 36, 37]), ('i_mux', [0, 28, 29, 30, "*

 * *            "31, 63])]), 'OVERVOLTAGE_PROTECTION': OrderedDict([('v_max', 3), ('i_config', "*

 * *            "OrderedDict([('L0', 2.1), ('L1', 2.1), ('L2', 2.1)])), ('i_ovp', OrderedDict([('L0', "*

 * *            "5.0), ('L1', 7.0), ('L2', 7.0)])), ('v_mux', [30, 32, 33, 37]), ('i_mux', [0, 28, 30, "*

 * *            '63])])}',*

 * *  […]*

```diff
@@ -235,14 +235,61 @@
             ],
             "n_meas": 5,
             "v_mux": [
                 4,
                 30
             ]
         },
+        "LP_MODE": {
+            "i_config": {
+                "L0": 2.1,
+                "L1": 2.1,
+                "L2": 2.1
+            },
+            "i_mux": [
+                0,
+                28,
+                29,
+                30,
+                31,
+                63
+            ],
+            "v_max": 2.0,
+            "v_mux": [
+                30,
+                33,
+                36,
+                37
+            ]
+        },
+        "OVERVOLTAGE_PROTECTION": {
+            "i_config": {
+                "L0": 2.1,
+                "L1": 2.1,
+                "L2": 2.1
+            },
+            "i_mux": [
+                0,
+                28,
+                30,
+                63
+            ],
+            "i_ovp": {
+                "L0": 5.0,
+                "L1": 7.0,
+                "L2": 7.0
+            },
+            "v_max": 3,
+            "v_mux": [
+                30,
+                32,
+                33,
+                37
+            ]
+        },
         "SLDO": {
             "extra_i": [],
             "i_max": {
                 "L0": 9.75,
                 "L1": 10.6,
                 "L2": 9.48
             },
@@ -294,14 +341,16 @@
                 "step": 100,
                 "stop": 4000
             }
         }
     },
     "yarr": {
         "controller": "configs/controller/specCfg-rd53b-16x1.json",
+        "lpm_digitalscan": "configs/scans/rd53b/lpm_digitalscan.json",
         "read_adc_exe": "./bin/read-adc",
         "read_ringosc_exe": "./bin/rd53bReadRingosc",
         "run_dir": "../Yarr",
         "scanConsole_exe": "./bin/scanConsole",
+        "switchLPM_exe": "./bin/switchLPM",
         "write_register_exe": "./bin/write-register"
     }
 }
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/configs/example_separate_vmux.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/configs/example_separate_vmux.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'tasks'": "{'LP_MODE': OrderedDict([('v_max', 2.0), ('i_config', OrderedDict([('L0', 2.1), "*

 * *            "('L1', 2.1), ('L2', 2.1)])), ('v_mux', [30, 33, 36, 37]), ('i_mux', [0, 28, 29, 30, "*

 * *            "31, 63])]), 'OVERVOLTAGE_PROTECTION': OrderedDict([('v_max', 3.0), ('i_config', "*

 * *            "OrderedDict([('L0', 2.1), ('L1', 2.1), ('L2', 2.1)])), ('i_ovp', OrderedDict([('L0', "*

 * *            "5.0), ('L1', 7.0), ('L2', 7.0)])), ('v_mux', [30, 32, 33, 37]), ('i_mux', [0, 28, 30, "*

 * *            '63])])}', […]*

```diff
@@ -238,14 +238,61 @@
             ],
             "n_meas": 5,
             "v_mux": [
                 4,
                 30
             ]
         },
+        "LP_MODE": {
+            "i_config": {
+                "L0": 2.1,
+                "L1": 2.1,
+                "L2": 2.1
+            },
+            "i_mux": [
+                0,
+                28,
+                29,
+                30,
+                31,
+                63
+            ],
+            "v_max": 2.0,
+            "v_mux": [
+                30,
+                33,
+                36,
+                37
+            ]
+        },
+        "OVERVOLTAGE_PROTECTION": {
+            "i_config": {
+                "L0": 2.1,
+                "L1": 2.1,
+                "L2": 2.1
+            },
+            "i_mux": [
+                0,
+                28,
+                30,
+                63
+            ],
+            "i_ovp": {
+                "L0": 5.0,
+                "L1": 7.0,
+                "L2": 7.0
+            },
+            "v_max": 3.0,
+            "v_mux": [
+                30,
+                32,
+                33,
+                37
+            ]
+        },
         "SLDO": {
             "extra_i": [],
             "i_max": {
                 "L0": 9.75,
                 "L1": 10.6,
                 "L2": 9.48
             },
@@ -297,14 +344,16 @@
                 "step": 100,
                 "stop": 4000
             }
         }
     },
     "yarr": {
         "controller": "configs/controller/specCfg-rd53b-16x1.json",
+        "lpm_digitalscan": "configs/scans/rd53b/lpm_digitalscan.json",
         "read_adc_exe": "./bin/read-adc",
         "read_ringosc_exe": "./bin/rd53bReadRingosc",
         "run_dir": "../Yarr",
         "scanConsole_exe": "./bin/scanConsole",
+        "switchLPM_exe": "./bin/switchLPM",
         "write_register_exe": "./bin/write-register"
     }
 }
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/module_state_template.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/module_state_template.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/ADC_CALIBRATION.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/ADC_CALIBRATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/ANALOG_READBACK.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/ANALOG_READBACK.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/SLDO.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/SLDO.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/data/schema/common.json` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/common.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/hardware_control_base.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/hardware_control_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 
 import logging
 import os
 import subprocess
 import time
 from pathlib import Path
 
-log = logging.getLogger(__name__)
+log = logging.getLogger("measurement")
 
 
 class hardware_control_base:
-    def __init__(self, config, name="hardware_control_base", verbose=False):
-        self._wd = os.getcwd()
+    def __init__(self, config, name="hardware_control_base"):
+        self._wd = Path.cwd()
         self._name = name
         self.run_dir = None
         member_variables = [
             attr
             for attr in dir(self)
             if not callable(getattr(self, attr)) and not attr.startswith("_")
         ]
-        for member in config.keys():
+        for member in config:
             if member in member_variables:
                 setattr(self, member, config[member])
 
         if self.run_dir == "emulator":
-            self.run_dir = os.getcwd()
+            self.run_dir = Path.cwd()
         else:
             self.run_dir = Path(self.run_dir)
 
     def send_command(
         self,
         cmd,
         purpose="send command",
@@ -37,27 +37,24 @@
         pause=0,
         success_code=0,
     ):
         extra_error_messages = extra_error_messages or []
 
         os.chdir(self._wd)
         os.chdir(self.run_dir)
-        result = subprocess.run(
-            cmd,
-            shell=True,
-            stdout=None if log.getEffectiveLevel() < logging.INFO else subprocess.PIPE,
-            stderr=None if log.getEffectiveLevel() < logging.INFO else subprocess.PIPE,
-        )
+        result = subprocess.run(cmd, shell=True, capture_output=True)
+        log.debug(result.stdout.decode("utf-8"))
         os.chdir(self._wd)
 
         if result.returncode != success_code:
             for extra_error_message in extra_error_messages:
                 log.info(f"[{self._name}] {extra_error_message}")
-            raise RuntimeError(f"[{self._name}] fail to {purpose}!!")
-        log.info(f"[{self._name}] {purpose}")
+            msg = f"[{self._name}] fail to {purpose}!!"
+            raise RuntimeError(msg)
+        log.debug(f"[{self._name}] {purpose}")
 
         time.sleep(pause)
 
         return result.returncode
 
     def send_command_and_read(
         self,
@@ -65,37 +62,37 @@
         type=float,
         purpose="send command and read",
         unit="",
         extra_error_messages=None,
         max_nTry=0,
         success_code=0,
     ):
-
         extra_error_messages = extra_error_messages or []
         os.chdir(self._wd)
         os.chdir(self.run_dir)
         result = subprocess.run(cmd, shell=True, stdout=subprocess.PIPE)
         os.chdir(self._wd)
 
-        log.info(result.stdout.decode())
+        log.debug(result.stdout.decode())
 
         # A while loop to retry communications in case of timeout error.
         # The maximum number of tries is determined by the function argument max_nTry.
         nTry = 0
         while result.returncode != 0 and nTry < max_nTry:
             nTry += 1
             for extra_error_message in extra_error_messages:
                 log.info(f"[{self._name}] {extra_error_message}")
             log.info(f"Try again. Send command and read attempt {nTry} time(s).")
             os.chdir(self._wd)
             os.chdir(self.run_dir)
             result = subprocess.run(cmd, shell=True, stdout=subprocess.PIPE)
             os.chdir(self._wd)
-            log.info(result.stdout.decode())
+            log.debug(result.stdout.decode())
 
         if result.returncode != success_code:
-            raise RuntimeError(f"[{self._name}] fail to {purpose}!!")
+            msg = f"[{self._name}] fail to {purpose}!!"
+            raise RuntimeError(msg)
         value = type(result.stdout.decode())
         for _extra_error_message in extra_error_messages:
             log.info(f"[{self._name}] {purpose}: {value}{unit}")
 
         return value, result.returncode
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/multimeter.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/multimeter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import logging
 
 from module_qc_tools.utils.hardware_control_base import hardware_control_base
 
-log = logging.getLogger(__name__)
+log = logging.getLogger("measurement")
 
 
 class multimeter(hardware_control_base):
     def __init__(self, config, name="multimeter", *args, **kwargs):
         self.dcv_cmd = []
         self.n_try = 0
         self.success_code = 0
         super().__init__(config, name, *args, **kwargs)
-        if any(["emulator" in dcv_cmd for dcv_cmd in self.dcv_cmd]):
+        if any("emulator" in dcv_cmd for dcv_cmd in self.dcv_cmd):
             log.info(f"[{name}] running multimeter emulator!!")
 
     def measure_dcv(self, channel=0):
-
         return self.send_command_and_read(
             self.dcv_cmd[channel],
             purpose=f"read voltage channel {channel}",
             unit="V",
             max_nTry=self.n_try,
             success_code=self.success_code,
         )
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/ntc.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/ntc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import logging
 
 from module_qc_tools.utils.hardware_control_base import hardware_control_base
 
-log = logging.getLogger(__name__)
+log = logging.getLogger("measurement")
 
 
 class ntc(hardware_control_base):
     def __init__(self, config, name="ntc", *args, **kwargs):
         self.cmd = ""
         self.n_try = 0
         self.success_code = 0
         super().__init__(config, name, *args, **kwargs)
         if "emulator" in self.cmd:
             log.info(f"[{name}] running NTC emulator!!")
 
     def read(self):
-
         return self.send_command_and_read(
             self.cmd,
             purpose="read temperature",
             unit="C",
             max_nTry=self.n_try,
             success_code=self.success_code,
         )
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/power_supply.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/power_supply.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import logging
 
 from module_qc_tools.utils.hardware_control_base import hardware_control_base
 
-log = logging.getLogger(__name__)
-logging.getLogger("module_qc_tools.utils.hardware_control_base").setLevel(logging.DEBUG)
+log = logging.getLogger("measurement")
 
 
 class power_supply(hardware_control_base):
     def __init__(self, config, name="power_supply", *args, **kwargs):
         self.on_cmd = ""
         self.off_cmd = ""
         self.set_cmd = ""
@@ -19,59 +18,55 @@
         self.n_try = 0
         self.success_code = 0
         super().__init__(config, name, *args, **kwargs)
         if "emulator" in self.on_cmd:
             log.info(f"[{name}] running power supply emulator!!")
 
     def on(self, v=None, i=None):
-
         cmd = f'{self.on_cmd.replace("{v}", str(v)).replace("{i}", str(i))}'
 
         return self.send_command(
             cmd,
             purpose=f"turn on power supply with {v}V, {i}A",
+            pause=1,
             success_code=self.success_code,
         )
 
     def set(self, v=None, i=None):
-
         cmd = f'{self.set_cmd.replace("{v}", str(v)).replace("{i}", str(i))}'
 
         return self.send_command(
             cmd,
             purpose=f"set power supply to {v}V, {i}A",
             pause=1,
             success_code=self.success_code,
         )
 
     def off(self):
-
         return self.send_command(
             self.off_cmd,
             purpose="turn off power supply",
             extra_error_messages=[
                 f"Run directory: `{self.run_dir}`"
                 f"Off command: `{self.off_cmd}`"
                 "Please manually turn off power supply!!"
             ],
             success_code=self.success_code,
         )
 
     def getV(self):
-
         return self.send_command_and_read(
             self.getV_cmd,
             purpose="read voltage",
             unit="V",
             max_nTry=self.n_try,
             success_code=self.success_code,
         )
 
     def getI(self):
-
         return self.send_command_and_read(
             self.getI_cmd,
             purpose="read current",
             unit="A",
             max_nTry=self.n_try,
             success_code=self.success_code,
         )
```

### Comparing `module_qc_tools-1.3.2rc0/src/module_qc_tools/utils/yarr.py` & `module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/yarr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,102 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
+import contextlib
 import json
 import logging
+import re
+from pathlib import Path
 
 from module_qc_tools.utils.hardware_control_base import hardware_control_base
+from module_qc_tools.utils.misc import bcolors
 
 # if sys.version_info >= (3, 9):
 #    from importlib import resources
 # else:
 #    import importlib_resources as resources
 
-log = logging.getLogger(__name__)
+log = logging.getLogger("measurement")
 
 
 class yarr(hardware_control_base):
     def __init__(self, config, name="yarr", *args, **kwargs):
         self.controller = ""
         self.connectivity = ""
         self.scanConsole_exe = ""
         self.write_register_exe = ""
         self.read_register_exe = ""
         self.read_adc_exe = ""
+        self.switchLPM_exe = ""
+        self.lpm_digitalscan = ""
         self.read_ringosc_exe = ""
         self.success_code = 0
         self.emulator = False
         super().__init__(config, name, *args, **kwargs)
         if "emulator" in self.scanConsole_exe:
             self.emulator = True
             log.info(f"[{name}] running scanConsole emulator!!")
         if "emulator" in self.write_register_exe:
             self.emulator = True
             log.info(f"[{name}] running write_register emulator!!")
+        if "emulator" in self.switchLPM_exe:
+            self.emulator = True
+            log.info(f"[{name}] running switchLPM emulator!!")
         connect_spec = self.get_connectivity()
         self._number_of_chips = len(connect_spec["chips"])
         self._disabled_chip_positions = set()
         for chip in range(self._number_of_chips):
             if not connect_spec["chips"][chip]["enable"]:
                 self._disabled_chip_positions.add(chip)
         self._register = [{} for chip in range(self._number_of_chips)]
 
     def running_emulator(self):
         return self.emulator
 
     def configure(self, skip_reset=False):
-
         cmd = f'{self.scanConsole_exe} -r {self.controller} -c {self.connectivity} {"--skip-reset" if skip_reset else ""}'
 
-        currLevel = logging.getLogger("module_qc_tools.utils").getEffectiveLevel()
-        logging.getLogger("module_qc_tools.utils").setLevel(logging.DEBUG)
+        currLevel = log.getEffectiveLevel()
+        log.setLevel(logging.DEBUG)
         # Below is the only case where success_code=1 is the default.
         # This is because the exit code of scanConsole for configuring the chip is 1 for success.
         # This will have to be removed once the YARR MR is merged (https://gitlab.cern.ch/YARR/YARR/-/issues/192).
         self.send_command(cmd, purpose="configure module", success_code=1)
-        logging.getLogger("module_qc_tools.utils").setLevel(currLevel)
+        log.setLevel(currLevel)
+
+        # Check for LP-mode
+        for handler in log.handlers:
+            if isinstance(handler, logging.FileHandler):
+                filename = handler.baseFilename
+                with Path(filename).open() as f:
+                    for line in f:
+                        if "LPM Status" in line:
+                            match = int(re.search(r":\s*(\d+)$", line).group(1))
+                            if match != 0:
+                                log.warning(
+                                    bcolors.WARNING
+                                    + "Attention! Module is in low-power mode. If this is not intended, you can turn it off by running `./bin/switchLPM off` in YARR directory"
+                                    + bcolors.ENDC
+                                )
+
         return 0
 
-    def write_register(self, name, value, chip_position=None):
+    def run_scan(self, scan, output, skip_reset=False):
+        cmd = f'{self.scanConsole_exe} -r {self.controller} -c {self.connectivity} -s {scan} -o {output} {"--skip-reset" if skip_reset else ""}'
+
+        log.info(f"Running YARR scan: {scan} ...")
+        # Always save scan output in log file
+        currLevel = log.getEffectiveLevel()
+        log.setLevel("DEBUG")
+        self.send_command(cmd, purpose="configure module", success_code=0)
+        log.setLevel(currLevel)
+
+        return 0
 
+    def write_register(self, name, value, chip_position=None):
         if chip_position in self._disabled_chip_positions:
             return 0
         if (
             chip_position is not None
             and self._register[chip_position].get(name) == value
         ):
             return 0
@@ -72,46 +107,36 @@
         else:
             for chip in range(self._number_of_chips):
                 self._register[chip][name] = value
 
         return 0
 
     def read_register(self, name, chip_position=None):
-
         if chip_position in self._disabled_chip_positions:
             return 0
         cmd = f'{self.read_register_exe} -r {self.controller} -c {self.connectivity} {"-i "+str(chip_position) if chip_position is not None else ""} {name}'
-        result = self.send_command_and_read(
+        return self.send_command_and_read(
             cmd, purpose="read register", success_code=self.success_code
         )
 
-        return result
-
     def read_adc(self, vmux, chip_position=None, readCurrent=False, rawCounts=False):
-
         if chip_position in self._disabled_chip_positions:
             return 0
-        cmd = f'{self.read_adc_exe} -r {self.controller} -c {self.connectivity} {"-i "+str(chip_position) if chip_position != None else ""} {"-I " if readCurrent else ""} {"-R " if rawCounts else ""} {vmux}'
-        result = self.send_command_and_read(
+        cmd = f'{self.read_adc_exe} -r {self.controller} -c {self.connectivity} {"-i "+str(chip_position) if chip_position is not None else ""} {"-I " if readCurrent else ""} {"-R " if rawCounts else ""} {vmux}'
+        return self.send_command_and_read(
             cmd, type=str, purpose="read adc", success_code=self.success_code
         )
 
-        return result
-
     def read_ringosc(self, name, chip_position=None):
-
         if chip_position in self._disabled_chip_positions:
             return 0
         cmd = f'{self.read_ringosc_exe} -r {self.controller} -c {self.connectivity} {"-i "+str(chip_position) if chip_position is not None else ""} {name}'
-        result = self.send_command_and_read(cmd, type=str, purpose="read ringsoc")
-
-        return result
+        return self.send_command_and_read(cmd, type=str, purpose="read ringsoc")
 
     def set_mux(self, chip_position, v_mux=-1, i_mux=-1, reset_other_chips=True):
-
         for chip in range(self._number_of_chips):
             if chip == chip_position:
                 # self.write_register(name="MonitorEnable", value=1, chip_position=str(chip))
 
                 # Set Vmux=1 to measure the I_mux pad voltage when a non-negative I_mux value is passed.
                 if i_mux >= 0:
                     v_mux = 1
@@ -128,63 +153,58 @@
                     )
             elif reset_other_chips:
                 self.write_register(name="MonitorV", value=63, chip_position=chip)
 
         return 0
 
     def reset_tempsens_enable(self, chip_position):
-
         self.write_register(
             name="MonSensSldoAnaEn", value=0, chip_position=chip_position
         )
         self.write_register(
             name="MonSensSldoDigEn", value=0, chip_position=chip_position
         )
         self.write_register(name="MonSensAcbEn", value=0, chip_position=chip_position)
 
         return 0
 
     def reset_tempsens_bias(self, chip_position):
-
         self.write_register(
             name="MonSensSldoAnaBias", value=0, chip_position=chip_position
         )
 
         self.write_register(
             name="MonSensSldoDigBias", value=0, chip_position=chip_position
         )
 
         self.write_register(name="MonSensAcbBias", value=0, chip_position=chip_position)
 
         return 0
 
     def reset_tempsens_dem(self, chip_position):
-
         self.write_register(
             name="MonSensSldoAnaDem", value=0, chip_position=chip_position
         )
 
         self.write_register(
             name="MonSensSldoDigDem", value=0, chip_position=chip_position
         )
 
         self.write_register(name="MonSensAcbDem", value=0, chip_position=chip_position)
 
         return 0
 
     def reset_tempsens(self, chip_position):
-
         self.reset_tempsens_enable(chip_position=chip_position)
         self.reset_tempsens_bias(chip_position=chip_position)
         self.reset_tempsens_dem(chip_position=chip_position)
 
         return 0
 
     def enable_tempsens(self, chip_position, v_mux=-1, reset_other_chips=True):
-
         # First reset all MOS sensors.
         self.reset_tempsens_enable(chip_position=chip_position)
         for chip in range(self._number_of_chips):
             if chip == chip_position:
                 if v_mux == 14:
                     self.write_register(
                         name="MonSensSldoAnaEn", value=1, chip_position=chip
@@ -194,26 +214,24 @@
                         name="MonSensSldoDigEn", value=1, chip_position=chip
                     )
                 elif v_mux == 18:
                     self.write_register(
                         name="MonSensAcbEn", value=1, chip_position=chip
                     )
                 else:
-                    raise RuntimeError(
-                        "Incorrect VMUX value for measuring temperature!"
-                    )
+                    msg = "Incorrect VMUX value for measuring temperature!"
+                    raise RuntimeError(msg)
             elif reset_other_chips:
                 self.reset_tempsens_enable(chip_position=chip)
 
         return 0
 
     def set_tempsens_bias(
         self, chip_position, v_mux=-1, bias=0, reset_other_chips=True
     ):
-
         for chip in range(self._number_of_chips):
             if chip == chip_position:
                 if v_mux == 14:
                     self.write_register(
                         name="MonSensSldoAnaSelBias", value=bias, chip_position=chip
                     )
                 elif v_mux == 16:
@@ -221,24 +239,22 @@
                         name="MonSensSldoDigSelBias", value=bias, chip_position=chip
                     )
                 elif v_mux == 18:
                     self.write_register(
                         name="MonSensAcbSelBias", value=bias, chip_position=chip
                     )
                 else:
-                    raise RuntimeError(
-                        "Incorrect VMUX value for measuring temperature!"
-                    )
+                    msg = "Incorrect VMUX value for measuring temperature!"
+                    raise RuntimeError(msg)
             elif reset_other_chips:
                 self.reset_tempsens(chip_position=chip)
 
         return 0
 
     def set_tempsens_dem(self, chip_position, v_mux=-1, dem=0, reset_other_chips=True):
-
         for chip in range(self._number_of_chips):
             if chip == chip_position:
                 if v_mux == 14:
                     self.write_register(
                         name="MonSensSldoAnaDem", value=dem, chip_position=chip
                     )
                 elif v_mux == 16:
@@ -246,55 +262,54 @@
                         name="MonSensSldoDigDem", value=dem, chip_position=chip
                     )
                 elif v_mux == 18:
                     self.write_register(
                         name="MonSensAcbDem", value=dem, chip_position=chip
                     )
                 else:
-                    raise RuntimeError(
-                        "Incorrect VMUX value for measuring temperature!"
-                    )
+                    msg = "Incorrect VMUX value for measuring temperature!"
+                    raise RuntimeError(msg)
             elif reset_other_chips:
                 self.reset_tempsens(chip_position=chip)
 
         return 0
 
     def set_trim(self, chip_position, v_mux=-1, trim=0, reset_other_chips=True):
-
         for chip in range(self._number_of_chips):
             if chip == chip_position:
                 if v_mux == 34:
                     self.write_register(
                         name="SldoTrimA", value=trim, chip_position=chip
                     )
                 elif v_mux == 38:
                     self.write_register(
                         name="SldoTrimD", value=trim, chip_position=chip
                     )
                 else:
-                    raise RuntimeError("Incorrect VMUX value for setting trim!")
+                    msg = "Incorrect VMUX value for setting trim!"
+                    raise RuntimeError(msg)
             elif reset_other_chips:
                 self.write_register(name="SldoTrimA", value=0, chip_position=chip)
                 self.write_register(name="SldoTrimD", value=0, chip_position=chip)
 
         return 0
 
-    def get_connectivity(self):
-        with open(self.connectivity) as file:
-            spec = json.load(file)
+    def switchLPM(self, position):
+        cmd = f"{self.switchLPM_exe} {position}"
+        return self.send_command(cmd, purpose="switch LP mode on/off")
 
-        return spec
+    def get_connectivity(self):
+        with Path(self.connectivity).open() as file:
+            return json.load(file)
 
     def get_config(self, chip_position):
         connect_spec = self.get_connectivity()
         config_path = connect_spec["chips"][chip_position]["config"]
         path = self.connectivity.rsplit("/", 1)[0] + "/" + config_path
 
-        with open(path) as file:
+        with Path(path).open() as file:
             spec = json.load(file)
 
-        try:
+        with contextlib.suppress(KeyError):
             spec["RD53B"].pop("PixelConfig")
-        except KeyError:
-            pass
 
         return spec
```

### Comparing `module_qc_tools-1.3.2rc0/.gitignore` & `module_qc_tools-1.3.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/LICENSE` & `module_qc_tools-1.3.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc0/README.md` & `module_qc_tools-1.3.2rc1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,50 @@
-# module-qc-tools v1.3.2rc0
+Metadata-Version: 2.1
+Name: module_qc_tools
+Version: 1.3.2rc1
+Summary: Module qc tools
+Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
+Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools/-/issues
+Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
+Author-email: Jay Chan <jay.chan@cern.ch>
+Maintainer-email: Giordon Stark <gstark@cern.ch>
+License: Copyright (c) 2018 The Python Packaging Authority
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: importlib-resources; python_version < '3.9'
+Requires-Dist: jsonschema
+Requires-Dist: module-qc-data-tools>=1.0.5
+Requires-Dist: numpy
+Requires-Dist: pre-commit
+Requires-Dist: requests
+Requires-Dist: tabulate
+Description-Content-Type: text/markdown
+
+# module-qc-tools v1.3.2rc1
 
 A general python tool for running ITkPixV1.1 module QC tests
 
 ## Table of contents
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
@@ -10,18 +52,21 @@
 4. [Configuration and external commands](#configuration-and-external-commands)
 5. [Measurements](#measurements)
    1. [ADC calibration](#adc-calibration)
    2. [Analog readback](#analog-readback)
    3. [SLDOVI](#sldovi)
    4. [VCal calibration](#vcal-calibration)
    5. [Injection capacitance](#injection-capacitance)
-6. [Schema check](#schema-check)
-7. [Time Estimates](#time-estimates)
-8. [Upload results to localDB](#upload-results-to-localdb)
-9. [For developer](#for-developer)
+   6. [Low Power Mode](#low-power-mode)
+   7. [Overvoltage protection](#overvoltage-protection)
+6. [Output data](#output-data)
+7. [Schema check](#schema-check)
+8. [Time Estimates](#time-estimates)
+9. [Upload results to localDB](#upload-results-to-localdb)
+10. [For developer](#for-developer)
 
 ## Requirements
 
 This tool requires users to have >= python3.7 with the following packages
 installed:
 
 - `numpy`
@@ -63,15 +108,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-tools==1.3.2rc0
+python -m pip install -U pip module-qc-tools==1.3.2rc1
 ```
 
 ## Usage
 
 After installation, one just needs to enter the virtual environment in each new
 session to use the scripts:
 
@@ -101,15 +146,18 @@
 ```json
 {
         "yarr": {
                 "run_dir": "../Yarr",
                 "controller": "configs/controller/specCfg-rd53b-16x1.json",
                 "scanConsole_exe": "./bin/scanConsole",
                 "write_register_exe": "./bin/write-register",
-                "read_adc_exe": "./bin/read-adc"
+                "read_adc_exe": "./bin/read-adc",
+                "switchLPM_exe": "./bin/switchLPM",
+                "lpm_digitalscan": "configs/scans/rd53b/lpm_digitalscan.json",
+                "read_ringosc_exe": "./bin/rd53bReadRingosc"
         },
         "power_supply": {
                 "run_dir": "../labRemote",
                 "on_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 power-on",
                 "off_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 power-off",
                 "set_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 set-current {i} {v}",
                 "getI_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 meas-current",
@@ -161,14 +209,18 @@
 - `controller`: path (relative to `run_dir` or absolute) to the controller file
 - `scanConsole_exe`: path (relative to `run_dir` or absolute) to the
   `scanConsole` executable
 - `write_register_exe`: path (relative to `run_dir` or absolute) to the
   `write_register` executable
 - `read_adc_exe`: path (relative to `run_dir` or absolute) to the `read_adc`
   executable
+- `switchLPM_exe`: path (relative to `run_dir` or absolute) to the `switchLPM`
+  executable
+- `lpm_digitalscan`: path (relative to `run_dir` or absolute) to the low-power
+  mode digital scan in YARR
 - `read_ringosc_exe`: path (relative to `run_dir` or absolute) to the
   `read_ringosc_exe` executable
 - `success_code`: exit status that indicates success. The default is 0 besides
   `configure`, which has exit status 1 for success. The user do not need to set
   the `success_code` as the default in QC software is synchronized with YARR.
 
 ### power_supply
@@ -266,28 +318,27 @@
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 $ measurement-ADC-CALIBRATION --help
-usage: measurement-ADC-CALIBRATION [-h] [-c CONFIG] [-i [INPUT_FILE [INPUT_FILE ...]]] [-o OUTPUT_DIR] [--verbose] [-m MODULE_CONNECTIVITY] [--permodule]
+usage: measurement-ADC-CALIBRATION [-h] [-c CONFIG] [-o OUTPUT_DIR] [--verbosity LEVEL] [-m MODULE_CONNECTIVITY] [--perchip]
 
 optional arguments:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         Config file
-  -i [INPUT_FILE [INPUT_FILE ...]], --input-file [INPUT_FILE [INPUT_FILE ...]]
-                        input file if exists
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
                         path to the module connectivity. Used also to identify the module SN, and to set the default output directory
-  --verbose             verbose mode
-  --permodule           Store results in one file per module (default: one file per chip)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
+  --perchip           Store results in one file per chip (default: one file per module)
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
@@ -331,30 +382,29 @@
 - `MonSensAcbDem`: Dem 0-15 for MOS sensor near center
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
-usage: measurement-ANALOG-READBACK [-h] [-c CONFIG] [-i [INPUT_FILE [INPUT_FILE ...]]] [-o OUTPUT_DIR]
-                                   [-m MODULE_CONNECTIVITY] [--verbose] [--permodule]
+usage: measurement-ANALOG-READBACK [-h] [-c CONFIG] [-o OUTPUT_DIR]
+                                   [-m MODULE_CONNECTIVITY] [--verbosity LEVEL] [--perchip]
 
 optional arguments:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         Config file
-  -i [INPUT_FILE [INPUT_FILE ...]], --input-file [INPUT_FILE [INPUT_FILE ...]]
-                        input file if exists
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
                         path to the module connectivity. Used also
                         to identify the module SN, and to set the default output directory
-  --verbose             verbose mode
-  --permodule           Store results in one file per module (default: one file per chip)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
+  --perchip           Store results in one file per chip (default: one file per module)
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
@@ -396,30 +446,29 @@
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 $ measurement-SLDO --help
-usage: measurement-SLDO [-h] [-c CONFIG] [-i [INPUT_FILE [INPUT_FILE ...]]] [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--permodule]
-                        [--verbose]
+usage: measurement-SLDO [-h] [-c CONFIG] [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--perchip]
+                        [--verbosity LEVEL]
 
 optional arguments:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         Config file
-  -i [INPUT_FILE [INPUT_FILE ...]], --input-file [INPUT_FILE [INPUT_FILE ...]]
-                        input file if exists
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
                         path to the module connectivity. Used also to identify the module SN, and to
                         set the default output directory
-  --permodule           Store results in one file per module (default: one file per chip)
-  --verbose             verbose mode
+  --perchip           Store results in one file per chip (default: one file per module)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
@@ -455,27 +504,28 @@
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 $ measurement-VCAL-CALIBRATION --help
-usage: measurement-VCAL-CALIBRATION [-h] [-c CONFIG] [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--verbose] [--permodule]
+usage: measurement-VCAL-CALIBRATION [-h] [-c CONFIG] [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--verbosity LEVEL] [--perchip]
 
 optional arguments:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         Config file
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
                         path to the module connectivity. Used also to identify the module SN, and to
                         set the default output directory
-  --verbose             verbose mode
-  --permodule           Store results in one file per module (default: one file per chip)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
+  --perchip           Store results in one file per chip (default: one file per module)
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
@@ -512,31 +562,30 @@
 - `i_mux`: list of Imux channels to be measured
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
-usage: measurement-INJECTION-CAPACITANCE [-h] [-c CONFIG] [-i [INPUT_FILE [INPUT_FILE ...]]]
-                                         [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--verbose]
-                                         [--permodule]
+usage: measurement-INJECTION-CAPACITANCE [-h] [-c CONFIG]
+                                         [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--verbosity]
+                                         [--perchip]
 
 optional arguments:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         Config file
-  -i [INPUT_FILE [INPUT_FILE ...]], --input-file [INPUT_FILE [INPUT_FILE ...]]
-                        input file if exists
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
                         path to the module connectivity. Used also
                         to identify the module SN, and to set the default output directory
-  --verbose             verbose mode
-  --permodule           Store results in one file per module (default: one file per chip)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
+  --perchip           Store results in one file per chip (default: one file per module)
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
@@ -554,26 +603,147 @@
 measurement-INJECTION-CAPACITANCE -c $(module-qc-tools
 --prefix)/configs/emulator_merged_vmux.json -o emulator/outputs/
 
 ```
 
 </details>
 
+### Low Power Mode
+
+`measurement-LP-MODE`
+
+This script will run the low power mode test (`task = LP_MODE`) as specified in
+the input configuration json file (i.e.
+`$(module-qc-tools --prefix)/configs/example_merged_vmux.json`).
+
+<details> <summary> Configuration settings </summary>
+
+- `v_max`: the voltage to be set to the power supply specific to this
+  measurement
+- `i_config`: the current at which the module should be configured specific for
+  this measurement
+- `v_mux`: list of Vmux channels to be measured
+- `i_mux`: list of Imux channels to be measured
+
+</details>
+
+<details> <summary> Help message </summary>
+
+```
+usage: measurement-LP-MODE [-h] [-c CONFIG] [-o OUTPUT_DIR]
+                                   [-m MODULE_CONNECTIVITY] [--verbosity LEVEL] [--perchip]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c CONFIG, --config CONFIG
+                        Config file
+  -o OUTPUT_DIR, --output-dir OUTPUT_DIR
+                        output directory
+  -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
+                        path to the module connectivity. Used also
+                        to identify the module SN, and to set the default output directory.
+                        Note that this measurement should be used using LP config therefore
+                        this should point to LP connectivity.
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
+  --perchip           Store results in one file per chip (default: one file per module)
+```
+
+</details>
+
+<details> <summary> Example </summary>
+
+```
+measurement-LP-MODE -c $(module-qc-tools --prefix)/configs/example_merged_vmux.json -m ~/module_data/20UPGR91301046/20UPGR91301046_L2_LP.json
+```
+
+</details>
+
+<details> <summary> Example command to run on the toy emulator </summary>
+
+```
+measurement-LP-MODE -c $(module-qc-tools --prefix)/configs/emulator_merged_vmux.json -o emulator/outputs/
+```
+
+</details>
+
+### Overvoltage Protection
+
+`measurement-OVERVOLTAGE-PROTECTION`
+
+This script will test the Overvolatge Protection (OVP)
+(`task = OVERVOLTAGE_PROTECTION`) as specified in the input configuration json
+file (i.e. `$(module-qc-tools --prefix)/configs/example_merged_vmux.json`).
+
+<details> <summary> Configuration settings </summary>
+
+- `v_max`: the voltage to be set to the power supply specific to this
+  measurement
+- `i_config`: the current at which the module should be configured specific for
+  this measurement
+- `v_mux`: list of Vmux channels to be measured
+- `i_mux`: list of Imux channels to be measured
+
+</details>
+
+<details> <summary> Help message </summary>
+
+```
+$ measurement-OVERVOLTAGE-PROTECTION --help
+usage: measurement-OVERVOLTAGE-PROTECTION [-h] [-c CONFIG] [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--perchip] [--verbosity LEVEL]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c CONFIG, --config CONFIG
+                        Config file
+  -o OUTPUT_DIR, --output-dir OUTPUT_DIR
+                        output directory
+  -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
+                        path to the module connectivity. Used also to identify the module SN, and to set the default output directory.
+                        Note that this measurement should be used using LP config therefore
+                        this should point to LP connectivity.
+  --perchip             Store results in one file per chip (default: one file per module)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
+
+```
+
+</details>
+
+<details> <summary> Example </summary>
+
+```
+measurement-OVERVOLTAGE-PROTECTION -c $(module-qc-tools --prefix)/configs/example_merged_vmux.json -m ~/module_data/20UPGR91301046/20UPGR91301046_L2_LP.json
+```
+
+</details>
+
+<details> <summary> Example command to run on the toy emulator </summary>
+
+```
+measurement-OVERVOLTAGE-PROTECTION -c $(module-qc-tools --prefix)/configs/emulator_merged_vmux.json -o emulator/outputs
+```
+
+</details>
+
 ## Output data
 
 The output of the measurements follows the structure below:
 
 ```
-|** Measurements |** <test_type> |** VCAL_CALIB |** <timestamp> |\_\_
-<chip_name/module_serial_number>.json
-
+|Measurements
+   |<test_type>
+   |VCAL_CALIB
+       |<timestamp>
+       |<YYYY-MM-DD_HHMMSS>
+           |<chip_name/module_serial_number>.json
 ```
 
 The test-type of each measuremnt is the corresponding test-code used in the
-Production Data Base. The naming iof each measuremnet script is chosen to be the
+Production Data Base. The naming of each measuremnet script is chosen to be the
 same as the test-type. The timestamp is chosen to be the start time of the
 measurement.
 
 ## Schema check
 
 The schema for the output json files is checked based on the schema files
 specified in the folder `schema`. To run the common schema check for all test
@@ -604,18 +774,20 @@
 </details>
 
 ## Time Estimates
 
 | Measurement     | Duration |
 | --------------- | -------- |
 | ADC calib       | 00:17:24 |
+| Analog Readback | 00:40:25 |
 | SLDO VI         | 00:32:00 |
 | Vcal calib      | 00:18:47 |
-| Analog Readback | 00:40:25 |
 | Injection Cap.  | 00:05:17 |
+| LP Mode         | 00:00:53 |
+| OVP             | 00:00:22 |
 
 ## Upload results to localDB
 
 The output measurement files can be uploaded to localDB using the following
 command:
 
 ```
@@ -634,16 +806,16 @@
 usage: module-qc-tools-upload [-h] [--path PATH] [--host HOST] [--port PORT] [-n]
 
 Walk through the specified directory (recursively) and attempt to submit all json files to LocalDB as the QC measurement
 
 optional arguments:
   -h, --help     show this help message and exit
   --path PATH    Path to directory with output measurement files
-  --host HOST    localDB server
-  --port PORT    localDB port
+  --host HOST    localDB server, default is localhost
+  --port PORT    localDB port, default is 5000
   -n, --dry-run  Dry-run, do not submit to localDB.
 ```
 
 </details>
 
 ## For Developer
```

### Comparing `module_qc_tools-1.3.2rc0/pyproject.toml` & `module_qc_tools-1.3.2rc1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -37,22 +37,25 @@
 
 [project.scripts]
 module-qc-tools = "module_qc_tools.cli.main:main"
 emulator-scanConsole = "module_qc_tools.cli.hardware_emulator:scanConsole"
 emulator-write-register = "module_qc_tools.cli.hardware_emulator:write_register"
 emulator-read-adc = "module_qc_tools.cli.hardware_emulator:read_adc"
 emulator-read-ringosc = "module_qc_tools.cli.hardware_emulator:read_ringosc"
+emulator-switch-lpm = "module_qc_tools.cli.hardware_emulator:switchLPM"
 emulator-control-ps = "module_qc_tools.cli.hardware_emulator:control_PS"
 emulator-measureV = "module_qc_tools.cli.hardware_emulator:measureV"
 emulator-measureT = "module_qc_tools.cli.hardware_emulator:measureT"
 measurement-ADC-CALIBRATION = "module_qc_tools.cli.ADC_CALIBRATION:main"
 measurement-ANALOG-READBACK = "module_qc_tools.cli.ANALOG_READBACK:main"
 measurement-SLDO = "module_qc_tools.cli.SLDO:main"
 measurement-VCAL-CALIBRATION = "module_qc_tools.cli.VCAL_CALIBRATION:main"
 measurement-INJECTION-CAPACITANCE = "module_qc_tools.cli.INJECTION_CAPACITANCE:main"
+measurement-LP-MODE = "module_qc_tools.cli.LP_MODE:main"
+measurement-OVERVOLTAGE-PROTECTION = "module_qc_tools.cli.OVERVOLTAGE_PROTECTION:main"
 module-qc-tools-upload = "module_qc_tools.cli.upload_localdb:main"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
@@ -89,16 +92,42 @@
 dependencies = [
     "pytest >=6",
 ]
 
 [tool.hatch.envs.dev.scripts]
 test = "pytest -ra"
 
-[tool.isort]
-profile = "black"
+[tool.ruff]
+select = [
+  "E", "F", "W", # flake8
+  "B",  "B904",  # flake8-bugbear
+  "I",           # isort
+  "ARG",         # flake8-unused-arguments
+  "C4",          # flake8-comprehensions
+  "EM",          # flake8-errmsg
+  "ICN",         # flake8-import-conventions
+  "ISC",         # flake8-implicit-str-concat
+  "PGH",         # pygrep-hooks
+  "PIE",         # flake8-pie
+  "PL",          # pylint
+  "PT",          # flake8-pytest-style
+  "PTH",         # flake8-use-pathlib
+  "RET",         # flake8-return
+  "RUF",         # Ruff-specific
+  "SIM",         # flake8-simplify
+  "T20",         # flake8-print
+  "UP",          # pyupgrade
+  "YTT",         # flake8-2020
+]
+extend-ignore = ["PLR", "E501"]
+target-version = "py37"
+src = ["src"]
+unfixable = ["T20", "F841"]
+exclude = []
+isort.required-imports = ["from __future__ import annotations"]
 
 [tool.pylint]
 master.py-version = "3.7"
 master.ignore-paths= ["src/module_qc_tools/_version.py"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
```

### Comparing `module_qc_tools-1.3.2rc0/PKG-INFO` & `module_qc_tools-1.3.2rc1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,8 @@
-Metadata-Version: 2.1
-Name: module_qc_tools
-Version: 1.3.2rc0
-Summary: Module qc tools
-Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
-Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools/-/issues
-Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
-Author-email: Jay Chan <jay.chan@cern.ch>
-Maintainer-email: Giordon Stark <gstark@cern.ch>
-License: Copyright (c) 2018 The Python Packaging Authority
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: importlib-resources; python_version < '3.9'
-Requires-Dist: jsonschema
-Requires-Dist: module-qc-data-tools>=1.0.5
-Requires-Dist: numpy
-Requires-Dist: pre-commit
-Requires-Dist: requests
-Requires-Dist: tabulate
-Description-Content-Type: text/markdown
-
-# module-qc-tools v1.3.2rc0
+# module-qc-tools v1.3.2rc1
 
 A general python tool for running ITkPixV1.1 module QC tests
 
 ## Table of contents
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
@@ -52,18 +10,21 @@
 4. [Configuration and external commands](#configuration-and-external-commands)
 5. [Measurements](#measurements)
    1. [ADC calibration](#adc-calibration)
    2. [Analog readback](#analog-readback)
    3. [SLDOVI](#sldovi)
    4. [VCal calibration](#vcal-calibration)
    5. [Injection capacitance](#injection-capacitance)
-6. [Schema check](#schema-check)
-7. [Time Estimates](#time-estimates)
-8. [Upload results to localDB](#upload-results-to-localdb)
-9. [For developer](#for-developer)
+   6. [Low Power Mode](#low-power-mode)
+   7. [Overvoltage protection](#overvoltage-protection)
+6. [Output data](#output-data)
+7. [Schema check](#schema-check)
+8. [Time Estimates](#time-estimates)
+9. [Upload results to localDB](#upload-results-to-localdb)
+10. [For developer](#for-developer)
 
 ## Requirements
 
 This tool requires users to have >= python3.7 with the following packages
 installed:
 
 - `numpy`
@@ -105,15 +66,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-tools==1.3.2rc0
+python -m pip install -U pip module-qc-tools==1.3.2rc1
 ```
 
 ## Usage
 
 After installation, one just needs to enter the virtual environment in each new
 session to use the scripts:
 
@@ -143,15 +104,18 @@
 ```json
 {
         "yarr": {
                 "run_dir": "../Yarr",
                 "controller": "configs/controller/specCfg-rd53b-16x1.json",
                 "scanConsole_exe": "./bin/scanConsole",
                 "write_register_exe": "./bin/write-register",
-                "read_adc_exe": "./bin/read-adc"
+                "read_adc_exe": "./bin/read-adc",
+                "switchLPM_exe": "./bin/switchLPM",
+                "lpm_digitalscan": "configs/scans/rd53b/lpm_digitalscan.json",
+                "read_ringosc_exe": "./bin/rd53bReadRingosc"
         },
         "power_supply": {
                 "run_dir": "../labRemote",
                 "on_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 power-on",
                 "off_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 power-off",
                 "set_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 set-current {i} {v}",
                 "getI_cmd": "./build/bin/powersupply -e ./src/configs/input-hw.json -n PS -c 1 meas-current",
@@ -203,14 +167,18 @@
 - `controller`: path (relative to `run_dir` or absolute) to the controller file
 - `scanConsole_exe`: path (relative to `run_dir` or absolute) to the
   `scanConsole` executable
 - `write_register_exe`: path (relative to `run_dir` or absolute) to the
   `write_register` executable
 - `read_adc_exe`: path (relative to `run_dir` or absolute) to the `read_adc`
   executable
+- `switchLPM_exe`: path (relative to `run_dir` or absolute) to the `switchLPM`
+  executable
+- `lpm_digitalscan`: path (relative to `run_dir` or absolute) to the low-power
+  mode digital scan in YARR
 - `read_ringosc_exe`: path (relative to `run_dir` or absolute) to the
   `read_ringosc_exe` executable
 - `success_code`: exit status that indicates success. The default is 0 besides
   `configure`, which has exit status 1 for success. The user do not need to set
   the `success_code` as the default in QC software is synchronized with YARR.
 
 ### power_supply
@@ -308,28 +276,27 @@
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 $ measurement-ADC-CALIBRATION --help
-usage: measurement-ADC-CALIBRATION [-h] [-c CONFIG] [-i [INPUT_FILE [INPUT_FILE ...]]] [-o OUTPUT_DIR] [--verbose] [-m MODULE_CONNECTIVITY] [--permodule]
+usage: measurement-ADC-CALIBRATION [-h] [-c CONFIG] [-o OUTPUT_DIR] [--verbosity LEVEL] [-m MODULE_CONNECTIVITY] [--perchip]
 
 optional arguments:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         Config file
-  -i [INPUT_FILE [INPUT_FILE ...]], --input-file [INPUT_FILE [INPUT_FILE ...]]
-                        input file if exists
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
                         path to the module connectivity. Used also to identify the module SN, and to set the default output directory
-  --verbose             verbose mode
-  --permodule           Store results in one file per module (default: one file per chip)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
+  --perchip           Store results in one file per chip (default: one file per module)
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
@@ -373,30 +340,29 @@
 - `MonSensAcbDem`: Dem 0-15 for MOS sensor near center
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
-usage: measurement-ANALOG-READBACK [-h] [-c CONFIG] [-i [INPUT_FILE [INPUT_FILE ...]]] [-o OUTPUT_DIR]
-                                   [-m MODULE_CONNECTIVITY] [--verbose] [--permodule]
+usage: measurement-ANALOG-READBACK [-h] [-c CONFIG] [-o OUTPUT_DIR]
+                                   [-m MODULE_CONNECTIVITY] [--verbosity LEVEL] [--perchip]
 
 optional arguments:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         Config file
-  -i [INPUT_FILE [INPUT_FILE ...]], --input-file [INPUT_FILE [INPUT_FILE ...]]
-                        input file if exists
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
                         path to the module connectivity. Used also
                         to identify the module SN, and to set the default output directory
-  --verbose             verbose mode
-  --permodule           Store results in one file per module (default: one file per chip)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
+  --perchip           Store results in one file per chip (default: one file per module)
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
@@ -438,30 +404,29 @@
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 $ measurement-SLDO --help
-usage: measurement-SLDO [-h] [-c CONFIG] [-i [INPUT_FILE [INPUT_FILE ...]]] [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--permodule]
-                        [--verbose]
+usage: measurement-SLDO [-h] [-c CONFIG] [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--perchip]
+                        [--verbosity LEVEL]
 
 optional arguments:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         Config file
-  -i [INPUT_FILE [INPUT_FILE ...]], --input-file [INPUT_FILE [INPUT_FILE ...]]
-                        input file if exists
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
                         path to the module connectivity. Used also to identify the module SN, and to
                         set the default output directory
-  --permodule           Store results in one file per module (default: one file per chip)
-  --verbose             verbose mode
+  --perchip           Store results in one file per chip (default: one file per module)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
@@ -497,27 +462,28 @@
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 $ measurement-VCAL-CALIBRATION --help
-usage: measurement-VCAL-CALIBRATION [-h] [-c CONFIG] [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--verbose] [--permodule]
+usage: measurement-VCAL-CALIBRATION [-h] [-c CONFIG] [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--verbosity LEVEL] [--perchip]
 
 optional arguments:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         Config file
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
                         path to the module connectivity. Used also to identify the module SN, and to
                         set the default output directory
-  --verbose             verbose mode
-  --permodule           Store results in one file per module (default: one file per chip)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
+  --perchip           Store results in one file per chip (default: one file per module)
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
@@ -554,31 +520,30 @@
 - `i_mux`: list of Imux channels to be measured
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
-usage: measurement-INJECTION-CAPACITANCE [-h] [-c CONFIG] [-i [INPUT_FILE [INPUT_FILE ...]]]
-                                         [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--verbose]
-                                         [--permodule]
+usage: measurement-INJECTION-CAPACITANCE [-h] [-c CONFIG]
+                                         [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--verbosity]
+                                         [--perchip]
 
 optional arguments:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         Config file
-  -i [INPUT_FILE [INPUT_FILE ...]], --input-file [INPUT_FILE [INPUT_FILE ...]]
-                        input file if exists
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
                         path to the module connectivity. Used also
                         to identify the module SN, and to set the default output directory
-  --verbose             verbose mode
-  --permodule           Store results in one file per module (default: one file per chip)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
+  --perchip           Store results in one file per chip (default: one file per module)
 ```
 
 </details>
 
 <details> <summary> Example </summary>
 
 ```
@@ -596,26 +561,147 @@
 measurement-INJECTION-CAPACITANCE -c $(module-qc-tools
 --prefix)/configs/emulator_merged_vmux.json -o emulator/outputs/
 
 ```
 
 </details>
 
+### Low Power Mode
+
+`measurement-LP-MODE`
+
+This script will run the low power mode test (`task = LP_MODE`) as specified in
+the input configuration json file (i.e.
+`$(module-qc-tools --prefix)/configs/example_merged_vmux.json`).
+
+<details> <summary> Configuration settings </summary>
+
+- `v_max`: the voltage to be set to the power supply specific to this
+  measurement
+- `i_config`: the current at which the module should be configured specific for
+  this measurement
+- `v_mux`: list of Vmux channels to be measured
+- `i_mux`: list of Imux channels to be measured
+
+</details>
+
+<details> <summary> Help message </summary>
+
+```
+usage: measurement-LP-MODE [-h] [-c CONFIG] [-o OUTPUT_DIR]
+                                   [-m MODULE_CONNECTIVITY] [--verbosity LEVEL] [--perchip]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c CONFIG, --config CONFIG
+                        Config file
+  -o OUTPUT_DIR, --output-dir OUTPUT_DIR
+                        output directory
+  -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
+                        path to the module connectivity. Used also
+                        to identify the module SN, and to set the default output directory.
+                        Note that this measurement should be used using LP config therefore
+                        this should point to LP connectivity.
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
+  --perchip           Store results in one file per chip (default: one file per module)
+```
+
+</details>
+
+<details> <summary> Example </summary>
+
+```
+measurement-LP-MODE -c $(module-qc-tools --prefix)/configs/example_merged_vmux.json -m ~/module_data/20UPGR91301046/20UPGR91301046_L2_LP.json
+```
+
+</details>
+
+<details> <summary> Example command to run on the toy emulator </summary>
+
+```
+measurement-LP-MODE -c $(module-qc-tools --prefix)/configs/emulator_merged_vmux.json -o emulator/outputs/
+```
+
+</details>
+
+### Overvoltage Protection
+
+`measurement-OVERVOLTAGE-PROTECTION`
+
+This script will test the Overvolatge Protection (OVP)
+(`task = OVERVOLTAGE_PROTECTION`) as specified in the input configuration json
+file (i.e. `$(module-qc-tools --prefix)/configs/example_merged_vmux.json`).
+
+<details> <summary> Configuration settings </summary>
+
+- `v_max`: the voltage to be set to the power supply specific to this
+  measurement
+- `i_config`: the current at which the module should be configured specific for
+  this measurement
+- `v_mux`: list of Vmux channels to be measured
+- `i_mux`: list of Imux channels to be measured
+
+</details>
+
+<details> <summary> Help message </summary>
+
+```
+$ measurement-OVERVOLTAGE-PROTECTION --help
+usage: measurement-OVERVOLTAGE-PROTECTION [-h] [-c CONFIG] [-o OUTPUT_DIR] [-m MODULE_CONNECTIVITY] [--perchip] [--verbosity LEVEL]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c CONFIG, --config CONFIG
+                        Config file
+  -o OUTPUT_DIR, --output-dir OUTPUT_DIR
+                        output directory
+  -m MODULE_CONNECTIVITY, --module-connectivity MODULE_CONNECTIVITY
+                        path to the module connectivity. Used also to identify the module SN, and to set the default output directory.
+                        Note that this measurement should be used using LP config therefore
+                        this should point to LP connectivity.
+  --perchip             Store results in one file per chip (default: one file per module)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default) WARNING, ERROR]
+
+```
+
+</details>
+
+<details> <summary> Example </summary>
+
+```
+measurement-OVERVOLTAGE-PROTECTION -c $(module-qc-tools --prefix)/configs/example_merged_vmux.json -m ~/module_data/20UPGR91301046/20UPGR91301046_L2_LP.json
+```
+
+</details>
+
+<details> <summary> Example command to run on the toy emulator </summary>
+
+```
+measurement-OVERVOLTAGE-PROTECTION -c $(module-qc-tools --prefix)/configs/emulator_merged_vmux.json -o emulator/outputs
+```
+
+</details>
+
 ## Output data
 
 The output of the measurements follows the structure below:
 
 ```
-|** Measurements |** <test_type> |** VCAL_CALIB |** <timestamp> |\_\_
-<chip_name/module_serial_number>.json
-
+|Measurements
+   |<test_type>
+   |VCAL_CALIB
+       |<timestamp>
+       |<YYYY-MM-DD_HHMMSS>
+           |<chip_name/module_serial_number>.json
 ```
 
 The test-type of each measuremnt is the corresponding test-code used in the
-Production Data Base. The naming iof each measuremnet script is chosen to be the
+Production Data Base. The naming of each measuremnet script is chosen to be the
 same as the test-type. The timestamp is chosen to be the start time of the
 measurement.
 
 ## Schema check
 
 The schema for the output json files is checked based on the schema files
 specified in the folder `schema`. To run the common schema check for all test
@@ -646,18 +732,20 @@
 </details>
 
 ## Time Estimates
 
 | Measurement     | Duration |
 | --------------- | -------- |
 | ADC calib       | 00:17:24 |
+| Analog Readback | 00:40:25 |
 | SLDO VI         | 00:32:00 |
 | Vcal calib      | 00:18:47 |
-| Analog Readback | 00:40:25 |
 | Injection Cap.  | 00:05:17 |
+| LP Mode         | 00:00:53 |
+| OVP             | 00:00:22 |
 
 ## Upload results to localDB
 
 The output measurement files can be uploaded to localDB using the following
 command:
 
 ```
@@ -676,16 +764,16 @@
 usage: module-qc-tools-upload [-h] [--path PATH] [--host HOST] [--port PORT] [-n]
 
 Walk through the specified directory (recursively) and attempt to submit all json files to LocalDB as the QC measurement
 
 optional arguments:
   -h, --help     show this help message and exit
   --path PATH    Path to directory with output measurement files
-  --host HOST    localDB server
-  --port PORT    localDB port
+  --host HOST    localDB server, default is localhost
+  --port PORT    localDB port, default is 5000
   -n, --dry-run  Dry-run, do not submit to localDB.
 ```
 
 </details>
 
 ## For Developer
```

