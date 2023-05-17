# Comparing `tmp/qiskit-nature-0.6.0.tar.gz` & `tmp/qiskit-nature-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qiskit-nature-0.6.0.tar", last modified: Fri Apr 14 13:12:08 2023, max compression
+gzip compressed data, was "dist/qiskit-nature-0.6.1.tar", last modified: Wed May 17 13:14:01 2023, max compression
```

## Comparing `qiskit-nature-0.6.0.tar` & `qiskit-nature-0.6.1.tar`

### file list

```diff
@@ -1,1104 +1,1104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/eigensolver_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/numpy_eigensolver_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/excited_states_eigensolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/excited_states_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/qeom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/adapt_vqe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/ground_state_eigensolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/ground_state_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/minimum_eigensolver_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/numpy_minimum_eigensolver_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13180 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_ucc_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_uvcc_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/initial_points/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/initial_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/initial_points/hf_initial_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/initial_points/initial_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/initial_points/mp2_initial_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/initial_points/vscf_initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/bopes_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20098 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/extrapolator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/potentials/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/potentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/potentials/energy_surface_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/potentials/harmonic_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/potentials/morse_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/potentials/potential_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/chc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/puccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/succd.py
--rw-r--r--   0 runner    (1001) docker     (123)    21323 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/ucc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/uccsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/utils/fermionic_excitation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/utils/vibration_excitation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/uvcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/uvccsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/bogoliubov_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/fermionic_gaussian_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/hartree_fock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/slater_determinant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/utils/givens_rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/vscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/converters/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/converters/second_quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21012 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/converters/second_quantization/qubit_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/converters/second_quantization/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/converters/second_quantization/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/converters/second_quantization/utils/list_or_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/deprecation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/bosonic_bases/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/bosonic_bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/bosonic_bases/bosonic_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/bosonic_bases/harmonic_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)    18545 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)    33098 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/qmolecule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/base_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/electronic_structure_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/electronic_structure_molecule_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/fcidumpd/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/fcidumpd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/fcidumpd/dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/fcidumpd/fcidumpdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/fcidumpd/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12784 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    27815 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/QCMatEl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18069 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/QCOpMat.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33018 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.F
--rw-r--r--   0 runner    (1001) docker     (123)   132096 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cp310-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   125952 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cp37-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   126464 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cp38-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   129024 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cp39-win_amd64.pyd
--rwxr-xr-x   0 runner    (1001) docker     (123)   556024 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-310-darwin.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   420344 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-310-x86_64-linux-gnu.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   481832 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-37m-darwin.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   452040 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-37m-x86_64-linux-gnu.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   481976 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-38-darwin.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   489696 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-38-x86_64-linux-gnu.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   525864 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-39-darwin.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   242888 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-39-x86_64-linux-gnu.so
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_forces_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_log_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_log_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gaussiandriver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/hdf5d/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/hdf5d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/hdf5d/hdf5driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/psi4d/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/psi4d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/psi4d/_template.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/psi4d/psi4driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/pyquanted/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/pyquanted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/pyquanted/pyquantedriver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/pyscfd/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/pyscfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27394 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/pyscfd/pyscfdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/vibrational_structure_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/vibrational_structure_molecule_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/units_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/drivers/watson_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/list_or_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22722 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/bksf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/bravyi_kitaev_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/direct_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/fermionic_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/jordan_wigner_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/linear_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/logarithmic_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/parity_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/qubit_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/spin_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/vibrational_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/operators/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27314 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/fermionic_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/quadratic_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/second_quantized_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    21402 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/spin_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23187 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/vibrational_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/optionals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/bead_contacts/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/bead_contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/bead_contacts/contact_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/bead_contacts/contact_map_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/bead_distances/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/bead_distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/bead_distances/distance_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/bead_distances/distance_map_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/data_loaders/energy_matrix_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/exceptions/invalid_residue_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/exceptions/invalid_side_chain_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/exceptions/invalid_size_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/mixed_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/miyazawa_jernigan_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/random_interaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/resources/mj_matrix.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/penalty_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/beads/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/beads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/beads/base_bead.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/beads/main_bead.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/beads/side_bead.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/chains/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/chains/base_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/chains/main_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/chains/side_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/pauli_ops_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/peptide.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/protein_folding_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    20630 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/qubit_op_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/qubit_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/qubit_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/qubit_utils/qubit_fixing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/qubit_utils/qubit_number_reducer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/residue_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/sampling/sampling_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/base_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/electronic/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/electronic/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/electronic/builders/hopping_ops_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/electronic/electronic_structure_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattice_model_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/boundary_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/hyper_cubic_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/line_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/square_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10928 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/triangular_lattice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/models/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/models/fermi_hubbard_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/models/ising_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/models/lattice_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/vibrational/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/vibrational/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/vibrational/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/vibrational/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/vibrational/builders/hopping_ops_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/vibrational/builders/vibrational_label_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/vibrational/vibrational_structure_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/grouped_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/driver_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/angular_momentum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/bases/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/bases/electronic_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/bases/electronic_basis_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/dipole_moment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/electronic_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/electronic_structure_driver_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/integrals/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/integrals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17698 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/integrals/electronic_integrals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/integrals/integral_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/integrals/one_body_electronic_integrals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/integrals/two_body_electronic_integrals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/magnetization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/particle_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/second_quantized_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/bases/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/bases/harmonic_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/bases/vibrational_basis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/integrals/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/integrals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/integrals/vibrational_integrals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/occupied_modals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/vibrational_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/vibrational_structure_driver_result.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/results/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/results/bopes_sampler_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/results/eigenstate_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/results/electronic_structure_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/results/lattice_model_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/results/protein_folding_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/results/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/results/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/results/utils/protein_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/results/utils/protein_shape_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/results/utils/protein_shape_file_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/results/vibrational_structure_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/runtime/vqe_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/eigensolver_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/numpy_eigensolver_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/excited_states_eigensolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/excited_states_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    55023 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/qeom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/qeom_electronic_ops_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/qeom_vibrational_ops_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/ground_state_eigensolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/ground_state_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/minimum_eigensolver_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/numpy_minimum_eigensolver_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_ucc_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_uvcc_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/initial_points/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/initial_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/initial_points/hf_initial_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/initial_points/initial_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/initial_points/mp2_initial_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/initial_points/vscf_initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/chc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/puccd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/succd.py
--rw-r--r--   0 runner    (1001) docker     (123)    24934 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/ucc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/uccsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/utils/fermionic_excitation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/utils/vibration_excitation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/uvcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/uvccsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/bogoliubov_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/fermionic_gaussian_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/hartree_fock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/slater_determinant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/utils/givens_rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/vscf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/base_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/electronic_structure_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12784 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    27815 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/QCMatEl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18069 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/QCOpMat.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33018 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.F
--rw-r--r--   0 runner    (1001) docker     (123)   132096 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cp310-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   129536 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cp311-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   125952 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cp37-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   126464 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cp38-win_amd64.pyd
--rw-r--r--   0 runner    (1001) docker     (123)   129024 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cp39-win_amd64.pyd
--rwxr-xr-x   0 runner    (1001) docker     (123)   556024 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-310-darwin.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   420344 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-310-x86_64-linux-gnu.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   167328 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-311-darwin.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   413656 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-311-x86_64-linux-gnu.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   481832 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-37m-darwin.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   452040 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-37m-x86_64-linux-gnu.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   481976 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-38-darwin.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   489696 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-38-x86_64-linux-gnu.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   525864 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-39-darwin.so
--rwxr-xr-x   0 runner    (1001) docker     (123)   242888 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-39-x86_64-linux-gnu.so
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gaussian_forces_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gaussian_log_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gaussian_log_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gaussian_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19213 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gaussiandriver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/psi4d/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/psi4d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/psi4d/_template.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/psi4d/psi4driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/pyscfd/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/pyscfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/pyscfd/pyscfdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/vibrational_structure_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/fcidump/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/fcidump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/fcidump/dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/fcidump/fcidump.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/fcidump/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/fcidump_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/molecule_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_basis_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    14946 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_schema_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_topology.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_wavefunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema_translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/watson/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/watson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/watson/watson_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/formats/watson_translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/electronic_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/fermi_hubbard_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/heisenberg_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/ising_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattice_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/boundary_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/hyper_cubic_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/line_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/square_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/triangular_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/quadratic_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/vibrational_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22931 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/bksf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/bravyi_kitaev_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/direct_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/fermionic_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/interleaved_qubit_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/jordan_wigner_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/linear_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/logarithmic_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/parity_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    26859 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/qubit_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12824 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/qubit_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/spin_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/tapered_qubit_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/vibrational_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/_bits_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/commutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    27586 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/electronic_integrals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25398 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/fermionic_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    27244 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/polynomial_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20279 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/sparse_label_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/spin_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/symmetric_two_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    25683 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/tensor_ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/vibrational_integrals.py
--rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/operators/vibrational_op.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/base_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/eigenstate_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/electronic_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/electronic_properties_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    15897 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/electronic_structure_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/electronic_structure_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/harmonic_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/lattice_model_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/lattice_model_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/lattice_properties_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/properties_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/vibrational_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/vibrational_properties_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/vibrational_structure_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/problems/vibrational_structure_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/properties/angular_momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/properties/dipole_moment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/properties/electronic_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/properties/magnetization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/properties/occupied_modals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/properties/particle_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/properties/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29154 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/transformers/active_space_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/transformers/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/transformers/basis_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/second_q/transformers/freeze_core_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/testing/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/transformers/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/transformers/second_quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/transformers/second_quantization/base_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/transformers/second_quantization/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/transformers/second_quantization/electronic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/transformers/second_quantization/electronic/active_space_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/transformers/second_quantization/electronic/freeze_core_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/utils/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/utils/opt_einsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/qiskit_nature/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    57099 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/qiskit_nature.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/algorithms/excited_state_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/excited_state_solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/algorithms/excited_state_solvers/eigensolver_factories/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/excited_state_solvers/eigensolver_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/excited_state_solvers/eigensolver_factories/test_numpy_eigensolver_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/excited_state_solvers/test_bosonic_esc_calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/excited_state_solvers/test_excited_states_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/minimum_eigensolver_factories/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/minimum_eigensolver_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_ucc_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_uvcc_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/test_adapt_vqe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/test_advanced_ucc_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    27402 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/test_groundstate_eigensolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/test_swaprz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/algorithms/initial_points/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/initial_points/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/algorithms/initial_points/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/initial_points/resources/test_mp2_initial_point.json
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/initial_points/test_hf_initial_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/initial_points/test_initial_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/initial_points/test_mp2_initial_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/initial_points/test_vscf_initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/algorithms/pes_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/pes_samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/algorithms/pes_samplers/potentials/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/pes_samplers/potentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/pes_samplers/potentials/test_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/pes_samplers/test_bopes_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/algorithms/pes_samplers/test_extrapolators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/circuit/library/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/test_chc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/test_puccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/test_succd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/test_ucc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/test_uccsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/test_uvcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/utils/test_fermionic_excitation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/utils/test_vibration_excitation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/ansatzes/utils/vibrational_op_label_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/circuit/library/initial_states/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/initial_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/initial_states/test_fermionic_gaussian_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/initial_states/test_hartree_fock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/initial_states/test_slater_determinant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/initial_states/test_vscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/circuit/library/test_bogoliubov_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/converters/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/converters/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/converters/second_quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/converters/second_quantization/test_qubit_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_h2.fcidump
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_lih.fcidump
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_lih.npz
--rw-r--r--   0 runner    (1001) docker     (123)    24909 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_oh.fcidump
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_oh.npz
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_methods_fcidump.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_forces.py
--rw-r--r--   0 runner    (1001) docker     (123)   940592 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_from_mat.mat
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_from_mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log_A03.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log_C01.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log_vibrational_energy.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_methods_gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/hdf5d/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/hdf5d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48547 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/hdf5d/test_driver_hdf5.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/hdf5d/test_driver_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/hdf5d/test_driver_hdf5_legacy.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/psi4d/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/psi4d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/psi4d/test_driver_methods_psi4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/psi4d/test_driver_psi4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/psi4d/test_driver_psi4_extra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/pyquanted/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/pyquanted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/pyquanted/test_driver_methods_pyquante.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/pyquanted/test_driver_pyquante.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/pyscfd/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/pyscfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/pyscfd/test_driver_methods_pyscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/pyscfd/test_driver_pyscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/test_driver_methods_gsc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/test_driver_molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/drivers/second_quantization/test_molecule_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/mappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/resources/bksf_lih.py
--rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/resources/reference_direct_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/test_bksf_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/test_bravyi_kitaev_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/test_direct_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/test_jordan_wigner_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/test_linear_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/test_logarithmic_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/mappers/second_quantization/test_parity_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/nature_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/operators/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/operators/second_quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24378 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/operators/second_quantization/test_fermionic_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/operators/second_quantization/test_quadratic_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/operators/second_quantization/test_spin_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/operators/second_quantization/test_vibrational_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/operators/second_quantization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/bead_contacts/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/bead_contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/bead_contacts/test_contact_map_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/bead_distances/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/bead_distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/bead_distances/test_distance_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/bead_distances/test_distance_map_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/data_loaders/test_energy_matrix_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/interactions/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/interactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/interactions/test_mixed_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/interactions/test_miyazawa_jernigan_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/interactions/test_random_interaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/beads/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/beads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/beads/test_bead_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/beads/test_bead_side.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/chains/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/chains/test_chain_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/chains/test_chain_side.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/test_peptide.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/qubit_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/qubit_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/qubit_utils/test_qubit_fixing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/qubit_utils/test_qubit_number_reducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_bead_main/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_bead_main/test_main_bead_constructor_expected_indic_0
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_bead_main/test_main_bead_constructor_expected_indic_1
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_bead_main/test_main_bead_constructor_expected_indic_2
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_bead_main/test_main_bead_constructor_expected_indic_3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_bead_side/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_bead_side/test_side_bead_constructor_expected_indic_0
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_bead_side/test_side_bead_constructor_expected_indic_1
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_bead_side/test_side_bead_constructor_expected_indic_2
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_bead_side/test_side_bead_constructor_expected_indic_3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_contact_map_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_2_expected_1
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_2_expected_2
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_3_expected_1
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_3_expected_2
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_3_expected_3
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_3_expected_4
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_3_expected_5
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_3_expected_6
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map/test_first_neighbor
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map/test_first_neighbor_side
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map/test_second_neighbor
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map/test_second_neighbor_2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_add_distances_side_chain
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_calc_distances_main_chain_1
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_calc_distances_main_chain_2
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_calc_distances_main_chain_3
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_calc_distances_main_chain_4
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_calc_total_distances_1
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_calc_total_distances_2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_protein_folding_problem/
--rw-r--r--   0 runner    (1001) docker     (123)   639850 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_protein_folding_problem/test_protein_folding_problem
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_protein_folding_problem/test_protein_folding_problem_2
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_protein_folding_problem/test_protein_folding_problem_2_second_bead_side_chain
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_build_qubit_op_2_expected
--rw-r--r--   0 runner    (1001) docker     (123)   294639 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_build_qubit_op_expected
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_check_turns_expected
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_check_turns_expected_t23
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_check_turns_expected_t2s3
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_check_turns_expected_t34
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_check_turns_expected_t3s4s
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_back_expected
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_back_side_chains_expected
--rw-r--r--   0 runner    (1001) docker     (123)    43153 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbbb_expected
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbsc_and_h_scbb_2_expected
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbsc_and_h_scbb_expected_h_bbsc
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbsc_and_h_scbb_expected_h_scbb
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_chiral_2_expected
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_chiral_expected
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/test_protein_folding_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/sampling/protein_folding/test_qubit_op_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/second_quantization/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/second_quantization/electronic/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/electronic/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/electronic/builders/test_hopping_ops_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/second_quantization/electronic/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/electronic/resources/H2_631g_ferm_op_active_space
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/electronic/resources/H2_631g_ferm_op_one_int
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/electronic/resources/H2_631g_ferm_op_two_ints
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/electronic/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/electronic/resources/resource_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/electronic/test_electronic_structure_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/lattices/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/lattices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/lattices/test_hyper_cubic_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/lattices/test_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/lattices/test_line_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/lattices/test_square_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/lattices/test_triangular_lattice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/models/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/models/test_fermi_hubbard_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/models/test_ising_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/lattice/test_lattice_model_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/second_quantization/vibrational/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/vibrational/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/second_quantization/vibrational/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/vibrational/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/vibrational/builders/test_hopping_ops_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/problems/second_quantization/vibrational/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/vibrational/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/vibrational/resources/expected_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/problems/second_quantization/vibrational/test_vibrational_structure_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/property_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/properties/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/resources/integral_property_op.json
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_second_q_op_alpha_and_beta_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_second_q_op_only_alpha_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_spin_alpha_and_beta_expected.numpy.bin
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_spin_only_alpha_expected.numpy.bin
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/test_integral_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/test_one_body_electronic_integrals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/test_two_body_electronic_integrals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/resources/angular_momentum_op.json
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/resources/dipole_moment_ops.json
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/resources/electronic_energy_op.json
--rw-r--r--   0 runner    (1001) docker     (123)    72011 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/resources/electronic_structure_driver_result.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/test_angular_momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/test_dipole_moment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/test_electronic_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/test_electronic_structure_driver_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/test_magnetization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/electronic/test_particle_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/test_second_quantized_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_basis_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_basis_2.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_basis_3.json
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_second_q_op_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_second_q_op_2.json
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_second_q_op_3.json
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/test_harmonic_basis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/resources/vibrational_energy_op.json
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/resources/vibrational_structure_driver_result.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/test_occupied_modals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/test_vibrational_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/test_vibrational_structure_driver_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/properties/test_grouped_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/resources/test_hdf5_error_import_failure.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/resources/test_hdf5_error_missing_class.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/resources/test_hdf5_error_multiple_groups.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/resources/test_hdf5_error_non_native.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/resources/test_hdf5_error_non_protocol.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/results/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/results/test_eigenstate_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/results/test_electronic_structure_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/results/test_protein_folding_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/results/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/results/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/results/utils/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/results/utils/resources/also_side_chains_test.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/results/utils/resources/only_main_chain_test.xyz
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/results/utils/test_protein_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/results/utils/test_protein_shape_file_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/runtime/fake_vqeruntime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/runtime/test_vqeprogram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/eigensolver_factories/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/eigensolver_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/eigensolver_factories/test_numpy_eigensolver_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/resources/expected_qeom_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/resources/expected_transition_amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/test_bosonic_esc_calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/test_excited_states_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/test_excited_states_solvers_auxiliaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/test_qeom_electronic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/test_qeom_vibrational_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_ucc_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_uvcc_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/test_advanced_ucc_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/test_groundstate_eigensolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    15768 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/test_groundstate_eigensolver_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/test_swaprz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/algorithms/initial_points/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/initial_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/initial_points/test_hf_initial_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/initial_points/test_initial_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/initial_points/test_mp2_initial_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/algorithms/initial_points/test_vscf_initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/test_chc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/test_puccd.py
--rw-r--r--   0 runner    (1001) docker     (123)    15295 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/test_succd.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/test_ucc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/test_uccsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/test_uvcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/utils/test_fermionic_excitation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/utils/test_vibration_excitation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/utils/vibrational_op_label_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/initial_states/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/initial_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/initial_states/test_fermionic_gaussian_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/initial_states/test_hartree_fock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/initial_states/test_hartree_fock_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/initial_states/test_slater_determinant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/initial_states/test_vscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/circuit/library/test_bogoliubov_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_forces.py
--rw-r--r--   0 runner    (1001) docker     (123)   940592 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_from_mat.mat
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_from_mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_log_A03.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_log_C01.txt
--rw-r--r--   0 runner    (1001) docker     (123)    90979 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_log_polyyne_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15480 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_log_vibrational_energy.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_methods_gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/drivers/psi4d/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/psi4d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/psi4d/test_driver_methods_psi4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/psi4d/test_driver_psi4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/psi4d/test_driver_psi4_extra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/drivers/pyscfd/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/pyscfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/pyscfd/test_driver_methods_pyscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/pyscfd/test_driver_pyscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/drivers/test_driver_methods_gsc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/formats/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/formats/fcidump/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/fcidump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump.py
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump_h2.fcidump
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump_lih.fcidump
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump_lih.npz
--rw-r--r--   0 runner    (1001) docker     (123)    24914 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump_oh.fcidump
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump_oh.npz
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_methods_fcidump.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/formats/qcschema/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/qcschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/qcschema/he2_energy_VV10_input.json
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/qcschema/he2_energy_VV10_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/qcschema/he2_energy_VV10_output.json
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/qcschema/he2_energy_VV10_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    24880 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/qcschema/legacy_electronic_structure_driver_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/qcschema/water_output.json
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/qcschema/water_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/qcschema/water_output_v3.json
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/qcschema/water_output_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/formats/test_qcschema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/lattices/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/lattices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/lattices/test_hyper_cubic_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/lattices/test_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/lattices/test_line_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/lattices/test_square_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/lattices/test_triangular_lattice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/resources/electronic_energy_op.json
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/test_electronic_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/test_fermi_hubbard_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/test_heisenberg_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/test_ising_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12151 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/test_quadratic_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/hamiltonians/test_vibrational_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/mappers/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/resources/bksf_lih.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/resources/reference_direct_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/test_bksf_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/test_bravyi_kitaev_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/test_direct_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/test_interleaved_qubit_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/test_jordan_wigner_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/test_linear_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/test_logarithmic_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/test_parity_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    27139 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/test_qubit_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    30564 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/mappers/test_tapered_qubit_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/operators/tensor_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/operators/test_commutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19776 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/operators/test_electronic_integrals.py
--rw-r--r--   0 runner    (1001) docker     (123)    26291 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/operators/test_fermionic_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    34652 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/operators/test_polynomial_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18867 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/operators/test_sparse_label_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/operators/test_spin_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/operators/test_symmetric_two_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/operators/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/operators/test_tensor_ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/operators/test_vibrational_op.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/problems/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    23464 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/resources/H2_631g_ferm_op.json
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/resources/H2_631g_ferm_op_active_space.json
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/resources/expected_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/test_eigenstate_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/test_electronic_properties_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/test_electronic_structure_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/test_electronic_structure_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/test_lattice_model_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/test_lattice_properties_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/test_properties_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/test_vibrational_properties_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/problems/test_vibrational_structure_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/properties/property_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/properties/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/properties/resources/angular_momentum_op.json
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/properties/resources/vibrational_energy_op.json
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/properties/test_angular_momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/properties/test_dipole_moment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/properties/test_electronic_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/properties/test_magnetization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/properties/test_occupied_modals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/properties/test_particle_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/second_q/transformers/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    24880 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/transformers/resources/BeH_sto3g_reduced.json
--rw-r--r--   0 runner    (1001) docker     (123)    34241 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/transformers/resources/LiH_sto3g_reduced.json
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/transformers/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/transformers/test_active_space_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/transformers/test_basis_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/transformers/test_freeze_core_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/second_q/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21557 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/test_end2end_with_vqe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/test_readme_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)    87427 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/BeH_sto3g.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    72011 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/BeH_sto3g_reduced.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    68723 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/H2_631g.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    64603 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/H2_sto3g.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    64603 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/H2_sto3g_v2.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    87427 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/LiH_sto3g.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    77027 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/LiH_sto3g_reduced.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/test_active_space_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/test_freeze_core_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:12:08.000000 qiskit-nature-0.6.0/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-14 13:11:53.000000 qiskit-nature-0.6.0/test/utils/test_linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/eigensolver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/numpy_eigensolver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/excited_states_eigensolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/excited_states_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/qeom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/adapt_vqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/ground_state_eigensolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/ground_state_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/minimum_eigensolver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/numpy_minimum_eigensolver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13180 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_ucc_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_uvcc_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/initial_points/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/initial_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/initial_points/hf_initial_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/initial_points/initial_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/initial_points/mp2_initial_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/initial_points/vscf_initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/bopes_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20098 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/extrapolator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/potentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/potentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/potentials/energy_surface_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/potentials/harmonic_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/potentials/morse_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/potentials/potential_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/chc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/puccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/succd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21323 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/ucc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/uccsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/utils/fermionic_excitation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/utils/vibration_excitation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/uvcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/uvccsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/bogoliubov_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/fermionic_gaussian_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/hartree_fock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/slater_determinant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/utils/givens_rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/vscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/converters/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/converters/second_quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21012 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/converters/second_quantization/qubit_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/converters/second_quantization/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/converters/second_quantization/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/converters/second_quantization/utils/list_or_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/bosonic_bases/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/bosonic_bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/bosonic_bases/bosonic_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/bosonic_bases/harmonic_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18545 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33098 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/qmolecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/base_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/electronic_structure_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/electronic_structure_molecule_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/fcidumpd/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/fcidumpd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/fcidumpd/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/fcidumpd/fcidumpdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/fcidumpd/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12784 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27815 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/QCMatEl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18069 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/QCOpMat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33018 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.F
+-rw-r--r--   0 runner    (1001) docker     (123)   132096 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cp310-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (123)   125952 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cp37-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (123)   126464 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cp38-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (123)   129024 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cp39-win_amd64.pyd
+-rwxr-xr-x   0 runner    (1001) docker     (123)   556024 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-310-darwin.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   420344 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-310-x86_64-linux-gnu.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   481832 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-37m-darwin.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   452040 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-37m-x86_64-linux-gnu.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   481976 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-38-darwin.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   489696 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   525864 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-39-darwin.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   242888 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_forces_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_log_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_log_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gaussiandriver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/hdf5d/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/hdf5d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/hdf5d/hdf5driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/psi4d/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/psi4d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/psi4d/_template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/psi4d/psi4driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/pyquanted/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/pyquanted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/pyquanted/pyquantedriver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/pyscfd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/pyscfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27394 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/pyscfd/pyscfdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/vibrational_structure_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/vibrational_structure_molecule_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/units_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/drivers/watson_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/list_or_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22722 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/bksf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/bravyi_kitaev_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/direct_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/fermionic_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/jordan_wigner_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/linear_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/logarithmic_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/parity_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/qubit_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/spin_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/vibrational_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27314 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/fermionic_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/quadratic_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/second_quantized_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21402 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/spin_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23187 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/vibrational_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/optionals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/bead_contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/bead_contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/bead_contacts/contact_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/bead_contacts/contact_map_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/bead_distances/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/bead_distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/bead_distances/distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/bead_distances/distance_map_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/data_loaders/energy_matrix_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/exceptions/invalid_residue_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/exceptions/invalid_side_chain_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/exceptions/invalid_size_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/mixed_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/miyazawa_jernigan_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/random_interaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/resources/mj_matrix.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/penalty_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/beads/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/beads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/beads/base_bead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/beads/main_bead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/beads/side_bead.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/chains/base_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/chains/main_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/chains/side_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/pauli_ops_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/peptide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/protein_folding_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20630 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/qubit_op_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/qubit_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/qubit_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/qubit_utils/qubit_fixing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/qubit_utils/qubit_number_reducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/residue_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/sampling/sampling_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/base_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/electronic/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/electronic/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/electronic/builders/hopping_ops_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/electronic/electronic_structure_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattice_model_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/boundary_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/hyper_cubic_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/line_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/square_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10928 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/triangular_lattice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/models/fermi_hubbard_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/models/ising_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/models/lattice_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/vibrational/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/vibrational/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/vibrational/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/vibrational/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/vibrational/builders/hopping_ops_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/vibrational/builders/vibrational_label_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/vibrational/vibrational_structure_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/grouped_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/driver_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/angular_momentum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/bases/electronic_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/bases/electronic_basis_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/dipole_moment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/electronic_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/electronic_structure_driver_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/integrals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/integrals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17698 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/integrals/electronic_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/integrals/integral_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/integrals/one_body_electronic_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/integrals/two_body_electronic_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/magnetization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/particle_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/second_quantized_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/bases/harmonic_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/bases/vibrational_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/integrals/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/integrals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/integrals/vibrational_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/occupied_modals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/vibrational_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/vibrational_structure_driver_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/results/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/results/bopes_sampler_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/results/eigenstate_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/results/electronic_structure_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/results/lattice_model_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/results/protein_folding_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/results/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/results/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/results/utils/protein_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/results/utils/protein_shape_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/results/utils/protein_shape_file_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/results/vibrational_structure_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/runtime/vqe_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/eigensolver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/numpy_eigensolver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/excited_states_eigensolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/excited_states_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55023 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/qeom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/qeom_electronic_ops_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/qeom_vibrational_ops_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/ground_state_eigensolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/ground_state_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/minimum_eigensolver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/numpy_minimum_eigensolver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_ucc_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_uvcc_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/initial_points/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/initial_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/initial_points/hf_initial_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/initial_points/initial_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/initial_points/mp2_initial_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/initial_points/vscf_initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/chc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/puccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/succd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/ucc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/uccsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/utils/fermionic_excitation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/utils/vibration_excitation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17251 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/uvcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/uvccsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/bogoliubov_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/fermionic_gaussian_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/hartree_fock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/slater_determinant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/utils/givens_rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/vscf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/base_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/electronic_structure_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12784 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27815 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/QCMatEl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18069 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/QCOpMat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33018 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.F
+-rw-r--r--   0 runner    (1001) docker     (123)   132096 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cp310-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (123)   129536 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cp311-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (123)   125952 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cp37-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (123)   126464 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cp38-win_amd64.pyd
+-rw-r--r--   0 runner    (1001) docker     (123)   129024 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cp39-win_amd64.pyd
+-rwxr-xr-x   0 runner    (1001) docker     (123)   556024 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-310-darwin.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   420344 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-310-x86_64-linux-gnu.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   167328 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-311-darwin.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   413656 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-311-x86_64-linux-gnu.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   481832 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-37m-darwin.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   452040 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-37m-x86_64-linux-gnu.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   481976 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-38-darwin.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   489696 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   525864 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-39-darwin.so
+-rwxr-xr-x   0 runner    (1001) docker     (123)   242888 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gaussian_forces_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gaussian_log_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gaussian_log_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gaussian_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19213 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gaussiandriver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/psi4d/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/psi4d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/psi4d/_template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/psi4d/psi4driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/pyscfd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/pyscfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/pyscfd/pyscfdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/vibrational_structure_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/fcidump/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/fcidump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/fcidump/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/fcidump/fcidump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/fcidump/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/fcidump_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/molecule_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_basis_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14946 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_schema_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_wavefunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema_translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/watson/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/watson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/watson/watson_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/formats/watson_translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/electronic_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/fermi_hubbard_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/heisenberg_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/ising_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattice_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/boundary_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/hyper_cubic_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/line_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/square_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/triangular_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/quadratic_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/vibrational_energy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22931 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/bksf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/bravyi_kitaev_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/direct_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/fermionic_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/interleaved_qubit_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/jordan_wigner_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/linear_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/logarithmic_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/parity_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26859 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/qubit_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/qubit_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/spin_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/tapered_qubit_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/vibrational_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/_bits_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/commutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27586 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/electronic_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25398 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/fermionic_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27244 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/polynomial_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20279 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/sparse_label_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/spin_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/symmetric_two_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25683 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/tensor_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/vibrational_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/operators/vibrational_op.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/base_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/eigenstate_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/electronic_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/electronic_properties_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16006 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/electronic_structure_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19107 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/electronic_structure_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/harmonic_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/lattice_model_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/lattice_model_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/lattice_properties_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/properties_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/vibrational_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/vibrational_properties_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/vibrational_structure_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/problems/vibrational_structure_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/properties/angular_momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/properties/dipole_moment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/properties/electronic_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/properties/magnetization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/properties/occupied_modals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/properties/particle_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/properties/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/transformers/active_space_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/transformers/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/transformers/basis_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/second_q/transformers/freeze_core_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/testing/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/transformers/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/transformers/second_quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/transformers/second_quantization/base_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/transformers/second_quantization/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/transformers/second_quantization/electronic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/transformers/second_quantization/electronic/active_space_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/transformers/second_quantization/electronic/freeze_core_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/utils/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/utils/opt_einsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/qiskit_nature/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    57099 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/qiskit_nature.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/algorithms/excited_state_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/excited_state_solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/algorithms/excited_state_solvers/eigensolver_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/excited_state_solvers/eigensolver_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/excited_state_solvers/eigensolver_factories/test_numpy_eigensolver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/excited_state_solvers/test_bosonic_esc_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/excited_state_solvers/test_excited_states_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/minimum_eigensolver_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/minimum_eigensolver_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_ucc_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_uvcc_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/test_adapt_vqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/test_advanced_ucc_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27402 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/test_groundstate_eigensolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/test_swaprz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/algorithms/initial_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/initial_points/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/algorithms/initial_points/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/initial_points/resources/test_mp2_initial_point.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/initial_points/test_hf_initial_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/initial_points/test_initial_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/initial_points/test_mp2_initial_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/initial_points/test_vscf_initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/algorithms/pes_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/pes_samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/algorithms/pes_samplers/potentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/pes_samplers/potentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/pes_samplers/potentials/test_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/pes_samplers/test_bopes_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/algorithms/pes_samplers/test_extrapolators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/circuit/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/test_chc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/test_puccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/test_succd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/test_ucc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/test_uccsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/test_uvcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/utils/test_fermionic_excitation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/utils/test_vibration_excitation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/ansatzes/utils/vibrational_op_label_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/circuit/library/initial_states/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/initial_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/initial_states/test_fermionic_gaussian_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/initial_states/test_hartree_fock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/initial_states/test_slater_determinant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/initial_states/test_vscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/circuit/library/test_bogoliubov_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/converters/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/converters/second_quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/converters/second_quantization/test_qubit_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_h2.fcidump
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_lih.fcidump
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_lih.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    24909 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_oh.fcidump
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_oh.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_methods_fcidump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_forces.py
+-rw-r--r--   0 runner    (1001) docker     (123)   940592 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_from_mat.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_from_mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log_A03.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log_C01.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log_vibrational_energy.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_methods_gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/hdf5d/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/hdf5d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48547 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/hdf5d/test_driver_hdf5.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/hdf5d/test_driver_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/hdf5d/test_driver_hdf5_legacy.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/psi4d/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/psi4d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/psi4d/test_driver_methods_psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/psi4d/test_driver_psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/psi4d/test_driver_psi4_extra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/pyquanted/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/pyquanted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/pyquanted/test_driver_methods_pyquante.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/pyquanted/test_driver_pyquante.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/pyscfd/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/pyscfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/pyscfd/test_driver_methods_pyscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/pyscfd/test_driver_pyscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/test_driver_methods_gsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/test_driver_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/drivers/second_quantization/test_molecule_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/mappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/resources/bksf_lih.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/resources/reference_direct_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/test_bksf_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/test_bravyi_kitaev_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/test_direct_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/test_jordan_wigner_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/test_linear_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/test_logarithmic_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/mappers/second_quantization/test_parity_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/nature_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/operators/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/operators/second_quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24378 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/operators/second_quantization/test_fermionic_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/operators/second_quantization/test_quadratic_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/operators/second_quantization/test_spin_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/operators/second_quantization/test_vibrational_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/operators/second_quantization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/bead_contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/bead_contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/bead_contacts/test_contact_map_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/bead_distances/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/bead_distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/bead_distances/test_distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/bead_distances/test_distance_map_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/data_loaders/test_energy_matrix_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/interactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/interactions/test_mixed_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/interactions/test_miyazawa_jernigan_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/interactions/test_random_interaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/beads/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/beads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/beads/test_bead_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/beads/test_bead_side.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/chains/test_chain_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/chains/test_chain_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/test_peptide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/qubit_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/qubit_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/qubit_utils/test_qubit_fixing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/qubit_utils/test_qubit_number_reducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_bead_main/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_bead_main/test_main_bead_constructor_expected_indic_0
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_bead_main/test_main_bead_constructor_expected_indic_1
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_bead_main/test_main_bead_constructor_expected_indic_2
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_bead_main/test_main_bead_constructor_expected_indic_3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_bead_side/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_bead_side/test_side_bead_constructor_expected_indic_0
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_bead_side/test_side_bead_constructor_expected_indic_1
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_bead_side/test_side_bead_constructor_expected_indic_2
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_bead_side/test_side_bead_constructor_expected_indic_3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_contact_map_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_2_expected_1
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_2_expected_2
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_3_expected_1
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_3_expected_2
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_3_expected_3
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_3_expected_4
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_3_expected_5
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_contact_map_builder/test_create_pauli_for_contacts_3_expected_6
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map/test_first_neighbor
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map/test_first_neighbor_side
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map/test_second_neighbor
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map/test_second_neighbor_2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_add_distances_side_chain
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_calc_distances_main_chain_1
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_calc_distances_main_chain_2
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_calc_distances_main_chain_3
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_calc_distances_main_chain_4
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_calc_total_distances_1
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map_builder/test_calc_total_distances_2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_protein_folding_problem/
+-rw-r--r--   0 runner    (1001) docker     (123)   639850 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_protein_folding_problem/test_protein_folding_problem
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_protein_folding_problem/test_protein_folding_problem_2
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_protein_folding_problem/test_protein_folding_problem_2_second_bead_side_chain
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_build_qubit_op_2_expected
+-rw-r--r--   0 runner    (1001) docker     (123)   294639 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_build_qubit_op_expected
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_check_turns_expected
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_check_turns_expected_t23
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_check_turns_expected_t2s3
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_check_turns_expected_t34
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_check_turns_expected_t3s4s
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_back_expected
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_back_side_chains_expected
+-rw-r--r--   0 runner    (1001) docker     (123)    43153 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbbb_expected
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbsc_and_h_scbb_2_expected
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbsc_and_h_scbb_expected_h_bbsc
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbsc_and_h_scbb_expected_h_scbb
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_chiral_2_expected
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_chiral_expected
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/test_protein_folding_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/sampling/protein_folding/test_qubit_op_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/second_quantization/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/second_quantization/electronic/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/electronic/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/electronic/builders/test_hopping_ops_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/second_quantization/electronic/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/electronic/resources/H2_631g_ferm_op_active_space
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/electronic/resources/H2_631g_ferm_op_one_int
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/electronic/resources/H2_631g_ferm_op_two_ints
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/electronic/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/electronic/resources/resource_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/electronic/test_electronic_structure_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/lattices/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/lattices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/lattices/test_hyper_cubic_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/lattices/test_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/lattices/test_line_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/lattices/test_square_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/lattices/test_triangular_lattice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/models/test_fermi_hubbard_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/models/test_ising_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/lattice/test_lattice_model_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/second_quantization/vibrational/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/vibrational/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/second_quantization/vibrational/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/vibrational/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/vibrational/builders/test_hopping_ops_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/problems/second_quantization/vibrational/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/vibrational/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/vibrational/resources/expected_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/problems/second_quantization/vibrational/test_vibrational_structure_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/property_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/properties/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/resources/integral_property_op.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_second_q_op_alpha_and_beta_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_second_q_op_only_alpha_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_spin_alpha_and_beta_expected.numpy.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_spin_only_alpha_expected.numpy.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/test_integral_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/test_one_body_electronic_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/test_two_body_electronic_integrals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/resources/angular_momentum_op.json
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/resources/dipole_moment_ops.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/resources/electronic_energy_op.json
+-rw-r--r--   0 runner    (1001) docker     (123)    72011 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/resources/electronic_structure_driver_result.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/test_angular_momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/test_dipole_moment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/test_electronic_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/test_electronic_structure_driver_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/test_magnetization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/electronic/test_particle_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/test_second_quantized_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_basis_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_basis_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_basis_3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_second_q_op_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_second_q_op_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_second_q_op_3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/test_harmonic_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/resources/vibrational_energy_op.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/resources/vibrational_structure_driver_result.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/test_occupied_modals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/test_vibrational_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/test_vibrational_structure_driver_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/properties/test_grouped_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/resources/test_hdf5_error_import_failure.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/resources/test_hdf5_error_missing_class.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/resources/test_hdf5_error_multiple_groups.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/resources/test_hdf5_error_non_native.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/resources/test_hdf5_error_non_protocol.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/results/test_eigenstate_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/results/test_electronic_structure_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/results/test_protein_folding_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/results/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/results/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/results/utils/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/results/utils/resources/also_side_chains_test.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/results/utils/resources/only_main_chain_test.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/results/utils/test_protein_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/results/utils/test_protein_shape_file_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/runtime/fake_vqeruntime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/runtime/test_vqeprogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/eigensolver_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/eigensolver_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/eigensolver_factories/test_numpy_eigensolver_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/resources/expected_qeom_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/resources/expected_transition_amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/test_bosonic_esc_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/test_excited_states_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/test_excited_states_solvers_auxiliaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/test_qeom_electronic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/test_qeom_vibrational_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_ucc_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_uvcc_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/test_advanced_ucc_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/test_groundstate_eigensolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15768 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/test_groundstate_eigensolver_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/test_swaprz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/algorithms/initial_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/initial_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/initial_points/test_hf_initial_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/initial_points/test_initial_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/initial_points/test_mp2_initial_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/algorithms/initial_points/test_vscf_initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/test_chc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/test_puccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15295 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/test_succd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/test_ucc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/test_uccsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/test_uvcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/utils/test_fermionic_excitation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/utils/test_vibration_excitation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/utils/vibrational_op_label_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/initial_states/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/initial_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/initial_states/test_fermionic_gaussian_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/initial_states/test_hartree_fock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/initial_states/test_hartree_fock_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/initial_states/test_slater_determinant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/initial_states/test_vscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/circuit/library/test_bogoliubov_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_forces.py
+-rw-r--r--   0 runner    (1001) docker     (123)   940592 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_from_mat.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_from_mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28437 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_log_A03.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_log_C01.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    90979 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_log_polyyne_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15480 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_log_vibrational_energy.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_methods_gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/drivers/psi4d/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/psi4d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/psi4d/test_driver_methods_psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/psi4d/test_driver_psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/psi4d/test_driver_psi4_extra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/drivers/pyscfd/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/pyscfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/pyscfd/test_driver_methods_pyscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/pyscfd/test_driver_pyscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/drivers/test_driver_methods_gsc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/formats/fcidump/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/fcidump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump_h2.fcidump
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump_lih.fcidump
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump_lih.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    24914 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump_oh.fcidump
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump_oh.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_methods_fcidump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/formats/qcschema/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/qcschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/qcschema/he2_energy_VV10_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/qcschema/he2_energy_VV10_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/qcschema/he2_energy_VV10_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/qcschema/he2_energy_VV10_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24880 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/qcschema/legacy_electronic_structure_driver_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/qcschema/water_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/qcschema/water_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/qcschema/water_output_v3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/qcschema/water_output_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/formats/test_qcschema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/lattices/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/lattices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/lattices/test_hyper_cubic_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/lattices/test_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/lattices/test_line_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/lattices/test_square_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/lattices/test_triangular_lattice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/resources/electronic_energy_op.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/test_electronic_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/test_fermi_hubbard_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/test_heisenberg_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/test_ising_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12151 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/test_quadratic_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/hamiltonians/test_vibrational_energy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/mappers/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/resources/bksf_lih.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/resources/reference_direct_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/test_bksf_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/test_bravyi_kitaev_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/test_direct_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/test_interleaved_qubit_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/test_jordan_wigner_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/test_linear_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/test_logarithmic_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/test_parity_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27139 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/test_qubit_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30564 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/mappers/test_tapered_qubit_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/operators/tensor_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/operators/test_commutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19776 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/operators/test_electronic_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26291 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/operators/test_fermionic_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34652 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/operators/test_polynomial_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18867 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/operators/test_sparse_label_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/operators/test_spin_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/operators/test_symmetric_two_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/operators/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/operators/test_tensor_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/operators/test_vibrational_op.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/problems/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    23464 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/resources/H2_631g_ferm_op.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/resources/H2_631g_ferm_op_active_space.json
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/resources/expected_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/test_eigenstate_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/test_electronic_properties_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/test_electronic_structure_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/test_electronic_structure_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/test_lattice_model_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/test_lattice_properties_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/test_properties_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/test_vibrational_properties_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/problems/test_vibrational_structure_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/properties/property_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/properties/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/properties/resources/angular_momentum_op.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/properties/resources/vibrational_energy_op.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/properties/test_angular_momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/properties/test_dipole_moment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/properties/test_electronic_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/properties/test_magnetization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/properties/test_occupied_modals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/properties/test_particle_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/second_q/transformers/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    24880 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/transformers/resources/BeH_sto3g_reduced.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34241 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/transformers/resources/LiH_sto3g_reduced.json
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/transformers/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/transformers/test_active_space_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/transformers/test_basis_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/transformers/test_freeze_core_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/second_q/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21557 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/test_end2end_with_vqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/test_readme_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)    87427 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/BeH_sto3g.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    72011 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/BeH_sto3g_reduced.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    68723 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/H2_631g.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    64603 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/H2_sto3g.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    64603 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/H2_sto3g_v2.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    87427 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/LiH_sto3g.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    77027 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/LiH_sto3g_reduced.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/test_active_space_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/test_freeze_core_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:14:01.000000 qiskit-nature-0.6.1/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-17 13:13:46.000000 qiskit-nature-0.6.1/test/utils/test_linalg.py
```

### Comparing `qiskit-nature-0.6.0/LICENSE.txt` & `qiskit-nature-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/PKG-INFO` & `qiskit-nature-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-nature
-Version: 0.6.0
+Version: 0.6.1
 Summary: Qiskit Nature: A library of quantum computing chemistry/physics experiments
 Home-page: https://github.com/Qiskit/qiskit-nature
 Author: Qiskit Nature Development Team
 Author-email: hello@qiskit.org
 License: Apache-2.0
 Keywords: qiskit sdk quantum nature chemistry physics
 Classifier: Environment :: Console
