# Comparing `tmp/qsolve-0.2.7.tar.gz` & `tmp/qsolve-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsolve-0.2.7.tar", last modified: Wed May 10 12:23:41 2023, max compression
+gzip compressed data, was "qsolve-0.2.8.tar", last modified: Wed May 10 13:12:23 2023, max compression
```

## Comparing `qsolve-0.2.7.tar` & `qsolve-0.2.8.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.110565 qsolve-0.2.7/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       31 2023-05-10 12:21:00.000000 qsolve-0.2.7/MANIFEST.in
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      790 2023-05-10 12:23:41.110565 qsolve-0.2.7/PKG-INFO
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      306 2023-05-04 13:53:12.000000 qsolve-0.2.7/README.md
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       38 2023-05-10 12:23:41.110565 qsolve-0.2.7/setup.cfg
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1078 2023-05-10 12:20:30.000000 qsolve-0.2.7/setup.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.090565 qsolve-0.2.7/src/
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.094565 qsolve-0.2.7/src/qsolve/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       33 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      403 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/constants.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.094565 qsolve-0.2.7/src/qsolve/core/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      258 2023-05-10 12:17:08.000000 qsolve-0.2.7/src/qsolve/core/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2755 2023-05-10 12:16:03.000000 qsolve-0.2.7/src/qsolve/core/fourier.pyc
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     5904 2023-05-10 12:16:03.000000 qsolve-0.2.7/src/qsolve/core/qsolve_core_gpe_1d.pyc
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     6904 2023-05-10 12:16:03.000000 qsolve-0.2.7/src/qsolve/core/qsolve_core_gpe_2d.pyc
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    15510 2023-05-10 12:16:03.000000 qsolve-0.2.7/src/qsolve/core/qsolve_core_gpe_3d.pyc
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.094565 qsolve-0.2.7/src/qsolve/figures/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       41 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.094565 qsolve-0.2.7/src/qsolve/figures/figure_main_1d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       41 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/figure_main_1d/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1868 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/figure_main_1d/fig_control_inputs.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2267 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/figures/figure_main_1d/fig_psi_abs_squared_1d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2607 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/figures/figure_main_1d/fig_psi_re_im_1d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     6056 2023-05-10 09:49:53.000000 qsolve-0.2.7/src/qsolve/figures/figure_main_1d/figure_main_1d.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.098565 qsolve-0.2.7/src/qsolve/figures/style/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/style/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4284 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/style/colors.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      225 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/style/hex2rgb.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1502 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/style/make_cmap.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1279 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/style/mpl_settings.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4727 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/style/mystyle.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      124 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/parameter.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.098565 qsolve-0.2.7/src/qsolve/potentials/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.098565 qsolve-0.2.7/src/qsolve/potentials/components_1d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      194 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/box_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      285 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/gaussian_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      126 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/gaussian_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      192 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/harmonic_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/harmonic_x_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/harmonic_y_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/harmonic_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      160 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/lattice_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2746 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/lesanovsky_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3134 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/lesanovsky_xy_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       64 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/tilt_x_3d.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.102565 qsolve-0.2.7/src/qsolve/potentials/components_2d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      194 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/box_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      213 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/gaussian_2d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       16 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/gaussian_y_2d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      154 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/harmonic_2d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/harmonic_x_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/harmonic_y_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/harmonic_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      160 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/lattice_z_3d.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.102565 qsolve-0.2.7/src/qsolve/potentials/components_3d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      194 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/box_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      285 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/gaussian_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      126 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/gaussian_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      192 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/harmonic_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/harmonic_x_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/harmonic_y_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/harmonic_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      160 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/lattice_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2746 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/lesanovsky_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3134 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/lesanovsky_xy_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       64 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/tilt_x_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      843 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/primes.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.102565 qsolve-0.2.7/src/qsolve/solvers/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      108 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.102565 qsolve-0.2.7/src/qsolve/solvers/solvers_1d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       39 2023-05-08 10:00:10.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_1d/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     7683 2023-05-10 12:15:09.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_1d/solver_gpe_1d.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.102565 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       53 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.106565 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      997 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/chemical_potential.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      860 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/compute_ground_state_solution.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1985 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/densities.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3251 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/energies.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4044 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/getter_functions.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      537 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_device.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1350 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_grid_2d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      587 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_potential.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      461 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_time_evolution.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      471 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/n_atoms.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       83 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/set_V.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      374 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/set_psi.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     5486 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/solver_gpe_2d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1525 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/spectrum.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1248 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/units.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.106565 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       53 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.106565 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      398 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/check_python_version.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1039 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/chemical_potential.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      877 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/compute_ground_state_solution.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1985 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/densities.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3937 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/energies.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     6584 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/getter_functions.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      537 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_device.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1974 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_grid_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      637 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_potential.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      159 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_seed.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      461 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_time_evolution.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1897 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_units.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      489 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/n_atoms.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       83 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/set_V.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      374 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/set_psi.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3308 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/solver_gpe_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1525 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/spectrum.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1110 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/units.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2683 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/units.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.110565 qsolve-0.2.7/src/qsolve/units_backup/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       30 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/units_backup/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1680 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/units_backup/units_1d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      899 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/units_backup/units_2d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1156 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/units_backup/units_3d.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.110565 qsolve-0.2.7/src/qsolve/utils/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/utils/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.094565 qsolve-0.2.7/src/qsolve.egg-info/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      790 2023-05-10 12:23:41.000000 qsolve-0.2.7/src/qsolve.egg-info/PKG-INFO
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     5183 2023-05-10 12:23:41.000000 qsolve-0.2.7/src/qsolve.egg-info/SOURCES.txt
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-05-10 12:23:41.000000 qsolve-0.2.7/src/qsolve.egg-info/dependency_links.txt
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        7 2023-05-10 12:23:41.000000 qsolve-0.2.7/src/qsolve.egg-info/top_level.txt
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.600289 qsolve-0.2.8/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       31 2023-05-10 12:21:00.000000 qsolve-0.2.8/MANIFEST.in
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      807 2023-05-10 13:12:23.596289 qsolve-0.2.8/PKG-INFO
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      306 2023-05-04 13:53:12.000000 qsolve-0.2.8/README.md
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       38 2023-05-10 13:12:23.600289 qsolve-0.2.8/setup.cfg
+-rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1095 2023-05-10 13:12:01.000000 qsolve-0.2.8/setup.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.588289 qsolve-0.2.8/src/
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.588289 qsolve-0.2.8/src/qsolve/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       33 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      403 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/constants.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.592290 qsolve-0.2.8/src/qsolve/core/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      258 2023-05-10 12:17:08.000000 qsolve-0.2.8/src/qsolve/core/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2755 2023-05-10 12:16:03.000000 qsolve-0.2.8/src/qsolve/core/fourier.pyc
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     5904 2023-05-10 12:16:03.000000 qsolve-0.2.8/src/qsolve/core/qsolve_core_gpe_1d.pyc
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     6904 2023-05-10 12:16:03.000000 qsolve-0.2.8/src/qsolve/core/qsolve_core_gpe_2d.pyc
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    15510 2023-05-10 12:16:03.000000 qsolve-0.2.8/src/qsolve/core/qsolve_core_gpe_3d.pyc
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.592290 qsolve-0.2.8/src/qsolve/figures/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       41 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/figures/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.592290 qsolve-0.2.8/src/qsolve/figures/figure_main_1d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       41 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/figures/figure_main_1d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1868 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/figures/figure_main_1d/fig_control_inputs.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2267 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/figures/figure_main_1d/fig_psi_abs_squared_1d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2607 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/figures/figure_main_1d/fig_psi_re_im_1d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     5507 2023-05-10 13:07:49.000000 qsolve-0.2.8/src/qsolve/figures/figure_main_1d/figure_main_1d.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.592290 qsolve-0.2.8/src/qsolve/figures/style/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/figures/style/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4284 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/figures/style/colors.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      225 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/figures/style/hex2rgb.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1502 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/figures/style/make_cmap.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1279 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/figures/style/mpl_settings.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4727 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/figures/style/mystyle.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      124 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/parameter.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.592290 qsolve-0.2.8/src/qsolve/potentials/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.592290 qsolve-0.2.8/src/qsolve/potentials/components_1d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/potentials/components_1d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      194 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/potentials/components_1d/box_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      285 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/potentials/components_1d/gaussian_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      126 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/potentials/components_1d/gaussian_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      192 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/potentials/components_1d/harmonic_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/potentials/components_1d/harmonic_x_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/potentials/components_1d/harmonic_y_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/potentials/components_1d/harmonic_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      160 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/potentials/components_1d/lattice_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2746 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/potentials/components_1d/lesanovsky_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3134 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/potentials/components_1d/lesanovsky_xy_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       64 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/potentials/components_1d/tilt_x_3d.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.592290 qsolve-0.2.8/src/qsolve/potentials/components_2d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_2d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      194 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_2d/box_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      213 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_2d/gaussian_2d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       16 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_2d/gaussian_y_2d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      154 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_2d/harmonic_2d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_2d/harmonic_x_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_2d/harmonic_y_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_2d/harmonic_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      160 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_2d/lattice_z_3d.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.592290 qsolve-0.2.8/src/qsolve/potentials/components_3d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_3d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      194 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_3d/box_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      285 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_3d/gaussian_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      126 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_3d/gaussian_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      192 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_3d/harmonic_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_3d/harmonic_x_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_3d/harmonic_y_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_3d/harmonic_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      160 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_3d/lattice_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2746 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_3d/lesanovsky_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3134 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_3d/lesanovsky_xy_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       64 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/potentials/components_3d/tilt_x_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      843 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/primes.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.592290 qsolve-0.2.8/src/qsolve/solvers/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      108 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.596289 qsolve-0.2.8/src/qsolve/solvers/solvers_1d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       39 2023-05-08 10:00:10.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_1d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     7683 2023-05-10 12:15:09.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_1d/solver_gpe_1d.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.596289 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       53 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.596289 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      997 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/chemical_potential.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      860 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/compute_ground_state_solution.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1985 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/densities.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3251 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/energies.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4044 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/getter_functions.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      537 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_device.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1350 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_grid_2d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      587 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_potential.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      461 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_time_evolution.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      471 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/n_atoms.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       83 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/set_V.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      374 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/set_psi.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     5486 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/solver_gpe_2d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1525 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/spectrum.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1248 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/units.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.596289 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       53 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.596289 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      398 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/check_python_version.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1039 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/chemical_potential.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      877 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/compute_ground_state_solution.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1985 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/densities.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3937 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/energies.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     6584 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/getter_functions.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      537 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_device.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1974 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_grid_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      637 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_potential.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      159 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_seed.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      461 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_time_evolution.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1897 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_units.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      489 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/n_atoms.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       83 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/set_V.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      374 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/set_psi.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3308 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/solver_gpe_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1525 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/spectrum.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1110 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/units.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2683 2023-05-08 08:28:31.000000 qsolve-0.2.8/src/qsolve/units.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.596289 qsolve-0.2.8/src/qsolve/units_backup/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       30 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/units_backup/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1680 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/units_backup/units_1d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      899 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/units_backup/units_2d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1156 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/units_backup/units_3d.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.596289 qsolve-0.2.8/src/qsolve/utils/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.8/src/qsolve/utils/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 13:12:23.588289 qsolve-0.2.8/src/qsolve.egg-info/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      807 2023-05-10 13:12:23.000000 qsolve-0.2.8/src/qsolve.egg-info/PKG-INFO
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     5183 2023-05-10 13:12:23.000000 qsolve-0.2.8/src/qsolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-05-10 13:12:23.000000 qsolve-0.2.8/src/qsolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        7 2023-05-10 13:12:23.000000 qsolve-0.2.8/src/qsolve.egg-info/top_level.txt
```

### Comparing `qsolve-0.2.7/PKG-INFO` & `qsolve-0.2.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: qsolve
-Version: 0.2.7
+Version: 0.2.8
 Summary: Numerical methods for the simulation of ultracold atom experiments
 Home-page: https://github.com/jfmennemann/qsolve
 Author: Jan-Frederik Mennemann
 Author-email: jfmennemann@gmx.de
