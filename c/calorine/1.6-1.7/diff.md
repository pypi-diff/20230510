# Comparing `tmp/calorine-1.6.tar.gz` & `tmp/calorine-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calorine-1.6.tar", last modified: Fri Apr 21 19:05:46 2023, max compression
+gzip compressed data, was "calorine-1.7.tar", last modified: Wed May 10 08:50:00 2023, max compression
```

## Comparing `calorine-1.6.tar` & `calorine-1.7.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.497277 calorine-1.6/
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-04-21 19:05:34.000000 calorine-1.6/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-21 19:05:34.000000 calorine-1.6/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-04-21 19:05:34.000000 calorine-1.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3227 2023-04-21 19:05:34.000000 calorine-1.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    11153 2023-04-21 19:05:34.000000 calorine-1.6/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1204 2023-04-21 19:05:34.000000 calorine-1.6/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    16725 2023-04-21 19:05:34.000000 calorine-1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1265 2023-04-21 19:05:46.497277 calorine-1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-04-21 19:05:34.000000 calorine-1.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.447273 calorine-1.6/calorine/
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-21 19:05:34.000000 calorine-1.6/calorine/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.450273 calorine-1.6/calorine/calculators/
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-04-21 19:05:34.000000 calorine-1.6/calorine/calculators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6498 2023-04-21 19:05:34.000000 calorine-1.6/calorine/calculators/cpunep.py
--rw-rw-rw-   0 root         (0) root         (0)    11345 2023-04-21 19:05:34.000000 calorine-1.6/calorine/calculators/gpunep.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.451274 calorine-1.6/calorine/gpumd/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-21 19:05:34.000000 calorine-1.6/calorine/gpumd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7717 2023-04-21 19:05:34.000000 calorine-1.6/calorine/gpumd/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.453274 calorine-1.6/calorine/nep/
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-04-21 19:05:34.000000 calorine-1.6/calorine/nep/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12807 2023-04-21 19:05:34.000000 calorine-1.6/calorine/nep/io.py
--rw-rw-rw-   0 root         (0) root         (0)     9877 2023-04-21 19:05:34.000000 calorine-1.6/calorine/nep/nep.py
--rw-rw-rw-   0 root         (0) root         (0)    14972 2023-04-21 19:05:34.000000 calorine-1.6/calorine/nep/potential.py
--rw-rw-rw-   0 root         (0) root         (0)     4779 2023-04-21 19:05:34.000000 calorine-1.6/calorine/nep/training_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.454274 calorine-1.6/calorine/tools/
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-04-21 19:05:34.000000 calorine-1.6/calorine/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5429 2023-04-21 19:05:34.000000 calorine-1.6/calorine/tools/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     3267 2023-04-21 19:05:34.000000 calorine-1.6/calorine/tools/phonons.py
--rw-rw-rw-   0 root         (0) root         (0)     2779 2023-04-21 19:05:34.000000 calorine-1.6/calorine/tools/stiffness.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2023-04-21 19:05:34.000000 calorine-1.6/calorine/tools/structures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.449273 calorine-1.6/calorine.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1265 2023-04-21 19:05:46.000000 calorine-1.6/calorine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4771 2023-04-21 19:05:46.000000 calorine-1.6/calorine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:05:46.000000 calorine-1.6/calorine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:05:46.000000 calorine-1.6/calorine.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-21 19:05:46.000000 calorine-1.6/calorine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-21 19:05:46.000000 calorine-1.6/calorine.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.457274 calorine-1.6/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.458274 calorine-1.6/doc/_static/
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-21 19:05:34.000000 calorine-1.6/doc/_static/custom.css
--rw-rw-rw-   0 root         (0) root         (0)     4286 2023-04-21 19:05:34.000000 calorine-1.6/doc/_static/logo.ico
--rw-rw-rw-   0 root         (0) root         (0)    18405 2023-04-21 19:05:34.000000 calorine-1.6/doc/_static/logo.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.459274 calorine-1.6/doc/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-04-21 19:05:34.000000 calorine-1.6/doc/_templates/breadcrumbs.html
--rw-rw-rw-   0 root         (0) root         (0)     2305 2023-04-21 19:05:34.000000 calorine-1.6/doc/_templates/page.html
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-04-21 19:05:34.000000 calorine-1.6/doc/_templates/versions.html
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-04-21 19:05:34.000000 calorine-1.6/doc/calculators.rst
--rw-rw-rw-   0 root         (0) root         (0)     2799 2023-04-21 19:05:34.000000 calorine-1.6/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-21 19:05:34.000000 calorine-1.6/doc/genindex.rst
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-04-21 19:05:34.000000 calorine-1.6/doc/gpumd.rst
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-21 19:05:34.000000 calorine-1.6/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-21 19:05:34.000000 calorine-1.6/doc/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-04-21 19:05:34.000000 calorine-1.6/doc/nep.rst
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-04-21 19:05:34.000000 calorine-1.6/doc/tools.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.463274 calorine-1.6/doc/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)    48216 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/calculators.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    48910 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/elastic_stiffness_tensor.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    57668 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/nep_descriptors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   707350 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/nep_model_inspection.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   215886 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/phonons.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    35580 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/structure_relaxation.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   162489 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/thermal_conductivity_from_bte.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   299804 2023-04-21 19:05:34.000000 calorine-1.6/doc/tutorials/visualize_descriptor_space_with_pca.ipynb
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 19:05:46.497277 calorine-1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4326 2023-04-21 19:05:34.000000 calorine-1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.441273 calorine-1.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.465275 calorine-1.6/src/nepy/
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-04-21 19:05:34.000000 calorine-1.6/src/nepy/README.md
--rw-rw-rw-   0 root         (0) root         (0)    81016 2023-04-21 19:05:34.000000 calorine-1.6/src/nepy/nep.cpp
--rw-rw-rw-   0 root         (0) root         (0)     4300 2023-04-21 19:05:34.000000 calorine-1.6/src/nepy/nep.h
--rw-rw-rw-   0 root         (0) root         (0)     6866 2023-04-21 19:05:34.000000 calorine-1.6/src/nepy/nepy.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-04-21 19:05:34.000000 calorine-1.6/src/nepy/nepy.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.470275 calorine-1.6/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.473275 calorine-1.6/tests/example_files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.474275 calorine-1.6/tests/example_files/dipole/
--rw-rw-rw-   0 root         (0) root         (0)    31383 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/dipole/dipole_test.out
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/dipole/test.xyz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.475275 calorine-1.6/tests/example_files/fcp/
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/fcp/fcp.txt
--rw-rw-rw-   0 root         (0) root         (0)     4988 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/fcp/fcs_order2.in
--rw-rw-rw-   0 root         (0) root         (0)     2376 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/fcp/r0.in
--rw-rw-rw-   0 root         (0) root         (0)     5520 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/hac.out
--rw-rw-rw-   0 root         (0) root         (0)     5520 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/hac_nan.out
--rw-rw-rw-   0 root         (0) root         (0)    12600 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/kappa.out
--rw-rw-rw-   0 root         (0) root         (0)    12600 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/kappa_nan.out
--rw-rw-rw-   0 root         (0) root         (0)    11400 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/loss.out
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.475275 calorine-1.6/tests/example_files/md_no_velocities_or_forces/
--rw-rw-rw-   0 root         (0) root         (0)     6001 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/md_no_velocities_or_forces/dump.xyz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.475275 calorine-1.6/tests/example_files/md_velocities_and_forces/
--rw-rw-rw-   0 root         (0) root         (0)     9605 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/md_velocities_and_forces/dump.xyz
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/nep.in
--rw-rw-rw-   0 root         (0) root         (0)    21699 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/nep.txt
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/run.in
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/thermo_ortho_v3.2.out
--rw-rw-rw-   0 root         (0) root         (0)     2709 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_files/thermo_tri_v3.2.out
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.482276 calorine-1.6/tests/example_output/
--rw-rw-rw-   0 root         (0) root         (0)     2522 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/CON_NEP2_dummy_CON_3atom_descriptor.out
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/CON_NEP2_dummy_CON_3atom_force.out
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/CON_NEP2_dummy_CON_3atom_virial.out
--rw-rw-rw-   0 root         (0) root         (0)     1942 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/CO_NEP2_dummy_CO_2atom_descriptor.out
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/CO_NEP2_dummy_CO_2atom_force.out
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/CO_NEP2_dummy_CO_2atom_virial.out
--rw-rw-rw-   0 root         (0) root         (0)     1942 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/C_NEP2_dummy_C_2atom_descriptor.out
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/C_NEP2_dummy_C_2atom_force.out
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/C_NEP2_dummy_C_2atom_virial.out
--rw-rw-rw-   0 root         (0) root         (0)     1942 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_descriptor.out
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_force.out
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_virial.out
--rw-rw-rw-   0 root         (0) root         (0)   145555 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_descriptor.out
--rw-rw-rw-   0 root         (0) root         (0)    13930 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_force.out
--rw-rw-rw-   0 root         (0) root         (0)    41677 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_virial.out
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_descriptor.out
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_force.out
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_virial.out
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.483276 calorine-1.6/tests/example_structures/
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_structures/CON_3atom.in
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_structures/CO_2atom.in
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_structures/C_2atom.in
--rw-rw-rw-   0 root         (0) root         (0)    20588 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_structures/PbTe_250atom.in
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-04-21 19:05:34.000000 calorine-1.6/tests/example_structures/PbTe_2atom.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.488276 calorine-1.6/tests/nep_models/
--rw-rw-rw-   0 root         (0) root         (0)    28522 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/CON_NEP2_dummy.txt
--rw-rw-rw-   0 root         (0) root         (0)    26644 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/CO_NEP2_dummy.txt
--rw-rw-rw-   0 root         (0) root         (0)    26642 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/C_NEP2_dummy.txt
--rw-rw-rw-   0 root         (0) root         (0)    52623 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/CsPbI3-SCAN.txt
--rw-rw-rw-   0 root         (0) root         (0)    26647 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/PbTe_NEP2_dummy.txt
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/README.md
--rw-rw-rw-   0 root         (0) root         (0)    21670 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/nep3_v3.2_PbTe_Fan22.txt
--rw-rw-rw-   0 root         (0) root         (0)    21687 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt
--rw-rw-rw-   0 root         (0) root         (0)    37053 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/nep4_PbTe.txt
--rw-rw-rw-   0 root         (0) root         (0)   381233 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/nep4_dipole_Christian.txt
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-04-21 19:05:34.000000 calorine-1.6/tests/nep_models/update_expted_descriptors.py
--rw-rw-rw-   0 root         (0) root         (0)     5445 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    17089 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_cpunep.py
--rw-rw-rw-   0 root         (0) root         (0)    11285 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_gpumd_io.py
--rw-rw-rw-   0 root         (0) root         (0)    17572 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_gpunep.py
--rw-rw-rw-   0 root         (0) root         (0)     3743 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_nep3_execution.py
--rw-rw-rw-   0 root         (0) root         (0)     3743 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_nep4_execution.py
--rw-rw-rw-   0 root         (0) root         (0)    14638 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_nep_io.py
--rw-rw-rw-   0 root         (0) root         (0)    11387 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_nep_nep.py
--rw-rw-rw-   0 root         (0) root         (0)     5690 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_nep_potential.py
--rw-rw-rw-   0 root         (0) root         (0)     2261 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_phonons.py
--rw-rw-rw-   0 root         (0) root         (0)     5360 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_setup_training.py
--rw-rw-rw-   0 root         (0) root         (0)     6833 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_stiffness.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2023-04-21 19:05:34.000000 calorine-1.6/tests/test_structures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.495277 calorine-1.6/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)    52623 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/CsPbI3-SCAN.txt
--rw-rw-rw-   0 root         (0) root         (0)    21687 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/PbTe_NEP3.txt
--rw-rw-rw-   0 root         (0) root         (0)    48216 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/calculators.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    48910 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/elastic_stiffness_tensor.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    44098 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/nep-graphite.txt
--rw-rw-rw-   0 root         (0) root         (0)   381233 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/nep4_dipole.txt
--rw-rw-rw-   0 root         (0) root         (0)    57668 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/nep_descriptors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   707350 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/nep_model_inspection.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:05:46.497277 calorine-1.6/tutorials/perovskite-structures/
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/perovskite-structures/CsPbI3-cubic-Pm-3m.xyz
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/perovskite-structures/CsPbI3-delta-Pnma.xyz
--rw-rw-rw-   0 root         (0) root         (0)     1327 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/perovskite-structures/CsPbI3-orthorhombic-Pnma.xyz
--rw-rw-rw-   0 root         (0) root         (0)      759 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/perovskite-structures/CsPbI3-tetragonal-I4mcm.xyz
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/perovskite-structures/CsPbI3-tetragonal-P4mbm.xyz
--rw-rw-rw-   0 root         (0) root         (0)   215886 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/phonons.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/prim-graphite.xyz
--rw-rw-rw-   0 root         (0) root         (0)    35580 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/structure_relaxation.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/structure_with_dipole.xyz
--rw-rw-rw-   0 root         (0) root         (0)   162489 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/thermal_conductivity_from_bte.ipynb
--rw-rw-rw-   0 root         (0) root         (0)   299804 2023-04-21 19:05:34.000000 calorine-1.6/tutorials/visualize_descriptor_space_with_pca.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.141219 calorine-1.7/
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-05-10 08:49:46.000000 calorine-1.7/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-05-10 08:49:46.000000 calorine-1.7/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-05-10 08:49:46.000000 calorine-1.7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3227 2023-05-10 08:49:46.000000 calorine-1.7/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11153 2023-05-10 08:49:46.000000 calorine-1.7/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2023-05-10 08:49:46.000000 calorine-1.7/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    16725 2023-05-10 08:49:46.000000 calorine-1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-05-10 08:50:00.141219 calorine-1.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-05-10 08:49:46.000000 calorine-1.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.088214 calorine-1.7/calorine/
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-05-10 08:49:46.000000 calorine-1.7/calorine/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.091214 calorine-1.7/calorine/calculators/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-05-10 08:49:46.000000 calorine-1.7/calorine/calculators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8480 2023-05-10 08:49:46.000000 calorine-1.7/calorine/calculators/cpunep.py
+-rw-rw-rw-   0 root         (0) root         (0)    11345 2023-05-10 08:49:46.000000 calorine-1.7/calorine/calculators/gpunep.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.092214 calorine-1.7/calorine/gpumd/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-10 08:49:46.000000 calorine-1.7/calorine/gpumd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7717 2023-05-10 08:49:46.000000 calorine-1.7/calorine/gpumd/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.093214 calorine-1.7/calorine/nep/
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-05-10 08:49:46.000000 calorine-1.7/calorine/nep/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13123 2023-05-10 08:49:46.000000 calorine-1.7/calorine/nep/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    24383 2023-05-10 08:49:46.000000 calorine-1.7/calorine/nep/nep.py
+-rw-rw-rw-   0 root         (0) root         (0)    14972 2023-05-10 08:49:46.000000 calorine-1.7/calorine/nep/potential.py
+-rw-rw-rw-   0 root         (0) root         (0)     4779 2023-05-10 08:49:46.000000 calorine-1.7/calorine/nep/training_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.098215 calorine-1.7/calorine/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-05-10 08:49:46.000000 calorine-1.7/calorine/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5429 2023-05-10 08:49:46.000000 calorine-1.7/calorine/tools/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3267 2023-05-10 08:49:46.000000 calorine-1.7/calorine/tools/phonons.py
+-rw-rw-rw-   0 root         (0) root         (0)     2779 2023-05-10 08:49:46.000000 calorine-1.7/calorine/tools/stiffness.py
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2023-05-10 08:49:46.000000 calorine-1.7/calorine/tools/structures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.090214 calorine-1.7/calorine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-05-10 08:49:59.000000 calorine-1.7/calorine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-05-10 08:50:00.000000 calorine-1.7/calorine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 08:49:59.000000 calorine-1.7/calorine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 08:49:59.000000 calorine-1.7/calorine.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-10 08:49:59.000000 calorine-1.7/calorine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-10 08:49:59.000000 calorine-1.7/calorine.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.100215 calorine-1.7/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.101215 calorine-1.7/doc/_static/
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-05-10 08:49:46.000000 calorine-1.7/doc/_static/custom.css
+-rw-rw-rw-   0 root         (0) root         (0)     4286 2023-05-10 08:49:46.000000 calorine-1.7/doc/_static/logo.ico
+-rw-rw-rw-   0 root         (0) root         (0)    18405 2023-05-10 08:49:46.000000 calorine-1.7/doc/_static/logo.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.102215 calorine-1.7/doc/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-10 08:49:46.000000 calorine-1.7/doc/_templates/breadcrumbs.html
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-05-10 08:49:46.000000 calorine-1.7/doc/_templates/page.html
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-05-10 08:49:46.000000 calorine-1.7/doc/_templates/versions.html
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-05-10 08:49:46.000000 calorine-1.7/doc/calculators.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2799 2023-05-10 08:49:46.000000 calorine-1.7/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-10 08:49:46.000000 calorine-1.7/doc/genindex.rst
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-05-10 08:49:46.000000 calorine-1.7/doc/gpumd.rst
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-05-10 08:49:46.000000 calorine-1.7/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-05-10 08:49:46.000000 calorine-1.7/doc/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-10 08:49:46.000000 calorine-1.7/doc/nep.rst
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-05-10 08:49:46.000000 calorine-1.7/doc/tools.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.106216 calorine-1.7/doc/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)    48216 2023-05-10 08:49:46.000000 calorine-1.7/doc/tutorials/calculators.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    48886 2023-05-10 08:49:46.000000 calorine-1.7/doc/tutorials/elastic_stiffness_tensor.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    57668 2023-05-10 08:49:46.000000 calorine-1.7/doc/tutorials/nep_descriptors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   707350 2023-05-10 08:49:46.000000 calorine-1.7/doc/tutorials/nep_model_inspection.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   215886 2023-05-10 08:49:46.000000 calorine-1.7/doc/tutorials/phonons.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    35580 2023-05-10 08:49:46.000000 calorine-1.7/doc/tutorials/structure_relaxation.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   162402 2023-05-10 08:49:46.000000 calorine-1.7/doc/tutorials/thermal_conductivity_from_bte.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   299804 2023-05-10 08:49:46.000000 calorine-1.7/doc/tutorials/visualize_descriptor_space_with_pca.ipynb
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 08:50:00.141219 calorine-1.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2023-05-10 08:49:46.000000 calorine-1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.082213 calorine-1.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.108216 calorine-1.7/src/nepy/
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-05-10 08:49:46.000000 calorine-1.7/src/nepy/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    92881 2023-05-10 08:49:46.000000 calorine-1.7/src/nepy/nep.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     4709 2023-05-10 08:49:46.000000 calorine-1.7/src/nepy/nep.h
+-rw-rw-rw-   0 root         (0) root         (0)    13815 2023-05-10 08:49:46.000000 calorine-1.7/src/nepy/nepy.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2023-05-10 08:49:46.000000 calorine-1.7/src/nepy/nepy.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.113216 calorine-1.7/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.116216 calorine-1.7/tests/example_files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.117216 calorine-1.7/tests/example_files/dipole/
+-rw-rw-rw-   0 root         (0) root         (0)    31383 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/dipole/dipole_test.out
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/dipole/test.xyz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.118217 calorine-1.7/tests/example_files/fcp/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/fcp/fcp.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4988 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/fcp/fcs_order2.in
+-rw-rw-rw-   0 root         (0) root         (0)     2376 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/fcp/r0.in
+-rw-rw-rw-   0 root         (0) root         (0)     5520 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/hac.out
+-rw-rw-rw-   0 root         (0) root         (0)     5520 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/hac_nan.out
+-rw-rw-rw-   0 root         (0) root         (0)    12600 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/kappa.out
+-rw-rw-rw-   0 root         (0) root         (0)    12600 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/kappa_nan.out
+-rw-rw-rw-   0 root         (0) root         (0)    11400 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/loss.out
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.118217 calorine-1.7/tests/example_files/md_no_velocities_or_forces/
+-rw-rw-rw-   0 root         (0) root         (0)     6001 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/md_no_velocities_or_forces/dump.xyz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.118217 calorine-1.7/tests/example_files/md_velocities_and_forces/
+-rw-rw-rw-   0 root         (0) root         (0)     9605 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/md_velocities_and_forces/dump.xyz
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/nep.in
+-rw-rw-rw-   0 root         (0) root         (0)    21699 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/nep.txt
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/run.in
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/thermo_ortho_v3.2.out
+-rw-rw-rw-   0 root         (0) root         (0)     2709 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_files/thermo_tri_v3.2.out
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.125217 calorine-1.7/tests/example_output/
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/CON_NEP2_dummy_CON_3atom_descriptor.out
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/CON_NEP2_dummy_CON_3atom_force.out
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/CON_NEP2_dummy_CON_3atom_virial.out
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/CO_NEP2_dummy_CO_2atom_descriptor.out
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/CO_NEP2_dummy_CO_2atom_force.out
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/CO_NEP2_dummy_CO_2atom_virial.out
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/C_NEP2_dummy_C_2atom_descriptor.out
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/C_NEP2_dummy_C_2atom_force.out
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/C_NEP2_dummy_C_2atom_virial.out
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_descriptor.out
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_force.out
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_virial.out
+-rw-rw-rw-   0 root         (0) root         (0)   145555 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_descriptor.out
+-rw-rw-rw-   0 root         (0) root         (0)    13930 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_force.out
+-rw-rw-rw-   0 root         (0) root         (0)    41677 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_virial.out
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_descriptor.out
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_force.out
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_virial.out
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.126217 calorine-1.7/tests/example_structures/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_structures/CON_3atom.in
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_structures/CO_2atom.in
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_structures/C_2atom.in
+-rw-rw-rw-   0 root         (0) root         (0)    20588 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_structures/PbTe_250atom.in
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-05-10 08:49:46.000000 calorine-1.7/tests/example_structures/PbTe_2atom.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.131218 calorine-1.7/tests/nep_models/
+-rw-rw-rw-   0 root         (0) root         (0)    28522 2023-05-10 08:49:46.000000 calorine-1.7/tests/nep_models/CON_NEP2_dummy.txt
+-rw-rw-rw-   0 root         (0) root         (0)    26644 2023-05-10 08:49:46.000000 calorine-1.7/tests/nep_models/CO_NEP2_dummy.txt
+-rw-rw-rw-   0 root         (0) root         (0)    26642 2023-05-10 08:49:46.000000 calorine-1.7/tests/nep_models/C_NEP2_dummy.txt
+-rw-rw-rw-   0 root         (0) root         (0)    52623 2023-05-10 08:49:46.000000 calorine-1.7/tests/nep_models/CsPbI3-SCAN.txt
+-rw-rw-rw-   0 root         (0) root         (0)    26647 2023-05-10 08:49:46.000000 calorine-1.7/tests/nep_models/PbTe_NEP2_dummy.txt
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-05-10 08:49:46.000000 calorine-1.7/tests/nep_models/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    21670 2023-05-10 08:49:46.000000 calorine-1.7/tests/nep_models/nep3_v3.2_PbTe_Fan22.txt
+-rw-rw-rw-   0 root         (0) root         (0)    21687 2023-05-10 08:49:46.000000 calorine-1.7/tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt
+-rw-rw-rw-   0 root         (0) root         (0)    37053 2023-05-10 08:49:46.000000 calorine-1.7/tests/nep_models/nep4_PbTe.txt
+-rw-rw-rw-   0 root         (0) root         (0)   381233 2023-05-10 08:49:46.000000 calorine-1.7/tests/nep_models/nep4_dipole_Christian.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2023-05-10 08:49:46.000000 calorine-1.7/tests/nep_models/update_expted_descriptors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5445 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    22464 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_cpunep.py
+-rw-rw-rw-   0 root         (0) root         (0)    11285 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_gpumd_io.py
+-rw-rw-rw-   0 root         (0) root         (0)    17572 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_gpunep.py
+-rw-rw-rw-   0 root         (0) root         (0)     3743 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_nep3_execution.py
+-rw-rw-rw-   0 root         (0) root         (0)     3743 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_nep4_execution.py
+-rw-rw-rw-   0 root         (0) root         (0)    14848 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_nep_io.py
+-rw-rw-rw-   0 root         (0) root         (0)    21406 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_nep_nep.py
+-rw-rw-rw-   0 root         (0) root         (0)     5690 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_nep_potential.py
+-rw-rw-rw-   0 root         (0) root         (0)     2261 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_phonons.py
+-rw-rw-rw-   0 root         (0) root         (0)     5360 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_setup_training.py
+-rw-rw-rw-   0 root         (0) root         (0)     6833 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_stiffness.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2023-05-10 08:49:46.000000 calorine-1.7/tests/test_structures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.138218 calorine-1.7/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)    52623 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/CsPbI3-SCAN.txt
+-rw-rw-rw-   0 root         (0) root         (0)    21687 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/PbTe_NEP3.txt
+-rw-rw-rw-   0 root         (0) root         (0)    48216 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/calculators.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    48886 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/elastic_stiffness_tensor.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    44098 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/nep-graphite.txt
+-rw-rw-rw-   0 root         (0) root         (0)   381233 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/nep4_dipole.txt
+-rw-rw-rw-   0 root         (0) root         (0)    57668 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/nep_descriptors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   707350 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/nep_model_inspection.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:50:00.140218 calorine-1.7/tutorials/perovskite-structures/
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/perovskite-structures/CsPbI3-cubic-Pm-3m.xyz
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/perovskite-structures/CsPbI3-delta-Pnma.xyz
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/perovskite-structures/CsPbI3-orthorhombic-Pnma.xyz
+-rw-rw-rw-   0 root         (0) root         (0)      759 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/perovskite-structures/CsPbI3-tetragonal-I4mcm.xyz
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/perovskite-structures/CsPbI3-tetragonal-P4mbm.xyz
+-rw-rw-rw-   0 root         (0) root         (0)   215886 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/phonons.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/prim-graphite.xyz
+-rw-rw-rw-   0 root         (0) root         (0)    35580 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/structure_relaxation.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/structure_with_dipole.xyz
+-rw-rw-rw-   0 root         (0) root         (0)   162402 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/thermal_conductivity_from_bte.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)   299804 2023-05-10 08:49:46.000000 calorine-1.7/tutorials/visualize_descriptor_space_with_pca.ipynb
```

### Comparing `calorine-1.6/.coveragerc` & `calorine-1.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `calorine-1.6/.gitignore` & `calorine-1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `calorine-1.6/.gitlab-ci.yml` & `calorine-1.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `calorine-1.6/CONTRIBUTING.md` & `calorine-1.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `calorine-1.6/Dockerfile` & `calorine-1.7/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 RUN \
   pip3 install --upgrade \
     pip \
   && \
   pip3 install --upgrade \
     coverage \
     flake8 \
