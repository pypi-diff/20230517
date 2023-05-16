# Comparing `tmp/module_qc_analysis_tools-1.3.1rc7.tar.gz` & `tmp/module_qc_analysis_tools-1.3.1rc8.tar.gz`

## Comparing `module_qc_analysis_tools-1.3.1rc7.tar` & `module_qc_analysis_tools-1.3.1rc8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/.flake8
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/.gitmodules
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/tbump.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/_version.py
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    18774 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/IV_MEASURE.py
--rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/LP_MODE.py
--rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py
--rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
--rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/SLDO.py
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/TUNING.py
--rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/__main__.py
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/globals.py
--rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/load_yarr_scans.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/main.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/overwrite_config.py
--rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/update_chip_config.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/analysis_cuts.json
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/pixel_classification.json
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/schema/info_schema.json
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
--rw-r--r--   0        0        0    26971 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/utils/analysis.py
--rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/utils/classification.py
--rw-r--r--   0        0        0    35221 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/utils/misc.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/tests/test_cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/tests/test_package.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/LICENSE
--rw-r--r--   0        0        0    21574 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/README.md
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/pyproject.toml
--rw-r--r--   0        0        0    23698 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/.flake8
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/.gitmodules
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/tbump.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/_version.py
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    22396 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/IV_MEASURE.py
+-rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/LP_MODE.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
+-rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
+-rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/TUNING.py
+-rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/__main__.py
+-rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/globals.py
+-rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/load_yarr_scans.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/main.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/overwrite_config.py
+-rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/update_chip_config.py
+-rw-r--r--   0        0        0     4804 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/analysis_cuts.json
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/pixel_classification.json
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/schema/info_schema.json
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
+-rw-r--r--   0        0        0    33126 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/utils/analysis.py
+-rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/utils/classification.py
+-rw-r--r--   0        0        0    36639 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/utils/misc.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/tests/test_cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/tests/test_package.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/LICENSE
+-rw-r--r--   0        0        0    25306 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/README.md
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/pyproject.toml
+-rw-r--r--   0        0        0    27430 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/PKG-INFO
```

### Comparing `module_qc_analysis_tools-1.3.1rc7/.gitlab-ci.yml` & `module_qc_analysis_tools-1.3.1rc8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/.pre-commit-config.yaml` & `module_qc_analysis_tools-1.3.1rc8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/tbump.toml` & `module_qc_analysis_tools-1.3.1rc8/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e33 2e31 7263 3722 0a0a  t = "1.3.1rc7"..
+00000010: 7420 3d20 2231 2e33 2e31 7263 3822 0a0a  t = "1.3.1rc8"..
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
-00000150: 2e33 2e31 7263 3720 e286 9220 7b6e 6577  .3.1rc7 ... {new
+00000150: 2e33 2e31 7263 3820 e286 9220 7b6e 6577  .3.1rc8 ... {new
 00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
 00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
 00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
 00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
 000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
 000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
 000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
```

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py`

 * *Files 12% similar despite different names*

```diff
@@ -180,14 +180,152 @@
     ax1.set_xlabel("Trim")
     ax1.set_ylabel(f"{vdd_name} (V)")
     ax1.legend()
     log.info(f" Saving {output_name}")
     fig.savefig(output_name)
 
 
+def plot_bank_vddd(rosc, vdd, rosc_name, p1, p0, bank_name, chipname, output_dir):
+    fig, ax1 = plt.subplots()
+    x_line = np.linspace(vdd[0], vdd[-1], 100)
+    for i, rosc_i in enumerate(rosc):
+        ax1.plot(vdd, rosc_i, "o", markersize=1)
+        ax1.plot(
+            x_line,
+            p1[i] * x_line + p0[i],
+            alpha=0.5,
+            label=f"{rosc_name[i]} ({p1[i]:.3e}, {p0[i]:.3e})",
+        )
+    ax1.set(
+        title=f"ROSC {bank_name} vs VDD Chip {chipname}",
+        xlabel="VDDD (V)",
+        ylabel="ROSC (MHz)",
+    )
+    ax1.legend()
+    plot_name = bank_name.replace(" ", "_")
+    log.info(f" Saving {chipname}_ROSC_vs_VDDD_{plot_name}.png")
+    fig.savefig(output_dir.joinpath(f"{chipname}_ROSC_vs_VDDD_{plot_name}.png"))
+    plt.close(fig)
+
+
+def plot_rosc_vs_vddd(rosc, vdd, chipname, output_dir, fit_method):
+    p1_list = []
+    p0_list = []
+
+    # Get SLOP and OFFSET
+    for _i, rosc_i in enumerate(rosc):
+        p1, p0 = (
+            linear_fit(vdd, rosc_i)
+            if fit_method == "root"
+            else linear_fit_np(vdd, rosc_i)
+        )
+        p1_list.append(p1)
+        p0_list.append(p0)
+
+    # Define names
+    bank_AB_name = [
+        "CLK 0",
+        "CLK 4",
+        "Inv 0",
+        "Inv 4",
+        "NAND 0",
+        "NAND 4",
+        "NOR 0",
+        "NOR 4",
+    ]
+    bank_B_FF_name = [
+        "Scan D FF 0",
+        "Scan D FF 0",
+        "D FF 0",
+        "D FF 0",
+        "Neg Edge D FF 1",
+        "Neg Edge D FF 1",
+    ]
+    bank_B_IVT_name = [
+        "LVT Inv 0",
+        "LVT Inv 4",
+        "LVT 4-input NAND 0",
+        "LVT 4-input NAND 4",
+    ]
+    bank_B_CAPA_name = [
+        "CAPA0",
+        "CAPA1",
+        "CAPA2",
+        "CAPA3",
+        "CAPA4",
+        "CAPA5",
+        "CAPA6",
+        "CAPA7",
+    ]
+
+    # Plot Bank A and Bank B
+    plot_bank_vddd(
+        rosc[:8],
+        vdd,
+        bank_AB_name,
+        p1_list[:8],
+        p0_list[:8],
+        "Bank A",
+        chipname,
+        output_dir,
+    )
+    plot_bank_vddd(
+        rosc[8:24:2],
+        vdd,
+        bank_AB_name,
+        p1_list[8:24:2],
+        p0_list[8:24:2],
+        "Bank B left",
+        chipname,
+        output_dir,
+    )
+    plot_bank_vddd(
+        rosc[9:24:2],
+        vdd,
+        bank_AB_name,
+        p1_list[9:24:2],
+        p0_list[9:24:2],
+        "Bank B right",
+        chipname,
+        output_dir,
+    )
+    plot_bank_vddd(
+        rosc[24:30],
+        vdd,
+        bank_B_FF_name,
+        p1_list[24:30],
+        p0_list[24:30],
+        "Bank B FF",
+        chipname,
+        output_dir,
+    )
+    plot_bank_vddd(
+        rosc[30:34],
+        vdd,
+        bank_B_IVT_name,
+        p1_list[30:34],
+        p0_list[30:34],
+        "Bank B LVT",
+        chipname,
+        output_dir,
+    )
+    plot_bank_vddd(
+        rosc[34:],
+        vdd,
+        bank_B_CAPA_name,
+        p1_list[34:],
+        p0_list[34:],
+        "Bank B Inj-cap-loaded 4-input NAND 4",
+        chipname,
+        output_dir,
+    )
+
+    return p1_list, p0_list
+
+
 @app.command()
 def main(
     input_meas: Path = OPTIONS["input_meas"],
     base_output_dir: Path = OPTIONS["output_dir"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
     input_layer: str = OPTIONS["layer"],
     permodule: bool = OPTIONS["permodule"],
@@ -372,42 +510,59 @@
                 data[chipname].add_parameter("AR_TEMP_NF_ASLDO", NfPar["NfASLDO"])
                 data[chipname].add_parameter("AR_TEMP_NF_DSLDO", NfPar["NfDSLDO"])
                 data[chipname].add_parameter("AR_TEMP_NF_ACB", NfPar["NfACB"])
                 data[chipname].add_parameter("AR_TEMP_POLY_TOP", EMPTY_VAL)
                 data[chipname].add_parameter("AR_TEMP_POLY_BOTTOM", EMPTY_VAL)
                 data[chipname].add_parameter("AR_TEMP_NF_TOP", EMPTY_VAL)
                 data[chipname].add_parameter("AR_TEMP_NF_BOTTOM", EMPTY_VAL)
-                data[chipname].add_parameter("AR_RING_OSCILATOR_A", [EMPTY_VAL] * 16)
-                data[chipname].add_parameter("AR_RING_OSCILATOR_B", [EMPTY_VAL] * 16)
                 # Load values to dictionary for QC analysis
                 tmpresults.update({"ChipNTC_vs_ExtExt": AR_TEMP_NTC - AR_TEMP_EXT})
                 tmpresults.update({"ASLDO_vs_ChipNTC": AR_TEMP_ASLDO - AR_TEMP_NTC})
                 tmpresults.update({"DSLDO_vs_ChipNTC": AR_TEMP_DSLDO - AR_TEMP_NTC})
                 tmpresults.update({"ACB_vs_ChipNTC": AR_TEMP_ACB - AR_TEMP_NTC})
 
             elif inputDF._subtestType == "AR_VDD":
                 vdda = calculated_data["VDDA"]["Values"].tolist()
                 vddd = calculated_data["VDDD"]["Values"].tolist()
                 trimA = calculated_data["SldoTrimA"]["Values"].tolist()
                 trimD = calculated_data["SldoTrimD"]["Values"].tolist()
-                # Add parameters for output file
-                data[chipname].add_parameter("AR_VDDA_VS_TRIM", round_list(vdda, 4))
-                data[chipname].add_parameter("AR_VDDD_VS_TRIM", round_list(vddd, 4))
                 output_name_vdda = output_dir.joinpath(f"{chipname}_VDDA_TRIM.png")
                 output_name_vddd = output_dir.joinpath(f"{chipname}_VDDD_TRIM.png")
+
+                # Plot VDDA/VDDD vs Trim
                 plot_vdd_vs_trim(
                     trimA, vdda, "VDDA", output_name_vdda, chipname, fit_method.value
                 )
                 plot_vdd_vs_trim(
                     trimD, vddd, "VDDD", output_name_vddd, chipname, fit_method.value
                 )
+
+                # Plot ROSC vs VDDD
+                rosc_list = [
+                    calculated_data[f"ROSC{i}"]["Values"].tolist() for i in range(1, 42)
+                ]
+                p1_list, p0_list = plot_rosc_vs_vddd(
+                    rosc_list,
+                    vddd,
+                    chipname,
+                    output_dir,
+                    fit_method.value,
+                )
+
+                # Add parameters for output file
+                data[chipname].add_parameter("AR_VDDA_VS_TRIM", round_list(vdda, 4))
+                data[chipname].add_parameter("AR_VDDD_VS_TRIM", round_list(vddd, 4))
+                data[chipname].add_parameter("AR_ROSC_SLOPE", round_list(p1_list, 4))
+                data[chipname].add_parameter("AR_ROSC_OFFSET", round_list(p0_list, 4))
+
                 # Load values to dictionary for QC analysis
                 tmpresults.update({"AR_VDDA_VS_TRIM": round_list(vdda, 4)})
                 tmpresults.update({"AR_VDDD_VS_TRIM": round_list(vddd, 4)})
-
+                tmpresults.update({"AR_ROSC_SLOPE": round_list(p1_list, 4)})
+                tmpresults.update({"AR_ROSC_OFFSET": round_list(p0_list, 4)})
             else:
                 log.warning(
                     bcolors.WARNING
                     + f"{filename}.json does not have any required subtestType. Skipping."
                     + bcolors.ENDC
                 )
                 continue
```

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/IV_MEASURE.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/IV_MEASURE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/LP_MODE.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/LP_MODE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/SLDO.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/SLDO.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/TUNING.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/TUNING.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/globals.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     readable=True,
     resolve_path=True,
 )
 OPTIONS["layer"]: str = typer.Option(
     "Unknown",
     "-l",
     "--layer",
-    help="Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2 (default)",
+    help="Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2 (default is automatically determined from the module SN)",
 )
 OPTIONS["moduleSN"]: str = typer.Option(
     ...,
     "-m",
     "--moduleSN",
     help="Module serial number",
 )
@@ -166,15 +166,15 @@
     writable=True,
     resolve_path=True,
 )
 OPTIONS["config_type"]: str = typer.Option(
     "",
     "-t",
     "--config-type",
-    help="The config type to be modified. E.g. E.g. L2_warm/l2_cold.",
+    help="The config type to be modified. E.g. L2_warm/L2_cold.",
 )
 OPTIONS["override"]: bool = typer.Option(
     False,
     help="Update chip configuration even if the chip failed QC",
 )
 OPTIONS["output_yarr"]: str = typer.Option(
     None,
```

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/load_yarr_scans.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/load_yarr_scans.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/main.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/overwrite_config.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/overwrite_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/update_chip_config.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/update_chip_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/analysis_cuts.json` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/analysis_cuts.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9907407407407408%*

 * *Differences: {"'ANALOG_READBACK'": "{'AR_ROSC_SLOPE': [600, 1800], 'AR_ROSC_OFFSET': [-1200, -300]}"}*

```diff
@@ -128,14 +128,22 @@
                 0.625
             ],
             "VrefOVP": [
                 1.768,
                 2.161
             ]
         },
+        "AR_ROSC_OFFSET": [
+            -1200,
+            -300
+        ],
+        "AR_ROSC_SLOPE": [
+            600,
+            1800
+        ],
         "AR_VDDA_VS_TRIM": {
             "VDD_TRIM_0": [
                 0.98355,
                 1.1593
             ],
             "VDD_step_size": [
                 0.01665,
```

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/pixel_classification.json` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/pixel_classification.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/schema/info_schema.json` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/schema/info_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/utils/analysis.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/utils/analysis.py`

 * *Files 13% similar despite different names*

```diff
@@ -251,14 +251,45 @@
                 tmp_pass_qc,
             ],
         )
 
     return pass_vdd_vs_trim_test, cell_text
 
 