-Keywords: ultracold atoms,simulations,Gross-Pitaevskii equation,thermal state sampling,time of flight
+Keywords: ultracold atoms,classical fields simulations,Gross-Pitaevskii equation,thermal state sampling,time of flight
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 
 # QSolve
 
 QSolve provides numerical methods for the simulation of ultracold quantum gases
```

### Comparing `qsolve-0.2.7/setup.py` & `qsolve-0.2.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     
     long_description = fh.read()
 
 
 setuptools.setup(
     name="qsolve",
-    version="0.2.7",
+    version="0.2.8",
     url = "https://github.com/jfmennemann/qsolve",
     author="Jan-Frederik Mennemann",
     author_email="jfmennemann@gmx.de",
     description="Numerical methods for the simulation of ultracold atom experiments",
     # long_description=read('README.md'),
     long_description=long_description,
     # long_description_content_type='text/markdown',
@@ -26,10 +26,10 @@
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.10',
     ],
     # package_data={'': ['/qsolve/qsolve/core/*.pyc']},
     # license="MIT",
-    keywords="ultracold atoms, simulations, Gross-Pitaevskii equation, thermal state sampling, time of flight"
+    keywords="ultracold atoms, classical fields simulations, Gross-Pitaevskii equation, thermal state sampling, time of flight"
 )