+    flake8-quotes \
     nbmake \
     pytest \
     setuptools_scm \
     twine \
     xdoctest
 
 # Packages needed for calorine (compare setup.py)
@@ -53,15 +54,15 @@
   pip3 install --upgrade \
     jinja2==3.0.3
 
 # Install GPUMD
 RUN \
   git clone https://github.com/brucefan1983/GPUMD.git && \
   cd GPUMD && \
-  git checkout v3.6 && \
+  git checkout v3.7 && \
   cd src && \
   make CFLAGS="-std=c++11 -O3 -arch=sm_72 -DDEBUG" -j4 && \
   mv gpumd nep /usr/local/bin/ && \
   cd ../.. && \
   rm -fr GPUMD
 
 CMD /bin/bash
```

### Comparing `calorine-1.6/LICENSE` & `calorine-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `calorine-1.6/PKG-INFO` & `calorine-1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: calorine
-Version: 1.6
+Version: 1.7
 Summary: A Python library for building and sampling NEP models via GPUMD simulations.
 Home-page: http://calorine.materialsmodeling.org/
 Author: calorine developer group
 License: Mozilla Public License 2.0 (MPL 2.0)
 Description: calorine
         ========
```

### Comparing `calorine-1.6/calorine/calculators/cpunep.py` & `calorine-1.7/calorine/calculators/cpunep.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Parameters
     ----------
     potential_filename : str
         Path to nep.txt potential
     atoms : Atoms
         Atoms to attach the calculator to
     label : str
-        Label for this calculator
+        Label for this calclator
     debug : bool, optional
         Flag to toggle debug mode. Prints GPUMD output. Defaults to False.
 
     Raises
     ------
     FileNotFoundError
         Raises FileNotFoundError if `potential_filename` does not point to a valid file.
@@ -35,49 +35,57 @@
     -------
 
     >>> calc = CPUNEP('nep.txt')
     >>> atoms.calc = calc
     >>> atoms.get_potential_energy()
     """
 
-    implemented_properties = ['energy', 'energies', 'forces', 'stress', 'dipole']
+    implemented_properties = [
+        'energy',
+        'energies',
+        'forces',
+        'stress',
+        'dipole',
+    ]
     debug = False
     nepy = None
 
-    def __init__(self,
-                 potential_filename: str,
-                 atoms: Atoms | None = None,
-                 label: str | None = None,
-                 debug: bool = False):
-
+    def __init__(
+        self,
+        potential_filename: str,
+        atoms: Atoms | None = None,
+        label: str | None = None,
+        debug: bool = False,
+    ):
         self.debug = debug
+
         if not os.path.exists(potential_filename):
             raise FileNotFoundError(f'{potential_filename} does not exist.')
         self.potential_filename = potential_filename
 
         # Initialize atoms, results and nepy - note that this is also done in Calculator.__init__()
         if atoms is not None:
             self.set_atoms(atoms)
-        parameters = {
-            'potential_filename': potential_filename
-        }
+        parameters = {'potential_filename': potential_filename}
         Calculator.__init__(self, label=label, atoms=atoms, **parameters)
         if atoms is not None:
             self._setup_nepy()
 
     def __str__(self) -> str:
         def indent(s: str, i: int) -> str:
             s = '\n'.join([i * ' ' + line for line in s.split('\n')])
             return s
 
-        parameters = '\n'.join([f'{key}: {value}' for key, value in self.parameters.items()])
+        parameters = '\n'.join(
+            [f'{key}: {value}' for key, value in self.parameters.items()]
+        )
         parameters = indent(parameters, 4)
         using_debug = '\nIn debug mode' if self.debug else ''
 
-        s = (f'{self.__class__.__name__}\n{parameters}{using_debug}')
+        s = f'{self.__class__.__name__}\n{parameters}{using_debug}'
         return s
 
     def _setup_nepy(self):
         """
         Creates an instance of the NEPY class and attaches it to the calculator object.
         The output from `nep.cpp` is only written to STDOUT if debug == True
         """
@@ -88,62 +96,76 @@
 
         N_atoms = len(self.atoms)
         self.N_atoms = N_atoms
         c = self.atoms.get_cell(complete=True).flatten()
         cell = [c[0], c[3], c[6], c[1], c[4], c[7], c[2], c[5], c[8]]
         symbols = self.atoms.get_chemical_symbols()
         positions = list(
-            self.atoms.get_positions().T.flatten())  # [x1, ..., xN, y1, ... yN,...]
+            self.atoms.get_positions().T.flatten()
+        )  # [x1, ..., xN, y1, ... yN,...]
+        masses = self.atoms.get_masses()
 
         # Disable output from C++ code by default
         if self.debug:
-            self.nepy = _nepy.NEPY(self.potential_filename, self.N_atoms,
-                                   cell, symbols, positions)
+            self.nepy = _nepy.NEPY(
+                self.potential_filename, self.N_atoms, cell, symbols, positions, masses
+            )
         else:
             with TemporaryFile('w') as f:
                 with contextlib.redirect_stdout(f):
-                    self.nepy = _nepy.NEPY(self.potential_filename,
-                                           self.N_atoms, cell, symbols, positions)
+                    self.nepy = _nepy.NEPY(
+                        self.potential_filename,
+                        self.N_atoms,
+                        cell,
+                        symbols,
+                        positions,
+                        masses,
+                    )
 
     def set_atoms(self, atoms: Atoms):
         """Updates the Atoms object.
 
         Parameters
         ----------
         atoms : Atoms
             Atoms to attach the calculator to
         """
         self.atoms = atoms
         self.results = {}
         self.nepy = None
 
     def _update_symbols(self):
-        """Update atom symbols in NEPY.
-        """
+        """Update atom symbols in NEPY."""
         symbols = self.atoms.get_chemical_symbols()
         self.nepy.set_symbols(symbols)
 
+    def _update_masses(self):
+        """Update atom masses in NEPY"""
+        masses = self.atoms.get_masses()
+        self.nepy.set_masses(masses)
+
     def _update_cell(self):
-        """Update cell parameters in NEPY.
-        """
+        """Update cell parameters in NEPY."""
         c = self.atoms.get_cell(complete=True).flatten()
         cell = [c[0], c[3], c[6], c[1], c[4], c[7], c[2], c[5], c[8]]
         self.nepy.set_cell(cell)
 
     def _update_positions(self):
-        """Update atom positions in NEPY.
-        """
+        """Update atom positions in NEPY."""
         positions = list(
-            self.atoms.get_positions().T.flatten())  # [x1, ..., xN, y1, ... yN,...]
+            self.atoms.get_positions().T.flatten()
+        )  # [x1, ..., xN, y1, ... yN,...]
         self.nepy.set_positions(positions)
 
-    def calculate(self,
-                  atoms: Atoms = None,
-                  properties: List[str] = None,
-                  system_changes: List[str] = all_changes):
+    def calculate(
+        self,
+        atoms: Atoms = None,
+        properties: List[str] = None,
+        system_changes: List[str] = all_changes,
+    ):
         """Calculate energy, per atom energies, forces, stress and dipole.
 
         Parameters
         ----------
         atoms : Atoms, optional
             System for which to calculate properties, by default None
         properties : List[str], optional
@@ -161,24 +183,74 @@
             self._setup_nepy()
         # Update existing NEPY interface
         for change in system_changes:
             if change == 'positions':
                 self._update_positions()
             elif change == 'numbers':
                 self._update_symbols()
+                self._update_masses()
             elif change == 'cell':
                 self._update_cell()
 
         energies, forces, virials = self.nepy.get_potential_forces_and_virials()
         energies_per_atom = np.array(energies)
         energy = energies_per_atom.sum()
         forces_per_atom = np.array(forces).reshape(-1, self.N_atoms).T
         virials_per_atom = np.array(virials).reshape(-1, self.N_atoms).T