@@ -112,16 +112,18 @@
 
 ## Authors and Citation
 
 Qiskit Nature was inspired, authored and brought about by the collective work of a team of researchers.
 Qiskit Nature continues to grow with the help and work of
 [many people](https://github.com/Qiskit/qiskit-nature/graphs/contributors), who contribute
 to the project at different levels.
-If you use Qiskit, please cite as per the provided
-[BibTeX file](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).
+If you use Qiskit Nature, please cite the following references:
+
+- Qiskit, as per the provided [BibTeX file](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).
+- Qiskit Nature, as per https://doi.org/10.5281/zenodo.7828767
 
 Please note that if you do not like the way your name is cited in the BibTex file then consult
 the information found in the [.mailmap](https://github.com/Qiskit/qiskit-nature/blob/main/.mailmap)
 file.
 
 ## License
```

### Comparing `qiskit-nature-0.6.0/README.md` & `qiskit-nature-0.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -81,16 +81,18 @@
 
 ## Authors and Citation
 
 Qiskit Nature was inspired, authored and brought about by the collective work of a team of researchers.
 Qiskit Nature continues to grow with the help and work of
 [many people](https://github.com/Qiskit/qiskit-nature/graphs/contributors), who contribute
 to the project at different levels.
-If you use Qiskit, please cite as per the provided
-[BibTeX file](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).
+If you use Qiskit Nature, please cite the following references:
+
+- Qiskit, as per the provided [BibTeX file](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).
+- Qiskit Nature, as per https://doi.org/10.5281/zenodo.7828767
 
 Please note that if you do not like the way your name is cited in the BibTex file then consult
 the information found in the [.mailmap](https://github.com/Qiskit/qiskit-nature/blob/main/.mailmap)
 file.
 
 ## License
```

### Comparing `qiskit-nature-0.6.0/qiskit_nature/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/eigensolver_factory.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/eigensolver_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/numpy_eigensolver_factory.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/eigensolver_factories/numpy_eigensolver_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/excited_states_eigensolver.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/excited_states_eigensolver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/excited_states_solver.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/excited_states_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/excited_states_solvers/qeom.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/excited_states_solvers/qeom.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/adapt_vqe.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/adapt_vqe.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/ground_state_eigensolver.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/ground_state_eigensolver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/ground_state_solver.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/ground_state_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/minimum_eigensolver_factory.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/minimum_eigensolver_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/numpy_minimum_eigensolver_factory.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/numpy_minimum_eigensolver_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_ucc_factory.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_ucc_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_uvcc_factory.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_uvcc_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/initial_points/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/initial_points/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/initial_points/hf_initial_point.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/initial_points/hf_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/initial_points/initial_point.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/initial_points/initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/initial_points/mp2_initial_point.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/initial_points/mp2_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/initial_points/vscf_initial_point.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/initial_points/vscf_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/bopes_sampler.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/bopes_sampler.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/extrapolator.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/extrapolator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/potentials/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/potentials/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/potentials/energy_surface_spline.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/potentials/energy_surface_spline.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/potentials/harmonic_potential.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/potentials/harmonic_potential.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/potentials/morse_potential.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/potentials/morse_potential.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/algorithms/pes_samplers/potentials/potential_base.py` & `qiskit-nature-0.6.1/qiskit_nature/algorithms/pes_samplers/potentials/potential_base.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/chc.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/chc.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/puccd.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/puccd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/succd.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/succd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/ucc.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/ucc.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/uccsd.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/uccsd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/utils/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/utils/fermionic_excitation_generator.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/utils/fermionic_excitation_generator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/utils/vibration_excitation_generator.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/utils/vibration_excitation_generator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/uvcc.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/uvcc.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/ansatzes/uvccsd.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/ansatzes/uvccsd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/bogoliubov_transform.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/bogoliubov_transform.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/fermionic_gaussian_state.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/fermionic_gaussian_state.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/hartree_fock.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/hartree_fock.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/slater_determinant.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/slater_determinant.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/utils/givens_rotations.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/utils/givens_rotations.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/circuit/library/initial_states/vscf.py` & `qiskit-nature-0.6.1/qiskit_nature/circuit/library/initial_states/vscf.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/constants.py` & `qiskit-nature-0.6.1/qiskit_nature/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/converters/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/converters/second_quantization/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/converters/second_quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/converters/second_quantization/qubit_converter.py` & `qiskit-nature-0.6.1/qiskit_nature/converters/second_quantization/qubit_converter.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/converters/second_quantization/utils/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/converters/second_quantization/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/converters/second_quantization/utils/list_or_dict.py` & `qiskit-nature-0.6.1/qiskit_nature/converters/second_quantization/utils/list_or_dict.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/deprecation.py` & `qiskit-nature-0.6.1/qiskit_nature/deprecation.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/bosonic_bases/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/bosonic_bases/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/bosonic_bases/bosonic_basis.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/bosonic_bases/bosonic_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/bosonic_bases/harmonic_basis.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/bosonic_bases/harmonic_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/molecule.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/molecule.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/qmolecule.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/qmolecule.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/base_driver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/base_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/electronic_structure_driver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/electronic_structure_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/electronic_structure_molecule_driver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/electronic_structure_molecule_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/fcidumpd/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/fcidumpd/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/fcidumpd/dumper.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/fcidumpd/dumper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/fcidumpd/fcidumpdriver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/fcidumpd/fcidumpdriver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/fcidumpd/parser.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/fcidumpd/parser.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/LICENSE.txt` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/QCMatEl.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/QCMatEl.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/QCOpMat.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/QCOpMat.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.F` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.F`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-310-darwin.so` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-310-x86_64-linux-gnu.so` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-37m-darwin.so` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-37m-darwin.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-37m-x86_64-linux-gnu.so` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-38-darwin.so` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-38-x86_64-linux-gnu.so` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-38-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-39-darwin.so` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-39-darwin.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-39-x86_64-linux-gnu.so` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gauopen/qcmatrixio.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_forces_driver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_forces_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_log_driver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_log_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_log_result.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_log_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_utils.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gaussian_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/gaussiand/gaussiandriver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/gaussiand/gaussiandriver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/hdf5d/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/hdf5d/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/hdf5d/hdf5driver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/hdf5d/hdf5driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/psi4d/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/psi4d/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/psi4d/_template.txt` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/psi4d/_template.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/psi4d/psi4driver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/psi4d/psi4driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/pyquanted/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/pyquanted/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/pyquanted/pyquantedriver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/pyquanted/pyquantedriver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/pyscfd/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/pyscfd/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/pyscfd/pyscfdriver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/pyscfd/pyscfdriver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/vibrational_structure_driver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/vibrational_structure_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/second_quantization/vibrational_structure_molecule_driver.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/second_quantization/vibrational_structure_molecule_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/units_type.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/units_type.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/drivers/watson_hamiltonian.py` & `qiskit-nature-0.6.1/qiskit_nature/drivers/watson_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/exceptions.py` & `qiskit-nature-0.6.1/qiskit_nature/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/hdf5.py` & `qiskit-nature-0.6.1/qiskit_nature/hdf5.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/list_or_dict.py` & `qiskit-nature-0.6.1/qiskit_nature/list_or_dict.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/logging.py` & `qiskit-nature-0.6.1/qiskit_nature/logging.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/bksf.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/bksf.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/bravyi_kitaev_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/bravyi_kitaev_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/direct_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/direct_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/fermionic_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/fermionic_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/jordan_wigner_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/jordan_wigner_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/linear_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/linear_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/logarithmic_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/logarithmic_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/parity_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/parity_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/qubit_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/qubit_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/spin_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/spin_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/mappers/second_quantization/vibrational_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/mappers/second_quantization/vibrational_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/operators/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/fermionic_op.py` & `qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/fermionic_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/quadratic_hamiltonian.py` & `qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/quadratic_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/second_quantized_op.py` & `qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/second_quantized_op.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2021, 2022.
+# (C) Copyright IBM 2021, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -32,14 +32,15 @@
     @abstractmethod
     def register_length(self) -> int:
         """Getter for the length of the particle register that the SumOp acts on."""
         raise NotImplementedError
 
     def __pow__(self, power):
         if power == 0:
+            # pylint: disable=too-many-function-args
             return self.__class__("I" * self.register_length)
 
         return super().__pow__(power)
 
     @abstractmethod
     def simplify(self, atol: Optional[float] = None):
         """Simplify the operator.
```

### Comparing `qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/spin_op.py` & `qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/spin_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/operators/second_quantization/vibrational_op.py` & `qiskit-nature-0.6.1/qiskit_nature/operators/second_quantization/vibrational_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/optionals.py` & `qiskit-nature-0.6.1/qiskit_nature/optionals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/bead_contacts/contact_map.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/bead_contacts/contact_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/bead_contacts/contact_map_builder.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/bead_contacts/contact_map_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/bead_distances/distance_map.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/bead_distances/distance_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/bead_distances/distance_map_builder.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/bead_distances/distance_map_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/data_loaders/energy_matrix_loader.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/data_loaders/energy_matrix_loader.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/exceptions/invalid_residue_exception.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/exceptions/invalid_residue_exception.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/exceptions/invalid_side_chain_exception.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/exceptions/invalid_side_chain_exception.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/exceptions/invalid_size_exception.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/exceptions/invalid_size_exception.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/interaction.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/interaction.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/mixed_interaction.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/mixed_interaction.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/miyazawa_jernigan_interaction.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/miyazawa_jernigan_interaction.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/random_interaction.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/random_interaction.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/resources/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/interactions/resources/mj_matrix.txt` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/interactions/resources/mj_matrix.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/penalty_parameters.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/penalty_parameters.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/beads/base_bead.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/beads/base_bead.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/beads/main_bead.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/beads/main_bead.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/beads/side_bead.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/beads/side_bead.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/chains/base_chain.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/chains/base_chain.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/chains/main_chain.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/chains/main_chain.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/chains/side_chain.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/chains/side_chain.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/pauli_ops_builder.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/pauli_ops_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/peptide/peptide.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/peptide/peptide.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/protein_folding_problem.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/protein_folding_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/qubit_op_builder.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/qubit_op_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/qubit_utils/qubit_fixing.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/qubit_utils/qubit_fixing.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/qubit_utils/qubit_number_reducer.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/qubit_utils/qubit_number_reducer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/protein_folding/residue_validator.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/protein_folding/residue_validator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/sampling/sampling_problem.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/sampling/sampling_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/base_problem.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/base_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/electronic/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/electronic/builders/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/electronic/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/electronic/builders/hopping_ops_builder.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/electronic/builders/hopping_ops_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/electronic/electronic_structure_problem.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/electronic/electronic_structure_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattice_model_problem.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattice_model_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/boundary_condition.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/boundary_condition.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/hyper_cubic_lattice.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/hyper_cubic_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/lattice.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/line_lattice.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/line_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/square_lattice.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/square_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/lattices/triangular_lattice.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/lattices/triangular_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/models/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/models/fermi_hubbard_model.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/models/fermi_hubbard_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/models/ising_model.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/models/ising_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/lattice/models/lattice_model.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/lattice/models/lattice_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/vibrational/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/vibrational/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/vibrational/builders/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/vibrational/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/vibrational/builders/hopping_ops_builder.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/vibrational/builders/hopping_ops_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/vibrational/builders/vibrational_label_builder.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/vibrational/builders/vibrational_label_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/problems/second_quantization/vibrational/vibrational_structure_problem.py` & `qiskit-nature-0.6.1/qiskit_nature/problems/second_quantization/vibrational/vibrational_structure_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/grouped_property.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/grouped_property.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/property.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/property.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/driver_metadata.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/driver_metadata.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/angular_momentum.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/angular_momentum.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/bases/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/bases/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/bases/electronic_basis.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/bases/electronic_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/bases/electronic_basis_transform.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/bases/electronic_basis_transform.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/dipole_moment.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/dipole_moment.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/electronic_energy.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/electronic_energy.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/electronic_structure_driver_result.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/electronic_structure_driver_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/integrals/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/integrals/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/integrals/electronic_integrals.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/integrals/electronic_integrals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/integrals/integral_property.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/integrals/integral_property.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/integrals/one_body_electronic_integrals.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/integrals/one_body_electronic_integrals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/integrals/two_body_electronic_integrals.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/integrals/two_body_electronic_integrals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/magnetization.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/magnetization.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/particle_number.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/particle_number.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/electronic/types.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/electronic/types.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/second_quantized_property.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/second_quantized_property.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/bases/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/bases/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/bases/harmonic_basis.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/bases/harmonic_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/bases/vibrational_basis.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/bases/vibrational_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/integrals/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/integrals/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/integrals/vibrational_integrals.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/integrals/vibrational_integrals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/occupied_modals.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/occupied_modals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/types.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/types.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/vibrational_energy.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/vibrational_energy.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/properties/second_quantization/vibrational/vibrational_structure_driver_result.py` & `qiskit-nature-0.6.1/qiskit_nature/properties/second_quantization/vibrational/vibrational_structure_driver_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/results/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/results/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/results/bopes_sampler_result.py` & `qiskit-nature-0.6.1/qiskit_nature/results/bopes_sampler_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/results/eigenstate_result.py` & `qiskit-nature-0.6.1/qiskit_nature/results/eigenstate_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/results/electronic_structure_result.py` & `qiskit-nature-0.6.1/qiskit_nature/results/electronic_structure_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/results/lattice_model_result.py` & `qiskit-nature-0.6.1/qiskit_nature/results/lattice_model_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/results/protein_folding_result.py` & `qiskit-nature-0.6.1/qiskit_nature/results/protein_folding_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/results/utils/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/results/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/results/utils/protein_plotter.py` & `qiskit-nature-0.6.1/qiskit_nature/results/utils/protein_plotter.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/results/utils/protein_shape_decoder.py` & `qiskit-nature-0.6.1/qiskit_nature/results/utils/protein_shape_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/results/utils/protein_shape_file_gen.py` & `qiskit-nature-0.6.1/qiskit_nature/results/utils/protein_shape_file_gen.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/results/vibrational_structure_result.py` & `qiskit-nature-0.6.1/qiskit_nature/results/vibrational_structure_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/runtime/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/runtime/vqe_client.py` & `qiskit-nature-0.6.1/qiskit_nature/runtime/vqe_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/eigensolver_factory.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/eigensolver_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/numpy_eigensolver_factory.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/eigensolver_factories/numpy_eigensolver_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/excited_states_eigensolver.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/excited_states_eigensolver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/excited_states_solver.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/excited_states_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/qeom.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/qeom.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/qeom_electronic_ops_builder.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/qeom_electronic_ops_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/excited_states_solvers/qeom_vibrational_ops_builder.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/excited_states_solvers/qeom_vibrational_ops_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/ground_state_eigensolver.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/ground_state_eigensolver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/ground_state_solver.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/ground_state_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/minimum_eigensolver_factory.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/minimum_eigensolver_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/numpy_minimum_eigensolver_factory.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/numpy_minimum_eigensolver_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_ucc_factory.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_ucc_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_uvcc_factory.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/vqe_uvcc_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/initial_points/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/initial_points/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/initial_points/hf_initial_point.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/initial_points/hf_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/initial_points/initial_point.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/initial_points/initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/initial_points/mp2_initial_point.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/initial_points/mp2_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/algorithms/initial_points/vscf_initial_point.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/algorithms/initial_points/vscf_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/chc.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/chc.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/puccd.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/puccd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/succd.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/succd.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from typing import Sequence, cast
 from collections import defaultdict
 
 import itertools
 import logging
 
 from qiskit.circuit import QuantumCircuit
-from qiskit.opflow import PauliSumOp
 from qiskit_nature import QiskitNatureError
 from qiskit_nature.deprecation import deprecate_arguments
 from qiskit_nature.second_q.mappers import QubitConverter, QubitMapper
 
 from qiskit_nature.second_q.operators import FermionicOp
 
 from .ucc import UCC
@@ -145,18 +144,14 @@
         self._invalidate()
         self._mirror = mirror
 
     def _filter_operators(self, operators):
         valid_operators, valid_excitations = [], []
         for op, ex in zip(operators, self._excitations_dict.values()):
             if op is not None:
-                # TODO: remove wrapping into PauliSumOp after the EvolvedOperatorAnsatz supports
-                # SparsePauliOp instances, too: https://github.com/Qiskit/qiskit-terra/pull/9537
-                if not isinstance(op, PauliSumOp):
-                    op = PauliSumOp(op)
                 valid_operators.append(op)
                 valid_excitations.extend(ex)
 
         self._excitation_list = valid_excitations
         self.operators = valid_operators
 
     def generate_excitations(
```

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/ucc.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/ucc.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 import logging
 from functools import partial
 from typing import Callable, Sequence
 
 from qiskit.circuit import QuantumCircuit
 from qiskit.circuit.library import EvolvedOperatorAnsatz
-from qiskit.opflow import PauliSumOp
 
 from qiskit_nature import QiskitNatureError
 from qiskit_nature.deprecation import deprecate_arguments, deprecate_property, warn_deprecated_type
 from qiskit_nature.second_q.mappers import QubitConverter, QubitMapper, TaperedQubitMapper
 from qiskit_nature.second_q.operators import FermionicOp, SparseLabelOp
 
 from .utils.fermionic_excitation_generator import generate_fermionic_excitations
@@ -353,18 +352,14 @@
 
         return super(UCC, self.__class__).operators.__get__(self)
 
     def _filter_operators(self, operators):
         valid_operators, valid_excitations = [], []
         for op, ex in zip(operators, self._excitation_list):
             if op is not None:
-                # TODO: remove wrapping into PauliSumOp after the EvolvedOperatorAnsatz supports
-                # SparsePauliOp instances, too: https://github.com/Qiskit/qiskit-terra/pull/9537
-                if not isinstance(op, PauliSumOp):
-                    op = PauliSumOp(op)
                 valid_operators.append(op)
                 valid_excitations.append(ex)
 
         self._excitation_list = valid_excitations
         self.operators = valid_operators
 
     def _invalidate(self):
```

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/uccsd.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/uccsd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/utils/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/utils/fermionic_excitation_generator.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/utils/fermionic_excitation_generator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/utils/vibration_excitation_generator.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/utils/vibration_excitation_generator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/uvcc.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/uvcc.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 import logging
 from functools import partial
 from typing import Callable, Sequence
 
 from qiskit.circuit import QuantumCircuit
 from qiskit.circuit.library import EvolvedOperatorAnsatz
-from qiskit.opflow import PauliSumOp
 
 from qiskit_nature import QiskitNatureError
 from qiskit_nature.deprecation import deprecate_arguments, deprecate_property, warn_deprecated_type
 from qiskit_nature.second_q.mappers import QubitConverter, QubitMapper, TaperedQubitMapper
 from qiskit_nature.second_q.operators import SparseLabelOp, VibrationalOp
 
 from .utils.vibration_excitation_generator import generate_vibration_excitations
@@ -249,18 +248,14 @@
 
         return super(UVCC, self.__class__).operators.__get__(self)
 
     def _filter_operators(self, operators):
         valid_operators, valid_excitations = [], []
         for op, ex in zip(operators, self._excitation_list):
             if op is not None:
-                # TODO: remove wrapping into PauliSumOp after the EvolvedOperatorAnsatz supports
-                # SparsePauliOp instances, too: https://github.com/Qiskit/qiskit-terra/pull/9537
-                if not isinstance(op, PauliSumOp):
-                    op = PauliSumOp(op)
                 valid_operators.append(op)
                 valid_excitations.append(ex)
 
         self._excitation_list = valid_excitations
         self.operators = valid_operators
 
     def _invalidate(self):
```

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/ansatzes/uvccsd.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/ansatzes/uvccsd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/bogoliubov_transform.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/bogoliubov_transform.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/fermionic_gaussian_state.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/fermionic_gaussian_state.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/hartree_fock.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/hartree_fock.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/slater_determinant.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/slater_determinant.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/utils/givens_rotations.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/utils/givens_rotations.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/circuit/library/initial_states/vscf.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/circuit/library/initial_states/vscf.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/base_driver.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/base_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/electronic_structure_driver.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/electronic_structure_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/LICENSE.txt` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/QCMatEl.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/QCMatEl.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/QCOpMat.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/QCOpMat.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.F` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.F`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-310-darwin.so` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-310-x86_64-linux-gnu.so` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-311-darwin.so` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-311-x86_64-linux-gnu.so` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-311-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-37m-darwin.so` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-37m-darwin.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-37m-x86_64-linux-gnu.so` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-38-darwin.so` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-38-x86_64-linux-gnu.so` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-38-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-39-darwin.so` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-39-darwin.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-39-x86_64-linux-gnu.so` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gauopen/qcmatrixio.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gaussian_forces_driver.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gaussian_forces_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gaussian_log_driver.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gaussian_log_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gaussian_log_result.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gaussian_log_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gaussian_utils.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gaussian_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/gaussiand/gaussiandriver.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/gaussiand/gaussiandriver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/psi4d/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/psi4d/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/psi4d/_template.txt` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/psi4d/_template.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/psi4d/psi4driver.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/psi4d/psi4driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/pyscfd/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/pyscfd/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/pyscfd/pyscfdriver.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/pyscfd/pyscfdriver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/drivers/vibrational_structure_driver.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/drivers/vibrational_structure_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/fcidump/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/fcidump/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/fcidump/dumper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/fcidump/dumper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/fcidump/fcidump.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/fcidump/fcidump.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/fcidump/parser.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/fcidump/parser.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/fcidump_translator.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/fcidump_translator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/molecule_info.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/molecule_info.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_base.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_base.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_basis_set.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_basis_set.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_error.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_error.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_model.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_properties.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_properties.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_provenance.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_provenance.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_schema.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_schema.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_schema_input.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_schema_input.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_topology.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_topology.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema/qc_wavefunction.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema/qc_wavefunction.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/qcschema_translator.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/qcschema_translator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/watson/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/watson/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/watson/watson_hamiltonian.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/watson/watson_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/formats/watson_translator.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/formats/watson_translator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/electronic_energy.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/electronic_energy.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/fermi_hubbard_model.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/fermi_hubbard_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/hamiltonian.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/heisenberg_model.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/heisenberg_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/ising_model.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/ising_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattice_model.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattice_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/boundary_condition.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/boundary_condition.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/hyper_cubic_lattice.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/hyper_cubic_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/lattice.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/line_lattice.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/line_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/square_lattice.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/square_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/lattices/triangular_lattice.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/lattices/triangular_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/quadratic_hamiltonian.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/quadratic_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/hamiltonians/vibrational_energy.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/hamiltonians/vibrational_energy.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/bksf.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/bksf.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/bravyi_kitaev_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/bravyi_kitaev_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/direct_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/direct_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/fermionic_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/fermionic_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/interleaved_qubit_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/interleaved_qubit_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/jordan_wigner_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/jordan_wigner_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/linear_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/linear_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/logarithmic_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/logarithmic_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/parity_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/parity_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/qubit_converter.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/qubit_converter.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/qubit_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/qubit_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,17 +291,17 @@
             # save the respective Pauli string in the pauli_str list.
             for term in terms:
                 char = term[0]
                 if char == "":
                     break
                 position = int(term[1])
                 if char == "+":
-                    ret_op = ret_op.compose(times_creation_op[position], front=True)
+                    ret_op = ret_op.compose(times_creation_op[position], front=True).simplify()
                 elif char == "-":
-                    ret_op = ret_op.compose(times_annihilation_op[position], front=True)
+                    ret_op = ret_op.compose(times_annihilation_op[position], front=True).simplify()
                 # catch any disallowed labels
                 else:
                     raise QiskitNatureError(
                         f"FermionicOp label included '{char}'. Allowed characters: I, N, E, +, -"
                     )
             ret_op_list.append(ret_op)
```

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/spin_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/spin_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/tapered_qubit_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/tapered_qubit_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/mappers/vibrational_mapper.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/mappers/vibrational_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/_bits_container.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/_bits_container.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/commutators.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/commutators.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/electronic_integrals.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/electronic_integrals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/fermionic_op.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/fermionic_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/polynomial_tensor.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/polynomial_tensor.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/sparse_label_op.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/sparse_label_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/spin_op.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/spin_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/symmetric_two_body.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/symmetric_two_body.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/tensor.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/tensor.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/tensor_ordering.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/tensor_ordering.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/vibrational_integrals.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/vibrational_integrals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/operators/vibrational_op.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/operators/vibrational_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/base_problem.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/base_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/eigenstate_result.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/eigenstate_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/electronic_basis.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/electronic_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/electronic_properties_container.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/electronic_properties_container.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/electronic_structure_problem.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/electronic_structure_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,16 @@
         result.combine(eigenstate_result)
         if isinstance(self.hamiltonian, Interpretable):
             self.hamiltonian.interpret(result)
         for prop in self.properties:
             if isinstance(prop, Interpretable):
                 prop.interpret(result)
         result.computed_energies = np.asarray([e.real for e in eigenstate_result.eigenvalues])
+        if self.reference_energy is not None:
+            result.hartree_fock_energy = self.reference_energy
         return result
 
     def get_default_filter_criterion(
         self,
     ) -> Optional[Callable[[Union[List, np.ndarray], float, Optional[List[float]]], bool]]:
         """Returns a default filter criterion method to filter the eigenvalues computed by the
         eigensolver. For more information see also
```

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/electronic_structure_result.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/electronic_structure_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
             )
             lines.append(
                 "  - computed part:      "
                 f"{_complex_to_string(self.computed_energies[0], self.formatting_precision)}"
             )
             for name, value in self.extracted_transformer_energies.items():
                 lines.append(
-                    "  - {name} extracted energy part: "
+                    f"  - {name} extracted energy part: "
                     f"{_complex_to_string(value, self.formatting_precision)}"
                 )
         if self.nuclear_repulsion_energy is not None:
             lines.append(
                 "~ Nuclear repulsion energy (Hartree): "
                 f"{_complex_to_string(self.nuclear_repulsion_energy, self.formatting_precision)}"
             )
```

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/harmonic_basis.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/harmonic_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/lattice_model_problem.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/lattice_model_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/lattice_model_result.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/lattice_model_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/lattice_properties_container.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/lattice_properties_container.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/properties_container.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/properties_container.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/vibrational_basis.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/vibrational_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/vibrational_properties_container.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/vibrational_properties_container.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/vibrational_structure_problem.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/vibrational_structure_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/problems/vibrational_structure_result.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/problems/vibrational_structure_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/properties/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/properties/angular_momentum.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/properties/angular_momentum.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/properties/dipole_moment.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/properties/dipole_moment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2021, 2022.
+# (C) Copyright IBM 2021, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
@@ -30,15 +30,15 @@
 class ElectronicDipoleMoment:
     r"""The ElectronicDipoleMoment property.
 
     This Property implements the operator which evaluates the **electronic** dipole moment, based on
     the electronic integrals:
 
     .. math::
-        \vec{d}_{pq} = \int \phi_{p} \frac{1}{\vec{r}} \phi_{q} ,
+        \vec{d}_{pq} = \int \phi_{p} \vec{r} \phi_{q} ,
 
     where the integral is over the all space. The operator can then be expressed as:
 
     .. math::
         \hat{d} = \sum_{p, q} d^x_{pq} a^\dagger_p a_q ,
 
     where :math:`x` can be any of the three Cartesian axes (:math:`\{x, y, z\}`).
```

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/properties/electronic_density.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/properties/electronic_density.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/properties/magnetization.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/properties/magnetization.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/properties/occupied_modals.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/properties/occupied_modals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/properties/particle_number.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/properties/particle_number.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/properties/protocols.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/properties/protocols.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/transformers/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/transformers/active_space_transformer.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/transformers/active_space_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,16 +245,16 @@
         new_problem.orbital_occupations = np.diag(
             cast(np.ndarray, self._active_density.alpha["+-"])
         )[self._active_orbs_indices]
         new_problem.orbital_occupations_b = np.diag(
             cast(np.ndarray, self._active_density.beta["+-"])
         )[self._active_orbs_indices]
         new_problem.num_particles = (
-            int(sum(new_problem.orbital_occupations)),
-            int(sum(new_problem.orbital_occupations_b)),
+            round(sum(new_problem.orbital_occupations)),
+            round(sum(new_problem.orbital_occupations_b)),
         )
 
         if problem.orbital_energies is not None:
             new_problem.orbital_energies = problem.orbital_energies[self._active_orbs_indices]
         if problem.orbital_energies_b is not None:
             new_problem.orbital_energies_b = problem.orbital_energies_b[self._active_orbs_indices]
```

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/transformers/base_transformer.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/transformers/base_transformer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/transformers/basis_transformer.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/transformers/basis_transformer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/second_q/transformers/freeze_core_transformer.py` & `qiskit-nature-0.6.1/qiskit_nature/second_q/transformers/freeze_core_transformer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/settings.py` & `qiskit-nature-0.6.1/qiskit_nature/settings.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/testing/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/testing/random.py` & `qiskit-nature-0.6.1/qiskit_nature/testing/random.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/transformers/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/transformers/second_quantization/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/transformers/second_quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/transformers/second_quantization/base_transformer.py` & `qiskit-nature-0.6.1/qiskit_nature/transformers/second_quantization/base_transformer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/transformers/second_quantization/electronic/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/transformers/second_quantization/electronic/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/transformers/second_quantization/electronic/active_space_transformer.py` & `qiskit-nature-0.6.1/qiskit_nature/transformers/second_quantization/electronic/active_space_transformer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/transformers/second_quantization/electronic/freeze_core_transformer.py` & `qiskit-nature-0.6.1/qiskit_nature/transformers/second_quantization/electronic/freeze_core_transformer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/units.py` & `qiskit-nature-0.6.1/qiskit_nature/units.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/utils/__init__.py` & `qiskit-nature-0.6.1/qiskit_nature/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/utils/linalg.py` & `qiskit-nature-0.6.1/qiskit_nature/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/utils/opt_einsum.py` & `qiskit-nature-0.6.1/qiskit_nature/utils/opt_einsum.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature/version.py` & `qiskit-nature-0.6.1/qiskit_nature/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/qiskit_nature.egg-info/PKG-INFO` & `qiskit-nature-0.6.1/qiskit_nature.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-nature
-Version: 0.6.0
+Version: 0.6.1
 Summary: Qiskit Nature: A library of quantum computing chemistry/physics experiments
 Home-page: https://github.com/Qiskit/qiskit-nature
 Author: Qiskit Nature Development Team
 Author-email: hello@qiskit.org
 License: Apache-2.0
 Keywords: qiskit sdk quantum nature chemistry physics
 Classifier: Environment :: Console
@@ -112,16 +112,18 @@
 
 ## Authors and Citation
 
 Qiskit Nature was inspired, authored and brought about by the collective work of a team of researchers.
 Qiskit Nature continues to grow with the help and work of
 [many people](https://github.com/Qiskit/qiskit-nature/graphs/contributors), who contribute
 to the project at different levels.
-If you use Qiskit, please cite as per the provided
-[BibTeX file](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).
+If you use Qiskit Nature, please cite the following references:
+
+- Qiskit, as per the provided [BibTeX file](https://github.com/Qiskit/qiskit/blob/master/Qiskit.bib).
+- Qiskit Nature, as per https://doi.org/10.5281/zenodo.7828767
 
 Please note that if you do not like the way your name is cited in the BibTex file then consult
 the information found in the [.mailmap](https://github.com/Qiskit/qiskit-nature/blob/main/.mailmap)
 file.
 
 ## License
```

### Comparing `qiskit-nature-0.6.0/qiskit_nature.egg-info/SOURCES.txt` & `qiskit-nature-0.6.1/qiskit_nature.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/setup.py` & `qiskit-nature-0.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,12 +73,12 @@
     packages=setuptools.find_packages(include=["qiskit_nature", "qiskit_nature.*"]),
     install_requires=REQUIREMENTS,
     include_package_data=True,
     python_requires=">=3.7",
     extras_require={
         "pyscf": ["pyscf; sys_platform != 'win32'"],
         "mpl": ["matplotlib>=3.3"],
-        "sparse": ["sparse; python_version < '3.11'"],
+        "sparse": ["sparse"],
         "opt_einsum": ["opt_einsum"],
     },
     zip_safe=False,
 )
```

### Comparing `qiskit-nature-0.6.0/test/__init__.py` & `qiskit-nature-0.6.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/excited_state_solvers/eigensolver_factories/test_numpy_eigensolver_factory.py` & `qiskit-nature-0.6.1/test/algorithms/excited_state_solvers/eigensolver_factories/test_numpy_eigensolver_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/excited_state_solvers/test_bosonic_esc_calculation.py` & `qiskit-nature-0.6.1/test/algorithms/excited_state_solvers/test_bosonic_esc_calculation.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/excited_state_solvers/test_excited_states_solvers.py` & `qiskit-nature-0.6.1/test/algorithms/excited_state_solvers/test_excited_states_solvers.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_ucc_factory.py` & `qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_ucc_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_uvcc_factory.py` & `qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_uvcc_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/test_adapt_vqe.py` & `qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/test_adapt_vqe.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/test_advanced_ucc_variants.py` & `qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/test_advanced_ucc_variants.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/test_groundstate_eigensolver.py` & `qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/test_groundstate_eigensolver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/ground_state_solvers/test_swaprz.py` & `qiskit-nature-0.6.1/test/algorithms/ground_state_solvers/test_swaprz.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/initial_points/resources/test_mp2_initial_point.json` & `qiskit-nature-0.6.1/test/algorithms/initial_points/resources/test_mp2_initial_point.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/initial_points/test_hf_initial_point.py` & `qiskit-nature-0.6.1/test/algorithms/initial_points/test_hf_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/initial_points/test_initial_point.py` & `qiskit-nature-0.6.1/test/algorithms/initial_points/test_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/initial_points/test_mp2_initial_point.py` & `qiskit-nature-0.6.1/test/algorithms/initial_points/test_mp2_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/initial_points/test_vscf_initial_point.py` & `qiskit-nature-0.6.1/test/algorithms/initial_points/test_vscf_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/pes_samplers/potentials/test_potential.py` & `qiskit-nature-0.6.1/test/algorithms/pes_samplers/potentials/test_potential.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/pes_samplers/test_bopes_sampler.py` & `qiskit-nature-0.6.1/test/algorithms/pes_samplers/test_bopes_sampler.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/algorithms/pes_samplers/test_extrapolators.py` & `qiskit-nature-0.6.1/test/algorithms/pes_samplers/test_extrapolators.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/ansatzes/test_chc.py` & `qiskit-nature-0.6.1/test/circuit/library/ansatzes/test_chc.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/ansatzes/test_puccd.py` & `qiskit-nature-0.6.1/test/circuit/library/ansatzes/test_puccd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/ansatzes/test_succd.py` & `qiskit-nature-0.6.1/test/circuit/library/ansatzes/test_succd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/ansatzes/test_ucc.py` & `qiskit-nature-0.6.1/test/circuit/library/ansatzes/test_ucc.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/ansatzes/test_uccsd.py` & `qiskit-nature-0.6.1/test/circuit/library/ansatzes/test_uccsd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/ansatzes/test_uvcc.py` & `qiskit-nature-0.6.1/test/circuit/library/ansatzes/test_uvcc.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/ansatzes/utils/test_fermionic_excitation_generator.py` & `qiskit-nature-0.6.1/test/circuit/library/ansatzes/utils/test_fermionic_excitation_generator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/ansatzes/utils/test_vibration_excitation_generator.py` & `qiskit-nature-0.6.1/test/circuit/library/ansatzes/utils/test_vibration_excitation_generator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/ansatzes/utils/vibrational_op_label_creator.py` & `qiskit-nature-0.6.1/test/circuit/library/ansatzes/utils/vibrational_op_label_creator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/initial_states/test_fermionic_gaussian_state.py` & `qiskit-nature-0.6.1/test/circuit/library/initial_states/test_fermionic_gaussian_state.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/initial_states/test_hartree_fock.py` & `qiskit-nature-0.6.1/test/circuit/library/initial_states/test_hartree_fock.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/initial_states/test_slater_determinant.py` & `qiskit-nature-0.6.1/test/circuit/library/initial_states/test_slater_determinant.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/initial_states/test_vscf.py` & `qiskit-nature-0.6.1/test/circuit/library/initial_states/test_vscf.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/circuit/library/test_bogoliubov_transform.py` & `qiskit-nature-0.6.1/test/circuit/library/test_bogoliubov_transform.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/converters/second_quantization/test_qubit_converter.py` & `qiskit-nature-0.6.1/test/converters/second_quantization/test_qubit_converter.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_dumper.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_dumper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_lih.fcidump` & `qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_lih.fcidump`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_lih.npz` & `qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_lih.npz`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_oh.fcidump` & `qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_oh.fcidump`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_oh.npz` & `qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_fcidump_oh.npz`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/fcidumpd/test_driver_methods_fcidump.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/fcidumpd/test_driver_methods_fcidump.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_extra.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_extra.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_forces.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_forces.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_from_mat.mat` & `qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_from_mat.mat`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_from_mat.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_from_mat.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log_A03.txt` & `qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log_A03.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log_C01.txt` & `qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log_C01.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log_vibrational_energy.hdf5` & `qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_gaussian_log_vibrational_energy.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/gaussiand/test_driver_methods_gaussian.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/gaussiand/test_driver_methods_gaussian.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/hdf5d/test_driver_hdf5.hdf5` & `qiskit-nature-0.6.1/test/drivers/second_quantization/hdf5d/test_driver_hdf5.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/hdf5d/test_driver_hdf5.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/hdf5d/test_driver_hdf5.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/hdf5d/test_driver_hdf5_legacy.hdf5` & `qiskit-nature-0.6.1/test/drivers/second_quantization/hdf5d/test_driver_hdf5_legacy.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/psi4d/test_driver_methods_psi4.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/psi4d/test_driver_methods_psi4.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/psi4d/test_driver_psi4.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/psi4d/test_driver_psi4.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/psi4d/test_driver_psi4_extra.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/psi4d/test_driver_psi4_extra.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/pyquanted/test_driver_methods_pyquante.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/pyquanted/test_driver_methods_pyquante.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/pyquanted/test_driver_pyquante.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/pyquanted/test_driver_pyquante.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/pyscfd/test_driver_methods_pyscf.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/pyscfd/test_driver_methods_pyscf.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/pyscfd/test_driver_pyscf.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/pyscfd/test_driver_pyscf.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/test_driver.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/test_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/test_driver_methods_gsc.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/test_driver_methods_gsc.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/test_driver_molecule.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/test_driver_molecule.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/drivers/second_quantization/test_molecule_driver.py` & `qiskit-nature-0.6.1/test/drivers/second_quantization/test_molecule_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/mappers/second_quantization/resources/bksf_lih.py` & `qiskit-nature-0.6.1/test/mappers/second_quantization/resources/bksf_lih.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/mappers/second_quantization/resources/reference_direct_mapper.py` & `qiskit-nature-0.6.1/test/mappers/second_quantization/resources/reference_direct_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/mappers/second_quantization/test_bksf_mapper.py` & `qiskit-nature-0.6.1/test/mappers/second_quantization/test_bksf_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/mappers/second_quantization/test_bravyi_kitaev_mapper.py` & `qiskit-nature-0.6.1/test/mappers/second_quantization/test_bravyi_kitaev_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/mappers/second_quantization/test_direct_mapper.py` & `qiskit-nature-0.6.1/test/mappers/second_quantization/test_direct_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/mappers/second_quantization/test_jordan_wigner_mapper.py` & `qiskit-nature-0.6.1/test/mappers/second_quantization/test_jordan_wigner_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/mappers/second_quantization/test_linear_mapper.py` & `qiskit-nature-0.6.1/test/mappers/second_quantization/test_linear_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/mappers/second_quantization/test_logarithmic_mapper.py` & `qiskit-nature-0.6.1/test/mappers/second_quantization/test_logarithmic_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/mappers/second_quantization/test_parity_mapper.py` & `qiskit-nature-0.6.1/test/mappers/second_quantization/test_parity_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/nature_test_case.py` & `qiskit-nature-0.6.1/test/nature_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/operators/second_quantization/test_fermionic_op.py` & `qiskit-nature-0.6.1/test/operators/second_quantization/test_fermionic_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/operators/second_quantization/test_quadratic_hamiltonian.py` & `qiskit-nature-0.6.1/test/operators/second_quantization/test_quadratic_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/operators/second_quantization/test_spin_op.py` & `qiskit-nature-0.6.1/test/operators/second_quantization/test_spin_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/operators/second_quantization/test_vibrational_op.py` & `qiskit-nature-0.6.1/test/operators/second_quantization/test_vibrational_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/operators/second_quantization/utils.py` & `qiskit-nature-0.6.1/test/operators/second_quantization/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/bead_contacts/test_contact_map_builder.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/bead_contacts/test_contact_map_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/bead_distances/test_distance_map.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/bead_distances/test_distance_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/bead_distances/test_distance_map_builder.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/bead_distances/test_distance_map_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/data_loaders/test_energy_matrix_loader.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/data_loaders/test_energy_matrix_loader.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/interactions/test_mixed_interaction.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/interactions/test_mixed_interaction.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/interactions/test_miyazawa_jernigan_interaction.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/interactions/test_miyazawa_jernigan_interaction.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/interactions/test_random_interaction.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/interactions/test_random_interaction.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/beads/test_bead_main.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/beads/test_bead_main.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/beads/test_bead_side.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/beads/test_bead_side.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/chains/test_chain_main.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/chains/test_chain_main.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/chains/test_chain_side.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/chains/test_chain_side.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/peptide/test_peptide.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/peptide/test_peptide.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/qubit_utils/test_qubit_fixing.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/qubit_utils/test_qubit_fixing.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/qubit_utils/test_qubit_number_reducer.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/qubit_utils/test_qubit_number_reducer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/file_parser.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/file_parser.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_distance_map/test_first_neighbor_side` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_distance_map/test_first_neighbor_side`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_protein_folding_problem/test_protein_folding_problem` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_protein_folding_problem/test_protein_folding_problem`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_protein_folding_problem/test_protein_folding_problem_2_second_bead_side_chain` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_protein_folding_problem/test_protein_folding_problem_2_second_bead_side_chain`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_build_qubit_op_2_expected` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_build_qubit_op_2_expected`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_build_qubit_op_expected` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_build_qubit_op_expected`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbbb_expected` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbbb_expected`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbsc_and_h_scbb_2_expected` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbsc_and_h_scbb_2_expected`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbsc_and_h_scbb_expected_h_bbsc` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbsc_and_h_scbb_expected_h_bbsc`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbsc_and_h_scbb_expected_h_scbb` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_bbsc_and_h_scbb_expected_h_scbb`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_chiral_expected` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/resources/test_qubit_op_builder/test_create_h_chiral_expected`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/test_protein_folding_problem.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/test_protein_folding_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/sampling/protein_folding/test_qubit_op_builder.py` & `qiskit-nature-0.6.1/test/problems/sampling/protein_folding/test_qubit_op_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/electronic/builders/test_hopping_ops_builder.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/electronic/builders/test_hopping_ops_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/electronic/resources/H2_631g_ferm_op_active_space` & `qiskit-nature-0.6.1/test/problems/second_quantization/electronic/resources/H2_631g_ferm_op_active_space`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/electronic/resources/H2_631g_ferm_op_two_ints` & `qiskit-nature-0.6.1/test/problems/second_quantization/electronic/resources/H2_631g_ferm_op_two_ints`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/electronic/resources/resource_reader.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/electronic/resources/resource_reader.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/electronic/test_electronic_structure_problem.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/electronic/test_electronic_structure_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/lattice/lattices/test_hyper_cubic_lattice.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/lattice/lattices/test_hyper_cubic_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/lattice/lattices/test_lattice.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/lattice/lattices/test_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/lattice/lattices/test_line_lattice.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/lattice/lattices/test_line_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/lattice/lattices/test_square_lattice.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/lattice/lattices/test_square_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/lattice/lattices/test_triangular_lattice.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/lattice/lattices/test_triangular_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/lattice/models/test_fermi_hubbard_model.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/lattice/models/test_fermi_hubbard_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/lattice/models/test_ising_model.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/lattice/models/test_ising_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/lattice/test_lattice_model_problem.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/lattice/test_lattice_model_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/vibrational/builders/test_hopping_ops_builder.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/vibrational/builders/test_hopping_ops_builder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/vibrational/resources/expected_ops.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/vibrational/resources/expected_ops.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/problems/second_quantization/vibrational/test_vibrational_structure_problem.py` & `qiskit-nature-0.6.1/test/problems/second_quantization/vibrational/test_vibrational_structure_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/property_test.py` & `qiskit-nature-0.6.1/test/properties/property_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/resources/integral_property_op.json` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/resources/integral_property_op.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_second_q_op_alpha_and_beta_expected.json` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_second_q_op_alpha_and_beta_expected.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_second_q_op_only_alpha_expected.json` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_second_q_op_only_alpha_expected.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_spin_alpha_and_beta_expected.numpy.bin` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_spin_alpha_and_beta_expected.numpy.bin`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_spin_only_alpha_expected.numpy.bin` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/resources/two_body_test_to_spin_only_alpha_expected.numpy.bin`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/test_integral_property.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/test_integral_property.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/test_one_body_electronic_integrals.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/test_one_body_electronic_integrals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/integrals/test_two_body_electronic_integrals.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/integrals/test_two_body_electronic_integrals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/resources/angular_momentum_op.json` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/resources/angular_momentum_op.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/resources/electronic_energy_op.json` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/resources/electronic_energy_op.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/resources/electronic_structure_driver_result.hdf5` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/resources/electronic_structure_driver_result.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/test_angular_momentum.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/test_angular_momentum.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/test_dipole_moment.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/test_dipole_moment.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/test_electronic_energy.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/test_electronic_energy.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/test_electronic_structure_driver_result.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/test_electronic_structure_driver_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/test_magnetization.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/test_magnetization.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/electronic/test_particle_number.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/electronic/test_particle_number.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/test_second_quantized_property.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/test_second_quantized_property.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_basis_2.json` & `qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_basis_2.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_second_q_op_2.json` & `qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/resources/test_harmonic_basis_to_second_q_op_2.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/bases/test_harmonic_basis.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/bases/test_harmonic_basis.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/resources/vibrational_energy_op.json` & `qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/resources/vibrational_energy_op.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/resources/vibrational_structure_driver_result.hdf5` & `qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/resources/vibrational_structure_driver_result.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/test_occupied_modals.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/test_occupied_modals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/test_vibrational_energy.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/test_vibrational_energy.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/second_quantization/vibrational/test_vibrational_structure_driver_result.py` & `qiskit-nature-0.6.1/test/properties/second_quantization/vibrational/test_vibrational_structure_driver_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/properties/test_grouped_property.py` & `qiskit-nature-0.6.1/test/properties/test_grouped_property.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/resources/test_hdf5_error_import_failure.hdf5` & `qiskit-nature-0.6.1/test/resources/test_hdf5_error_import_failure.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/resources/test_hdf5_error_missing_class.hdf5` & `qiskit-nature-0.6.1/test/resources/test_hdf5_error_missing_class.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/resources/test_hdf5_error_multiple_groups.hdf5` & `qiskit-nature-0.6.1/test/resources/test_hdf5_error_multiple_groups.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/resources/test_hdf5_error_non_native.hdf5` & `qiskit-nature-0.6.1/test/resources/test_hdf5_error_non_native.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/resources/test_hdf5_error_non_protocol.hdf5` & `qiskit-nature-0.6.1/test/resources/test_hdf5_error_non_protocol.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/results/test_eigenstate_result.py` & `qiskit-nature-0.6.1/test/results/test_eigenstate_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/results/test_electronic_structure_result.py` & `qiskit-nature-0.6.1/test/results/test_electronic_structure_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/results/test_protein_folding_result.py` & `qiskit-nature-0.6.1/test/results/test_protein_folding_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/results/utils/test_protein_decoder.py` & `qiskit-nature-0.6.1/test/results/utils/test_protein_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/results/utils/test_protein_shape_file_gen.py` & `qiskit-nature-0.6.1/test/results/utils/test_protein_shape_file_gen.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/runtime/__init__.py` & `qiskit-nature-0.6.1/test/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/runtime/fake_vqeruntime.py` & `qiskit-nature-0.6.1/test/runtime/fake_vqeruntime.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/runtime/test_vqeprogram.py` & `qiskit-nature-0.6.1/test/runtime/test_vqeprogram.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/eigensolver_factories/test_numpy_eigensolver_factory.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/eigensolver_factories/test_numpy_eigensolver_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/resources/expected_qeom_ops.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/resources/expected_qeom_ops.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/resources/expected_transition_amplitudes.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/resources/expected_transition_amplitudes.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/test_bosonic_esc_calculation.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/test_bosonic_esc_calculation.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/test_excited_states_solvers.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/test_excited_states_solvers.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/test_excited_states_solvers_auxiliaries.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/test_excited_states_solvers_auxiliaries.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/test_qeom_electronic_ops.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/test_qeom_electronic_ops.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/excited_state_solvers/test_qeom_vibrational_ops.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/excited_state_solvers/test_qeom_vibrational_ops.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_ucc_factory.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_ucc_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_uvcc_factory.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/minimum_eigensolver_factories/test_vqe_uvcc_factory.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/test_advanced_ucc_variants.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/test_advanced_ucc_variants.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/test_groundstate_eigensolver.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/test_groundstate_eigensolver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/test_groundstate_eigensolver_mapper.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/test_groundstate_eigensolver_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/ground_state_solvers/test_swaprz.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/ground_state_solvers/test_swaprz.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/initial_points/test_hf_initial_point.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/initial_points/test_hf_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/initial_points/test_initial_point.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/initial_points/test_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/initial_points/test_mp2_initial_point.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/initial_points/test_mp2_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/algorithms/initial_points/test_vscf_initial_point.py` & `qiskit-nature-0.6.1/test/second_q/algorithms/initial_points/test_vscf_initial_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/test_chc.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/test_chc.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/test_puccd.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/test_puccd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/test_succd.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/test_succd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/test_ucc.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/test_ucc.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/test_uccsd.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/test_uccsd.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/test_uvcc.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/test_uvcc.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/utils/test_fermionic_excitation_generator.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/utils/test_fermionic_excitation_generator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/utils/test_vibration_excitation_generator.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/utils/test_vibration_excitation_generator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/ansatzes/utils/vibrational_op_label_creator.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/ansatzes/utils/vibrational_op_label_creator.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/initial_states/test_fermionic_gaussian_state.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/initial_states/test_fermionic_gaussian_state.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/initial_states/test_hartree_fock.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/initial_states/test_hartree_fock.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/initial_states/test_hartree_fock_mapper.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/initial_states/test_hartree_fock_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/initial_states/test_slater_determinant.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/initial_states/test_slater_determinant.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/initial_states/test_vscf.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/initial_states/test_vscf.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/circuit/library/test_bogoliubov_transform.py` & `qiskit-nature-0.6.1/test/second_q/circuit/library/test_bogoliubov_transform.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian.py` & `qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_extra.py` & `qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_extra.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_forces.py` & `qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_forces.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_from_mat.mat` & `qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_from_mat.mat`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_from_mat.py` & `qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_from_mat.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_log.py` & `qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_log.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_log_A03.txt` & `qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_log_A03.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_log_C01.txt` & `qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_log_C01.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_log_polyyne_2.txt` & `qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_log_polyyne_2.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_gaussian_log_vibrational_energy.hdf5` & `qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_gaussian_log_vibrational_energy.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/gaussiand/test_driver_methods_gaussian.py` & `qiskit-nature-0.6.1/test/second_q/drivers/gaussiand/test_driver_methods_gaussian.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/psi4d/test_driver_methods_psi4.py` & `qiskit-nature-0.6.1/test/second_q/drivers/psi4d/test_driver_methods_psi4.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/psi4d/test_driver_psi4.py` & `qiskit-nature-0.6.1/test/second_q/drivers/psi4d/test_driver_psi4.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/psi4d/test_driver_psi4_extra.py` & `qiskit-nature-0.6.1/test/second_q/drivers/psi4d/test_driver_psi4_extra.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/pyscfd/test_driver_methods_pyscf.py` & `qiskit-nature-0.6.1/test/second_q/drivers/pyscfd/test_driver_methods_pyscf.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/pyscfd/test_driver_pyscf.py` & `qiskit-nature-0.6.1/test/second_q/drivers/pyscfd/test_driver_pyscf.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/test_driver.py` & `qiskit-nature-0.6.1/test/second_q/drivers/test_driver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/drivers/test_driver_methods_gsc.py` & `qiskit-nature-0.6.1/test/second_q/drivers/test_driver_methods_gsc.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump.py` & `qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump_dumper.py` & `qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump_dumper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump_lih.fcidump` & `qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump_lih.fcidump`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump_lih.npz` & `qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump_lih.npz`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump_oh.fcidump` & `qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump_oh.fcidump`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_fcidump_oh.npz` & `qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_fcidump_oh.npz`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/fcidump/test_methods_fcidump.py` & `qiskit-nature-0.6.1/test/second_q/formats/fcidump/test_methods_fcidump.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/qcschema/he2_energy_VV10_input.py` & `qiskit-nature-0.6.1/test/second_q/formats/qcschema/he2_energy_VV10_input.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/qcschema/he2_energy_VV10_output.json` & `qiskit-nature-0.6.1/test/second_q/formats/qcschema/he2_energy_VV10_output.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/qcschema/he2_energy_VV10_output.py` & `qiskit-nature-0.6.1/test/second_q/formats/qcschema/he2_energy_VV10_output.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/qcschema/legacy_electronic_structure_driver_result.json` & `qiskit-nature-0.6.1/test/second_q/formats/qcschema/legacy_electronic_structure_driver_result.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/qcschema/water_output.json` & `qiskit-nature-0.6.1/test/second_q/formats/qcschema/water_output.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/qcschema/water_output.py` & `qiskit-nature-0.6.1/test/second_q/formats/qcschema/water_output.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/qcschema/water_output_v3.json` & `qiskit-nature-0.6.1/test/second_q/formats/qcschema/water_output_v3.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/qcschema/water_output_v3.py` & `qiskit-nature-0.6.1/test/second_q/formats/qcschema/water_output_v3.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/formats/test_qcschema.py` & `qiskit-nature-0.6.1/test/second_q/formats/test_qcschema.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/hamiltonians/lattices/test_hyper_cubic_lattice.py` & `qiskit-nature-0.6.1/test/second_q/hamiltonians/lattices/test_hyper_cubic_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/hamiltonians/lattices/test_lattice.py` & `qiskit-nature-0.6.1/test/second_q/hamiltonians/lattices/test_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/hamiltonians/lattices/test_line_lattice.py` & `qiskit-nature-0.6.1/test/second_q/hamiltonians/lattices/test_line_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/hamiltonians/lattices/test_square_lattice.py` & `qiskit-nature-0.6.1/test/second_q/hamiltonians/lattices/test_square_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/hamiltonians/lattices/test_triangular_lattice.py` & `qiskit-nature-0.6.1/test/second_q/hamiltonians/lattices/test_triangular_lattice.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/hamiltonians/resources/electronic_energy_op.json` & `qiskit-nature-0.6.1/test/second_q/hamiltonians/resources/electronic_energy_op.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/hamiltonians/test_electronic_energy.py` & `qiskit-nature-0.6.1/test/second_q/hamiltonians/test_electronic_energy.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/hamiltonians/test_fermi_hubbard_model.py` & `qiskit-nature-0.6.1/test/second_q/hamiltonians/test_fermi_hubbard_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/hamiltonians/test_heisenberg_model.py` & `qiskit-nature-0.6.1/test/second_q/hamiltonians/test_heisenberg_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/hamiltonians/test_ising_model.py` & `qiskit-nature-0.6.1/test/second_q/hamiltonians/test_ising_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/hamiltonians/test_quadratic_hamiltonian.py` & `qiskit-nature-0.6.1/test/second_q/hamiltonians/test_quadratic_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/hamiltonians/test_vibrational_energy.py` & `qiskit-nature-0.6.1/test/second_q/hamiltonians/test_vibrational_energy.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/mappers/resources/bksf_lih.py` & `qiskit-nature-0.6.1/test/second_q/mappers/resources/bksf_lih.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/mappers/resources/reference_direct_mapper.py` & `qiskit-nature-0.6.1/test/second_q/mappers/resources/reference_direct_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/mappers/test_bksf_mapper.py` & `qiskit-nature-0.6.1/test/second_q/mappers/test_bksf_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/mappers/test_bravyi_kitaev_mapper.py` & `qiskit-nature-0.6.1/test/second_q/mappers/test_bravyi_kitaev_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/mappers/test_direct_mapper.py` & `qiskit-nature-0.6.1/test/second_q/mappers/test_direct_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/mappers/test_interleaved_qubit_mapper.py` & `qiskit-nature-0.6.1/test/second_q/mappers/test_interleaved_qubit_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/mappers/test_jordan_wigner_mapper.py` & `qiskit-nature-0.6.1/test/second_q/mappers/test_jordan_wigner_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/mappers/test_linear_mapper.py` & `qiskit-nature-0.6.1/test/second_q/mappers/test_linear_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/mappers/test_logarithmic_mapper.py` & `qiskit-nature-0.6.1/test/second_q/mappers/test_logarithmic_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/mappers/test_parity_mapper.py` & `qiskit-nature-0.6.1/test/second_q/mappers/test_parity_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/mappers/test_qubit_converter.py` & `qiskit-nature-0.6.1/test/second_q/mappers/test_qubit_converter.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/mappers/test_tapered_qubit_mapper.py` & `qiskit-nature-0.6.1/test/second_q/mappers/test_tapered_qubit_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/operators/tensor_test_cases.py` & `qiskit-nature-0.6.1/test/second_q/operators/tensor_test_cases.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/operators/test_commutators.py` & `qiskit-nature-0.6.1/test/second_q/operators/test_commutators.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/operators/test_electronic_integrals.py` & `qiskit-nature-0.6.1/test/second_q/operators/test_electronic_integrals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/operators/test_fermionic_op.py` & `qiskit-nature-0.6.1/test/second_q/operators/test_fermionic_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/operators/test_polynomial_tensor.py` & `qiskit-nature-0.6.1/test/second_q/operators/test_polynomial_tensor.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/operators/test_sparse_label_op.py` & `qiskit-nature-0.6.1/test/second_q/operators/test_sparse_label_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/operators/test_spin_op.py` & `qiskit-nature-0.6.1/test/second_q/operators/test_spin_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/operators/test_symmetric_two_body.py` & `qiskit-nature-0.6.1/test/second_q/operators/test_symmetric_two_body.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/operators/test_tensor.py` & `qiskit-nature-0.6.1/test/second_q/operators/test_tensor.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/operators/test_tensor_ordering.py` & `qiskit-nature-0.6.1/test/second_q/operators/test_tensor_ordering.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/operators/test_vibrational_op.py` & `qiskit-nature-0.6.1/test/second_q/operators/test_vibrational_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/problems/resources/H2_631g_ferm_op.json` & `qiskit-nature-0.6.1/test/second_q/problems/resources/H2_631g_ferm_op.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/problems/resources/H2_631g_ferm_op_active_space.json` & `qiskit-nature-0.6.1/test/second_q/problems/resources/H2_631g_ferm_op_active_space.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/problems/resources/expected_ops.py` & `qiskit-nature-0.6.1/test/second_q/problems/resources/expected_ops.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/problems/test_eigenstate_result.py` & `qiskit-nature-0.6.1/test/second_q/problems/test_eigenstate_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/problems/test_electronic_properties_container.py` & `qiskit-nature-0.6.1/test/second_q/problems/test_electronic_properties_container.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/problems/test_electronic_structure_result.py` & `qiskit-nature-0.6.1/test/second_q/problems/test_electronic_structure_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/problems/test_lattice_model_problem.py` & `qiskit-nature-0.6.1/test/second_q/problems/test_lattice_model_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/problems/test_lattice_properties_container.py` & `qiskit-nature-0.6.1/test/second_q/problems/test_lattice_properties_container.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/problems/test_properties_container.py` & `qiskit-nature-0.6.1/test/second_q/problems/test_properties_container.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/problems/test_vibrational_properties_container.py` & `qiskit-nature-0.6.1/test/second_q/problems/test_vibrational_properties_container.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/problems/test_vibrational_structure_problem.py` & `qiskit-nature-0.6.1/test/second_q/problems/test_vibrational_structure_problem.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/properties/property_test.py` & `qiskit-nature-0.6.1/test/second_q/properties/property_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/properties/resources/angular_momentum_op.json` & `qiskit-nature-0.6.1/test/second_q/properties/resources/angular_momentum_op.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/properties/resources/vibrational_energy_op.json` & `qiskit-nature-0.6.1/test/second_q/properties/resources/vibrational_energy_op.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/properties/test_angular_momentum.py` & `qiskit-nature-0.6.1/test/second_q/properties/test_angular_momentum.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/properties/test_dipole_moment.py` & `qiskit-nature-0.6.1/test/second_q/properties/test_dipole_moment.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/properties/test_electronic_density.py` & `qiskit-nature-0.6.1/test/second_q/properties/test_electronic_density.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/properties/test_magnetization.py` & `qiskit-nature-0.6.1/test/second_q/properties/test_magnetization.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/properties/test_occupied_modals.py` & `qiskit-nature-0.6.1/test/second_q/properties/test_occupied_modals.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/properties/test_particle_number.py` & `qiskit-nature-0.6.1/test/second_q/properties/test_particle_number.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/transformers/resources/BeH_sto3g_reduced.json` & `qiskit-nature-0.6.1/test/second_q/transformers/resources/BeH_sto3g_reduced.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/transformers/resources/LiH_sto3g_reduced.json` & `qiskit-nature-0.6.1/test/second_q/transformers/resources/LiH_sto3g_reduced.json`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/transformers/test_active_space_transformer.py` & `qiskit-nature-0.6.1/test/second_q/transformers/test_active_space_transformer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/transformers/test_basis_transformer.py` & `qiskit-nature-0.6.1/test/second_q/transformers/test_basis_transformer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/transformers/test_freeze_core_transformer.py` & `qiskit-nature-0.6.1/test/second_q/transformers/test_freeze_core_transformer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/second_q/utils.py` & `qiskit-nature-0.6.1/test/second_q/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/test_deprecation.py` & `qiskit-nature-0.6.1/test/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/test_end2end_with_vqe.py` & `qiskit-nature-0.6.1/test/test_end2end_with_vqe.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/test_hdf5.py` & `qiskit-nature-0.6.1/test/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/test_logging.py` & `qiskit-nature-0.6.1/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/test_readme_sample.py` & `qiskit-nature-0.6.1/test/test_readme_sample.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/BeH_sto3g.hdf5` & `qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/BeH_sto3g.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/BeH_sto3g_reduced.hdf5` & `qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/BeH_sto3g_reduced.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/H2_631g.hdf5` & `qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/H2_631g.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/H2_sto3g.hdf5` & `qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/H2_sto3g.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/H2_sto3g_v2.hdf5` & `qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/H2_sto3g_v2.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/LiH_sto3g.hdf5` & `qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/LiH_sto3g.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/LiH_sto3g_reduced.hdf5` & `qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/LiH_sto3g_reduced.hdf5`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/test_active_space_transformer.py` & `qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/test_active_space_transformer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/transformers/second_quantization/electronic/test_freeze_core_transformer.py` & `qiskit-nature-0.6.1/test/transformers/second_quantization/electronic/test_freeze_core_transformer.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-0.6.0/test/utils/test_linalg.py` & `qiskit-nature-0.6.1/test/utils/test_linalg.py`

 * *Files identical despite different names*