```

### Comparing `qsolve-0.2.7/src/qsolve/core/fourier.pyc` & `qsolve-0.2.8/src/qsolve/core/fourier.pyc`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/core/qsolve_core_gpe_1d.pyc` & `qsolve-0.2.8/src/qsolve/core/qsolve_core_gpe_1d.pyc`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/core/qsolve_core_gpe_2d.pyc` & `qsolve-0.2.8/src/qsolve/core/qsolve_core_gpe_2d.pyc`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/core/qsolve_core_gpe_3d.pyc` & `qsolve-0.2.8/src/qsolve/core/qsolve_core_gpe_3d.pyc`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/figures/figure_main_1d/fig_control_inputs.py` & `qsolve-0.2.8/src/qsolve/figures/figure_main_1d/fig_control_inputs.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/figures/figure_main_1d/fig_psi_abs_squared_1d.py` & `qsolve-0.2.8/src/qsolve/figures/figure_main_1d/fig_psi_abs_squared_1d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/figures/figure_main_1d/fig_psi_re_im_1d.py` & `qsolve-0.2.8/src/qsolve/figures/figure_main_1d/fig_psi_re_im_1d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/figures/figure_main_1d/figure_main_1d.py` & `qsolve-0.2.8/src/qsolve/figures/figure_main_1d/figure_main_1d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import matplotlib.pyplot as plt
 