-        stress = -(np.sum(virials_per_atom, axis=0) / atoms.get_volume()).reshape((3, 3))
+        stress = -(np.sum(virials_per_atom, axis=0) / self.atoms.get_volume()).reshape(
+            (3, 3)
+        )
         stress = full_3x3_to_voigt_6_stress(stress)
 
         dipole = np.array(self.nepy.get_dipole())
 
         self.results['energy'] = energy
         self.results['forces'] = forces_per_atom
         self.results['stress'] = stress
         self.results['dipole'] = dipole
+
+    def get_dipole_gradient(
+        self,
+        displacement: float = 0.01,
+        method: str = 'central difference',
+        charge: float = 1.0,
+    ):
+        """Calculates the dipole gradient using finite differences.
+
+        Parameters
+        ----------
+        structure
+            Input structure
+        potential_filename
+            Path to NEP potential. Defaults to None.
+        method
+            Method for computing gradient with finite differences.
+            One of 'forward difference' and 'central difference'.
+            Defaults to 'central difference'
+        displacement
+            Displacement in Å to use for finite differences. Defaults to 0.01 Å.
+        charge
+            System charge in units of the elemental charge.
+            Used for correcting the dipoles before computing the gradient.
+            Defaults to 1.0.
+
+        Returns
+        ------- dipole gradient with shape `(N, 3, 3)`
+        """
+        if displacement <= 0:
+            raise ValueError('displacement must be > 0 Å')
+
+        implemented_methods = {'forward difference': 0, 'central difference': 1}
+
+        if method not in implemented_methods.keys():
+            raise ValueError(f'Invalid method {method} for calculating gradient')
+
+        if self.nepy is None:
+            # Create new NEPY interface
+            self._setup_nepy()
+
+        dipole_gradient = np.array(
+            self.nepy.get_dipole_gradient(
+                displacement, implemented_methods[method], charge
+            )
+        ).reshape(self.N_atoms, 3, 3)
+        return dipole_gradient
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `calorine-1.6/calorine/calculators/gpunep.py` & `calorine-1.7/calorine/calculators/gpunep.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/calorine/gpumd/io.py` & `calorine-1.7/calorine/gpumd/io.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/calorine/nep/io.py` & `calorine-1.7/calorine/nep/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any, Dict, Iterable, List, NamedTuple, TextIO, Tuple
+from warnings import warn
 from os.path import exists, join as join_path
 import numpy as np
 from pandas import DataFrame
 from ase import Atoms
 from ase.units import GPa
 from ase.io import read, write
 from ase.stress import voigt_6_to_full_3x3_stress
@@ -21,26 +22,26 @@
 
     """
     data = np.loadtxt(filename)
     if isinstance(data[0], np.float64):
         # If only a single row in loss.out, append a dimension
         data = data.reshape(1, -1)
     if len(data[0]) != 10:
-        raise ValueError(f'Input file contains {len(data[0])} data columns.'
-                         f' Expected 10 columns.')
+        raise ValueError(
+            f'Input file contains {len(data[0])} data columns.' f' Expected 10 columns.'
+        )
     tags = 'total_loss L1 L2'
     tags += ' RMSE_E_train RMSE_F_train RMSE_V_train'
     tags += ' RMSE_E_test RMSE_F_test RMSE_V_test'
     generations = range(100, len(data) * 100 + 1, 100)
     df = DataFrame(data=data[:, 1:], columns=tags.split(), index=generations)
     return df
 
 
-def _write_structure_in_nep_format(structure: Atoms,
-                                   f: TextIO) -> None:
+def _write_structure_in_nep_format(structure: Atoms, f: TextIO) -> None:
     """Write structure block into a file-like object in format readable by nep executable.
 
     Parameters
     ----------
     structure
         input structure; must hold information regarding energy and forces
     f
@@ -63,38 +64,36 @@
     except RuntimeError:
         raise RuntimeError('Failed to retrieve energy and/or forces for structure')
     if np.isclose(structure.get_volume(), 0):
         raise ValueError('Structure cell must have a non-zero volume!')
     try:
         stress = structure.get_stress(voigt=False).flatten()
         stress = ' '.join([f'{s:.6f}' for s in stress])
-        structure.info['stress'] = f'\"{stress}\"'
+        structure.info['stress'] = f'"{stress}"'
     except RuntimeError:
-        print('Warning: Failed to retrieve stresses for structure')
+        warn('Failed to retrieve stresses for structure')
     write(filename=f, images=structure, write_info=True, format='extxyz')
 
 
-def write_structures(outfile: str,
-                     structures: List[Atoms]) -> None:
+def write_structures(outfile: str, structures: List[Atoms]) -> None:
     """Writes structures for training/testing in format readable by nep executable.
 
     Parameters
     ----------
     outfile
         output filename
     structures
         list of structures with energy, forces, and (possibly) stresses
     """
     with open(outfile, 'w') as f:
         for structure in structures:
             _write_structure_in_nep_format(structure, f)
 
 
-def write_nepfile(parameters: NamedTuple,
-                  dirname: str) -> None:
+def write_nepfile(parameters: NamedTuple, dirname: str) -> None:
     """Writes parameters file for NEP construction.
 
     Parameters
     ----------
     parameters
         input parameters; see `here <https://gpumd.org/nep/input_parameters/index.html>`__
     dirname
@@ -126,16 +125,23 @@
                 continue
             if flds[0].startswith('#'):
                 continue
             settings[flds[0]] = ' '.join(flds[1:])
     for key, val in settings.items():
         if key in ['version', 'neuron', 'generation', 'batch', 'population']:
             settings[key] = int(val)
-        elif key in ['lambda_1', 'lambda_2', 'lambda_e', 'lambda_f', 'lambda_v',
-                     'lambda_shear', 'force_delta']:
+        elif key in [
+            'lambda_1',
+            'lambda_2',
+            'lambda_e',
+            'lambda_f',
+            'lambda_v',
+            'lambda_shear',
+            'force_delta',
+        ]:
             settings[key] = float(val)
         elif key in ['cutoff', 'n_max', 'l_max', 'basis_size', 'zbl', 'type_weight']:
             settings[key] = [float(v) for v in val.split()]
         elif key == 'type':
             types = val.split()
             types[0] = int(types[0])
             settings[key] = types
@@ -160,80 +166,90 @@
     path = join_path(dirname)
     if not exists(path):
         raise ValueError(f'Directory {path} does not exist')
 
     structures = {}
 
     for stype in ['train', 'test']:
-        structures[stype] = read(join_path(dirname, f'{stype}.xyz'), format='extxyz', index=':')
+        structures[stype] = read(
+            join_path(dirname, f'{stype}.xyz'), format='extxyz', index=':'
+        )
 
         ts, ps = _read_data_file(path, f'energy_{stype}.out')
         n_structures = len(structures[stype])
-        assert len(ts) == n_structures, \
-            f'Number of structures in energy_{stype}.out ({len(ts)})' \
+        assert len(ts) == n_structures, (
+            f'Number of structures in energy_{stype}.out ({len(ts)})'
             f' and {stype}.xyz ({n_structures}) inconsistent'
+        )
         for structure, t, p in zip(structures[stype], ts, ps):
             structure.info['energy_target'] = t
             structure.info['energy_predicted'] = p
 
         ts, ps = _read_data_file(path, f'force_{stype}.out')
         n_atoms_total = sum([len(s) for s in structures[stype]])
-        assert len(ts) == n_atoms_total, \
-            f'Number of structures in force_{stype}.out ({len(ts)})' \
+        assert len(ts) == n_atoms_total, (
+            f'Number of structures in force_{stype}.out ({len(ts)})'
             f' and {stype}.xyz ({n_structures}) inconsistent'
+        )
         n = 0
         for structure in structures[stype]:
             nat = len(structure)
-            structure.info['force_target'] = np.array(ts[n:n+nat]).reshape(nat, 3)
-            structure.info['force_predicted'] = np.array(ps[n:n+nat]).reshape(nat, 3)
+            structure.info['force_target'] = np.array(ts[n: n + nat]).reshape(nat, 3)
+            structure.info['force_predicted'] = np.array(ps[n: n + nat]).reshape(
+                nat, 3
+            )
             n += nat
 
         ts, ps = _read_data_file(path, f'virial_{stype}.out')
-        assert len(ts) == 6 * n_structures, \
+        ts = np.array(ts).reshape((-1, 6))  # GPUMD 3.6 compatibility
+        ps = np.array(ps).reshape((-1, 6))
+        assert len(ts) == n_structures, \
             f'Number of structures in virial_{stype}.out ({len(ts)})' \
             f' and {stype}.xyz ({n_structures}) inconsistent'
-        ts = np.array(ts).reshape((6, n_structures)).T
-        ps = np.array(ps).reshape((6, n_structures)).T
         for structure, t, p in zip(structures[stype], ts, ps):
             assert np.shape(t) == (6,)
             structure.info['virial_target'] = t
             structure.info['virial_predicted'] = p
             conv = len(structure) / structure.get_volume() / GPa
             structure.info['stress_target'] = t * conv
             structure.info['stress_predicted'] = p * conv
 
     return structures['train'], structures['test']
 
 
-def _read_data_file(dirname: str,
-                    fname: str):
+def _read_data_file(dirname: str, fname: str):
     """Private function that parses energy/force/virial_*.out files and
     returns their content for further processing.
     """
     path = join_path(dirname, fname)
     if not exists(path):
         raise ValueError(f'Directory {path} does not exist')
     with open(path, 'r') as f:
         lines = f.readlines()
     target, predicted = [], []
     for line in lines:
         flds = line.split()
-        if len(flds) == 6:
+        if len(flds) == 12:  # Virial after GPUMD 3.7
+            predicted.append([float(s) for s in flds[0:6]])
+            target.append([float(s) for s in flds[6:12]])
+        elif len(flds) == 6:  # Force
             predicted.append([float(s) for s in flds[0:3]])
             target.append([float(s) for s in flds[3:6]])
-        elif len(flds) == 2:
+        elif len(flds) == 2:  # Energy, virial before GPUMD 3.7
             predicted.append(float(flds[0]))
             target.append(float(flds[1]))
     return target, predicted
 
 
-def get_parity_data(structures: List[Atoms],
-                    property: str,
-                    selection: List[str] = None,
-                    flatten: bool = False) -> DataFrame:
+def get_parity_data(
+    structures: List[Atoms],
+    property: str,
+    selection: List[str] = None,
+    flatten: bool = False,
+) -> DataFrame:
     """Returns the predicted and target energies, forces, virials or stresses
     from a list of structures in a format suitable for generating parity plots.
 
     The structures should  have been read using :func:`read_structures
     <calorine.nep.read_structures>`, such that the ``info``-object is
     populated with keys on the form ``<property>_<type>`` where ``<property>``
     is one of ``energy``, ``force``, ``virial``, and stress, and ``<type>`` is one
@@ -252,31 +268,30 @@
         A list containing which components to return, and/or the absolute value.
         Possible values are ``x``, ``y``, ``z``, ``xx``, ``yy``,
         ``zz``, ``yz``, ``xz``, ``xy``, ``abs``, ``pressure``.
     flatten
         if True return flattened lists; this is useful for flattening
         the components of force or virials into a simple list
     """
-    data = {
-        'predicted': [],
-        'target': []
-    }
+    data = {'predicted': [], 'target': []}
     voigt_mapping = {
         'x': 0,
         'y': 1,
         'z': 2,
         'xx': 0,
         'yy': 1,
         'zz': 2,
         'yz': 3,
         'xz': 4,
-        'xy': 5
+        'xy': 5,
     }
     if property not in ('energy', 'force', 'virial', 'stress'):
-        raise ValueError("`property` must be one of 'energy', 'force', 'virial', 'stress'.")
+        raise ValueError(
+            "`property` must be one of 'energy', 'force', 'virial', 'stress'."
+        )
     if property == 'energy' and selection:
         raise ValueError('Selection does nothing for scalar-valued `energy`.')
     if property != 'stress' and selection and 'pressure' in selection:
         raise ValueError(f'Cannot calculate pressure for `{property}`.')
     for structure in structures:
         for stype in data:
             property_with_stype = f'{property}_{stype}'
@@ -291,32 +306,35 @@
             selected_values = []
             for select in selection:
                 if property == 'force':
                     # flip to get (n_components, n_structures)
                     extracted_property = extracted_property.T
                 if select == 'abs':
                     if property == 'force':
-                        selected_values.append(np.linalg.norm(extracted_property, axis=0))
+                        selected_values.append(
+                            np.linalg.norm(extracted_property, axis=0)
+                        )
                     else:
                         # property can only be in ('virial', 'stress')
                         full_tensor = voigt_6_to_full_3x3_stress(extracted_property)
                         selected_values.append(np.linalg.norm(full_tensor))
                     continue
 
                 if select == 'pressure' and property == 'stress':
                     total_stress = extracted_property
-                    selected_values.append(- np.sum(total_stress[:3]) / 3)
+                    selected_values.append(-np.sum(total_stress[:3]) / 3)
                     continue
 
                 if select not in voigt_mapping:
                     raise ValueError(f'Selection `{select}` is not allowed.')
                 index = voigt_mapping[select]
                 if index >= extracted_property.shape[0]:
                     raise ValueError(
-                        f'Selection `{select}` is not compatible with property `{property}`.')
+                        f'Selection `{select}` is not compatible with property `{property}`.'
+                    )
                 selected_values.append(extracted_property[index])
             data[stype].append(selected_values)
     if flatten:
         for key, value in data.items():
             if len(np.shape(value[0])) > 0:
                 data[key] = np.concatenate(value).ravel().tolist()
     return DataFrame(data)
```

### Comparing `calorine-1.6/calorine/nep/potential.py` & `calorine-1.7/calorine/nep/potential.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/calorine/nep/training_factory.py` & `calorine-1.7/calorine/nep/training_factory.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/calorine/tools/__init__.py` & `calorine-1.7/calorine/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/calorine/tools/analysis.py` & `calorine-1.7/calorine/tools/analysis.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/calorine/tools/phonons.py` & `calorine-1.7/calorine/tools/phonons.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/calorine/tools/stiffness.py` & `calorine-1.7/calorine/tools/stiffness.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/calorine/tools/structures.py` & `calorine-1.7/calorine/tools/structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     structure
         atomic configuration to relax
     fmax
         if the absolute force for all atoms falls below this value the relaxation is stopped
     steps
         maximum number of relaxation steps the minimizer is allowed to take
     minimizer
-        minimizer to use; possible values: 'bfgs', 'cg', 'fire', 'gpmin', 'bfgs-scipy'
+        minimizer to use; possible values: 'bfgs', 'fire', 'gpmin', 'bfgs-scipy'
     constant_cell
         if True do not relax the cell or the volume
     constant_volume
         if True relax the cell shape but keep the volume constant
     kwargs
         keyword arguments to be handed over to the minimizer; possible arguments can be found
         in the `ASE documentation <https://wiki.fysik.dtu.dk/ase/ase/optimize.html>`_
```

### Comparing `calorine-1.6/calorine.egg-info/PKG-INFO` & `calorine-1.7/calorine.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: calorine
-Version: 1.6
+Version: 1.7
 Summary: A Python library for building and sampling NEP models via GPUMD simulations.
 Home-page: http://calorine.materialsmodeling.org/
 Author: calorine developer group
 License: Mozilla Public License 2.0 (MPL 2.0)
 Description: calorine
         ========
```

### Comparing `calorine-1.6/calorine.egg-info/SOURCES.txt` & `calorine-1.7/calorine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/_static/custom.css` & `calorine-1.7/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/_static/logo.ico` & `calorine-1.7/doc/_static/logo.ico`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/_static/logo.png` & `calorine-1.7/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/_templates/page.html` & `calorine-1.7/doc/_templates/page.html`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/_templates/versions.html` & `calorine-1.7/doc/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/calculators.rst` & `calorine-1.7/doc/calculators.rst`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/conf.py` & `calorine-1.7/doc/conf.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/index.rst` & `calorine-1.7/doc/index.rst`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/installation.rst` & `calorine-1.7/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/tutorials/calculators.ipynb` & `calorine-1.7/doc/tutorials/calculators.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/tutorials/elastic_stiffness_tensor.ipynb` & `calorine-1.7/doc/tutorials/elastic_stiffness_tensor.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'In the second part we then consider the orthorhombic "*

 * *            'structure of CsPbI$_3$, which allows us to demonstrate the difference between relaxed '*

 * *            "$c_{ij}$ and clamped elastic constants $c_{ij}^0$.\\n')], delete: [2]}}, 20: "*

 * *            "{'source': {insert: [(0, '## CsPbI$_3$\\n'), (5, 'To illustrate this effect, we here "*

 * *            'consider the elastic stiffness tensors in orthorhombic structure of CsPbI$_3$, which '*

 * *            'we descr […]*

