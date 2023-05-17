# Comparing `tmp/cosapp-0.13.1.tar.gz` & `tmp/cosapp-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosapp-0.13.1.tar", last modified: Mon Apr  3 13:55:58 2023, max compression
+gzip compressed data, was "cosapp-0.14.0.tar", last modified: Wed May 17 16:52:54 2023, max compression
```

## Comparing `cosapp-0.13.1.tar` & `cosapp-0.14.0.tar`

### file list

```diff
@@ -1,490 +1,445 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.307814 cosapp-0.13.1/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-04-03 13:55:20.000000 cosapp-0.13.1/AUTHORS.md
--rw-rw-rw-   0 root         (0) root         (0)     3488 2023-04-03 13:55:20.000000 cosapp-0.13.1/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)    37745 2023-04-03 13:55:20.000000 cosapp-0.13.1/HISTORY.md
--rw-rw-rw-   0 root         (0) root         (0)     6572 2023-04-03 13:55:20.000000 cosapp-0.13.1/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      756 2023-04-03 13:55:20.000000 cosapp-0.13.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    40207 2023-04-03 13:55:58.307814 cosapp-0.13.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-04-03 13:55:20.000000 cosapp-0.13.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.143801 cosapp-0.13.1/cosapp/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.146802 cosapp-0.13.1/cosapp/base/
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.148802 cosapp-0.13.1/cosapp/core/
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4354 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/configuration_schema.json
--rw-rw-rw-   0 root         (0) root         (0)    18754 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/eval_str.py
--rw-rw-rw-   0 root         (0) root         (0)    15279 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.151802 cosapp-0.13.1/cosapp/core/numerics/
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/numerics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27230 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/numerics/basics.py
--rw-rw-rw-   0 root         (0) root         (0)    27969 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/numerics/boundary.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/numerics/enum.py
--rw-rw-rw-   0 root         (0) root         (0)    13455 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/numerics/residues.py
--rw-rw-rw-   0 root         (0) root         (0)    19400 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/numerics/root.py
--rw-rw-rw-   0 root         (0) root         (0)    15550 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/numerics/sobol_seq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.152802 cosapp-0.13.1/cosapp/core/signal/
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/signal/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4972 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/signal/signal.py
--rw-rw-rw-   0 root         (0) root         (0)     1812 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/signal/slot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.156802 cosapp-0.13.1/cosapp/core/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8079 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    15027 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/tests/test_AssignString.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/tests/test_ContextLocals.py
--rw-rw-rw-   0 root         (0) root         (0)    12340 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/tests/test_EvalString.py
--rw-rw-rw-   0 root         (0) root         (0)    12359 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/tests/test_Module.py
--rw-rw-rw-   0 root         (0) root         (0)     6502 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/tests/test_coSAppConfiguration.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/tests/test_time.py
--rw-rw-rw-   0 root         (0) root         (0)     2013 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/core/variableref.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.162803 cosapp-0.13.1/cosapp/drivers/
--rw-rw-rw-   0 root         (0) root         (0)      936 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3031 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/abstractsetofcases.py
--rw-rw-rw-   0 root         (0) root         (0)    12048 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/abstractsolver.py
--rw-rw-rw-   0 root         (0) root         (0)     8607 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/driver.py
--rw-rw-rw-   0 root         (0) root         (0)     9484 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/influence.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/iterativecase.py
--rw-rw-rw-   0 root         (0) root         (0)     2867 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/lineardoe.py
--rw-rw-rw-   0 root         (0) root         (0)     3131 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/metasystembuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    10683 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/montecarlo.py
--rw-rw-rw-   0 root         (0) root         (0)    26507 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/nonlinearsolver.py
--rw-rw-rw-   0 root         (0) root         (0)    22309 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/optimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/optionaldriver.py
--rw-rw-rw-   0 root         (0) root         (0)     6655 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/runonce.py
--rw-rw-rw-   0 root         (0) root         (0)    11447 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/runsinglecase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.164803 cosapp-0.13.1/cosapp/drivers/time/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1017 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/euler.py
--rw-rw-rw-   0 root         (0) root         (0)    19963 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3457 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/runge_kutta.py
--rw-rw-rw-   0 root         (0) root         (0)    13729 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/scenario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.172803 cosapp-0.13.1/cosapp/drivers/time/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15016 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     6501 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_BouncingBall.py
--rw-rw-rw-   0 root         (0) root         (0)     2599 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_DiscreteStepper.py
--rw-rw-rw-   0 root         (0) root         (0)     4202 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_EulerExplicit.py
--rw-rw-rw-   0 root         (0) root         (0)    18994 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_ExplicitTimeDriver.py
--rw-rw-rw-   0 root         (0) root         (0)     1501 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_InterpolAssignString.py
--rw-rw-rw-   0 root         (0) root         (0)     2419 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_Interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     5336 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_NewtonPendulum.py
--rw-rw-rw-   0 root         (0) root         (0)    25908 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_RungeKutta.py
--rw-rw-rw-   0 root         (0) root         (0)    22334 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_Scenario.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_SystemInterpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     1633 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_TimeAssignString.py
--rw-rw-rw-   0 root         (0) root         (0)     4551 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_TimeStepManager.py
--rw-rw-rw-   0 root         (0) root         (0)     8108 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_TimeUnknownDict.py
--rw-rw-rw-   0 root         (0) root         (0)     4478 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_TimeUnknownStack.py
--rw-rw-rw-   0 root         (0) root         (0)     2914 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_TimeVarManager.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_TwoPointCubicInterpolator.py
--rw-rw-rw-   0 root         (0) root         (0)      771 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_TwoPointCubicPolynomial.py
--rw-rw-rw-   0 root         (0) root         (0)     9926 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_event_cascades.py
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/tests/test_modevar_init.py
--rw-rw-rw-   0 root         (0) root         (0)    21544 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/time/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    15033 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1657 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/drivers/validitycheck.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.173804 cosapp-0.13.1/cosapp/multimode/
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/multimode/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5937 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/multimode/discreteStepper.py
--rw-rw-rw-   0 root         (0) root         (0)    11879 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/multimode/event.py
--rw-rw-rw-   0 root         (0) root         (0)     2503 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/multimode/zeroCrossing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.175804 cosapp-0.13.1/cosapp/patterns/
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/patterns/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3411 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/patterns/observer.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/patterns/singleton.py
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/patterns/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.178804 cosapp-0.13.1/cosapp/ports/
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/ports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16228 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/ports/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/ports/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/ports/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4019 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/ports/mode_variable.py
--rw-rw-rw-   0 root         (0) root         (0)    33760 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/ports/port.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/ports/unit_library.ini
--rw-rw-rw-   0 root         (0) root         (0)    33349 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/ports/units.py
--rw-rw-rw-   0 root         (0) root         (0)    31409 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/ports/variable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.180804 cosapp-0.13.1/cosapp/recorders/
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/recorders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4628 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/recorders/dataframe_recorder.py
--rw-rw-rw-   0 root         (0) root         (0)     7847 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/recorders/dsv_recorder.py
--rw-rw-rw-   0 root         (0) root         (0)    13366 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/recorders/recorder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.183804 cosapp-0.13.1/cosapp/systems/
--rw-rw-rw-   0 root         (0) root         (0)      741 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/systems/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6623 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/systems/externalsystem.py
--rw-rw-rw-   0 root         (0) root         (0)    13327 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/systems/metamodels.py
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/systems/processsystem.py
--rw-rw-rw-   0 root         (0) root         (0)   130933 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/systems/system.py
--rw-rw-rw-   0 root         (0) root         (0)     3095 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/systems/system.schema.json
--rw-rw-rw-   0 root         (0) root         (0)     3122 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/systems/systemConnector.py
--rw-rw-rw-   0 root         (0) root         (0)    15645 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/systems/systemSurrogate.py
--rw-rw-rw-   0 root         (0) root         (0)     5515 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/systems/systemfamily.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.188805 cosapp-0.13.1/cosapp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/all_tests.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.195805 cosapp-0.13.1/cosapp/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/default_dataframe.json
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/export_doe.cs
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/export_doe.csv
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/export_doe.json
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/export_doe.txt
--rw-rw-rw-   0 root         (0) root         (0)     1701 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config.json
--rw-rw-rw-   0 root         (0) root         (0)      738 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config_ducts.json
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config_pressureloss.json
--rw-rw-rw-   0 root         (0) root         (0)      312 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config_pressureloss1.json
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config_pressureloss11.json
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config_pressureloss11bis.json
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config_pressureloss12.json
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config_pressureloss121.json
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config_pressureloss131.json
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config_pressureloss2.json
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config_pressureloss22.json
--rw-rw-rw-   0 root         (0) root         (0)     2537 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config_pressureloss222.json
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/data/system_config_pressureloss2tank.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.196805 cosapp-0.13.1/cosapp/tests/library/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/library/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/library/ports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.199806 cosapp-0.13.1/cosapp/tests/library/systems/
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/library/systems/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7259 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/library/systems/basicalgebra.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/library/systems/dynamics.py
--rw-rw-rw-   0 root         (0) root         (0)     3257 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/library/systems/elec.py
--rw-rw-rw-   0 root         (0) root         (0)     8536 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/library/systems/multiply.py
--rw-rw-rw-   0 root         (0) root         (0)    12162 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/library/systems/others.py
--rw-rw-rw-   0 root         (0) root         (0)     4826 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/library/systems/pressurelossvarious.py
--rw-rw-rw-   0 root         (0) root         (0)     1986 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/library/systems/vectors.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/test_ComplexDuct.py
--rw-rw-rw-   0 root         (0) root         (0)    10101 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/test_MathematicalProblem_integration.py
--rw-rw-rw-   0 root         (0) root         (0)    10645 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/test_Turbofan.py
--rw-rw-rw-   0 root         (0) root         (0)     3960 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/test_dynamics.py
--rw-rw-rw-   0 root         (0) root         (0)     6650 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/test_electric_circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     9228 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/test_multimode.py
--rw-rw-rw-   0 root         (0) root         (0)     8095 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/test_system_pressureloss.py
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/test_tutorials.py
--rw-rw-rw-   0 root         (0) root         (0)    11887 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/test_unknown_aliasing.py
--rw-rw-rw-   0 root         (0) root         (0)     5568 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tests/test_visitor_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.200806 cosapp-0.13.1/cosapp/tools/
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.201806 cosapp-0.13.1/cosapp/tools/fmu/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/fmu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22009 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/fmu/exporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3204 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/fmu/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.203806 cosapp-0.13.1/cosapp/tools/fmu/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/fmu/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2606 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/fmu/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    13896 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/fmu/tests/test_exporter.py
--rw-rw-rw-   0 root         (0) root         (0)     1686 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/fmu/tests/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     4104 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/help.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.203806 cosapp-0.13.1/cosapp/tools/module_parser/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/module_parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13683 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/module_parser/parseModule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.205806 cosapp-0.13.1/cosapp/tools/problem_viewer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7945 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/problem_viewer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.205806 cosapp-0.13.1/cosapp/tools/problem_viewer/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   250263 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/tests/test_viewmodeldata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.206806 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/
--rw-rw-rw-   0 root         (0) root         (0)     9254 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.208806 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/libs/
--rw-rw-rw-   0 root         (0) root         (0)     9483 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/libs/awesomplete.js
--rw-rw-rw-   0 root         (0) root         (0)   211120 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/libs/d3.v4.min.js
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/libs/http.js
--rw-rw-rw-   0 root         (0) root         (0)    86659 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/libs/jquery-3.2.1.min.js
--rw-rw-rw-   0 root         (0) root         (0)     4679 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/libs/vkBeautify.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.211806 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/constants.js
--rw-rw-rw-   0 root         (0) root         (0)    16285 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/draw.js
--rw-rw-rw-   0 root         (0) root         (0)     5771 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/legend.js
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/modal.js
--rw-rw-rw-   0 root         (0) root         (0)    70307 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/ptN2.js
--rw-rw-rw-   0 root         (0) root         (0)     9486 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/search.js
--rw-rw-rw-   0 root         (0) root         (0)     4155 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/svg.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.212807 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/style/
--rw-rw-rw-   0 root         (0) root         (0)     1815 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/style/awesomplete.css
--rw-rw-rw-   0 root         (0) root         (0)     5612 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/style/fontello.woff
--rw-rw-rw-   0 root         (0) root         (0)     5815 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/style/partition_tree.css
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/problem_viewer/webview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.214807 cosapp-0.13.1/cosapp/tools/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.216807 cosapp-0.13.1/cosapp/tools/templates/lib/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/templates/lib/Readme.txt
--rw-rw-rw-   0 root         (0) root         (0)   236746 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/templates/lib/d3.min.js
--rw-rw-rw-   0 root         (0) root         (0)    23777 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/templates/lib/vis.min.css
--rw-rw-rw-   0 root         (0) root         (0)   663624 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/templates/lib/vis.min.js
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/templates/pythonfmu.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.217807 cosapp-0.13.1/cosapp/tools/templates/src/
--rw-rw-rw-   0 root         (0) root         (0)     4751 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/templates/src/d3_draw.js
--rw-rw-rw-   0 root         (0) root         (0)      451 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/templates/src/d3_styles.css
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/templates/system_d3.html
--rw-rw-rw-   0 root         (0) root         (0)     8155 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/templates/system_repr.html
--rw-rw-rw-   0 root         (0) root         (0)     6675 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.219807 cosapp-0.13.1/cosapp/tools/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/views/baseRenderer.py
--rw-rw-rw-   0 root         (0) root         (0)     6755 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/views/d3js.py
--rw-rw-rw-   0 root         (0) root         (0)     4612 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/views/markdown.py
--rw-rw-rw-   0 root         (0) root         (0)    20440 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/views/prettyprint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.221807 cosapp-0.13.1/cosapp/tools/views/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/views/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2105 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/views/tests/test_VisJsRenderer.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/views/tests/test_d3.py
--rw-rw-rw-   0 root         (0) root         (0)     7823 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/views/tests/test_markdown.py
--rw-rw-rw-   0 root         (0) root         (0)     5912 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/views/tests/test_prettyprint.py
--rw-rw-rw-   0 root         (0) root         (0)    16980 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tools/views/visjs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.232808 cosapp-0.13.1/cosapp/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)     3222 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/00-Introduction.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19320 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/01-Systems.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    14666 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/02-Ports.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    18911 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/03-Drivers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2711 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/04-Triggers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17810 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/05-Validation.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10286 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/06-Visibility.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8547 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/07-Metamodels.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19784 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/08-Multipoints-Design.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    14617 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/09-MonteCarlo.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5749 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/10-Recorders.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10084 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/11-DesignMethods.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    11006 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/CustomConnectors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3536 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/FMI.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    28157 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/Guidelines.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    14967 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/HybridSimulations.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    13505 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/Logging.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4336 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/Optimization.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17402 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/SystemSurrogates.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    21247 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/SystemSurrogatesAdvanced.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17257 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/Targets.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19106 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/TimeDriver.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    16763 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/TimeDriverAdvanced.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19331 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/TipsAndTricks.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10059 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/Visitors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10314 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/aa-SimpleCircuit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/exprampode_fmu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.241809 cosapp-0.13.1/cosapp/tutorials/images/
--rw-rw-rw-   0 root         (0) root         (0)     3204 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/cosapp.svg
--rw-rw-rw-   0 root         (0) root         (0)    17745 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/design_circuit.svg
--rw-rw-rw-   0 root         (0) root         (0)    23419 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/drivers_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     6953 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/drivers_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     7366 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/drivers_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    40831 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/drivers_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     8450 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/drivers_5.svg
--rw-rw-rw-   0 root         (0) root         (0)     4537 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/drivers_nonlinear.svg
--rw-rw-rw-   0 root         (0) root         (0)     2309 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/experimental.svg
--rw-rw-rw-   0 root         (0) root         (0)    10190 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/in_progress.svg
--rw-rw-rw-   0 root         (0) root         (0)    26687 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/ports_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    19983 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/ports_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    30601 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/ports_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    16538 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/simple_circuit.svg
--rw-rw-rw-   0 root         (0) root         (0)     9156 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/systems_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    18904 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/systems_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    18945 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/systems_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    24136 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/systems_4.svg
--rw-rw-rw-   0 root         (0) root         (0)    28090 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/systems_5.svg
--rw-rw-rw-   0 root         (0) root         (0)     5070 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/tanks.svg
--rw-rw-rw-   0 root         (0) root         (0)    27536 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/triggers_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    24504 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/triggers_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6961 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/validity.svg
--rw-rw-rw-   0 root         (0) root         (0)    85431 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/images/visibility.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.243809 cosapp-0.13.1/cosapp/tutorials/multimode/
--rw-rw-rw-   0 root         (0) root         (0)     7019 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/multimode/BouncingBall.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4001 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/multimode/MultimodeOde.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5205 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/multimode/NewtonPendulum.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.243809 cosapp-0.13.1/cosapp/tutorials/optimization/
--rw-rw-rw-   0 root         (0) root         (0)     7559 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/optimization/BetzLimit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8420 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/optimization/Sellar.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4400 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/quickstart.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3233 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/tutorials/time_solutions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.249809 cosapp-0.13.1/cosapp/utils/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.250810 cosapp-0.13.1/cosapp/utils/distributions/
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/distributions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/distributions/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)     2693 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/distributions/normal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.252810 cosapp-0.13.1/cosapp/utils/distributions/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/distributions/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1809 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/distributions/tests/test_distribution.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/distributions/tests/test_normal.py
--rw-rw-rw-   0 root         (0) root         (0)     2912 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/distributions/tests/test_triangular.py
--rw-rw-rw-   0 root         (0) root         (0)     1219 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/distributions/tests/test_uniform.py
--rw-rw-rw-   0 root         (0) root         (0)     4207 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/distributions/triangular.py
--rw-rw-rw-   0 root         (0) root         (0)     2193 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/distributions/uniform.py
--rw-rw-rw-   0 root         (0) root         (0)     6715 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/find_variables.py
--rw-rw-rw-   0 root         (0) root         (0)     3677 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/graph_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4604 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/json.py
--rw-rw-rw-   0 root         (0) root         (0)    16769 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     3694 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/naming.py
--rw-rw-rw-   0 root         (0) root         (0)    14038 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/options_dictionary.py
--rw-rw-rw-   0 root         (0) root         (0)     5169 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     3856 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/pull_variables.py
--rw-rw-rw-   0 root         (0) root         (0)     1761 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/state_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.255810 cosapp-0.13.1/cosapp/utils/surrogate_models/
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     9528 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/kriging.py
--rw-rw-rw-   0 root         (0) root         (0)    39321 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/multifi_cokriging.py
--rw-rw-rw-   0 root         (0) root         (0)     5292 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/nearest_neighbor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.257810 cosapp-0.13.1/cosapp/utils/surrogate_models/nn_interpolators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/nn_interpolators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5286 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/nn_interpolators/linear_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     3158 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/nn_interpolators/nn_base.py
--rw-rw-rw-   0 root         (0) root         (0)    18553 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/nn_interpolators/rbf_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     5287 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/nn_interpolators/weighted_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/response_surface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.258810 cosapp-0.13.1/cosapp/utils/surrogate_models/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4611 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/tests/test_kriging.py
--rw-rw-rw-   0 root         (0) root         (0)     6925 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/tests/test_multifi_cokriging.py
--rw-rw-rw-   0 root         (0) root         (0)    16170 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/tests/test_nearest_neighbor.py
--rw-rw-rw-   0 root         (0) root         (0)     3709 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/surrogate_models/tests/test_response_surface.py
--rw-rw-rw-   0 root         (0) root         (0)     7110 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/testing.py
--rw-rw-rw-   0 root         (0) root         (0)     1334 2023-04-03 13:55:20.000000 cosapp-0.13.1/cosapp/utils/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.145801 cosapp-0.13.1/cosapp.egg-info/
--rw-r--r--   0 root         (0) root         (0)    40207 2023-04-03 13:55:58.000000 cosapp-0.13.1/cosapp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15810 2023-04-03 13:55:58.000000 cosapp-0.13.1/cosapp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 13:55:58.000000 cosapp-0.13.1/cosapp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 13:55:58.000000 cosapp-0.13.1/cosapp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      247 2023-04-03 13:55:58.000000 cosapp-0.13.1/cosapp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-03 13:55:58.000000 cosapp-0.13.1/cosapp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.262810 cosapp-0.13.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     6810 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)    11424 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/contributing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.263810 cosapp-0.13.1/docs/cosapp_theme/
--rw-rw-rw-   0 root         (0) root         (0)     2422 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/layout.html
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/searchbox.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.264811 cosapp-0.13.1/docs/cosapp_theme/static/
--rw-rw-rw-   0 root         (0) root         (0)     8997 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/cosapp.css_t
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.268811 cosapp-0.13.1/docs/cosapp_theme/static/css/
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/css/custom.css
--rw-rw-rw-   0 root         (0) root         (0)    31000 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/css/font-awesome.min.css
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/css/font.css
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/css/highlight.css
--rw-rw-rw-   0 root         (0) root         (0)    40062 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/css/kube.css
--rw-rw-rw-   0 root         (0) root         (0)     8764 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/css/kube.demo.css
--rw-rw-rw-   0 root         (0) root         (0)     9250 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/css/kube.legenda.css
--rw-rw-rw-   0 root         (0) root         (0)    30268 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/css/kube.min.css
--rw-rw-rw-   0 root         (0) root         (0)    26211 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/css/master.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.272811 cosapp-0.13.1/docs/cosapp_theme/static/font/
--rw-rw-rw-   0 root         (0) root         (0)   297272 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/font/Lato-Black.woff
--rw-rw-rw-   0 root         (0) root         (0)   328952 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/font/Lato-Bold.woff
--rw-rw-rw-   0 root         (0) root         (0)   347092 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/font/Lato-BoldItalic.woff
--rw-rw-rw-   0 root         (0) root         (0)   343528 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/font/Lato-Italic.woff
--rw-rw-rw-   0 root         (0) root         (0)   323172 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/font/Lato-Regular.woff
--rw-rw-rw-   0 root         (0) root         (0)   326132 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/font/Lato-Semibold.woff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.273811 cosapp-0.13.1/docs/cosapp_theme/static/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    98024 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/fonts/fontawesome-webfont.woff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.273811 cosapp-0.13.1/docs/cosapp_theme/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     5930 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/img/cosapp.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.276811 cosapp-0.13.1/docs/cosapp_theme/static/js/
--rw-rw-rw-   0 root         (0) root         (0)    84380 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/js/jquery-2.1.4.min.js
--rw-rw-rw-   0 root         (0) root         (0)    56646 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/js/kube.js
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/js/kube.legenda.js
--rw-rw-rw-   0 root         (0) root         (0)    31683 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/js/kube.min.js
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/js/master.js
--rw-rw-rw-   0 root         (0) root         (0)    12047 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/js/tocbot.min.js
--rw-rw-rw-   0 root         (0) root         (0)     5219 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/static/sidebar.js_t
--rw-rw-rw-   0 root         (0) root         (0)      736 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/cosapp_theme/theme.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.277812 cosapp-0.13.1/docs/developer/
--rw-rw-rw-   0 root         (0) root         (0)     2923 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/developer/installation_cases.rst
--rw-rw-rw-   0 root         (0) root         (0)     8633 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/developer/logger.rst
--rw-rw-rw-   0 root         (0) root         (0)     1846 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/developer/project_structure.rst
--rw-rw-rw-   0 root         (0) root         (0)    12553 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/developer/scenarii.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/history.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.278812 cosapp-0.13.1/docs/img/
--rw-rw-rw-   0 root         (0) root         (0)     2475 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/img/gitlab-cosapp-f4950f.svg
--rw-rw-rw-   0 root         (0) root         (0)     4393 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/img/website-docs-blue.svg
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/license.rst
--rw-rw-rw-   0 root         (0) root         (0)     6499 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.137801 cosapp-0.13.1/docs/nb_thumbnails/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.282812 cosapp-0.13.1/docs/nb_thumbnails/_images/
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/nb_thumbnails/_images/desktop-download.svg
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/nb_thumbnails/_images/eye.svg
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/nb_thumbnails/_images/file-code.svg
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/nb_thumbnails/_images/file-text.svg
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/nb_thumbnails/_images/fold.svg
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/nb_thumbnails/_images/package.svg
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/nb_thumbnails/_images/pencil.svg
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/nb_thumbnails/_images/play.svg
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/nb_thumbnails/_images/plug.svg
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/nb_thumbnails/_images/pulse.svg
--rw-rw-rw-   0 root         (0) root         (0)      729 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/nb_thumbnails/_images/verified.svg
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/nb_thumbnails/_images/zap.svg
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.283812 cosapp-0.13.1/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)     3694 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/source/modules.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.284812 cosapp-0.13.1/docs/tools/
--rw-rw-rw-   0 root         (0) root         (0)    12905 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tools/mermaid.py
--rw-rw-rw-   0 root         (0) root         (0)    10299 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tools/mermaid_inheritance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.295813 cosapp-0.13.1/docs/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)     3222 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/00-Introduction.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19320 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/01-Systems.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    14666 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/02-Ports.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    18911 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/03-Drivers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2711 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/04-Triggers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17810 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/05-Validation.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10286 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/06-Visibility.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8547 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/07-Metamodels.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19784 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/08-Multipoints-Design.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    14617 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/09-MonteCarlo.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5749 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/10-Recorders.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10084 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/11-DesignMethods.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    11006 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/CustomConnectors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3536 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/FMI.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    28157 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/Guidelines.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    14967 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/HybridSimulations.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    13505 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/Logging.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4336 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/Optimization.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17402 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/SystemSurrogates.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    21247 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/SystemSurrogatesAdvanced.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17257 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/Targets.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19106 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/TimeDriver.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    16763 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/TimeDriverAdvanced.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19331 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/TipsAndTricks.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10059 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/Visitors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10314 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/aa-SimpleCircuit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/exprampode_fmu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.305814 cosapp-0.13.1/docs/tutorials/images/
--rw-rw-rw-   0 root         (0) root         (0)    84424 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/Moise_tables_loi.jpg
--rw-rw-rw-   0 root         (0) root         (0)     3204 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/cosapp.svg
--rw-rw-rw-   0 root         (0) root         (0)    17745 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/design_circuit.svg
--rw-rw-rw-   0 root         (0) root         (0)    23419 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/drivers_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     6953 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/drivers_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     7366 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/drivers_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    40831 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/drivers_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     8450 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/drivers_5.svg
--rw-rw-rw-   0 root         (0) root         (0)     4537 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/drivers_nonlinear.svg
--rw-rw-rw-   0 root         (0) root         (0)     2309 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/experimental.svg
--rw-rw-rw-   0 root         (0) root         (0)    10190 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/in_progress.svg
--rw-rw-rw-   0 root         (0) root         (0)    26687 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/ports_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    19983 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/ports_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    30601 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/ports_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    16538 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/simple_circuit.svg
--rw-rw-rw-   0 root         (0) root         (0)     9156 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/systems_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    18904 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/systems_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    18945 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/systems_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    24136 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/systems_4.svg
--rw-rw-rw-   0 root         (0) root         (0)    28090 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/systems_5.svg
--rw-rw-rw-   0 root         (0) root         (0)     5070 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/tanks.svg
--rw-rw-rw-   0 root         (0) root         (0)    27536 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/triggers_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    24504 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/triggers_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6961 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/validity.svg
--rw-rw-rw-   0 root         (0) root         (0)    85431 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/images/visibility.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.306814 cosapp-0.13.1/docs/tutorials/multimode/
--rw-rw-rw-   0 root         (0) root         (0)     7019 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/multimode/BouncingBall.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4001 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/multimode/MultimodeOde.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5205 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/multimode/NewtonPendulum.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:55:58.307814 cosapp-0.13.1/docs/tutorials/optimization/
--rw-rw-rw-   0 root         (0) root         (0)     7559 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/optimization/BetzLimit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8420 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/optimization/Sellar.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4400 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/quickstart.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3233 2023-04-03 13:55:20.000000 cosapp-0.13.1/docs/tutorials/time_solutions.py
--rw-rw-rw-   0 root         (0) root         (0)     2013 2023-04-03 13:55:58.308814 cosapp-0.13.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-04-03 13:55:20.000000 cosapp-0.13.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.819207 cosapp-0.14.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-05-17 16:52:15.000000 cosapp-0.14.0/AUTHORS.md
+-rw-rw-rw-   0 root         (0) root         (0)     3488 2023-05-17 16:52:15.000000 cosapp-0.14.0/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)    40522 2023-05-17 16:52:15.000000 cosapp-0.14.0/HISTORY.md
+-rw-rw-rw-   0 root         (0) root         (0)     6572 2023-05-17 16:52:15.000000 cosapp-0.14.0/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-05-17 16:52:15.000000 cosapp-0.14.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    42984 2023-05-17 16:52:54.820207 cosapp-0.14.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-05-17 16:52:15.000000 cosapp-0.14.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.670197 cosapp-0.14.0/cosapp/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.672197 cosapp-0.14.0/cosapp/base/
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.675198 cosapp-0.14.0/cosapp/core/
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4354 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/configuration_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)    18754 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/eval_str.py
+-rw-rw-rw-   0 root         (0) root         (0)    15819 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.679198 cosapp-0.14.0/cosapp/core/numerics/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/numerics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27541 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/numerics/basics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28053 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/numerics/boundary.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/numerics/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2948 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/numerics/mathematicalproblem.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)    13455 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/numerics/residues.py
+-rw-rw-rw-   0 root         (0) root         (0)    19400 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/numerics/root.py
+-rw-rw-rw-   0 root         (0) root         (0)    15550 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/numerics/sobol_seq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.680198 cosapp-0.14.0/cosapp/core/signal/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/signal/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4972 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/signal/signal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1812 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/signal/slot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.682198 cosapp-0.14.0/cosapp/core/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15027 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/tests/test_AssignString.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/tests/test_ContextLocals.py
+-rw-rw-rw-   0 root         (0) root         (0)    12340 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/tests/test_EvalString.py
+-rw-rw-rw-   0 root         (0) root         (0)    13397 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/tests/test_Module.py
+-rw-rw-rw-   0 root         (0) root         (0)     6502 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/tests/test_coSAppConfiguration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/tests/test_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/core/variableref.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.689199 cosapp-0.14.0/cosapp/drivers/
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3030 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/abstractsetofcases.py
+-rw-rw-rw-   0 root         (0) root         (0)    12109 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/abstractsolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     8692 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/driver.py
+-rw-rw-rw-   0 root         (0) root         (0)     9484 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/influence.py
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/iterativecase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/lineardoe.py
+-rw-rw-rw-   0 root         (0) root         (0)     3131 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/metasystembuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    10683 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/montecarlo.py
+-rw-rw-rw-   0 root         (0) root         (0)    26684 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/nonlinearsolver.py
+-rw-rw-rw-   0 root         (0) root         (0)    22339 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/optimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/optionaldriver.py
+-rw-rw-rw-   0 root         (0) root         (0)     6655 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/runonce.py
+-rw-rw-rw-   0 root         (0) root         (0)    11432 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/runsinglecase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.691199 cosapp-0.14.0/cosapp/drivers/time/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/euler.py
+-rw-rw-rw-   0 root         (0) root         (0)    19963 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3457 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/runge_kutta.py
+-rw-rw-rw-   0 root         (0) root         (0)    13729 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/scenario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.699199 cosapp-0.14.0/cosapp/drivers/time/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6501 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_BouncingBall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_DiscreteStepper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_EulerExplicit.py
+-rw-rw-rw-   0 root         (0) root         (0)    18994 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_ExplicitTimeDriver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1501 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_InterpolAssignString.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_Interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5336 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_NewtonPendulum.py
+-rw-rw-rw-   0 root         (0) root         (0)    25908 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_RungeKutta.py
+-rw-rw-rw-   0 root         (0) root         (0)    22334 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_Scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_SystemInterpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1633 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_TimeAssignString.py
+-rw-rw-rw-   0 root         (0) root         (0)     4551 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_TimeStepManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     8108 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_TimeUnknownDict.py
+-rw-rw-rw-   0 root         (0) root         (0)     4478 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_TimeUnknownStack.py
+-rw-rw-rw-   0 root         (0) root         (0)     2914 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_TimeVarManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_TwoPointCubicInterpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)      771 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_TwoPointCubicPolynomial.py
+-rw-rw-rw-   0 root         (0) root         (0)     9926 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_event_cascades.py
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/tests/test_modevar_init.py
+-rw-rw-rw-   0 root         (0) root         (0)    21544 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/time/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    15033 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1657 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/drivers/validitycheck.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.700199 cosapp-0.14.0/cosapp/multimode/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/multimode/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5937 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/multimode/discreteStepper.py
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/multimode/event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/multimode/zeroCrossing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.702200 cosapp-0.14.0/cosapp/patterns/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/patterns/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3411 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/patterns/observer.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/patterns/singleton.py
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/patterns/visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.705200 cosapp-0.14.0/cosapp/ports/
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/ports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16228 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/ports/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/ports/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/ports/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4019 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/ports/mode_variable.py
+-rw-rw-rw-   0 root         (0) root         (0)    34280 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/ports/port.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/ports/unit_library.ini
+-rw-rw-rw-   0 root         (0) root         (0)    33349 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/ports/units.py
+-rw-rw-rw-   0 root         (0) root         (0)    31409 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/ports/variable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.707200 cosapp-0.14.0/cosapp/recorders/
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/recorders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4628 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/recorders/dataframe_recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)     7847 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/recorders/dsv_recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)    13366 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/recorders/recorder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.711200 cosapp-0.14.0/cosapp/systems/
+-rw-rw-rw-   0 root         (0) root         (0)      741 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/systems/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6623 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/systems/externalsystem.py
+-rw-rw-rw-   0 root         (0) root         (0)    13327 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/systems/metamodels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/systems/processsystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     5246 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/systems/structure.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)   132189 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/systems/system.py
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/systems/system.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/systems/systemConnector.py
+-rw-rw-rw-   0 root         (0) root         (0)    15645 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/systems/systemSurrogate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5515 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/systems/systemfamily.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.712200 cosapp-0.14.0/cosapp/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.713200 cosapp-0.14.0/cosapp/tools/fmu/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/fmu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22009 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/fmu/exporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/fmu/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.714200 cosapp-0.14.0/cosapp/tools/fmu/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/fmu/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13896 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/fmu/tests/test_exporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/fmu/tests/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     4104 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/help.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.715200 cosapp-0.14.0/cosapp/tools/module_parser/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/module_parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4279 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/module_parser/package_metadata.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)    14861 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/module_parser/parseModule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.716200 cosapp-0.14.0/cosapp/tools/problem_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7945 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/problem_viewer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.717201 cosapp-0.14.0/cosapp/tools/problem_viewer/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   250263 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/tests/test_viewmodeldata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.718201 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/
+-rw-rw-rw-   0 root         (0) root         (0)     9254 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.720201 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/libs/
+-rw-rw-rw-   0 root         (0) root         (0)     9483 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/libs/awesomplete.js
+-rw-rw-rw-   0 root         (0) root         (0)   211120 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/libs/d3.v4.min.js
+-rw-rw-rw-   0 root         (0) root         (0)      925 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/libs/http.js
+-rw-rw-rw-   0 root         (0) root         (0)    86659 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/libs/jquery-3.2.1.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     4679 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/libs/vkBeautify.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.723201 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/constants.js
+-rw-rw-rw-   0 root         (0) root         (0)    16285 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/draw.js
+-rw-rw-rw-   0 root         (0) root         (0)     5771 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/legend.js
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/modal.js
+-rw-rw-rw-   0 root         (0) root         (0)    70307 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/ptN2.js
+-rw-rw-rw-   0 root         (0) root         (0)     9486 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/search.js
+-rw-rw-rw-   0 root         (0) root         (0)     4155 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/svg.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.724201 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/style/
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/style/awesomplete.css
+-rw-rw-rw-   0 root         (0) root         (0)     5612 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/style/fontello.woff
+-rw-rw-rw-   0 root         (0) root         (0)     5815 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/style/partition_tree.css
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/problem_viewer/webview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.726201 cosapp-0.14.0/cosapp/tools/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.727201 cosapp-0.14.0/cosapp/tools/templates/lib/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/templates/lib/Readme.txt
+-rw-rw-rw-   0 root         (0) root         (0)   236746 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/templates/lib/d3.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    23777 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/templates/lib/vis.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   663624 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/templates/lib/vis.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/templates/pythonfmu.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.729201 cosapp-0.14.0/cosapp/tools/templates/src/
+-rw-rw-rw-   0 root         (0) root         (0)     4751 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/templates/src/d3_draw.js
+-rw-rw-rw-   0 root         (0) root         (0)      451 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/templates/src/d3_styles.css
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/templates/system_d3.html
+-rw-rw-rw-   0 root         (0) root         (0)     8155 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/templates/system_repr.html
+-rw-rw-rw-   0 root         (0) root         (0)     6675 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.731202 cosapp-0.14.0/cosapp/tools/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/views/baseRenderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6755 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/views/d3js.py
+-rw-rw-rw-   0 root         (0) root         (0)     4760 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/views/markdown.py
+-rw-rw-rw-   0 root         (0) root         (0)    20440 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/views/prettyprint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.733202 cosapp-0.14.0/cosapp/tools/views/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/views/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/views/tests/test_VisJsRenderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/views/tests/test_d3.py
+-rw-rw-rw-   0 root         (0) root         (0)     7823 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/views/tests/test_markdown.py
+-rw-rw-rw-   0 root         (0) root         (0)     5912 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/views/tests/test_prettyprint.py
+-rw-rw-rw-   0 root         (0) root         (0)    16980 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tools/views/visjs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.744202 cosapp-0.14.0/cosapp/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/00-Introduction.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19776 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/01-Systems.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    14740 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/02-Ports.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    18911 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/03-Drivers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2711 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/04-Triggers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    17810 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/05-Validation.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10286 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/06-Visibility.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8547 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/07-Metamodels.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19784 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/08-Multipoints-Design.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    14617 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/09-MonteCarlo.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5749 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/10-Recorders.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10084 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/11-DesignMethods.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    11006 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/CustomConnectors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/FMI.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    28157 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/Guidelines.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    14967 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/HybridSimulations.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    13505 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/Logging.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4336 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/Optimization.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    17402 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/SystemSurrogates.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    21247 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/SystemSurrogatesAdvanced.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    17257 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/Targets.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19106 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/TimeDriver.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    16763 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/TimeDriverAdvanced.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19331 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/TipsAndTricks.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10059 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/Visitors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10314 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/aa-SimpleCircuit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/exprampode_fmu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.754203 cosapp-0.14.0/cosapp/tutorials/images/
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/cosapp.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17745 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/design_circuit.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23419 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/drivers_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6953 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/drivers_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7366 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/drivers_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    40831 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/drivers_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8450 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/drivers_5.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4537 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/drivers_nonlinear.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/experimental.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10190 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/in_progress.svg
+-rw-rw-rw-   0 root         (0) root         (0)    26687 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/ports_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19983 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/ports_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    30601 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/ports_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16538 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/simple_circuit.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9156 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/systems_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18904 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/systems_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18945 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/systems_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24136 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/systems_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)    28090 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/systems_5.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/tanks.svg
+-rw-rw-rw-   0 root         (0) root         (0)    27536 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/triggers_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24504 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/triggers_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6961 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/validity.svg
+-rw-rw-rw-   0 root         (0) root         (0)    85431 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/images/visibility.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.755203 cosapp-0.14.0/cosapp/tutorials/multimode/
+-rw-rw-rw-   0 root         (0) root         (0)     7019 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/multimode/BouncingBall.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/multimode/MultimodeOde.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5205 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/multimode/NewtonPendulum.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.756203 cosapp-0.14.0/cosapp/tutorials/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)     7559 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/optimization/BetzLimit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8420 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/optimization/Sellar.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4400 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/quickstart.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/tutorials/time_solutions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.761203 cosapp-0.14.0/cosapp/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.763204 cosapp-0.14.0/cosapp/utils/distributions/
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/distributions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/distributions/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     2693 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/distributions/normal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.765204 cosapp-0.14.0/cosapp/utils/distributions/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/distributions/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1809 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/distributions/tests/test_distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/distributions/tests/test_normal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2912 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/distributions/tests/test_triangular.py
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/distributions/tests/test_uniform.py
+-rw-rw-rw-   0 root         (0) root         (0)     4207 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/distributions/triangular.py
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/distributions/uniform.py
+-rw-rw-rw-   0 root         (0) root         (0)     6715 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/find_variables.py
+-rw-rw-rw-   0 root         (0) root         (0)     3677 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/graph_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4604 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/json.py
+-rw-rw-rw-   0 root         (0) root         (0)    16769 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     3694 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/naming.py
+-rw-rw-rw-   0 root         (0) root         (0)    14038 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/options_dictionary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5169 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3856 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/pull_variables.py
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/state_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.767204 cosapp-0.14.0/cosapp/utils/surrogate_models/
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     9528 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/kriging.py
+-rw-rw-rw-   0 root         (0) root         (0)    39321 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/multifi_cokriging.py
+-rw-rw-rw-   0 root         (0) root         (0)     5292 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/nearest_neighbor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.769204 cosapp-0.14.0/cosapp/utils/surrogate_models/nn_interpolators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/nn_interpolators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5286 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/nn_interpolators/linear_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3158 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/nn_interpolators/nn_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    18553 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/nn_interpolators/rbf_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5287 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/nn_interpolators/weighted_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/response_surface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.771204 cosapp-0.14.0/cosapp/utils/surrogate_models/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4611 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/tests/test_kriging.py
+-rw-rw-rw-   0 root         (0) root         (0)     6925 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/tests/test_multifi_cokriging.py
+-rw-rw-rw-   0 root         (0) root         (0)    16170 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/tests/test_nearest_neighbor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/surrogate_models/tests/test_response_surface.py
+-rw-rw-rw-   0 root         (0) root         (0)     8056 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/testing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1334 2023-05-17 16:52:15.000000 cosapp-0.14.0/cosapp/utils/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.672197 cosapp-0.14.0/cosapp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    42984 2023-05-17 16:52:54.000000 cosapp-0.14.0/cosapp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14182 2023-05-17 16:52:54.000000 cosapp-0.14.0/cosapp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 16:52:54.000000 cosapp-0.14.0/cosapp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 16:52:54.000000 cosapp-0.14.0/cosapp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-17 16:52:54.000000 cosapp-0.14.0/cosapp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-17 16:52:54.000000 cosapp-0.14.0/cosapp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.775205 cosapp-0.14.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     6810 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11424 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/contributing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.776204 cosapp-0.14.0/docs/cosapp_theme/
+-rw-rw-rw-   0 root         (0) root         (0)     2422 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/layout.html
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/searchbox.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.777205 cosapp-0.14.0/docs/cosapp_theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)     8997 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/cosapp.css_t
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.780205 cosapp-0.14.0/docs/cosapp_theme/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/css/custom.css
+-rw-rw-rw-   0 root         (0) root         (0)    31000 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/css/font-awesome.min.css
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/css/font.css
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/css/highlight.css
+-rw-rw-rw-   0 root         (0) root         (0)    40062 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/css/kube.css
+-rw-rw-rw-   0 root         (0) root         (0)     8764 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/css/kube.demo.css
+-rw-rw-rw-   0 root         (0) root         (0)     9250 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/css/kube.legenda.css
+-rw-rw-rw-   0 root         (0) root         (0)    30268 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/css/kube.min.css
+-rw-rw-rw-   0 root         (0) root         (0)    26211 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/css/master.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.784205 cosapp-0.14.0/docs/cosapp_theme/static/font/
+-rw-rw-rw-   0 root         (0) root         (0)   297272 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/font/Lato-Black.woff
+-rw-rw-rw-   0 root         (0) root         (0)   328952 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/font/Lato-Bold.woff
+-rw-rw-rw-   0 root         (0) root         (0)   347092 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/font/Lato-BoldItalic.woff
+-rw-rw-rw-   0 root         (0) root         (0)   343528 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/font/Lato-Italic.woff
+-rw-rw-rw-   0 root         (0) root         (0)   323172 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/font/Lato-Regular.woff
+-rw-rw-rw-   0 root         (0) root         (0)   326132 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/font/Lato-Semibold.woff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.785205 cosapp-0.14.0/docs/cosapp_theme/static/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    98024 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/fonts/fontawesome-webfont.woff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.786205 cosapp-0.14.0/docs/cosapp_theme/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/img/cosapp.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.788205 cosapp-0.14.0/docs/cosapp_theme/static/js/
+-rw-rw-rw-   0 root         (0) root         (0)    84380 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/js/jquery-2.1.4.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    56646 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/js/kube.js
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/js/kube.legenda.js
+-rw-rw-rw-   0 root         (0) root         (0)    31683 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/js/kube.min.js
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/js/master.js
+-rw-rw-rw-   0 root         (0) root         (0)    12047 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/js/tocbot.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     5219 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/static/sidebar.js_t
+-rw-rw-rw-   0 root         (0) root         (0)      736 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/cosapp_theme/theme.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.790205 cosapp-0.14.0/docs/developer/
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/developer/installation_cases.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8633 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/developer/logger.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/developer/project_structure.rst
+-rw-rw-rw-   0 root         (0) root         (0)    12553 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/developer/scenarii.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/history.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.790205 cosapp-0.14.0/docs/img/
+-rw-rw-rw-   0 root         (0) root         (0)     2475 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/img/gitlab-cosapp-f4950f.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4393 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/img/website-docs-blue.svg
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/license.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6499 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.664197 cosapp-0.14.0/docs/nb_thumbnails/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.795206 cosapp-0.14.0/docs/nb_thumbnails/_images/
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/nb_thumbnails/_images/desktop-download.svg
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/nb_thumbnails/_images/eye.svg
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/nb_thumbnails/_images/file-code.svg
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/nb_thumbnails/_images/file-text.svg
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/nb_thumbnails/_images/fold.svg
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/nb_thumbnails/_images/package.svg
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/nb_thumbnails/_images/pencil.svg
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/nb_thumbnails/_images/play.svg
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/nb_thumbnails/_images/plug.svg
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/nb_thumbnails/_images/pulse.svg
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/nb_thumbnails/_images/verified.svg
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/nb_thumbnails/_images/zap.svg
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.795206 cosapp-0.14.0/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)     3736 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/source/modules.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.796206 cosapp-0.14.0/docs/tools/
+-rw-rw-rw-   0 root         (0) root         (0)    12905 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tools/mermaid.py
+-rw-rw-rw-   0 root         (0) root         (0)    10299 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tools/mermaid_inheritance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.807206 cosapp-0.14.0/docs/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/00-Introduction.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19776 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/01-Systems.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    14740 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/02-Ports.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    18911 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/03-Drivers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2711 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/04-Triggers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    17810 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/05-Validation.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10286 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/06-Visibility.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8547 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/07-Metamodels.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19784 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/08-Multipoints-Design.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    14617 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/09-MonteCarlo.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5749 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/10-Recorders.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10084 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/11-DesignMethods.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    11006 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/CustomConnectors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/FMI.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    28157 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/Guidelines.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    14967 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/HybridSimulations.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    13505 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/Logging.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4336 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/Optimization.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    17402 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/SystemSurrogates.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    21247 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/SystemSurrogatesAdvanced.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    17257 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/Targets.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19106 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/TimeDriver.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    16763 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/TimeDriverAdvanced.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19331 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/TipsAndTricks.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10059 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/Visitors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10314 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/aa-SimpleCircuit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/exprampode_fmu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.817207 cosapp-0.14.0/docs/tutorials/images/
+-rw-rw-rw-   0 root         (0) root         (0)    84424 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/Moise_tables_loi.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/cosapp.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17745 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/design_circuit.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23419 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/drivers_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6953 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/drivers_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7366 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/drivers_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    40831 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/drivers_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8450 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/drivers_5.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4537 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/drivers_nonlinear.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/experimental.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10190 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/in_progress.svg
+-rw-rw-rw-   0 root         (0) root         (0)    26687 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/ports_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19983 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/ports_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    30601 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/ports_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16538 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/simple_circuit.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9156 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/systems_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18904 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/systems_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18945 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/systems_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24136 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/systems_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)    28090 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/systems_5.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/tanks.svg
+-rw-rw-rw-   0 root         (0) root         (0)    27536 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/triggers_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24504 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/triggers_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6961 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/validity.svg
+-rw-rw-rw-   0 root         (0) root         (0)    85431 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/images/visibility.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.819207 cosapp-0.14.0/docs/tutorials/multimode/
+-rw-rw-rw-   0 root         (0) root         (0)     7019 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/multimode/BouncingBall.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/multimode/MultimodeOde.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5205 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/multimode/NewtonPendulum.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 16:52:54.819207 cosapp-0.14.0/docs/tutorials/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)     7559 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/optimization/BetzLimit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8420 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/optimization/Sellar.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4400 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/quickstart.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2023-05-17 16:52:15.000000 cosapp-0.14.0/docs/tutorials/time_solutions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-05-17 16:52:54.821208 cosapp-0.14.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-17 16:52:15.000000 cosapp-0.14.0/setup.py
```

### Comparing `cosapp-0.13.1/AUTHORS.md` & `cosapp-0.14.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/CONTRIBUTING.md` & `cosapp-0.14.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/HISTORY.md` & `cosapp-0.14.0/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,71 @@
 # History
 