-from PyQt5 import QtWidgets
-
 from scipy import constants
 
 import numpy as np
 
 from .fig_psi_abs_squared_1d import fig_psi_abs_squared_1d
 from .fig_psi_re_im_1d import fig_psi_re_im_1d
 
@@ -104,39 +102,24 @@
         # -----------------------------------------------------------------------------------------
         plt.rcParams.update({'font.size': 10})
         # -----------------------------------------------------------------------------------------
 
         # -----------------------------------------------------------------------------------------
         self.fig_name = "figure_main"
                 
-        self.fig = plt.figure(self.fig_name, facecolor="white")
-
-        window = self.fig.canvas.window()
-        
-        window.findChild(QtWidgets.QToolBar).setVisible(False)
-        window.statusBar().setVisible(False)
-        # -----------------------------------------------------------------------------------------
-
-        # -----------------------------------------------------------------------------------------
-        n_pixels_x = 1200
-        n_pixels_y = 800
-
-        pos_x = 2560 - n_pixels_x
-        pos_y = 0
-
-        window.setGeometry(pos_x, pos_y, n_pixels_x, n_pixels_y)
+        self.fig = plt.figure(self.fig_name, figsize=(8, 8), facecolor="white")
         # -----------------------------------------------------------------------------------------
 
         # -----------------------------------------------------------------------------------------
         width_ratios = [1, 1]
 
         self.gridspec = self.fig.add_gridspec(nrows=3, ncols=2,
-                                              left=0.055, right=0.985,
+                                              left=0.1, right=0.9,
                                               bottom=0.08, top=0.95,
-                                              wspace=0.35,
+                                              wspace=0.4,
                                               hspace=0.7,
                                               width_ratios=width_ratios,
                                               height_ratios=[1, 1, 1])
 
         ax_00 = self.fig.add_subplot(self.gridspec[0, 0])
         ax_10 = self.fig.add_subplot(self.gridspec[1, 0])