```diff
@@ -29,15 +29,15 @@
         {
             "cell_type": "markdown",
             "id": "43ba3fde-7ecc-436a-b0b6-510bf9bdf333",
             "metadata": {},
             "source": [
                 "This tutorial illustrates the calculation of the elastic stiffness tensor $c_{ij}$ and its relation to the sound velocity.\n",
                 "In the first part we use silver in its face-centered cubic (FCC) ground state structure described by an effective medium theory (EMT) potential as a particular simple example.\n",
-                "In the second part we then consider the orthorhombic structure of CsPbI<sub>3</sub>, which allows us to demonstrate the difference between relaxed $c_{ij}$ and clamped elastic constants $c_{ij}^0$.\n",
+                "In the second part we then consider the orthorhombic structure of CsPbI$_3$, which allows us to demonstrate the difference between relaxed $c_{ij}$ and clamped elastic constants $c_{ij}^0$.\n",
                 "\n",
                 "For background on crystal elasticity and the role of symmetry you can consult, e.g., Nye, *Physical Properties of Crystals: Their Representation by Tensors and Matrices*, Oxford University Press (1957)."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "aa3f7c76-8e88-4b4f-86ea-547e67660845",
@@ -298,20 +298,20 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "fcb3b571-11ed-4605-a383-bc80c71371e5",
             "metadata": {},
             "source": [
-                "## CsPbI<sub>3</sub>\n",
+                "## CsPbI$_3$\n",
                 "\n",
                 "In materials with internal degrees of freedom one can distinguish the so-called relaxed $c_{ij}$ and clamped elastic constants $c_{ij}^0$.\n",
                 "In the former case, the ionic positions are allowed to relax after application of a macroscopic strain, whereas in the latter the relative coordinates are kept fixed.\n",
                 "\n",
-                "To illustrate this effect, we here consider the elastic stiffness tensors in orthorhombic structure of CsPbI<sub>3</sub>, which we describe using a neuroevolution potential (NEP) taken from Fransson *et al.*, [arxiv:2301.03497](https://doi.org/10.48550/arXiv.2301.03497)."
+                "To illustrate this effect, we here consider the elastic stiffness tensors in orthorhombic structure of CsPbI$_3$, which we describe using a neuroevolution potential (NEP) taken from Fransson *et al.*, [arxiv:2301.03497](https://doi.org/10.48550/arXiv.2301.03497)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "id": "37012612-3abc-4d5c-99db-489c8d57edd0",
             "metadata": {},
```

### Comparing `calorine-1.6/doc/tutorials/nep_descriptors.ipynb` & `calorine-1.7/doc/tutorials/nep_descriptors.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/tutorials/nep_model_inspection.ipynb` & `calorine-1.7/doc/tutorials/nep_model_inspection.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/tutorials/phonons.ipynb` & `calorine-1.7/doc/tutorials/phonons.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/tutorials/structure_relaxation.ipynb` & `calorine-1.7/doc/tutorials/structure_relaxation.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.6/doc/tutorials/thermal_conductivity_from_bte.ipynb` & `calorine-1.7/doc/tutorials/thermal_conductivity_from_bte.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995715082908163%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'Here, we provide an introductory tutorial on how to use "*

 * *            '[phono3py](https://phonopy.github.io/phono3py/) to compute the thermal conductivity '*

 * *            'using a neuroevolution potential (NEP) via the Boltzmann transport equation '*

 * *            "(BTE).\\n'), (3, 'The system under study is graphite represented by a NEP model "*

 * *            "developed in [this paper](https://doi.org/10.48550/arXiv.2304.06978).\\n'), (11, '2. "*

 * *            'Compute the f […]*

```diff
@@ -3,52 +3,50 @@
         {
             "cell_type": "markdown",
             "id": "2e9ac128",
             "metadata": {},
             "source": [
                 "# Thermal conductivity from BTE\n",
                 "\n",
-                "Here, we provide an introductory tutorial on how to use `phono3py <https://phonopy.github.io/phono3py/>`_ to compute the thermal conductivity using a neuroevolution potential (NEP) via the Boltzmann transport equation (BTE).\n",
-                "The system under study is graphite represented by a NEP model developed in `this paper <https://doi.org/10.48550/arXiv.2304.06978>`_.\n",
+                "Here, we provide an introductory tutorial on how to use [phono3py](https://phonopy.github.io/phono3py/) to compute the thermal conductivity using a neuroevolution potential (NEP) via the Boltzmann transport equation (BTE).\n",
+                "The system under study is graphite represented by a NEP model developed in [this paper](https://doi.org/10.48550/arXiv.2304.06978).\n",
                 "Note that `phono3py` also allows you to compute other phonon properties such as, e.g., phonon lifetimes.\n",
                 "\n",
                 "## Workflow\n",
                 "\n",
                 "The steps required are:\n",
                 "\n",
                 "1. Relax the primitive cell\n",
-                "2. Compute the force constants (`fc2.hdf5`, `fc3.hdf5`) using NEP for all structures generated by `phono3py`\n",
+                "2. Compute the force constants (`fc2.hdf5`, `fc3.hdf5`) using the NEP model for all structures generated by `phono3py`\n",
                 "3. Run the thermal conductivity calculation\n",
                 "\n",
                 "Since `phono3py` does not have a python API we will call it through its command line interface via the `os.system` function.\n",
                 "\n",
                 "\n",
                 "## BTE computational parameters\n",
                 "\n",
-                "<div class=\\\"alert alert-block alert-info\\\">\n",
-                "<b>Note 1:</b>\n",
+                "**Note 1:**\n",
                 "In order to achive converged force constants one must use a sufficiently large supercell, the size of which is specified via the `--dim` option.\n",
                 "Here, we, however, use a rather small supercell in order for the tutorial to run faster.\n",
                 "\n",
-                "<b>Note 2:</b>\n",
+                "**Note 2:**\n",
                 "Here, we use the `phono3py` default displacement amplitude of 0.03 \u00c5 when generating supercells for the force-constant extraction.\n",
                 "This may not be suitable for every materials.\n",
                 "\n",
-                "<b>Note 3:</b>\n",
+                "**Note 3:**\n",
                 "In order to achieve convergence of the thermal conductivity one should use a larger q-point mesh (`--mesh`), but here we use a rather small mesh in order for the tutorial to complete within an acceptable time.\n",
                 "\n",
-                "<b>Note 4:</b>\n",
-                "In order to obtain accurate predictions for the thermal conductivity in graphite one should employ the `--lbte` (see `here <https://phonopy.github.io/phono3py/direct-solution.html>`_ for more information).\n",
+                "**Note 4:**\n",
+                "In order to obtain accurate predictions for the thermal conductivity in graphite one should employ the `--lbte` (see [here](https://phonopy.github.io/phono3py/direct-solution.html) for more information).\n",
                 "This method is, however, more costly both computationally and with respect to memory.\n",
                 "For simpliticity we therefore limit ourselves to the relaxation time approximation (RTA), which is invoked via the `--bterta` option.\n",
-                "</div>\n",
                 "\n",
                 "## Miscellaneous\n",
                 "\n",
-                "Additional related tutorials can be found on the `hiphive website <https://hiphive.materialsmodeling.org/tutorial/compute_third_order_properties.html) and [here](https://hiphive.materialsmodeling.org/tutorial/compute_third_order_properties.html>`_."
+                "Additional related tutorials can be found on the [hiphive website](https://hiphive.materialsmodeling.org/tutorial/compute_third_order_properties.html) and [here](https://hiphive.materialsmodeling.org/tutorial/compute_third_order_properties.html)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "757e4176",
             "metadata": {},