+def perform_qc_analysis_AR_ROSC(_test_type, qc_config, _layer_name, results, key):
+    # QC analysis for ROSC_VS_VDDD
+    pass_rosc_vs_vddd_test = True
+
+    cell_text = np.empty(0)
+
+    lower_bound = qc_config[0]
+    upper_bound = qc_config[1]
+
+    for i in range(len(results)):
+        tmp_pass_qc = True
+        if (results[i] < lower_bound) or (results[i] > upper_bound):
+            tmp_pass_qc = False
+        if tmp_pass_qc:
+            print_output_pass(f"{key}_{i}", results[i], lower_bound, upper_bound)
+        else:
+            print_output_fail(f"{key}_{i}", results[i], lower_bound, upper_bound)
+        cell_text = np.append(
+            cell_text,
+            [
+                f"{key}_{i}",
+                round(results[i], 4),
+                f"[{lower_bound}, {upper_bound}]",
+                tmp_pass_qc,
+            ],
+        )
+        pass_rosc_vs_vddd_test = pass_rosc_vs_vddd_test and tmp_pass_qc
+
+    return pass_rosc_vs_vddd_test, cell_text
+
+
 def perform_qc_analysis(test_type, qc_selections, layer_name, results):
     log.info("")
     log.info("Performing QC analysis!")
     log.info("")
 
     check_qc_selections = qc_selections.copy()
 