```

### Comparing `qsolve-0.2.7/src/qsolve/figures/style/colors.py` & `qsolve-0.2.8/src/qsolve/figures/style/colors.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/figures/style/make_cmap.py` & `qsolve-0.2.8/src/qsolve/figures/style/make_cmap.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/figures/style/mpl_settings.py` & `qsolve-0.2.8/src/qsolve/figures/style/mpl_settings.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/figures/style/mystyle.py` & `qsolve-0.2.8/src/qsolve/figures/style/mystyle.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/potentials/components_1d/lesanovsky_3d.py` & `qsolve-0.2.8/src/qsolve/potentials/components_1d/lesanovsky_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/potentials/components_1d/lesanovsky_xy_3d.py` & `qsolve-0.2.8/src/qsolve/potentials/components_1d/lesanovsky_xy_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/potentials/components_3d/lesanovsky_3d.py` & `qsolve-0.2.8/src/qsolve/potentials/components_3d/lesanovsky_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/potentials/components_3d/lesanovsky_xy_3d.py` & `qsolve-0.2.8/src/qsolve/potentials/components_3d/lesanovsky_xy_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/primes.py` & `qsolve-0.2.8/src/qsolve/primes.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_1d/solver_gpe_1d.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_1d/solver_gpe_1d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/chemical_potential.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/chemical_potential.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/compute_ground_state_solution.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/compute_ground_state_solution.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/densities.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/densities.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/energies.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/energies.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/getter_functions.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/getter_functions.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_device.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_device.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_grid_2d.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_grid_2d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_potential.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_potential.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/solver_gpe_2d.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/solver_gpe_2d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/spectrum.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/spectrum.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/units.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_2d/solver_gpe_2d/units.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/chemical_potential.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/chemical_potential.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/compute_ground_state_solution.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/compute_ground_state_solution.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/densities.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/densities.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/energies.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/energies.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/getter_functions.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/getter_functions.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_device.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_device.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_grid_3d.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_grid_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_potential.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_potential.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_units.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_units.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/solver_gpe_3d.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/solver_gpe_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/spectrum.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/spectrum.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/units.py` & `qsolve-0.2.8/src/qsolve/solvers/solvers_3d/solver_gpe_3d/units.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/units.py` & `qsolve-0.2.8/src/qsolve/units.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/units_backup/units_1d.py` & `qsolve-0.2.8/src/qsolve/units_backup/units_1d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/units_backup/units_2d.py` & `qsolve-0.2.8/src/qsolve/units_backup/units_2d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve/units_backup/units_3d.py` & `qsolve-0.2.8/src/qsolve/units_backup/units_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.7/src/qsolve.egg-info/PKG-INFO` & `qsolve-0.2.8/src/qsolve.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: qsolve
-Version: 0.2.7
+Version: 0.2.8
 Summary: Numerical methods for the simulation of ultracold atom experiments
 Home-page: https://github.com/jfmennemann/qsolve
 Author: Jan-Frederik Mennemann
 Author-email: jfmennemann@gmx.de
-Keywords: ultracold atoms,simulations,Gross-Pitaevskii equation,thermal state sampling,time of flight
+Keywords: ultracold atoms,classical fields simulations,Gross-Pitaevskii equation,thermal state sampling,time of flight
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 
 # QSolve
 
 QSolve provides numerical methods for the simulation of ultracold quantum gases
```

### Comparing `qsolve-0.2.7/src/qsolve.egg-info/SOURCES.txt` & `qsolve-0.2.8/src/qsolve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