@@ -132,15 +130,15 @@
             "id": "f7f9bdfa",
             "metadata": {},
             "source": [
                 "## Construction of force constants\n",
                 "\n",
                 "Next, we construct the force constants.\n",
                 "Here, we use the approach implemented in `phono3py`, which generates the second and third force constants by systematic enumeration and numerical evaluation of the derivatives involved.\n",
-                "Especially for more complex materials, say systems with larger unit cells and/or lower symmetry, it can be beneficial to use regression based approaches such as the one implemented in, e.g., `hiphive <https://hiphive.materialsmodeling.org/>`_.\n",
+                "Especially for more complex materials, say systems with larger unit cells and/or lower symmetry, it can be beneficial to use regression based approaches such as the one implemented in, e.g., [hiphive](https://hiphive.materialsmodeling.org/).\n",
                 "\n",
                 "First, we call `phono3py` to generate a series of configurations (supercells) with systematic displacements."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
```

### Comparing `calorine-1.6/doc/tutorials/visualize_descriptor_space_with_pca.ipynb` & `calorine-1.7/doc/tutorials/visualize_descriptor_space_with_pca.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.6/setup.py` & `calorine-1.7/setup.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/src/nepy/nep.cpp` & `calorine-1.7/src/nepy/nep.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 #include <iterator>
 #include <sstream>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string>
 #include <vector>
 
+#if defined(_OPENMP)
+#include <omp.h>
+#endif
+
 namespace
 {
 const int MAX_NEURON = 200; // maximum number of neurons in the hidden layer
 const int MN = 1000;        // maximum number of neighbors for one atom
 const int NUM_OF_ABC = 24;  // 3 + 5 + 7 + 9 for L_max = 4
 const int MAX_NUM_N = 20;   // n_max+1 = 19+1
 const int MAX_DIM = MAX_NUM_N * 7;
@@ -792,14 +796,84 @@
   find_q_with_4body(n_max_angular_plus_1, n, s, q);
   double s0_sq = s[0] * s[0];
   double s1_sq_plus_s2_sq = s[1] * s[1] + s[2] * s[2];
   q[5 * n_max_angular_plus_1 + n] = C5B[0] * s0_sq * s0_sq + C5B[1] * s0_sq * s1_sq_plus_s2_sq +
                                     C5B[2] * s1_sq_plus_s2_sq * s1_sq_plus_s2_sq;
 }
 
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+const int table_length = 2001;
+const int table_segments = table_length - 1;
+const double table_resolution = 0.0005;
+
+void find_index_and_weight(
+  const double d12_reduced,
+  int& index_left,
+  int& index_right,
+  double& weight_left,
+  double& weight_right)
+{
+  double d12_index = d12_reduced * table_segments;
+  index_left = int(d12_index);
+  if (index_left == table_segments) {
+    --index_left;
+  }
+  index_right = index_left + 1;
+  weight_right = d12_index - index_left;
+  weight_left = 1.0 - weight_right;
+}
+
+void construct_table_radial_or_angular(
+  const int version,
+  const int num_types,
+  const int num_types_sq,
+  const int n_max,
+  const int basis_size,
+  const double rc,
+  const double rcinv,
+  const double* c,
+  double* gn,
+  double* gnp)
+{
+  for (int table_index = 0; table_index < table_length; ++table_index) {
+    double d12 = table_index * table_resolution * rc;
+    double fc12, fcp12;
+    find_fc_and_fcp(rc, rcinv, d12, fc12, fcp12);
+    for (int t1 = 0; t1 < num_types; ++t1) {
+      for (int t2 = 0; t2 < num_types; ++t2) {
+        int t12 = t1 * num_types + t2;
+        double fn12[MAX_NUM_N];
+        double fnp12[MAX_NUM_N];
+        if (version == 2) {
+          find_fn_and_fnp(n_max, rcinv, d12, fc12, fcp12, fn12, fnp12);
+          for (int n = 0; n <= n_max; ++n) {
+            int index_all = (table_index * num_types_sq + t12) * (n_max + 1) + n;
+            gn[index_all] = fn12[n] * ((num_types == 1) ? 1.0 : c[n * num_types_sq + t12]);
+            gnp[index_all] = fnp12[n] * ((num_types == 1) ? 1.0 : c[n * num_types_sq + t12]);
+          }
+        } else {
+          find_fn_and_fnp(basis_size, rcinv, d12, fc12, fcp12, fn12, fnp12);
+          for (int n = 0; n <= n_max; ++n) {
+            double gn12 = 0.0;
+            double gnp12 = 0.0;
+            for (int k = 0; k <= basis_size; ++k) {
+              gn12 += fn12[k] * c[(n * (basis_size + 1) + k) * num_types_sq + t12];
+              gnp12 += fnp12[k] * c[(n * (basis_size + 1) + k) * num_types_sq + t12];
+            }
+            int index_all = (table_index * num_types_sq + t12) * (n_max + 1) + n;
+            gn[index_all] = gn12;
+            gnp[index_all] = gnp12;
+          }
+        }
+      }
+    }
+  }
+}
+#endif
+
 void find_descriptor_small_box(
   const bool calculating_potential,
   const bool calculating_descriptor,
   const bool calculating_latent_space,
   NEP3::ParaMB& paramb,
   NEP3::ANN& annmb,
   const int N,
@@ -810,29 +884,51 @@
   const int* g_type,
   const double* g_x12_radial,
   const double* g_y12_radial,
   const double* g_z12_radial,
   const double* g_x12_angular,
   const double* g_y12_angular,
   const double* g_z12_angular,
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+  const double* g_gn_radial,
+  const double* g_gn_angular,
+#endif
   double* g_Fp,
   double* g_sum_fxyz,
   double* g_potential,
   double* g_descriptor,
   double* g_latent_space)
 {
+#if defined(_OPENMP)
+#pragma omp parallel for
+#endif
   for (int n1 = 0; n1 < N; ++n1) {
     int t1 = g_type[n1];
     double q[MAX_DIM] = {0.0};
 
     for (int i1 = 0; i1 < g_NN_radial[n1]; ++i1) {
       int index = i1 * N + n1;
       int n2 = g_NL_radial[index];
       double r12[3] = {g_x12_radial[index], g_y12_radial[index], g_z12_radial[index]};
       double d12 = sqrt(r12[0] * r12[0] + r12[1] * r12[1] + r12[2] * r12[2]);
+
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+      int index_left, index_right;
+      double weight_left, weight_right;
+      find_index_and_weight(
+        d12 * paramb.rcinv_radial, index_left, index_right, weight_left, weight_right);
+      int t12 = t1 * paramb.num_types + g_type[n2];
+      for (int n = 0; n <= paramb.n_max_radial; ++n) {
+        q[n] +=
+          g_gn_radial[(index_left * paramb.num_types_sq + t12) * (paramb.n_max_radial + 1) + n] *
+            weight_left +
+          g_gn_radial[(index_right * paramb.num_types_sq + t12) * (paramb.n_max_radial + 1) + n] *
+            weight_right;
+      }
+#else
       double fc12;
       find_fc(paramb.rc_radial, paramb.rcinv_radial, d12, fc12);
       int t2 = g_type[n2];
       double fn12[MAX_NUM_N];
       if (paramb.version == 2) {
         find_fn(paramb.n_max_radial, paramb.rcinv_radial, d12, fc12, fn12);
         for (int n = 0; n <= paramb.n_max_radial; ++n) {
@@ -849,23 +945,37 @@
             int c_index = (n * (paramb.basis_size_radial + 1) + k) * paramb.num_types_sq;
             c_index += t1 * paramb.num_types + t2;
             gn12 += fn12[k] * annmb.c[c_index];
           }
           q[n] += gn12;
         }
       }
+#endif
     }
 
     for (int n = 0; n <= paramb.n_max_angular; ++n) {
       double s[NUM_OF_ABC] = {0.0};
       for (int i1 = 0; i1 < g_NN_angular[n1]; ++i1) {
         int index = i1 * N + n1;
         int n2 = g_NL_angular[index];
         double r12[3] = {g_x12_angular[index], g_y12_angular[index], g_z12_angular[index]};
         double d12 = sqrt(r12[0] * r12[0] + r12[1] * r12[1] + r12[2] * r12[2]);
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+        int index_left, index_right;
+        double weight_left, weight_right;
+        find_index_and_weight(
+          d12 * paramb.rcinv_angular, index_left, index_right, weight_left, weight_right);
+        int t12 = t1 * paramb.num_types + g_type[n2];
+        double gn12 =
+          g_gn_angular[(index_left * paramb.num_types_sq + t12) * (paramb.n_max_angular + 1) + n] *
+            weight_left +
+          g_gn_angular[(index_right * paramb.num_types_sq + t12) * (paramb.n_max_angular + 1) + n] *
+            weight_right;
+        accumulate_s(d12, r12[0], r12[1], r12[2], gn12, s);
+#else
         double fc12;
         find_fc(paramb.rc_angular, paramb.rcinv_angular, d12, fc12);
         int t2 = g_type[n2];
         if (paramb.version == 2) {
           double fn;
           find_fn(n, paramb.rcinv_angular, d12, fc12, fn);
           fn *=
@@ -881,14 +991,15 @@
           for (int k = 0; k <= paramb.basis_size_angular; ++k) {
             int c_index = (n * (paramb.basis_size_angular + 1) + k) * paramb.num_types_sq;
             c_index += t1 * paramb.num_types + t2 + paramb.num_c_radial;
             gn12 += fn12[k] * annmb.c[c_index];
           }
           accumulate_s(d12, r12[0], r12[1], r12[2], gn12, s);
         }
+#endif
       }
       if (paramb.num_L == paramb.L_max) {
         find_q(paramb.n_max_angular + 1, n, s, q + (paramb.n_max_radial + 1));
       } else if (paramb.num_L == paramb.L_max + 1) {
         find_q_with_4body(paramb.n_max_angular + 1, n, s, q + (paramb.n_max_radial + 1));
       } else {
         find_q_with_5body(paramb.n_max_angular + 1, n, s, q + (paramb.n_max_radial + 1));
@@ -939,34 +1050,54 @@
   const int* g_NN,
   const int* g_NL,
   const int* g_type,
   const double* g_x12,
   const double* g_y12,
   const double* g_z12,
   const double* g_Fp,
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+  const double* g_gnp_radial,
+#endif
   double* g_fx,
   double* g_fy,
   double* g_fz,
   double* g_virial)
 {
   for (int n1 = 0; n1 < N; ++n1) {
     int t1 = g_type[n1];
     for (int i1 = 0; i1 < g_NN[n1]; ++i1) {
       int index = i1 * N + n1;
       int n2 = g_NL[index];
       int t2 = g_type[n2];
       double r12[3] = {g_x12[index], g_y12[index], g_z12[index]};
       double d12 = sqrt(r12[0] * r12[0] + r12[1] * r12[1] + r12[2] * r12[2]);
       double d12inv = 1.0 / d12;
+      double f12[3] = {0.0};
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+      int index_left, index_right;
+      double weight_left, weight_right;
+      find_index_and_weight(
+        d12 * paramb.rcinv_radial, index_left, index_right, weight_left, weight_right);
+      int t12 = t1 * paramb.num_types + t2;
+      for (int n = 0; n <= paramb.n_max_radial; ++n) {
+        double gnp12 =
+          g_gnp_radial[(index_left * paramb.num_types_sq + t12) * (paramb.n_max_radial + 1) + n] *
+            weight_left +
+          g_gnp_radial[(index_right * paramb.num_types_sq + t12) * (paramb.n_max_radial + 1) + n] *
+            weight_right;
+        double tmp12 = g_Fp[n1 + n * N] * gnp12 * d12inv;
+        for (int d = 0; d < 3; ++d) {
+          f12[d] += tmp12 * r12[d];
+        }
+      }
+#else
       double fc12, fcp12;
       find_fc_and_fcp(paramb.rc_radial, paramb.rcinv_radial, d12, fc12, fcp12);
       double fn12[MAX_NUM_N];
       double fnp12[MAX_NUM_N];
-
-      double f12[3] = {0.0};
       if (paramb.version == 2) {
         find_fn_and_fnp(paramb.n_max_radial, paramb.rcinv_radial, d12, fc12, fcp12, fn12, fnp12);
         for (int n = 0; n <= paramb.n_max_radial; ++n) {
           double tmp12 = g_Fp[n1 + n * N] * fnp12[n] * d12inv;
           tmp12 *= (paramb.num_types == 1)
                      ? 1.0
                      : annmb.c[(n * paramb.num_types + t1) * paramb.num_types + t2];
@@ -986,14 +1117,15 @@
           }
           double tmp12 = g_Fp[n1 + n * N] * gnp12 * d12inv;
           for (int d = 0; d < 3; ++d) {
             f12[d] += tmp12 * r12[d];
           }
         }
       }
+#endif
 
       if (!is_dipole) {
         g_fx[n1] += f12[0];
         g_fy[n1] += f12[1];
         g_fz[n1] += f12[2];
         g_fx[n2] -= f12[0];
         g_fy[n2] -= f12[1];
@@ -1026,14 +1158,18 @@
   const int* g_NL_angular,
   const int* g_type,
   const double* g_x12,
   const double* g_y12,
   const double* g_z12,
   const double* g_Fp,
   const double* g_sum_fxyz,
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+  const double* g_gn_angular,
+  const double* g_gnp_angular,
+#endif
   double* g_fx,
   double* g_fy,
   double* g_fz,
   double* g_virial)
 {
   for (int n1 = 0; n1 < N; ++n1) {
 
@@ -1049,18 +1185,44 @@
     int t1 = g_type[n1];
 
     for (int i1 = 0; i1 < g_NN_angular[n1]; ++i1) {
       int index = i1 * N + n1;
       int n2 = g_NL_angular[n1 + N * i1];
       double r12[3] = {g_x12[index], g_y12[index], g_z12[index]};
       double d12 = sqrt(r12[0] * r12[0] + r12[1] * r12[1] + r12[2] * r12[2]);
+      double f12[3] = {0.0};
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+      int index_left, index_right;
+      double weight_left, weight_right;
+      find_index_and_weight(
+        d12 * paramb.rcinv_angular, index_left, index_right, weight_left, weight_right);
+      int t12 = t1 * paramb.num_types + g_type[n2];
+      for (int n = 0; n <= paramb.n_max_angular; ++n) {
+        int index_left_all =
+          (index_left * paramb.num_types_sq + t12) * (paramb.n_max_angular + 1) + n;
+        int index_right_all =
+          (index_right * paramb.num_types_sq + t12) * (paramb.n_max_angular + 1) + n;
+        double gn12 =
+          g_gn_angular[index_left_all] * weight_left + g_gn_angular[index_right_all] * weight_right;
+        double gnp12 = g_gnp_angular[index_left_all] * weight_left +
+                       g_gnp_angular[index_right_all] * weight_right;
+        if (paramb.num_L == paramb.L_max) {
+          accumulate_f12(n, paramb.n_max_angular + 1, d12, r12, gn12, gnp12, Fp, sum_fxyz, f12);
+        } else if (paramb.num_L == paramb.L_max + 1) {
+          accumulate_f12_with_4body(
+            n, paramb.n_max_angular + 1, d12, r12, gn12, gnp12, Fp, sum_fxyz, f12);
+        } else {
+          accumulate_f12_with_5body(
+            n, paramb.n_max_angular + 1, d12, r12, gn12, gnp12, Fp, sum_fxyz, f12);
+        }
+      }
+#else
       double fc12, fcp12;
       find_fc_and_fcp(paramb.rc_angular, paramb.rcinv_angular, d12, fc12, fcp12);
       int t2 = g_type[n2];
-      double f12[3] = {0.0};
 
       if (paramb.version == 2) {
         for (int n = 0; n <= paramb.n_max_angular; ++n) {
           double fn;
           double fnp;
           find_fn_and_fnp(n, paramb.rcinv_angular, d12, fc12, fcp12, fn, fnp);
           const double c =
@@ -1093,14 +1255,15 @@
               n, paramb.n_max_angular + 1, d12, r12, gn12, gnp12, Fp, sum_fxyz, f12);
           } else {
             accumulate_f12_with_5body(
               n, paramb.n_max_angular + 1, d12, r12, gn12, gnp12, Fp, sum_fxyz, f12);
           }
         }
       }
+#endif
 
       if (!is_dipole) {
         g_fx[n1] += f12[0];
         g_fy[n1] += f12[1];
         g_fz[n1] += f12[2];
         g_fx[n2] -= f12[0];
         g_fy[n2] -= f12[1];
@@ -1201,14 +1364,18 @@
   NEP3::ANN& annmb,
   int N,
   int* g_ilist,
   int* g_NN,
   int** g_NL,
   int* g_type,
   double** g_pos,
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+  const double* g_gn_radial,
+  const double* g_gn_angular,
+#endif
   double* g_Fp,
   double* g_sum_fxyz,
   double& g_total_potential,
   double* g_potential)
 {
   for (int ii = 0; ii < N; ++ii) {
     int n1 = g_ilist[ii];
@@ -1221,18 +1388,32 @@
         g_pos[n2][0] - g_pos[n1][0], g_pos[n2][1] - g_pos[n1][1], g_pos[n2][2] - g_pos[n1][2]};
 
       double d12sq = r12[0] * r12[0] + r12[1] * r12[1] + r12[2] * r12[2];
       if (d12sq >= paramb.rc_radial * paramb.rc_radial) {
         continue;
       }
       double d12 = sqrt(d12sq);
+      int t2 = g_type[n2] - 1; // from LAMMPS to NEP convention
 
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+      int index_left, index_right;
+      double weight_left, weight_right;
+      find_index_and_weight(
+        d12 * paramb.rcinv_radial, index_left, index_right, weight_left, weight_right);
+      int t12 = t1 * paramb.num_types + t2;
+      for (int n = 0; n <= paramb.n_max_radial; ++n) {
+        q[n] +=
+          g_gn_radial[(index_left * paramb.num_types_sq + t12) * (paramb.n_max_radial + 1) + n] *
+            weight_left +
+          g_gn_radial[(index_right * paramb.num_types_sq + t12) * (paramb.n_max_radial + 1) + n] *
+            weight_right;
+      }
+#else
       double fc12;
       find_fc(paramb.rc_radial, paramb.rcinv_radial, d12, fc12);
-      int t2 = g_type[n2] - 1; // from LAMMPS to NEP convention
       double fn12[MAX_NUM_N];
       if (paramb.version == 2) {
         find_fn(paramb.n_max_radial, paramb.rcinv_radial, d12, fc12, fn12);
         for (int n = 0; n <= paramb.n_max_radial; ++n) {
           double c = (paramb.num_types == 1)
                        ? 1.0
                        : annmb.c[(n * paramb.num_types + t1) * paramb.num_types + t2];
@@ -1246,32 +1427,47 @@
             int c_index = (n * (paramb.basis_size_radial + 1) + k) * paramb.num_types_sq;
             c_index += t1 * paramb.num_types + t2;
             gn12 += fn12[k] * annmb.c[c_index];
           }
           q[n] += gn12;
         }
       }
+#endif
     }
 
     for (int n = 0; n <= paramb.n_max_angular; ++n) {
       double s[NUM_OF_ABC] = {0.0};
       for (int i1 = 0; i1 < g_NN[n1]; ++i1) {
         int n2 = g_NL[n1][i1];
         double r12[3] = {
           g_pos[n2][0] - g_pos[n1][0], g_pos[n2][1] - g_pos[n1][1], g_pos[n2][2] - g_pos[n1][2]};
 
         double d12sq = r12[0] * r12[0] + r12[1] * r12[1] + r12[2] * r12[2];
         if (d12sq >= paramb.rc_angular * paramb.rc_angular) {
           continue;
         }
         double d12 = sqrt(d12sq);
+        int t2 = g_type[n2] - 1; // from LAMMPS to NEP convention
 
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+        int index_left, index_right;
+        double weight_left, weight_right;
+        find_index_and_weight(
+          d12 * paramb.rcinv_angular, index_left, index_right, weight_left, weight_right);
+        int t12 = t1 * paramb.num_types + t2;
+        double gn12 =
+          g_gn_angular[(index_left * paramb.num_types_sq + t12) * (paramb.n_max_angular + 1) + n] *
+            weight_left +
+          g_gn_angular[(index_right * paramb.num_types_sq + t12) * (paramb.n_max_angular + 1) + n] *
+            weight_right;
+        accumulate_s(d12, r12[0], r12[1], r12[2], gn12, s);
+#else
         double fc12;
         find_fc(paramb.rc_angular, paramb.rcinv_angular, d12, fc12);
-        int t2 = g_type[n2] - 1; // from LAMMPS to NEP convention
+
         if (paramb.version == 2) {
           double fn;
           find_fn(n, paramb.rcinv_angular, d12, fc12, fn);
           fn *=
             (paramb.num_types == 1)
               ? 1.0
               : annmb.c
@@ -1284,14 +1480,15 @@
           for (int k = 0; k <= paramb.basis_size_angular; ++k) {
             int c_index = (n * (paramb.basis_size_angular + 1) + k) * paramb.num_types_sq;
             c_index += t1 * paramb.num_types + t2 + paramb.num_c_radial;
             gn12 += fn12[k] * annmb.c[c_index];
           }
           accumulate_s(d12, r12[0], r12[1], r12[2], gn12, s);
         }
+#endif
       }
       if (paramb.num_L == paramb.L_max) {
         find_q(paramb.n_max_angular + 1, n, s, q + (paramb.n_max_radial + 1));
       } else if (paramb.num_L == paramb.L_max + 1) {
         find_q_with_4body(paramb.n_max_angular + 1, n, s, q + (paramb.n_max_radial + 1));
       } else {
         find_q_with_5body(paramb.n_max_angular + 1, n, s, q + (paramb.n_max_radial + 1));
@@ -1327,14 +1524,17 @@
   int N,
   int* g_ilist,
   int* g_NN,
   int** g_NL,
   int* g_type,
   double** g_pos,
   double* g_Fp,
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+  const double* g_gnp_radial,
+#endif
   double** g_force,
   double g_total_virial[6],
   double** g_virial)
 {
   for (int ii = 0; ii < N; ++ii) {
     int n1 = g_ilist[ii];
     int t1 = g_type[n1] - 1; // from LAMMPS to NEP convention
@@ -1345,22 +1545,38 @@
         g_pos[n2][0] - g_pos[n1][0], g_pos[n2][1] - g_pos[n1][1], g_pos[n2][2] - g_pos[n1][2]};
 
       double d12sq = r12[0] * r12[0] + r12[1] * r12[1] + r12[2] * r12[2];
       if (d12sq >= paramb.rc_radial * paramb.rc_radial) {
         continue;
       }
       double d12 = sqrt(d12sq);
-
       double d12inv = 1.0 / d12;
+      double f12[3] = {0.0};
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+      int index_left, index_right;
+      double weight_left, weight_right;
+      find_index_and_weight(
+        d12 * paramb.rcinv_radial, index_left, index_right, weight_left, weight_right);
+      int t12 = t1 * paramb.num_types + t2;
+      for (int n = 0; n <= paramb.n_max_radial; ++n) {
+        double gnp12 =
+          g_gnp_radial[(index_left * paramb.num_types_sq + t12) * (paramb.n_max_radial + 1) + n] *
+            weight_left +
+          g_gnp_radial[(index_right * paramb.num_types_sq + t12) * (paramb.n_max_radial + 1) + n] *
+            weight_right;
+        double tmp12 = g_Fp[n1 + n * N] * gnp12 * d12inv;
+        for (int d = 0; d < 3; ++d) {
+          f12[d] += tmp12 * r12[d];
+        }
+      }
+#else
       double fc12, fcp12;
       find_fc_and_fcp(paramb.rc_radial, paramb.rcinv_radial, d12, fc12, fcp12);
       double fn12[MAX_NUM_N];
       double fnp12[MAX_NUM_N];
-
-      double f12[3] = {0.0};
       if (paramb.version == 2) {
         find_fn_and_fnp(paramb.n_max_radial, paramb.rcinv_radial, d12, fc12, fcp12, fn12, fnp12);
         for (int n = 0; n <= paramb.n_max_radial; ++n) {
           double tmp12 = g_Fp[n1 + n * N] * fnp12[n] * d12inv;
           tmp12 *= (paramb.num_types == 1)
                      ? 1.0
                      : annmb.c[(n * paramb.num_types + t1) * paramb.num_types + t2];
@@ -1380,14 +1596,15 @@
           }
           double tmp12 = g_Fp[n1 + n * N] * gnp12 * d12inv;
           for (int d = 0; d < 3; ++d) {
             f12[d] += tmp12 * r12[d];
           }
         }
       }
+#endif
 
       g_force[n1][0] += f12[0];
       g_force[n1][1] += f12[1];
       g_force[n1][2] += f12[2];
       g_force[n2][0] -= f12[0];
       g_force[n2][1] -= f12[1];
       g_force[n2][2] -= f12[2];
@@ -1421,14 +1638,18 @@
   int* g_ilist,
   int* g_NN,
   int** g_NL,
   int* g_type,
   double** g_pos,
   double* g_Fp,
   double* g_sum_fxyz,
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+  const double* g_gn_angular,
+  const double* g_gnp_angular,
+#endif
   double** g_force,
   double g_total_virial[6],
   double** g_virial)
 {
   for (int ii = 0; ii < N; ++ii) {
     int n1 = g_ilist[ii];
     double Fp[MAX_DIM_ANGULAR] = {0.0};
@@ -1448,20 +1669,45 @@
         g_pos[n2][0] - g_pos[n1][0], g_pos[n2][1] - g_pos[n1][1], g_pos[n2][2] - g_pos[n1][2]};
 
       double d12sq = r12[0] * r12[0] + r12[1] * r12[1] + r12[2] * r12[2];
       if (d12sq >= paramb.rc_angular * paramb.rc_angular) {
         continue;
       }
       double d12 = sqrt(d12sq);
-
-      double fc12, fcp12;
-      find_fc_and_fcp(paramb.rc_angular, paramb.rcinv_angular, d12, fc12, fcp12);
       int t2 = g_type[n2] - 1; // from LAMMPS to NEP convention
       double f12[3] = {0.0};
 
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+      int index_left, index_right;
+      double weight_left, weight_right;
+      find_index_and_weight(
+        d12 * paramb.rcinv_angular, index_left, index_right, weight_left, weight_right);
+      int t12 = t1 * paramb.num_types + t2;
+      for (int n = 0; n <= paramb.n_max_angular; ++n) {
+        int index_left_all =
+          (index_left * paramb.num_types_sq + t12) * (paramb.n_max_angular + 1) + n;
+        int index_right_all =
+          (index_right * paramb.num_types_sq + t12) * (paramb.n_max_angular + 1) + n;
+        double gn12 =
+          g_gn_angular[index_left_all] * weight_left + g_gn_angular[index_right_all] * weight_right;
+        double gnp12 = g_gnp_angular[index_left_all] * weight_left +
+                       g_gnp_angular[index_right_all] * weight_right;
+        if (paramb.num_L == paramb.L_max) {
+          accumulate_f12(n, paramb.n_max_angular + 1, d12, r12, gn12, gnp12, Fp, sum_fxyz, f12);
+        } else if (paramb.num_L == paramb.L_max + 1) {
+          accumulate_f12_with_4body(
+            n, paramb.n_max_angular + 1, d12, r12, gn12, gnp12, Fp, sum_fxyz, f12);
+        } else {
+          accumulate_f12_with_5body(
+            n, paramb.n_max_angular + 1, d12, r12, gn12, gnp12, Fp, sum_fxyz, f12);
+        }
+      }
+#else
+      double fc12, fcp12;
+      find_fc_and_fcp(paramb.rc_angular, paramb.rcinv_angular, d12, fc12, fcp12);
       if (paramb.version == 2) {
         for (int n = 0; n <= paramb.n_max_angular; ++n) {
           double fn;
           double fnp;
           find_fn_and_fnp(n, paramb.rcinv_angular, d12, fc12, fcp12, fn, fnp);
           const double c =
             (paramb.num_types == 1)
@@ -1493,14 +1739,15 @@
               n, paramb.n_max_angular + 1, d12, r12, gn12, gnp12, Fp, sum_fxyz, f12);
           } else {
             accumulate_f12_with_5body(
               n, paramb.n_max_angular + 1, d12, r12, gn12, gnp12, Fp, sum_fxyz, f12);
           }
         }
       }
+#endif
 
       g_force[n1][0] += f12[0];
       g_force[n1][1] += f12[1];
       g_force[n1][2] += f12[2];
       g_force[n2][0] -= f12[0];
       g_force[n2][1] -= f12[1];
       g_force[n2][2] -= f12[2];
@@ -1734,14 +1981,17 @@
   double* g_x12_radial = r12.data();
   double* g_y12_radial = r12.data() + size_x12;
   double* g_z12_radial = r12.data() + size_x12 * 2;
   double* g_x12_angular = r12.data() + size_x12 * 3;
   double* g_y12_angular = r12.data() + size_x12 * 4;
   double* g_z12_angular = r12.data() + size_x12 * 5;
 
+#if defined(_OPENMP)
+#pragma omp parallel for
+#endif
   for (int n1 = 0; n1 < N; ++n1) {
     double x1 = g_x[n1];
     double y1 = g_y[n1];
     double z1 = g_z[n1];
     int count_radial = 0;
     int count_angular = 0;
     for (int n2 = 0; n2 < N; ++n2) {
@@ -2003,14 +2253,19 @@
         : paramb.num_types_sq * (paramb.n_max_radial + paramb.n_max_angular + 2);
   }
   annmb.num_para += num_para_descriptor;
 
   paramb.num_c_radial =
     paramb.num_types_sq * (paramb.n_max_radial + 1) * (paramb.basis_size_radial + 1);
 
+  if (paramb.version == 2) {
+    paramb.num_c_radial =
+      (paramb.num_types == 1) ? 0 : paramb.num_types_sq * (paramb.n_max_radial + 1);
+  }
+
   // NN and descriptor parameters
   parameters.resize(annmb.num_para);
   for (int n = 0; n < annmb.num_para; ++n) {
     tokens = get_tokens(input);
     parameters[n] = get_double_from_token(tokens[0], __FILE__, __LINE__);
   }
   update_potential(parameters.data(), annmb);
@@ -2034,14 +2289,18 @@
       tokens = get_tokens(input);
       zbl.para[d] = get_double_from_token(tokens[0], __FILE__, __LINE__);
     }
     zbl.num_types = paramb.num_types;
   }
   input.close();
 
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+  construct_table(parameters.data());
+#endif
+
   // only report for rank_0
   if (is_rank_0) {
 
     if (paramb.num_types == 1) {
       std::cout << "Use the NEP" << paramb.version << " potential with " << paramb.num_types
                 << " atom type.\n";
     } else {
@@ -2095,14 +2354,35 @@
     ann.w1[t] = pointer;
     pointer += ann.num_neurons1;
   }
   ann.b1 = pointer;
   ann.c = ann.b1 + 1;
 }
 
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+void NEP3::construct_table(double* parameters)
+{
+  gn_radial.resize(table_length * paramb.num_types_sq * (paramb.n_max_radial + 1));
+  gnp_radial.resize(table_length * paramb.num_types_sq * (paramb.n_max_radial + 1));
+  gn_angular.resize(table_length * paramb.num_types_sq * (paramb.n_max_angular + 1));
+  gnp_angular.resize(table_length * paramb.num_types_sq * (paramb.n_max_angular + 1));
+  double* c_pointer =
+    parameters +
+    (annmb.dim + 2) * annmb.num_neurons1 * (paramb.version == 4 ? paramb.num_types : 1) + 1;
+  construct_table_radial_or_angular(
+    paramb.version, paramb.num_types, paramb.num_types_sq, paramb.n_max_radial,
+    paramb.basis_size_radial, paramb.rc_radial, paramb.rcinv_radial, c_pointer, gn_radial.data(),
+    gnp_radial.data());
+  construct_table_radial_or_angular(
+    paramb.version, paramb.num_types, paramb.num_types_sq, paramb.n_max_angular,
+    paramb.basis_size_angular, paramb.rc_angular, paramb.rcinv_angular,
+    c_pointer + paramb.num_c_radial, gn_angular.data(), gnp_angular.data());
+}
+#endif
+
 void NEP3::allocate_memory(const int N)
 {
   if (num_atoms < N) {
     NN_radial.resize(N);
     NL_radial.resize(N * MN);
     NN_angular.resize(N);
     NL_angular.resize(N * MN);
@@ -2156,26 +2436,36 @@
   find_neighbor_list_small_box(
     paramb.rc_radial, paramb.rc_angular, N, box, position, num_cells, ebox, NN_radial, NL_radial,
     NN_angular, NL_angular, r12);
 
   find_descriptor_small_box(
     true, false, false, paramb, annmb, N, NN_radial.data(), NL_radial.data(), NN_angular.data(),
     NL_angular.data(), type.data(), r12.data(), r12.data() + size_x12, r12.data() + size_x12 * 2,
-    r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, Fp.data(),
-    sum_fxyz.data(), potential.data(), nullptr, nullptr);
+    r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5,
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+    gn_radial.data(), gn_angular.data(),
+#endif
+    Fp.data(), sum_fxyz.data(), potential.data(), nullptr, nullptr);
 
   find_force_radial_small_box(
     false, paramb, annmb, N, NN_radial.data(), NL_radial.data(), type.data(), r12.data(),
-    r12.data() + size_x12, r12.data() + size_x12 * 2, Fp.data(), force.data(), force.data() + N,
-    force.data() + N * 2, virial.data());
+    r12.data() + size_x12, r12.data() + size_x12 * 2, Fp.data(),
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+    gnp_radial.data(),
+#endif
+    force.data(), force.data() + N, force.data() + N * 2, virial.data());
 
   find_force_angular_small_box(
     false, paramb, annmb, N, NN_angular.data(), NL_angular.data(), type.data(),
     r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, Fp.data(),
-    sum_fxyz.data(), force.data(), force.data() + N, force.data() + N * 2, virial.data());
+    sum_fxyz.data(),
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+    gn_angular.data(), gnp_angular.data(),
+#endif
+    force.data(), force.data() + N, force.data() + N * 2, virial.data());
 
   if (zbl.enabled) {
     find_force_ZBL_small_box(
       N, zbl, NN_angular.data(), NL_angular.data(), type.data(), r12.data() + size_x12 * 3,
       r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, force.data(), force.data() + N,
       force.data() + N * 2, virial.data(), potential.data());
   }
@@ -2204,16 +2494,19 @@
   find_neighbor_list_small_box(
     paramb.rc_radial, paramb.rc_angular, N, box, position, num_cells, ebox, NN_radial, NL_radial,
     NN_angular, NL_angular, r12);
 
   find_descriptor_small_box(
     false, true, false, paramb, annmb, N, NN_radial.data(), NL_radial.data(), NN_angular.data(),
     NL_angular.data(), type.data(), r12.data(), r12.data() + size_x12, r12.data() + size_x12 * 2,
-    r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, Fp.data(),
-    sum_fxyz.data(), nullptr, descriptor.data(), nullptr);
+    r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5,
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+    gn_radial.data(), gn_angular.data(),
+#endif
+    Fp.data(), sum_fxyz.data(), nullptr, descriptor.data(), nullptr);
 }
 
 void NEP3::find_latent_space(
   const std::vector<int>& type,
   const std::vector<double>& box,
   const std::vector<double>& position,
   std::vector<double>& latent_space)