@@ -307,14 +338,27 @@
                 results.get(key),
                 key,
             )
             cell_text = np.append(cell_text, new_cell_text)
             passes_qc_overall = passes_qc_overall and passes_qc_test
             continue
 
+        # Handle AR_ROSC_SLOPE and AR_ROSC_OFFSET separately
+        if ("AR_ROSC_SLOPE" in key) or ("AR_ROSC_OFFSET" in key):
+            passes_qc_test, new_cell_text = perform_qc_analysis_AR_ROSC(
+                test_type,
+                qc_selections.get(key),
+                layer_name,
+                results.get(key),
+                key,
+            )
+            cell_text = np.append(cell_text, new_cell_text)
+            passes_qc_overall = passes_qc_overall and passes_qc_test
+            continue
+
         log.debug(f" QC selections for {key}: {qc_selections.get(key)}")
         if type(qc_selections.get(key)) is list:
             if len(qc_selections.get(key)) != 2:
                 log.error(
                     bcolors.ERROR
                     + f" QC selections for {key} are ill-formatted, should be list of length 2! Please fix: {qc_selections.get(key)} . Skipping."
                     + bcolors.ENDC
@@ -464,14 +508,18 @@
     results = outputDF.get("results")
 
     # Temporary solution to avoid error when indexing array that doesn't exist
     if not results.get("AR_VDDA_VS_TRIM"):
         results.update({"AR_VDDA_VS_TRIM": [-1] * 16})
     if not results.get("AR_VDDD_VS_TRIM"):
         results.update({"AR_VDDD_VS_TRIM": [-1] * 16})
+    if not results.get("AR_ROSC_SLOPE"):
+        results.update({"AR_ROSC_SLOPE": [-1] * 41})
+    if not results.get("AR_ROSC_OFFSET"):
+        results.update({"AR_ROSC_OFFSET": [-1] * 41})
     if not results.get("AR_NOMINAL_SETTINGS"):
         results.update({"AR_NOMINAL_SETTINGS": [-1] * 72})
     analysis_version = results.get("property").get("ANALYSIS_VERSION")
     meas_version = results.get("Metadata").get("MEASUREMENT_VERSION")
 
     url = {
         "ADC_CALIBRATION": f"https://docs.google.com/forms/d/e/1FAIpQLSegDYRQ1Foe5eTuSOVZUXe0d1f_Bh5v3rhsffCnu9DUDFR69A/formResponse?usp=pp_url\
@@ -676,15 +724,97 @@
 	&entry.1293594936={results.get('AR_VDDD_VS_TRIM')[8]}\
 	&entry.2099215210={results.get('AR_VDDD_VS_TRIM')[9]}\
 	&entry.413539179={results.get('AR_VDDD_VS_TRIM')[10]}\
 	&entry.1080321692={results.get('AR_VDDD_VS_TRIM')[11]}\
 	&entry.259801418={results.get('AR_VDDD_VS_TRIM')[12]}\
 	&entry.2100743637={results.get('AR_VDDD_VS_TRIM')[13]}\
 	&entry.1600042255={results.get('AR_VDDD_VS_TRIM')[14]}\
-	&entry.50695564={results.get('AR_VDDD_VS_TRIM')[15]}",
+	&entry.50695564={results.get('AR_VDDD_VS_TRIM')[15]}\
+	&entry.1267721453={results.get('AR_ROSC_SLOPE')[0]}\
+	&entry.1108238171={results.get('AR_ROSC_SLOPE')[1]}\
+	&entry.405342661={results.get('AR_ROSC_SLOPE')[2]}\
+	&entry.2036291468={results.get('AR_ROSC_SLOPE')[3]}\
+	&entry.1125126277={results.get('AR_ROSC_SLOPE')[4]}\
+	&entry.509984940={results.get('AR_ROSC_SLOPE')[5]}\
+	&entry.1518471801={results.get('AR_ROSC_SLOPE')[6]}\
+	&entry.1010295649={results.get('AR_ROSC_SLOPE')[7]}\
+	&entry.1658294866={results.get('AR_ROSC_SLOPE')[8]}\
+	&entry.1700088219={results.get('AR_ROSC_SLOPE')[9]}\
+	&entry.1990240042={results.get('AR_ROSC_SLOPE')[10]}\
+	&entry.1994855141={results.get('AR_ROSC_SLOPE')[11]}\
+	&entry.2004501020={results.get('AR_ROSC_SLOPE')[12]}\
+	&entry.619680759={results.get('AR_ROSC_SLOPE')[13]}\
+	&entry.1547920247={results.get('AR_ROSC_SLOPE')[14]}\
+	&entry.112225409={results.get('AR_ROSC_SLOPE')[15]}\
+	&entry.8615499={results.get('AR_ROSC_SLOPE')[16]}\
+	&entry.447685801={results.get('AR_ROSC_SLOPE')[17]}\
+	&entry.948996117={results.get('AR_ROSC_SLOPE')[18]}\
+	&entry.549701779={results.get('AR_ROSC_SLOPE')[19]}\
+	&entry.2034139644={results.get('AR_ROSC_SLOPE')[20]}\
+	&entry.1738370945={results.get('AR_ROSC_SLOPE')[21]}\
+	&entry.680984854={results.get('AR_ROSC_SLOPE')[22]}\
+	&entry.380214201={results.get('AR_ROSC_SLOPE')[23]}\
+	&entry.1949714184={results.get('AR_ROSC_SLOPE')[24]}\
+	&entry.2080061991={results.get('AR_ROSC_SLOPE')[25]}\
+	&entry.1355093371={results.get('AR_ROSC_SLOPE')[26]}\
+	&entry.983676271={results.get('AR_ROSC_SLOPE')[27]}\
+	&entry.1022530148={results.get('AR_ROSC_SLOPE')[28]}\
+	&entry.2066074162={results.get('AR_ROSC_SLOPE')[29]}\
+	&entry.1683950787={results.get('AR_ROSC_SLOPE')[30]}\
+	&entry.1799042116={results.get('AR_ROSC_SLOPE')[31]}\
+	&entry.352512380={results.get('AR_ROSC_SLOPE')[32]}\
+	&entry.953608394={results.get('AR_ROSC_SLOPE')[33]}\
+	&entry.1335702676={results.get('AR_ROSC_SLOPE')[34]}\
+	&entry.1182244852={results.get('AR_ROSC_SLOPE')[35]}\
+	&entry.869372092={results.get('AR_ROSC_SLOPE')[36]}\
+	&entry.1109476155={results.get('AR_ROSC_SLOPE')[37]}\
+	&entry.696844799={results.get('AR_ROSC_SLOPE')[38]}\
+	&entry.881044474={results.get('AR_ROSC_SLOPE')[39]}\
+	&entry.210472674={results.get('AR_ROSC_SLOPE')[40]}\
+	&entry.294359514={results.get('AR_ROSC_OFFSET')[0]}\
+	&entry.218278347={results.get('AR_ROSC_OFFSET')[1]}\
+	&entry.1296340612={results.get('AR_ROSC_OFFSET')[2]}\
+	&entry.325246147={results.get('AR_ROSC_OFFSET')[3]}\
+	&entry.1461792727={results.get('AR_ROSC_OFFSET')[4]}\
+	&entry.147717067={results.get('AR_ROSC_OFFSET')[5]}\
+	&entry.308162325={results.get('AR_ROSC_OFFSET')[6]}\
+	&entry.340294729={results.get('AR_ROSC_OFFSET')[7]}\
+	&entry.1216091165={results.get('AR_ROSC_OFFSET')[8]}\
+	&entry.1537892680={results.get('AR_ROSC_OFFSET')[9]}\
+	&entry.651177331={results.get('AR_ROSC_OFFSET')[10]}\
+	&entry.346475768={results.get('AR_ROSC_OFFSET')[11]}\
+	&entry.1035896081={results.get('AR_ROSC_OFFSET')[12]}\
+	&entry.2143379250={results.get('AR_ROSC_OFFSET')[13]}\
+	&entry.923945135={results.get('AR_ROSC_OFFSET')[14]}\
+	&entry.989723257={results.get('AR_ROSC_OFFSET')[15]}\
+	&entry.971816065={results.get('AR_ROSC_OFFSET')[16]}\
+	&entry.552958174={results.get('AR_ROSC_OFFSET')[17]}\
+	&entry.739541542={results.get('AR_ROSC_OFFSET')[18]}\
+	&entry.186269499={results.get('AR_ROSC_OFFSET')[19]}\
+	&entry.502633129={results.get('AR_ROSC_OFFSET')[20]}\
+	&entry.1532319666={results.get('AR_ROSC_OFFSET')[21]}\
+	&entry.1786481368={results.get('AR_ROSC_OFFSET')[22]}\
+	&entry.921537910={results.get('AR_ROSC_OFFSET')[23]}\
+	&entry.91112264={results.get('AR_ROSC_OFFSET')[24]}\
+	&entry.1403783859={results.get('AR_ROSC_OFFSET')[25]}\
+	&entry.880466574={results.get('AR_ROSC_OFFSET')[26]}\
+	&entry.255500529={results.get('AR_ROSC_OFFSET')[27]}\
+	&entry.406968658={results.get('AR_ROSC_OFFSET')[28]}\
+	&entry.252699286={results.get('AR_ROSC_OFFSET')[29]}\
+	&entry.73007307={results.get('AR_ROSC_OFFSET')[30]}\
+	&entry.22088182={results.get('AR_ROSC_OFFSET')[31]}\
+	&entry.460622752={results.get('AR_ROSC_OFFSET')[32]}\
+	&entry.987149730={results.get('AR_ROSC_OFFSET')[33]}\
+	&entry.1559814776={results.get('AR_ROSC_OFFSET')[34]}\
+	&entry.1700713522={results.get('AR_ROSC_OFFSET')[35]}\
+	&entry.417646576={results.get('AR_ROSC_OFFSET')[36]}\
+	&entry.1968942403={results.get('AR_ROSC_OFFSET')[37]}\
+	&entry.1596668024={results.get('AR_ROSC_OFFSET')[38]}\
+	&entry.2058648829={results.get('AR_ROSC_OFFSET')[39]}\
+	&entry.1785914={results.get('AR_ROSC_OFFSET')[40]}",
     }
     log.info(
         bcolors.WARNING
         + "Copy the following URL into a browser to submit these results: \n"
         + url.get(outputDF.get("testType")).replace("\t", "")
         + "\n"
         + "View submitted results at: https://docs.google.com/spreadsheets/d/1pw_07F94fg2GJQr8wlvhaRUV63uhsAuBt_S1FEFBzBU/view"
```

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/utils/classification.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/utils/classification.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/utils/misc.py` & `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,56 @@
                     ],
                 },
                 "AR_VDD": {
                     "required_keys": [
                         "Vmux34",
                         "Vmux38",
                         "Vmux30",
+                        "ROSC0",
+                        "ROSC1",
+                        "ROSC2",
+                        "ROSC3",
+                        "ROSC4",
+                        "ROSC5",
+                        "ROSC6",
+                        "ROSC7",
+                        "ROSC8",
+                        "ROSC9",
+                        "ROSC10",
+                        "ROSC11",
+                        "ROSC12",
+                        "ROSC13",
+                        "ROSC14",
+                        "ROSC15",
+                        "ROSC16",
+                        "ROSC17",
+                        "ROSC18",
+                        "ROSC19",
+                        "ROSC20",
+                        "ROSC21",
+                        "ROSC22",
+                        "ROSC23",
+                        "ROSC24",
+                        "ROSC25",
+                        "ROSC26",
+                        "ROSC27",
+                        "ROSC28",
+                        "ROSC29",
+                        "ROSC30",
+                        "ROSC31",
+                        "ROSC32",
+                        "ROSC33",
+                        "ROSC34",
+                        "ROSC35",
+                        "ROSC36",
+                        "ROSC37",
+                        "ROSC38",
+                        "ROSC39",
+                        "ROSC40",
+                        "ROSC41",
                     ],
                 },
             },
             "OVERVOLTAGE_PROTECTION": {
                 "required_keys": [
                     "Temperature",
                     "Current",
```

### Comparing `module_qc_analysis_tools-1.3.1rc7/tests/test_cli.py` & `module_qc_analysis_tools-1.3.1rc8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/.gitignore` & `module_qc_analysis_tools-1.3.1rc8/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/LICENSE` & `module_qc_analysis_tools-1.3.1rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/README.md` & `module_qc_analysis_tools-1.3.1rc8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-analysis-tools v1.3.1rc7
+# module-qc-analysis-tools v1.3.1rc8
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -16,17 +16,19 @@
 2. [Installation](#installation)
 3. [Scripts](#scripts)
    1. [ADC calibration](#adc_calibration)
    2. [Analog readback](#analog_readback)
    3. [SLDOVI](#sldo)
    4. [VCal calibration](#vcal_calibration)
    5. [Injection capacitance](#injection_capacitance)
-   6. [Minimum health](#minimum_health)
-   7. [Tuning performance](#tuning_performance)
-   8. [Pixel failure](#pixel_failure)
+   6. [Low Power Mode](#lp_mode)
+   7. [Overvoltage Protection](#overvoltage_protection)
+   8. [Minimum health](#minimum_health)
+   9. [Tuning performance](#tuning_performance)
+   10. [Pixel failure](#pixel_failure)
 4. [Notes](#notes)
    1. [Submit QC results](#submit-qc-results)
    2. [Example commands](#example-commands-for-a-chip-in-a-quad-module-L2)
    3. [Update chip config](#update-chip-config)
    4. [Load YARR scans](#load-yarr-scans)
 5. [For developer](#for-developer)
 
@@ -69,15 +71,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc7
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc8
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
@@ -220,15 +222,15 @@
 This analysis script performs the injection capacitance. It produces several
 diagnostic plots and an output file with the measured pixel injection
 capacitance.
 
 <details> <summary> analysis-INJECTION-CAPACITANCE --help </summary>
 
 ```
-$ analysis-INJECTION-CAPACITANCE
+$ analysis-INJECTION-CAPACITANCE --help
 usage: analysis-INJECTION-CAPACITANCE [-h] -i INPUT_MEAS [-o OUTPUT_DIR] [-q QC_CRITERIA] [-l LAYER] [--permodule]
                                       [-v VERBOSITY]
 
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT_MEAS, --input-meas INPUT_MEAS
                         path to the input measurement file or directory containing input measurement files.
@@ -241,14 +243,75 @@
   --permodule           Store results in one file per module (default: one file per chip)
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
 ```
 
 </details>
 
+### `LP_MODE`
+
+This analysis script performs the Low Power mode analysis. It produces an output
+file with the measured internal voltages and currents in low power mode.
+
+<details> <summary> analysis-LP-MODE --help </summary>
+
+```
+$ analysis-LP-MODE --help
+usage: analysis-LP-MODE [-h] -i INPUT_MEAS [-o OUTPUT_DIR] [-q QC_CRITERIA] [-l LAYER] [--permodule]
+                                      [-v VERBOSITY]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i INPUT_MEAS, --input-meas INPUT_MEAS
+                        path to the input measurement file or directory containing input measurement files.
+  -o OUTPUT_DIR, --output-dir OUTPUT_DIR
+                        output directory
+  -q QC_CRITERIA, --qc-criteria QC_CRITERIA
+                        path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
+  -l LAYER, --layer LAYER
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0,
+L1, L$
+  --permodule           Store results in one file per module (default: one file per chip)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default), WARNING, ERROR]
+```
+
+</details>
+
+### `OVERVOLTAGE_PROTECTION`
+
+This analysis script performs the Overvoltage protection analysis. It produces
+an output file with the measured internal voltages and currents in low power
+mode and when overvoltage protection mechanism is activated.
+
+<details> <summary> analysis-OVERVOLTAGE-PROTECTION --help </summary>
+
+```
+$ analysis-OVERVOLTAGE-PROTECTION --help
+usage: analysis-OVERVOLTAGE-PROTECTION [-h] -i INPUT_MEAS [-o OUTPUT_DIR] [-q QC_CRITERIA] [-l LAYER] [--permodule]
+                                      [-v VERBOSITY]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i INPUT_MEAS, --input-meas INPUT_MEAS
+                        path to the input measurement file or directory containing input measurement files.
+  -o OUTPUT_DIR, --output-dir OUTPUT_DIR
+                        output directory
+  -q QC_CRITERIA, --qc-criteria QC_CRITERIA
+                        path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
+  -l LAYER, --layer LAYER
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0,
+L1, L$
+  --permodule           Store results in one file per module (default: one file per chip)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default), WARNING, ERROR]
+```
+
+</details>
+
 ### `MIN_HEALTH_TEST`
 
 This analysis script performs the minimum health analysis of YARR Scans. It
 produces an output file with key parameters (number of dead/bad pixels, ...).
 Note that the YARR scans to be used in the analysis should be identified with
 `analysis-load-yarr-scans`, see [Load Yarr Scans](#load-yarr-scans).
 
@@ -271,15 +334,15 @@
                                   path to json file with pixel failure
                                   selection criteria  [default:
                                   /home/eathompson/module-qc-analysis-tools/sr
                                   c/module_qc_analysis_tools/data/pixel_classi
                                   fication.json]
   -l, --layer TEXT                Layer of module, used for applying correct
                                   QC criteria settings. Options: L0, L1, L2
-                                  (default)  [default: Unknown]
+                                  (default is automatically determined from module SN)
   -o, --output-dir PATH           output directory  [default: outputs]
   --permodule / --no-permodule    Store results in one file per module
                                   (default: one file per chip)  [default: no-
                                   permodule]
   -v, --verbosity [DEBUG|INFO|WARNING|ERROR]
                                   Log level [options: DEBUG, INFO (default)
                                   WARNING, ERROR]  [default: LogLevel.info]
@@ -313,15 +376,15 @@
                                   path to json file with pixel failure
                                   selection criteria  [default:
                                   /home/eathompson/module-qc-analysis-tools/sr
                                   c/module_qc_analysis_tools/data/pixel_classi
                                   fication.json]
   -l, --layer TEXT                Layer of module, used for applying correct
                                   QC criteria settings. Options: L0, L1, L2
-                                  (default)  [default: Unknown]
+                                  (default is automatically determined from module SN)
   -o, --output-dir PATH           output directory  [default: outputs]
   --permodule / --no-permodule    Store results in one file per module
                                   (default: one file per chip)  [default: no-
                                   permodule]
   -v, --verbosity [DEBUG|INFO|WARNING|ERROR]
                                   Log level [options: DEBUG, INFO (default)
                                   WARNING, ERROR]  [default: LogLevel.info]
@@ -356,15 +419,15 @@
                                   path to json file with pixel failure
                                   selection criteria  [default:
                                   /home/eathompson/module-qc-analysis-tools/sr
                                   c/module_qc_analysis_tools/data/pixel_classi
                                   fication.json]
   -l, --layer TEXT                Layer of module, used for applying correct
                                   QC criteria settings. Options: L0, L1, L2
-                                  (default)  [default: Unknown]
+                                  (default is automatically determined from module SN)
   -o, --output-dir PATH           output directory  [default: outputs]
   --permodule / --no-permodule    Store results in one file per module
                                   (default: one file per chip)  [default: no-
                                   permodule]
   -v, --verbosity [DEBUG|INFO|WARNING|ERROR]
                                   Log level [options: DEBUG, INFO (default)
                                   WARNING, ERROR]  [default: LogLevel.info]
@@ -386,35 +449,51 @@
 can be viewed here:
 https://docs.google.com/spreadsheets/d/1pw_07F94fg2GJQr8wlvhaRUV63uhsAuBt_S1FEFBzBU/view
 . While all submitted results will be recorded, only the latest results for each
 chip / test will be analyzed. If a mistake was realized in the submitted
 results, one can re-run the analysis and re-submit the results to overwrite the
 original results.
 
-### `Example commands for a chip in a quad module L2`
+### `Example commands for a chip in a quad module`
 
 ```
-analysis-ADC-CALIBRATION -i ../module-qc-tools/emulator/outputs/Measurements/ADC_CALIBRATION/1000000001/ --layer L2
-analysis-SLDO -i ../module-qc-tools/emulator/outputs/Measurements/SLDO/1000000001/ --layer L2
-analysis-ANALOG-READBACK -i ../module-qc-tools/emulator/outputs/Measurements/ANALOG_READBACK/1000000001/ --layer L2
-analysis-VCAL-CALIBRATION -i ../module-qc-tools/emulator/outputs/Measurements/VCAL_CALIBRATION/1000000001/ --layer L2
-analysis-INJECTION-CAPACITANCE -i ../module-qc-tools/emulator/outputs/Measurements/INJECTION_CAPACITANCE/1000000001/ --layer L2
+analysis-ADC-CALIBRATION -i ../module-qc-tools/emulator/outputs/Measurements/ADC_CALIBRATION/1000000001/
+analysis-SLDO -i ../module-qc-tools/emulator/outputs/Measurements/SLDO/1000000001/
+analysis-ANALOG-READBACK -i ../module-qc-tools/emulator/outputs/Measurements/ANALOG_READBACK/1000000001/
+analysis-VCAL-CALIBRATION -i ../module-qc-tools/emulator/outputs/Measurements/VCAL_CALIBRATION/1000000001/
+analysis-INJECTION-CAPACITANCE -i ../module-qc-tools/emulator/outputs/Measurements/INJECTION_CAPACITANCE/1000000001/
 ```
 
 ### `Update Chip Config`
 
 After each analysis, update the settings in the chip config by running:
 
 ```
 analysis-update-chip-config -i <path to analysis output directory> -c <path to YARR config directory> -t <config type>
 ```
 
 This script reads the analysis test type and update the corresponding parameters
 in the chip config.
 
+<details> <summary> analysis-update-chip-config --help </summary>
+
+```
+analysis-update-chip-config -h
+
+-i,  --input-dir                              Analysis output directory [default: None] [required]
+-c,  --config-dir                             Path to the module configuration directory to be modified [default: None] [required]
+-t,  --config-type                            The config type to be modified. E.g. L2_warm/L2_cold.
+     --override/--no-override                 Update chip configuration even if the chip failed QC [default: no-override]
+     --install-completion                     Install completion for the current shell.
+     --show-completion                        Show completion for the current shell, to copy it or customize the installation.
+-h,  --help                                   Show this message and exit.
+```
+
+</details>
+
 ### `Load YARR Scans`
 
 Before running analysis of YARR scans (`MIN_HEALTH_TEST`, `TUNING`,
 `PIXEL_FAILURE_ANALYSIS`), the YARR scans to be analyzed need to be identified.
 This is done locally using the following script:
 
 <details> <summary> analysis-load-yarr-scans --help </summary>
```

### Comparing `module_qc_analysis_tools-1.3.1rc7/pyproject.toml` & `module_qc_analysis_tools-1.3.1rc8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc7/PKG-INFO` & `module_qc_analysis_tools-1.3.1rc8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-analysis-tools
-Version: 1.3.1rc7
+Version: 1.3.1rc8
 Summary: Module qc analysis tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -34,15 +34,15 @@
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
 Requires-Dist: matplotlib
 Requires-Dist: module-qc-data-tools>=1.0.6
 Requires-Dist: numpy
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# module-qc-analysis-tools v1.3.1rc7
+# module-qc-analysis-tools v1.3.1rc8
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -56,17 +56,19 @@
 2. [Installation](#installation)
 3. [Scripts](#scripts)
    1. [ADC calibration](#adc_calibration)
    2. [Analog readback](#analog_readback)
    3. [SLDOVI](#sldo)
    4. [VCal calibration](#vcal_calibration)
    5. [Injection capacitance](#injection_capacitance)
-   6. [Minimum health](#minimum_health)
-   7. [Tuning performance](#tuning_performance)
-   8. [Pixel failure](#pixel_failure)
+   6. [Low Power Mode](#lp_mode)
+   7. [Overvoltage Protection](#overvoltage_protection)
+   8. [Minimum health](#minimum_health)
+   9. [Tuning performance](#tuning_performance)
+   10. [Pixel failure](#pixel_failure)
 4. [Notes](#notes)
    1. [Submit QC results](#submit-qc-results)
    2. [Example commands](#example-commands-for-a-chip-in-a-quad-module-L2)
    3. [Update chip config](#update-chip-config)
    4. [Load YARR scans](#load-yarr-scans)
 5. [For developer](#for-developer)
 
@@ -109,15 +111,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc7
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc8
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
@@ -260,15 +262,15 @@
 This analysis script performs the injection capacitance. It produces several
 diagnostic plots and an output file with the measured pixel injection
 capacitance.
 
 <details> <summary> analysis-INJECTION-CAPACITANCE --help </summary>
 
 ```
-$ analysis-INJECTION-CAPACITANCE
+$ analysis-INJECTION-CAPACITANCE --help
 usage: analysis-INJECTION-CAPACITANCE [-h] -i INPUT_MEAS [-o OUTPUT_DIR] [-q QC_CRITERIA] [-l LAYER] [--permodule]
                                       [-v VERBOSITY]
 
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT_MEAS, --input-meas INPUT_MEAS
                         path to the input measurement file or directory containing input measurement files.
@@ -281,14 +283,75 @@
   --permodule           Store results in one file per module (default: one file per chip)
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
 ```
 
 </details>
 
+### `LP_MODE`
+
+This analysis script performs the Low Power mode analysis. It produces an output
+file with the measured internal voltages and currents in low power mode.
+
+<details> <summary> analysis-LP-MODE --help </summary>
+
+```
+$ analysis-LP-MODE --help
+usage: analysis-LP-MODE [-h] -i INPUT_MEAS [-o OUTPUT_DIR] [-q QC_CRITERIA] [-l LAYER] [--permodule]
+                                      [-v VERBOSITY]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i INPUT_MEAS, --input-meas INPUT_MEAS
+                        path to the input measurement file or directory containing input measurement files.
+  -o OUTPUT_DIR, --output-dir OUTPUT_DIR
+                        output directory
+  -q QC_CRITERIA, --qc-criteria QC_CRITERIA
+                        path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
+  -l LAYER, --layer LAYER
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0,
+L1, L$
+  --permodule           Store results in one file per module (default: one file per chip)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default), WARNING, ERROR]
+```
+
+</details>
+
+### `OVERVOLTAGE_PROTECTION`
+
+This analysis script performs the Overvoltage protection analysis. It produces
+an output file with the measured internal voltages and currents in low power
+mode and when overvoltage protection mechanism is activated.
+
+<details> <summary> analysis-OVERVOLTAGE-PROTECTION --help </summary>
+
+```
+$ analysis-OVERVOLTAGE-PROTECTION --help
+usage: analysis-OVERVOLTAGE-PROTECTION [-h] -i INPUT_MEAS [-o OUTPUT_DIR] [-q QC_CRITERIA] [-l LAYER] [--permodule]
+                                      [-v VERBOSITY]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i INPUT_MEAS, --input-meas INPUT_MEAS
+                        path to the input measurement file or directory containing input measurement files.
+  -o OUTPUT_DIR, --output-dir OUTPUT_DIR
+                        output directory
+  -q QC_CRITERIA, --qc-criteria QC_CRITERIA
+                        path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
+  -l LAYER, --layer LAYER
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0,
+L1, L$
+  --permodule           Store results in one file per module (default: one file per chip)
+  -v VERBOSITY, --verbosity VERBOSITY
+                        Log level [options: DEBUG, INFO (default), WARNING, ERROR]
+```
+
+</details>
+
 ### `MIN_HEALTH_TEST`
 
 This analysis script performs the minimum health analysis of YARR Scans. It
 produces an output file with key parameters (number of dead/bad pixels, ...).
 Note that the YARR scans to be used in the analysis should be identified with
 `analysis-load-yarr-scans`, see [Load Yarr Scans](#load-yarr-scans).
 
@@ -311,15 +374,15 @@
                                   path to json file with pixel failure
                                   selection criteria  [default:
                                   /home/eathompson/module-qc-analysis-tools/sr
                                   c/module_qc_analysis_tools/data/pixel_classi
                                   fication.json]
   -l, --layer TEXT                Layer of module, used for applying correct
                                   QC criteria settings. Options: L0, L1, L2
-                                  (default)  [default: Unknown]
+                                  (default is automatically determined from module SN)
   -o, --output-dir PATH           output directory  [default: outputs]
   --permodule / --no-permodule    Store results in one file per module
                                   (default: one file per chip)  [default: no-
                                   permodule]
   -v, --verbosity [DEBUG|INFO|WARNING|ERROR]
                                   Log level [options: DEBUG, INFO (default)
                                   WARNING, ERROR]  [default: LogLevel.info]
@@ -353,15 +416,15 @@
                                   path to json file with pixel failure
                                   selection criteria  [default:
                                   /home/eathompson/module-qc-analysis-tools/sr
                                   c/module_qc_analysis_tools/data/pixel_classi
                                   fication.json]
   -l, --layer TEXT                Layer of module, used for applying correct
                                   QC criteria settings. Options: L0, L1, L2
-                                  (default)  [default: Unknown]
+                                  (default is automatically determined from module SN)
   -o, --output-dir PATH           output directory  [default: outputs]
   --permodule / --no-permodule    Store results in one file per module
                                   (default: one file per chip)  [default: no-
                                   permodule]
   -v, --verbosity [DEBUG|INFO|WARNING|ERROR]
                                   Log level [options: DEBUG, INFO (default)
                                   WARNING, ERROR]  [default: LogLevel.info]
@@ -396,15 +459,15 @@
                                   path to json file with pixel failure
                                   selection criteria  [default:
                                   /home/eathompson/module-qc-analysis-tools/sr
                                   c/module_qc_analysis_tools/data/pixel_classi
                                   fication.json]
   -l, --layer TEXT                Layer of module, used for applying correct
                                   QC criteria settings. Options: L0, L1, L2
-                                  (default)  [default: Unknown]
+                                  (default is automatically determined from module SN)
   -o, --output-dir PATH           output directory  [default: outputs]
   --permodule / --no-permodule    Store results in one file per module
                                   (default: one file per chip)  [default: no-
                                   permodule]
   -v, --verbosity [DEBUG|INFO|WARNING|ERROR]
                                   Log level [options: DEBUG, INFO (default)
                                   WARNING, ERROR]  [default: LogLevel.info]
@@ -426,35 +489,51 @@
 can be viewed here:
 https://docs.google.com/spreadsheets/d/1pw_07F94fg2GJQr8wlvhaRUV63uhsAuBt_S1FEFBzBU/view
 . While all submitted results will be recorded, only the latest results for each
 chip / test will be analyzed. If a mistake was realized in the submitted
 results, one can re-run the analysis and re-submit the results to overwrite the
 original results.
 
-### `Example commands for a chip in a quad module L2`
+### `Example commands for a chip in a quad module`
 
 ```
-analysis-ADC-CALIBRATION -i ../module-qc-tools/emulator/outputs/Measurements/ADC_CALIBRATION/1000000001/ --layer L2
-analysis-SLDO -i ../module-qc-tools/emulator/outputs/Measurements/SLDO/1000000001/ --layer L2
-analysis-ANALOG-READBACK -i ../module-qc-tools/emulator/outputs/Measurements/ANALOG_READBACK/1000000001/ --layer L2
-analysis-VCAL-CALIBRATION -i ../module-qc-tools/emulator/outputs/Measurements/VCAL_CALIBRATION/1000000001/ --layer L2
-analysis-INJECTION-CAPACITANCE -i ../module-qc-tools/emulator/outputs/Measurements/INJECTION_CAPACITANCE/1000000001/ --layer L2
+analysis-ADC-CALIBRATION -i ../module-qc-tools/emulator/outputs/Measurements/ADC_CALIBRATION/1000000001/
+analysis-SLDO -i ../module-qc-tools/emulator/outputs/Measurements/SLDO/1000000001/
+analysis-ANALOG-READBACK -i ../module-qc-tools/emulator/outputs/Measurements/ANALOG_READBACK/1000000001/
+analysis-VCAL-CALIBRATION -i ../module-qc-tools/emulator/outputs/Measurements/VCAL_CALIBRATION/1000000001/
+analysis-INJECTION-CAPACITANCE -i ../module-qc-tools/emulator/outputs/Measurements/INJECTION_CAPACITANCE/1000000001/
 ```
 
 ### `Update Chip Config`
 
 After each analysis, update the settings in the chip config by running:
 
 ```
 analysis-update-chip-config -i <path to analysis output directory> -c <path to YARR config directory> -t <config type>
 ```
 
 This script reads the analysis test type and update the corresponding parameters
 in the chip config.
 
+<details> <summary> analysis-update-chip-config --help </summary>
+
+```
+analysis-update-chip-config -h
+
+-i,  --input-dir                              Analysis output directory [default: None] [required]
+-c,  --config-dir                             Path to the module configuration directory to be modified [default: None] [required]
+-t,  --config-type                            The config type to be modified. E.g. L2_warm/L2_cold.
+     --override/--no-override                 Update chip configuration even if the chip failed QC [default: no-override]
+     --install-completion                     Install completion for the current shell.
+     --show-completion                        Show completion for the current shell, to copy it or customize the installation.
+-h,  --help                                   Show this message and exit.
+```
+
+</details>
+
 ### `Load YARR Scans`
 
 Before running analysis of YARR scans (`MIN_HEALTH_TEST`, `TUNING`,
 `PIXEL_FAILURE_ANALYSIS`), the YARR scans to be analyzed need to be identified.
 This is done locally using the following script:
 
 <details> <summary> analysis-load-yarr-scans --help </summary>
```

