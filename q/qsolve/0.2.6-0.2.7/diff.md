# Comparing `tmp/qsolve-0.2.6.tar.gz` & `tmp/qsolve-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsolve-0.2.6.tar", last modified: Wed Apr 26 08:44:41 2023, max compression
+gzip compressed data, was "qsolve-0.2.7.tar", last modified: Wed May 10 12:23:41 2023, max compression
```

## Comparing `qsolve-0.2.6.tar` & `qsolve-0.2.7.tar`

### file list

```diff
@@ -1,187 +1,130 @@
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.278969 qsolve-0.2.6/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       30 2023-04-21 08:03:18.000000 qsolve-0.2.6/MANIFEST.in
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      790 2023-04-26 08:44:41.278969 qsolve-0.2.6/PKG-INFO
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      306 2023-04-21 08:33:35.000000 qsolve-0.2.6/README.md
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       38 2023-04-26 08:44:41.278969 qsolve-0.2.6/setup.cfg
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1078 2023-04-26 08:44:35.000000 qsolve-0.2.6/setup.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.258969 qsolve-0.2.6/src/
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.258969 qsolve-0.2.6/src/qsolve/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.262969 qsolve-0.2.6/src/qsolve/core/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       33 2023-04-26 07:07:03.000000 qsolve-0.2.6/src/qsolve/core/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)  1122464 2023-04-26 08:16:08.000000 qsolve-0.2.6/src/qsolve/core/qsolve_core_gpe_3d.cpython-310-x86_64-linux-gnu.so
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.262969 qsolve-0.2.6/src/qsolve/examples/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.262969 qsolve-0.2.6/src/qsolve/examples/examples_3d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.262969 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     9301 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/evaluation.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.262969 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.266969 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        2 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1527 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_control_inputs.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1466 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1093 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_xy.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1120 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_xz.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1609 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_y.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1517 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1260 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_global_phase_difference.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1235 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_number_imbalance.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      905 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_xy.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      982 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_xz.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1205 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_z_x1_x2.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1785 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1516 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_y.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1880 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    11931 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/figure_main.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.266969 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4527 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/colors.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      225 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/hex2rgb.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1502 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/make_cmap.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1279 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/mpl_settings.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4727 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/mystyle.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.266969 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/frames/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/frames/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    12119 2023-04-26 07:20:39.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/main_ground_state_computation.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      695 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/potential_harmonic.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.266969 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     8374 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/evaluation.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.266969 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.270969 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        2 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1527 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_control_inputs.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1466 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1101 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_xy.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1128 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_xz.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1609 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_y.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1841 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1260 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_global_phase_difference.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1247 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_number_imbalance.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      905 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_xy.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      982 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_xz.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1205 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_z_x1_x2.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    12277 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/figure_main.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.270969 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1212 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_mask_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1216 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_tof_final.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1160 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1228 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_mask_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1216 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_tof_final.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1172 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     9121 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/figure_tof.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.270969 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1212 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_mask_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1216 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_tof_final.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1160 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1228 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_mask_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1216 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_tof_final.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1172 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1263 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xy_mask_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1259 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xy_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1299 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xz_mask_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1259 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xz_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    10384 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/figure_tof_extended.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.270969 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4527 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/colors.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      225 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/hex2rgb.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1502 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/make_cmap.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1279 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/mpl_settings.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4727 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/mystyle.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.270969 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/frames/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/frames/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    21115 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_tilt_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    17753 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_xy_tilt_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    17874 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_xy_tilt_x_box_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2138 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_tilt_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1961 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_xy_tilt_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2371 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_xy_tilt_x_box_z.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.274969 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4566 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/evaluation.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.274969 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.274969 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        2 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2247 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_control_inputs.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1466 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1105 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_xy.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1064 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_xz.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1670 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_y.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1404 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1535 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_z_eff.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1663 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_phase_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1884 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_phase_z_eff.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1785 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1033 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_xy.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      940 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_xz.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1516 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_y.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1880 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    11597 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/figure_main.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.274969 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4527 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/colors.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      225 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/hex2rgb.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1502 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/make_cmap.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1279 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/mpl_settings.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4727 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/mystyle.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.274969 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/frames/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/frames/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    13033 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/main_harmonic_xy_gaussian_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    12883 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/main_harmonic_xy_lattice_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1369 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/potential_harmonic_xy_gaussian_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1325 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/potential_harmonic_xy_lattice_z.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.274969 qsolve-0.2.6/src/qsolve/potentials/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.278969 qsolve-0.2.6/src/qsolve/potentials/components_3d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/components_3d/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      194 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/components_3d/box_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      285 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/components_3d/gaussian_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      126 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/components_3d/gaussian_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      192 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/components_3d/harmonic_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/components_3d/harmonic_x_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/components_3d/harmonic_y_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/components_3d/harmonic_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      160 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/components_3d/lattice_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2746 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/components_3d/lesanovsky_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3134 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/components_3d/lesanovsky_xy_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       64 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/potentials/components_3d/tilt_x_3d.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.278969 qsolve-0.2.6/src/qsolve/solvers/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       36 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.278969 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       53 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.278969 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      398 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/check_python_version.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1039 2023-04-26 07:57:30.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/chemical_potential.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      877 2023-04-26 07:56:21.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/compute_ground_state_solution.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1985 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/densities.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3937 2023-04-26 07:59:00.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/energies.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     6584 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/getter_functions.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      537 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_device.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1980 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_grid_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      637 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_potential.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      159 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_seed.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      461 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_time_evolution.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1897 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_units.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      489 2023-04-19 10:18:35.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/n_atoms.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       83 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/set_V.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      374 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/set_psi.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3308 2023-04-19 10:17:25.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/solver_gpe_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1525 2023-04-26 08:25:51.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/spectrum.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1110 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/units.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.278969 qsolve-0.2.6/src/qsolve/utils/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/utils/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      843 2023-04-06 16:50:20.000000 qsolve-0.2.6/src/qsolve/utils/primes.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-26 08:44:41.262969 qsolve-0.2.6/src/qsolve.egg-info/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      790 2023-04-26 08:44:41.000000 qsolve-0.2.6/src/qsolve.egg-info/PKG-INFO
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    11797 2023-04-26 08:44:41.000000 qsolve-0.2.6/src/qsolve.egg-info/SOURCES.txt
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-04-26 08:44:41.000000 qsolve-0.2.6/src/qsolve.egg-info/dependency_links.txt
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        7 2023-04-26 08:44:41.000000 qsolve-0.2.6/src/qsolve.egg-info/top_level.txt
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.110565 qsolve-0.2.7/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       31 2023-05-10 12:21:00.000000 qsolve-0.2.7/MANIFEST.in
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      790 2023-05-10 12:23:41.110565 qsolve-0.2.7/PKG-INFO
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      306 2023-05-04 13:53:12.000000 qsolve-0.2.7/README.md
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       38 2023-05-10 12:23:41.110565 qsolve-0.2.7/setup.cfg
+-rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1078 2023-05-10 12:20:30.000000 qsolve-0.2.7/setup.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.090565 qsolve-0.2.7/src/
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.094565 qsolve-0.2.7/src/qsolve/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       33 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      403 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/constants.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.094565 qsolve-0.2.7/src/qsolve/core/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      258 2023-05-10 12:17:08.000000 qsolve-0.2.7/src/qsolve/core/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2755 2023-05-10 12:16:03.000000 qsolve-0.2.7/src/qsolve/core/fourier.pyc
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     5904 2023-05-10 12:16:03.000000 qsolve-0.2.7/src/qsolve/core/qsolve_core_gpe_1d.pyc
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     6904 2023-05-10 12:16:03.000000 qsolve-0.2.7/src/qsolve/core/qsolve_core_gpe_2d.pyc
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    15510 2023-05-10 12:16:03.000000 qsolve-0.2.7/src/qsolve/core/qsolve_core_gpe_3d.pyc
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.094565 qsolve-0.2.7/src/qsolve/figures/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       41 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.094565 qsolve-0.2.7/src/qsolve/figures/figure_main_1d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       41 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/figure_main_1d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1868 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/figure_main_1d/fig_control_inputs.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2267 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/figures/figure_main_1d/fig_psi_abs_squared_1d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2607 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/figures/figure_main_1d/fig_psi_re_im_1d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     6056 2023-05-10 09:49:53.000000 qsolve-0.2.7/src/qsolve/figures/figure_main_1d/figure_main_1d.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.098565 qsolve-0.2.7/src/qsolve/figures/style/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/style/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4284 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/style/colors.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      225 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/style/hex2rgb.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1502 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/style/make_cmap.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1279 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/style/mpl_settings.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4727 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/figures/style/mystyle.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      124 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/parameter.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.098565 qsolve-0.2.7/src/qsolve/potentials/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.098565 qsolve-0.2.7/src/qsolve/potentials/components_1d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      194 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/box_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      285 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/gaussian_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      126 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/gaussian_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      192 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/harmonic_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/harmonic_x_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/harmonic_y_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/harmonic_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      160 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/lattice_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2746 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/lesanovsky_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3134 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/lesanovsky_xy_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       64 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/potentials/components_1d/tilt_x_3d.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.102565 qsolve-0.2.7/src/qsolve/potentials/components_2d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      194 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/box_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      213 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/gaussian_2d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       16 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/gaussian_y_2d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      154 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/harmonic_2d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/harmonic_x_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/harmonic_y_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/harmonic_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      160 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_2d/lattice_z_3d.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.102565 qsolve-0.2.7/src/qsolve/potentials/components_3d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      194 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/box_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      285 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/gaussian_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      126 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/gaussian_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      192 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/harmonic_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/harmonic_x_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/harmonic_y_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/harmonic_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      160 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/lattice_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2746 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/lesanovsky_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3134 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/lesanovsky_xy_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       64 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/potentials/components_3d/tilt_x_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      843 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/primes.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.102565 qsolve-0.2.7/src/qsolve/solvers/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      108 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.102565 qsolve-0.2.7/src/qsolve/solvers/solvers_1d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       39 2023-05-08 10:00:10.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_1d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     7683 2023-05-10 12:15:09.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_1d/solver_gpe_1d.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.102565 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       53 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.106565 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      997 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/chemical_potential.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      860 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/compute_ground_state_solution.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1985 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/densities.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3251 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/energies.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4044 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/getter_functions.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      537 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_device.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1350 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_grid_2d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      587 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_potential.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      461 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_time_evolution.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      471 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/n_atoms.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       83 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/set_V.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      374 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/set_psi.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     5486 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/solver_gpe_2d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1525 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/spectrum.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1248 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/units.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.106565 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       53 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.106565 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      398 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/check_python_version.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1039 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/chemical_potential.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      877 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/compute_ground_state_solution.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1985 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/densities.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3937 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/energies.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     6584 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/getter_functions.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      537 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_device.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1974 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_grid_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      637 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_potential.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      159 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_seed.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      461 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_time_evolution.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1897 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_units.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      489 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/n_atoms.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       83 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/set_V.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      374 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/set_psi.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3308 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/solver_gpe_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1525 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/spectrum.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1110 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/units.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2683 2023-05-08 08:28:31.000000 qsolve-0.2.7/src/qsolve/units.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.110565 qsolve-0.2.7/src/qsolve/units_backup/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       30 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/units_backup/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1680 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/units_backup/units_1d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      899 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/units_backup/units_2d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1156 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/units_backup/units_3d.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.110565 qsolve-0.2.7/src/qsolve/utils/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-04 13:53:12.000000 qsolve-0.2.7/src/qsolve/utils/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-05-10 12:23:41.094565 qsolve-0.2.7/src/qsolve.egg-info/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      790 2023-05-10 12:23:41.000000 qsolve-0.2.7/src/qsolve.egg-info/PKG-INFO
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     5183 2023-05-10 12:23:41.000000 qsolve-0.2.7/src/qsolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-05-10 12:23:41.000000 qsolve-0.2.7/src/qsolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        7 2023-05-10 12:23:41.000000 qsolve-0.2.7/src/qsolve.egg-info/top_level.txt
```

### Comparing `qsolve-0.2.6/PKG-INFO` & `qsolve-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsolve
-Version: 0.2.6
+Version: 0.2.7
 Summary: Numerical methods for the simulation of ultracold atom experiments
 Home-page: https://github.com/jfmennemann/qsolve
 Author: Jan-Frederik Mennemann
 Author-email: jfmennemann@gmx.de
 Keywords: ultracold atoms,simulations,Gross-Pitaevskii equation,thermal state sampling,time of flight
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qsolve-0.2.6/setup.py` & `qsolve-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     
     long_description = fh.read()
 
 
 setuptools.setup(
     name="qsolve",
-    version="0.2.6",
+    version="0.2.7",
     url = "https://github.com/jfmennemann/qsolve",
     author="Jan-Frederik Mennemann",
     author_email="jfmennemann@gmx.de",
     description="Numerical methods for the simulation of ultracold atom experiments",
     # long_description=read('README.md'),
     long_description=long_description,
     # long_description_content_type='text/markdown',
```

### Comparing `qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/colors.py` & `qsolve-0.2.7/src/qsolve/figures/style/colors.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 # -------------------------------------------------------------------------------------------------
 black = '#000000'
 white = '#ffffff'
 # -------------------------------------------------------------------------------------------------
 
 
-
 # flat_ui_palette_v1
 
 peter_river = '#3498db'
 wet_asphalt = '#34495e'
 orange      = '#f39c12'
 alizarin    = '#e74c3c'
 emerald     = '#2ecc71'
@@ -77,41 +76,35 @@
 colors = [black_rgb, wisteria_rgb, belize_hole_rgb, peter_river_rgb, white_rgb]
 
 positions = [0.0, 0.2, 0.5, 0.6, 1.0]
 
 cmap_density = make_cmap(colors, positions=positions)
 # -------------------------------------------------------------------------------------------------
 
+
 # -------------------------------------------------------------------------------------------------
 # colormap real part
 
-# colors_tmp = [radical_red_rgb, black_rgb, peter_river_rgb]
-# positions_tmp = [0.0, 0.5, 1.0]
-#
-# cmap_real_part = make_cmap(colors_tmp, positions=positions_tmp)
-#
-# color_1_tmp = cmap_real_part(0.25)
-# color_2_tmp = cmap_real_part(0.75)
-#
-# colors_tmp = [radical_red_rgb, color_1_tmp, black_rgb, color_2_tmp, peter_river_rgb]
-# positions_tmp = [0.0, 0.4, 0.5, 0.6, 1.0]
-#
-# cmap_real_part = make_cmap(colors_tmp, positions=positions_tmp)
+colors_tmp = [radical_red_rgb, black_rgb, peter_river_rgb]
+positions_tmp = [0.0, 0.5, 1.0]
 
-cmap_real = matplotlib.cm.PRGn
-# -------------------------------------------------------------------------------------------------
+cmap_real_part = make_cmap(colors_tmp, positions=positions_tmp)
 
-# -------------------------------------------------------------------------------------------------
-# colormap imaginary part
+color_1_tmp = cmap_real_part(0.25)
+color_2_tmp = cmap_real_part(0.75)
 
-cmap_imag = matplotlib.cm.PRGn
-# -------------------------------------------------------------------------------------------------
+colors_tmp = [radical_red_rgb, color_1_tmp, black_rgb, color_2_tmp, peter_river_rgb]
+positions_tmp = [0.0, 0.4, 0.5, 0.6, 1.0]
 
+cmap_real_part = make_cmap(colors_tmp, positions=positions_tmp)
 
+# cmap_real = matplotlib.cm.PRGn
 
+cmap_real_part = matplotlib.cm.RdBu
+# -------------------------------------------------------------------------------------------------
 
 # cmap = matplotlib.cm.PiYG
 # cmap = matplotlib.cm.PRGn
 # cmap = matplotlib.cm.RdGy
 # cmap = matplotlib.cm.RdBu
 # cmap = matplotlib.cm.RdYlBu
 # cmap = matplotlib.cm.bwr
```

### Comparing `qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/make_cmap.py` & `qsolve-0.2.7/src/qsolve/figures/style/make_cmap.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/mpl_settings.py` & `qsolve-0.2.7/src/qsolve/figures/style/mpl_settings.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/mystyle.py` & `qsolve-0.2.7/src/qsolve/figures/style/mystyle.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_z.py` & `qsolve-0.2.7/src/qsolve/figures/figure_main_1d/fig_psi_abs_squared_1d.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,64 @@
+import numpy as np
+
 from numpy import zeros_like
 
 from numpy import pi
 
 from .. style import colors
 
 
-class fig_density_z(object):
+class fig_psi_abs_squared_1d(object):
 
     def __init__(self, ax, settings):
 
         self.hbar = settings.hbar
 
-        self.m_atom = settings.m_atom
-
-        self.line_density_z_x1, = ax.plot(settings.z, zeros_like(settings.z), linewidth=1, linestyle='-',
-                                          color=colors.peter_river, label=r'$|\psi(x_1, 0, z)|^2$')
+        # -----------------------------------------------------------------------------------------
+        self.line_density, = ax.plot(
+            settings.x, zeros_like(settings.x), linewidth=1, linestyle='-',
+            color=colors.wet_asphalt, label=r'$\rho$')
 
-        self.line_density_z_x2, = ax.plot(settings.z, zeros_like(settings.z), linewidth=1, linestyle='-',
-                                          color=colors.wet_asphalt, label=r'$|\psi(x_2, 0, z)|^2$')
-
-        ax.set_xlim(settings.z_min, settings.z_max)
+        ax.set_xlim(settings.x_min, settings.x_max)
         
         ax.set_ylim(settings.density_min, settings.density_max)
 
-        ax.set_xlabel(settings.label_z)
+        ax.set_xlabel(settings.label_x)
         
-        ax.set_xticks(settings.z_ticks)
+        ax.set_xticks(settings.x_ticks)
         
         ax.grid(visible=True, which='major', color=settings.color_gridlines_major, linestyle='-', linewidth=0.5)
         
-        ax.set_ylabel(settings.label_density)
+        ax.set_ylabel(r'$\mu \mathrm{m}^{-1}$', labelpad=0)
+        # -----------------------------------------------------------------------------------------
+
+        # -----------------------------------------------------------------------------------------
+        ax2 = ax.twinx()
 
-        ax_V_z_x1 = ax.twinx()
+        self.line_V, = ax2.plot(
+            settings.x, zeros_like(settings.x), linewidth=settings.linewidth_V, linestyle='-',
+            color=settings.linecolor_V, label=r'$V$')
 
-        self.line_V_z_x1, = ax_V_z_x1.plot(settings.z, zeros_like(settings.z), linewidth=1, linestyle='-',
-                                           color=colors.sun_flower, label=r'$V(x_1, 0, z)$')
+        ax2.set_xlim(settings.x_min, settings.x_max)
+        ax2.set_ylim(settings.V_min, settings.V_max)
 
-        ax_V_z_x1.set_xlim(settings.z_min, settings.z_max)
-        ax_V_z_x1.set_ylim(settings.V_min, settings.V_max)
+        ax2.set_ylabel(r'$h \times \mathrm{kHz}$', labelpad=10)
+        # -----------------------------------------------------------------------------------------
 
-        ax_V_z_x1.set_ylabel(settings.label_V)
+        # -----------------------------------------------------------------------------------------
+        lines, labels = ax.get_legend_handles_labels()
+        lines2, labels2 = ax2.get_legend_handles_labels()
+        ax2.legend(lines + lines2, labels + labels2,
+                   loc='upper right', bbox_to_anchor=(1.0, 1.25), fancybox=True, framealpha=1, ncol=1)
+        # -----------------------------------------------------------------------------------------
 
-        ax_V_z_x1.legend(loc='upper right', bbox_to_anchor=(1.0, 1.0), fancybox=False, framealpha=1.0, ncol=1)
+    def update(self, psi, V):
 
-    def update(self, density_z_x1, density_z_x2, V_z_x1):
+        density = np.abs(psi)**2
 
         scaling_V = self.hbar * 2 * pi * 1000
 
-        V_z_x1 = V_z_x1 / scaling_V
+        V = V / scaling_V
 
-        self.line_density_z_x1.set_ydata(density_z_x1)
-        self.line_density_z_x2.set_ydata(density_z_x2)
+        self.line_density.set_ydata(density / 1e6)
 
-        self.line_V_z_x1.set_ydata(V_z_x1)
+        self.line_V.set_ydata(V)
```

### Comparing `qsolve-0.2.6/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_phase_z_eff.py` & `qsolve-0.2.7/src/qsolve/figures/figure_main_1d/fig_psi_re_im_1d.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,72 @@
 import numpy as np
 
 from numpy import zeros_like
 
 from numpy import pi
 
+import math
+
 from .. style import colors
 
 
-class fig_phase_z_eff(object):
+class fig_psi_re_im_1d(object):
 
     def __init__(self, ax, settings):
 
         self.hbar = settings.hbar
 
-        self.m_atom = settings.m_atom
+        # -----------------------------------------------------------------------------------------
+        self.line_psi_re, = ax.plot(
+            settings.x, zeros_like(settings.x), linewidth=1, linestyle='-',
+            color=colors.wet_asphalt, label=r'$\operatorname{Re}{\psi}$')
+
+        self.line_psi_im, = ax.plot(
+            settings.x, zeros_like(settings.x), linewidth=1, linestyle='--',
+            color=colors.wet_asphalt, label=r'$\operatorname{Im}{\psi}$')
 
-        self.line_phase_z_eff, = ax.plot(settings.z, zeros_like(settings.z), linewidth=1, linestyle='-', color=colors.wet_asphalt, label='effective')
-        self.line_phase_z, = ax.plot(settings.z, zeros_like(settings.z), linewidth=1, linestyle='--', color=colors.peter_river, label='$x=y=0$')
+        ax.set_xlim(settings.x_min, settings.x_max)
 
-        ax.set_xlim(settings.z_min, settings.z_max)
-        ax.set_ylim(-1.2, 1.2)
+        ax.set_ylim(settings.real_part_min, settings.real_part_max)
 
-        ax.set_xlabel(settings.label_z)
+        ax.set_xlabel(settings.label_x)
         
-        ax.set_xticks(settings.z_ticks)
+        ax.set_xticks(settings.x_ticks)
         
         ax.grid(visible=True, which='major', color=settings.color_gridlines_major, linestyle='-', linewidth=0.5)
 
-        ax.set_ylabel(r'$\cos(\varphi)$')
-
-        ax.legend(loc='lower right', bbox_to_anchor=(1.0, 0.0),
-                  fancybox=settings.fancybox, framealpha=settings.framealpha, ncol=1)
+        ax.set_ylabel(r'$\mu \mathrm{m}^{-1 \, / \, 2}$', labelpad=0)
+        # -----------------------------------------------------------------------------------------
 
         # -----------------------------------------------------------------------------------------
-        ax_V_z = ax.twinx()
-    
-        self.line_V_z, = ax_V_z.plot(settings.z, zeros_like(settings.z),
-                                     linewidth=1, linestyle='-', color=colors.sun_flower)
+        ax2 = ax.twinx()
+
+        self.line_V, = ax2.plot(
+            settings.x, zeros_like(settings.x),
+            linewidth=settings.linewidth_V, linestyle='-', color=settings.linecolor_V, label=r'$V$')
 
-        ax_V_z.set_xlim(settings.z_min, settings.z_max)
-        ax_V_z.set_ylim(settings.V_min, settings.V_max)
+        ax2.set_xlim(settings.x_min, settings.x_max)
+        ax2.set_ylim(settings.V_min, settings.V_max)
         
-        ax_V_z.set_ylabel(settings.label_V)
+        ax2.set_ylabel(r'$h \times \mathrm{kHz}$', labelpad=10)
         # -----------------------------------------------------------------------------------------
 
-    def update(self, phase_z_eff, phase_z, V_z):
+        # -----------------------------------------------------------------------------------------
+        lines, labels = ax.get_legend_handles_labels()
+        lines2, labels2 = ax2.get_legend_handles_labels()
+        ax2.legend(lines + lines2, labels + labels2,
+                   loc='upper right', bbox_to_anchor=(1.0, 1.25), fancybox=True, framealpha=1, ncol=1)
+        # -----------------------------------------------------------------------------------------
+
+    def update(self, psi, V):
 
+        psi_re = np.real(psi)
+        psi_im = np.imag(psi)
+        
         scaling_V = self.hbar * 2 * pi * 1000
         
-        V_z = V_z / scaling_V
-
-        self.line_phase_z_eff.set_ydata(np.cos(phase_z_eff))
-        self.line_phase_z.set_ydata(np.cos(phase_z))
+        V = V / scaling_V
+        
+        self.line_psi_re.set_ydata(psi_re / math.sqrt(1e6))
+        self.line_psi_im.set_ydata(psi_im / math.sqrt(1e6))
 
-        self.line_V_z.set_ydata(V_z)
+        self.line_V.set_ydata(V)
```

### Comparing `qsolve-0.2.6/src/qsolve/potentials/components_3d/lesanovsky_3d.py` & `qsolve-0.2.7/src/qsolve/potentials/components_1d/lesanovsky_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/potentials/components_3d/lesanovsky_xy_3d.py` & `qsolve-0.2.7/src/qsolve/potentials/components_1d/lesanovsky_xy_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/chemical_potential.py` & `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/chemical_potential.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/compute_ground_state_solution.py` & `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/compute_ground_state_solution.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/densities.py` & `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/densities.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/energies.py` & `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/energies.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/getter_functions.py` & `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/getter_functions.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_device.py` & `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/init_device.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_grid_3d.py` & `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_grid_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 
 import numpy as np
 
-from qsolve.utils.primes import get_prime_factors
+from qsolve.primes import get_prime_factors
 
 
 def init_grid(self, kwargs):
 
     self.x_min = kwargs['x_min'] / self.units.unit_length
     self.x_max = kwargs['x_max'] / self.units.unit_length
```

### Comparing `qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_potential.py` & `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_potential.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_units.py` & `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_units.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/solver_gpe_3d.py` & `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/solver_gpe_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/spectrum.py` & `qsolve-0.2.7/src/qsolve/solvers/solvers_2d/solver_gpe_2d/spectrum.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/solvers/solvers_3d/solver_gpe_3d/units.py` & `qsolve-0.2.7/src/qsolve/solvers/solvers_3d/solver_gpe_3d/units.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve/utils/primes.py` & `qsolve-0.2.7/src/qsolve/primes.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.6/src/qsolve.egg-info/PKG-INFO` & `qsolve-0.2.7/src/qsolve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsolve
-Version: 0.2.6
+Version: 0.2.7
 Summary: Numerical methods for the simulation of ultracold atom experiments
 Home-page: https://github.com/jfmennemann/qsolve
 Author: Jan-Frederik Mennemann
 Author-email: jfmennemann@gmx.de
 Keywords: ultracold atoms,simulations,Gross-Pitaevskii equation,thermal state sampling,time of flight
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