@@ -2235,16 +2528,19 @@
   find_neighbor_list_small_box(
     paramb.rc_radial, paramb.rc_angular, N, box, position, num_cells, ebox, NN_radial, NL_radial,
     NN_angular, NL_angular, r12);
 
   find_descriptor_small_box(
     false, false, true, paramb, annmb, N, NN_radial.data(), NL_radial.data(), NN_angular.data(),
     NL_angular.data(), type.data(), r12.data(), r12.data() + size_x12, r12.data() + size_x12 * 2,
-    r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, Fp.data(),
-    sum_fxyz.data(), nullptr, nullptr, latent_space.data());
+    r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5,
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+    gn_radial.data(), gn_angular.data(),
+#endif
+    Fp.data(), sum_fxyz.data(), nullptr, nullptr, latent_space.data());
 }
 
 void NEP3::find_dipole(
   const std::vector<int>& type,
   const std::vector<double>& box,
   const std::vector<double>& position,
   std::vector<double>& dipole)
@@ -2271,26 +2567,36 @@
   find_neighbor_list_small_box(
     paramb.rc_radial, paramb.rc_angular, N, box, position, num_cells, ebox, NN_radial, NL_radial,
     NN_angular, NL_angular, r12);
 
   find_descriptor_small_box(
     true, false, false, paramb, annmb, N, NN_radial.data(), NL_radial.data(), NN_angular.data(),
     NL_angular.data(), type.data(), r12.data(), r12.data() + size_x12, r12.data() + size_x12 * 2,
-    r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, Fp.data(),
-    sum_fxyz.data(), potential.data(), nullptr, nullptr);
+    r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5,
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+    gn_radial.data(), gn_angular.data(),
+#endif
+    Fp.data(), sum_fxyz.data(), potential.data(), nullptr, nullptr);
 
   find_force_radial_small_box(
     true, paramb, annmb, N, NN_radial.data(), NL_radial.data(), type.data(), r12.data(),
-    r12.data() + size_x12, r12.data() + size_x12 * 2, Fp.data(), nullptr, nullptr, nullptr,
-    virial.data());
+    r12.data() + size_x12, r12.data() + size_x12 * 2, Fp.data(),
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+    gnp_radial.data(),
+#endif
+    nullptr, nullptr, nullptr, virial.data());
 
   find_force_angular_small_box(
     true, paramb, annmb, N, NN_angular.data(), NL_angular.data(), type.data(),
     r12.data() + size_x12 * 3, r12.data() + size_x12 * 4, r12.data() + size_x12 * 5, Fp.data(),
-    sum_fxyz.data(), nullptr, nullptr, nullptr, virial.data());
+    sum_fxyz.data(),
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+    gn_angular.data(), gnp_angular.data(),
+#endif
+    nullptr, nullptr, nullptr, virial.data());
 
   for (int d = 0; d < 3; ++d) {
     dipole[d] = 0.0;
     for (int n = 0; n < N; ++n) {
       dipole[d] += virial[d * N + n];
     }
   }
@@ -2311,19 +2617,29 @@
 {
   if (num_atoms < N) {
     Fp.resize(N * annmb.dim);
     sum_fxyz.resize(N * (paramb.n_max_angular + 1) * NUM_OF_ABC);
     num_atoms = N;
   }
   find_descriptor_for_lammps(
-    paramb, annmb, N, ilist, NN, NL, type, pos, Fp.data(), sum_fxyz.data(), total_potential,
-    potential);
+    paramb, annmb, N, ilist, NN, NL, type, pos,
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+    gn_radial.data(), gn_angular.data(),
+#endif
+    Fp.data(), sum_fxyz.data(), total_potential, potential);
   find_force_radial_for_lammps(
-    paramb, annmb, N, ilist, NN, NL, type, pos, Fp.data(), force, total_virial, virial);
+    paramb, annmb, N, ilist, NN, NL, type, pos, Fp.data(),
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+    gnp_radial.data(),
+#endif
+    force, total_virial, virial);
   find_force_angular_for_lammps(
-    paramb, annmb, N, ilist, NN, NL, type, pos, Fp.data(), sum_fxyz.data(), force, total_virial,
-    virial);
+    paramb, annmb, N, ilist, NN, NL, type, pos, Fp.data(), sum_fxyz.data(),
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+    gn_angular.data(), gnp_angular.data(),
+#endif
+    force, total_virial, virial);
   if (zbl.enabled) {
     find_force_ZBL_for_lammps(
       zbl, N, ilist, NN, NL, type, pos, force, total_virial, virial, total_potential, potential);
   }
 }
```

### Comparing `calorine-1.6/src/nepy/nep.h` & `calorine-1.7/src/nepy/nep.h`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     along with NEP_CPU.  If not, see <http://www.gnu.org/licenses/>.
 */
 
 #pragma once
 #include <string>
 #include <vector>
 
+// #define USE_TABLE_FOR_RADIAL_FUNCTIONS
+
 class NEP3
 {
 public:
   struct ParaMB {
     int version = 2;
     double rc_radial = 0.0;
     double rc_angular = 0.0;
@@ -128,8 +130,16 @@
   std::vector<double> r12;
   std::vector<double> Fp;
   std::vector<double> sum_fxyz;
   std::vector<double> parameters;
   std::vector<std::string> element_list;
   void update_potential(double* parameters, ANN& ann);
   void allocate_memory(const int N);
+
+#ifdef USE_TABLE_FOR_RADIAL_FUNCTIONS
+  std::vector<double> gn_radial;   // tabulated gn_radial functions
+  std::vector<double> gnp_radial;  // tabulated gnp_radial functions
+  std::vector<double> gn_angular;  // tabulated gn_angular functions
+  std::vector<double> gnp_angular; // tabulated gnp_angular functions
+  void construct_table(double* parameters);
+#endif
 };
```

### Comparing `calorine-1.6/src/nepy/nepy.h` & `calorine-1.7/src/nepy/nepy.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 #include "nep.h"
 using namespace std;
 
 // Local struct to hold an atomic configuration.