+## 0.14.0 (2023-05-17)
+
+### New features & API changes
+
+* Improved performance, through a revised clean/dirty mechanism (MR [#215](https://gitlab.com/cosapp/cosapp/-/merge_requests/215)).
+* Possibility to add a contextual description to sub-systems and ports of a system, as well as sub-drivers (MR [#216](https://gitlab.com/cosapp/cosapp/-/merge_requests/216)). This feature is useful for automatic documentation tools, and has been included in the Markdown representation of systems (also used in function `cosapp.tools.display_doc`). Example:
+  
+  ```python
+  from cosapp.base import System
+  from my_module import FlowPort
+  
+  class MySystem(System):
+      def setup(self):
+          self.add_input(FlowPort, "fl_in1", desc="Primary inlet flow port")
+          self.add_input(FlowPort, "fl_in2", desc="Secondary inlet flow port")
+  
+          self.add_output(FlowPort, "fl_out")
+  ```
+  
+* New hook function `_parse_module_config`, returning pre-defined settings for `cosapp.tools.parse_module` (MR [#218](https://gitlab.com/cosapp/cosapp/-/merge_requests/218)). This allows module maintainers to simply call
+  
+  ```python
+  from cosapp.tools import parse_module
+  import my_module
+  
+  parse_module(my_module)
+  ```
+
+  instead of, *e.g.*,
+
+  ```python
+  parse_module(
+      my_module,
+      ctor_config={
+          "ComplexSystem1": [
+              dict(n=1, foo=0.5),
+              dict(n=2, foo=0.1),
+          ],
+          "ComplexSystem2": [
+              dict(xi=0.0, __alias__="ComplexSystem2_a"),
+              dict(xi=1.0, __alias__="ComplexSystem2_b"),
+          ],
+      },
+      excludes=["Foo*", "*Bar?"],
+  )
+  ```
+
+  provided `my_module._parse_module_config()` returns a dictionary specifying the values of `ctor_config`, `excludes`, *etc.*
+
+- Make `SolverResults` a `dataclass`, for easier handling of `NonLinearSolver.results`, *e.g.* (MR [#220](https://gitlab.com/cosapp/cosapp/-/merge_requests/220)).
+- Expose attribute `problem` in system setup (MR [#221](https://gitlab.com/cosapp/cosapp/-/merge_requests/221)). Previously, `problem` was only exposed in method `System.transition`.
+
+### Bug fixes and code quality
+
+* Fix bug in `NonLinearSolver` log message (MR [#214](https://gitlab.com/cosapp/cosapp/-/merge_requests/214)).
+* Add missing JSON file in PyPI and conda packages, preventing the use of `cosapp.tools.parse_module` (MR [#219](https://gitlab.com/cosapp/cosapp/-/merge_requests/219)).
+
+### Documentation
+
+* Illustrate port and sub-system description in tutorials (MR [#215](https://gitlab.com/cosapp/cosapp/-/merge_requests/215)).
+
+
 ## 0.13.1 (2023-04-03)
 
 ### Bug fixes and code quality
 
 * Update test baseline to pass in a Python 3.11 environment (MR [#200](https://gitlab.com/cosapp/cosapp/-/merge_requests/200)).
 * Creation of a dummy system factory, mostly for tests (MR [#201](https://gitlab.com/cosapp/cosapp/-/merge_requests/201)).
 * Improve clean/dirty mechanism (MR [#202](https://gitlab.com/cosapp/cosapp/-/merge_requests/202)) and fix incorrect clean/dirty status with surrogate models (MR [#205](https://gitlab.com/cosapp/cosapp/-/merge_requests/205)).
@@ -33,61 +95,61 @@
 
 * Module `connectors` moved from `cosapp.core` to `cosapp.ports` (MR [#189](https://gitlab.com/cosapp/cosapp/-/merge_requests/189)).
 * New "direct" (with no unit conversion) connector classes `PlainConnector`, `CopyConnector` and `DeepCopyConnector`, in `cosapp.ports.connectors` (MR [#188](https://gitlab.com/cosapp/cosapp/-/merge_requests/188)).
 * New method `MathematicalProblem.is_empty()`, equivalent to `shape == (0, 0)` (MR [#186](https://gitlab.com/cosapp/cosapp/-/merge_requests/186)).
 * Improved VisJs graph rendering, by limiting node size for long system names (MR [#184](https://gitlab.com/cosapp/cosapp/-/merge_requests/184)).
 * New utility functions `get_state` and `set_state` in `cosapp.utils`, for quick system data recovery (MR [#193](https://gitlab.com/cosapp/cosapp/-/merge_requests/193)):
 
-```python
-from cosapp.utils import get_state, set_state
-
-s = SomeSystem('s')
-# ... many design steps, say
-
-# Save state in local object
-designed = get_state(s)
-
-s.drivers.clear()
-s.add_driver(SomeDriver('driver'))
-
-try:
-    s.run_drivers()
-except:
-    # Recover previous state
-    set_state(s, designed)
-```
+  ```python
+  from cosapp.utils import get_state, set_state
+  
+  s = SomeSystem('s')
+  # ... many design steps, say
+  
+  # Save state in local object
+  designed = get_state(s)
+  
+  s.drivers.clear()
+  s.add_driver(SomeDriver('driver'))
+  
+  try:
+      s.run_drivers()
+  except:
+      # Recover previous state
+      set_state(s, designed)
+  ```
 
 * Functions `radians`, `degrees` and `arctan2`/`atan2` have been added to the scope of `EvalString` objects, and can therefore be used in equations, *e.g.* (MR [#178](https://gitlab.com/cosapp/cosapp/-/merge_requests/178)).
 * Recorders can now record constant properties (MR [#181](https://gitlab.com/cosapp/cosapp/-/merge_requests/181)).
 * Deprecation of `System.get_unsolved_problem` in favour of new method `assembled_problem` (MR [#174](https://gitlab.com/cosapp/cosapp/-/merge_requests/174)).
 * Inner off-design problem of systems is now exposed as attribute `problem`, but only within the `transition` method (MR [#174](https://gitlab.com/cosapp/cosapp/-/merge_requests/174)). This allows users to add or remove off-design constraints during event-driven transitions, while keeping this property inaccessible the rest of the time.
 
-```python
-from cosapp.base import System
-from math import sin, cos
-
-class SomeSystem(System):
-    def setup(self):
-        self.add_inward('x', 0.0)
-        self.add_inward('y', 0.0)
-        self.add_outward('z', 0.0)
-        a = self.add_event('event_a', trigger='x > y')
-        b = self.add_event('event_b', trigger='x < y')
-    
-    def compute(self):
-        self.z = cos(self.x) * sin(self.y)
-
-    def transition(self):
-        offdesign = self.problem
-        if self.event_a.present:
-            offdesign.clear()
-            offdesign.add_equation('z == 0.5').add_unknown('x')
-        if self.event_b.present:
-            offdesign.clear()
-```
+  ```python
+  from cosapp.base import System
+  from math import sin, cos
+  
+  class SomeSystem(System):
+      def setup(self):
+          self.add_inward('x', 0.0)
+          self.add_inward('y', 0.0)
+          self.add_outward('z', 0.0)
+          a = self.add_event('event_a', trigger='x > y')
+          b = self.add_event('event_b', trigger='x < y')
+      
+      def compute(self):
+          self.z = cos(self.x) * sin(self.y)
+  
+      def transition(self):
+          offdesign = self.problem
+          if self.event_a.present:
+              offdesign.clear()
+              offdesign.add_equation('z == 0.5').add_unknown('x')
+          if self.event_b.present:
+              offdesign.clear()
+  ```
 
 ### Bug fixes and code quality
 
 * Fix serialization bugs for systems with setup parameters (MR [#180](https://gitlab.com/cosapp/cosapp/-/merge_requests/180)) and `None` variables (MR [#172](https://gitlab.com/cosapp/cosapp/-/merge_requests/172)).
 * Bug fix on event time calculation involving array transients (MR [#177](https://gitlab.com/cosapp/cosapp/-/merge_requests/177)).
 * Bug fix on possible name conflicts in connector storage (MR [#173](https://gitlab.com/cosapp/cosapp/-/merge_requests/173)).
 * Fix inconsistent behaviour of `System.add_child` when a `pulling` error is raised (MR [#197](https://gitlab.com/cosapp/cosapp/-/merge_requests/197)).
@@ -144,79 +206,79 @@
 
 ### New features & API changes
 
 * Simplification of driver `Optimizer`:
   * Suppression of sub-driver `runner` (MR [#136](https://gitlab.com/cosapp/cosapp/-/merge_requests/136)). This change introduces new methods `set_objective`, `add_unknowns` and `add_constraints` in driver `Optimizer`.
   * Optimization constraints are now declared with human-readable expressions in `Optimizer.add_constraints` (MR [#138](https://gitlab.com/cosapp/cosapp/-/merge_requests/138)).
 
-Before:
+  Before:
+    
+  ```python
+  from cosapp.drivers import Optimizer
   
-```python
-from cosapp.drivers import Optimizer
-
-s = SomeSystem('s')
-optim = s.add_driver(Optimizer('optim'))
-
-optim.runner.set_objective('cost')
-optim.runner.add_unknown(['a', 'b', 'p_in.x'])
-# Enter constraints as non-negative expressions:
-optim.runner.add_constraints([
-    "b - a",  # b >= a
-    "a",      # a >= 0
-    "1 - a",  # a <= 1
-])
-optim.runner.add_constraints(
-    "p_out.y",
-    inequality = False,  # p_out.y == 0
-)
-
-s.run_drivers()
-```
-
-After:
-  
-```python
-optim.set_objective('cost')
-optim.add_unknown(['a', 'b', 'p_in.x'])
-optim.add_constraints(
-    "b >= a",
-    "0 <= a <= 1",
-    "p_out.y == 0",
-)
-```
+  s = SomeSystem('s')
+  optim = s.add_driver(Optimizer('optim'))
+  
+  optim.runner.set_objective('cost')
+  optim.runner.add_unknown(['a', 'b', 'p_in.x'])
+  # Enter constraints as non-negative expressions:
+  optim.runner.add_constraints([
+      "b - a",  # b >= a
+      "a",      # a >= 0
+      "1 - a",  # a <= 1
+  ])
+  optim.runner.add_constraints(
+      "p_out.y",
+      inequality = False,  # p_out.y == 0
+  )
+  
+  s.run_drivers()
+  ```
+  
+  After:
+    
+  ```python
+  optim.set_objective('cost')
+  optim.add_unknown(['a', 'b', 'p_in.x'])
+  optim.add_constraints(
+      "b >= a",
+      "0 <= a <= 1",
+      "p_out.y == 0",
+  )
+  ```
 
   * New, convenient iterators and setters for ports (MR [#137](https://gitlab.com/cosapp/cosapp/-/merge_requests/137)):
   
-```python
-from cosapp.base import Port, System
-
-class XyzPort(Port):
-    def setup(self):
-        self.add_variable('x')
-        self.add_variable('y')
-        self.add_variable('z')
-
-class SomeSystem(System):
-    def setup(self):
-        self.add_input(XyzPort, 'p_in')
-        self.add_output(XyzPort, 'p_out')
-    
-    def compute(self):
-        self.p_out.set_from(self.p_in)  # assign values from `p_in`
-        self.p_out.z = 0.0
-
-s = SomeSystem('s')
-# Multi-variable setter `set_values`
-s.p_in.set_values(x=1, y=-0.5, z=0.1)
-
-s.run_once()
-# Dict-like (key, value) iterator `items`:
-for varname, value in s.p_out.items():
-    print(f"p_out.{varname} = {value})
-```
+  ```python
+  from cosapp.base import Port, System
+  
+  class XyzPort(Port):
+      def setup(self):
+          self.add_variable('x')
+          self.add_variable('y')
+          self.add_variable('z')
+  
+  class SomeSystem(System):
+      def setup(self):
+          self.add_input(XyzPort, 'p_in')
+          self.add_output(XyzPort, 'p_out')
+      
+      def compute(self):
+          self.p_out.set_from(self.p_in)  # assign values from `p_in`
+          self.p_out.z = 0.0
+  
+  s = SomeSystem('s')
+  # Multi-variable setter `set_values`
+  s.p_in.set_values(x=1, y=-0.5, z=0.1)
+  
+  s.run_once()
+  # Dict-like (key, value) iterator `items`:
+  for varname, value in s.p_out.items():
+      print(f"p_out.{varname} = {value})
+  ```
 
 ### Documentation
 
 * Updated tutorials on ports (MR [#139](https://gitlab.com/cosapp/cosapp/-/merge_requests/139)) and on optimization (MR [#140](https://gitlab.com/cosapp/cosapp/-/merge_requests/140)).
 
 ### Bug fixes and code quality
```

### Comparing `cosapp-0.13.1/LICENSE.rst` & `cosapp-0.14.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/MANIFEST.in` & `cosapp-0.14.0/MANIFEST.in`

 * *Files 16% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 include CONTRIBUTING.md
 include HISTORY.md
 include LICENSE.rst
 include README.md
 
 include cosapp/core/configuration_schema.json
 include cosapp/ports/unit_library.ini
-include cosapp/systems/system.schema.json
+recursive-include cosapp *.schema.json
 recursive-include cosapp/tools/templates *
 recursive-include cosapp/tools/problem_viewer/visualization *
-
 recursive-include cosapp/tutorials *.ipynb *.svg *.py
 
-recursive-include cosapp/tests *
-recursive-exclude cosapp/tests *.html
+recursive-exclude * conftest.py
+recursive-exclude */tests __init__.py test_*.py
 recursive-exclude * __pycache__
 recursive-exclude * *.py[co]
+prune */tests
 
 recursive-include docs *.rst conf.py Makefile make.bat *.jpg *.png *.gif *.svg *.ipynb *.py
 recursive-exclude docs source/_autosummary/*
 prune docs/_build
 
 recursive-include docs/cosapp_theme *
```

### Comparing `cosapp-0.13.1/PKG-INFO` & `cosapp-0.14.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosapp
-Version: 0.13.1
+Version: 0.14.0
 Summary: CoSApp, the Collaborative System Approach.
 Home-page: https://cosapp.readthedocs.io
 Author: CoSApp Development Team
 License: Apache-2.0
 Keywords: cosapp,system simulation,system design
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: extra
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.rst
 
 # CoSApp - Collaborative System Approach
@@ -55,14 +55,76 @@
 # Try it now!
 Run a Jupyter Lab instance with binder to try out CoSApp features through examples.
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/cosapp%2Fcosapp/master?urlpath=lab/tree/docs/tutorials)
 
 # History
 
+## 0.14.0 (2023-05-17)
+
+### New features & API changes
+
+* Improved performance, through a revised clean/dirty mechanism (MR [#215](https://gitlab.com/cosapp/cosapp/-/merge_requests/215)).
+* Possibility to add a contextual description to sub-systems and ports of a system, as well as sub-drivers (MR [#216](https://gitlab.com/cosapp/cosapp/-/merge_requests/216)). This feature is useful for automatic documentation tools, and has been included in the Markdown representation of systems (also used in function `cosapp.tools.display_doc`). Example:
+  
+  ```python
+  from cosapp.base import System
+  from my_module import FlowPort
+  
+  class MySystem(System):
+      def setup(self):
+          self.add_input(FlowPort, "fl_in1", desc="Primary inlet flow port")
+          self.add_input(FlowPort, "fl_in2", desc="Secondary inlet flow port")
+  
+          self.add_output(FlowPort, "fl_out")
+  ```
+  
+* New hook function `_parse_module_config`, returning pre-defined settings for `cosapp.tools.parse_module` (MR [#218](https://gitlab.com/cosapp/cosapp/-/merge_requests/218)). This allows module maintainers to simply call
+  
+  ```python
+  from cosapp.tools import parse_module
+  import my_module
+  
+  parse_module(my_module)
+  ```
+
+  instead of, *e.g.*,
+
+  ```python
+  parse_module(
+      my_module,
+      ctor_config={
+          "ComplexSystem1": [
+              dict(n=1, foo=0.5),
+              dict(n=2, foo=0.1),
+          ],
+          "ComplexSystem2": [
+              dict(xi=0.0, __alias__="ComplexSystem2_a"),
+              dict(xi=1.0, __alias__="ComplexSystem2_b"),
+          ],
+      },
+      excludes=["Foo*", "*Bar?"],
+  )
+  ```
+
+  provided `my_module._parse_module_config()` returns a dictionary specifying the values of `ctor_config`, `excludes`, *etc.*
+
+- Make `SolverResults` a `dataclass`, for easier handling of `NonLinearSolver.results`, *e.g.* (MR [#220](https://gitlab.com/cosapp/cosapp/-/merge_requests/220)).
+- Expose attribute `problem` in system setup (MR [#221](https://gitlab.com/cosapp/cosapp/-/merge_requests/221)). Previously, `problem` was only exposed in method `System.transition`.
+
+### Bug fixes and code quality
+
+* Fix bug in `NonLinearSolver` log message (MR [#214](https://gitlab.com/cosapp/cosapp/-/merge_requests/214)).
+* Add missing JSON file in PyPI and conda packages, preventing the use of `cosapp.tools.parse_module` (MR [#219](https://gitlab.com/cosapp/cosapp/-/merge_requests/219)).
+
+### Documentation
+
+* Illustrate port and sub-system description in tutorials (MR [#215](https://gitlab.com/cosapp/cosapp/-/merge_requests/215)).
+
+
 ## 0.13.1 (2023-04-03)
 
 ### Bug fixes and code quality
 
 * Update test baseline to pass in a Python 3.11 environment (MR [#200](https://gitlab.com/cosapp/cosapp/-/merge_requests/200)).
 * Creation of a dummy system factory, mostly for tests (MR [#201](https://gitlab.com/cosapp/cosapp/-/merge_requests/201)).
 * Improve clean/dirty mechanism (MR [#202](https://gitlab.com/cosapp/cosapp/-/merge_requests/202)) and fix incorrect clean/dirty status with surrogate models (MR [#205](https://gitlab.com/cosapp/cosapp/-/merge_requests/205)).
@@ -92,61 +154,61 @@
 
 * Module `connectors` moved from `cosapp.core` to `cosapp.ports` (MR [#189](https://gitlab.com/cosapp/cosapp/-/merge_requests/189)).
 * New "direct" (with no unit conversion) connector classes `PlainConnector`, `CopyConnector` and `DeepCopyConnector`, in `cosapp.ports.connectors` (MR [#188](https://gitlab.com/cosapp/cosapp/-/merge_requests/188)).
 * New method `MathematicalProblem.is_empty()`, equivalent to `shape == (0, 0)` (MR [#186](https://gitlab.com/cosapp/cosapp/-/merge_requests/186)).
 * Improved VisJs graph rendering, by limiting node size for long system names (MR [#184](https://gitlab.com/cosapp/cosapp/-/merge_requests/184)).
 * New utility functions `get_state` and `set_state` in `cosapp.utils`, for quick system data recovery (MR [#193](https://gitlab.com/cosapp/cosapp/-/merge_requests/193)):
 
-```python
-from cosapp.utils import get_state, set_state
-
-s = SomeSystem('s')
-# ... many design steps, say
-
-# Save state in local object
-designed = get_state(s)
-
-s.drivers.clear()
-s.add_driver(SomeDriver('driver'))
-
-try:
-    s.run_drivers()
-except:
-    # Recover previous state
-    set_state(s, designed)
-```
+  ```python
+  from cosapp.utils import get_state, set_state
+  
+  s = SomeSystem('s')
+  # ... many design steps, say
+  
+  # Save state in local object
+  designed = get_state(s)
+  
+  s.drivers.clear()
+  s.add_driver(SomeDriver('driver'))
+  
+  try:
+      s.run_drivers()
+  except:
+      # Recover previous state
+      set_state(s, designed)
+  ```
 
 * Functions `radians`, `degrees` and `arctan2`/`atan2` have been added to the scope of `EvalString` objects, and can therefore be used in equations, *e.g.* (MR [#178](https://gitlab.com/cosapp/cosapp/-/merge_requests/178)).
 * Recorders can now record constant properties (MR [#181](https://gitlab.com/cosapp/cosapp/-/merge_requests/181)).
 * Deprecation of `System.get_unsolved_problem` in favour of new method `assembled_problem` (MR [#174](https://gitlab.com/cosapp/cosapp/-/merge_requests/174)).
 * Inner off-design problem of systems is now exposed as attribute `problem`, but only within the `transition` method (MR [#174](https://gitlab.com/cosapp/cosapp/-/merge_requests/174)). This allows users to add or remove off-design constraints during event-driven transitions, while keeping this property inaccessible the rest of the time.
 
-```python
-from cosapp.base import System
-from math import sin, cos
-
-class SomeSystem(System):
-    def setup(self):
-        self.add_inward('x', 0.0)
-        self.add_inward('y', 0.0)
-        self.add_outward('z', 0.0)
-        a = self.add_event('event_a', trigger='x > y')
-        b = self.add_event('event_b', trigger='x < y')
-    
-    def compute(self):
-        self.z = cos(self.x) * sin(self.y)
-
-    def transition(self):
-        offdesign = self.problem
-        if self.event_a.present:
-            offdesign.clear()
-            offdesign.add_equation('z == 0.5').add_unknown('x')
-        if self.event_b.present:
-            offdesign.clear()
-```
+  ```python
+  from cosapp.base import System
+  from math import sin, cos
+  
+  class SomeSystem(System):
+      def setup(self):
+          self.add_inward('x', 0.0)
+          self.add_inward('y', 0.0)
+          self.add_outward('z', 0.0)
+          a = self.add_event('event_a', trigger='x > y')
+          b = self.add_event('event_b', trigger='x < y')
+      
+      def compute(self):
+          self.z = cos(self.x) * sin(self.y)
+  
+      def transition(self):
+          offdesign = self.problem
+          if self.event_a.present:
+              offdesign.clear()
+              offdesign.add_equation('z == 0.5').add_unknown('x')
+          if self.event_b.present:
+              offdesign.clear()
+  ```
 
 ### Bug fixes and code quality
 
 * Fix serialization bugs for systems with setup parameters (MR [#180](https://gitlab.com/cosapp/cosapp/-/merge_requests/180)) and `None` variables (MR [#172](https://gitlab.com/cosapp/cosapp/-/merge_requests/172)).
 * Bug fix on event time calculation involving array transients (MR [#177](https://gitlab.com/cosapp/cosapp/-/merge_requests/177)).
 * Bug fix on possible name conflicts in connector storage (MR [#173](https://gitlab.com/cosapp/cosapp/-/merge_requests/173)).
 * Fix inconsistent behaviour of `System.add_child` when a `pulling` error is raised (MR [#197](https://gitlab.com/cosapp/cosapp/-/merge_requests/197)).
@@ -203,79 +265,79 @@
 
 ### New features & API changes
 
 * Simplification of driver `Optimizer`:
   * Suppression of sub-driver `runner` (MR [#136](https://gitlab.com/cosapp/cosapp/-/merge_requests/136)). This change introduces new methods `set_objective`, `add_unknowns` and `add_constraints` in driver `Optimizer`.
   * Optimization constraints are now declared with human-readable expressions in `Optimizer.add_constraints` (MR [#138](https://gitlab.com/cosapp/cosapp/-/merge_requests/138)).
 
-Before:
+  Before:
+    
+  ```python
+  from cosapp.drivers import Optimizer
   
-```python
-from cosapp.drivers import Optimizer
-
-s = SomeSystem('s')
-optim = s.add_driver(Optimizer('optim'))
-
-optim.runner.set_objective('cost')
-optim.runner.add_unknown(['a', 'b', 'p_in.x'])
-# Enter constraints as non-negative expressions:
-optim.runner.add_constraints([
-    "b - a",  # b >= a
-    "a",      # a >= 0
-    "1 - a",  # a <= 1
-])
-optim.runner.add_constraints(
-    "p_out.y",
-    inequality = False,  # p_out.y == 0
-)
-
-s.run_drivers()
-```
-
-After:
-  
-```python
-optim.set_objective('cost')
-optim.add_unknown(['a', 'b', 'p_in.x'])
-optim.add_constraints(
-    "b >= a",
-    "0 <= a <= 1",
-    "p_out.y == 0",
-)
-```
+  s = SomeSystem('s')
+  optim = s.add_driver(Optimizer('optim'))
+  
+  optim.runner.set_objective('cost')
+  optim.runner.add_unknown(['a', 'b', 'p_in.x'])
+  # Enter constraints as non-negative expressions:
+  optim.runner.add_constraints([
+      "b - a",  # b >= a
+      "a",      # a >= 0
+      "1 - a",  # a <= 1
+  ])
+  optim.runner.add_constraints(
+      "p_out.y",
+      inequality = False,  # p_out.y == 0
+  )
+  
+  s.run_drivers()
+  ```
+  
+  After:
+    
+  ```python
+  optim.set_objective('cost')
+  optim.add_unknown(['a', 'b', 'p_in.x'])
+  optim.add_constraints(
+      "b >= a",
+      "0 <= a <= 1",
+      "p_out.y == 0",
+  )
+  ```
 
   * New, convenient iterators and setters for ports (MR [#137](https://gitlab.com/cosapp/cosapp/-/merge_requests/137)):
   
-```python
-from cosapp.base import Port, System
-
-class XyzPort(Port):
-    def setup(self):
-        self.add_variable('x')
-        self.add_variable('y')
-        self.add_variable('z')
-
-class SomeSystem(System):
-    def setup(self):
-        self.add_input(XyzPort, 'p_in')
-        self.add_output(XyzPort, 'p_out')
-    
-    def compute(self):
-        self.p_out.set_from(self.p_in)  # assign values from `p_in`
-        self.p_out.z = 0.0
-
-s = SomeSystem('s')
-# Multi-variable setter `set_values`
-s.p_in.set_values(x=1, y=-0.5, z=0.1)
-
-s.run_once()
-# Dict-like (key, value) iterator `items`:
-for varname, value in s.p_out.items():
-    print(f"p_out.{varname} = {value})
-```
+  ```python
+  from cosapp.base import Port, System
+  
+  class XyzPort(Port):
+      def setup(self):
+          self.add_variable('x')
+          self.add_variable('y')
+          self.add_variable('z')
+  
+  class SomeSystem(System):
+      def setup(self):
+          self.add_input(XyzPort, 'p_in')
+          self.add_output(XyzPort, 'p_out')
+      
+      def compute(self):
+          self.p_out.set_from(self.p_in)  # assign values from `p_in`
+          self.p_out.z = 0.0
+  
+  s = SomeSystem('s')
+  # Multi-variable setter `set_values`
+  s.p_in.set_values(x=1, y=-0.5, z=0.1)
+  
+  s.run_once()
+  # Dict-like (key, value) iterator `items`:
+  for varname, value in s.p_out.items():
+      print(f"p_out.{varname} = {value})
+  ```
 
 ### Documentation
 
 * Updated tutorials on ports (MR [#139](https://gitlab.com/cosapp/cosapp/-/merge_requests/139)) and on optimization (MR [#140](https://gitlab.com/cosapp/cosapp/-/merge_requests/140)).
 
 ### Bug fixes and code quality
```

### Comparing `cosapp-0.13.1/README.md` & `cosapp-0.14.0/README.md`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/config.py` & `cosapp-0.14.0/cosapp/core/config.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/configuration_schema.json` & `cosapp-0.14.0/cosapp/core/configuration_schema.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/eval_str.py` & `cosapp-0.14.0/cosapp/core/eval_str.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/module.py` & `cosapp-0.14.0/cosapp/core/module.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,60 +31,63 @@
     # by activating decorators of the kind @abc.abstractclass, etc.
     """
     A class to describe generic properties and functions of a component that can be single or
     made of child `Module`.
 
     Parameters
     ----------
-    name: str
-        Name of the `Module`
+    - name [str]:
+        `Module` name
 
     Attributes
     ----------
-    name : str
+    - name [str]:
         `Module` name
-    children : Dict[str, Module]
+    - children [dict[str, Module]]:
         Sub-modules of current `Module`, referenced by names.
-    parent : Module
+    - parent [Module]:
         Parent `Module` of current `Module`; `None` if there is no parent.
-    exec_order : MappingView[str]
+    - exec_order [Iterator[str]]:
         Execution order in which sub-modules should be computed.
+    - description [str]:
+        `Module` description.
 
-    _active : bool
+    - _active [bool]:
         If False, the `Module` will not execute its `run_once` method
-    _compute_calls: int
+    - _compute_calls [int]:
         Store if the number of times :py:meth:`~cosapp.core.module.Module.compute` was called (due to inhibition of clean status)
 
     Signals
     -------
-    setup_ran : Signal()
+    - setup_ran [Signal]:
         Signal emitted after :py:meth:`~cosapp.core.module.Module.call_setup_run` execution
-    computed : Signal()
+    - computed [Signal]:
         Signal emitted after the :py:meth:`~cosapp.core.module.Module.compute` stack (= after :py:meth:`~cosapp.core.module.Module._post_compute`) execution
-    clean_ran : Signal()
+    - clean_ran [Signal]:
         Signal emitted after the :py:meth:`~cosapp.core.module.Module.call_clean_run` execution
     """
 
     __slots__ = (
         '__weakref__', '_name', 'children', 'parent', '_active',
         '_compute_calls', 'setup_ran', 'computed', 'clean_ran',
-        '__members',
+        '__members', '_desc',
     )
 
     _name_check = NameChecker(excluded=CommonPorts.names())
 
     def __init__(self, name: str):
         """`Module` constructor
 
         Parameters
         ----------
-        name: str, optional
-            Name of the `Module`
+        - name [str]:
+            Module name
         """
         self._name = self._name_check(name)
+        self._desc = ""
         self.children: Dict[str, Module] = collections.OrderedDict()
         self.parent: Optional[Module] = None
         self._active: bool = True
         self._compute_calls: int = 0
 
         # Signals
         self.setup_ran = Signal(name="cosapp.core.module.Module.setup_ran")
@@ -145,14 +148,24 @@
         return self._name
 
     @name.setter
     def name(self, name: str) -> None:
         self._name = self._name_check(name)
 
     @property
+    def description(self) -> str:
+        """str: Module description"""
+        return self._desc
+
+    @description.setter
+    def description(self, desc: str) -> None:
+        check_arg(desc, 'description', str)
+        self._desc = desc
+
+    @property
     def exec_order(self) -> MappingView[str]:
         """MappingView[str]: sub-module execution order, as a name iterator"""
         return self.children.keys()
 
     @exec_order.setter
     def exec_order(self, namelist: Sequence[str]) -> None:
         if not isinstance(namelist, Sequence):
@@ -290,27 +303,33 @@
             child = child.parent
             if child is None:
                 raise ValueError(
                     f"{other.name!r} is not a child of {self.name!r}."
                 )
         return ".".join(reversed(path))
 
-    def add_child(self, child: Child, execution_index: Optional[int] = None) -> Child:
+    def add_child(self, child: Child, execution_index: Optional[int]=None, desc="") -> Child:
         """Add a child `Module` to the current `Module`.
 
         When adding a child `Module`, it is possible to specified its position
         in the execution order.
 
         Parameters
         ----------
-        child: Module
+        - child [Module]:
             `Module` to add to the current `Module`
-        execution_index: int, optional
+        - execution_index [int, optional]:
             Index of the execution order list at which the `Module` should be inserted;
             default latest.
+        - desc [str, optional]:
+            Module description in the context of its parent module.
+
+        Returns
+        -------
+        `child`
         """
         # Type validation
         check_arg(child, 'child', Module)
 
         specific_order = None
         if execution_index is not None:
             check_arg(execution_index, 'execution_index', Integral, lambda i: i >= 0)
@@ -320,14 +339,15 @@
         if child.name in self.children:
             raise ValueError(
                 "{} {!r} cannot be added, as Module already contains an object with the same name"
                 "".format(type(child).__qualname__, child.name)
             )
 
         child.parent = self
+        child.description = desc
         self.children[child.name] = child
         self._add_member(child.name)
 
         if specific_order:
             self.exec_order = specific_order
 
         return child
```

### Comparing `cosapp-0.13.1/cosapp/core/numerics/basics.py` & `cosapp-0.14.0/cosapp/core/numerics/basics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 import logging
 from collections import OrderedDict
 from numbers import Number
+from dataclasses import dataclass, field
 from typing import (
     Any, Dict, Iterable, Optional,
     Sequence, Union, Tuple, List,
     Set, Callable, NamedTuple,
 )
 
 import numpy
@@ -15,53 +16,61 @@
 from cosapp.core.numerics.residues import Residue, DeferredResidue
 from cosapp.utils.naming import natural_varname
 from cosapp.utils.helpers import check_arg
 
 logger = logging.getLogger(__name__)
 
 
+def default_array_factory(shape=0, dtype=float):
+    """Default factory for dataclass fields."""
+    def factory():
+        return numpy.empty(shape, dtype=dtype)
+    return factory
+
+
+@dataclass
 class SolverResults:
-    """Storage class for solver solution
+    """Data class for solver solution
 
     Attributes
     ----------
-    x : Sequence[float]
-        Solution vector
-    success : bool
+    - x [numpy.ndarray[float]]:
+        Solution vector.
+    - fun [numpy.ndarray[float]]:
+        Values of the objective function.
+    - success [bool]:
         Whether or not the solver exited successfully.
-    message : str
+    - message [str]:
         Description of the cause of the termination.
-    fun : ndarray
-        Values of objective function.
-    jac_lup : (ndarray[float], ndarray[int]), optional
-        LU decomposition of Jacobian given as tuple (LU, perm); (None, None) if not available.
-    jac : ndarray, optional
+    - tol [float, optional]:
+        Tolerance level; `NaN` if not available.
+    - jac [numpy.ndarray[float], optional]
         Values of function Jacobian; None if not available.
-    jac_errors : dict, optional
-        Dictionary with singular Jacobian matrix error indexes
-    jac_calls : int
-        Number of calls to the Jacobian matrix calculation
-    fres_calls : int
-        Number of calls to the residues function
-    trace : List[Dict[str, Any]]
-        Resolution history (if requested) with the evolution of x, residues and jacobian
+    - jac_lup [tuple(numpy.ndarray[float], numpy.ndarray[int]), optional]
+        LU decomposition of Jacobian given as tuple (LU, perm); (None, None) if not available.
+    - jac_calls [int]:
+        Number of calls to the Jacobian matrix calculation.
+    - fres_calls [int]:
+        Number of calls to the residues function.
+    - jac_errors [dict, optional]:
+        Dictionary with singular Jacobian matrix error indexes.
+    - trace [list[dict[str, Any]]]:
+        Resolution history (if requested) with the evolution of x, residues and jacobian.
     """
-
-    def __init__(self):
-        self.x = list()  # type: Sequence[float]
-        self.success = False  # type: bool
-        self.message = ''  # type: str
-        self.fun = numpy.array([], dtype=float)  # type: numpy.ndarray
-        self.tol = numpy.nan
-        self.jac_lup = (None, None)  # type: Optional[Tuple[numpy.ndarray, numpy.ndarray]]
-        self.jac = None  # type: Optional[numpy.ndarray]
-        self.jac_errors = dict()
-        self.jac_calls = 0  # type: int
-        self.fres_calls = 0  # type: int
-        self.trace = list()  # type: List[Dict[str, Any]]
+    x: numpy.ndarray = field(default_factory=default_array_factory())
+    fun: numpy.ndarray = field(default_factory=default_array_factory())
+    success: bool = False
+    message: str = ''
+    tol: float = numpy.nan
+    jac: Optional[numpy.ndarray] = None
+    jac_lup: Optional[Tuple[numpy.ndarray, numpy.ndarray]] = (None, None)
+    jac_calls: int = 0
+    fres_calls: int = 0
+    jac_errors: dict = field(default_factory=dict)
+    trace: List[Dict[str, Any]] = field(default_factory=list)
 
 
 class WeakDeferredResidue(NamedTuple):
     deferred: DeferredResidue
     weak: bool = False
 
     @property
```

### Comparing `cosapp-0.13.1/cosapp/core/numerics/boundary.py` & `cosapp-0.14.0/cosapp/core/numerics/boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,37 +176,43 @@
                     )
                 )
         self.__info.mask = mask
 
     @property
     def value(self) -> Union[Number, numpy.ndarray]:
         """Number or numpy.ndarray: Current value of the boundary."""
+        # TODO: incoherent behaviour
+        # should be equivalent to:
+        # return value if mask is None else value[mask]
         value = self.__info.ref.value
-        if self.mask is None:
+        mask = self.mask
+        if mask is None:
             return value
-        elif numpy.any(self.mask):
-            return value[self.mask]
-        else:
-            return numpy.empty(0)
+        if numpy.any(mask):
+            return value[mask]
+        return numpy.empty(0)
 
     @value.setter
     def value(self, new: Union[Number, numpy.ndarray]) -> None:
         ref = self.__info.ref
+        mask = self.mask
 
-        if self.mask is None:
+        if mask is None:
             if not numpy.array_equal(ref.value, new):
                 ref.value = new
                 self.touch()
-        elif numpy.any(self.mask) and not numpy.array_equal(ref.value[self.mask], new):
-            ref.value[self.mask] = new
+
+        elif numpy.any(mask) and not numpy.array_equal(ref.value[mask], new):
+            ref.value[mask] = new
             self.touch()
 
     def touch(self) -> None:
-        """Set owner system as 'dirty'."""
+        """Set owner port as 'dirty'."""
         self.port.touch()
+        self.port.owner.touch()
 
     @property
     def default_value(self) -> Union[Number, numpy.ndarray, None]:
         """Number, numpy.ndarray or None: default value for the boundary."""
         if self._default_value is None or self.mask is None:
             return self._default_value
         else:
@@ -313,26 +319,26 @@
     def set_to_default(self) -> None:
         """Set the current value with the default one."""
         if self._default_value is None:
             # This is to verbose and not understable with a classical use
             # logger.warning(f"No default value given for variable '{self.context.name}.{self.name}'. It will be skipped.")
             return
 
-        nan_mask = numpy.isfinite(self._default_value)
-        if self.mask is None:
-            if numpy.all(nan_mask):
+        def apply_mask(mask: numpy.ndarray):
+            if numpy.all(mask):
                 self.value = self.default_value
             else:
-                self.value[nan_mask] = self.default_value[nan_mask]
+                self.value[mask] = self.default_value[mask]
+
+        nan_mask = numpy.isfinite(self._default_value)
+        if self.mask is None:
+            apply_mask(nan_mask)
         else:
             sub_mask = nan_mask[self.mask]
-            if numpy.all(sub_mask):
-                self.value = self.default_value
-            else:
-                self.value[sub_mask] = self.default_value[sub_mask]
+            apply_mask(sub_mask)
 
 
 class Unknown(Boundary):
     """Numerical solver unknown.
 
     Parameters
     ----------
```

### Comparing `cosapp-0.13.1/cosapp/core/numerics/enum.py` & `cosapp-0.14.0/cosapp/core/numerics/enum.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/numerics/residues.py` & `cosapp-0.14.0/cosapp/core/numerics/residues.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/numerics/root.py` & `cosapp-0.14.0/cosapp/core/numerics/root.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/numerics/sobol_seq.py` & `cosapp-0.14.0/cosapp/core/numerics/sobol_seq.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/signal/signal.py` & `cosapp-0.14.0/cosapp/core/signal/signal.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/signal/slot.py` & `cosapp-0.14.0/cosapp/core/signal/slot.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/tests/test_AssignString.py` & `cosapp-0.14.0/cosapp/core/tests/test_AssignString.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/tests/test_ContextLocals.py` & `cosapp-0.14.0/cosapp/core/tests/test_ContextLocals.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/tests/test_EvalString.py` & `cosapp-0.14.0/cosapp/core/tests/test_EvalString.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/tests/test_Module.py` & `cosapp-0.14.0/cosapp/core/tests/test_Module.py`

 * *Files 11% similar despite different names*

```diff
@@ -95,22 +95,48 @@
     ("outwards", ValueError),
     (23, TypeError),
     (1.0, TypeError),
     (dict(a=True), TypeError),
     (list(), TypeError),
 ])
 def test_Module__init__(name, error):
+    """Test Module initialization"""
     if error is None:
         module = Module(name)
         assert module.name == name
+        assert module.description == ""
+
     else:
         with pytest.raises(error):
             Module(name)
 
 
+@pytest.mark.parametrize(
+    "desc, expected", [
+        ("A really great module", does_not_raise()),
+        ("~~ non-alphanumeric start ~~", does_not_raise()),
+        ("", does_not_raise()),
+        (None, pytest.raises(TypeError)),
+        (0, pytest.raises(TypeError)),
+        (0.0, pytest.raises(TypeError)),
+        (list(), pytest.raises(TypeError)),
+        (dict(cool=True), pytest.raises(TypeError)),
+    ],
+)
+def test_Module_description(desc: str, expected):
+    """Test `description` getter & setter"""
+    module = Module('foo')
+    assert module.name == "foo"
+    assert module.description == ""
+
+    with expected:
+        module.description = desc
+        assert module.description == desc
+
+
 def test_Module__weakref__(fake):
     with no_exception():
         proxy = weakref.proxy(fake)
 
 
 def test_Module_name_setter():
     module = Module("foo")
@@ -179,14 +205,22 @@
     m.run_once()
     assert m.compute_calls == 1
 
     m.call_setup_run()  # Reset counter
     assert m.compute_calls == 0
 
 
+def test_Module_add_child_desc():
+    top = Module("top")
+    foo = top.add_child(Module("foo"))
+    bar = top.add_child(Module("bar"), desc="A great sub-module")
+    assert foo.description == ""
+    assert bar.description == "A great sub-module"
+
+
 def test_Module_size():
     s = Module("s")
     T = Module("T")
     u = Module("u")
     v = Module("v")
 
     s.add_child(T)
```

### Comparing `cosapp-0.13.1/cosapp/core/tests/test_coSAppConfiguration.py` & `cosapp-0.14.0/cosapp/core/tests/test_coSAppConfiguration.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/tests/test_time.py` & `cosapp-0.14.0/cosapp/core/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/time.py` & `cosapp-0.14.0/cosapp/core/time.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/core/variableref.py` & `cosapp-0.14.0/cosapp/core/variableref.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/__init__.py` & `cosapp-0.14.0/cosapp/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/abstractsetofcases.py` & `cosapp-0.14.0/cosapp/drivers/abstractsetofcases.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     @abc.abstractmethod
     def _build_cases(self) -> None:
         """Generator of cases."""
         pass
 
     def _postcase(self, case_idx: int, case: Any):
-        """Hook to be called before running each case.
+        """Hook to be called after running each case.
         
         Parameters
         ----------
         case_idx : int
             Index of the case
         case : Any
             Parameters for this case
```

### Comparing `cosapp-0.13.1/cosapp/drivers/abstractsolver.py` & `cosapp-0.14.0/cosapp/drivers/abstractsolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,17 @@
             
             else:
                 logger.debug(f"Skip {self.name} execution - Inactive")
 
     def _precompute(self) -> None:
         # TODO we should check that all variables are of numerical types
         super()._precompute()
+        self.touch_unknowns()
+
+    def touch_unknowns(self):
         for unknown in self.problem.unknowns.values():
             unknown.touch()
 
     @abc.abstractmethod
     def set_iteratives(self, x: Sequence[float]) -> None:
         pass
```

### Comparing `cosapp-0.13.1/cosapp/drivers/driver.py` & `cosapp-0.14.0/cosapp/drivers/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,19 +65,19 @@
         owner: Optional["cosapp.systems.System"] = None,
         **kwargs
     ) -> None:
         """Initialize driver
 
         Parameters
         ----------
-        name: str
-            Name of the `Driver`.
-        owner: System, optional
+        - name [str]:
+            Driver name
+        - owner [System, optional]:
             :py:class:`~cosapp.systems.system.System` to which driver belongs; defaults to `None`.
-        **kwargs: Dict[str, Any]
+        - **kwargs:
             Optional keywords arguments.
         """
         from cosapp.systems import System
 
         super().__init__(name)
         self._owner: Optional[System] = None
         self._recorder: Optional[BaseRecorder] = None
@@ -205,46 +205,46 @@
         if self.owner.parent is None and self.parent is None:
             logger.info(
                 " # Ending driver {!r} on {!r} in {} seconds\n".format(
                     self.name, self.owner.name, round(time.time() - self.start_time, 3)
                 )
             )
 
-    def add_child(self, child: AnyDriver, execution_index: Optional[int] = None) -> AnyDriver:
+    def add_child(self, child: AnyDriver, execution_index: Optional[int]=None, desc="") -> AnyDriver:
         """Add a child `Driver` to the current `Driver`.
 
         When adding a child `Driver`, it is possible to specified its position in the execution
         order.
 
         Parameters
         ----------
-        child: Driver
+        - child: Driver
             `Driver` to add to the current `Driver`
-        execution_index: int, optional
+        - execution_index: int, optional
             Index of the execution order list at which the `Module` should be inserted;
             default latest.
+        - desc [str, optional]:
+            Sub-driver description in the context of its parent driver.
 
         Returns
         -------
         `child`
 
         Notes
         -----
         The added child will have its owner set to that of current driver.
         """
         check_arg(child, 'child', Driver)
-        
-        driver = super().add_child(child, execution_index)
-        driver.owner = self.owner
+        child.owner = self.owner
 
-        return driver
+        return super().add_child(child, execution_index, desc)
 
-    def add_driver(self, child: AnyDriver, execution_index: Optional[int] = None) -> AnyDriver:
+    def add_driver(self, child: AnyDriver, execution_index: Optional[int]=None, desc="") -> AnyDriver:
         """Alias for :py:meth:`~cosapp.drivers.driver.Driver.add_child`."""
-        return self.add_child(child, execution_index)
+        return self.add_child(child, execution_index, desc)
 
     def add_recorder(self, recorder: Recorder) -> Recorder:
         check_arg(recorder, 'recorder', BaseRecorder)
 
         self._recorder = recorder
         self._recorder.watched_object = self.owner
         self._recorder._owner = self
```

### Comparing `cosapp-0.13.1/cosapp/drivers/influence.py` & `cosapp-0.14.0/cosapp/drivers/influence.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/iterativecase.py` & `cosapp-0.14.0/cosapp/drivers/iterativecase.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/lineardoe.py` & `cosapp-0.14.0/cosapp/drivers/lineardoe.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/metasystembuilder.py` & `cosapp-0.14.0/cosapp/drivers/metasystembuilder.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/montecarlo.py` & `cosapp-0.14.0/cosapp/drivers/montecarlo.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/nonlinearsolver.py` & `cosapp-0.14.0/cosapp/drivers/nonlinearsolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,41 +98,43 @@
     @property
     def results(self) -> SolverResults:
         """SolverResults: structure containing solver results,
         together with additional detail.
         """
         return self.__results
 
-    def add_child(self, child: AnyDriver, execution_index: Optional[int] = None) -> AnyDriver:
+    def add_child(self, child: AnyDriver, execution_index: Optional[int]=None, desc="") -> AnyDriver:
         """Add a child `Driver` to the current `Driver`.
 
         When adding a child `Driver`, it is possible to specified its position in the execution order.
 
         Child `Port`, `inwards` and `outwards` can also be pulled at the parent level by providing either
         the name of the port/inward/outward or a list of them or the name mapping of the child element
         (dictionary keys) to the parent element (dictionary values).
         If the argument is not a dictionary, the name in the parent system will be the same as in the child.
 
         Parameters
         ----------
-        child: Module
-            `Module` to add to the current `Module`
-        execution_index: int, optional
+        - child: Driver
+            `Driver` to add to the current `Driver`
+        - execution_index: int, optional
             Index of the execution order list at which the `Module` should be inserted;
-            default is latest.
+            default latest.
+        - desc [str, optional]:
+            Sub-driver description in the context of its parent driver.
 
         Notes
         -----
         The added child will have its owner set to match the one of the current driver.
         """
         default_driver = self._default_driver_name
         if len(self.children) == 1 and default_driver in self.children:
             self.pop_child(default_driver)
         self.compute_jacobian = True
-        return super().add_child(child, execution_index)
+        return super().add_child(child, execution_index, desc)
 
     def is_standalone(self) -> bool:
         """Is this Driver able to solve a system?
 
         Returns
         -------
         bool
@@ -259,14 +261,15 @@
             case.add_offdesign_problem(handler.offdesign)
             # Assemble case problems (design & off-design)
             wrapper = get_key_wrapper(case)
             problem.extend(local.design, copy=False, residue_wrapper=wrapper)
             problem.extend(local.offdesign, copy=False, unknown_wrapper=wrapper, residue_wrapper=wrapper)
             self.initial_values = numpy.append(self.initial_values, case.get_init(self.force_init))
 
+        self.touch_unknowns()
         logger.debug(
             "\n".join([
                 "Mathematical problem:",
                 f"{'<empty>' if self.problem.is_empty() else self.problem}",
             ])
         )
 
@@ -434,23 +437,26 @@
         bool
             Should the provided record be logged?
         """
         message = record.getMessage()
         activate = getattr(record, "activate", None)
         emit_record = super().log_debug_message(handler, record, format)
 
+        try:
+            self.options["history"] = activate
+        except (KeyError, TypeError):
+            pass
+
         if message.endswith("call_setup_run") or message.endswith("call_clean_run"):
             emit_record = False
 
         elif activate == True:
-            self.options["history"] = True
             emit_record = False
 
         elif activate == False:
-            self.options["history"] = False
             emit_record = False
 
             message = ""
             unknown_trace = None
             residue_trace = None
             residue_names = self.problem.residues_names
             unknown_names = self.problem.unknowns_names
```

### Comparing `cosapp-0.13.1/cosapp/drivers/optimizer.py` & `cosapp-0.14.0/cosapp/drivers/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,14 +287,15 @@
 
     def setup_run(self):
         """Method called once before starting any simulation."""
         super().setup_run()
         
         # Resolve unknown aliasing and connected unknowns
         self.problem = dealias_problem(self._raw_problem)
+        self.touch_unknowns()
 
     def _fun_wrapper(self, expression: EvalString) -> Callable[[numpy.ndarray], float]:
         """Wrapper around objective and constraint expression to propagate the x values in the
             `System` owner.
 
         Parameters
         ----------
```

### Comparing `cosapp-0.13.1/cosapp/drivers/optionaldriver.py` & `cosapp-0.14.0/cosapp/drivers/optionaldriver.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/runonce.py` & `cosapp-0.14.0/cosapp/drivers/runonce.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/runsinglecase.py` & `cosapp-0.14.0/cosapp/drivers/runsinglecase.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         owner_changed = False
         for assignment in self.case_values:
             value, changed = assignment.exec()
             if changed:
                 owner_changed = True
 
         if owner_changed:
-            self.owner.set_dirty(PortType.IN)
+            self.owner.touch()
 
         # Set offdesign variables
         design_unknowns = set(self.design.unknowns)
         problem = self.get_problem()
         for name, unknown in problem.unknowns.items():
             if name in design_unknowns:
                 continue
```

### Comparing `cosapp-0.13.1/cosapp/drivers/time/euler.py` & `cosapp-0.14.0/cosapp/drivers/time/euler.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/interfaces.py` & `cosapp-0.14.0/cosapp/drivers/time/interfaces.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/runge_kutta.py` & `cosapp-0.14.0/cosapp/drivers/time/runge_kutta.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/scenario.py` & `cosapp-0.14.0/cosapp/drivers/time/scenario.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_BouncingBall.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_BouncingBall.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_DiscreteStepper.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_DiscreteStepper.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_EulerExplicit.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_EulerExplicit.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_ExplicitTimeDriver.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_ExplicitTimeDriver.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_InterpolAssignString.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_InterpolAssignString.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_Interpolator.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_Interpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_NewtonPendulum.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_NewtonPendulum.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_RungeKutta.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_RungeKutta.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_Scenario.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_Scenario.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_SystemInterpolator.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_SystemInterpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_TimeAssignString.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_TimeAssignString.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_TimeStepManager.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_TimeStepManager.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_TimeUnknownDict.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_TimeUnknownDict.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_TimeUnknownStack.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_TimeUnknownStack.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_TimeVarManager.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_TimeVarManager.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_TwoPointCubicInterpolator.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_TwoPointCubicInterpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_TwoPointCubicPolynomial.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_TwoPointCubicPolynomial.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_event_cascades.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_event_cascades.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/tests/test_modevar_init.py` & `cosapp-0.14.0/cosapp/drivers/time/tests/test_modevar_init.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/time/utils.py` & `cosapp-0.14.0/cosapp/drivers/time/utils.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/utils.py` & `cosapp-0.14.0/cosapp/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/drivers/validitycheck.py` & `cosapp-0.14.0/cosapp/drivers/validitycheck.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/multimode/discreteStepper.py` & `cosapp-0.14.0/cosapp/multimode/discreteStepper.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/multimode/event.py` & `cosapp-0.14.0/cosapp/multimode/event.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/multimode/zeroCrossing.py` & `cosapp-0.14.0/cosapp/multimode/zeroCrossing.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/patterns/observer.py` & `cosapp-0.14.0/cosapp/patterns/observer.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/patterns/singleton.py` & `cosapp-0.14.0/cosapp/patterns/singleton.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/patterns/visitor.py` & `cosapp-0.14.0/cosapp/patterns/visitor.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/ports/connectors.py` & `cosapp-0.14.0/cosapp/ports/connectors.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/ports/enum.py` & `cosapp-0.14.0/cosapp/ports/enum.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/ports/mode_variable.py` & `cosapp-0.14.0/cosapp/ports/mode_variable.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/ports/port.py` & `cosapp-0.14.0/cosapp/ports/port.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,18 @@
         direction : {PortType.IN, PortType.OUT}
             Port direction
         """
         if not isinstance(direction, PortType):
             raise TypeError(f"Direction must be PortType; got {direction}.")
         from cosapp.systems import System
 
+        self.__is_clean = False
         self._variables: Dict[str, BaseVariable] = OrderedDict()
         self._name: str = self._name_check(name)
+        self._desc: str = ""
         self._direction: PortType = direction
         self._owner: Optional[System] = None
         self.__clearance: Scope = None
         self.scope_clearance = Scope.PRIVATE
 
     def accept(self, visitor: visitor.Visitor) -> None:
         """Specifies course of action when visited by `visitor`"""
@@ -105,32 +107,51 @@
             path = owner.path_namelist()
             if trim_root:
                 path = path[1:]
         path.append(self.name)
         return ".".join(path)
 
     @property
+    def description(self) -> str:
+        """str: Port description"""
+        return self._desc
+
+    @description.setter
+    def description(self, desc: str) -> None:
+        check_arg(desc, 'description', str)
+        self._desc = desc
+
+    @property
     def direction(self) -> PortType:
         """:obj:`PortType.IN` or :obj:`PortType.OUT` : Port direction"""
         return self._direction
 
     @property
     def is_input(self) -> bool:
         """bool: True if port is an input, False otherwise."""
         return self._direction == PortType.IN
 
     @property
     def is_output(self) -> bool:
         """bool: True if port is an output, False otherwise."""
         return self._direction == PortType.OUT
 
+    @property
+    def is_clean(self) -> bool:
+        return self.__is_clean
+
+    def set_clean(self) -> None:
+        """Set port as 'clean'."""
+        self.__is_clean = True
+
     def touch(self) -> None:
-        """Set owner system as 'dirty' in port direction."""
-        if self._owner:
-            self._owner.set_dirty(self.direction)
+        """Set port as 'dirty'."""
+        self.__is_clean = False
+        if self._owner and self.is_input:
+            self._owner.touch()
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}: {self.serialize_data()!r}"
 
     def _repr_markdown_(self) -> str:
         """Returns the representation of this port variables in Markdown format.
 
@@ -237,15 +258,15 @@
         setattr(self, name, value)
 
     # TODO should we override __setattr__ to forward setting to the source port? and/or raise an
     #   error if it is not possible - for example if the source is an output variable
     def __set_notype_checking(self, key, value):
         super().__setattr__(key, value)
 
-        if key in self._variables:
+        if self.__is_clean and key in self._variables:
             self.touch()
 
     def validate(self, key: str, value: Any) -> None:
         """Check if a variable is in the scope of the user and the type is valid.
         
         Parameters
         ----------
@@ -795,15 +816,15 @@
             `Port` name
         direction : {PortType.IN, PortType.OUT}
             `Port` direction
         variables : Dict[str, Any], optional
             Dictionary of variables with their value and details; default: None = default value
         """
         super().__init__(name, direction)
-        self._locked = False  # type: bool
+        self.__locked = False  # type: bool
 
         self.setup()
 
         if variables is not None:
             check_arg(variables, "variables", dict)
             for name, value in variables.items():
                 variable_value = value
@@ -822,15 +843,15 @@
                             variable_value = value
                         else:
                             raise
 
                 if variable_value is not None:
                     self[name] = variable_value
 
-        self._locked = True
+        self.__locked = True
 
     def setup(self) -> None:
         """`Port` variables are defined in this function by calling `add_variable`.
 
         This function allows to populate a customized `Port` class. The `add_variable`
         function is only callable in the frame of this function.
 
@@ -892,15 +913,15 @@
         desc : str, optional
             Variable description; default ''        
         distribution : Distribution, optional
             Probability distribution of the variable; default None (no distribution)
         scope : Scope {PRIVATE, PROTECTED, PUBLIC}, optional
             Variable visibility; default PUBLIC
         """
-        if self._locked:
+        if self.__locked:
             raise AttributeError("add_variable cannot be called outside `setup`.")
 
         super().add_variable(
             name,
             value=value,
             unit=unit,
             dtype=dtype,
```

### Comparing `cosapp-0.13.1/cosapp/ports/unit_library.ini` & `cosapp-0.14.0/cosapp/ports/unit_library.ini`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/ports/units.py` & `cosapp-0.14.0/cosapp/ports/units.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/ports/variable.py` & `cosapp-0.14.0/cosapp/ports/variable.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/recorders/dataframe_recorder.py` & `cosapp-0.14.0/cosapp/recorders/dataframe_recorder.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/recorders/dsv_recorder.py` & `cosapp-0.14.0/cosapp/recorders/dsv_recorder.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/recorders/recorder.py` & `cosapp-0.14.0/cosapp/recorders/recorder.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/systems/__init__.py` & `cosapp-0.14.0/cosapp/systems/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/systems/externalsystem.py` & `cosapp-0.14.0/cosapp/systems/externalsystem.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/systems/metamodels.py` & `cosapp-0.14.0/cosapp/systems/metamodels.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/systems/processsystem.py` & `cosapp-0.14.0/cosapp/systems/processsystem.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/systems/system.py` & `cosapp-0.14.0/cosapp/systems/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     manual = "manual"
     best_fidelity_to_cost = "best_fidelity_to_cost_ratio"
     high_fidelity = "highest_fidelity"
     low_fidelity = "lowest_fidelity"
     high_cost = "highest_cost"
     low_cost = "lowest_cost"
 
+
 # Default value use in list_inputs method to be able to tell if the caller set a value to out_stream
 _DEFAULT_OUT_STREAM = object()
 
 
 class System(Module, TimeObserver):
     # TODO check and complete documentation
     """
@@ -112,15 +113,15 @@
         Variable name mapping to its value by reference
 
     _locked : bool
         if True, `add_input`, `add_output`, `add_inward` and `add_outward` are desactivated. This is
         the default behavior outside the `setup` function.
     _active : bool
         if False, the `System` will not execute its `compute` method
-    _is_clean : dict[bool]
+    _is_tree_clean : bool
         Reflects the status of the inputs and outputs. `clean` status means the group of ports was not updated since
         last computation of the `System`
     _compute_calls: bool
         Store if the `System` was computed at last call or not (due to inhibition of clean status)
 
     Examples
     --------
@@ -156,15 +157,15 @@
     >>>             self.max_roots.x = max(self.roots)
     >>>         else:
     >>>             self.roots = None
     >>>             self.max_roots.x = np.nan
     """
 
     __slots__ = (
-        '__context_lock', '_is_clean', '_locked', '_math',
+        '__context_lock', '_is_tree_clean', '_locked', '_math',
         'design_methods', 'drivers', 'inputs', 'outputs', 'name2variable',
         '__readonly', '__events', '_meta', '__runner', '__input_mapping',
         '__loop_problem', '__child_connectors', '__pulling_connectors',
         '__free_problem',
     )
 
     INWARDS = CommonPorts.INWARDS.value  # type: ClassVar[str]
@@ -212,37 +213,43 @@
             if is_master:
                 cls.__master_set = False
                 BasePort.set_type_checking(True)  # Reactivate type ckecking
                 from cosapp.drivers.optionaldriver import OptionalDriver
                 OptionalDriver.set_inhibited(False)
 
     def __init__(self, name: str, **kwargs):
-        """Initialize a System"""
+        """Initialize a System
+
+        Parameters
+        ----------
+        - name [str]:
+            System name
+        """
         Module.__init__(self, name)
         TimeObserver.__init__(self, sign_in=False)
         from cosapp.drivers import Driver
 
         self._math = self.new_problem(name)
         self.__loop_problem = self.new_problem('loop')
         self.drivers = collections.OrderedDict()  # type: Dict[str, Driver]
         self.design_methods = dict()  # type: Dict[str, MathematicalProblem]
         self.__readonly = dict()  # type: Dict[str, Any]
         self.__ctor_kwargs = kwargs.copy()
 
         self.__context_lock = ContextLock()
         self.__free_problem = ContextLock()
-        self.inputs = collections.OrderedDict()  # type: Dict[str, BasePort]
+        self.inputs = dict()  # type: Dict[str, BasePort]
         self.outputs = dict()  # type: Dict[str, BasePort]
         self.__events = dict()  # type: Dict[str, Event]
         # Connectors are grouped in a dictionary where the key is the sink system i.e. the receiving system
         self.__child_connectors = dict()  # type: Dict[str, List[SystemConnector]]
         self.__pulling_connectors = list()  # type: List[SystemConnector]
-        
+
         self._locked = False  # type: bool
-        self._is_clean = dict.fromkeys(PortType, False)
+        self._is_tree_clean = False
         self._meta = None
         self.__runner = self  # type: Union[System, SystemSurrogate]
         self.__input_mapping = None  # type: Dict[str, VariableReference]
         # For efficiency purpose, links to objects are stored as reference
         # !! name2variable must be the latest attribute set 
         # => lock __setattr__ on previously defined attributes
         self.name2variable = dict()  # type: Dict[str, VariableReference]
@@ -253,16 +260,17 @@
         self._add_port(ModeVarPort(System.MODEVARS_IN, PortType.IN))
         self._add_port(ModeVarPort(System.MODEVARS_OUT, PortType.OUT))
 
         # Customized subclass `System` before applying user wishes
         kwargs = self._initialize(**kwargs)
 
         # Customized the `System` according to user wishes
-        self.setup(**kwargs)
-        self.update()
+        with self.__free_problem:
+            self.setup(**kwargs)
+            self.update()
 
         self.__enforce_scope()
         self._locked = True
 
     def _update(self, dt) -> None:
         """Required by `TimeObserver` base class"""
         pass
@@ -286,41 +294,54 @@
             Direction of interest
 
         Returns
         -------
         bool
             Clean status
         """
-        return all(self._is_clean.values()) if direction is None else self._is_clean[direction]
+        if direction == PortType.IN:
+            ports = self.inputs.values()
+        elif direction == PortType.OUT:
+            ports = self.outputs.values()
+        else:
+            ports = self.ports()
+
+        return all(port.is_clean for port in ports)
 
     def set_clean(self, direction: PortType) -> None:
         """Set to clean ports of a certain direction.
 
         Parameters
         ----------
         direction : PortType
             Direction to set
         """
-        self._is_clean[direction] = True
+        ports = self.inputs.values() if direction == PortType.IN else self.outputs.values()
+        for port in ports:
+            port.set_clean()
 
     def set_dirty(self, direction: PortType) -> None:
         """Set to dirty ports of a certain direction.
 
         Parameters
         ----------
         direction : PortType
             Direction to set
         """
-        self._is_clean[direction] = False
-        if (
-            direction == PortType.IN
-            and self.parent is not None
-            and self.parent.is_clean(direction)
-        ):
-            self.parent.set_dirty(direction)
+        if direction == PortType.IN:
+            self.touch()
+        else:
+            for port in self.outputs.values():
+                port.touch()
+
+    def touch(self):
+        for system in self.path_to_root():
+            if not system._is_tree_clean:
+                break
+            system._is_tree_clean = False
 
     def __enforce_scope(self) -> None:
         """Encapsulate input ports for which some variables are out of scope."""
         if self._user_context is None:
 
             def get_context(
                 tags: FrozenSet[str], roles: FrozenSet[FrozenSet[str]]
@@ -396,17 +417,15 @@
         Returns
         -------
         Dict[str, Any]
             Optional keywords arguments not consumed by `_initialize`
         """
         return kwargs
 
-    def setup(
-        self, **kwargs
-    ) -> None:  # TODO update doc for **kwargs and add unit tests
+    def setup(self, **kwargs) -> None:
         """`System` port and/or child `System` are defined in this function.
 
         This function allows to populate a customized `System` class. The helper functions for the
         user are:
 
         - `add_input` : add an input port
         - `add_output` : add an output port
@@ -607,32 +626,34 @@
         """Dict[str, Any]: list of read-only properties and associated values"""
         return MappingProxyType(self.__readonly)
 
     def add_input(self,
         port_class: Type[AnyPort],
         name: str,
         variables: Optional[Dict[str, Any]] = None,
+        desc: str = "",
     ) -> AnyPort:
         """Add an input `Port` to the `System`.
 
         This function cannot be called outside `System.setup`.
 
         Parameters
         ----------
-        port_class: type
+        - port_class [type[Port]]
             Class of the `Port` to create
-        name : str
+        - name [str]:
             `Port` name
-        variables : Dict[str, Any], optional
+        - desc [str, optional]:
+            `Port` description
+        - variables [dict[str, Any], optional]:
             Dictionary of initial values (default: None)
 
         Returns
         -------
-        Port
-            The created port
+        The created port
 
         Examples
         --------
 
         >>> class MyModule(System):
         >>>     def setup(self):
         >>>         self.add_input(MyPort, 'p_in1')
@@ -643,40 +664,42 @@
         # Type validation
         check_arg(port_class, 'port_class', type)
         if not issubclass(port_class, Port):
             raise TypeError(
                 f"port_class should be a subclass of Port; got {type(port_class).__name__}."
             )
         new_port = port_class(name, PortType.IN, variables=variables)
-        self._add_port(new_port)
+        self._add_port(new_port, desc)
         self.__reset_input_mapping()
         return new_port
 
     def add_output(self,
         port_class: Type[AnyPort],
         name: str,
-        variables: Optional[Dict[str, Any]] = None
+        variables: Optional[Dict[str, Any]] = None,
+        desc: str = "",
     ) -> AnyPort:
         """Add an output `Port` to the `System`.
 
         This function cannot be called outside `System.setup`.
 
         Parameters
         ----------
-        port_class: type
+        - port_class [type[Port]]
             Class of the `Port` to create
-        name : str
+        - name [str]:
             `Port` name
-        variables : Dict[str, Any], optional
+        - desc [str, optional]:
+            `Port` description
+        - variables [dict[str, Any], optional]:
             Dictionary of initial values (default: None)
 
         Returns
         -------
-        Port
-            The created port
+        The created port
 
         Examples
         --------
 
         >>> class MyModule(System):
         >>>     def setup(self):
         >>>         self.add_output(MyPort, 'p_out1')
@@ -687,32 +710,33 @@
         # Type validation
         check_arg(port_class, 'port_class', type)
         if not issubclass(port_class, Port):
             raise TypeError(
                 f"port_class should be a subclass of Port; got {type(port_class).__name__}."
             )
         new_port = port_class(name, PortType.OUT, variables=variables)
-        self._add_port(new_port)
+        self._add_port(new_port, desc)
         return new_port
 
-    def _add_port(self, port: BasePort) -> None:
+    def _add_port(self, port: BasePort, desc="") -> None:
         """Add a port to the system
 
         Parameters
         ----------
         port : `BasePort`
             instance of a port class
         """
         if port.name in self:
             ptype = type(port).__qualname__
             raise ValueError(
                 f"Port {ptype} cannot be added as there already exists an object within system named {port.name!r}"
             )
 
         port.owner = self
+        port.description = desc
         if port.is_input:
             inputs = self.inputs
             if port.name in inputs:
                 raise ValueError(f"Port name {port.name!r} already exists as input")
             inputs[port.name] = port
             port_key = (port.name, VariableReference(context=self, mapping=inputs, key=port.name))
         elif port.is_output:
@@ -1208,16 +1232,16 @@
         if order == 1:
             return lambda s: f"d({s})/dt"
         elif order > 1:
             return lambda s: "d^{0}({1})/dt^{0}".format(s, order)
         return lambda s: s
 
     def _precompute(self) -> None:
-        if len(self._math.rates) > 0:
-            self.set_dirty(PortType.IN)  # ensured that system is recomputed at first time step
+        for rate in self._math.rates.values():
+            rate.touch()  # ensured that system is recomputed at first time step
 
     def check(self, name: Optional[str] = None) -> Union[Dict[str, Validity], Validity]:
         """Get variable value validity for a given variable, port or system or all of them.
 
         If `name` is not provided, returns a dictionary with the validity of all `System` variables;
         i.e. all variables in input and output ports including inwards and outwards of this system and
         all its children.
@@ -1453,41 +1477,48 @@
         )
         return self.assembled_problem()
 
     def add_child(self,
         child: AnySystem,
         execution_index: Optional[int] = None,
         pulling: Optional[Union[str, List[str], Dict[str, str]]] = None,
+        desc: str = "",
     ) -> AnySystem:
         """Add a child `System` to the current `System`.
 
         When adding a child `System`, it is possible to specified its position in the execution
         order.
 
-        Child `Port`, `inwards` and `outwards` can also be pulled at the parent level by providing either
-        the name of the port/inward/outward or a list of them or the name mapping of the child element
+        Child ports or individual `inwards` and `outwards` can also be pulled at the parent level by providing
+        either the name of the port/inward/outward or a list of them or the name mapping of the child element
         (dictionary keys) to the parent element (dictionary values).
         If the argument is not a dictionary, the name in the parent system will be the same as in
         the child.
 
         Parameters
         ----------
-        child: System
+        - child [System]:
             `System` to add to the current `System`
-        execution_index: int, optional
+        execution_index [int, optional]:
             Index of the execution order list at which the `System` should be inserted;
             default latest.
-        pulling: str or List[str] or Dict[str, str], optional
+        - pulling [str or list[str] or dict[str, str], optional]:
             Map of child ports to pulled ports at the parent system level; default None (no pulling)
+        - desc [str, optional]:
+            Sub-system description in the context of its parent.
+
+        Returns
+        -------
+        `child`
         """
         # Type validation
         check_arg(child, 'child', System)
         check_arg(pulling, 'pulling', (type(None), str, list, dict, set))
 
-        child = super().add_child(child, execution_index)
+        child = super().add_child(child, execution_index, desc)
 
         if child.name in self.name2variable:
             if isinstance(self[child.name], System):
                 logger.warning(
                     f"A subsystem named {child.name} already exists within system {self.name}."
                     f" Child system {child!r} will overwrite it."
                 )
@@ -1512,17 +1543,17 @@
         if pulling is not None:
             try:
                 pull_variables(child, pulling)
             except (ConnectorError, UnitError):
                 self.pop_child(child.name)
                 raise
 
-        # If child is added outside of `setup`, system must be declared as dirty
+        # If child is added outside of `setup`, we must force system tree inspection
         # to ensure input propagation during the next system execution.
-        self.set_dirty(PortType.IN)
+        self.touch()
 
         return child
 
     def pop_child(self, name: str) -> System:
         """Remove the subsystem called `name`.
 
         Parameters
@@ -2077,15 +2108,16 @@
         if not skip_driver:
             for driver in self.drivers.values():
                 driver.call_clean_run()
 
     def _postcompute(self) -> None:
         """Actions performed after the `System.compute` call."""
         if self.is_clean(PortType.IN):
-            self.set_clean(PortType.OUT)
+            if self._is_tree_clean:
+                self.set_clean(PortType.OUT)
         else:
             self.set_clean(PortType.IN)
             self.set_dirty(PortType.OUT)
 
             # Evaluate the residues
             for residue in self.residues.values():
                 residue.update()
@@ -2142,46 +2174,52 @@
                 logger.debug("Start setup_run recursive calls.")
                 self.call_setup_run(skip_driver=True)
 
             with self.log_context(" - run_once"):
                 if self.is_active():
                     self._precompute()
 
-                    if not self.is_clean(PortType.IN):
+                    dirty_inputs = not self.is_clean(PortType.IN)
+
+                    if dirty_inputs:
                         logger.debug(f"Call {self.name}.compute_before")
                         with self.__context_lock:
                             self.compute_before()
                     else:
                         logger.debug(f"Skip {self.name}.compute_before - Clean inputs")
 
-                    if not self.is_clean():
+                    dirty_tree = not self._is_tree_clean
+                    any_dirty_child = False
+
+                    if dirty_inputs or dirty_tree:
                         for child in self.children.values():
                             # Update connectors
                             for connector in self.__child_connectors.get(child.name, []):
                                 connector.transfer()
-                            # Execute the child
+                            # Execute sub-system
                             logger.debug(f"Call {self.name}.{child.name}.run_once()")
                             child.run_once()
+                            any_dirty_child |= not child.is_clean()
 
                         # Pull values from subsystems
                         for connector in self.__pulling_connectors:
                             connector.transfer()
-                    else:
-                        logger.debug(f"Skip {self.name} children execution - Clean interfaces")
 
-                    if not self.is_clean(PortType.IN):
+                    if dirty_inputs or any_dirty_child:
                         logger.debug(f"Call {self.name}.compute")
                         self._compute_calls += 1
                         with self.__context_lock:
                             self.__runner.compute()
                     else:
                         logger.debug(f"Skip {self.name}.compute - Clean inputs")
 
+                    self._is_tree_clean = not any_dirty_child
                     self._postcompute()
                     self.computed.emit()
+
                 else:
                     logger.debug(f"Skip {self.name} execution - Inactive")
 
             if is_master:
                 logger.debug("Start clean_run recursive calls.")
                 self.call_clean_run(skip_driver=True)
 
@@ -2193,21 +2231,22 @@
         """
         with System.set_master(repr(self), type_checking=False) as is_master:
             if is_master:
                 self.open_loops()
                 logger.debug("Start setup_run recursive calls.")
                 self.call_setup_run()
 
-            if self.drivers and self.any_active_driver():
+            if self.any_active_driver():
                 if self.is_standalone():  # System not standalone can't set the mathematical problem
                     logger.debug(f"Exec order for {self.name}: {list(self.exec_order)}")
 
                 for driver in self.drivers.values():
                     logger.debug(f"Call driver {driver.name}.run_once on {self.name}")
                     driver.run_once()
+
             else:
                 self.run_children_drivers()
 
             if is_master:
                 logger.debug("Start clean_run recursive calls.")
                 self.call_clean_run()
                 self.close_loops()
@@ -2220,45 +2259,51 @@
                 logger.debug("Start setup_run recursive calls.")
                 self.call_setup_run()
 
             with self.log_context(" - run_children_drivers"):
                 if self.is_active():
                     self._precompute()
 
-                    if not self.is_clean(PortType.IN):
+                    dirty_inputs = not self.is_clean(PortType.IN)
+
+                    if dirty_inputs:
                         logger.debug(f"Call {self.name}.compute_before")
                         with self.__context_lock:
                             self.compute_before()
                     else:
                         logger.debug(f"Skip {self.name}.compute_before - Clean inputs")
 
-                    if not self.is_clean():
-                        sys_connectors = self.__child_connectors
+                    dirty_tree = not self._is_tree_clean
+                    any_dirty_child = False
+
+                    if dirty_inputs or dirty_tree:
                         for child in self.children.values():
                             # Update connectors
-                            for connector in sys_connectors.get(child.name, []):
+                            for connector in self.__child_connectors.get(child.name, []):
                                 connector.transfer()
-                            # Execute the child
+                            # Execute sub-system
+                            logger.debug(f"Call {self.name}.{child.name}.run_once()")
                             child.run_drivers()
+                            any_dirty_child |= not child.is_clean()
 
                         # Pull values from subsystems
                         for connector in self.__pulling_connectors:
                             connector.transfer()
-                    else:
-                        logger.debug(f"Skip {self.name} children execution - Clean interfaces")
-
-                    if not self.is_clean(PortType.IN):
+                    
+                    if dirty_inputs or any_dirty_child:
                         self._compute_calls += 1
                         with self.__context_lock:
                             self.__runner.compute()
                     else:
                         logger.debug(f"Skip {self.name}.compute - Clean inputs")
 
+                    self._is_tree_clean = not any_dirty_child
                     self._postcompute()
                     self.computed.emit()
+
                 else:
                     logger.debug(f"Skip {self.name} execution - Inactive")
 
             if is_master:
                 logger.debug("Start clean_run recursive calls.")
                 self.call_clean_run()
 
@@ -3289,15 +3334,17 @@
             self._active = True
             self.__runner = self._meta
         
         else:
             self._set_recursive_active_status(True)
             self.__runner = self
 
-        self.set_dirty(PortType.IN)
+        self.touch()
+        for port in self.inputs.values():
+            port.touch()
 
     @property
     def has_surrogate(self) -> bool:
         """bool: True if system has a surrogate model (even if inactive), False otherwise."""
         return self._meta is not None
 
     def _set_recursive_active_status(self, active_status: bool) -> None:
```

### Comparing `cosapp-0.13.1/cosapp/systems/system.schema.json` & `cosapp-0.14.0/cosapp/systems/system.schema.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/systems/systemConnector.py` & `cosapp-0.14.0/cosapp/systems/systemConnector.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 class SystemConnector(Proxy):
     """Connector proxy used in `System`
     """
     def __init__(self, connector: BaseConnector):
         self.check(connector)
         super().__init__(connector)
         self.__noise: Dict[str, Any] = {}
+        self.source.touch()
         self.activate()
 
     @staticmethod
     def check(wrappee: Any) -> None:
         """Checks whether `wrappee` can be wrapped in a `SystemConnector`
         proxy; raises an exception if not.
 
@@ -67,32 +68,27 @@
             Perturbation value
         """
         if name not in self.sink_variables():
             raise ValueError(
                 "Perturbations can only be added on sink variables"
             )
         self.__noise[name] = value
-        self.source.owner.set_dirty(PortType.IN)
+        self.sink.owner.touch()
 
     def clear_noise(self) -> None:
         self.__noise.clear()
 
-    def __add_noise(self) -> None:
-        if self.__noise:
-            sink: BasePort = self.sink
-            for var, perturbation in self.__noise.items():
-                sink[var] += perturbation
-            sink.touch()
-
     def __repr__(self):
         return repr(self.__wrapped__)
     
     def transfer(self) -> None:
         """Transfer values from `source` to `sink`."""
         if self.__is_active:
             sink: BasePort = self.sink
             source: BasePort = self.source
+            noise = self.__noise
 
-            if not source.owner.is_clean(source.direction):
+            if not source.is_clean or noise:
                 sink.touch()
                 self.__wrapped__.transfer()
-            self.__add_noise()
+                for varname, perturbation in noise.items():
+                    sink[varname] += perturbation
```

### Comparing `cosapp-0.13.1/cosapp/systems/systemSurrogate.py` & `cosapp-0.14.0/cosapp/systems/systemSurrogate.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/systems/systemfamily.py` & `cosapp-0.14.0/cosapp/systems/systemfamily.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/__init__.py` & `cosapp-0.14.0/cosapp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/fmu/exporter.py` & `cosapp-0.14.0/cosapp/tools/fmu/exporter.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/fmu/logging.py` & `cosapp-0.14.0/cosapp/tools/fmu/logging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/fmu/tests/test_exporter.py` & `cosapp-0.14.0/cosapp/tools/fmu/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/fmu/tests/test_logging.py` & `cosapp-0.14.0/cosapp/tools/fmu/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/help.py` & `cosapp-0.14.0/cosapp/tools/help.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/module_parser/parseModule.py` & `cosapp-0.14.0/cosapp/tools/module_parser/parseModule.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                     if fnmatchcase(name, pattern):
                         include = False
                         break
         return include
     
     def issubclass_strict(obj: type, base: type) -> bool:
         """Strict version of `issubclass`, returning `False` for base class."""
-        return obj is not base and issubclass(obj, base)
+        return issubclass(obj, base) and obj is not base
     
     modules = extract_modules(module)
     systemSet, portSet = set(), set()
     for mod in modules:
         for _, obj in getmembers(mod):
             if isclass(obj) and is_included(obj.__name__):
                 if issubclass_strict(obj, System):
@@ -104,15 +104,15 @@
                     portSet.add(obj)
     return systemSet, portSet
 
 
 def get_data_from_class(
     dtype: Union[Type[System],Type[Port]],
     package_name: Optional[str] = None,
-    ports: Optional[Set[Port]] = None,
+    ports: Optional[Set[Type[Port]]] = None,
     *args,
     **kwargs
 ):
     """Get informations from a system or a port
 
     Parameters:
     -----------
@@ -126,23 +126,32 @@
     - *args, **kwargs:
         Additional arguments forwarded to class constructor, if required.
 
     Returns:
     --------
     dict[str, Any]
     """
+    if ports is None:
+        def register_port(port: BasePort):
+            pass
+    else:
+        def register_port(port: BasePort):
+            if isinstance(port, Port):
+                ports.add(type(port))
+
     def get_all_port_data(portDict: Dict[str, BasePort]):
         portList = []
         for port in portDict.values():
             if len(port) > 0:
                 portList.append(get_port_data(port))
-                if ports is not None:
-                    ports.add(port.__class__)
+                register_port(port)
         return portList or None
 
+    sysPackage = package_name or dtype.__module__.split('.', maxsplit=1)[0]
+
     def get_port_data(port: BasePort, is_port_type=False):
         ptype = type(port)
         typename = ptype.__name__
         modname = ptype.__module__
         if is_port_type:
             portDict = {
                 'name': typename,
@@ -230,15 +239,14 @@
             mathProblemDict['nEquations'] = problem.n_equations
 
         return mathProblemDict
 
     if issubclass(dtype, System):
         systemType = dtype.__name__
         systemName = kwargs.pop('__alias__', systemType)
-        sysPackage = package_name or dtype.__module__.split('.', maxsplit=1)[0]
         system = dtype('bogus', *args, **kwargs)
         desc = get_system_doc(dtype)
         inputs = get_all_port_data(system.inputs)
         outputs = get_all_port_data(system.outputs)
         mathProblemDict = get_math_problem(system)
         dtypeDict = {
             'name': systemName,
@@ -319,61 +327,65 @@
     metadata = {
         'name': package_name,
         'systems': get_all_class_data(systemSet, ctor_config, ports=portSet),
     }
     # Add port metadata *after* system metadata
     metadata['ports'] = get_all_class_data(portSet, ctor_config)
 
-    with open(
-        os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), "packageData.schema.json"
-        )
-    ) as fp:
-        config_schema = json.load(fp)
-
     try:
         metadata['version'] = module.__version__
     except AttributeError:
         pass
 
+    pwd = os.path.dirname(os.path.abspath(__file__))
+    with open(os.path.join(pwd, "package_metadata.schema.json")) as fp:
+        config_schema = json.load(fp)
+
     jsonschema.validate(metadata, config_schema)
 
     return metadata
 
 
 def parse_module(
     module: ModuleType,
-    ctor_config: SystemConfig = {},
+    ctor_config: Optional[SystemConfig] = None,
     package_name: Optional[str] = None,
-    includes: SearchPattern = '*',
-    excludes: SearchPattern = None,
+    includes: Optional[SearchPattern] = None,
+    excludes: Optional[SearchPattern] = None,
     path: Optional[Union[str, Path]] = None,
 ) -> None:
     """Creates a json file containing the metadata
     of all systems and ports found in `module`.
     
     Parameters:
     -----------
     - module [ModuleType]:
         Python module to be parsed.
     - ctor_config [dict[str, list[dict[str, any]] | dict[str, Any]]] (optional):
         Dictionary or list of dictionaries containing kwargs required for system/port
         construction (if any), referenced by class names (keys).
         If the dictionary contains key '__alias__', the class will be
         renamed into the associated value.
-    - packageName [str] (optional):
+    - package_name [str] (optional):
         Custom package name.
     - includes [str or List[str]] (optional):
         System and port names matching these patterns will be included.
     - excludes [str or List[str]] (optional):
         System and port names matching these patterns will be excluded
         (ports used by included systems will always be included).
     - path [str | pathlib.Path] (optional):
         Optional path of output file <packageName or module.__name__>.json
         (current directory by default).
+
+    Use pre-defined settings
+    ------------------------
+    Pre-defined values of optional arguments `ctor_config`, `package_name`, `includes` and `excludes`
+    may be specified at module level by implementing hook function `_parse_module_config`,
+    returning preset values in a dictionary of the kind {option: value}.
+    Typically, `_parse_module_config` may be defined in the `__init__.py` file of the module.
     
     Examples:
     ---------
     >>> parse_module(module1)
     >>>
     >>> parse_module(
     >>>     module2,
@@ -382,24 +394,41 @@
     >>>         'SystemB': [
     >>>             dict(foo=0),
     >>>             dict(foo=None, __alias__='SystemB [default]'),
     >>>         ],
     >>>     },
     >>> )
     """
-    if package_name is None:
-        package_name = module.__name__
-    
-    metadata = get_data_from_module(
-        module,
+    settings = dict(
         ctor_config=ctor_config,
         package_name=package_name,
         includes=includes,
         excludes=excludes,
     )
+    default_settings = dict(
+        ctor_config={},
+        includes='*',
+        excludes=None,
+        package_name=module.__name__,
+    )
+    try:
+        # Check if module has a pre-defined settings
+        get_module_settings = getattr(module, "_parse_module_config")
+    except AttributeError:
+        pass
+    else:
+        logger.info("Use pre-defined settings returned by `_parse_module_config`")
+        default_settings.update(get_module_settings())
+
+    # Apply user settings, if specified
+    for name, value in settings.items():
+        if value is None:
+            settings[name] = default_settings[name]
+
+    metadata = get_data_from_module(module, **settings)
 
     try:
         version = metadata['version']
     except KeyError:
         filename = f"{package_name}.json"
     else:
         filename = f"{package_name} - {version}.json"
```

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/problem_viewer.py` & `cosapp-0.14.0/cosapp/tools/problem_viewer/problem_viewer.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/tests/test_viewmodeldata.py` & `cosapp-0.14.0/cosapp/tools/problem_viewer/tests/test_viewmodeldata.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/index.html` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/index.html`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/libs/awesomplete.js` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/libs/awesomplete.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/libs/d3.v4.min.js` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/libs/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/libs/http.js` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/libs/http.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/libs/jquery-3.2.1.min.js` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/libs/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/libs/vkBeautify.js` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/libs/vkBeautify.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/constants.js` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/constants.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/draw.js` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/draw.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/legend.js` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/legend.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/modal.js` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/modal.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/ptN2.js` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/ptN2.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/search.js` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/search.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/src/svg.js` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/src/svg.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/style/awesomplete.css` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/style/awesomplete.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/style/fontello.woff` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/style/fontello.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/problem_viewer/visualization/style/partition_tree.css` & `cosapp-0.14.0/cosapp/tools/problem_viewer/visualization/style/partition_tree.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/templates/lib/d3.min.js` & `cosapp-0.14.0/cosapp/tools/templates/lib/d3.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/templates/lib/vis.min.css` & `cosapp-0.14.0/cosapp/tools/templates/lib/vis.min.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/templates/lib/vis.min.js` & `cosapp-0.14.0/cosapp/tools/templates/lib/vis.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/templates/pythonfmu.j2` & `cosapp-0.14.0/cosapp/tools/templates/pythonfmu.j2`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/templates/src/d3_draw.js` & `cosapp-0.14.0/cosapp/tools/templates/src/d3_draw.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/templates/system_repr.html` & `cosapp-0.14.0/cosapp/tools/templates/system_repr.html`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/trigger.py` & `cosapp-0.14.0/cosapp/tools/trigger.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/views/baseRenderer.py` & `cosapp-0.14.0/cosapp/tools/views/baseRenderer.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/views/d3js.py` & `cosapp-0.14.0/cosapp/tools/views/d3js.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/views/markdown.py` & `cosapp-0.14.0/cosapp/tools/views/markdown.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,16 +21,19 @@
         Returns
         -------
         List[str]
             List of Markdown strings representing port variables as a table, with header.
         """
         port = self.port
         name = port.full_name() if contextual else port.name
+        info = type(port).__name__
+        if (desc := port.description):
+            info += f", {desc}"
         doc = []
-        doc.extend([f"`{name}`: {type(port).__name__}"])
+        doc.append(f"`{name}`: {info}")
         doc.extend(self.var_repr())
         return doc
 
     def var_repr(self) -> List[str]:
         """Returns the representation of port variables in Markdown format,
         as a list of strings (same as `content`, without name header).
 
@@ -112,36 +115,40 @@
 
     Returns
     -------
     str
         Markdown formatted representation
     """
     doc = list()
-    if len(system.tags) > 0:
+    if system.tags:
         doc.extend(["", f"**Tags**: {list(system.tags)!s}", ""])
 
-    if len(system.children) > 0:
+    def get_child_doc(s: System) -> str:
+        info = type(s).__name__
+        if (desc := s.description):
+            info += f", {desc}"
+        return f"- `{s.name}`: {info}"
+
+    if system.children:
         doc.extend(["", "### Child components", ""])
-        doc.extend(
-            f"- `{name}`: {type(child).__name__}"
-            for name, child in system.children.items()
-        )
+        doc.extend(map(get_child_doc, system.children.values()))
 
     def dump_port_data(header, port_dict):
-        if all(len(port) == 0 for port in port_dict.values()):
-            return
-        doc.extend(["", f"### {header.title()}", ""])
+        port_docs = []
         for port in port_dict.values():
             if len(port) > 0:
                 formatter = PortMarkdownFormatter(port)
                 port_doc = formatter.content(contextual=False)
                 port_doc[0] = f"- {port_doc[0]}"
-                doc.extend(port_doc)
+                port_docs.extend(port_doc)
+        if port_docs:
+            doc.extend(["", f"### {header.title()}", ""])
+            doc.extend(port_docs)
 
     dump_port_data("inputs", system.inputs)
     dump_port_data("outputs", system.outputs)
 
-    if hasattr(system, "residues") and len(system.residues) > 0:
+    if system.residues:
         doc.extend(["", "### Residues", ""])
         doc.append(", ".join(f"`{key}`" for key in system.residues))
 
     return "\n".join(doc)
```

### Comparing `cosapp-0.13.1/cosapp/tools/views/prettyprint.py` & `cosapp-0.14.0/cosapp/tools/views/prettyprint.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/views/tests/test_VisJsRenderer.py` & `cosapp-0.14.0/cosapp/tools/views/tests/test_VisJsRenderer.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/views/tests/test_d3.py` & `cosapp-0.14.0/cosapp/tools/views/tests/test_d3.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/views/tests/test_markdown.py` & `cosapp-0.14.0/cosapp/tools/views/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/views/tests/test_prettyprint.py` & `cosapp-0.14.0/cosapp/tools/views/tests/test_prettyprint.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tools/views/visjs.py` & `cosapp-0.14.0/cosapp/tools/views/visjs.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/00-Introduction.ipynb` & `cosapp-0.14.0/cosapp/tutorials/00-Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/01-Systems.ipynb` & `cosapp-0.14.0/cosapp/tutorials/01-Systems.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978052524927525%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(19, "s = Multiply(name=\'s\')")], delete: [19]}}, 9: '*

 * *            "{'source': {insert: [(19, '- **unit**: Physical unit of the variable, given by a "*

 * *            'string. **CoSApp** will take care of unit conversion between connected systems. '*

 * *            'However, *units are not enforced* inside a `System`. Therefore, module developers '*

 * *            "must ensure that all variables are consistently converted in method `compute`.\\n'), "*

 * *            "(20, '- **desc* […]*

```diff
@@ -67,15 +67,15 @@
                 "        self.add_inward('K1', 1.0)\n",
                 "        self.add_outward('delta_x', 0.0)\n",
                 "\n",
                 "    def compute(self): # `compute` method defines what the system does\n",
                 "        self.p_out.x = self.p_in.x * self.K1\n",
                 "        self.delta_x = self.p_out.x - self.p_in.x\n",
                 "\n",
-                "s = Multiply(name='mult')"
+                "s = Multiply(name='s')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "![Multiple systems](images/systems_1.svg)"
@@ -98,14 +98,15 @@
                 "s.K1 = 5.\n",
                 "s.run_once()\n",
                 "\n",
                 "s.p_out"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "More information on ports (`inputs` *and* `outputs`) can be found in a dedicated [Port tutorial](02-Ports.ipynb).\n",
                 "\n",
                 "#### `inwards` and `outwards` ports\n",
                 "\n",
@@ -120,61 +121,68 @@
                 "- An *inward* is an input parameter needed by the system to compute its output. For example, the pressure losses coefficient of a duct is an inward, used to compute the output flow port from its input flow port.\n",
                 "- An *outward* is an output variable deduced from inputs, such as an intermediate variable of a computation, which is exposed to other systems. For instance, the difference between the input and output pressures in a duct system is a local variable, which may be of interest to neighbouring systems. Another example is the table object read from a filename (the filename being usually an *inward*). \n",
                 "\n",
                 "An inward `x` (resp. outward) defined in system `s` can be accessed as either `s.x` or `s.inwards.x` (resp. `s.outwards.x`).\n",
                 "\n",
                 "All variables in **CoSApp** accept additional information:\n",
                 "\n",
-                "- *unit*: Physical unit of the variable, given by a string. **CoSApp** will take care of unit conversion between connected systems. However, *units are not enforced* inside a `System`. Therefore, module developers must ensure that all variables are consistently converted in method `compute`.\n",
-                "- *desc*: Short description of the variable.\n",
-                "- *dtype*: If you need to force certain data type(s) on a variable, a tuple of acceptable types can be provided through this keyword. If that information is not supplied, dtype is inferred from the variable value; *e.g.* a number (`int` or `float`) will be typed as `Number`."
+                "- **unit**: Physical unit of the variable, given by a string. **CoSApp** will take care of unit conversion between connected systems. However, *units are not enforced* inside a `System`. Therefore, module developers must ensure that all variables are consistently converted in method `compute`.\n",
+                "- **desc**: Short description of the variable.\n",
+                "- **dtype**: If you need to force certain data type(s) on a variable, a tuple of acceptable types can be provided through this keyword. If that information is not supplied, dtype is inferred from the variable value; *e.g.* a number (`int` or `float`) will be typed as `Number`.\n",
+                "\n",
+                "Methods `add_input` and `add_output` also accept optional argument `desc`, if a contextual description is desired."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "class MultiplyAdvanced(System):\n",
                 "\n",
                 "    def setup(self):\n",
-                "        self.add_input(DemoPort, 'p_in')\n",
-                "        # Inward and outward variables accept optional dtype and unit\n",
+                "        # Inwput and output ports accept optional description `desc`\n",
+                "        self.add_input(DemoPort, 'p_in', desc='Port containing values to be multiplied')\n",
+                "        # Inward and outward variables accept optional `dtype` and `unit`\n",
                 "        self.add_inward('K1', 1, dtype=int, desc='Multiplication coefficient')\n",
                 "        self.add_outward('delta_x',\n",
                 "            value = 0.0,\n",
                 "            unit = 'Pa',\n",
                 "            dtype = (int, float), \n",
                 "            desc = \"Difference between `DemoPort` output and input\"\n",
                 "        )\n",
                 "        self.add_output(DemoPort, 'p_out')\n",
                 "\n",
                 "    def compute(self):\n",
                 "        self.p_out.x = self.p_in.x * self.K1\n",
                 "        self.delta_x = self.p_out.x - self.p_in.x\n",
                 "\n",
-                "advanced = MultiplyAdvanced(name='mult')\n",
+                "\n",
+                "advanced = MultiplyAdvanced('advanced')\n",
                 "\n",
                 "print(\n",
-                "    f\"Inwards: \\n  {advanced.inwards}\",\n",
-                "    f\"Outwards:\\n  {advanced.outwards}\",\n",
+                "    f\"{advanced.inwards  = }\",\n",
+                "    f\"{advanced.outwards = }\",\n",
                 "    sep=\"\\n\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Composite Systems\n",
                 "\n",
                 "Composite systems contain sub-systems, referred to as `children`.\n",
                 "\n",
                 "Sub-systems are added to a composite system using method `add_child`.\n",
+                "Like ports and variables, sub-systems can be briefly described in the context of their parent system, with optional argument `desc`.\n",
+                "\n",
                 "Connections between child systems are declared at parent level, with method `connect`.\n",
                 "The typical syntax is `parent.connect(child1.portA, child2.portB)`.\n",
                 "\n",
                 "`Port` connections are described in detail in the [Port tutorial](02-Ports.ipynb)."
             ]
         },
         {
@@ -182,22 +190,22 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "class MultiplyComplexSystem(System):\n",
                 "\n",
                 "    def setup(self):\n",
-                "        # Children\n",
-                "        self.add_child(Multiply('mult1'))  # add a sub-system\n",
+                "        # Sub-systems\n",
+                "        self.add_child(Multiply('mult1'), desc='Primary sub-system')\n",
                 "        self.add_child(Multiply('mult2'))\n",
                 "        \n",
                 "        # Connectors\n",
                 "        self.connect(self.mult1.p_out, self.mult2.p_in)  # connect ports of sub-systems\n",
                 "\n",
-                "head = MultiplyComplexSystem(name='head')"
+                "head = MultiplyComplexSystem('head')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "![Connection between Systems](images/systems_2.svg)"
```

### Comparing `cosapp-0.13.1/cosapp/tutorials/02-Ports.ipynb` & `cosapp-0.14.0/cosapp/tutorials/02-Ports.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990301724137931%*

 * *Differences: {"'cells'": '{17: {\'source\': {insert: [(18, \'print(\\n\'), (19, \'    f"{h.monitor.a = '*

 * *            '}",\\n\'), (20, \'    f"{h.demo1.p_out = }",\\n\'), (21, \')\')], delete: [19, 18]}}, '*

 * *            '19: {\'source\': [\'print(f"{h.demo2.p_in = }")\']}, 20: {\'source\': '*

 * *            '[\'print(f"{h.monitor.outwards = }")\']}}'}*

```diff
@@ -247,16 +247,18 @@
                 "h.add_child(MonitorSystem('monitor'))\n",
                 "# Connect `h.monitor.a` to `h.demo1.p_out.a`\n",
                 "h.connect(h.monitor.inwards, h.demo1.p_out, 'a')\n",
                 "\n",
                 "h.demo1.p_in.set_values(a=50., b=0., c=25.)\n",
                 "h.run_once()\n",
                 "\n",
-                "print(f\"{h.monitor.a = }\")\n",
-                "h.demo1.p_out"
+                "print(\n",
+                "    f\"{h.monitor.a = }\",\n",
+                "    f\"{h.demo1.p_out = }\",\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In the example above, variable `a` from port `inwards` has been connected to variable `a` from port `demo1.p_out`.\n",
@@ -284,24 +286,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "h.demo2.p_in"
+                "print(f\"{h.demo2.p_in = }\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "h.monitor.outwards"
+                "print(f\"{h.monitor.outwards = }\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Example with unit conversions"
```

### Comparing `cosapp-0.13.1/cosapp/tutorials/03-Drivers.ipynb` & `cosapp-0.14.0/cosapp/tutorials/03-Drivers.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/04-Triggers.ipynb` & `cosapp-0.14.0/cosapp/tutorials/04-Triggers.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/05-Validation.ipynb` & `cosapp-0.14.0/cosapp/tutorials/05-Validation.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/06-Visibility.ipynb` & `cosapp-0.14.0/cosapp/tutorials/06-Visibility.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/07-Metamodels.ipynb` & `cosapp-0.14.0/cosapp/tutorials/07-Metamodels.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/08-Multipoints-Design.ipynb` & `cosapp-0.14.0/cosapp/tutorials/08-Multipoints-Design.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/09-MonteCarlo.ipynb` & `cosapp-0.14.0/cosapp/tutorials/09-MonteCarlo.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/10-Recorders.ipynb` & `cosapp-0.14.0/cosapp/tutorials/10-Recorders.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/11-DesignMethods.ipynb` & `cosapp-0.14.0/cosapp/tutorials/11-DesignMethods.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/CustomConnectors.ipynb` & `cosapp-0.14.0/cosapp/tutorials/CustomConnectors.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/FMI.ipynb` & `cosapp-0.14.0/cosapp/tutorials/FMI.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/Guidelines.ipynb` & `cosapp-0.14.0/cosapp/tutorials/Guidelines.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/HybridSimulations.ipynb` & `cosapp-0.14.0/cosapp/tutorials/HybridSimulations.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/Logging.ipynb` & `cosapp-0.14.0/cosapp/tutorials/Logging.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/Optimization.ipynb` & `cosapp-0.14.0/cosapp/tutorials/Optimization.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/SystemSurrogates.ipynb` & `cosapp-0.14.0/cosapp/tutorials/SystemSurrogates.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/SystemSurrogatesAdvanced.ipynb` & `cosapp-0.14.0/cosapp/tutorials/SystemSurrogatesAdvanced.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/Targets.ipynb` & `cosapp-0.14.0/cosapp/tutorials/Targets.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/TimeDriver.ipynb` & `cosapp-0.14.0/cosapp/tutorials/TimeDriver.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/TimeDriverAdvanced.ipynb` & `cosapp-0.14.0/cosapp/tutorials/TimeDriverAdvanced.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/TipsAndTricks.ipynb` & `cosapp-0.14.0/cosapp/tutorials/TipsAndTricks.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/Visitors.ipynb` & `cosapp-0.14.0/cosapp/tutorials/Visitors.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/aa-SimpleCircuit.ipynb` & `cosapp-0.14.0/cosapp/tutorials/aa-SimpleCircuit.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/exprampode_fmu.py` & `cosapp-0.14.0/cosapp/tutorials/exprampode_fmu.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/cosapp.svg` & `cosapp-0.14.0/cosapp/tutorials/images/cosapp.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/design_circuit.svg` & `cosapp-0.14.0/cosapp/tutorials/images/design_circuit.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/drivers_1.svg` & `cosapp-0.14.0/cosapp/tutorials/images/drivers_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/drivers_2.svg` & `cosapp-0.14.0/cosapp/tutorials/images/drivers_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/drivers_3.svg` & `cosapp-0.14.0/cosapp/tutorials/images/drivers_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/drivers_4.svg` & `cosapp-0.14.0/cosapp/tutorials/images/drivers_4.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/drivers_5.svg` & `cosapp-0.14.0/cosapp/tutorials/images/drivers_5.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/drivers_nonlinear.svg` & `cosapp-0.14.0/cosapp/tutorials/images/drivers_nonlinear.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/experimental.svg` & `cosapp-0.14.0/cosapp/tutorials/images/experimental.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/in_progress.svg` & `cosapp-0.14.0/cosapp/tutorials/images/in_progress.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/ports_1.svg` & `cosapp-0.14.0/cosapp/tutorials/images/ports_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/ports_2.svg` & `cosapp-0.14.0/cosapp/tutorials/images/ports_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/ports_3.svg` & `cosapp-0.14.0/cosapp/tutorials/images/ports_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/simple_circuit.svg` & `cosapp-0.14.0/cosapp/tutorials/images/simple_circuit.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/systems_1.svg` & `cosapp-0.14.0/cosapp/tutorials/images/systems_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/systems_2.svg` & `cosapp-0.14.0/cosapp/tutorials/images/systems_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/systems_3.svg` & `cosapp-0.14.0/cosapp/tutorials/images/systems_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/systems_4.svg` & `cosapp-0.14.0/cosapp/tutorials/images/systems_4.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/systems_5.svg` & `cosapp-0.14.0/cosapp/tutorials/images/systems_5.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/tanks.svg` & `cosapp-0.14.0/cosapp/tutorials/images/tanks.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/triggers_1.svg` & `cosapp-0.14.0/cosapp/tutorials/images/triggers_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/triggers_2.svg` & `cosapp-0.14.0/cosapp/tutorials/images/triggers_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/validity.svg` & `cosapp-0.14.0/cosapp/tutorials/images/validity.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/images/visibility.svg` & `cosapp-0.14.0/cosapp/tutorials/images/visibility.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/multimode/BouncingBall.ipynb` & `cosapp-0.14.0/cosapp/tutorials/multimode/BouncingBall.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/multimode/MultimodeOde.ipynb` & `cosapp-0.14.0/cosapp/tutorials/multimode/MultimodeOde.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/multimode/NewtonPendulum.ipynb` & `cosapp-0.14.0/cosapp/tutorials/multimode/NewtonPendulum.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/optimization/BetzLimit.ipynb` & `cosapp-0.14.0/cosapp/tutorials/optimization/BetzLimit.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/optimization/Sellar.ipynb` & `cosapp-0.14.0/cosapp/tutorials/optimization/Sellar.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/quickstart.ipynb` & `cosapp-0.14.0/cosapp/tutorials/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/tutorials/time_solutions.py` & `cosapp-0.14.0/cosapp/tutorials/time_solutions.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/distributions/distribution.py` & `cosapp-0.14.0/cosapp/utils/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/distributions/normal.py` & `cosapp-0.14.0/cosapp/utils/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/distributions/tests/test_distribution.py` & `cosapp-0.14.0/cosapp/utils/distributions/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/distributions/tests/test_normal.py` & `cosapp-0.14.0/cosapp/utils/distributions/tests/test_normal.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/distributions/tests/test_triangular.py` & `cosapp-0.14.0/cosapp/utils/distributions/tests/test_triangular.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/distributions/tests/test_uniform.py` & `cosapp-0.14.0/cosapp/utils/distributions/tests/test_uniform.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/distributions/triangular.py` & `cosapp-0.14.0/cosapp/utils/distributions/triangular.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/distributions/uniform.py` & `cosapp-0.14.0/cosapp/utils/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/find_variables.py` & `cosapp-0.14.0/cosapp/utils/find_variables.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/graph_analysis.py` & `cosapp-0.14.0/cosapp/utils/graph_analysis.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/helpers.py` & `cosapp-0.14.0/cosapp/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/json.py` & `cosapp-0.14.0/cosapp/utils/json.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/logging.py` & `cosapp-0.14.0/cosapp/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/naming.py` & `cosapp-0.14.0/cosapp/utils/naming.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/options_dictionary.py` & `cosapp-0.14.0/cosapp/utils/options_dictionary.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/parsing.py` & `cosapp-0.14.0/cosapp/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/pull_variables.py` & `cosapp-0.14.0/cosapp/utils/pull_variables.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/state_io.py` & `cosapp-0.14.0/cosapp/utils/state_io.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/__init__.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/base.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/base.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/kriging.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/kriging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/multifi_cokriging.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/multifi_cokriging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/nearest_neighbor.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/nn_interpolators/linear_interpolator.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/nn_interpolators/linear_interpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/nn_interpolators/nn_base.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/nn_interpolators/nn_base.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/nn_interpolators/rbf_interpolator.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/nn_interpolators/rbf_interpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/nn_interpolators/weighted_interpolator.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/nn_interpolators/weighted_interpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/response_surface.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/response_surface.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/tests/test_kriging.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/tests/test_kriging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/tests/test_multifi_cokriging.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/tests/test_multifi_cokriging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/tests/test_nearest_neighbor.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/tests/test_nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/surrogate_models/tests/test_response_surface.py` & `cosapp-0.14.0/cosapp/utils/surrogate_models/tests/test_response_surface.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp/utils/testing.py` & `cosapp-0.14.0/cosapp/utils/testing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Utility functions for testing purposes"""
 import numpy
+import pytest
 import inspect
 import warnings
 import itertools
 from numbers import Number
 from contextlib import contextmanager
 from typing import Tuple, Dict, Any, Union, Iterable, Type, Optional
 from cosapp.base import System
@@ -55,14 +56,35 @@
         iterator,
         dtype=float,
         count=actual.size,
     )
     return errors.reshape(actual.shape)
 
 
+def assert_close_dict(actual: dict, expected: dict, abs=None, rel=None) -> None:
+    """Assert that `actual` and `expected` dictionaries are identical, within given tolerance bounds.
+    Works recursively with nested dictionaries.
+    """
+    def assert_close(actual: dict, expected: dict, context=""):
+        """Recursive test function, with contextual message"""
+        assert set(actual) == set(expected), context
+        for key, value in expected.items():
+            local_context = f"{context}[{key!r}]"
+            if isinstance(value, dict):
+                assert_close(actual[key], value, context=local_context)
+            else:
+                try:
+                    expected_value = pytest.approx(value, abs=abs, rel=rel)
+                except TypeError:
+                    expected_value = value
+                assert actual[key] == expected_value, f"key {local_context}"
+
+    assert_close(actual, expected)
+
+
 def get_args(*args, **kwargs) -> ArgsKwargs:
     """Utility function to collect args and kwargs in a tuple"""
     return args, kwargs
 
 
 @contextmanager
 def no_exception():
```

### Comparing `cosapp-0.13.1/cosapp/utils/validate.py` & `cosapp-0.14.0/cosapp/utils/validate.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/cosapp.egg-info/PKG-INFO` & `cosapp-0.14.0/cosapp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosapp
-Version: 0.13.1
+Version: 0.14.0
 Summary: CoSApp, the Collaborative System Approach.
 Home-page: https://cosapp.readthedocs.io
 Author: CoSApp Development Team
 License: Apache-2.0
 Keywords: cosapp,system simulation,system design
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: extra
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.rst
 
 # CoSApp - Collaborative System Approach
@@ -55,14 +55,76 @@
 # Try it now!
 Run a Jupyter Lab instance with binder to try out CoSApp features through examples.
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/cosapp%2Fcosapp/master?urlpath=lab/tree/docs/tutorials)
 
 # History
 
+## 0.14.0 (2023-05-17)
+
+### New features & API changes
+
+* Improved performance, through a revised clean/dirty mechanism (MR [#215](https://gitlab.com/cosapp/cosapp/-/merge_requests/215)).
+* Possibility to add a contextual description to sub-systems and ports of a system, as well as sub-drivers (MR [#216](https://gitlab.com/cosapp/cosapp/-/merge_requests/216)). This feature is useful for automatic documentation tools, and has been included in the Markdown representation of systems (also used in function `cosapp.tools.display_doc`). Example:
+  
+  ```python
+  from cosapp.base import System
+  from my_module import FlowPort
+  
+  class MySystem(System):
+      def setup(self):
+          self.add_input(FlowPort, "fl_in1", desc="Primary inlet flow port")
+          self.add_input(FlowPort, "fl_in2", desc="Secondary inlet flow port")
+  
+          self.add_output(FlowPort, "fl_out")
+  ```
+  
+* New hook function `_parse_module_config`, returning pre-defined settings for `cosapp.tools.parse_module` (MR [#218](https://gitlab.com/cosapp/cosapp/-/merge_requests/218)). This allows module maintainers to simply call
+  
+  ```python
+  from cosapp.tools import parse_module
+  import my_module
+  
+  parse_module(my_module)
+  ```
+
+  instead of, *e.g.*,
+
+  ```python
+  parse_module(
+      my_module,
+      ctor_config={
+          "ComplexSystem1": [
+              dict(n=1, foo=0.5),
+              dict(n=2, foo=0.1),
+          ],
+          "ComplexSystem2": [
+              dict(xi=0.0, __alias__="ComplexSystem2_a"),
+              dict(xi=1.0, __alias__="ComplexSystem2_b"),
+          ],
+      },
+      excludes=["Foo*", "*Bar?"],
+  )
+  ```
+
+  provided `my_module._parse_module_config()` returns a dictionary specifying the values of `ctor_config`, `excludes`, *etc.*
+
+- Make `SolverResults` a `dataclass`, for easier handling of `NonLinearSolver.results`, *e.g.* (MR [#220](https://gitlab.com/cosapp/cosapp/-/merge_requests/220)).
+- Expose attribute `problem` in system setup (MR [#221](https://gitlab.com/cosapp/cosapp/-/merge_requests/221)). Previously, `problem` was only exposed in method `System.transition`.
+
+### Bug fixes and code quality
+
+* Fix bug in `NonLinearSolver` log message (MR [#214](https://gitlab.com/cosapp/cosapp/-/merge_requests/214)).
+* Add missing JSON file in PyPI and conda packages, preventing the use of `cosapp.tools.parse_module` (MR [#219](https://gitlab.com/cosapp/cosapp/-/merge_requests/219)).
+
+### Documentation
+
+* Illustrate port and sub-system description in tutorials (MR [#215](https://gitlab.com/cosapp/cosapp/-/merge_requests/215)).
+
+
 ## 0.13.1 (2023-04-03)
 
 ### Bug fixes and code quality
 
 * Update test baseline to pass in a Python 3.11 environment (MR [#200](https://gitlab.com/cosapp/cosapp/-/merge_requests/200)).
 * Creation of a dummy system factory, mostly for tests (MR [#201](https://gitlab.com/cosapp/cosapp/-/merge_requests/201)).
 * Improve clean/dirty mechanism (MR [#202](https://gitlab.com/cosapp/cosapp/-/merge_requests/202)) and fix incorrect clean/dirty status with surrogate models (MR [#205](https://gitlab.com/cosapp/cosapp/-/merge_requests/205)).
@@ -92,61 +154,61 @@
 
 * Module `connectors` moved from `cosapp.core` to `cosapp.ports` (MR [#189](https://gitlab.com/cosapp/cosapp/-/merge_requests/189)).
 * New "direct" (with no unit conversion) connector classes `PlainConnector`, `CopyConnector` and `DeepCopyConnector`, in `cosapp.ports.connectors` (MR [#188](https://gitlab.com/cosapp/cosapp/-/merge_requests/188)).
 * New method `MathematicalProblem.is_empty()`, equivalent to `shape == (0, 0)` (MR [#186](https://gitlab.com/cosapp/cosapp/-/merge_requests/186)).
 * Improved VisJs graph rendering, by limiting node size for long system names (MR [#184](https://gitlab.com/cosapp/cosapp/-/merge_requests/184)).
 * New utility functions `get_state` and `set_state` in `cosapp.utils`, for quick system data recovery (MR [#193](https://gitlab.com/cosapp/cosapp/-/merge_requests/193)):
 
-```python
-from cosapp.utils import get_state, set_state
-
-s = SomeSystem('s')
-# ... many design steps, say
-
-# Save state in local object
-designed = get_state(s)
-
-s.drivers.clear()
-s.add_driver(SomeDriver('driver'))
-
-try:
-    s.run_drivers()
-except:
-    # Recover previous state
-    set_state(s, designed)
-```
+  ```python
+  from cosapp.utils import get_state, set_state
+  
+  s = SomeSystem('s')
+  # ... many design steps, say
+  
+  # Save state in local object
+  designed = get_state(s)
+  
+  s.drivers.clear()
+  s.add_driver(SomeDriver('driver'))
+  
+  try:
+      s.run_drivers()
+  except:
+      # Recover previous state
+      set_state(s, designed)
+  ```
 
 * Functions `radians`, `degrees` and `arctan2`/`atan2` have been added to the scope of `EvalString` objects, and can therefore be used in equations, *e.g.* (MR [#178](https://gitlab.com/cosapp/cosapp/-/merge_requests/178)).
 * Recorders can now record constant properties (MR [#181](https://gitlab.com/cosapp/cosapp/-/merge_requests/181)).
 * Deprecation of `System.get_unsolved_problem` in favour of new method `assembled_problem` (MR [#174](https://gitlab.com/cosapp/cosapp/-/merge_requests/174)).
 * Inner off-design problem of systems is now exposed as attribute `problem`, but only within the `transition` method (MR [#174](https://gitlab.com/cosapp/cosapp/-/merge_requests/174)). This allows users to add or remove off-design constraints during event-driven transitions, while keeping this property inaccessible the rest of the time.
 
-```python
-from cosapp.base import System
-from math import sin, cos
-
-class SomeSystem(System):
-    def setup(self):
-        self.add_inward('x', 0.0)
-        self.add_inward('y', 0.0)
-        self.add_outward('z', 0.0)
-        a = self.add_event('event_a', trigger='x > y')
-        b = self.add_event('event_b', trigger='x < y')
-    
-    def compute(self):
-        self.z = cos(self.x) * sin(self.y)
-
-    def transition(self):
-        offdesign = self.problem
-        if self.event_a.present:
-            offdesign.clear()
-            offdesign.add_equation('z == 0.5').add_unknown('x')
-        if self.event_b.present:
-            offdesign.clear()
-```
+  ```python
+  from cosapp.base import System
+  from math import sin, cos
+  
+  class SomeSystem(System):
+      def setup(self):
+          self.add_inward('x', 0.0)
+          self.add_inward('y', 0.0)
+          self.add_outward('z', 0.0)
+          a = self.add_event('event_a', trigger='x > y')
+          b = self.add_event('event_b', trigger='x < y')
+      
+      def compute(self):
+          self.z = cos(self.x) * sin(self.y)
+  
+      def transition(self):
+          offdesign = self.problem
+          if self.event_a.present:
+              offdesign.clear()
+              offdesign.add_equation('z == 0.5').add_unknown('x')
+          if self.event_b.present:
+              offdesign.clear()
+  ```
 
 ### Bug fixes and code quality
 
 * Fix serialization bugs for systems with setup parameters (MR [#180](https://gitlab.com/cosapp/cosapp/-/merge_requests/180)) and `None` variables (MR [#172](https://gitlab.com/cosapp/cosapp/-/merge_requests/172)).
 * Bug fix on event time calculation involving array transients (MR [#177](https://gitlab.com/cosapp/cosapp/-/merge_requests/177)).
 * Bug fix on possible name conflicts in connector storage (MR [#173](https://gitlab.com/cosapp/cosapp/-/merge_requests/173)).
 * Fix inconsistent behaviour of `System.add_child` when a `pulling` error is raised (MR [#197](https://gitlab.com/cosapp/cosapp/-/merge_requests/197)).
@@ -203,79 +265,79 @@
 
 ### New features & API changes
 
 * Simplification of driver `Optimizer`:
   * Suppression of sub-driver `runner` (MR [#136](https://gitlab.com/cosapp/cosapp/-/merge_requests/136)). This change introduces new methods `set_objective`, `add_unknowns` and `add_constraints` in driver `Optimizer`.
   * Optimization constraints are now declared with human-readable expressions in `Optimizer.add_constraints` (MR [#138](https://gitlab.com/cosapp/cosapp/-/merge_requests/138)).
 
-Before:
+  Before:
+    
+  ```python
+  from cosapp.drivers import Optimizer
   
-```python
-from cosapp.drivers import Optimizer
-
-s = SomeSystem('s')
-optim = s.add_driver(Optimizer('optim'))
-
-optim.runner.set_objective('cost')
-optim.runner.add_unknown(['a', 'b', 'p_in.x'])
-# Enter constraints as non-negative expressions:
-optim.runner.add_constraints([
-    "b - a",  # b >= a
-    "a",      # a >= 0
-    "1 - a",  # a <= 1
-])
-optim.runner.add_constraints(
-    "p_out.y",
-    inequality = False,  # p_out.y == 0
-)
-
-s.run_drivers()
-```
-
-After:
-  
-```python
-optim.set_objective('cost')
-optim.add_unknown(['a', 'b', 'p_in.x'])
-optim.add_constraints(
-    "b >= a",
-    "0 <= a <= 1",
-    "p_out.y == 0",
-)
-```
+  s = SomeSystem('s')
+  optim = s.add_driver(Optimizer('optim'))
+  
+  optim.runner.set_objective('cost')
+  optim.runner.add_unknown(['a', 'b', 'p_in.x'])
+  # Enter constraints as non-negative expressions:
+  optim.runner.add_constraints([
+      "b - a",  # b >= a
+      "a",      # a >= 0
+      "1 - a",  # a <= 1
+  ])
+  optim.runner.add_constraints(
+      "p_out.y",
+      inequality = False,  # p_out.y == 0
+  )
+  
+  s.run_drivers()
+  ```
+  
+  After:
+    
+  ```python
+  optim.set_objective('cost')
+  optim.add_unknown(['a', 'b', 'p_in.x'])
+  optim.add_constraints(
+      "b >= a",
+      "0 <= a <= 1",
+      "p_out.y == 0",
+  )
+  ```
 
   * New, convenient iterators and setters for ports (MR [#137](https://gitlab.com/cosapp/cosapp/-/merge_requests/137)):
   
-```python
-from cosapp.base import Port, System
-
-class XyzPort(Port):
-    def setup(self):
-        self.add_variable('x')
-        self.add_variable('y')
-        self.add_variable('z')
-
-class SomeSystem(System):
-    def setup(self):
-        self.add_input(XyzPort, 'p_in')
-        self.add_output(XyzPort, 'p_out')
-    
-    def compute(self):
-        self.p_out.set_from(self.p_in)  # assign values from `p_in`
-        self.p_out.z = 0.0
-
-s = SomeSystem('s')
-# Multi-variable setter `set_values`
-s.p_in.set_values(x=1, y=-0.5, z=0.1)
-
-s.run_once()
-# Dict-like (key, value) iterator `items`:
-for varname, value in s.p_out.items():
-    print(f"p_out.{varname} = {value})
-```
+  ```python
+  from cosapp.base import Port, System
+  
+  class XyzPort(Port):
+      def setup(self):
+          self.add_variable('x')
+          self.add_variable('y')
+          self.add_variable('z')
+  
+  class SomeSystem(System):
+      def setup(self):
+          self.add_input(XyzPort, 'p_in')
+          self.add_output(XyzPort, 'p_out')
+      
+      def compute(self):
+          self.p_out.set_from(self.p_in)  # assign values from `p_in`
+          self.p_out.z = 0.0
+  
+  s = SomeSystem('s')
+  # Multi-variable setter `set_values`
+  s.p_in.set_values(x=1, y=-0.5, z=0.1)
+  
+  s.run_once()
+  # Dict-like (key, value) iterator `items`:
+  for varname, value in s.p_out.items():
+      print(f"p_out.{varname} = {value})
+  ```
 
 ### Documentation
 
 * Updated tutorials on ports (MR [#139](https://gitlab.com/cosapp/cosapp/-/merge_requests/139)) and on optimization (MR [#140](https://gitlab.com/cosapp/cosapp/-/merge_requests/140)).
 
 ### Bug fixes and code quality
```

### Comparing `cosapp-0.13.1/cosapp.egg-info/SOURCES.txt` & `cosapp-0.14.0/cosapp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 cosapp/core/module.py
 cosapp/core/time.py
 cosapp/core/variableref.py
 cosapp/core/numerics/__init__.py
 cosapp/core/numerics/basics.py
 cosapp/core/numerics/boundary.py
 cosapp/core/numerics/enum.py
+cosapp/core/numerics/mathematicalproblem.schema.json
 cosapp/core/numerics/residues.py
 cosapp/core/numerics/root.py
 cosapp/core/numerics/sobol_seq.py
 cosapp/core/signal/__init__.py
 cosapp/core/signal/signal.py
 cosapp/core/signal/slot.py
 cosapp/core/tests/__init__.py
-cosapp/core/tests/conftest.py
 cosapp/core/tests/test_AssignString.py
 cosapp/core/tests/test_ContextLocals.py
 cosapp/core/tests/test_EvalString.py
 cosapp/core/tests/test_Module.py
 cosapp/core/tests/test_coSAppConfiguration.py
 cosapp/core/tests/test_time.py
 cosapp/drivers/__init__.py
@@ -59,15 +59,14 @@
 cosapp/drivers/time/__init__.py
 cosapp/drivers/time/euler.py
 cosapp/drivers/time/interfaces.py
 cosapp/drivers/time/runge_kutta.py
 cosapp/drivers/time/scenario.py
 cosapp/drivers/time/utils.py
 cosapp/drivers/time/tests/__init__.py
-cosapp/drivers/time/tests/conftest.py
 cosapp/drivers/time/tests/test_BouncingBall.py
 cosapp/drivers/time/tests/test_DiscreteStepper.py
 cosapp/drivers/time/tests/test_EulerExplicit.py
 cosapp/drivers/time/tests/test_ExplicitTimeDriver.py
 cosapp/drivers/time/tests/test_InterpolAssignString.py
 cosapp/drivers/time/tests/test_Interpolator.py
 cosapp/drivers/time/tests/test_NewtonPendulum.py
@@ -104,71 +103,31 @@
 cosapp/recorders/dataframe_recorder.py
 cosapp/recorders/dsv_recorder.py
 cosapp/recorders/recorder.py
 cosapp/systems/__init__.py
 cosapp/systems/externalsystem.py
 cosapp/systems/metamodels.py
 cosapp/systems/processsystem.py
+cosapp/systems/structure.schema.json
 cosapp/systems/system.py
 cosapp/systems/system.schema.json
 cosapp/systems/systemConnector.py
 cosapp/systems/systemSurrogate.py
 cosapp/systems/systemfamily.py
-cosapp/tests/__init__.py
-cosapp/tests/all_tests.py
-cosapp/tests/conftest.py
-cosapp/tests/test_ComplexDuct.py
-cosapp/tests/test_MathematicalProblem_integration.py
-cosapp/tests/test_Turbofan.py
-cosapp/tests/test_dynamics.py
-cosapp/tests/test_electric_circuit.py
-cosapp/tests/test_multimode.py
-cosapp/tests/test_system_pressureloss.py
-cosapp/tests/test_tutorials.py
-cosapp/tests/test_unknown_aliasing.py
-cosapp/tests/test_visitor_integration.py
-cosapp/tests/data/default_dataframe.json
-cosapp/tests/data/export_doe.cs
-cosapp/tests/data/export_doe.csv
-cosapp/tests/data/export_doe.json
-cosapp/tests/data/export_doe.txt
-cosapp/tests/data/system_config.json
-cosapp/tests/data/system_config_ducts.json
-cosapp/tests/data/system_config_pressureloss.json
-cosapp/tests/data/system_config_pressureloss1.json
-cosapp/tests/data/system_config_pressureloss11.json
-cosapp/tests/data/system_config_pressureloss11bis.json
-cosapp/tests/data/system_config_pressureloss12.json
-cosapp/tests/data/system_config_pressureloss121.json
-cosapp/tests/data/system_config_pressureloss131.json
-cosapp/tests/data/system_config_pressureloss2.json
-cosapp/tests/data/system_config_pressureloss22.json
-cosapp/tests/data/system_config_pressureloss222.json
-cosapp/tests/data/system_config_pressureloss2tank.json
-cosapp/tests/library/__init__.py
-cosapp/tests/library/ports.py
-cosapp/tests/library/systems/__init__.py
-cosapp/tests/library/systems/basicalgebra.py
-cosapp/tests/library/systems/dynamics.py
-cosapp/tests/library/systems/elec.py
-cosapp/tests/library/systems/multiply.py
-cosapp/tests/library/systems/others.py
-cosapp/tests/library/systems/pressurelossvarious.py
-cosapp/tests/library/systems/vectors.py
 cosapp/tools/__init__.py
 cosapp/tools/help.py
 cosapp/tools/trigger.py
 cosapp/tools/fmu/__init__.py
 cosapp/tools/fmu/exporter.py
 cosapp/tools/fmu/logging.py
 cosapp/tools/fmu/tests/__init__.py
-cosapp/tools/fmu/tests/conftest.py
 cosapp/tools/fmu/tests/test_exporter.py
 cosapp/tools/fmu/tests/test_logging.py
 cosapp/tools/module_parser/__init__.py
+cosapp/tools/module_parser/package_metadata.schema.json
 cosapp/tools/module_parser/parseModule.py
 cosapp/tools/problem_viewer/__init__.py
 cosapp/tools/problem_viewer/problem_viewer.py
 cosapp/tools/problem_viewer/webview.py
 cosapp/tools/problem_viewer/tests/__init__.py
 cosapp/tools/problem_viewer/tests/test_viewmodeldata.py
 cosapp/tools/problem_viewer/visualization/index.html
```

### Comparing `cosapp-0.13.1/docs/Makefile` & `cosapp-0.14.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/conf.py` & `cosapp-0.14.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/layout.html` & `cosapp-0.14.0/docs/cosapp_theme/layout.html`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/searchbox.html` & `cosapp-0.14.0/docs/cosapp_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/cosapp.css_t` & `cosapp-0.14.0/docs/cosapp_theme/static/cosapp.css_t`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/css/custom.css` & `cosapp-0.14.0/docs/cosapp_theme/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/css/font-awesome.min.css` & `cosapp-0.14.0/docs/cosapp_theme/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/css/font.css` & `cosapp-0.14.0/docs/cosapp_theme/static/css/font.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/css/highlight.css` & `cosapp-0.14.0/docs/cosapp_theme/static/css/highlight.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/css/kube.css` & `cosapp-0.14.0/docs/cosapp_theme/static/css/kube.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/css/kube.demo.css` & `cosapp-0.14.0/docs/cosapp_theme/static/css/kube.demo.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/css/kube.legenda.css` & `cosapp-0.14.0/docs/cosapp_theme/static/css/kube.legenda.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/css/kube.min.css` & `cosapp-0.14.0/docs/cosapp_theme/static/css/kube.min.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/css/master.css` & `cosapp-0.14.0/docs/cosapp_theme/static/css/master.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/font/Lato-Black.woff` & `cosapp-0.14.0/docs/cosapp_theme/static/font/Lato-Black.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/font/Lato-Bold.woff` & `cosapp-0.14.0/docs/cosapp_theme/static/font/Lato-Bold.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/font/Lato-BoldItalic.woff` & `cosapp-0.14.0/docs/cosapp_theme/static/font/Lato-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/font/Lato-Italic.woff` & `cosapp-0.14.0/docs/cosapp_theme/static/font/Lato-Italic.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/font/Lato-Regular.woff` & `cosapp-0.14.0/docs/cosapp_theme/static/font/Lato-Regular.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/font/Lato-Semibold.woff` & `cosapp-0.14.0/docs/cosapp_theme/static/font/Lato-Semibold.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/fonts/fontawesome-webfont.woff` & `cosapp-0.14.0/docs/cosapp_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/img/cosapp.svg` & `cosapp-0.14.0/docs/cosapp_theme/static/img/cosapp.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/js/jquery-2.1.4.min.js` & `cosapp-0.14.0/docs/cosapp_theme/static/js/jquery-2.1.4.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/js/kube.js` & `cosapp-0.14.0/docs/cosapp_theme/static/js/kube.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/js/kube.min.js` & `cosapp-0.14.0/docs/cosapp_theme/static/js/kube.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/js/tocbot.min.js` & `cosapp-0.14.0/docs/cosapp_theme/static/js/tocbot.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/static/sidebar.js_t` & `cosapp-0.14.0/docs/cosapp_theme/static/sidebar.js_t`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/cosapp_theme/theme.conf` & `cosapp-0.14.0/docs/cosapp_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/developer/installation_cases.rst` & `cosapp-0.14.0/docs/developer/installation_cases.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/developer/logger.rst` & `cosapp-0.14.0/docs/developer/logger.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/developer/project_structure.rst` & `cosapp-0.14.0/docs/developer/project_structure.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/developer/scenarii.rst` & `cosapp-0.14.0/docs/developer/scenarii.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/img/gitlab-cosapp-f4950f.svg` & `cosapp-0.14.0/docs/img/gitlab-cosapp-f4950f.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/img/website-docs-blue.svg` & `cosapp-0.14.0/docs/img/website-docs-blue.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/index.rst` & `cosapp-0.14.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/installation.rst` & `cosapp-0.14.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/make.bat` & `cosapp-0.14.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/nb_thumbnails/_images/verified.svg` & `cosapp-0.14.0/docs/nb_thumbnails/_images/verified.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/source/modules.rst` & `cosapp-0.14.0/docs/source/modules.rst`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
    cosapp.recorders.dsv_recorder
 
    cosapp.tools.fmu.exporter
    cosapp.tools.problem_viewer.problem_viewer
    cosapp.tools.problem_viewer.webview
    cosapp.tools.help
    cosapp.tools.trigger
+   cosapp.tools.module_parser.parseModule
 
    cosapp.utils.distributions.distribution
    cosapp.utils.distributions.normal
    cosapp.utils.distributions.triangular
    cosapp.utils.distributions.uniform
 
    cosapp.utils.context
```

### Comparing `cosapp-0.13.1/docs/tools/mermaid.py` & `cosapp-0.14.0/docs/tools/mermaid.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tools/mermaid_inheritance.py` & `cosapp-0.14.0/docs/tools/mermaid_inheritance.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/00-Introduction.ipynb` & `cosapp-0.14.0/docs/tutorials/00-Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/01-Systems.ipynb` & `cosapp-0.14.0/docs/tutorials/01-Systems.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978052524927525%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(19, "s = Multiply(name=\'s\')")], delete: [19]}}, 9: '*

 * *            "{'source': {insert: [(19, '- **unit**: Physical unit of the variable, given by a "*

 * *            'string. **CoSApp** will take care of unit conversion between connected systems. '*

 * *            'However, *units are not enforced* inside a `System`. Therefore, module developers '*

 * *            "must ensure that all variables are consistently converted in method `compute`.\\n'), "*

 * *            "(20, '- **desc* […]*

```diff
@@ -67,15 +67,15 @@
                 "        self.add_inward('K1', 1.0)\n",
                 "        self.add_outward('delta_x', 0.0)\n",
                 "\n",
                 "    def compute(self): # `compute` method defines what the system does\n",
                 "        self.p_out.x = self.p_in.x * self.K1\n",
                 "        self.delta_x = self.p_out.x - self.p_in.x\n",
                 "\n",
-                "s = Multiply(name='mult')"
+                "s = Multiply(name='s')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "![Multiple systems](images/systems_1.svg)"
@@ -98,14 +98,15 @@
                 "s.K1 = 5.\n",
                 "s.run_once()\n",
                 "\n",
                 "s.p_out"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "More information on ports (`inputs` *and* `outputs`) can be found in a dedicated [Port tutorial](02-Ports.ipynb).\n",
                 "\n",
                 "#### `inwards` and `outwards` ports\n",
                 "\n",
@@ -120,61 +121,68 @@
                 "- An *inward* is an input parameter needed by the system to compute its output. For example, the pressure losses coefficient of a duct is an inward, used to compute the output flow port from its input flow port.\n",
                 "- An *outward* is an output variable deduced from inputs, such as an intermediate variable of a computation, which is exposed to other systems. For instance, the difference between the input and output pressures in a duct system is a local variable, which may be of interest to neighbouring systems. Another example is the table object read from a filename (the filename being usually an *inward*). \n",
                 "\n",
                 "An inward `x` (resp. outward) defined in system `s` can be accessed as either `s.x` or `s.inwards.x` (resp. `s.outwards.x`).\n",
                 "\n",
                 "All variables in **CoSApp** accept additional information:\n",
                 "\n",
-                "- *unit*: Physical unit of the variable, given by a string. **CoSApp** will take care of unit conversion between connected systems. However, *units are not enforced* inside a `System`. Therefore, module developers must ensure that all variables are consistently converted in method `compute`.\n",
-                "- *desc*: Short description of the variable.\n",
-                "- *dtype*: If you need to force certain data type(s) on a variable, a tuple of acceptable types can be provided through this keyword. If that information is not supplied, dtype is inferred from the variable value; *e.g.* a number (`int` or `float`) will be typed as `Number`."
+                "- **unit**: Physical unit of the variable, given by a string. **CoSApp** will take care of unit conversion between connected systems. However, *units are not enforced* inside a `System`. Therefore, module developers must ensure that all variables are consistently converted in method `compute`.\n",
+                "- **desc**: Short description of the variable.\n",
+                "- **dtype**: If you need to force certain data type(s) on a variable, a tuple of acceptable types can be provided through this keyword. If that information is not supplied, dtype is inferred from the variable value; *e.g.* a number (`int` or `float`) will be typed as `Number`.\n",
+                "\n",
+                "Methods `add_input` and `add_output` also accept optional argument `desc`, if a contextual description is desired."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "class MultiplyAdvanced(System):\n",
                 "\n",
                 "    def setup(self):\n",
-                "        self.add_input(DemoPort, 'p_in')\n",
-                "        # Inward and outward variables accept optional dtype and unit\n",
+                "        # Inwput and output ports accept optional description `desc`\n",
+                "        self.add_input(DemoPort, 'p_in', desc='Port containing values to be multiplied')\n",
+                "        # Inward and outward variables accept optional `dtype` and `unit`\n",
                 "        self.add_inward('K1', 1, dtype=int, desc='Multiplication coefficient')\n",
                 "        self.add_outward('delta_x',\n",
                 "            value = 0.0,\n",
                 "            unit = 'Pa',\n",
                 "            dtype = (int, float), \n",
                 "            desc = \"Difference between `DemoPort` output and input\"\n",
                 "        )\n",
                 "        self.add_output(DemoPort, 'p_out')\n",
                 "\n",
                 "    def compute(self):\n",
                 "        self.p_out.x = self.p_in.x * self.K1\n",
                 "        self.delta_x = self.p_out.x - self.p_in.x\n",
                 "\n",
-                "advanced = MultiplyAdvanced(name='mult')\n",
+                "\n",
+                "advanced = MultiplyAdvanced('advanced')\n",
                 "\n",
                 "print(\n",
-                "    f\"Inwards: \\n  {advanced.inwards}\",\n",
-                "    f\"Outwards:\\n  {advanced.outwards}\",\n",
+                "    f\"{advanced.inwards  = }\",\n",
+                "    f\"{advanced.outwards = }\",\n",
                 "    sep=\"\\n\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Composite Systems\n",
                 "\n",
                 "Composite systems contain sub-systems, referred to as `children`.\n",
                 "\n",
                 "Sub-systems are added to a composite system using method `add_child`.\n",
+                "Like ports and variables, sub-systems can be briefly described in the context of their parent system, with optional argument `desc`.\n",
+                "\n",
                 "Connections between child systems are declared at parent level, with method `connect`.\n",
                 "The typical syntax is `parent.connect(child1.portA, child2.portB)`.\n",
                 "\n",
                 "`Port` connections are described in detail in the [Port tutorial](02-Ports.ipynb)."
             ]
         },
         {
@@ -182,22 +190,22 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "class MultiplyComplexSystem(System):\n",
                 "\n",
                 "    def setup(self):\n",
-                "        # Children\n",
-                "        self.add_child(Multiply('mult1'))  # add a sub-system\n",
+                "        # Sub-systems\n",
+                "        self.add_child(Multiply('mult1'), desc='Primary sub-system')\n",
                 "        self.add_child(Multiply('mult2'))\n",
                 "        \n",
                 "        # Connectors\n",
                 "        self.connect(self.mult1.p_out, self.mult2.p_in)  # connect ports of sub-systems\n",
                 "\n",
-                "head = MultiplyComplexSystem(name='head')"
+                "head = MultiplyComplexSystem('head')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "![Connection between Systems](images/systems_2.svg)"
```

### Comparing `cosapp-0.13.1/docs/tutorials/02-Ports.ipynb` & `cosapp-0.14.0/docs/tutorials/02-Ports.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990301724137931%*

 * *Differences: {"'cells'": '{17: {\'source\': {insert: [(18, \'print(\\n\'), (19, \'    f"{h.monitor.a = '*

 * *            '}",\\n\'), (20, \'    f"{h.demo1.p_out = }",\\n\'), (21, \')\')], delete: [19, 18]}}, '*

 * *            '19: {\'source\': [\'print(f"{h.demo2.p_in = }")\']}, 20: {\'source\': '*

 * *            '[\'print(f"{h.monitor.outwards = }")\']}}'}*

```diff
@@ -247,16 +247,18 @@
                 "h.add_child(MonitorSystem('monitor'))\n",
                 "# Connect `h.monitor.a` to `h.demo1.p_out.a`\n",
                 "h.connect(h.monitor.inwards, h.demo1.p_out, 'a')\n",
                 "\n",
                 "h.demo1.p_in.set_values(a=50., b=0., c=25.)\n",
                 "h.run_once()\n",
                 "\n",
-                "print(f\"{h.monitor.a = }\")\n",
-                "h.demo1.p_out"
+                "print(\n",
+                "    f\"{h.monitor.a = }\",\n",
+                "    f\"{h.demo1.p_out = }\",\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In the example above, variable `a` from port `inwards` has been connected to variable `a` from port `demo1.p_out`.\n",
@@ -284,24 +286,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "h.demo2.p_in"
+                "print(f\"{h.demo2.p_in = }\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "h.monitor.outwards"
+                "print(f\"{h.monitor.outwards = }\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Example with unit conversions"
```

### Comparing `cosapp-0.13.1/docs/tutorials/03-Drivers.ipynb` & `cosapp-0.14.0/docs/tutorials/03-Drivers.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/04-Triggers.ipynb` & `cosapp-0.14.0/docs/tutorials/04-Triggers.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/05-Validation.ipynb` & `cosapp-0.14.0/docs/tutorials/05-Validation.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/06-Visibility.ipynb` & `cosapp-0.14.0/docs/tutorials/06-Visibility.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/07-Metamodels.ipynb` & `cosapp-0.14.0/docs/tutorials/07-Metamodels.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/08-Multipoints-Design.ipynb` & `cosapp-0.14.0/docs/tutorials/08-Multipoints-Design.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/09-MonteCarlo.ipynb` & `cosapp-0.14.0/docs/tutorials/09-MonteCarlo.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/10-Recorders.ipynb` & `cosapp-0.14.0/docs/tutorials/10-Recorders.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/11-DesignMethods.ipynb` & `cosapp-0.14.0/docs/tutorials/11-DesignMethods.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/CustomConnectors.ipynb` & `cosapp-0.14.0/docs/tutorials/CustomConnectors.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/FMI.ipynb` & `cosapp-0.14.0/docs/tutorials/FMI.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/Guidelines.ipynb` & `cosapp-0.14.0/docs/tutorials/Guidelines.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/HybridSimulations.ipynb` & `cosapp-0.14.0/docs/tutorials/HybridSimulations.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/Logging.ipynb` & `cosapp-0.14.0/docs/tutorials/Logging.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/Optimization.ipynb` & `cosapp-0.14.0/docs/tutorials/Optimization.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/SystemSurrogates.ipynb` & `cosapp-0.14.0/docs/tutorials/SystemSurrogates.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/SystemSurrogatesAdvanced.ipynb` & `cosapp-0.14.0/docs/tutorials/SystemSurrogatesAdvanced.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/Targets.ipynb` & `cosapp-0.14.0/docs/tutorials/Targets.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/TimeDriver.ipynb` & `cosapp-0.14.0/docs/tutorials/TimeDriver.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/TimeDriverAdvanced.ipynb` & `cosapp-0.14.0/docs/tutorials/TimeDriverAdvanced.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/TipsAndTricks.ipynb` & `cosapp-0.14.0/docs/tutorials/TipsAndTricks.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/Visitors.ipynb` & `cosapp-0.14.0/docs/tutorials/Visitors.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/aa-SimpleCircuit.ipynb` & `cosapp-0.14.0/docs/tutorials/aa-SimpleCircuit.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/exprampode_fmu.py` & `cosapp-0.14.0/docs/tutorials/exprampode_fmu.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/Moise_tables_loi.jpg` & `cosapp-0.14.0/docs/tutorials/images/Moise_tables_loi.jpg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/cosapp.svg` & `cosapp-0.14.0/docs/tutorials/images/cosapp.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/design_circuit.svg` & `cosapp-0.14.0/docs/tutorials/images/design_circuit.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/drivers_1.svg` & `cosapp-0.14.0/docs/tutorials/images/drivers_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/drivers_2.svg` & `cosapp-0.14.0/docs/tutorials/images/drivers_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/drivers_3.svg` & `cosapp-0.14.0/docs/tutorials/images/drivers_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/drivers_4.svg` & `cosapp-0.14.0/docs/tutorials/images/drivers_4.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/drivers_5.svg` & `cosapp-0.14.0/docs/tutorials/images/drivers_5.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/drivers_nonlinear.svg` & `cosapp-0.14.0/docs/tutorials/images/drivers_nonlinear.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/experimental.svg` & `cosapp-0.14.0/docs/tutorials/images/experimental.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/in_progress.svg` & `cosapp-0.14.0/docs/tutorials/images/in_progress.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/ports_1.svg` & `cosapp-0.14.0/docs/tutorials/images/ports_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/ports_2.svg` & `cosapp-0.14.0/docs/tutorials/images/ports_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/ports_3.svg` & `cosapp-0.14.0/docs/tutorials/images/ports_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/simple_circuit.svg` & `cosapp-0.14.0/docs/tutorials/images/simple_circuit.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/systems_1.svg` & `cosapp-0.14.0/docs/tutorials/images/systems_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/systems_2.svg` & `cosapp-0.14.0/docs/tutorials/images/systems_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/systems_3.svg` & `cosapp-0.14.0/docs/tutorials/images/systems_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/systems_4.svg` & `cosapp-0.14.0/docs/tutorials/images/systems_4.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/systems_5.svg` & `cosapp-0.14.0/docs/tutorials/images/systems_5.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/tanks.svg` & `cosapp-0.14.0/docs/tutorials/images/tanks.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/triggers_1.svg` & `cosapp-0.14.0/docs/tutorials/images/triggers_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/triggers_2.svg` & `cosapp-0.14.0/docs/tutorials/images/triggers_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/validity.svg` & `cosapp-0.14.0/docs/tutorials/images/validity.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/images/visibility.svg` & `cosapp-0.14.0/docs/tutorials/images/visibility.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/multimode/BouncingBall.ipynb` & `cosapp-0.14.0/docs/tutorials/multimode/BouncingBall.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/multimode/MultimodeOde.ipynb` & `cosapp-0.14.0/docs/tutorials/multimode/MultimodeOde.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/multimode/NewtonPendulum.ipynb` & `cosapp-0.14.0/docs/tutorials/multimode/NewtonPendulum.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/optimization/BetzLimit.ipynb` & `cosapp-0.14.0/docs/tutorials/optimization/BetzLimit.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/optimization/Sellar.ipynb` & `cosapp-0.14.0/docs/tutorials/optimization/Sellar.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/quickstart.ipynb` & `cosapp-0.14.0/docs/tutorials/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/docs/tutorials/time_solutions.py` & `cosapp-0.14.0/docs/tutorials/time_solutions.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.13.1/setup.cfg` & `cosapp-0.14.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	Programming Language :: Python :: 3.10
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 test_suite = cosapp.tests.all_tests.suite
-python_requires = >= 3.7
+python_requires = >= 3.8
 install_requires = 
 	pandas
 	jsonschema
 	numpy>=1.12
 	scipy
 	wrapt
 tests_require = 
@@ -80,14 +80,15 @@
 
 [coverage:run]
 source = 
 	cosapp
 omit = 
 	*/tests/*
 	*/test_*
+	*/conftest.py
 	cosapp/tools/templates/*
 	cosapp/utils/testing.py
 
 [coverage:report]
 exclude_lines = 
 	pragma: no cover
```

### Comparing `cosapp-0.13.1/setup.py` & `cosapp-0.14.0/setup.py`

 * *Files identical despite different names*