-struct Atom
-{
-    int N;
-    std::vector<int> type;
-    std::vector<double> cell, position;
+struct Atom {
+  int N;
+  std::vector<int> type;
+  std::vector<double> cell, position, mass;
 };
 
-class NEPY
-{
+class NEPY {
 private:
-    NEP3 nep;
-    struct Atom atom;
-    std::string potential_filename;
+  NEP3 nep;
+  struct Atom atom;
+  std::string potential_filename;
 
 public:
-    NEPY(const std::string &potential_filename, int N_atoms, std::vector<double> box, std::vector<std::string> atom_symbols, std::vector<double> positions);
-    std::vector<double> getDescriptors();
-    std::vector<double> getDipole();
-    std::vector<double> getLatentSpace();
-    std::tuple<std::vector<double>, std::vector<double>, std::vector<double>> getPotentialForcesAndVirials();
-    std::vector<std::string> _getAtomSymbols(std::string potential_filename);
-    void _convertAtomTypeNEPIndex(int N, std::vector<std::string> atom_symbols, std::vector<std::string> model_atom_symbols, std::vector<int> &type);
-    void setPositions(std::vector<double> positions);
-    void setCell(std::vector<double> cell);
-    void setSymbols(std::vector<std::string> atom_symbols);
+  NEPY(const std::string &potential_filename, int N_atoms,
+       std::vector<double> box, std::vector<std::string> atom_symbols,
+       std::vector<double> positions, std::vector<double> masses);
+  std::vector<double> getDescriptors();
+  std::vector<double> getDipole();
+  std::vector<double> getDipoleGradient(double displacement, int method,
+                                        double charge);
+  std::vector<double> getLatentSpace();
+  std::tuple<std::vector<double>, std::vector<double>, std::vector<double>>
+  getPotentialForcesAndVirials();
+  std::vector<std::string> _getAtomSymbols(std::string potential_filename);
+  void _convertAtomTypeNEPIndex(int N, std::vector<std::string> atom_symbols,
+                                std::vector<std::string> model_atom_symbols,
+                                std::vector<int> &type);
+  void _getCenterOfMass(std::vector<double> center_of_mass);
+  void setPositions(std::vector<double> positions);
+  void setCell(std::vector<double> cell);
+  void setMasses(std::vector<double> masses);
+  void setSymbols(std::vector<std::string> atom_symbols);
 };
```

### Comparing `calorine-1.6/tests/example_files/dipole/dipole_test.out` & `calorine-1.7/tests/example_files/dipole/dipole_test.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_files/dipole/test.xyz` & `calorine-1.7/tests/example_files/dipole/test.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_files/fcp/fcs_order2.in` & `calorine-1.7/tests/example_files/fcp/fcs_order2.in`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_files/fcp/r0.in` & `calorine-1.7/tests/example_files/fcp/r0.in`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_files/hac.out` & `calorine-1.7/tests/example_files/hac.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_files/hac_nan.out` & `calorine-1.7/tests/example_files/hac_nan.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_files/kappa.out` & `calorine-1.7/tests/example_files/kappa.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_files/loss.out` & `calorine-1.7/tests/example_files/loss.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_files/md_no_velocities_or_forces/dump.xyz` & `calorine-1.7/tests/example_files/md_no_velocities_or_forces/dump.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_files/md_velocities_and_forces/dump.xyz` & `calorine-1.7/tests/example_files/md_velocities_and_forces/dump.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_files/nep.txt` & `calorine-1.7/tests/example_files/nep.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_files/thermo_ortho_v3.2.out` & `calorine-1.7/tests/example_files/thermo_ortho_v3.2.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_files/thermo_tri_v3.2.out` & `calorine-1.7/tests/example_files/thermo_tri_v3.2.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_output/CON_NEP2_dummy_CON_3atom_descriptor.out` & `calorine-1.7/tests/example_output/CON_NEP2_dummy_CON_3atom_descriptor.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_output/CO_NEP2_dummy_CO_2atom_descriptor.out` & `calorine-1.7/tests/example_output/CO_NEP2_dummy_CO_2atom_descriptor.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_output/C_NEP2_dummy_C_2atom_descriptor.out` & `calorine-1.7/tests/example_output/C_NEP2_dummy_C_2atom_descriptor.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_descriptor.out` & `calorine-1.7/tests/example_output/PbTe_NEP2_dummy_PbTe_2atom_descriptor.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_descriptor.out` & `calorine-1.7/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_descriptor.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_force.out` & `calorine-1.7/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_force.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_virial.out` & `calorine-1.7/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_250atom_virial.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_descriptor.out` & `calorine-1.7/tests/example_output/nep3_v3.3.1_PbTe_Fan22_PbTe_2atom_descriptor.out`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/example_structures/PbTe_250atom.in` & `calorine-1.7/tests/example_structures/PbTe_250atom.in`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/nep_models/CON_NEP2_dummy.txt` & `calorine-1.7/tests/nep_models/CON_NEP2_dummy.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/nep_models/CO_NEP2_dummy.txt` & `calorine-1.7/tests/nep_models/CO_NEP2_dummy.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/nep_models/C_NEP2_dummy.txt` & `calorine-1.7/tests/nep_models/C_NEP2_dummy.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/nep_models/CsPbI3-SCAN.txt` & `calorine-1.7/tests/nep_models/CsPbI3-SCAN.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/nep_models/PbTe_NEP2_dummy.txt` & `calorine-1.7/tests/nep_models/PbTe_NEP2_dummy.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/nep_models/nep3_v3.2_PbTe_Fan22.txt` & `calorine-1.7/tests/nep_models/nep3_v3.2_PbTe_Fan22.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt` & `calorine-1.7/tests/nep_models/nep3_v3.3.1_PbTe_Fan22.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/nep_models/nep4_PbTe.txt` & `calorine-1.7/tests/nep_models/nep4_PbTe.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/nep_models/nep4_dipole_Christian.txt` & `calorine-1.7/tests/nep_models/nep4_dipole_Christian.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/nep_models/update_expted_descriptors.py` & `calorine-1.7/tests/nep_models/update_expted_descriptors.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def execute_model_in_temporary_directory(model, structure):
     with tempfile.TemporaryDirectory() as tmpdirname:
         print('created temporary directory', tmpdirname)
         # copy structure and model
         shutil.copy(f'{model}.txt', f'{tmpdirname}/nep.txt')
         shutil.copy(f'{structure_dir}/{structure}.in', f'{tmpdirname}/xyz.in')
         # Execute
-        subprocess.Popen(["cat", "xyz.in"],  cwd=tmpdirname)
+        subprocess.Popen(['cat', 'xyz.in'],  cwd=tmpdirname)
         subprocess.Popen([executable, '.'], cwd=tmpdirname).wait()
         # Copy back results
         shutil.copy(f'{tmpdirname}/descriptor.out',
                     f'{output_dir}/{model}_{structure}_descriptor.out')
         shutil.copy(f'{tmpdirname}/force_analytical.out',
                     f'{output_dir}/{model}_{structure}_force.out')
         shutil.copy(f'{tmpdirname}/virial.out',
```

### Comparing `calorine-1.6/tests/test_analysis.py` & `calorine-1.7/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/test_gpumd_io.py` & `calorine-1.7/tests/test_gpumd_io.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/test_gpunep.py` & `calorine-1.7/tests/test_gpunep.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/test_nep3_execution.py` & `calorine-1.7/tests/test_nep3_execution.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/test_nep4_execution.py` & `calorine-1.7/tests/test_nep4_execution.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/test_nep_io.py` & `calorine-1.7/tests/test_nep_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import pytest
 import numpy as np
 from ase.io import read
 from ase import Atoms
 from ase.build import bulk
 from ase.stress import voigt_6_to_full_3x3_stress
 from ase.calculators.lj import LennardJones
-from calorine.nep import (read_loss, read_nepfile,
-                          write_structures, get_parity_data)
+from calorine.nep import read_loss, read_nepfile, write_structures, get_parity_data
 
 
 @pytest.fixture
 def PbTe():
     PbTeBulk = bulk('PbTe', crystalstructure='rocksalt', a=4)
     PbTeBulk[0].position += np.array([0.03, 0.02, 0])
     return PbTeBulk
@@ -18,40 +17,32 @@
 
 @pytest.fixture
 def TenPbTeWithInfo(PbTe):
     n_structures = 10
     structures = []
     for i in range(n_structures):
         # Test with differently sized structures in the test set
-        atoms = PbTe.copy().repeat(i+1)
+        atoms = PbTe.copy().repeat(i + 1)
         natoms = len(atoms)
         atoms.info['energy_target'] = float(i)
         atoms.info['energy_predicted'] = float(i)
-        atoms.info['force_target'] = np.arange(i, natoms*3+i).reshape((natoms, 3))
-        atoms.info['force_predicted'] = np.arange(i, natoms*3+i).reshape((natoms, 3))
-        atoms.info['virial_target'] = -np.arange(i, 6+i).reshape(6)
-        atoms.info['virial_predicted'] = -np.arange(i, 6+i).reshape(6)
-        atoms.info['stress_target'] = -np.arange(i, 6+i).reshape(6)
-        atoms.info['stress_predicted'] = -np.arange(i, 6+i).reshape(6)
+        atoms.info['force_target'] = np.arange(i, natoms * 3 + i).reshape((natoms, 3))
+        atoms.info['force_predicted'] = np.arange(i, natoms * 3 + i).reshape(
+            (natoms, 3)
+        )
+        atoms.info['virial_target'] = -np.arange(i, 6 + i).reshape(6)
+        atoms.info['virial_predicted'] = -np.arange(i, 6 + i).reshape(6)
+        atoms.info['stress_target'] = -np.arange(i, 6 + i).reshape(6)
+        atoms.info['stress_predicted'] = -np.arange(i, 6 + i).reshape(6)
         structures.append(atoms)
     return structures
 
 
 def sel2idx(select: str) -> int:
-    map = {
-        'x': 0,
-        'y': 1,
-        'z': 2,
-        'xx': 0,
-        'yy': 1,
-        'zz': 2,
-        'yz': 3,
-        'xz': 4,
-        'xy': 5
-    }
+    map = {'x': 0, 'y': 1, 'z': 2, 'xx': 0, 'yy': 1, 'zz': 2, 'yz': 3, 'xz': 4, 'xy': 5}
     return map[select]
 
 
 # --- read_nepfile ---
 def test_read_nepfile_unknown_setting(tmpdir):
     """Reads a nep.in file with a comment"""
     p = tmpdir.join('nep.in')
@@ -94,31 +85,47 @@
     assert settings == {}
 
 
 # --- read_loss ---
 def test_read_loss():
     """Reads a loss.out file"""
     loss = read_loss('tests/example_files/loss.out')
-    columns_check = loss.columns == ['total_loss', 'L1', 'L2',
-                                     'RMSE_E_train', 'RMSE_F_train', 'RMSE_V_train',
-                                     'RMSE_E_test', 'RMSE_F_test', 'RMSE_V_test']
+    columns_check = loss.columns == [
+        'total_loss',
+        'L1',
+        'L2',
+        'RMSE_E_train',
+        'RMSE_F_train',
+        'RMSE_V_train',
+        'RMSE_E_test',
+        'RMSE_F_test',
+        'RMSE_V_test',
+    ]
     assert columns_check.all()
     assert isinstance(loss.index[0], int)
     assert loss.index[0] == 100
     assert len(loss) == 95
 
 
 def test_read_loss_single_row(tmpdir):
     """Tries to read a loss.out file that has only a single row"""
     p = tmpdir.join('loss.out')
     p.write('100 2 3 4 5 6 7 8 9 10\n')
     loss = read_loss(str(p))
-    columns_check = loss.columns == ['total_loss', 'L1', 'L2',
-                                     'RMSE_E_train', 'RMSE_F_train', 'RMSE_V_train',
-                                     'RMSE_E_test', 'RMSE_F_test', 'RMSE_V_test']
+    columns_check = loss.columns == [
+        'total_loss',
+        'L1',
+        'L2',
+        'RMSE_E_train',
+        'RMSE_F_train',
+        'RMSE_V_train',
+        'RMSE_E_test',
+        'RMSE_F_test',
+        'RMSE_V_test',
+    ]
     assert columns_check.all()
     assert isinstance(loss.index[0], int)
     assert loss.index[0] == 100
 
 
 def test_read_loss_malformed_file(tmpdir):
     """Tries to read a malformed loss.out file"""
@@ -132,22 +139,31 @@
 # --- write_structures ---
 def test_write_structures_single_structure(tmpdir, PbTe):
     """Writes a structure to a extxyz-file"""
     p = tmpdir.join('train.xyz')
     PbTe.calc = LennardJones()
     write_structures(str(p), [PbTe])
     read_structure = read(str(p), format='extxyz')
-    assert np.isclose(read_structure.cell.volume, PbTe.cell.volume, atol=1e-12, rtol=1e-6)
-    assert np.isclose(read_structure.get_potential_energy(),
-                      PbTe.get_potential_energy(), atol=1e-12, rtol=1e-6)
+    assert np.isclose(
+        read_structure.cell.volume, PbTe.cell.volume, atol=1e-12, rtol=1e-6
+    )
+    assert np.isclose(
+        read_structure.get_potential_energy(),
+        PbTe.get_potential_energy(),
+        atol=1e-12,
+        rtol=1e-6,
+    )
     assert np.allclose(read_structure.positions, PbTe.positions, atol=1e-12, rtol=1e-6)
-    assert np.allclose(read_structure.get_forces(), PbTe.get_forces(), atol=1e-12, rtol=1e-6)
+    assert np.allclose(
+        read_structure.get_forces(), PbTe.get_forces(), atol=1e-12, rtol=1e-6
+    )
     # Written accuracy is around 2e-6
-    assert np.allclose(read_structure.get_stress(),
-                       PbTe.get_stress(voigt=True), atol=1e-12, rtol=1e-5)
+    assert np.allclose(
+        read_structure.get_stress(), PbTe.get_stress(voigt=True), atol=1e-12, rtol=1e-5
+    )
 
 
 def test_write_structures_with_weight(tmpdir, PbTe):
     """Writes structures with weight to an extxyz-file"""
     p = tmpdir.join('train.xyz')
     structure1 = PbTe.copy()
     structure2 = PbTe.copy()
@@ -182,161 +198,208 @@
     C = Atoms('C', positions=[(0, 0, 0)])
     with pytest.raises(RuntimeError) as e:
         write_structures(str(p), [C])
     assert 'Failed to retrieve energy and/or forces for structure' in str(e)
 
 
 def test_write_structure_without_cell(tmpdir):
-    """Tries to write a structure without a calculator attached"""
+    """Tries to write a structure without a proper cell"""
     p = tmpdir.join('train.xyz')
     C = Atoms('C', positions=[(0, 0, 0)])
     C.calc = LennardJones()
     with pytest.raises(ValueError) as e:
         write_structures(str(p), [C])
     assert 'You have 0 lattice vectors: volume not defined' in str(e)
 
 
+def test_write_structure_with_zero_cell_volume(tmpdir):
+    """Tries to write a structure without a proper celld"""
+    p = tmpdir.join('train.xyz')
+    C = Atoms('C', positions=[(0, 0, 0)], cell=[1e-12, 1e-12, 1e-12])
+    C.calc = LennardJones()
+    with pytest.raises(ValueError) as e:
+        write_structures(str(p), [C])
+    assert 'Structure cell must have a non-zero volume' in str(e)
+
+
 # get_parity_data
-@pytest.mark.parametrize('property',
-                         ['energy', 'force', 'virial', 'stress'])
+@pytest.mark.parametrize('property', ['energy', 'force', 'virial', 'stress'])
 def test_get_parity_data(property, TenPbTeWithInfo):
     """Extracts parity data from a list of structures"""
     df = get_parity_data(structures=TenPbTeWithInfo, property=property)
     assert np.all(df.columns == ['predicted', 'target'])
     assert len(df['target']) == 10
     assert len(df['target']) == len(df['predicted'])
     if not property == 'energy':
         assert df['target'][0].shape == df['predicted'][0].shape
 
 
-@pytest.mark.parametrize('property, selection',
-                         [('force', ['x']),
-                          ('virial', ['x', 'y', 'z']),
-                          ('stress', ['xx', 'yy', 'zz'])
-                          ])
+@pytest.mark.parametrize(
+    'property, selection',
+    [('force', ['x']), ('virial', ['x', 'y', 'z']), ('stress', ['xx', 'yy', 'zz'])],
+)
 def test_get_parity_data_diagonal_components(TenPbTeWithInfo, property, selection):
     """Extracts parity data from a list of structures, selecting properties on the diagonal."""
-    df = get_parity_data(structures=TenPbTeWithInfo, property=property, selection=selection)
+    df = get_parity_data(
+        structures=TenPbTeWithInfo, property=property, selection=selection
+    )
     for i, structure in enumerate(TenPbTeWithInfo):
         assert len(df['target'][i]) == len(selection)
         assert len(df['target'][i]) == len(df['predicted'][i])
         for j, select in enumerate(selection):
             if property == 'force':
-                expected_target = structure.info[f'{property}_target'][:, sel2idx(select)]
-                expected_predicted = structure.info[f'{property}_predicted'][:, sel2idx(select)]
+                expected_target = structure.info[f'{property}_target'][
+                    :, sel2idx(select)
+                ]
+                expected_predicted = structure.info[f'{property}_predicted'][
+                    :, sel2idx(select)
+                ]
             elif property in ('virial', 'stress'):
                 expected_target = structure.info[f'{property}_target'][sel2idx(select)]
-                expected_predicted = structure.info[f'{property}_predicted'][sel2idx(select)]
+                expected_predicted = structure.info[f'{property}_predicted'][
+                    sel2idx(select)
+                ]
             assert np.all(df['target'][i][j] == expected_target)
             assert np.all(df['predicted'][i][j] == expected_predicted)
 
 
-@pytest.mark.parametrize('property, selection',
-                         [('virial', ['yz', 'xz', 'xy']),
-                          ('stress', ['yz', 'xz', 'xy'])
-                          ])
+@pytest.mark.parametrize(
+    'property, selection',
+    [('virial', ['yz', 'xz', 'xy']), ('stress', ['yz', 'xz', 'xy'])],
+)
 def test_get_parity_data_off_diagonal_components(TenPbTeWithInfo, property, selection):
     """Extracts parity data from a list of structures, selecting properties on the off-diagonal."""
-    df = get_parity_data(structures=TenPbTeWithInfo, property=property, selection=selection)
+    df = get_parity_data(
+        structures=TenPbTeWithInfo, property=property, selection=selection
+    )
     for i, structure in enumerate(TenPbTeWithInfo):
         assert len(df['target'][i]) == len(selection)
         assert len(df['target'][i]) == len(df['predicted'][i])
         for j, select in enumerate(selection):
             expected_target = structure.info[f'{property}_target'][sel2idx(select)]
-            expected_predicted = structure.info[f'{property}_predicted'][sel2idx(select)]
+            expected_predicted = structure.info[f'{property}_predicted'][
+                sel2idx(select)
+            ]
             assert np.all(df['target'][i][j] == expected_target)
             assert np.all(df['predicted'][i][j] == expected_predicted)
 
 
-@pytest.mark.parametrize('property, selection',
-                         [('force', ['abs']),
-                          ('virial', ['abs']),
-                          ('stress', ['abs'])
-                          ])
+@pytest.mark.parametrize(
+    'property, selection',
+    [('force', ['abs']), ('virial', ['abs']), ('stress', ['abs'])],
+)
 def test_get_parity_data_abs(TenPbTeWithInfo, property, selection):
     """Extracts parity data from a list of structures, calculating the absolute value"""
-    df = get_parity_data(structures=TenPbTeWithInfo, property=property, selection=selection)
+    df = get_parity_data(
+        structures=TenPbTeWithInfo, property=property, selection=selection
+    )
     for i, structure in enumerate(TenPbTeWithInfo):
         assert len(df['target'][i]) == len(selection)
         assert len(df['target'][i]) == len(df['predicted'][i])
         for j, _ in enumerate(selection):
             if property == 'force':
-                expected_target = np.linalg.norm(structure.info[f'{property}_target'], axis=1)
-                expected_predicted = np.linalg.norm(structure.info[f'{property}_predicted'], axis=1)
+                expected_target = np.linalg.norm(
+                    structure.info[f'{property}_target'], axis=1
+                )
+                expected_predicted = np.linalg.norm(
+                    structure.info[f'{property}_predicted'], axis=1
+                )
             elif property in ('virial', 'stress'):
-                expected_target = np.linalg.norm(voigt_6_to_full_3x3_stress(
-                    structure.info[f'{property}_target']))
-                expected_predicted = np.linalg.norm(voigt_6_to_full_3x3_stress(
-                    structure.info[f'{property}_predicted']))
+                expected_target = np.linalg.norm(
+                    voigt_6_to_full_3x3_stress(structure.info[f'{property}_target'])
+                )
+                expected_predicted = np.linalg.norm(
+                    voigt_6_to_full_3x3_stress(structure.info[f'{property}_predicted'])
+                )
             assert np.all(df['target'][i][j] == expected_target)
             assert np.all(df['predicted'][i][j] == expected_predicted)
 
 
-@pytest.mark.parametrize('property, selection',
-                         [('stress', ['pressure'])])
+@pytest.mark.parametrize('property, selection', [('stress', ['pressure'])])
 def test_get_parity_data_pressure(TenPbTeWithInfo, property, selection):
     """Extracts parity data from a list of structures, calculating the pressure"""
-    df = get_parity_data(structures=TenPbTeWithInfo, property=property, selection=selection)
+    df = get_parity_data(
+        structures=TenPbTeWithInfo, property=property, selection=selection
+    )
     for i, structure in enumerate(TenPbTeWithInfo):
         assert len(df['target'][i]) == len(selection)
         assert len(df['target'][i]) == len(df['predicted'][i])
         for j, _ in enumerate(selection):
             expected_target = -np.sum(structure.info[f'{property}_target'][:3]) / 3
-            expected_predicted = -np.sum(structure.info[f'{property}_predicted'][:3]) / 3
+            expected_predicted = (
+                -np.sum(structure.info[f'{property}_predicted'][:3]) / 3
+            )
             assert np.all(df['target'][i][j] == expected_target)
             assert np.all(df['predicted'][i][j] == expected_predicted)
 
 
-@pytest.mark.parametrize('property, selection, output',
-                         [('energy', ['x'],
-                           'Selection does nothing for scalar-valued `energy`.'),
-                          ('force', ['pressure'],
-                          'Cannot calculate pressure for `force`.'),
-                          ('force', ['xy'],
-                          'Selection `xy` is not compatible with property `force`.'),
-                          ('virial', ['zy'],
-                          'Selection `zy` is not allowed.')
-                          ])
-def test_get_parity_data_invalid_selection(TenPbTeWithInfo, property, selection, output):
+@pytest.mark.parametrize(
+    'property, selection, output',
+    [
+        ('energy', ['x'], 'Selection does nothing for scalar-valued `energy`.'),
+        ('force', ['pressure'], 'Cannot calculate pressure for `force`.'),
+        ('force', ['xy'], 'Selection `xy` is not compatible with property `force`.'),
+        ('virial', ['zy'], 'Selection `zy` is not allowed.'),
+    ],
+)
+def test_get_parity_data_invalid_selection(
+    TenPbTeWithInfo, property, selection, output
+):
     """Tries to extract parity data from structures with an invalid selection"""
     with pytest.raises(ValueError) as e:
-        get_parity_data(structures=TenPbTeWithInfo, property=property, selection=selection)
+        get_parity_data(
+            structures=TenPbTeWithInfo, property=property, selection=selection
+        )
     assert output in str(e)
 
 
-@pytest.mark.parametrize('property, output',
-                         [('bounciness',
-                           "`property` must be one of 'energy', 'force', 'virial', 'stress'."),
-                          ])
+@pytest.mark.parametrize(
+    'property, output',
+    [
+        (
+            'bounciness',
+            "`property` must be one of 'energy', 'force', 'virial', 'stress'.",  # noqa
+        ),
+    ],
+)
 def test_get_parity_data_invalid_property(TenPbTeWithInfo, property, output):
     """Tries to extract parity data from structures with an invalid property"""
     with pytest.raises(ValueError) as e:
         get_parity_data(structures=TenPbTeWithInfo, property=property)
     assert output in str(e)
 
 
 def test_get_parity_data_missing_info():
     """Raises error when property(ies) is missing in atom info dictionary"""
     n_structures = 10
     structures = []
     for _ in range(n_structures):
         # Test with differently sized structures in the test set
         natoms = np.random.randint(1, 10)
-        atoms = Atoms('C'*natoms)
+        atoms = Atoms('C' * natoms)
         atoms.info['energy_target'] = 1.0
         structures.append(atoms)
     with pytest.raises(KeyError) as e:
         get_parity_data(structures, property='energy')
     assert 'energy_predicted does not exist in info object!' in str(e)
 
 
-@pytest.mark.parametrize('property, count_wo_flatten, count_with_flatten',
-                         [('energy', 10, 10),
-                          ('force', 10, 18150),
-                          ('virial', 10, 60),
-                          ])
-def test_get_parity_data_flatten(property, count_wo_flatten, count_with_flatten, TenPbTeWithInfo):
+@pytest.mark.parametrize(
+    'property, count_wo_flatten, count_with_flatten',
+    [
+        ('energy', 10, 10),
+        ('force', 10, 18150),
+        ('virial', 10, 60),
+    ],
+)
+def test_get_parity_data_flatten(
+    property, count_wo_flatten, count_with_flatten, TenPbTeWithInfo
+):
     """Checks the option to flatten the data."""
-    df_wo_flatten = get_parity_data(structures=TenPbTeWithInfo, property=property, flatten=False)
+    df_wo_flatten = get_parity_data(
+        structures=TenPbTeWithInfo, property=property, flatten=False
+    )
     assert len(df_wo_flatten) == count_wo_flatten
-    df_with_flatten = get_parity_data(structures=TenPbTeWithInfo, property=property, flatten=True)
+    df_with_flatten = get_parity_data(
+        structures=TenPbTeWithInfo, property=property, flatten=True
+    )
     assert len(df_with_flatten) == count_with_flatten
```

### Comparing `calorine-1.6/tests/test_nep_potential.py` & `calorine-1.7/tests/test_nep_potential.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,24 +146,24 @@
     for fld in ['radial_cutoff', 'angular_cutoff', 'max_neighbors_radial',
                 'max_neighbors_angular', 'n_max_radial', 'l_max', 'n_neuron']:
         assert fld in s
 
 
 def test_read_malformed_potential(tmp_path):
     """Should fail, raising an IOError."""
-    p = tmp_path / "nep.txt"
+    p = tmp_path / 'nep.txt'
     rows = [str(i) for i in range(7)]
     rows.append('invalid parameter')
     text = '\n'.join(rows)
     p.write_text(text)
     with pytest.raises(IOError) as e:
         read_potential(p)
     assert 'Failed to parse line 7 from' in str(e)
 
 
 def test_read_invalid_keyword(tmp_path):
     """Should fail, raising a ValueError."""
-    p = tmp_path / "nep.txt"
+    p = tmp_path / 'nep.txt'
     p.write_text('unknown\n')
     with pytest.raises(ValueError) as e:
         read_potential(p)
     assert 'Unknown field: unknown' in str(e)
```

### Comparing `calorine-1.6/tests/test_phonons.py` & `calorine-1.7/tests/test_phonons.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/test_setup_training.py` & `calorine-1.7/tests/test_setup_training.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/test_stiffness.py` & `calorine-1.7/tests/test_stiffness.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tests/test_structures.py` & `calorine-1.7/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/CsPbI3-SCAN.txt` & `calorine-1.7/tutorials/CsPbI3-SCAN.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/PbTe_NEP3.txt` & `calorine-1.7/tutorials/PbTe_NEP3.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/calculators.ipynb` & `calorine-1.7/tutorials/calculators.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/elastic_stiffness_tensor.ipynb` & `calorine-1.7/tutorials/elastic_stiffness_tensor.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'In the second part we then consider the orthorhombic "*

 * *            'structure of CsPbI$_3$, which allows us to demonstrate the difference between relaxed '*

 * *            "$c_{ij}$ and clamped elastic constants $c_{ij}^0$.\\n')], delete: [2]}}, 20: "*

 * *            "{'source': {insert: [(0, '## CsPbI$_3$\\n'), (5, 'To illustrate this effect, we here "*

 * *            'consider the elastic stiffness tensors in orthorhombic structure of CsPbI$_3$, which '*

 * *            'we descr […]*

```diff
@@ -29,15 +29,15 @@
         {
             "cell_type": "markdown",
             "id": "43ba3fde-7ecc-436a-b0b6-510bf9bdf333",
             "metadata": {},
             "source": [
                 "This tutorial illustrates the calculation of the elastic stiffness tensor $c_{ij}$ and its relation to the sound velocity.\n",
                 "In the first part we use silver in its face-centered cubic (FCC) ground state structure described by an effective medium theory (EMT) potential as a particular simple example.\n",
-                "In the second part we then consider the orthorhombic structure of CsPbI<sub>3</sub>, which allows us to demonstrate the difference between relaxed $c_{ij}$ and clamped elastic constants $c_{ij}^0$.\n",
+                "In the second part we then consider the orthorhombic structure of CsPbI$_3$, which allows us to demonstrate the difference between relaxed $c_{ij}$ and clamped elastic constants $c_{ij}^0$.\n",
                 "\n",
                 "For background on crystal elasticity and the role of symmetry you can consult, e.g., Nye, *Physical Properties of Crystals: Their Representation by Tensors and Matrices*, Oxford University Press (1957)."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "aa3f7c76-8e88-4b4f-86ea-547e67660845",
@@ -298,20 +298,20 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "fcb3b571-11ed-4605-a383-bc80c71371e5",
             "metadata": {},
             "source": [
-                "## CsPbI<sub>3</sub>\n",
+                "## CsPbI$_3$\n",
                 "\n",
                 "In materials with internal degrees of freedom one can distinguish the so-called relaxed $c_{ij}$ and clamped elastic constants $c_{ij}^0$.\n",
                 "In the former case, the ionic positions are allowed to relax after application of a macroscopic strain, whereas in the latter the relative coordinates are kept fixed.\n",
                 "\n",
-                "To illustrate this effect, we here consider the elastic stiffness tensors in orthorhombic structure of CsPbI<sub>3</sub>, which we describe using a neuroevolution potential (NEP) taken from Fransson *et al.*, [arxiv:2301.03497](https://doi.org/10.48550/arXiv.2301.03497)."
+                "To illustrate this effect, we here consider the elastic stiffness tensors in orthorhombic structure of CsPbI$_3$, which we describe using a neuroevolution potential (NEP) taken from Fransson *et al.*, [arxiv:2301.03497](https://doi.org/10.48550/arXiv.2301.03497)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "id": "37012612-3abc-4d5c-99db-489c8d57edd0",
             "metadata": {},
```

### Comparing `calorine-1.6/tutorials/nep-graphite.txt` & `calorine-1.7/tutorials/nep-graphite.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/nep4_dipole.txt` & `calorine-1.7/tutorials/nep4_dipole.txt`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/nep_descriptors.ipynb` & `calorine-1.7/tutorials/nep_descriptors.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/nep_model_inspection.ipynb` & `calorine-1.7/tutorials/nep_model_inspection.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/perovskite-structures/CsPbI3-delta-Pnma.xyz` & `calorine-1.7/tutorials/perovskite-structures/CsPbI3-delta-Pnma.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/perovskite-structures/CsPbI3-orthorhombic-Pnma.xyz` & `calorine-1.7/tutorials/perovskite-structures/CsPbI3-orthorhombic-Pnma.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/perovskite-structures/CsPbI3-tetragonal-I4mcm.xyz` & `calorine-1.7/tutorials/perovskite-structures/CsPbI3-tetragonal-I4mcm.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/perovskite-structures/CsPbI3-tetragonal-P4mbm.xyz` & `calorine-1.7/tutorials/perovskite-structures/CsPbI3-tetragonal-P4mbm.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/phonons.ipynb` & `calorine-1.7/tutorials/phonons.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/structure_relaxation.ipynb` & `calorine-1.7/tutorials/structure_relaxation.ipynb`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/structure_with_dipole.xyz` & `calorine-1.7/tutorials/structure_with_dipole.xyz`

 * *Files identical despite different names*

### Comparing `calorine-1.6/tutorials/thermal_conductivity_from_bte.ipynb` & `calorine-1.7/tutorials/thermal_conductivity_from_bte.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995715082908163%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'Here, we provide an introductory tutorial on how to use "*

 * *            '[phono3py](https://phonopy.github.io/phono3py/) to compute the thermal conductivity '*

 * *            'using a neuroevolution potential (NEP) via the Boltzmann transport equation '*

 * *            "(BTE).\\n'), (3, 'The system under study is graphite represented by a NEP model "*

 * *            "developed in [this paper](https://doi.org/10.48550/arXiv.2304.06978).\\n'), (11, '2. "*

 * *            'Compute the f […]*

```diff
@@ -3,52 +3,50 @@
         {
             "cell_type": "markdown",
             "id": "2e9ac128",
             "metadata": {},
             "source": [
                 "# Thermal conductivity from BTE\n",
                 "\n",
-                "Here, we provide an introductory tutorial on how to use `phono3py <https://phonopy.github.io/phono3py/>`_ to compute the thermal conductivity using a neuroevolution potential (NEP) via the Boltzmann transport equation (BTE).\n",
-                "The system under study is graphite represented by a NEP model developed in `this paper <https://doi.org/10.48550/arXiv.2304.06978>`_.\n",
+                "Here, we provide an introductory tutorial on how to use [phono3py](https://phonopy.github.io/phono3py/) to compute the thermal conductivity using a neuroevolution potential (NEP) via the Boltzmann transport equation (BTE).\n",
+                "The system under study is graphite represented by a NEP model developed in [this paper](https://doi.org/10.48550/arXiv.2304.06978).\n",
                 "Note that `phono3py` also allows you to compute other phonon properties such as, e.g., phonon lifetimes.\n",
                 "\n",
                 "## Workflow\n",
                 "\n",
                 "The steps required are:\n",
                 "\n",
                 "1. Relax the primitive cell\n",
-                "2. Compute the force constants (`fc2.hdf5`, `fc3.hdf5`) using NEP for all structures generated by `phono3py`\n",
+                "2. Compute the force constants (`fc2.hdf5`, `fc3.hdf5`) using the NEP model for all structures generated by `phono3py`\n",
                 "3. Run the thermal conductivity calculation\n",
                 "\n",
                 "Since `phono3py` does not have a python API we will call it through its command line interface via the `os.system` function.\n",
                 "\n",
                 "\n",
                 "## BTE computational parameters\n",
                 "\n",
-                "<div class=\\\"alert alert-block alert-info\\\">\n",
-                "<b>Note 1:</b>\n",
+                "**Note 1:**\n",
                 "In order to achive converged force constants one must use a sufficiently large supercell, the size of which is specified via the `--dim` option.\n",
                 "Here, we, however, use a rather small supercell in order for the tutorial to run faster.\n",
                 "\n",
-                "<b>Note 2:</b>\n",
+                "**Note 2:**\n",
                 "Here, we use the `phono3py` default displacement amplitude of 0.03 \u00c5 when generating supercells for the force-constant extraction.\n",
                 "This may not be suitable for every materials.\n",
                 "\n",
-                "<b>Note 3:</b>\n",
+                "**Note 3:**\n",
                 "In order to achieve convergence of the thermal conductivity one should use a larger q-point mesh (`--mesh`), but here we use a rather small mesh in order for the tutorial to complete within an acceptable time.\n",
                 "\n",
-                "<b>Note 4:</b>\n",
-                "In order to obtain accurate predictions for the thermal conductivity in graphite one should employ the `--lbte` (see `here <https://phonopy.github.io/phono3py/direct-solution.html>`_ for more information).\n",
+                "**Note 4:**\n",
+                "In order to obtain accurate predictions for the thermal conductivity in graphite one should employ the `--lbte` (see [here](https://phonopy.github.io/phono3py/direct-solution.html) for more information).\n",
                 "This method is, however, more costly both computationally and with respect to memory.\n",
                 "For simpliticity we therefore limit ourselves to the relaxation time approximation (RTA), which is invoked via the `--bterta` option.\n",
-                "</div>\n",
                 "\n",
                 "## Miscellaneous\n",
                 "\n",
-                "Additional related tutorials can be found on the `hiphive website <https://hiphive.materialsmodeling.org/tutorial/compute_third_order_properties.html) and [here](https://hiphive.materialsmodeling.org/tutorial/compute_third_order_properties.html>`_."
+                "Additional related tutorials can be found on the [hiphive website](https://hiphive.materialsmodeling.org/tutorial/compute_third_order_properties.html) and [here](https://hiphive.materialsmodeling.org/tutorial/compute_third_order_properties.html)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "757e4176",
             "metadata": {},
@@ -132,15 +130,15 @@
             "id": "f7f9bdfa",
             "metadata": {},
             "source": [
                 "## Construction of force constants\n",
                 "\n",
                 "Next, we construct the force constants.\n",
                 "Here, we use the approach implemented in `phono3py`, which generates the second and third force constants by systematic enumeration and numerical evaluation of the derivatives involved.\n",
-                "Especially for more complex materials, say systems with larger unit cells and/or lower symmetry, it can be beneficial to use regression based approaches such as the one implemented in, e.g., `hiphive <https://hiphive.materialsmodeling.org/>`_.\n",
+                "Especially for more complex materials, say systems with larger unit cells and/or lower symmetry, it can be beneficial to use regression based approaches such as the one implemented in, e.g., [hiphive](https://hiphive.materialsmodeling.org/).\n",
                 "\n",
                 "First, we call `phono3py` to generate a series of configurations (supercells) with systematic displacements."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
```

### Comparing `calorine-1.6/tutorials/visualize_descriptor_space_with_pca.ipynb` & `calorine-1.7/tutorials/visualize_descriptor_space_with_pca.ipynb`

 * *Files identical despite different names*

