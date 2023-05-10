# Comparing `tmp/geowatch-0.6.3.tar.gz` & `tmp/geowatch-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geowatch-0.6.3.tar", last modified: Wed May  3 04:02:52 2023, max compression
+gzip compressed data, was "geowatch-0.6.6.tar", last modified: Wed May 10 18:09:56 2023, max compression
```

## Comparing `geowatch-0.6.3.tar` & `geowatch-0.6.6.tar`

### file list

```diff
@@ -1,1042 +1,1048 @@
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.957887 geowatch-0.6.3/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19164 2023-05-03 00:21:52.000000 geowatch-0.6.3/CHANGELOG.md
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7765 2023-04-29 23:47:47.000000 geowatch-0.6.3/Dockerfile
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11343 2022-12-02 18:15:30.000000 geowatch-0.6.3/LICENSE
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      313 2022-06-07 15:49:12.000000 geowatch-0.6.3/MANIFEST.in
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7494 2023-05-03 04:02:52.957887 geowatch-0.6.3/PKG-INFO
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6414 2023-05-03 00:21:52.000000 geowatch-0.6.3/README.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1646 2023-05-02 02:20:39.000000 geowatch-0.6.3/conda_env.yml
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      406 2022-06-07 15:49:12.000000 geowatch-0.6.3/conftest.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      642 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/README.rst
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/algorithms/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1556 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/algorithms/fusion_overview.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2557 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/algorithms/sensorchan_specs.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      533 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/algorithms/ta2_deep_dive_info.md
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/data/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6892 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/data/access_dvc_repos.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1625 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/data/internal_resources.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1269 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/data/using_smartwatch_dvc.rst
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/debugging/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1598 2023-04-03 19:39:09.000000 geowatch-0.6.3/docs/debugging/debugging_cmdqueue.rst
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/development/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6332 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/development/coding_conventions.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3525 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/development/coding_tips.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1903 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/development/contribution_instructions.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3258 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/development/rebasing_procedure.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11705 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/development/ta2_feature_integration.md
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/environment/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10365 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/environment/getting_started_aws.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6890 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/environment/getting_started_dvc.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1172 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/environment/getting_started_kubectl.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6599 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/environment/getting_started_ssh_keys.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      544 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/environment/install_python.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2234 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/environment/install_python_conda.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6368 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/environment/install_python_pyenv.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3099 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/environment/installing_geowatch.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6791 2023-05-03 04:02:03.000000 geowatch-0.6.3/docs/environment/windows.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       24 2023-03-21 17:57:36.000000 geowatch-0.6.3/docs/index.rst
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/misc/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6162 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/misc/structure_proposal.md
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1986 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/misc/supporting_projects.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11380 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/mlops.md
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5235 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/onboarding.rst
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/smartflow/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2767 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/smartflow/getting_started_smartflow.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3465 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/smartflow/smartflow_copying_large_files_to_efs.md
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20420 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/smartflow/smartflow_running_the_system.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3164 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/smartflow/smartflow_training_fusion_models.md
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/testing/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2015 2023-04-29 23:47:47.000000 geowatch-0.6.3/docs/testing/running_ci_locally.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2139 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/testing/testing_practices.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14398 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/watch_cli.rst
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/geowatch/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      163 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       69 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/__main__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/cli/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      167 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       73 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/__main__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/animate_visualizations.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/baseline_framework_egress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/baseline_framework_ingress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/baseline_framework_kwcoco_egress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/baseline_framework_kwcoco_ingress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/cluster_sites.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_add_watch_fields.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_align.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_align_geotiffs.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_average_features.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_clean_geotiffs.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_combine_features.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_crop_tracks.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_intensity_histograms.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_reformat_channels.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_remove_bad_images.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_remove_empty_images.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_shard.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_spectra.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_time_combine.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_update_geotiff_metadata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_visualize_videos.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/concat_kwcoco_videos.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/crop_sites_to_regions.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/cli/dag_cli/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_bas_datagen.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_bas_fusion.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_pseudolive_consolidate.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_psuedolive_copy_previous.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_sc_datagen.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_sc_fusion.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_teamfeat_invariants.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/extend_sc_sites.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      176 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/find_dvc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/geojson_site_stats.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/geotiffs_to_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/gifify.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/kwcoco_to_geojson.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/merge_region_models.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/mlops_cli.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/prepare_splits.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/prepare_ta2_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/prepare_teamfeats.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/pseudolive_consolidate.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/reproject_annotations.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/run_fusion_predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/run_metrics_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/run_tracker.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/split_videos.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/stac_search.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/ta1_stac_to_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/torch_model_stats.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/validate_annotation_schemas.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/watch_coco_stats.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/demo/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      168 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/demo_region.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/dummy_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/landsat_demodata.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/demo/metrics_demo/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/metrics_demo/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/metrics_demo/demo_rendering.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/metrics_demo/demo_truth.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/metrics_demo/demo_utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/metrics_demo/generate_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/metrics_demo/site_perterbing.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/nitf_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/sentinel2_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/smart_kwcoco_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/stac_demo.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/exceptions.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/geoannots/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      173 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/geoannots/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/geoannots/geomodels.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/geoannots/make_region_from_sites.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/gis/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      167 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/digital_globe.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/elevation.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/geotiff.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/gis/sensors/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/sensors/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/sensors/sentinel2.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/spatial_reference.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/heuristics.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/mlops/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      169 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       75 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/__main__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/aggregate.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/aggregate_loader.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/confusion_visualization.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/confusor_analysis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/manager.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/mlops/old/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      173 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/expt_manager.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/expt_report.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/expt_state.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/old_pipeline_nodes.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/old_plots.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/pipeline_v1.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/plots.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/pipeline_nodes.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/repackager.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/schedule_evaluation.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/smart_global_helper.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/smart_pipeline.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/smart_result_parser.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/monkey/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      170 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/_monkey_fbeta.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_albumentations.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_lightning.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_numpy.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_pil.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_tensorflow.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_torch.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_torchmetrics.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/rc/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      166 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/rc/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/rc/registry.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/stac/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      168 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/stac/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/stac/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/stac/stac_search_builder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/stac/util_stac.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/tasks/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      169 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/tasks/cold/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/assemble_cold_result_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/export_change_map.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/export_cold_result_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/prepare_ard.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/prepare_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/tile_processing.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/tile_processing_kwcoco.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/tasks/depth/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/backbone.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/demo_transform.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/dzyne_img_util.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/modules_monkeypatch.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/pl_highres_verify.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/dino_detector/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/dino_detector/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/dino_detector/package_building_detector.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/dino_detector/predict.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/fusion/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      176 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       82 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/__main__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/aggregate_results.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/fusion/architectures/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/architectures/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/architectures/segmenter_decoder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/architectures/sits.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/architectures/transformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/architectures/unet_blur.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/architectures/wu_mae.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/coco_stitcher.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/batch_visualization.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/data_augment.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/data_utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/demos_for_slides.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/kwcoco_datamodule.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      203 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/kwcoco_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/kwcoco_video_data.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/qa_bands.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/smart_mixins.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/spacetime_grid_builder.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      216 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/affinity.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/exceptions.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/plots.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/sampler.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      226 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/time_kernel_grammar.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/evaluate.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/fit_lightning.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/fusion/methods/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/channelwise_transformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/heterogeneous.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/network_modules.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/noop_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/unet_baseline.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/watch_module_mixins.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/organize.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      367 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/production.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/invariants/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/change.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/invariants/data/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/data/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/data/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/data/multi_image_datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/data/other_datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/fit_segment.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/iarpa_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/pretext_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/segmentation_model.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/landcover/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/detector.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/model_info.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/nets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/metrics/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/metrics/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/metrics/merge_iarpa_metrics.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/metrics/viz_sc_results.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      203 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/datasets/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/datasets/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/datasets/base_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      228 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/datasets/iarpa_kwdataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      231 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/datasets/iarpa_sc_kwdataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/datasets/peo_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/fit.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/apnb.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/base_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/discritizers.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/dynamic_unet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      233 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/early_fusion_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      237 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/early_fusion_mat_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      232 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/late_fusion_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      227 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/mat_ed_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      228 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/patch_transformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      238 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/patch_transformer_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      222 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/peri_resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/pos_embedding.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/self_attention.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      237 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/siamese_feature_diff_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      231 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/siamese_fusion_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      229 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/simple_cnn_encoder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/simple_decoder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      222 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/timesformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/unet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/unet_lstm.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/vit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/predict_sc.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/util_config.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      219 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/util_misc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/util_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/util_paths.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/util_visualize.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.905887 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.905887 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/bigearthnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/deepglobe.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/dynamicearthnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/hrscd.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/iarpa_contrastive_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/iarpa_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/inria.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/s2_self.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/s2mcp.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/spacenet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/spacenet2.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/sysucd.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.905887 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/bigearthnet_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/change_vector_analysis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      219 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/cluster_labeling.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      218 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/compare_vw_maps.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/deepglobe_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      222 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/deepglobe_train_val.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      227 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/dynamicearthnet_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      231 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/evaluation_method_comparison.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/hrscd_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/iarpa_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/iarpa_patch_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/inria_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/moco_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      229 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/moco_unsupervised_material.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      239 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/mt_material_clustering_tranfer_learn.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      237 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/multi_temporal_material_clustering.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      218 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/onera_fine_tune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/onera_patch_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/onera_patch_finetune2.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/onera_patch_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/onera_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      227 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_net.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      230 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      234 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet_enc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/setr_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/shallow_seg_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/sim_contrastive_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/spacenet2_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/supervised_clustering.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      219 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/sysu_patch_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/fit.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/canny_edge.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/deeplab.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/deeplabWS.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/deeplab_diff.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/encoding.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/gci.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/linear_classifier.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/losses.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/moco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/quantizer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/resnetGNWS.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      228 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/resnet_classification_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/resnet_enc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/sg.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/shallow_seg.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/supcon.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/tex_refine.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/transformer_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/transformer_seg.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/predict_patchwise.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      203 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/predict_test.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/scripts/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/scripts/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/scripts/filter_by_sensor.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/scripts/labelbox2coco.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/convert_sysucd_to_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/cva.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/eval_utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/visualization.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/tracking/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/from_heatmap.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/from_polygon.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/normalize.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/phase.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/visualize.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/drop0_datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/fit.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/models/resnets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/models/unet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/models/unet_blur.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/predict.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/data/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/data/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/data/create_splits.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      246 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/create_splits_unmasked.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/time_sort_S7.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/time_sort_module.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.913887 geowatch-0.6.3/geowatch/utils/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      169 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/configargparse_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/ext_monai.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/ijson_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/kwcoco_extensions.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.913887 geowatch-0.6.3/geowatch/utils/lightning_ext/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/argparse_ext.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.917887 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/auto_resumer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/batch_plotter.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/packager.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/state_logger.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/tensorboard_plotter.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/text_logger.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/demo.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/lightning_cli_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/monkeypatches.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/old_parser_devices.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/util_device.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/util_globals.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/util_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/partial_format.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/process_context.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/result_analysis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/reverse_hashid.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/simple_dvc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/slugify_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_bands.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_codes.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_data.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_dotdict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_environ.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_eval.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_gdal.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_girder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_gis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_globals.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_hardware.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_iter.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_json.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_kwarray.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_kwimage.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_kwplot.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_locks.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_logging.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_nesting.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_netharn.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_pandas.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_parallel.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_param_grid.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_path.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_pattern.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_progress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_raster.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_regex.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_resolution.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_resources.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_rgdc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_s3.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_stringalgo.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_time.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_torchmetrics.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_yaml.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.885887 geowatch-0.6.3/geowatch.egg-info/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7494 2023-05-03 04:02:52.000000 geowatch-0.6.3/geowatch.egg-info/PKG-INFO
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    40654 2023-05-03 04:02:52.000000 geowatch-0.6.3/geowatch.egg-info/SOURCES.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        1 2023-05-03 04:02:52.000000 geowatch-0.6.3/geowatch.egg-info/dependency_links.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-05-03 04:02:52.000000 geowatch-0.6.3/geowatch.egg-info/entry_points.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        1 2023-04-27 14:57:33.000000 geowatch-0.6.3/geowatch.egg-info/not-zip-safe
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18527 2023-05-03 04:02:52.000000 geowatch-0.6.3/geowatch.egg-info/requires.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       15 2023-05-03 04:02:52.000000 geowatch-0.6.3/geowatch.egg-info/top_level.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2429 2023-04-29 23:47:47.000000 geowatch-0.6.3/pyproject.toml
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.917887 geowatch-0.6.3/requirements/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       68 2023-05-02 02:20:39.000000 geowatch-0.6.3/requirements/cold.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      562 2023-05-03 00:21:52.000000 geowatch-0.6.3/requirements/development.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       19 2023-05-02 02:20:39.000000 geowatch-0.6.3/requirements/dvc.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      445 2023-04-29 21:01:30.000000 geowatch-0.6.3/requirements/gdal.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      889 2023-04-03 19:39:09.000000 geowatch-0.6.3/requirements/graphics.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      979 2023-04-03 19:39:09.000000 geowatch-0.6.3/requirements/headless.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      110 2023-05-02 02:20:39.000000 geowatch-0.6.3/requirements/linting.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/requirements/mmcv.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      318 2023-05-02 02:20:39.000000 geowatch-0.6.3/requirements/optional.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9002 2023-05-03 00:21:52.000000 geowatch-0.6.3/requirements/runtime.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       86 2023-05-02 02:20:39.000000 geowatch-0.6.3/requirements/tensorflow.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       88 2023-04-29 21:01:30.000000 geowatch-0.6.3/requirements/tests.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      115 2023-04-29 21:01:30.000000 geowatch-0.6.3/requirements.txt
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      823 2023-04-03 19:39:09.000000 geowatch-0.6.3/run_tests.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       38 2023-05-03 04:02:52.957887 geowatch-0.6.3/setup.cfg
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10526 2023-05-03 00:21:52.000000 geowatch-0.6.3/setup.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.917887 geowatch-0.6.3/tests/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1271 2023-04-29 23:47:47.000000 geowatch-0.6.3/tests/test_cli.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2530 2023-04-29 23:47:47.000000 geowatch-0.6.3/tests/test_heterogeneous_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4038 2022-12-02 18:15:30.000000 geowatch-0.6.3/tests/test_init_from_pretrained.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2277 2023-03-21 17:57:36.000000 geowatch-0.6.3/tests/test_kwcoco_dataloader.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8409 2023-05-03 00:21:52.000000 geowatch-0.6.3/tests/test_lightning_cli_fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4446 2023-04-29 21:01:30.000000 geowatch-0.6.3/tests/test_load_models.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4367 2023-04-29 23:47:47.000000 geowatch-0.6.3/tests/test_mlops_scheduler.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7349 2023-04-29 21:01:30.000000 geowatch-0.6.3/tests/test_predict_latest_models.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4669 2023-04-29 21:01:30.000000 geowatch-0.6.3/tests/test_predict_old_fusion_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3440 2023-04-29 23:47:47.000000 geowatch-0.6.3/tests/test_predict_small_region.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6717 2023-04-29 21:01:30.000000 geowatch-0.6.3/tests/test_save_packages.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2514 2022-12-20 16:17:52.000000 geowatch-0.6.3/tests/test_sensor_metadata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13860 2023-04-29 23:47:47.000000 geowatch-0.6.3/tests/test_tracker.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      134 2022-06-07 15:49:12.000000 geowatch-0.6.3/tests/test_version.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.917887 geowatch-0.6.3/watch/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6332 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      139 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/__main__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.921887 geowatch-0.6.3/watch/cli/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       98 2023-01-18 16:43:36.000000 geowatch-0.6.3/watch/cli/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5685 2023-05-03 00:37:18.000000 geowatch-0.6.3/watch/cli/__main__.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     7854 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/animate_visualizations.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6116 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/cli/baseline_framework_egress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16017 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/cli/baseline_framework_ingress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6070 2022-12-14 20:49:04.000000 geowatch-0.6.3/watch/cli/baseline_framework_kwcoco_egress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3673 2022-12-14 20:49:04.000000 geowatch-0.6.3/watch/cli/baseline_framework_kwcoco_ingress.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10809 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/cluster_sites.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     6201 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/cli/coco_add_watch_fields.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    95340 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/cli/coco_align.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      215 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/coco_align_geotiffs.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    32128 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/coco_average_features.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    34654 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/coco_clean_geotiffs.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     9577 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/coco_combine_features.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22525 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/coco_crop_tracks.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      224 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/coco_intensity_histograms.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10091 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/coco_reformat_channels.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    11078 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/coco_remove_bad_images.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2653 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/coco_shard.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    32293 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/coco_spectra.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    44062 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/cli/coco_time_combine.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4771 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/coco_update_geotiff_metadata.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    61339 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/cli/coco_visualize_videos.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1814 2022-12-14 20:49:04.000000 geowatch-0.6.3/watch/cli/concat_kwcoco_videos.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15924 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/crop_sites_to_regions.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.925887 geowatch-0.6.3/watch/cli/dag_cli/
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)       89 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/dag_cli/__init__.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    15320 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/dag_cli/run_bas_datagen.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    13342 2023-05-01 17:33:03.000000 geowatch-0.6.3/watch/cli/dag_cli/run_bas_fusion.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10286 2023-05-01 17:33:03.000000 geowatch-0.6.3/watch/cli/dag_cli/run_dino_sv.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6939 2023-05-01 19:59:37.000000 geowatch-0.6.3/watch/cli/dag_cli/run_dzyne_parallel_site_vali.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     3529 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/dag_cli/run_pseudolive_consolidate.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     3062 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/dag_cli/run_psuedolive_copy_previous.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     7796 2023-05-01 17:33:03.000000 geowatch-0.6.3/watch/cli/dag_cli/run_sc_datagen.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    12667 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/dag_cli/run_sc_fusion.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6224 2023-05-01 17:33:03.000000 geowatch-0.6.3/watch/cli/dag_cli/run_sv_datagen.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     5581 2023-04-03 20:48:44.000000 geowatch-0.6.3/watch/cli/dag_cli/run_teamfeat_invariants.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5448 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/dag_cli/run_teamfeat_landcover.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11711 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/cli/extend_sc_sites.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4586 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/find_dvc.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    12269 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/geojson_site_stats.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14799 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/geotiffs_to_kwcoco.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10815 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/cli/gifify.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    60306 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/kwcoco_to_geojson.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4375 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/cli/merge_region_models.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/mlops_cli.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10349 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/prepare_splits.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    38053 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/prepare_ta2_dataset.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    29934 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/prepare_teamfeats.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14855 2022-12-14 20:49:04.000000 geowatch-0.6.3/watch/cli/pseudolive_consolidate.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    69727 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/cli/reproject_annotations.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       84 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/cli/run_fusion_predict.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    20415 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/run_metrics_framework.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      271 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/cli/run_tracker.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4224 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/split_videos.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22737 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/stac_search.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    27798 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/ta1_stac_to_kwcoco.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     9391 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/torch_model_stats.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16252 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/validate_annotation_schemas.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    15553 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/cli/watch_coco_stats.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.925887 geowatch-0.6.3/watch/demo/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2624 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/demo/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20892 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/demo/demo_region.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      563 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/demo/dummy_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7543 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/demo/landsat_demodata.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.925887 geowatch-0.6.3/watch/demo/metrics_demo/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      138 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/demo/metrics_demo/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7448 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/demo/metrics_demo/demo_rendering.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24604 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/demo/metrics_demo/demo_truth.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13005 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/demo/metrics_demo/demo_utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6307 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/demo/metrics_demo/generate_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15545 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/demo/metrics_demo/site_perterbing.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    29938 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/demo/nitf_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3676 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/demo/sentinel2_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25225 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/demo/smart_kwcoco_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4089 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/demo/stac_demo.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/exceptions.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.925887 geowatch-0.6.3/watch/geoannots/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      989 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/geoannots/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2308 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/geoannots/geococo_objects.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16872 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/geoannots/geomodels.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.925887 geowatch-0.6.3/watch/gis/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1645 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/gis/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9291 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/gis/digital_globe.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10020 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/gis/elevation.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    51299 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/gis/geotiff.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.925887 geowatch-0.6.3/watch/gis/sensors/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      326 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/gis/sensors/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6516 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/gis/sensors/sentinel2.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13106 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/gis/spatial_reference.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    26467 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/heuristics.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/mlops/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/mlops/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      670 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/mlops/__main__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    70579 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/mlops/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    70055 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/mlops/aggregate.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17109 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/mlops/aggregate_loader.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23469 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/mlops/confusion_visualization.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25565 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/mlops/confusor_analysis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    40297 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/mlops/manager.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/mlops/old/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/mlops/old/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18067 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/mlops/old/expt_manager.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39383 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/mlops/old/expt_report.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    44820 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/mlops/old/expt_state.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39219 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/mlops/old/old_pipeline_nodes.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10290 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/mlops/old/old_plots.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8717 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/mlops/old/pipeline_v1.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39647 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/mlops/old/plots.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    55208 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/mlops/pipeline_nodes.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12686 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/mlops/repackager.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16868 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/mlops/schedule_evaluation.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22712 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/mlops/smart_global_helper.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    32124 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/mlops/smart_pipeline.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    33368 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/mlops/smart_result_parser.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/monkey/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       62 2022-12-14 20:49:53.000000 geowatch-0.6.3/watch/monkey/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4095 2022-12-14 20:49:53.000000 geowatch-0.6.3/watch/monkey/_monkey_fbeta.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4047 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/monkey/monkey_albumentations.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      280 2022-12-14 20:49:53.000000 geowatch-0.6.3/watch/monkey/monkey_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1187 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/monkey/monkey_lightning.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       68 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/monkey/monkey_numpy.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2022-12-14 20:49:53.000000 geowatch-0.6.3/watch/monkey/monkey_pil.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/monkey/monkey_tensorflow.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      658 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/monkey/monkey_torch.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      601 2022-12-14 20:49:53.000000 geowatch-0.6.3/watch/monkey/monkey_torchmetrics.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/rc/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1715 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/rc/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9626 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/rc/registry.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/stac/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       66 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/stac/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17312 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/stac/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14251 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/stac/stac_search_builder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9733 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/stac/util_stac.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/tasks/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1677 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/tasks/cold/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/tasks/cold/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17557 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/cold/assemble_cold_result_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21171 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/tasks/cold/export_change_map.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18314 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/cold/export_cold_result_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17004 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/tasks/cold/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    73485 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/cold/prepare_ard.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23475 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/cold/prepare_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30062 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/tasks/cold/tile_processing.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    28290 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/cold/tile_processing_kwcoco.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.933887 geowatch-0.6.3/watch/tasks/depth/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/depth/__init__.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4501 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/depth/backbone.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6559 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/depth/config.json
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6816 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/depth/datasets.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4372 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/depth/demo_transform.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     8379 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/depth/dzyne_img_util.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      295 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/depth/modules_monkeypatch.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     5239 2022-08-09 13:10:41.000000 geowatch-0.6.3/watch/tasks/depth/pl_highres_verify.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24371 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/depth/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5689 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/depth/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.933887 geowatch-0.6.3/watch/tasks/depthPCD/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-01 19:59:37.000000 geowatch-0.6.3/watch/tasks/depthPCD/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6700 2023-05-01 19:59:37.000000 geowatch-0.6.3/watch/tasks/depthPCD/model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      407 2023-05-01 19:59:37.000000 geowatch-0.6.3/watch/tasks/depthPCD/model_test.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20132 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/depthPCD/score_tracks.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.933887 geowatch-0.6.3/watch/tasks/dino_detector/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/dino_detector/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24608 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/dino_detector/building_validator.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10562 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/dino_detector/predict.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.933887 geowatch-0.6.3/watch/tasks/fusion/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2501 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/fusion/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       72 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/fusion/__main__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    82304 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/fusion/aggregate_results.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.933887 geowatch-0.6.3/watch/tasks/fusion/architectures/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      233 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/fusion/architectures/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11883 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/architectures/segmenter_decoder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5979 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/tasks/fusion/architectures/sits.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    51015 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/architectures/transformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4989 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/fusion/architectures/unet_blur.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6302 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/architectures/wu_mae.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    36730 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/fusion/coco_stitcher.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/fusion/datamodules/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      336 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9680 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    48055 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/batch_visualization.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8458 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/data_augment.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18677 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/data_utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9780 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/demos_for_slides.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    29470 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/kwcoco_datamodule.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)   149541 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/kwcoco_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      373 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/kwcoco_video_data.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23364 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/qa_bands.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14225 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/smart_mixins.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    53890 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/spacetime_grid_builder.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1527 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10375 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    44675 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/affinity.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       44 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/exceptions.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9422 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/plots.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39631 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/sampler.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3384 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/time_kernel_grammar.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7352 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    55018 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/evaluate.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    28542 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19157 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/fusion/fit_lightning.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/fusion/methods/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      741 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/tasks/fusion/methods/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    81666 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/methods/channelwise_transformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    79880 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/methods/heterogeneous.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25464 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/methods/network_modules.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8960 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/methods/noop_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    28643 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/methods/unet_baseline.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    32192 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/methods/watch_module_mixins.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4468 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/organize.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    61763 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/tasks/fusion/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14896 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/fusion/production.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16789 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/invariants/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/invariants/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13603 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/invariants/change.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/invariants/data/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/invariants/data/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    35389 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/invariants/data/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20577 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/invariants/data/multi_image_datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25778 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/invariants/data/other_datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5589 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/invariants/fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4483 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/invariants/fit_segment.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6709 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/invariants/iarpa_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24584 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/invariants/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15963 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/invariants/pretext_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12941 2022-08-09 13:10:41.000000 geowatch-0.6.3/watch/tasks/invariants/segmentation_model.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/landcover/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/landcover/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6028 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/landcover/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5623 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/landcover/detector.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      103 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/landcover/fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2377 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/landcover/model_info.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2360 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/tasks/landcover/nets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12281 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/landcover/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      349 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/landcover/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/metrics/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/tasks/metrics/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    26517 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/tasks/metrics/merge_iarpa_metrics.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11867 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/metrics/viz_sc_results.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8025 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    33579 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/base_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    31719 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/iarpa_kwdataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19805 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/iarpa_sc_kwdataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    34195 2022-08-09 13:10:41.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/peo_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/fit.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.941887 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22473 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9162 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/apnb.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5007 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/base_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8375 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/discritizers.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4272 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/dynamic_unet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1276 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/early_fusion_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3510 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/early_fusion_mat_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7979 2022-08-09 13:10:41.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/late_fusion_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5652 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/mat_ed_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16573 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/patch_transformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2864 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/patch_transformer_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11476 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/peri_resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6888 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/pos_embedding.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15931 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3732 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/self_attention.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6771 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/siamese_feature_diff_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3779 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/siamese_fusion_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1833 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/simple_cnn_encoder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9772 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/simple_decoder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24297 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/timesformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6020 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/unet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8684 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/unet_lstm.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4982 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/vit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10698 2022-08-09 13:10:41.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9087 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/predict_sc.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.941887 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      115 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_config.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10512 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_misc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2112 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1508 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_paths.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9883 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_visualize.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.941887 geowatch-0.6.3/watch/tasks/rutgers_material_seg/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.941887 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3274 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11109 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/bigearthnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4313 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/deepglobe.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5959 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/dynamicearthnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4659 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/hrscd.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13129 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/iarpa_contrastive_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8257 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/iarpa_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6702 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/inria.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3910 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/s2_self.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3309 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/s2mcp.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4659 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/spacenet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6266 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/spacenet2.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3830 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/sysucd.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.945887 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    42088 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/bigearthnet_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19562 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/change_vector_analysis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    26483 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/cluster_labeling.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    52228 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/compare_vw_maps.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    40645 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/deepglobe_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17085 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/deepglobe_train_val.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    46366 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/dynamicearthnet_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    42111 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/evaluation_method_comparison.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    45044 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/hrscd_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    45628 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/iarpa_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/iarpa_patch_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    45044 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/inria_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16504 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/moco_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21771 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/moco_unsupervised_material.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10831 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/mt_material_clustering_tranfer_learn.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4437 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/multi_temporal_material_clustering.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    61390 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_fine_tune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    49788 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    65883 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune2.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    78136 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_patch_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    56648 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    70057 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_net.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    67609 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    66954 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet_enc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30059 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/setr_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    32133 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/shallow_seg_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    35336 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/sim_contrastive_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    48335 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/spacenet2_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7030 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/supervised_clustering.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    60321 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/sysu_patch_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       70 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/fit.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1466 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7650 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/canny_edge.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13281 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/deeplab.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17807 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/deeplabWS.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13507 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/deeplab_diff.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2845 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/encoding.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3794 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/gci.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      658 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/linear_classifier.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11714 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/losses.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5727 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/moco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9085 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/quantizer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11438 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7592 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnetGNWS.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12182 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnet_classification_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19182 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnet_enc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1414 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/sg.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4967 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/shallow_seg.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7222 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/supcon.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4278 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/tex_refine.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12022 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/transformer_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6462 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/transformer_seg.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    33755 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14703 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/predict_patchwise.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14964 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/predict_test.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/rutgers_material_seg/scripts/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/scripts/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1884 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/scripts/filter_by_sensor.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3932 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/scripts/labelbox2coco.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5761 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/convert_sysucd_to_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3861 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/cva.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12756 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/eval_utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13993 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9925 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/visualization.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1728 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7209 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/base_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11244 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/image_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11762 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/material_pixel_dataset.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      446 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5883 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/models/material_mlp.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6146 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/predict.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/sam/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/sam/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17730 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/sam/predict.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/tracking/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1582 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/tracking/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    58501 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/tracking/from_heatmap.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2904 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/tracking/from_polygon.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30472 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/tracking/normalize.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21464 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/tracking/phase.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23668 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/tracking/utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7531 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/tracking/visualize.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15495 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/drop0_datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3118 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/fit.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5614 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/resnets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5466 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/unet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10027 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/unet_blur.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8395 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/predict.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2057 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/create_splits.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2093 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/create_splits_unmasked.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16199 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5987 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/time_sort_S7.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4070 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/time_sort_module.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      594 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.953887 geowatch-0.6.3/watch/utils/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2803 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12992 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/configargparse_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    48556 2023-02-02 14:12:29.000000 geowatch-0.6.3/watch/utils/ext_monai.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11626 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/utils/ijson_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)   116465 2023-05-02 20:05:02.000000 geowatch-0.6.3/watch/utils/kwcoco_extensions.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.957887 geowatch-0.6.3/watch/utils/lightning_ext/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      376 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/utils/lightning_ext/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21356 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/lightning_ext/_jsonargparse_ext_ge_4_21.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20330 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/lightning_ext/_jsonargparse_ext_lt_4_21.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7034 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/argparse_ext.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.957887 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1244 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5735 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/auto_resumer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8793 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/batch_plotter.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10112 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/packager.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2693 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/state_logger.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16120 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/tensorboard_plotter.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13026 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/text_logger.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4371 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/demo.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3211 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/lightning_ext/lightning_cli_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2022-12-14 20:49:53.000000 geowatch-0.6.3/watch/utils/lightning_ext/monkeypatches.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7558 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/utils/lightning_ext/old_parser_devices.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5712 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/utils/lightning_ext/util_device.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      303 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/utils/lightning_ext/util_globals.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      434 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/utils/lightning_ext/util_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10606 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/partial_format.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11208 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/process_context.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    56465 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/result_analysis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5456 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/reverse_hashid.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13733 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/simple_dvc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8514 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/utils/slugify_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    41201 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/util_bands.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1059 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/utils/util_codes.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12129 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/utils/util_data.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7144 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_dotdict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1813 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/utils/util_environ.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2733 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_eval.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7920 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/utils/util_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    47570 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_gdal.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6368 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/utils/util_girder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    43860 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/util_gis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2747 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/utils/util_globals.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2039 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/utils/util_hardware.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2589 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/utils/util_iter.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3455 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_json.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    41820 2023-05-01 17:33:03.000000 geowatch-0.6.3/watch/utils/util_kwarray.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    67297 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/util_kwimage.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14504 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/util_kwplot.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3771 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/utils/util_locks.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8978 2022-12-14 20:49:04.000000 geowatch-0.6.3/watch/utils/util_logging.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1035 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_nesting.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12514 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_netharn.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10172 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/util_nvidia.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10275 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_pandas.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5746 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_parallel.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25992 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/utils/util_param_grid.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18404 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_path.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13282 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_pattern.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23235 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_progress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15872 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/utils/util_raster.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3028 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/utils/util_regex.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7614 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/utils/util_resolution.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3542 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/utils/util_resources.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3083 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/utils/util_rgdc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      570 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/utils/util_s3.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7307 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/utils/util_stringalgo.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13699 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/utils/util_time.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1786 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/utils/util_torchmetrics.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2133 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/utils/util_windows.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9413 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/util_yaml.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.167926 geowatch-0.6.6/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20124 2023-05-10 15:57:19.000000 geowatch-0.6.6/CHANGELOG.md
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7765 2023-04-29 23:47:47.000000 geowatch-0.6.6/Dockerfile
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11343 2022-12-02 18:15:30.000000 geowatch-0.6.6/LICENSE
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      313 2022-06-07 15:49:12.000000 geowatch-0.6.6/MANIFEST.in
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7494 2023-05-10 18:09:56.167926 geowatch-0.6.6/PKG-INFO
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6414 2023-05-03 00:21:52.000000 geowatch-0.6.6/README.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1646 2023-05-02 02:20:39.000000 geowatch-0.6.6/conda_env.yml
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      406 2022-06-07 15:49:12.000000 geowatch-0.6.6/conftest.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.515930 geowatch-0.6.6/docs/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      642 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/README.rst
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.515930 geowatch-0.6.6/docs/algorithms/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1556 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/algorithms/fusion_overview.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2557 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/algorithms/sensorchan_specs.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      533 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/algorithms/ta2_deep_dive_info.md
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.515930 geowatch-0.6.6/docs/data/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6892 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/data/access_dvc_repos.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1625 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/data/internal_resources.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1269 2023-05-03 00:21:52.000000 geowatch-0.6.6/docs/data/using_smartwatch_dvc.rst
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.515930 geowatch-0.6.6/docs/debugging/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1598 2023-04-03 19:39:09.000000 geowatch-0.6.6/docs/debugging/debugging_cmdqueue.rst
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.519930 geowatch-0.6.6/docs/development/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6332 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/development/coding_conventions.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3525 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/development/coding_tips.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1903 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/development/contribution_instructions.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3258 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/development/rebasing_procedure.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11705 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/development/ta2_feature_integration.md
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.523930 geowatch-0.6.6/docs/environment/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10365 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/environment/getting_started_aws.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6890 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/environment/getting_started_dvc.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1172 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/environment/getting_started_kubectl.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6599 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/environment/getting_started_ssh_keys.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      544 2023-05-03 00:21:52.000000 geowatch-0.6.6/docs/environment/install_python.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2234 2023-05-03 00:21:52.000000 geowatch-0.6.6/docs/environment/install_python_conda.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6368 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/environment/install_python_pyenv.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3099 2023-05-03 00:21:52.000000 geowatch-0.6.6/docs/environment/installing_geowatch.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6791 2023-05-10 18:09:10.000000 geowatch-0.6.6/docs/environment/windows.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       24 2023-03-21 17:57:36.000000 geowatch-0.6.6/docs/index.rst
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.523930 geowatch-0.6.6/docs/misc/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6162 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/misc/structure_proposal.md
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1986 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/misc/supporting_projects.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11380 2023-05-03 00:21:52.000000 geowatch-0.6.6/docs/mlops.md
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5235 2023-05-03 00:21:52.000000 geowatch-0.6.6/docs/onboarding.rst
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.527930 geowatch-0.6.6/docs/smartflow/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2767 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/smartflow/getting_started_smartflow.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3465 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/smartflow/smartflow_copying_large_files_to_efs.md
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23221 2023-05-09 01:10:52.000000 geowatch-0.6.6/docs/smartflow/smartflow_running_the_system.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3164 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/smartflow/smartflow_training_fusion_models.md
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.531930 geowatch-0.6.6/docs/testing/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2015 2023-04-29 23:47:47.000000 geowatch-0.6.6/docs/testing/running_ci_locally.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2139 2023-05-02 02:20:39.000000 geowatch-0.6.6/docs/testing/testing_practices.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14398 2023-05-03 00:21:52.000000 geowatch-0.6.6/docs/watch_cli.rst
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.535930 geowatch-0.6.6/geowatch/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      163 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       69 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/__main__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.543930 geowatch-0.6.6/geowatch/cli/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      167 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       73 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/__main__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/animate_visualizations.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/baseline_framework_egress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/baseline_framework_ingress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/baseline_framework_kwcoco_egress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/baseline_framework_kwcoco_ingress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/cluster_sites.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_add_watch_fields.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_align.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_align_geotiffs.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_average_features.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_clean_geotiffs.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_combine_features.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_crop_tracks.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_intensity_histograms.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_reformat_channels.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_remove_bad_images.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_remove_empty_images.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_shard.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_spectra.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_time_combine.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_update_geotiff_metadata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/coco_visualize_videos.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/concat_kwcoco_videos.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/crop_sites_to_regions.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.551930 geowatch-0.6.6/geowatch/cli/dag_cli/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/dag_cli/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/dag_cli/run_bas_datagen.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/dag_cli/run_bas_fusion.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/dag_cli/run_pseudolive_consolidate.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/dag_cli/run_psuedolive_copy_previous.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/dag_cli/run_sc_datagen.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/dag_cli/run_sc_fusion.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/dag_cli/run_teamfeat_invariants.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/extend_sc_sites.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      176 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/find_dvc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/geojson_site_stats.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/geotiffs_to_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/gifify.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/kwcoco_to_geojson.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/merge_region_models.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/mlops_cli.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/prepare_splits.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/prepare_ta2_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/prepare_teamfeats.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/pseudolive_consolidate.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/reproject_annotations.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/run_fusion_predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/run_metrics_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/run_tracker.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.551930 geowatch-0.6.6/geowatch/cli/special/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 16:57:53.000000 geowatch-0.6.6/geowatch/cli/special/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/split_videos.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/stac_search.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/ta1_stac_to_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/torch_model_stats.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/validate_annotation_schemas.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/cli/watch_coco_stats.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.555930 geowatch-0.6.6/geowatch/demo/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      168 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/demo_region.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/dummy_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/landsat_demodata.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.555930 geowatch-0.6.6/geowatch/demo/metrics_demo/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/metrics_demo/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/metrics_demo/demo_rendering.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/metrics_demo/demo_truth.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/metrics_demo/demo_utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/metrics_demo/generate_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/metrics_demo/site_perterbing.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/nitf_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/sentinel2_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/smart_kwcoco_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/demo/stac_demo.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/exceptions.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.559930 geowatch-0.6.6/geowatch/geoannots/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      173 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/geoannots/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/geoannots/geomodels.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/geoannots/make_region_from_sites.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.559930 geowatch-0.6.6/geowatch/gis/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      167 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/gis/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/gis/digital_globe.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/gis/elevation.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/gis/geotiff.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.559930 geowatch-0.6.6/geowatch/gis/sensors/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/gis/sensors/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/gis/sensors/sentinel2.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/gis/spatial_reference.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/heuristics.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.563930 geowatch-0.6.6/geowatch/mlops/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      169 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       75 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/__main__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/aggregate.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/aggregate_loader.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/confusion_visualization.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/confusor_analysis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/manager.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.567930 geowatch-0.6.6/geowatch/mlops/old/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      173 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/old/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/old/expt_manager.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/old/expt_report.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/old/expt_state.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/old/old_pipeline_nodes.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/old/old_plots.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/old/pipeline_v1.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/old/plots.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/pipeline_nodes.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/repackager.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/schedule_evaluation.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/smart_global_helper.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/smart_pipeline.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/mlops/smart_result_parser.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.567930 geowatch-0.6.6/geowatch/monkey/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      170 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/monkey/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/monkey/_monkey_fbeta.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/monkey/monkey_albumentations.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/monkey/monkey_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/monkey/monkey_lightning.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/monkey/monkey_numpy.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/monkey/monkey_pil.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/monkey/monkey_tensorflow.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/monkey/monkey_torch.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/monkey/monkey_torchmetrics.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.567930 geowatch-0.6.6/geowatch/rc/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      166 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/rc/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/rc/registry.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.567930 geowatch-0.6.6/geowatch/stac/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      168 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/stac/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/stac/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/stac/stac_search_builder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/stac/util_stac.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.567930 geowatch-0.6.6/geowatch/tasks/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      169 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.571930 geowatch-0.6.6/geowatch/tasks/cold/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/cold/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/cold/assemble_cold_result_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/cold/export_change_map.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/cold/export_cold_result_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/cold/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/cold/prepare_ard.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/cold/prepare_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/cold/tile_processing.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/cold/tile_processing_kwcoco.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.571930 geowatch-0.6.6/geowatch/tasks/depth/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/depth/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/depth/backbone.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/depth/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/depth/demo_transform.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/depth/dzyne_img_util.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/depth/modules_monkeypatch.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/depth/pl_highres_verify.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/depth/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/depth/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.571930 geowatch-0.6.6/geowatch/tasks/dino_detector/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/dino_detector/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/dino_detector/package_building_detector.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/dino_detector/predict.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.575930 geowatch-0.6.6/geowatch/tasks/fusion/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      176 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       82 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/__main__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/aggregate_results.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.575930 geowatch-0.6.6/geowatch/tasks/fusion/architectures/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/architectures/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/architectures/segmenter_decoder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/architectures/sits.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/architectures/transformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/architectures/unet_blur.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/architectures/wu_mae.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/coco_stitcher.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.583930 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/batch_visualization.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/data_augment.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/data_utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/demos_for_slides.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/kwcoco_datamodule.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      203 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/kwcoco_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/kwcoco_video_data.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/qa_bands.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/smart_mixins.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/spacetime_grid_builder.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.587930 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/temporal_sampling/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/temporal_sampling/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      216 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/temporal_sampling/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/temporal_sampling/affinity.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/temporal_sampling/exceptions.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/temporal_sampling/plots.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/temporal_sampling/sampler.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      226 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/temporal_sampling/time_kernel_grammar.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/datamodules/temporal_sampling/utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/evaluate.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/fit_lightning.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.591930 geowatch-0.6.6/geowatch/tasks/fusion/methods/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/methods/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/methods/channelwise_transformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/methods/heterogeneous.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/methods/network_modules.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/methods/noop_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/methods/unet_baseline.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/methods/watch_module_mixins.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/organize.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      367 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/production.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/fusion/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.591930 geowatch-0.6.6/geowatch/tasks/invariants/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/invariants/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/invariants/change.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.595930 geowatch-0.6.6/geowatch/tasks/invariants/data/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/invariants/data/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/invariants/data/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/invariants/data/multi_image_datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/invariants/data/other_datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/invariants/fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/invariants/fit_segment.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/invariants/iarpa_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/invariants/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/invariants/pretext_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/invariants/segmentation_model.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.607930 geowatch-0.6.6/geowatch/tasks/landcover/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/landcover/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/landcover/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/landcover/detector.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/landcover/fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/landcover/model_info.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/landcover/nets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/landcover/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/landcover/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.607930 geowatch-0.6.6/geowatch/tasks/metrics/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/metrics/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/metrics/merge_iarpa_metrics.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/metrics/viz_sc_results.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.607930 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      203 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.611930 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/datasets/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/datasets/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/datasets/base_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      228 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/datasets/iarpa_kwdataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      231 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/datasets/iarpa_sc_kwdataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/datasets/peo_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/fit.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.619929 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/apnb.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/base_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/discritizers.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/dynamic_unet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      233 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/early_fusion_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      237 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/early_fusion_mat_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      232 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/late_fusion_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      227 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/mat_ed_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      228 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/patch_transformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      238 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/patch_transformer_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      222 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/peri_resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/pos_embedding.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/self_attention.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      237 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/siamese_feature_diff_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      231 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/siamese_fusion_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      229 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/simple_cnn_encoder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/simple_decoder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      222 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/timesformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/unet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/unet_lstm.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/models/vit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/predict_sc.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.619929 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/utils/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/utils/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/utils/util_config.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      219 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/utils/util_misc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/utils/util_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/utils/util_paths.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_change_detection/utils/util_visualize.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.619929 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.627930 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/bigearthnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/deepglobe.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/dynamicearthnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/hrscd.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/iarpa_contrastive_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/iarpa_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/inria.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/s2_self.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/s2mcp.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/spacenet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/spacenet2.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/datasets/sysucd.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.631929 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/bigearthnet_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/change_vector_analysis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      219 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/cluster_labeling.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      218 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/compare_vw_maps.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/deepglobe_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      222 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/deepglobe_train_val.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      227 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/dynamicearthnet_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      231 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/evaluation_method_comparison.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/hrscd_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/iarpa_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/iarpa_patch_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/inria_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/moco_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      229 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/moco_unsupervised_material.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      239 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/mt_material_clustering_tranfer_learn.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      237 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/multi_temporal_material_clustering.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      218 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/onera_fine_tune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/onera_patch_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/onera_patch_finetune2.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/onera_patch_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/onera_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      227 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_net.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      230 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      234 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet_enc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/setr_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/shallow_seg_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/sim_contrastive_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/spacenet2_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/supervised_clustering.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      219 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/experiments/sysu_patch_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/fit.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.635929 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/canny_edge.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/deeplab.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/deeplabWS.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/deeplab_diff.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/encoding.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/gci.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/linear_classifier.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/losses.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/moco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/quantizer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/resnetGNWS.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      228 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/resnet_classification_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/resnet_enc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/sg.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/shallow_seg.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/supcon.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/tex_refine.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/transformer_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/models/transformer_seg.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/predict_patchwise.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      203 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/predict_test.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.635929 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/scripts/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/scripts/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/scripts/filter_by_sensor.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/scripts/labelbox2coco.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.635929 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/utils/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/utils/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/utils/convert_sysucd_to_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/utils/cva.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/utils/eval_utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/utils/utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/rutgers_material_seg/utils/visualization.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.707929 geowatch-0.6.6/geowatch/tasks/tracking/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/tracking/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/tracking/from_heatmap.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/tracking/from_polygon.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/tracking/normalize.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/tracking/phase.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/tracking/utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/tracking/visualize.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.711929 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/drop0_datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/fit.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.711929 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/models/resnets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/models/unet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/models/unet_blur.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/predict.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.711929 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/spacenet/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/spacenet/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.715929 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/spacenet/data/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/spacenet/data/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/spacenet/data/create_splits.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.715929 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      246 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/create_splits_unmasked.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/spacenet/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/time_sort_S7.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/time_sort_module.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/tasks/uky_temporal_prediction/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.747929 geowatch-0.6.6/geowatch/utils/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      169 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/configargparse_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/ext_monai.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/ijson_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/kwcoco_extensions.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.747929 geowatch-0.6.6/geowatch/utils/lightning_ext/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/argparse_ext.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.751929 geowatch-0.6.6/geowatch/utils/lightning_ext/callbacks/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/callbacks/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/callbacks/auto_resumer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/callbacks/batch_plotter.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/callbacks/packager.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/callbacks/state_logger.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/callbacks/tensorboard_plotter.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/callbacks/text_logger.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/demo.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/lightning_cli_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/monkeypatches.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/old_parser_devices.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/util_device.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/util_globals.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/lightning_ext/util_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/partial_format.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/process_context.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/result_analysis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/reverse_hashid.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/simple_dvc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/slugify_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_bands.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_codes.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_data.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_dotdict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_environ.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_eval.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_gdal.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_girder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_gis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_globals.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_hardware.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_iter.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_json.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_kwarray.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_kwimage.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_kwplot.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_locks.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_logging.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_nesting.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_netharn.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_pandas.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_parallel.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_param_grid.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_path.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_pattern.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_progress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_raster.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_regex.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_resolution.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_resources.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_rgdc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_s3.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_stringalgo.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_time.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_torchmetrics.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.6/geowatch/utils/util_yaml.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.535930 geowatch-0.6.6/geowatch.egg-info/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7494 2023-05-10 18:09:55.000000 geowatch-0.6.6/geowatch.egg-info/PKG-INFO
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    40794 2023-05-10 18:09:55.000000 geowatch-0.6.6/geowatch.egg-info/SOURCES.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        1 2023-05-10 18:09:55.000000 geowatch-0.6.6/geowatch.egg-info/dependency_links.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-05-10 18:09:55.000000 geowatch-0.6.6/geowatch.egg-info/entry_points.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        1 2023-04-27 14:57:33.000000 geowatch-0.6.6/geowatch.egg-info/not-zip-safe
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18527 2023-05-10 18:09:55.000000 geowatch-0.6.6/geowatch.egg-info/requires.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       15 2023-05-10 18:09:55.000000 geowatch-0.6.6/geowatch.egg-info/top_level.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2429 2023-04-29 23:47:47.000000 geowatch-0.6.6/pyproject.toml
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.755929 geowatch-0.6.6/requirements/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       68 2023-05-02 02:20:39.000000 geowatch-0.6.6/requirements/cold.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      562 2023-05-03 00:21:52.000000 geowatch-0.6.6/requirements/development.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       19 2023-05-02 02:20:39.000000 geowatch-0.6.6/requirements/dvc.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      445 2023-04-29 21:01:30.000000 geowatch-0.6.6/requirements/gdal.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      889 2023-04-03 19:39:09.000000 geowatch-0.6.6/requirements/graphics.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      979 2023-04-03 19:39:09.000000 geowatch-0.6.6/requirements/headless.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      110 2023-05-02 02:20:39.000000 geowatch-0.6.6/requirements/linting.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.6/requirements/mmcv.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      318 2023-05-02 02:20:39.000000 geowatch-0.6.6/requirements/optional.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9002 2023-05-10 15:57:19.000000 geowatch-0.6.6/requirements/runtime.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       86 2023-05-02 02:20:39.000000 geowatch-0.6.6/requirements/tensorflow.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       88 2023-04-29 21:01:30.000000 geowatch-0.6.6/requirements/tests.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      115 2023-04-29 21:01:30.000000 geowatch-0.6.6/requirements.txt
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      823 2023-04-03 19:39:09.000000 geowatch-0.6.6/run_tests.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       38 2023-05-10 18:09:56.167926 geowatch-0.6.6/setup.cfg
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10526 2023-05-03 00:21:52.000000 geowatch-0.6.6/setup.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.763929 geowatch-0.6.6/tests/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1271 2023-04-29 23:47:47.000000 geowatch-0.6.6/tests/test_cli.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2530 2023-04-29 23:47:47.000000 geowatch-0.6.6/tests/test_heterogeneous_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4038 2022-12-02 18:15:30.000000 geowatch-0.6.6/tests/test_init_from_pretrained.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2277 2023-03-21 17:57:36.000000 geowatch-0.6.6/tests/test_kwcoco_dataloader.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8409 2023-05-03 00:21:52.000000 geowatch-0.6.6/tests/test_lightning_cli_fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4446 2023-04-29 21:01:30.000000 geowatch-0.6.6/tests/test_load_models.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4367 2023-04-29 23:47:47.000000 geowatch-0.6.6/tests/test_mlops_scheduler.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7349 2023-04-29 21:01:30.000000 geowatch-0.6.6/tests/test_predict_latest_models.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4669 2023-04-29 21:01:30.000000 geowatch-0.6.6/tests/test_predict_old_fusion_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3440 2023-04-29 23:47:47.000000 geowatch-0.6.6/tests/test_predict_small_region.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6717 2023-04-29 21:01:30.000000 geowatch-0.6.6/tests/test_save_packages.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2514 2022-12-20 16:17:52.000000 geowatch-0.6.6/tests/test_sensor_metadata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13860 2023-04-29 23:47:47.000000 geowatch-0.6.6/tests/test_tracker.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      134 2022-06-07 15:49:12.000000 geowatch-0.6.6/tests/test_version.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.763929 geowatch-0.6.6/watch/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6511 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      139 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/__main__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.795929 geowatch-0.6.6/watch/cli/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       98 2023-01-18 16:43:36.000000 geowatch-0.6.6/watch/cli/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5685 2023-05-03 00:37:18.000000 geowatch-0.6.6/watch/cli/__main__.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     8875 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/cli/animate_visualizations.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6116 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/cli/baseline_framework_egress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16017 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/cli/baseline_framework_ingress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6070 2022-12-14 20:49:04.000000 geowatch-0.6.6/watch/cli/baseline_framework_kwcoco_egress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3673 2022-12-14 20:49:04.000000 geowatch-0.6.6/watch/cli/baseline_framework_kwcoco_ingress.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10809 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/cli/cluster_sites.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     6026 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/cli/coco_add_watch_fields.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    92765 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/cli/coco_align.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      215 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/cli/coco_align_geotiffs.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    32128 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/cli/coco_average_features.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    35436 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/cli/coco_clean_geotiffs.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     9577 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/cli/coco_combine_features.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22526 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/cli/coco_crop_tracks.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      224 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/cli/coco_intensity_histograms.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10102 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/cli/coco_reformat_channels.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    11078 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/cli/coco_remove_bad_images.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2679 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/cli/coco_shard.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    32293 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/cli/coco_spectra.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    47649 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/cli/coco_time_combine.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4845 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/cli/coco_update_geotiff_metadata.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    61854 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/cli/coco_visualize_videos.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1814 2022-12-14 20:49:04.000000 geowatch-0.6.6/watch/cli/concat_kwcoco_videos.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15924 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/cli/crop_sites_to_regions.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.807928 geowatch-0.6.6/watch/cli/dag_cli/
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)       89 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/cli/dag_cli/__init__.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    15320 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/cli/dag_cli/run_bas_datagen.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    13342 2023-05-01 17:33:03.000000 geowatch-0.6.6/watch/cli/dag_cli/run_bas_fusion.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10286 2023-05-01 17:33:03.000000 geowatch-0.6.6/watch/cli/dag_cli/run_dino_sv.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6939 2023-05-01 19:59:37.000000 geowatch-0.6.6/watch/cli/dag_cli/run_dzyne_parallel_site_vali.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     3529 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/cli/dag_cli/run_pseudolive_consolidate.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     3062 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/cli/dag_cli/run_psuedolive_copy_previous.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     7796 2023-05-01 17:33:03.000000 geowatch-0.6.6/watch/cli/dag_cli/run_sc_datagen.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    12667 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/cli/dag_cli/run_sc_fusion.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6224 2023-05-01 17:33:03.000000 geowatch-0.6.6/watch/cli/dag_cli/run_sv_datagen.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     5581 2023-04-03 20:48:44.000000 geowatch-0.6.6/watch/cli/dag_cli/run_teamfeat_invariants.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5448 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/cli/dag_cli/run_teamfeat_landcover.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11711 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/cli/extend_sc_sites.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4607 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/cli/find_dvc.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    12269 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/cli/geojson_site_stats.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14799 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/cli/geotiffs_to_kwcoco.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10815 2023-05-02 02:20:39.000000 geowatch-0.6.6/watch/cli/gifify.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    60496 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/cli/kwcoco_to_geojson.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4316 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/cli/merge_region_models.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/cli/mlops_cli.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10354 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/cli/prepare_splits.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    38086 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/cli/prepare_ta2_dataset.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    29987 2023-05-08 21:30:48.000000 geowatch-0.6.6/watch/cli/prepare_teamfeats.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14855 2022-12-14 20:49:04.000000 geowatch-0.6.6/watch/cli/pseudolive_consolidate.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    69727 2023-05-03 04:02:03.000000 geowatch-0.6.6/watch/cli/reproject_annotations.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       84 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/cli/run_fusion_predict.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    20415 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/cli/run_metrics_framework.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      271 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/cli/run_tracker.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.807928 geowatch-0.6.6/watch/cli/special/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 16:58:17.000000 geowatch-0.6.6/watch/cli/special/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1269 2023-05-10 17:13:51.000000 geowatch-0.6.6/watch/cli/special/finish_install.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4224 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/cli/split_videos.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22737 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/cli/stac_search.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    27798 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/cli/ta1_stac_to_kwcoco.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     9391 2023-05-10 18:09:10.000000 geowatch-0.6.6/watch/cli/torch_model_stats.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16252 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/cli/validate_annotation_schemas.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    15553 2023-05-02 02:20:39.000000 geowatch-0.6.6/watch/cli/watch_coco_stats.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.811928 geowatch-0.6.6/watch/demo/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2624 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/demo/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20892 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/demo/demo_region.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      563 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/demo/dummy_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7543 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/demo/landsat_demodata.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.819928 geowatch-0.6.6/watch/demo/metrics_demo/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      138 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/demo/metrics_demo/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7448 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/demo/metrics_demo/demo_rendering.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24604 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/demo/metrics_demo/demo_truth.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13005 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/demo/metrics_demo/demo_utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6307 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/demo/metrics_demo/generate_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15545 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/demo/metrics_demo/site_perterbing.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    29938 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/demo/nitf_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3676 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/demo/sentinel2_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25225 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/demo/smart_kwcoco_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4089 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/demo/stac_demo.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/exceptions.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.823928 geowatch-0.6.6/watch/geoannots/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      989 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/geoannots/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2308 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/geoannots/geococo_objects.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20233 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/geoannots/geomodels.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.823928 geowatch-0.6.6/watch/gis/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1645 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/gis/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9291 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/gis/digital_globe.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10020 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/gis/elevation.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    51517 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/gis/geotiff.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.827928 geowatch-0.6.6/watch/gis/sensors/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      326 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/gis/sensors/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6516 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/gis/sensors/sentinel2.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13106 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/gis/spatial_reference.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30310 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/heuristics.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.831928 geowatch-0.6.6/watch/mlops/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/mlops/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      670 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/mlops/__main__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    71493 2023-05-10 18:09:10.000000 geowatch-0.6.6/watch/mlops/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    70322 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/mlops/aggregate.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17377 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/mlops/aggregate_loader.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23469 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/mlops/confusion_visualization.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    27693 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/mlops/confusor_analysis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    40996 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/mlops/manager.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.839928 geowatch-0.6.6/watch/mlops/old/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/mlops/old/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18067 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/mlops/old/expt_manager.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39383 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/mlops/old/expt_report.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    44820 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/mlops/old/expt_state.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39219 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/mlops/old/old_pipeline_nodes.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10290 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/mlops/old/old_plots.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8717 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/mlops/old/pipeline_v1.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39647 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/mlops/old/plots.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    55834 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/mlops/pipeline_nodes.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12686 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/mlops/repackager.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16868 2023-05-10 18:09:10.000000 geowatch-0.6.6/watch/mlops/schedule_evaluation.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23776 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/mlops/smart_global_helper.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    35544 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/mlops/smart_pipeline.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    33368 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/mlops/smart_result_parser.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1042 2023-05-05 18:22:11.000000 geowatch-0.6.6/watch/mlops/write_analysis_script.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.847928 geowatch-0.6.6/watch/monkey/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       62 2022-12-14 20:49:53.000000 geowatch-0.6.6/watch/monkey/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4095 2022-12-14 20:49:53.000000 geowatch-0.6.6/watch/monkey/_monkey_fbeta.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4047 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/monkey/monkey_albumentations.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      280 2022-12-14 20:49:53.000000 geowatch-0.6.6/watch/monkey/monkey_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1187 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/monkey/monkey_lightning.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       68 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/monkey/monkey_numpy.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2022-12-14 20:49:53.000000 geowatch-0.6.6/watch/monkey/monkey_pil.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/monkey/monkey_tensorflow.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      658 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/monkey/monkey_torch.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      601 2022-12-14 20:49:53.000000 geowatch-0.6.6/watch/monkey/monkey_torchmetrics.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.851928 geowatch-0.6.6/watch/rc/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1715 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/rc/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9626 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/rc/registry.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.851928 geowatch-0.6.6/watch/stac/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       66 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/stac/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17312 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/stac/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14634 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/stac/stac_search_builder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9733 2023-05-02 02:20:39.000000 geowatch-0.6.6/watch/stac/util_stac.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.851928 geowatch-0.6.6/watch/tasks/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1677 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.855928 geowatch-0.6.6/watch/tasks/cold/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/tasks/cold/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19968 2023-05-08 21:30:48.000000 geowatch-0.6.6/watch/tasks/cold/assemble_cold_result_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21171 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/tasks/cold/export_change_map.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18403 2023-05-08 21:30:48.000000 geowatch-0.6.6/watch/tasks/cold/export_cold_result_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17519 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/tasks/cold/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    73485 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/cold/prepare_ard.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23475 2023-05-02 02:20:39.000000 geowatch-0.6.6/watch/tasks/cold/prepare_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30062 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/tasks/cold/tile_processing.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    28290 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/tasks/cold/tile_processing_kwcoco.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.859928 geowatch-0.6.6/watch/tasks/depth/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/depth/__init__.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4501 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/depth/backbone.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6559 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/depth/config.json
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6816 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/depth/datasets.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4372 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/depth/demo_transform.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     8379 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/depth/dzyne_img_util.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      295 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/depth/modules_monkeypatch.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     5239 2022-08-09 13:10:41.000000 geowatch-0.6.6/watch/tasks/depth/pl_highres_verify.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24371 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/depth/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5689 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/depth/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.859928 geowatch-0.6.6/watch/tasks/depth_pcd/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/tasks/depth_pcd/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6704 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/tasks/depth_pcd/model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      409 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/tasks/depth_pcd/model_test.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24803 2023-05-10 18:09:10.000000 geowatch-0.6.6/watch/tasks/depth_pcd/score_tracks.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.859928 geowatch-0.6.6/watch/tasks/dino_detector/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/dino_detector/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24661 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/tasks/dino_detector/building_validator.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10562 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/dino_detector/predict.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.867928 geowatch-0.6.6/watch/tasks/fusion/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2501 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/fusion/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       72 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/fusion/__main__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    82304 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/tasks/fusion/aggregate_results.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.871928 geowatch-0.6.6/watch/tasks/fusion/architectures/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      233 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/fusion/architectures/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11883 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/fusion/architectures/segmenter_decoder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5979 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/tasks/fusion/architectures/sits.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    51145 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/tasks/fusion/architectures/transformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4989 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/fusion/architectures/unet_blur.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6302 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/fusion/architectures/wu_mae.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    37328 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/tasks/fusion/coco_stitcher.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.875928 geowatch-0.6.6/watch/tasks/fusion/datamodules/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      336 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9680 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    48055 2023-05-02 02:20:39.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/batch_visualization.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8458 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/data_augment.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18677 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/data_utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9780 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/demos_for_slides.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30066 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/kwcoco_datamodule.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)   149541 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/kwcoco_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      373 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/kwcoco_video_data.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23364 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/qa_bands.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14225 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/smart_mixins.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    53890 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/spacetime_grid_builder.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.883928 geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1527 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10375 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    44675 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/affinity.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       44 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/exceptions.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9422 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/plots.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39631 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/sampler.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3384 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/time_kernel_grammar.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7352 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    55018 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/fusion/evaluate.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    28542 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/fusion/fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19157 2023-05-02 02:20:39.000000 geowatch-0.6.6/watch/tasks/fusion/fit_lightning.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.887928 geowatch-0.6.6/watch/tasks/fusion/methods/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      741 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/tasks/fusion/methods/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    82694 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/tasks/fusion/methods/channelwise_transformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    79880 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/fusion/methods/heterogeneous.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25464 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/fusion/methods/network_modules.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8960 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/fusion/methods/noop_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    28643 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/fusion/methods/unet_baseline.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    32439 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/tasks/fusion/methods/watch_module_mixins.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4468 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/fusion/organize.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    61865 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/tasks/fusion/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14958 2023-05-10 15:57:19.000000 geowatch-0.6.6/watch/tasks/fusion/production.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16789 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/fusion/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.891928 geowatch-0.6.6/watch/tasks/invariants/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/invariants/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13603 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/invariants/change.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.895928 geowatch-0.6.6/watch/tasks/invariants/data/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/invariants/data/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    35588 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/tasks/invariants/data/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20577 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/invariants/data/multi_image_datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25778 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/invariants/data/other_datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5589 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/tasks/invariants/fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4483 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/invariants/fit_segment.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6709 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/invariants/iarpa_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24760 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/tasks/invariants/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15963 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/tasks/invariants/pretext_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12941 2022-08-09 13:10:41.000000 geowatch-0.6.6/watch/tasks/invariants/segmentation_model.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.895928 geowatch-0.6.6/watch/tasks/landcover/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/landcover/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6028 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/landcover/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5623 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/landcover/detector.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      103 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/landcover/fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2377 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/landcover/model_info.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2360 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/tasks/landcover/nets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12281 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/tasks/landcover/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      349 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/landcover/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.899928 geowatch-0.6.6/watch/tasks/metrics/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/tasks/metrics/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    26517 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/tasks/metrics/merge_iarpa_metrics.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11867 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/metrics/viz_sc_results.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.899928 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.903928 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/datasets/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8025 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/datasets/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    33579 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/datasets/base_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    31719 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/datasets/iarpa_kwdataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19805 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/datasets/iarpa_sc_kwdataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    34195 2022-08-09 13:10:41.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/datasets/peo_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/fit.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.915928 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22473 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9162 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/apnb.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5007 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/base_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8375 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/discritizers.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4272 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/dynamic_unet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1276 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/early_fusion_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3510 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/early_fusion_mat_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7979 2022-08-09 13:10:41.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/late_fusion_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5652 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/mat_ed_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16573 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/patch_transformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2864 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/patch_transformer_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11476 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/peri_resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6888 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/pos_embedding.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15931 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3732 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/self_attention.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6771 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/siamese_feature_diff_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3779 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/siamese_fusion_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1833 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/simple_cnn_encoder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9772 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/simple_decoder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24297 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/timesformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6020 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/unet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8684 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/unet_lstm.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4982 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/vit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10698 2022-08-09 13:10:41.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9087 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/predict_sc.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.915928 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/utils/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/utils/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      115 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/utils/util_config.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10512 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/utils/util_misc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2112 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/utils/util_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1508 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/utils/util_paths.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9883 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/utils/util_visualize.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.915928 geowatch-0.6.6/watch/tasks/rutgers_material_seg/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.923928 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3274 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11109 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/bigearthnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4313 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/deepglobe.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5959 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/dynamicearthnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4659 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/hrscd.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13129 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/iarpa_contrastive_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8257 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/iarpa_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6702 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/inria.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3910 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/s2_self.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3309 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/s2mcp.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4659 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/spacenet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6266 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/spacenet2.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3830 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/sysucd.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:55.947928 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    42088 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/bigearthnet_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19562 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/change_vector_analysis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    26483 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/cluster_labeling.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    52228 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/compare_vw_maps.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    40645 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/deepglobe_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17085 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/deepglobe_train_val.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    46366 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/dynamicearthnet_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    42111 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/evaluation_method_comparison.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    45044 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/hrscd_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    45628 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/iarpa_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/iarpa_patch_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    45044 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/inria_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16504 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/moco_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21771 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/moco_unsupervised_material.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10831 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/mt_material_clustering_tranfer_learn.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4437 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/multi_temporal_material_clustering.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    61390 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/onera_fine_tune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    49788 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    65883 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune2.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    78136 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/onera_patch_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    56648 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/onera_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    70057 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_net.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    67609 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    66954 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet_enc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30059 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/setr_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    32133 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/shallow_seg_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    35336 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/sim_contrastive_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    48335 2023-04-19 20:35:11.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/spacenet2_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7030 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/supervised_clustering.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    60321 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/sysu_patch_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       70 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/fit.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.103927 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1466 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7650 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/canny_edge.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13281 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/deeplab.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17807 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/deeplabWS.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13507 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/deeplab_diff.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2845 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/encoding.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3794 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/gci.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      658 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/linear_classifier.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11714 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/losses.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5727 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/moco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9085 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/quantizer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11438 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7592 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/resnetGNWS.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12182 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/resnet_classification_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19182 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/resnet_enc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1414 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/sg.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4967 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/shallow_seg.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7222 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/supcon.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4278 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/tex_refine.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12022 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/transformer_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6462 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/transformer_seg.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    33755 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14703 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/predict_patchwise.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14964 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/predict_test.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.107927 geowatch-0.6.6/watch/tasks/rutgers_material_seg/scripts/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/scripts/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1884 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/scripts/filter_by_sensor.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3932 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/scripts/labelbox2coco.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.107927 geowatch-0.6.6/watch/tasks/rutgers_material_seg/utils/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/utils/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5761 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/utils/convert_sysucd_to_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3861 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/utils/cva.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12756 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/utils/eval_utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13993 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/utils/utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9925 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg/utils/visualization.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.107927 geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.111927 geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/datasets/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1728 2022-12-20 16:17:52.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/datasets/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7209 2022-12-20 16:17:52.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/datasets/base_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11244 2022-12-20 16:17:52.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/datasets/image_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11762 2022-12-20 16:17:52.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/datasets/material_pixel_dataset.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.111927 geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      446 2022-12-20 16:17:52.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5883 2022-12-20 16:17:52.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/models/material_mlp.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6146 2022-12-20 16:17:52.000000 geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/predict.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.111927 geowatch-0.6.6/watch/tasks/sam/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-02 02:20:39.000000 geowatch-0.6.6/watch/tasks/sam/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17730 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/tasks/sam/predict.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.119927 geowatch-0.6.6/watch/tasks/tracking/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1582 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/tasks/tracking/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    58673 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/tasks/tracking/from_heatmap.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2904 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/tracking/from_polygon.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30472 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/tracking/normalize.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21464 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/tasks/tracking/phase.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23668 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/tasks/tracking/utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7531 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/tasks/tracking/visualize.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.123926 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15495 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/drop0_datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3118 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/fit.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.123926 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5614 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/models/resnets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5466 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/models/unet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10027 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/models/unet_blur.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8395 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/predict.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.123926 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/spacenet/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/spacenet/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.127926 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/spacenet/data/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/spacenet/data/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2057 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/spacenet/data/create_splits.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.127926 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2093 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/create_splits_unmasked.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16199 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/spacenet/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5987 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/time_sort_S7.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4070 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/time_sort_module.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      594 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/tasks/uky_temporal_prediction/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.155926 geowatch-0.6.6/watch/utils/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2803 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/utils/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12992 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/configargparse_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    49713 2023-05-08 21:30:41.000000 geowatch-0.6.6/watch/utils/ext_monai.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11626 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/utils/ijson_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)   116813 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/utils/kwcoco_extensions.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.163926 geowatch-0.6.6/watch/utils/lightning_ext/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      376 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/utils/lightning_ext/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21356 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/utils/lightning_ext/_jsonargparse_ext_ge_4_21.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20330 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/utils/lightning_ext/_jsonargparse_ext_lt_4_21.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7034 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/lightning_ext/argparse_ext.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-10 18:09:56.167926 geowatch-0.6.6/watch/utils/lightning_ext/callbacks/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1244 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/utils/lightning_ext/callbacks/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5735 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/lightning_ext/callbacks/auto_resumer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8793 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/lightning_ext/callbacks/batch_plotter.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10112 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/lightning_ext/callbacks/packager.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2693 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/lightning_ext/callbacks/state_logger.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16120 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/lightning_ext/callbacks/tensorboard_plotter.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13026 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/lightning_ext/callbacks/text_logger.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4371 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/lightning_ext/demo.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3211 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/utils/lightning_ext/lightning_cli_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2022-12-14 20:49:53.000000 geowatch-0.6.6/watch/utils/lightning_ext/monkeypatches.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7558 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/utils/lightning_ext/old_parser_devices.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5712 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/utils/lightning_ext/util_device.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      303 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/utils/lightning_ext/util_globals.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      434 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/utils/lightning_ext/util_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10606 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/partial_format.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11208 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/process_context.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    56710 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/utils/result_analysis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5456 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/reverse_hashid.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14160 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/utils/simple_dvc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8514 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/utils/slugify_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    41201 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/utils/util_bands.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1059 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/utils/util_codes.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12129 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/utils/util_data.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7144 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/util_dotdict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1813 2023-02-27 18:47:15.000000 geowatch-0.6.6/watch/utils/util_environ.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8342 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/utils/util_eval.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7920 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/utils/util_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    50402 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/utils/util_gdal.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6368 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/utils/util_girder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    43860 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/utils/util_gis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2970 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/utils/util_globals.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2039 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/utils/util_hardware.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2589 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/utils/util_iter.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3455 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/util_json.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    41820 2023-05-01 17:33:03.000000 geowatch-0.6.6/watch/utils/util_kwarray.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    67297 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/utils/util_kwimage.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14504 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/utils/util_kwplot.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3771 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/utils/util_locks.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8978 2022-12-14 20:49:04.000000 geowatch-0.6.6/watch/utils/util_logging.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1035 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/util_nesting.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12514 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/util_netharn.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10172 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/utils/util_nvidia.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10275 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/util_pandas.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5747 2023-05-09 01:10:52.000000 geowatch-0.6.6/watch/utils/util_parallel.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25992 2023-05-02 02:20:39.000000 geowatch-0.6.6/watch/utils/util_param_grid.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18404 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/util_path.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13282 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/util_pattern.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23235 2023-04-29 21:01:30.000000 geowatch-0.6.6/watch/utils/util_progress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15872 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/utils/util_raster.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3028 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/utils/util_regex.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7614 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/utils/util_resolution.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4674 2023-05-05 02:31:10.000000 geowatch-0.6.6/watch/utils/util_resources.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3083 2022-06-07 15:49:12.000000 geowatch-0.6.6/watch/utils/util_rgdc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      570 2022-12-02 18:15:30.000000 geowatch-0.6.6/watch/utils/util_s3.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7307 2023-03-21 17:57:36.000000 geowatch-0.6.6/watch/utils/util_stringalgo.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13699 2023-04-03 19:39:09.000000 geowatch-0.6.6/watch/utils/util_time.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1786 2022-12-20 16:17:52.000000 geowatch-0.6.6/watch/utils/util_torchmetrics.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2133 2023-05-03 00:21:52.000000 geowatch-0.6.6/watch/utils/util_windows.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9413 2023-04-29 23:47:47.000000 geowatch-0.6.6/watch/utils/util_yaml.py
```

### Comparing `geowatch-0.6.3/CHANGELOG.md` & `geowatch-0.6.6/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,46 @@
 # Changelog
 
 This changelog follows the specifications detailed in: [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html), although we have not yet reached a `1.0.0` release.
 
 
-## Version 0.6.2 - Target 2023-05-x
+## Version 0.6.4 - Target 2023-05-x
 
 ### Added
 
 * SAM - segment anything features
-* DZYNE site validation: depthPCD task
+* DZYNE site validation: `depth_pcd` task
 * fusion.predict can now output pngs
+* Added `request_rlimit_nofile` to KWCocoVideoDataModule for easier ulimit configuration
+* The `fusion.predict` script can now output predictions in cog or png format
+* Added transient labels to heuristics
+* Add `rescale_nans` param to MultimodalTransformer.
+* Add `cooldown` argument to coco align script to specify time between tries.
+* Integrated `depth_pcd` into MLOps under the `sv_depth_filter` node.
 
 ### Changed
 
 * Tweaked dependencies for windows
 * The kwcoco video dataset now respects the weight attribute in annotations.
 * Reorganized docs
 * `coco_align` now uses process context
 * Change weights now use geometric mean instead of direct product
+* Documentation improvements
+* Now using scriptconfig in fusion.predict
+* Reworked how submatrices behave in mlops, added submatrices1, submatrices2. Concept might need refinement.
+* Update site / region schemas
+
+
+### Fixed
+* safer no longer uses `temp_file` on windows
+* Erroneous assertion errors in reproject and kwcoco-to-geotiffs
+* Issue where `DINO_SV` would write region models to the out-site-manifest, now correctly points at site models.
+* Bug in coco-align where nodata values were not properly set on data that moved through gdal-merge.
+
 
 ## Version 0.5.6 - Target 2023-04-30
 
 ### Added
 * `coco_time_combine` can now ignore seasons / handle median images with less memory
 * `use_grid_negatives` as dataset option, which can be set to "cleared" to only use negatives from cleared regions.
 * Add `modality_dropout` to kwcoco dataloader
```

### Comparing `geowatch-0.6.3/Dockerfile` & `geowatch-0.6.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/LICENSE` & `geowatch-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/PKG-INFO` & `geowatch-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geowatch
-Version: 0.6.3
+Version: 0.6.6
 Home-page: https://gitlab.kitware.com/computer-vision/geowatch.git
 Author: GEOWATCH developers
 Author-email: kitware@kitware.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `geowatch-0.6.3/README.rst` & `geowatch-0.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/conda_env.yml` & `geowatch-0.6.6/conda_env.yml`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/README.rst` & `geowatch-0.6.6/docs/README.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/algorithms/fusion_overview.rst` & `geowatch-0.6.6/docs/algorithms/fusion_overview.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/algorithms/sensorchan_specs.rst` & `geowatch-0.6.6/docs/algorithms/sensorchan_specs.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/algorithms/ta2_deep_dive_info.md` & `geowatch-0.6.6/docs/algorithms/ta2_deep_dive_info.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/data/access_dvc_repos.rst` & `geowatch-0.6.6/docs/data/access_dvc_repos.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/data/internal_resources.rst` & `geowatch-0.6.6/docs/data/internal_resources.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/data/using_smartwatch_dvc.rst` & `geowatch-0.6.6/docs/data/using_smartwatch_dvc.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/debugging/debugging_cmdqueue.rst` & `geowatch-0.6.6/docs/debugging/debugging_cmdqueue.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/development/coding_conventions.rst` & `geowatch-0.6.6/docs/development/coding_conventions.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/development/coding_tips.rst` & `geowatch-0.6.6/docs/development/coding_tips.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/development/contribution_instructions.rst` & `geowatch-0.6.6/docs/development/contribution_instructions.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/development/rebasing_procedure.rst` & `geowatch-0.6.6/docs/development/rebasing_procedure.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/development/ta2_feature_integration.md` & `geowatch-0.6.6/docs/development/ta2_feature_integration.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/environment/getting_started_aws.rst` & `geowatch-0.6.6/docs/environment/getting_started_aws.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/environment/getting_started_dvc.rst` & `geowatch-0.6.6/docs/environment/getting_started_dvc.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/environment/getting_started_kubectl.rst` & `geowatch-0.6.6/docs/environment/getting_started_kubectl.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/environment/getting_started_ssh_keys.rst` & `geowatch-0.6.6/docs/environment/getting_started_ssh_keys.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/environment/install_python.rst` & `geowatch-0.6.6/docs/environment/install_python.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/environment/install_python_conda.rst` & `geowatch-0.6.6/docs/environment/install_python_conda.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/environment/install_python_pyenv.rst` & `geowatch-0.6.6/docs/environment/install_python_pyenv.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/environment/installing_geowatch.rst` & `geowatch-0.6.6/docs/environment/installing_geowatch.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/environment/windows.rst` & `geowatch-0.6.6/docs/environment/windows.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/misc/structure_proposal.md` & `geowatch-0.6.6/docs/misc/structure_proposal.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/misc/supporting_projects.rst` & `geowatch-0.6.6/docs/misc/supporting_projects.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/mlops.md` & `geowatch-0.6.6/docs/mlops.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/onboarding.rst` & `geowatch-0.6.6/docs/onboarding.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/smartflow/getting_started_smartflow.rst` & `geowatch-0.6.6/docs/smartflow/getting_started_smartflow.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/smartflow/smartflow_copying_large_files_to_efs.md` & `geowatch-0.6.6/docs/smartflow/smartflow_copying_large_files_to_efs.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/smartflow/smartflow_running_the_system.rst` & `geowatch-0.6.6/docs/smartflow/smartflow_running_the_system.rst`

 * *Files 4% similar despite different names*

```diff
@@ -431,34 +431,105 @@
         airflow dags unpause kit_ta2_preeval10_pyenv_t31_batch_$REGION_ID
     done
 
 
     # Status queries
     airflow dags list-jobs -d kit_ta2_preeval10_pyenv_t33_post1_batch_KR_R001 -o yaml
     airflow dags list-runs -d kit_ta2_preeval10_pyenv_t33_post1_batch_KR_R001 -o yaml
+    airflow dags list-runs -d kit_eval_11_rerun_batch_AE_R001 -o yaml
     '
 
 
     ### Alternative - execute commands from local shell
     # Oddly this tends to send outputs with color that we need to strip out.
+    JQ_QUERY='.items[] | select(.metadata.name | startswith("airflow-scheduler-")) | .metadata.name'
+    AIRFLOW_SCHEDULER_POD_NAME=$(kubectl -n airflow get pods -o json | jq -r "$JQ_QUERY")
+    export AIRFLOW_SCHEDULER_POD_NAME
     kubectl -n airflow exec -it pods/$AIRFLOW_SCHEDULER_POD_NAME -- airflow dags list -o json > dags.json
     cat dags.json | sed -r "s/\x1B\[([0-9]{1,3}(;[0-9]{1,2};?)?)?[mGK]//g" | cat > dags_nocolor.json
 
+    airflow dag_state kit_eval_11_rerun_batch_AE_C002
+
+    # Note:
+    # This idea will be further developed in
+    ~/code/watch-smartflow-dags/monitor_dags.py
+
     python -c "if True:
         import json
         import pathlib
         import cmd_queue
 
         # Build pattern to identify the jobs you want to run
         import xdev
         pattern = xdev.MultiPattern.coerce([
-            f'kit_ta2_preeval10_pyenv_t{t}*'
-            for t in [31, 35]
+            'kit_eval_11_rerun_batch*'
+            #f'kit_ta2_preeval10_pyenv_t{t}*'
+            #for t in [31, 35]
         ])
-        data = json.loads(pathlib.Path('dags_nocolor.json').read_text())
+        # FIXME: the json can be output with an error, need to strip it.
+        text = pathlib.Path('dags_nocolor.json').read_text()
+        data = json.loads(text[86:])
+
+
+        valid_rows = []
+        for item in data:
+            if pattern.match(item['dag_id']):
+                valid_rows.append(item)
+
+
+        if 0:
+            # Query the status of the selected dags
+            import os
+            AIRFLOW_SCHEDULER_POD_NAME = os.environ['AIRFLOW_SCHEDULER_POD_NAME']
+            prefix = f'kubectl -n airflow exec -it pods/{AIRFLOW_SCHEDULER_POD_NAME} -- '
+
+            import base64
+            # easy-to-represent char encoding of the strip ansi pattern
+            pat = base64.b32decode(b'DNOFWKC3GAWTSXL3GEWDG7JIHNNTALJZLV5TCLBSPU5T6KJ7FE7VW3KHJNOQ====').decode('utf8')
+            import re
+            pat = re.compile(pat)
+            from watch.utils.util_yaml import Yaml
+            row_to_states = {}
+            for row in valid_rows:
+                dag_id = row['dag_id']
+                info = ub.cmd(prefix + f'airflow dags list-runs -d {dag_id} -o yaml', shell=True)
+                text = pat.sub('', info['out'])
+                states = Yaml.loads(text)
+                print(ub.urepr(states))
+                row_to_states[dag_id] = states
+
+            orig_row = {r['dag_id']: r for r in valid_rows}
+            dag_info_rows = []
+            for dag_id, states in row_to_states.items():
+                row = orig_row[dag_id]
+                if len(states) == 0:
+                    row['status'] = None
+                else:
+                    mrs = states[-1]
+                    row['status'] = mrs['state']
+                    row['execution_date'] = mrs['execution_date']
+                    row['run_id'] = mrs['run_id']
+                    row['start_date'] = mrs['start_date']
+                    row['end_date'] = mrs['end_date']
+                dag_info_rows.append(row)
+
+            import pandas as pd
+            df = pd.DataFrame(dag_info_rows)
+            import rich
+            rich.print(df)
+
+            num_need_run = pd.isna(df['status']).sum()
+            num_running = (df['status'] == 'running').sum()
+            print(f'num_need_run={num_need_run}')
+            print(f'num_running={num_running}')
+
+        import pandas as pd
+        df = pd.DataFrame(valid_rows)
+        import rich
+        rich.print(df)
 
         # Build cmd-queue with the commands to execute
         queue = cmd_queue.Queue.create(backend='serial')
         prefix = 'kubectl -n airflow exec -it pods/$AIRFLOW_SCHEDULER_POD_NAME -- '
         for item in data:
             if pattern.match(item['dag_id']):
                 print(item['dag_id'])
```

### Comparing `geowatch-0.6.3/docs/smartflow/smartflow_training_fusion_models.md` & `geowatch-0.6.6/docs/smartflow/smartflow_training_fusion_models.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/testing/running_ci_locally.rst` & `geowatch-0.6.6/docs/testing/running_ci_locally.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/testing/testing_practices.rst` & `geowatch-0.6.6/docs/testing/testing_practices.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/docs/watch_cli.rst` & `geowatch-0.6.6/docs/watch_cli.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/geowatch.egg-info/PKG-INFO` & `geowatch-0.6.6/geowatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geowatch
-Version: 0.6.3
+Version: 0.6.6
 Home-page: https://gitlab.kitware.com/computer-vision/geowatch.git
 Author: GEOWATCH developers
 Author-email: kitware@kitware.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `geowatch-0.6.3/geowatch.egg-info/SOURCES.txt` & `geowatch-0.6.6/geowatch.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 geowatch/cli/dag_cli/run_bas_datagen.py
 geowatch/cli/dag_cli/run_bas_fusion.py
 geowatch/cli/dag_cli/run_pseudolive_consolidate.py
 geowatch/cli/dag_cli/run_psuedolive_copy_previous.py
 geowatch/cli/dag_cli/run_sc_datagen.py
 geowatch/cli/dag_cli/run_sc_fusion.py
 geowatch/cli/dag_cli/run_teamfeat_invariants.py
+geowatch/cli/special/__init__.py
 geowatch/demo/__init__.py
 geowatch/demo/demo_region.py
 geowatch/demo/dummy_demodata.py
 geowatch/demo/landsat_demodata.py
 geowatch/demo/nitf_demodata.py
 geowatch/demo/sentinel2_demodata.py
 geowatch/demo/smart_kwcoco_demodata.py
@@ -551,14 +552,16 @@
 watch/cli/dag_cli/run_pseudolive_consolidate.py
 watch/cli/dag_cli/run_psuedolive_copy_previous.py
 watch/cli/dag_cli/run_sc_datagen.py
 watch/cli/dag_cli/run_sc_fusion.py
 watch/cli/dag_cli/run_sv_datagen.py
 watch/cli/dag_cli/run_teamfeat_invariants.py
 watch/cli/dag_cli/run_teamfeat_landcover.py
+watch/cli/special/__init__.py
+watch/cli/special/finish_install.py
 watch/demo/__init__.py
 watch/demo/demo_region.py
 watch/demo/dummy_demodata.py
 watch/demo/landsat_demodata.py
 watch/demo/nitf_demodata.py
 watch/demo/sentinel2_demodata.py
 watch/demo/smart_kwcoco_demodata.py
@@ -589,14 +592,15 @@
 watch/mlops/manager.py
 watch/mlops/pipeline_nodes.py
 watch/mlops/repackager.py
 watch/mlops/schedule_evaluation.py
 watch/mlops/smart_global_helper.py
 watch/mlops/smart_pipeline.py
 watch/mlops/smart_result_parser.py
+watch/mlops/write_analysis_script.py
 watch/mlops/old/__init__.py
 watch/mlops/old/expt_manager.py
 watch/mlops/old/expt_report.py
 watch/mlops/old/expt_state.py
 watch/mlops/old/old_pipeline_nodes.py
 watch/mlops/old/old_plots.py
 watch/mlops/old/pipeline_v1.py
@@ -633,18 +637,18 @@
 watch/tasks/depth/datasets.py
 watch/tasks/depth/demo_transform.py
 watch/tasks/depth/dzyne_img_util.py
 watch/tasks/depth/modules_monkeypatch.py
 watch/tasks/depth/pl_highres_verify.py
 watch/tasks/depth/predict.py
 watch/tasks/depth/utils.py
-watch/tasks/depthPCD/__init__.py
-watch/tasks/depthPCD/model.py
-watch/tasks/depthPCD/model_test.py
-watch/tasks/depthPCD/score_tracks.py
+watch/tasks/depth_pcd/__init__.py
+watch/tasks/depth_pcd/model.py
+watch/tasks/depth_pcd/model_test.py
+watch/tasks/depth_pcd/score_tracks.py
 watch/tasks/dino_detector/__init__.py
 watch/tasks/dino_detector/building_validator.py
 watch/tasks/dino_detector/predict.py
 watch/tasks/fusion/__init__.py
 watch/tasks/fusion/__main__.py
 watch/tasks/fusion/aggregate_results.py
 watch/tasks/fusion/coco_stitcher.py
```

### Comparing `geowatch-0.6.3/geowatch.egg-info/requires.txt` & `geowatch-0.6.6/geowatch.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 fasteners>=0.16.3
 more_itertools>=8.12.0
 pint>=0.17
 retry>=0.9.2
 girder_client>=3.1.15
 tempenv>=0.2.0
 pystac_client>=0.5.1
-scriptconfig>=0.7.7
+scriptconfig>=0.7.8
 pygtrie>=2.3.3
 networkx>=2.8.0
 python_dateutil>=2.8.2
 pytimeparse>=1.1.8
 progiter>=1.1.0
 fire>=0.4.0
 lark>=1.1.2
@@ -202,15 +202,15 @@
 fasteners>=0.16.3
 more_itertools>=8.12.0
 pint>=0.17
 retry>=0.9.2
 girder_client>=3.1.15
 tempenv>=0.2.0
 pystac_client>=0.5.1
-scriptconfig>=0.7.7
+scriptconfig>=0.7.8
 pygtrie>=2.3.3
 networkx>=2.8.0
 python_dateutil>=2.8.2
 pytimeparse>=1.1.8
 progiter>=1.1.0
 fire>=0.4.0
 lark>=1.1.2
@@ -292,15 +292,15 @@
 fasteners==0.16.3
 more_itertools==8.12.0
 pint==0.17
 retry==0.9.2
 girder_client==3.1.15
 tempenv==0.2.0
 pystac_client==0.5.1
-scriptconfig==0.7.7
+scriptconfig==0.7.8
 pygtrie==2.3.3
 networkx==2.8.0
 python_dateutil==2.8.2
 pytimeparse==1.1.8
 progiter==1.1.0
 fire==0.4.0
 lark==1.1.2
@@ -771,15 +771,15 @@
 fasteners==0.16.3
 more_itertools==8.12.0
 pint==0.17
 retry==0.9.2
 girder_client==3.1.15
 tempenv==0.2.0
 pystac_client==0.5.1
-scriptconfig==0.7.7
+scriptconfig==0.7.8
 pygtrie==2.3.3
 networkx==2.8.0
 python_dateutil==2.8.2
 pytimeparse==1.1.8
 progiter==1.1.0
 fire==0.4.0
 lark==1.1.2
```

### Comparing `geowatch-0.6.3/pyproject.toml` & `geowatch-0.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/requirements/development.txt` & `geowatch-0.6.6/requirements/development.txt`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/requirements/graphics.txt` & `geowatch-0.6.6/requirements/graphics.txt`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/requirements/headless.txt` & `geowatch-0.6.6/requirements/headless.txt`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/requirements/runtime.txt` & `geowatch-0.6.6/requirements/runtime.txt`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 lxml>=4.6.3     ; python_version < '3.11' and python_version >= '3.10'    # Python 3.10
 lxml>=4.5.2     ; python_version < '3.10' and python_version >= '3.9'     # Python 3.9
 lxml>=4.4.1     ; python_version < '3.9'  and python_version >= '3.8'     # Python 3.8
 lxml>=4.2.4     ; python_version < '3.8'  and python_version >= '3.7'     # Python 3.7
 
 tempenv>=0.2.0
 pystac_client>=0.5.1
-scriptconfig>=0.7.7
+scriptconfig>=0.7.8
 pygtrie>=2.3.3
 # protobuf>=3.15.8
 networkx>=2.8.0
 python_dateutil>=2.8.2
 pytimeparse>=1.1.8
 progiter>=1.1.0
 fire>=0.4.0
```

### Comparing `geowatch-0.6.3/run_tests.py` & `geowatch-0.6.6/run_tests.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/setup.py` & `geowatch-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_cli.py` & `geowatch-0.6.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_heterogeneous_model.py` & `geowatch-0.6.6/tests/test_heterogeneous_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_init_from_pretrained.py` & `geowatch-0.6.6/tests/test_init_from_pretrained.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_kwcoco_dataloader.py` & `geowatch-0.6.6/tests/test_kwcoco_dataloader.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_lightning_cli_fit.py` & `geowatch-0.6.6/tests/test_lightning_cli_fit.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_load_models.py` & `geowatch-0.6.6/tests/test_load_models.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_mlops_scheduler.py` & `geowatch-0.6.6/tests/test_mlops_scheduler.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_predict_latest_models.py` & `geowatch-0.6.6/tests/test_predict_latest_models.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_predict_old_fusion_model.py` & `geowatch-0.6.6/tests/test_predict_old_fusion_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_predict_small_region.py` & `geowatch-0.6.6/tests/test_predict_small_region.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_save_packages.py` & `geowatch-0.6.6/tests/test_save_packages.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_sensor_metadata.py` & `geowatch-0.6.6/tests/test_sensor_metadata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/tests/test_tracker.py` & `geowatch-0.6.6/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/__init__.py` & `geowatch-0.6.6/watch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 The GEOWATCH module
 
 Useful environs:
     DVC_DATA_DPATH=$(geowatch_dvc --tags='phase2_data' --hardware=auto)
     DVC_EXPT_DPATH=$(geowatch_dvc --tags='phase2_expt' --hardware=auto)
+    DATA_DVC_DPAVH=$DVC_DATA_DPATH
+    EXPT_DVC_DPATH=$DVC_EXPT_DPATH
 """
 import os
 import sys
 import ubelt as ub
 import warnings
 
 
-__version__ = '0.6.3'
+__version__ = '0.6.6'
 
 
 # ~/code/watch/dev/maintain/generate_authors.py
 __author__ = 'GEOWATCH Developers, Kitware Inc., Jon Crall, David Joy, Matthew Bernstein, Connor Greenwell, Benjamin Brodie, Peri Akiva, Usman Rafique, Jacob DeRosa, Matthew Purri, Ajay Upadhyaya, Ji Won Suh, Jacob Birge, Ryan LaClair, Scott Workman, Dexter Lau, Sergii Skakun, Aram Ansary Ogholbake, Cohen Archbold, Bane Sullivan, Srikumar Sastry, Armin Hadzic'
 
 __author_email__ = 'kitware@kitware.com, jon.crall@kitware.com'
 __url__ = 'https://gitlab.kitware.com/computer-vision/geowatch'
@@ -44,15 +46,17 @@
 
 def _import_troublesome_module(modname):
     """
     Defines exactly how to import each troublesome (binary) module
     """
     if modname == 'gdal':
         from osgeo import gdal as module
-        module.UseExceptions()
+        gdal = module
+        if not getattr(gdal, '_UserHasSpecifiedIfUsingExceptions', lambda: False)():
+            gdal.UseExceptions()
     elif modname == 'pyproj':
         import pyproj as module
         from pyproj import CRS  # NOQA
     elif modname == 'geopandas':
         with warnings.catch_warnings():
             warnings.filterwarnings('ignore', (
                 '.*is incompatible with the GEOS version '
```

### Comparing `geowatch-0.6.3/watch/cli/__main__.py` & `geowatch-0.6.6/watch/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/animate_visualizations.py` & `geowatch-0.6.6/watch/cli/animate_visualizations.py`

 * *Files 11% similar despite different names*

```diff
@@ -101,14 +101,19 @@
     pman = util_progress.ProgressManager()
     pman.__enter__()
 
     # prog = ub.ProgIter(desc='submit video jobs', verbose=3)
     prog = pman.progiter(desc='submit video jobs')
     prog.begin()
 
+    with_gif = 'auto'
+    with_mp4 = True
+
+    outputs = []
+
     for type_ in types:
         for video_dpath in video_dpaths:
             prog.set_extra('type_={!r} video_dpath={!r}'.format(type_, video_dpath))
             prog.step()
             video_name = video_dpath.name
 
             if zoom_to_tracks:
@@ -130,42 +135,64 @@
                             if len(frame_fpaths) < 300:
                                 gif_fname = '{}{}_{}.gif'.format(track_name, type_, chan_dpath.name)
                                 gif_fpath = track_subdpath / gif_fname
                                 pool.submit(
                                     gifify.ffmpeg_animate_frames, frame_fpaths,
                                     gif_fpath, in_framerate=frames_per_second,
                                     verbose=verbose_worker)
+                                outputs.append({
+                                    'fpath': gif_fpath,
+                                    'type': 'gif',
+                                })
                             ani_fname = '{}{}_{}.mp4'.format(track_name, type_, chan_dpath.name)
                             ani_fpath = track_subdpath / ani_fname
                             pool.submit(
                                 gifify.ffmpeg_animate_frames, frame_fpaths,
                                 ani_fpath, in_framerate=frames_per_second,
                                 verbose=verbose_worker)
+                            outputs.append({
+                                'fpath': ani_fpath,
+                                'type': 'mp4',
+                            })
 
             else:
                 type_dpath = video_dpath / type_
                 if channels is None:
                     channel_dpaths = [p for p in type_dpath.glob('*') if p.is_dir()]
                 else:
                     channel_dpaths = [type_dpath / c.path_sanitize()
                                       for c in channels.streams()]
                 for chan_dpath in channel_dpaths:
                     frame_fpaths = sorted(chan_dpath.glob('*'))
                     if len(frame_fpaths):
-                        if len(frame_fpaths) < 300:
+                        with_gif_resolved = with_gif
+                        if with_gif == 'auto':
+                            with_gif_resolved = len(frame_fpaths) < 300
+
+                        if with_gif_resolved:
                             gif_fname = '{}{}_{}.gif'.format(video_name, type_, chan_dpath.name)
                             gif_fpath = video_dpath / gif_fname
                             pool.submit(
                                 gifify.ffmpeg_animate_frames, frame_fpaths, gif_fpath,
                                 in_framerate=frames_per_second, verbose=verbose_worker)
-                        ani_fname = '{}{}_{}.mp4'.format(video_name, type_, chan_dpath.name)
-                        ani_fpath = video_dpath / ani_fname
-                        pool.submit(
-                            gifify.ffmpeg_animate_frames, frame_fpaths, ani_fpath,
-                            in_framerate=frames_per_second, verbose=verbose_worker)
+                            outputs.append({
+                                'fpath': gif_fpath,
+                                'type': 'gif',
+                            })
+
+                        if with_mp4:
+                            ani_fname = '{}{}_{}.mp4'.format(video_name, type_, chan_dpath.name)
+                            ani_fpath = video_dpath / ani_fname
+                            pool.submit(
+                                gifify.ffmpeg_animate_frames, frame_fpaths, ani_fpath,
+                                in_framerate=frames_per_second, verbose=verbose_worker)
+                            outputs.append({
+                                'fpath': ani_fpath,
+                                'type': 'mp4',
+                            })
     prog.end()
 
     failed = []
     # for job in ub.ProgIter(pool.as_completed(), total=len(pool), desc='collect animate jobs'):
     for job in pman.progiter(pool.as_completed(), total=len(pool), desc='collect animate jobs'):
         try:
             job.result()
@@ -180,14 +207,15 @@
 
     pman.__exit__(None, None, None)
 
     print('Wrote animations to viz_dpath = {!r}'.format(viz_dpath))
     # The animation jobs can do something weird to the tty, so we should try
     # and fix it.
     ub.cmd('stty sane')
+    return outputs
 
 
 if __name__ == '__main__':
     """
     CommandLine:
         python ~/code/watch/watch/cli/animate_visualizations.py
     """
```

### Comparing `geowatch-0.6.3/watch/cli/baseline_framework_egress.py` & `geowatch-0.6.6/watch/cli/baseline_framework_egress.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/baseline_framework_ingress.py` & `geowatch-0.6.6/watch/cli/baseline_framework_ingress.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/baseline_framework_kwcoco_egress.py` & `geowatch-0.6.6/watch/cli/baseline_framework_kwcoco_egress.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/baseline_framework_kwcoco_ingress.py` & `geowatch-0.6.6/watch/cli/baseline_framework_kwcoco_ingress.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/cluster_sites.py` & `geowatch-0.6.6/watch/cli/cluster_sites.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/coco_add_watch_fields.py` & `geowatch-0.6.6/watch/cli/coco_add_watch_fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,56 @@
+#!/usr/bin/env python3
 """
 Adds fields needed by ndsampler to correctly "watch" a region.
 
 Some of this is done hueristically. We assume images come from certain sensors.
 We assume input is orthorectified.  We assume some GSD "target" gsd for video
 and image processing. Note a video GSD will typically be much higher (i.e.
 lower resolution) than an image GSD.
+
+SeeAlso:
+    ~/code/watch/watch/utils/kwcoco_extensions.py
 """
 import ubelt as ub
 import scriptconfig as scfg
 
 
 class AddWatchFieldsConfig(scfg.DataConfig):
     """
     Updates image transforms in a kwcoco json file to align all videos to a
     target GSD.
     """
-    __default__ = {
-        'src': scfg.Value('data.kwcoco.json', help='input kwcoco filepath', position=1),
+    src = scfg.Value('data.kwcoco.json', help='input kwcoco filepath', position=1)
 
-        'dst': scfg.Value(None, help='output kwcoco filepath', position=2),
+    dst = scfg.Value(None, help='output kwcoco filepath', position=2)
 
-        'inplace': scfg.Value(False, isflag=True, help=ub.paragraph(
-            '''
-            if True and dst is unspecified then the output will overwrite the input
-            ''')),
+    inplace = scfg.Value(False, isflag=True, help=ub.paragraph(
+        '''
+        if True and dst is unspecified then the output will overwrite the input
+        '''))
 
-        'target_gsd': scfg.Value(10.0, help='compute transforms for a target gsd'),
+    target_gsd = scfg.Value(10.0, help='compute transforms for a target gsd')
 
-        'overwrite': scfg.Value(False, help='if True overwrites introspectable fields'),
+    overwrite = scfg.Value(False, help='if True overwrites introspectable fields')
 
-        'edit_geotiff_metadata': scfg.Value(False, help='if True MODIFIES THE UNDERLYING IMAGES to ensure geodata is propogated'),
+    edit_geotiff_metadata = scfg.Value(False, help='if True MODIFIES THE UNDERLYING IMAGES to ensure geodata is propogated')
 
-        'default_gsd': scfg.Value(None, help='if specified, assumed any images without geo-metadata have this GSD'),
+    default_gsd = scfg.Value(None, help='if specified, assumed any images without geo-metadata have this GSD')
 
-        'workers': scfg.Value(0, type=str, help='number of io threads'),
+    workers = scfg.Value(0, type=str, help='number of io threads')
 
-        'mode': scfg.Value('process', help='can be thread, process, or serial'),
+    mode = scfg.Value('process', help='can be thread, process, or serial')
 
-        'enable_video_stats': scfg.Value(True, help='set to False to disable video stats'),
+    enable_video_stats = scfg.Value(True, help='set to False to disable video stats')
 
-        'enable_valid_region': scfg.Value(False, help='set to True to enable valid region computation'),
+    enable_valid_region = scfg.Value(False, help='set to True to enable valid region computation')
 
-        'enable_intensity_stats': scfg.Value(False, help='if True, will compute intensity statistics on each channel of each image'),
+    enable_intensity_stats = scfg.Value(False, help='if True, will compute intensity statistics on each channel of each image')
 
-        'remove_broken': scfg.Value(False, help='if True, will remove any image that fails population (e.g. caused by a 404)')
-    }
+    remove_broken = scfg.Value(False, help='if True, will remove any image that fails population (e.g. caused by a 404)')
 
 
 def main(cmdline=True, **kwargs):
     r"""
     CommandLine:
 
         kwcoco toydata --key vidshapes8-multispectral --dst toydata.kwcoco.json
@@ -70,45 +72,37 @@
 
     Ignore:
         python -m watch.cli.coco_add_watch_fields \
             --src=$HOME/data/dvc-repos/smart_watch_dvc/drop0_aligned_msi/data.kwcoco.json \
             --dst=$HOME/data/dvc-repos/smart_watch_dvc/drop0_aligned_msi/data.kwcoco.new.json \
             --target_gsd=10
 
-    jq .images[0].auxiliary[0] $HOME/data/dvc-repos/smart_watch_dvc/drop0_aligned_msi/data.kwcoco.new.json
-    jq .images[0].auxiliary[0] $HOME/data/dvc-repos/smart_watch_dvc/drop0_aligned_msi/data.kwcoco.json
+        jq .images[0].auxiliary[0] $HOME/data/dvc-repos/smart_watch_dvc/drop0_aligned_msi/data.kwcoco.new.json
+        jq .images[0].auxiliary[0] $HOME/data/dvc-repos/smart_watch_dvc/drop0_aligned_msi/data.kwcoco.json
 
     Example:
         >>> from watch.cli.coco_add_watch_fields import *  # NOQA
         >>> import kwcoco
         >>> # TODO: make a demo dataset with some sort of gsd metadata
         >>> dset = kwcoco.CocoDataset.demo('vidshapes8-multispectral')
         >>> print('dset = {!r}'.format(dset))
         >>> target_gsd = 13.0
-        >>> main(cmdline=False, src=dset, target_gsd=target_gsd, default_gsd=1)
+        >>> main(cmdline=False, src=dset, dst='return', target_gsd=target_gsd, default_gsd=1)
         >>> print('dset.index.imgs[1] = ' + ub.urepr(dset.index.imgs[1], nl=2))
         >>> print('dset.index.videos = {}'.format(ub.urepr(dset.index.videos, nl=1)))
-
-    Ignore:
-        kwargs = {
-            'src': ub.expandpath('~/data/dvc-repos/smart_watch_dvc/drop0_aligned/data.kwcoco.json'),
-            'target_gsd': 10.0,
-            'dst': None,
-        }
-        kwargs['src'] = kwargs['dst']
-        main(**kwargs)
     """
+    import rich
+    config = AddWatchFieldsConfig.cli(default=kwargs, cmdline=cmdline, strict=True)
+    rich.print('config = {}'.format(ub.urepr(config, nl=1)))
     from watch import heuristics
     import numpy as np
     import kwcoco
     import kwimage
     from watch.utils import util_parallel
     from watch.utils import kwcoco_extensions
-    config = AddWatchFieldsConfig(kwargs, cmdline=cmdline)
-    print('config = {}'.format(ub.urepr(dict(config), nl=1)))
 
     if config['dst'] is None:
         if config['inplace']:
             config['dst'] = config['dst'] = config['src']
         else:
             raise ValueError('must specify dst: {}'.format(config['dst']))
 
@@ -141,15 +135,17 @@
             offset =  np.asarray(kwimage.Affine.coerce(img['warp_img_to_vid']))[:, 2]
             if np.any(np.abs(offset) > 100):
                 print('img = {}'.format(ub.urepr(img, nl=-1)))
                 print('warning there is a large offset (this is ok if we are not expecting this dataset to be aligned)')
                 print('offset = {!r}'.format(offset))
                 print('{}, {}'.format(gid, img['warp_img_to_vid']))
 
-    if config['dst'] is not None:
+    if config['dst'] == 'return':
+        return dset
+    elif config['dst'] is not None:
         print('write dataset')
         dset.fpath = config['dst']
         print('dset.fpath = {!r}'.format(dset.fpath))
         dset.dump(dset.fpath, newlines=True)
     else:
         print('not writing')
```

### Comparing `geowatch-0.6.3/watch/cli/coco_align.py` & `geowatch-0.6.6/watch/cli/coco_align.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,27 +52,14 @@
         --workers=10 \
         --aux_workers=2 \
         --context_factor=1 \
         --visualize=False \
         --geo_preprop=False \
         --include_sensors=WV \
         --keep img
-
-
-TODO:
-    - [ ] Add method for extracting "negative ROIs" that are nearby
-        "positive ROIs".
-
-    - [X] Diagnose and Fix PROJ errors:
-
-        ```
-        ERROR 1: PROJ: proj_create: unrecognized format / unknown name
-        ERROR 1: PROJ: proj_create_from_database: Cannot find proj.db
-        ```
-    - [ ] Rename file to coco_geoalign.py
 """
 import os
 import scriptconfig as scfg
 import ubelt as ub
 import warnings
 
 DEBUG = 0
@@ -84,100 +71,201 @@
     profile = ub.identity
 
 
 class AssetExtractConfig(scfg.DataConfig):
     """
     Part of the extract config for asset jobs
     """
-    keep = 'none'
-    include_channels = None
-    exclude_channels = None
-    force_nodata = None
-    tries = 2
-    asset_timeout = None
-    force_min_gsd  =  None
-    hack_lazy = False
-    verbose = 0
+    keep = scfg.Value(None, help=ub.paragraph(
+            '''
+            Level of detail to overwrite existing data at, since this is
+            slow. "none": overwrite all, including existing images
+            "img": only add new images "roi": only add new ROIs "roi-
+            img": only add new ROIs and only new images within those
+            ROIs (good for rerunning failed jobs)
+            '''))
+
+    corruption_checks = scfg.Value(False, help=ub.paragraph(
+        '''
+        Check for image cache corruption after a "cache hit" to make sure we
+        can read the image and it isn't corrupted. If it is, delete it and
+        reprocess.
+        '''))
+
+    include_channels = scfg.Value(None, help=ub.paragraph(
+            '''
+            If specified only align the given channels
+            '''))
+    exclude_channels = scfg.Value(None, help='If specified ignore these channels')
+
+    force_nodata = scfg.Value(None, help=ub.paragraph(
+            '''
+            if specified, forces nodata to this value (e.g. -9999)
+            Ideally this is not needed and all source geotiffs properly
+            specify nodata.
+
+            NOTE: We currently must specify this to handle gdal-merge
+            correctly. Perhasp in the future we may be able to introspect, but
+            for now specify it.
+            '''))
+
+    tries = scfg.Value(2, help=ub.paragraph(
+            '''
+            The maximum number of times to retry failed gdal warp
+            commands before stopping.
+            '''), alias=['warp_tries'])
+
+    cooldown = scfg.Value(10, help='seconds between tries after a failed attempt')
+
+    asset_timeout = scfg.Value('4hours', help=ub.paragraph(
+            '''
+            The maximum amount of time to spend pulling down a single
+            image asset before giving up
+            '''))
 
+    force_min_gsd = scfg.Value(None, help=ub.paragraph(
+            '''
+            Force output crops to be at least this minimum GSD (e.g. if
+            set to 10.0 an input image with a 30.0 GSD will have an
+            output GSD of 30.0, whereas in input image with a 0.5 GSD
+            will have it set to 10.0 during cropping)
+            '''))
 
-class ImageExtractConfig(scfg.DataConfig):
+    hack_lazy = scfg.Value(False, isflag=True, help=ub.paragraph(
+            '''
+            Hack lazy is a proof of concept with the intent on speeding
+            up the download / cropping of data by flattening the gdal
+            processing into a single queue of parallel processes
+            executed via a command queue. By running once with this flag
+            on, it will execute the command queue, and then running
+            again, it should see all of the data as existing and
+            construct the aligned kwcoco dataset as normal.
+            '''))
+
+    verbose = scfg.Value(0, help=ub.paragraph(
+            '''
+            Note: no silent mode, 0 is just least verbose.
+            '''))
+
+    def __post_init__(config):
+        if isinstance(config['force_min_gsd'], str):
+            if config['force_min_gsd'].lower().endswith('gsd'):
+                config['force_min_gsd'] = float(config['force_min_gsd'][:-3].strip())
+
+
+class ImageExtractConfig(AssetExtractConfig):
     """
     Part of the extract config for image jobs
     """
-    rpc_align_method = 'orthorectify'
-    aux_workers = 0
-    keep = 'none'
-    include_channels = None
-    exclude_channels = None
-    force_nodata = None
-    tries = 2
-    image_timeout = None
-    asset_timeout = None
-    force_min_gsd  =  None
-    hack_lazy = False
-    verbose = 0
-    num_start_frames = None
-    num_end_frames = None
+    # TODO: change this name to just align-method or something
+    rpc_align_method = scfg.Value('orthorectify', help=ub.paragraph(
+            '''
+            Can be one of: (1) orthorectify - which uses gdalwarp with
+            -rpc if available otherwise falls back to affine transform,
+            (2) pixel_crop - which warps annotations onto pixel with
+            RPCs but only crops the original image without distortion,
+            (3) affine_warp - which ignores RPCs and uses the affine
+            transform in the geotiff metadata.
+            '''))
 
+    aux_workers = scfg.Value(0, type=str, help='additional inner threads for aux imgs')
+
+    image_timeout = scfg.Value('8hours', help=ub.paragraph(
+            '''
+            The maximum amount of time to spend pulling down a all image
+            assets before giving up
+            '''))
 
-class ExtractConfig(scfg.DataConfig):
+    num_start_frames = scfg.Value(None, help=ub.paragraph(
+        '''
+        if specified, attempt to only gather this many high quality images at
+        the start of a sequence.
+        '''))
+
+    num_end_frames = scfg.Value(None, help=ub.paragraph(
+        '''
+        if specified, attempt to only gather this many high quality images at
+        the end of a sequence.
+        '''))
+
+
+class ExtractConfig(ImageExtractConfig):
     """
     This is a subset of the above config for arguments a passed to
     extract_overlaps. We may use this config as a base class to inherit from,
     but for now we duplicate param names.
     """
-    rpc_align_method = 'orthorectify'
-    write_subsets = True
-    visualize = True
-    img_workers = 0
-    aux_workers = 0
-    keep = 'none'
-    target_gsd = 10
-    debug_valid_regions = False
-    include_channels = None
-    exclude_channels = None
-    tries = 2
-    image_timeout = None
-    asset_timeout = None
-    force_nodata = None
-    verbose = 0
-    force_min_gsd  =  None
-    hack_lazy = False
-    max_frames = None
-    num_start_frames = None
-    num_end_frames = None
+    write_subsets = scfg.Value(True, isflag=1, help=ub.paragraph(
+            '''
+            if True, writes a separate kwcoco file for every discovered
+            ROI in addition to the final kwcoco file.
+            '''))
 
+    visualize = scfg.Value(False, isflag=1, help=ub.paragraph(
+            '''
+            if True, normalize and draw image / annotation sequences
+            when extracting.
+            '''))
 
-class CocoAlignGeotiffConfig(scfg.DataConfig):
+    img_workers = scfg.Value(0, type=str, help=ub.paragraph(
+            '''
+            number of parallel procs. This can also be an expression
+            accepted by coerce_num_workers.
+            '''), alias=['max_workers', 'workers'])
+
+    target_gsd = scfg.Value(10, help=ub.paragraph(
+            '''
+            initial **virtual** gsd to use for the output video files
+            '''))
+
+    debug_valid_regions = scfg.Value(False, isflag=1, help=ub.paragraph(
+            '''
+            write valid region visualizations to help debug "black
+            images" issues.
+            '''))
+
+    max_frames = scfg.Value(None, help=ub.paragraph(
+        '''
+        Limit the number of frames per video (mainly for debugging)
+        '''))
+
+    def __post_init__(config):
+        super().__post_init__()
+        if isinstance(config['target_gsd'], str):
+            if config['target_gsd'].lower().endswith('gsd'):
+                config['target_gsd'] = int(config['target_gsd'][:-3].strip())
+
+
+class CocoAlignGeotiffConfig(ExtractConfig):
     """
     Create a dataset of aligned temporal sequences around objects of interest
     in an unstructured collection of annotated geotiffs.
 
     High Level Steps:
         * Find a set of geospatial AOIs
         * For each AOI find all images that overlap
         * Orthorectify (or warp) the selected spatial region and its
           annotations to a cannonical space.
     """
     __command__ = 'align'
     __alias__ = ['coco_align', 'coco_align_geotiff']
 
-    src = scfg.Value('in.geojson.json', help='input dataset to chip')
+    src = scfg.Value('in.geojson.json', help='input dataset to chip', group='inputs')
     dst = scfg.Value(None, help=ub.paragraph(
             '''
             bundle directory or kwcoco json file for the output
-            '''))
+            '''), group='outputs')
 
-    img_workers = scfg.Value(0, type=str, help=ub.paragraph(
+    regions = scfg.Value('annots', help=ub.paragraph(
             '''
-            number of parallel procs. This can also be an expression
-            accepted by coerce_num_workers.
-            '''), alias=['max_workers', 'workers'])
-
-    aux_workers = scfg.Value(0, type=str, help='additional inner threads for aux imgs')
+            Strategy for extracting regions, if annots, uses the convex
+            hulls of clustered annotations. Can also be a path to a
+            geojson file to use pre-defined regions.
+            '''), group='inputs')
+    site_summary = scfg.Value(False, help='Crop to site summaries instead')
 
     context_factor = scfg.Value(1.0, help=ub.paragraph(
             '''
             Scale factor to expand each ROI by crop regions by.
             '''))
     minimum_size = scfg.Value(None, help=ub.paragraph(
             '''
@@ -187,190 +275,38 @@
             1280 meters tall and wide.
             '''))
     convexify_regions = scfg.Value(False, help=ub.paragraph(
             '''
             if True, ensure that the regions are convex
             '''))
 
-    regions = scfg.Value('annots', help=ub.paragraph(
-            '''
-            Strategy for extracting regions, if annots, uses the convex
-            hulls of clustered annotations. Can also be a path to a
-            geojson file to use pre-defined regions.
-            '''))
-    site_summary = scfg.Value(False, help='Crop to site summaries instead')
-
-    rpc_align_method = scfg.Value('orthorectify', help=ub.paragraph(
-            '''
-            Can be one of: (1) orthorectify - which uses gdalwarp with
-            -rpc if available otherwise falls back to affine transform,
-            (2) pixel_crop - which warps annotations onto pixel with
-            RPCs but only crops the original image without distortion,
-            (3) affine_warp - which ignores RPCs and uses the affine
-            transform in the geotiff metadata.
-            '''))
-    write_subsets = scfg.Value(True, isflag=1, help=ub.paragraph(
-            '''
-            if True, writes a separate kwcoco file for every discovered
-            ROI in addition to the final kwcoco file.
-            '''))
-    visualize = scfg.Value(False, isflag=1, help=ub.paragraph(
-            '''
-            if True, normalize and draw image / annotation sequences
-            when extracting.
-            '''))
-    debug_valid_regions = scfg.Value(False, isflag=1, help=ub.paragraph(
-            '''
-            write valid region visualizations to help debug "black
-            images" issues.
-            '''))
-    keep = scfg.Value(None, help=ub.paragraph(
-            '''
-            Level of detail to overwrite existing data at, since this is
-            slow. "none": overwrite all, including existing images
-            "img": only add new images "roi": only add new ROIs "roi-
-            img": only add new ROIs and only new images within those
-            ROIs (good for rerunning failed jobs)
-            '''))
-    skip_geo_preprop = scfg.Value(False, help='DEPRECATED use geo_preop instead')
     geo_preprop = scfg.Value('auto', help='force if we check geo properties or not')
 
     include_sensors = scfg.Value(None, help=ub.paragraph(
             '''
             if specified can be comma separated valid sensors
             '''))
     exclude_sensors = scfg.Value(None, help=ub.paragraph(
             '''
             if specified can be comma separated invalid sensors
             '''))
-    include_channels = scfg.Value(None, help=ub.paragraph(
-            '''
-            If specified only align the given channels
-            '''))
-    exclude_channels = scfg.Value(None, help='If specified ignore these channels')
 
-    target_gsd = scfg.Value(10, help=ub.paragraph(
-            '''
-            initial **virtual** gsd to use for the output video files
-            '''))
     edit_geotiff_metadata = scfg.Value(False, help=ub.paragraph(
             '''
             if True MODIFIES THE UNDERLYING IMAGES to ensure geodata is
             propogated
             '''))
-    max_frames = scfg.Value(None, help=None)
-    warp_tries = scfg.Value(2, help=ub.paragraph(
-            '''
-            The maximum number of times to retry failed gdal warp
-            commands before stopping.
-            '''))
-
-    # TODO: change this name to just align-method or something
-    image_timeout = scfg.Value('8hours', help=ub.paragraph(
-            '''
-            The maximum amount of time to spend pulling down a all image
-            assets before giving up
-            '''))
-    asset_timeout = scfg.Value('4hours', help=ub.paragraph(
-            '''
-            The maximum amount of time to spend pulling down a single
-            image asset before giving up
-            '''))
-
-    verbose = scfg.Value(0, help=ub.paragraph(
-            '''
-            Note: no silent mode, 0 is just least verbose.
-            '''))
-
-    force_nodata = scfg.Value(None, help=ub.paragraph(
-            '''
-            if specified, forces nodata to this value (e.g. -9999)
-            Ideally this is not needed and all source geotiffs properly
-            specify nodata
-            '''))
-
-    force_min_gsd = scfg.Value(None, help=ub.paragraph(
-            '''
-            Force output crops to be at least this minimum GSD (e.g. if
-            set to 10.0 an input image with a 30.0 GSD will have an
-            output GSD of 30.0, whereas in input image with a 0.5 GSD
-            will have it set to 10.0 during cropping)
-            '''))
-
-    hack_lazy = scfg.Value(False, isflag=True, help=ub.paragraph(
-            '''
-            Hack lazy is a proof of concept with the intent on speeding
-            up the download / cropping of data by flattening the gdal
-            processing into a single queue of parallel processes
-            executed via a command queue. By running once with this flag
-            on, it will execute the command queue, and then running
-            again, it should see all of the data as existing and
-            construct the aligned kwcoco dataset as normal.
-            '''))
-
-    num_start_frames = scfg.Value(None, help=ub.paragraph(
-        '''
-        if specified, attempt to only gather this many high quality images at
-        the start of a sequence.
-        '''))
-
-    num_end_frames = scfg.Value(None, help=ub.paragraph(
-        '''
-        if specified, attempt to only gather this many high quality images at
-        the end of a sequence.
-        '''))
-
-    def __post_init__(config):
-        if isinstance(config['target_gsd'], str):
-            if config['target_gsd'].lower().endswith('gsd'):
-                config['target_gsd'] = int(config['target_gsd'][:-3].strip())
-
-        if isinstance(config['force_min_gsd'], str):
-            if config['force_min_gsd'].lower().endswith('gsd'):
-                config['force_min_gsd'] = float(config['force_min_gsd'][:-3].strip())
 
 
 @profile
 def main(cmdline=True, **kw):
     """
     Main function for coco_align.
     See :class:``CocoAlignGeotiffConfig` for details
 
-    Ignore:
-        from watch.cli.coco_align import *  # NOQA
-        import kwcoco
-        cmdline = False
-        src = ub.expandpath('~/data/dvc-repos/smart_watch_dvc/drop1/data.kwcoco.json')
-        dst = ub.expandpath('~/data/dvc-repos/smart_watch_dvc/Drop1-Aligned-L1/_test/test.kwcoco.json')
-        regions = ub.expandpath('~/data/dvc-repos/smart_watch_dvc/drop1/region_models/LT_R001.geojson')
-        regions = ub.expandpath('~/data/dvc-repos/smart_watch_dvc/drop1/all_regions.geojson')
-        kw = {
-            'src': src,
-            'dst': dst,
-            'regions': regions,
-            'keep': 'none',
-            'exclude_sensors': ['WV'],
-        }
-
-    Ignore:
-        from watch.cli.coco_align import *  # NOQA
-        import watch
-        dvc_dpath = watch.find_smart_dvc_dpath(hardware='hdd')
-        base_fpath = dvc_dpath / 'Aligned-Drop3-TA1-2022-03-10/data.kwcoco.json'
-        src = base_fpath
-        dst = dvc_dpath / 'Cropped-Drop3-TA1-2022-03-10/data.kwcoco.json'
-        sites = dvc_dpath / 'annotations/site_models/*.geojson'
-        cmdline = 0
-        kw = {
-            'src': src,
-            'dst': dst,
-            'regions': sites,
-            'keep': 'none',
-        }
-
     CommandLine:
         xdoctest -m watch.cli.coco_align main:0
 
     Example:
         >>> from watch.cli.coco_align import *  # NOQA
         >>> from watch.demo.landsat_demodata import grab_landsat_product
         >>> from watch.gis.geotiff import geotiff_metadata
@@ -394,17 +330,17 @@
         >>> # information like segmentation and bad bbox, but for this
         >>> # test config it is
         >>> coco_dset.add_annotation(
         >>>     image_id=gid, bbox=[0, 0, 0, 0], segmentation_geos=sseg_geos)
         >>> #
         >>> # Create arguments to the script
         >>> dpath = ub.Path.appdir('watch/test/coco_align').ensuredir()
-        >>> dst = ub.ensuredir((dpath, 'align_bundle1'))
-        >>> ub.delete(dst)
-        >>> dst = ub.ensuredir(dst)
+        >>> dst = (dpath / 'align_bundle1').ensuredir()
+        >>> dst.delete()
+        >>> dst.ensuredir()
         >>> kw = {
         >>>     'src': coco_dset,
         >>>     'dst': dst,
         >>>     'regions': 'annots',
         >>>     'workers': 2,
         >>>     'aux_workers': 2,
         >>>     'convexify_regions': True,
@@ -468,31 +404,32 @@
         >>> asset = coco_img.primary_asset()
         >>> parent_fpath = asset['parent_file_name']
         >>> crop_fpath = ub.Path(new_dset.bundle_dpath) / asset['file_name']
         >>> info = geotiff_crs_info(crop_fpath)
         >>> assert(all(info['meter_per_pxl'] == 60.0))
 
     Example:
-        >>> # xdoctest: +REQUIRES(--slow)
+        >>> # xdoctest: +REQUIRES(env:SLOW_DOCTEST)
         >>> from watch.cli.coco_align import *  # NOQA
         >>> from watch.demo.smart_kwcoco_demodata import demo_kwcoco_with_heatmaps
+        >>> from watch.utils import util_gdal
         >>> import kwimage
+        >>> import geojson
+        >>> import json
         >>> coco_dset = demo_kwcoco_with_heatmaps(num_videos=2, num_frames=2)
         >>> dpath = ub.Path.appdir('watch/test/coco_align2').ensuredir()
         >>> dst = (dpath / 'align_bundle2').delete().ensuredir()
         >>> # Create a dummy region file to crop to.
         >>> first_img = coco_dset.images().take([0]).coco_images[0]
-        >>> from osgeo import gdal
         >>> first_fpath = first_img.primary_image_filepath()
-        >>> geo_poly = kwimage.Polygon.coerce(gdal.Info(first_fpath, format='json')['wgs84Extent'])
+        >>> ds = util_gdal.GdalDataset.open(first_fpath)
+        >>> geo_poly = kwimage.Polygon.coerce(ds.info()['wgs84Extent'])
         >>> region_shape = kwimage.Polygon.random(n=8, convex=False, rng=3)
         >>> geo_transform = kwimage.Affine.fit(region_shape.bounding_box().corners(), geo_poly.bounding_box().corners())
         >>> region_poly = region_shape.warp(geo_transform)
-        >>> import geojson
-        >>> import json
         >>> region_feature = geojson.Feature(
         >>>     properties={
         >>>         "type": "region",
         >>>         "region_id": "DUMMY_R042",
         >>>         "start_date": '1970-01-01',
         >>>         "end_date":  '2970-01-01',
         >>>     },
@@ -542,17 +479,15 @@
     rich.print(ub.urepr(config))
 
     from kwcoco.util.util_json import ensure_json_serializable
     from watch.utils import util_gis
     from watch.utils import util_parallel
     from watch.utils import util_resolution
     from watch.utils import kwcoco_extensions
-    import os
     import kwcoco
-    # import socket
     import pandas as pd
     import warnings
     import kwimage
 
     # Store that this dataset is a result of a process.
     # Note what the process is, what its arguments are, and where the process
     # was executed.
@@ -564,25 +499,14 @@
 
     config_dict = ensure_json_serializable(config_dict)
 
     if os.environ.get('GDAL_DISABLE_READDIR_ON_OPEN') != 'EMPTY_DIR':
         warnings.warn('environ GDAL_DISABLE_READDIR_ON_OPEN should probably be set to EMPTY_DIR')
         os.environ['GDAL_DISABLE_READDIR_ON_OPEN'] = 'EMPTY_DIR'
 
-    # TODO: use ProcessContext instead
-    # process_info = {
-    #     'type': 'process',
-    #     'properties': {
-    #         'name': 'coco_align',
-    #         'args': config_dict,
-    #         'hostname': socket.gethostname(),
-    #         'cwd': os.getcwd(),
-    #         'timestamp': ub.timestamp(),
-    #     }
-    # }
     from watch.utils import process_context
     proc_context = process_context.ProcessContext(
         name='coco_align',
         type='process',
         config=config_dict,
     )
     proc_context.start()
@@ -628,14 +552,17 @@
                 if 'site' in type_to_subdf:
                     # This is a site model
                     df = type_to_subdf['site']
                 elif 'region' in type_to_subdf:
                     # This is a region model
                     df = type_to_subdf['region']
             parts.append(df)
+
+        if not len(parts):
+            raise ValueError('No regions to crop to were found')
         region_df = pd.concat(parts)
         print(f'Loaded {len(region_df)} regions to crop')
 
     # Load the dataset and extract geotiff metadata from each image.
     coco_dset = kwcoco.CocoDataset.coerce(config.src)
     valid_gids = kwcoco_extensions.filter_image_ids(
         coco_dset,
@@ -643,17 +570,14 @@
         exclude_sensors=config['exclude_sensors'],
     )
 
     if proc_context is not None:
         proc_context.add_disk_info(coco_dset.fpath)
 
     geo_preprop = config['geo_preprop']
-    if config['skip_geo_preprop']:
-        warnings.warn('skip_geo_preprop is deprecated', DeprecationWarning)
-        geo_preprop = False
     if geo_preprop == 'auto':
         if len(valid_gids):
             coco_img = coco_dset.coco_image(ub.peek(valid_gids))
             geo_preprop = not any('geos_corners' in obj for obj in coco_img.iter_asset_objs())
             print('auto-choose geo_preprop = {!r}'.format(geo_preprop))
 
     if geo_preprop:
@@ -683,15 +607,14 @@
     print('cube.img_geos_df =\n{}'.format(cube.img_geos_df))
 
     if config['convexify_regions']:
         # Exapnd the ROI by the context factor
         region_df['geometry'] = region_df['geometry'].convex_hull
 
     # Convert the ROI to a bounding box
-    # region_df['geometry'] = region_df['geometry'].apply(shapely_bounding_box)
     context_factor = config['context_factor']
     if context_factor != 1:
         # Exapnd the ROI by the context factor
         region_df['geometry'] = region_df['geometry'].scale(
             xfact=context_factor, yfact=context_factor, origin='center')
 
     minimum_size = config['minimum_size']
@@ -728,32 +651,31 @@
     ]
     to_extract = cube.query_image_overlaps(region_df)
 
     if config['hack_lazy']:
         lazy_commands = []
 
     extract_kwargs = ub.udict(config) & ExtractConfig.__default__.keys()
-    extract_kwargs['tries'] = config['warp_tries']
+    extract_config = ExtractConfig(**extract_kwargs)
 
     for image_overlaps in ub.ProgIter(to_extract, desc='extract ROI videos', verbose=3):
         video_name = image_overlaps['video_name']
         print('video_name = {!r}'.format(video_name))
 
         sub_bundle_dpath = ub.Path(extract_dpath) / video_name
         print('sub_bundle_dpath = {!r}'.format(sub_bundle_dpath))
 
-        extract_kwargs = ExtractConfig(**extract_kwargs)
         new_dset = cube.extract_overlaps(
-            image_overlaps, extract_dpath, new_dset=new_dset, **extract_kwargs
+            image_overlaps, extract_dpath, new_dset=new_dset,
+            extract_config=extract_config,
         )
         if config['hack_lazy']:
             lazy_commands.extend(new_dset)
 
     if config['hack_lazy']:
-
         # Execute the gdal jobs in a single super queue
         import cmd_queue
         # queue = cmd_queue.Queue.create('serial')
         queue = cmd_queue.Queue.create(
             'tmux', size=config.img_workers, name='hack_lazy_' + video_name,
             environ={
                 k: v for k, v in os.environ.items()
@@ -764,20 +686,22 @@
         )
         for commands in lazy_commands:
             prev = None
             for command in commands:
                 prev = queue.submit(command, depends=prev)
                 prev.logs = False
 
-        print(f'{len(queue.jobs)=}')
-        queue.run(
-            # with_textual=False
-            with_textual='auto'
-        )
+        queue.print_commands()
 
+        print(f'{len(queue.jobs)=}')
+        if config['hack_lazy'] != 'dry':
+            queue.run(
+                # with_textual=False
+                with_textual='auto'
+            )
         raise Exception('hack_lazy always fails')
 
     kwcoco_extensions.reorder_video_frames(new_dset)
 
     proc_context.stop()
 
     new_dset.fpath = dst_fpath
@@ -793,15 +717,15 @@
         rerooted_dataset.reroot(new_root=output_bundle_dpath, absolute=False)
 
     rerooted_dataset.dump(rerooted_dataset.fpath, newlines=True)
     print('finished')
     return rerooted_dataset
 
 
-class SimpleDataCube(object):
+class SimpleDataCube:
     """
     Given a CocoDataset containing geotiffs, provide a simple API to extract a
     region in some coordinate space.
 
     Intended usage is to use :func:`query_image_overlaps` to find images that
     overlap an ROI, then then :func:`extract_overlaps` to warp spatial subsets
     of that data into an aligned temporal sequence.
@@ -1140,15 +1064,15 @@
                         'sub_bundle_dname': sub_bundle_dname,
                     }
                     to_extract.append(image_overlaps)
         return to_extract
 
     @profile
     def extract_overlaps(cube, image_overlaps, extract_dpath, new_dset=None,
-                         **extract_kwargs):
+                         extract_config=None):
         """
         Given a region of interest, extract an aligned temporal sequence
         of data to a specified directory.
 
         Args:
             image_overlaps (dict): Information about images in an ROI and their
                 temporal order computed from :func:``query_image_overlaps``.
@@ -1156,62 +1080,59 @@
             extract_dpath (str):
                 where to dump the data extracted from this ROI.
 
             new_dset (kwcoco.CocoDataset | None):
                 if specified, add extracted images and annotations to this
                 dataset, otherwise create a new dataset.
 
-            **kwargs:
-                see the config
+            extract_config (ExtractConfig):
+                configuration for how to perform the extract task.
 
         Returns:
             kwcoco.CocoDataset: the given or new dataset that was modified
 
         Example:
-            >>> # xdoctest: +REQUIRES(--slow)
+            >>> # xdoctest: +REQUIRES(env:SLOW_DOCTEST)
             >>> from watch.cli.coco_align import *  # NOQA
+            >>> import kwcoco
             >>> cube, region_df = SimpleDataCube.demo(with_region=True)
             >>> extract_dpath = ub.Path.appdir('watch/test/coco_align/demo_extract_overlaps').ensuredir()
             >>> rpc_align_method = 'orthorectify'
             >>> new_dset = kwcoco.CocoDataset()
-            >>> visualize = True
-            >>> img_workers = 32
             >>> to_extract = cube.query_image_overlaps(region_df)
             >>> image_overlaps = to_extract[0]
+            >>> extract_config = ExtractConfig(img_workers=32, visualize=True)
             >>> cube.extract_overlaps(image_overlaps, extract_dpath,
-            >>>                       new_dset=new_dset, visualize=visualize,
-            >>>                       img_workers=img_workers)
+            >>>                       new_dset=new_dset, extract_config=extract_config)
 
         Example:
-            >>> # xdoctest: +REQUIRES(--slow)
+            >>> # xdoctest: +REQUIRES(env:SLOW_DOCTEST)
             >>> from watch.cli.coco_align import *  # NOQA
+            >>> import kwcoco
             >>> cube, region_df = SimpleDataCube.demo(with_region=True, extra=True)
             >>> extract_dpath = ub.Path.appdir('watch/test/coco_align/demo_extract_overlaps2').ensuredir()
             >>> rpc_align_method = 'orthorectify'
-            >>> visualize = True
-            >>> img_workers = 0
             >>> to_extract = cube.query_image_overlaps(region_df)
             >>> new_dset = kwcoco.CocoDataset()
             >>> image_overlaps = to_extract[1]
+            >>> extract_config = ExtractConfig(img_workers=0, visualize=True)
             >>> cube.extract_overlaps(image_overlaps, extract_dpath,
-            >>>                       new_dset=new_dset, visualize=visualize,
-            >>>                       img_workers=img_workers)
-
-            xdev.profile_now(SimpleDataCube.demo)
+            >>>                       new_dset=new_dset,
+            >>>                       extract_config=extract_config)
         """
         from kwcoco.util.util_json import ensure_json_serializable
         import geopandas as gpd
         from watch.utils import util_time
         from watch.utils import util_gis
         from watch.utils import kwcoco_extensions
         import kwcoco
         import kwimage
         import pandas as pd
         coco_dset = cube.coco_dset
-        extract_config = ExtractConfig(**extract_kwargs)
+        assert extract_config is not None
 
         datetime_to_gids = image_overlaps['datetime_to_gids']
         space_str = image_overlaps['space_str']
         space_box = image_overlaps['space_box']
         space_region = image_overlaps['space_region']
         video_name = image_overlaps['video_name']
         video_props = image_overlaps['properties']
@@ -1410,15 +1331,15 @@
                     space_str=space_str,
                     space_region=space_region,
                     space_box=space_box,
                     start_gid=start_gid,
                     start_aid=start_aid,
                     local_epsg=local_epsg,
                     other_imgs=other_imgs,
-                    **img_config)
+                    img_config=img_config)
                 job.request_idx = request_idx
                 start_gid = start_gid + 1
                 start_aid = start_aid + len(anns)
                 frame_index = frame_index + 1
 
         # return
 
@@ -1427,17 +1348,15 @@
         if extract_config.image_timeout is not None:
             image_timeout = util_time.coerce_timedelta(extract_config.image_timeout).total_seconds()
 
         if extract_config.hack_lazy:
             lazy_commands = []
 
         from concurrent.futures import TimeoutError
-        for job in image_jobs.as_completed(desc='collect extract jobs',
-                                           progkw=dict(freq=1)):
-
+        for job in image_jobs.as_completed(desc='collect extract jobs', progkw={'clearline': False}):
             try:
                 new_img, new_anns = job.result(timeout=image_timeout)
             except SkipImage:
                 # TODO: if we are only requesting a subset of images we may
                 # want to submit a new image job to take the place of this
                 # failed image.
                 unrequested_datetimes
@@ -1575,22 +1494,23 @@
 
 
 def _handle_multiple_images_per_date(coco_dset, gids, local_epsg,
                                      sh_space_region_local, extract_config,
                                      prog, cube, space_region_crs84,
                                      extract_dpath, video_name, iso_time,
                                      space_str, space_region_local):
+    """
+    We got multiple images for the same timestamp.  Im not sure if this is
+    necessary but thig logic attempts to sort them such that the "best" image
+    to use is first.  Ideally gdalwarp would take care of this but I'm not sure
+    it does.
+    """
     import geopandas as gpd
-    import pandas as pd  # NOQA
     from shapely import geometry
     from watch.utils import util_gis
-    # We got multiple images for the same timestamp.  Im not sure
-    # if this is necessary but thig logic attempts to sort them
-    # such that the "best" image to use is first.  Ideally gdalwarp
-    # would take care of this but I'm not sure it does.
     conflict_imges = coco_dset.images(gids)
     sensors = list(conflict_imges.lookup('sensor_coarse', None))
 
     groups = []
 
     for sensor_coarse, sensor_gids in ub.group_items(conflict_imges, sensors).items():
         rows = []
@@ -1683,15 +1603,15 @@
                       space_str,
                       space_region,
                       space_box,
                       start_gid,
                       start_aid,
                       local_epsg=None,
                       other_imgs=None,
-                      **kwargs):
+                      img_config=None):
     """
     Threaded worker function for :func:`SimpleDataCube.extract_overlaps`.
 
     Returns:
         Tuple[Dict, Dict] : new_img, new_anns
     """
     # from tempenv import TemporaryEnvironment  # NOQA
@@ -1711,18 +1631,15 @@
     from watch.utils import kwcoco_extensions
     from watch.utils import util_time
     from osgeo import osr
     import kwimage
     osr.GetPROJSearchPaths()
     from kwcoco.coco_image import CocoImage
 
-    img_config = ImageExtractConfig(**kwargs)
-
-    rpc_align_method = img_config.rpc_align_method
-    verbose = img_config.verbose
+    assert img_config is not None
 
     if img_config.image_timeout is not None:
         img_config.image_timeout = util_time.coerce_timedelta(img_config.image_timeout).total_seconds()
     if img_config.asset_timeout is not None:
         img_config.asset_timeout = util_time.coerce_timedelta(img_config.asset_timeout).total_seconds()
 
     coco_img = CocoImage(img)
@@ -1765,40 +1682,41 @@
         else:
             if 'geotiff_metadata' not in obj:
                 kwcoco_extensions._populate_canvas_obj(bundle_dpath, obj,
                                                        keep_geotiff_metadata=True)
             if obj['geotiff_metadata']['is_rpc']:
                 is_rpc = True
 
-    if is_rpc and rpc_align_method != 'affine_warp':
-        align_method = rpc_align_method
+    if is_rpc and img_config.rpc_align_method != 'affine_warp':
+        align_method = img_config.rpc_align_method
     else:
         align_method = 'affine_warp'
 
     dst_dpath = ub.ensuredir((sub_bundle_dpath, sensor_coarse, align_method))
 
     job_list = []
 
     # Turn off internal threading because we refactored this to thread over all
     # images instead
     asset_jobs = ub.JobPool(mode='thread', max_workers=img_config.aux_workers)
 
+    verbose = img_config.verbose
     aux_verbose = (verbose > 3) or (verbose > 1 and (img_config.aux_workers == 0))
     asset_config = AssetExtractConfig(
         **(ub.udict(img_config) & set(AssetExtractConfig.__default__.keys()))
     )
     asset_config['verbose'] = aux_verbose
 
     for obj_group in ub.ProgIter(obj_groups, desc='submit warp assets', verbose=verbose):
         job = asset_jobs.submit(
             _aligncrop, obj_group, bundle_dpath, name, sensor_coarse,
             dst_dpath, space_region, space_box, align_method,
             is_multi_image,
             local_epsg=local_epsg,
-            **asset_config,
+            asset_config=asset_config,
         )
         job_list.append(job)
 
     dst_list = []
     for job in asset_jobs.as_completed(desc='collect warp assets {}'.format(name),
                                        timeout=img_config.image_timeout,
                                        progkw=dict(enabled=DEBUG, verbose=verbose)):
@@ -1972,19 +1890,14 @@
         new_anns.append(ann)
 
     if DEBUG:
         print(f'Finished extract img job: {new_gid}')
     return new_img, new_anns
 
 
-def shapely_bounding_box(geom):
-    import shapely
-    return shapely.geometry.box(*geom.bounds)
-
-
 def _fix_geojson_poly(geo):
     """
     We were given geojson polygons with one fewer layers of nesting than
     the spec allows for. Fix this.
 
     Example:
         >>> import kwimage
@@ -2031,20 +1944,22 @@
                sensor_coarse,
                dst_dpath,
                space_region,
                space_box,
                align_method,
                is_multi_image,
                local_epsg=None,
-               **kwargs):
+               asset_config=None):
     import watch
     import kwcoco
     from watch.utils import util_gdal
+    from os.path import join
 
-    asset_config = AssetExtractConfig(**kwargs)
+    assert asset_config is not None
+    # asset_config = AssetExtractConfig(**kwargs)
     verbose = asset_config.verbose
 
     # NOTE: https://github.com/dwtkns/gdal-cheat-sheet
     first_obj = obj_group[0]
     chan_code = obj_group[0].get('channels', '')
 
     # Prevent long names for docker (limit is 242 chars)
@@ -2071,45 +1986,46 @@
         multi_dpath = ub.ensuredir((dst_dpath, name))
         dst_gpath = ub.Path(multi_dpath) / (name + '_' + chan_pname + '.tif')
     else:
         dst_gpath = ub.Path(dst_dpath) / (name + '.tif')
 
     input_gnames = [obj.get('file_name', None) for obj in obj_group]
     assert all(n is not None for n in input_gnames)
-    input_gpaths = [str(ub.Path(bundle_dpath) / n) for n in input_gnames]
+
+    # Must use join over pathlib because Path strips http:// to http:/
+    input_gpaths = [join(bundle_dpath, n) for n in input_gnames]
 
     dst = {
         'file_name': os.fspath(dst_gpath),
     }
     if first_obj.get('channels', None):
         dst['channels'] = first_obj['channels']
     if first_obj.get('num_bands', None):
         dst['num_bands'] = first_obj['num_bands']
 
     already_exists = dst_gpath.exists()
     needs_recompute = not (already_exists and asset_config.keep in {'img', 'roi-img'})
 
     if not needs_recompute:
-        DOUBLE_CHECK = 1
-        if DOUBLE_CHECK:
+        if asset_config.corruption_checks:
             # Sometimes the data will exist, but it's bad data. Check for this.
             try:
-                ref = util_gdal.GdalOpen(dst_gpath, mode='r')
+                ref = util_gdal.GdalDataset.open(dst_gpath, mode='r')
                 ref
             except RuntimeError:
                 # Data is likely corrupted
                 needs_recompute = True
                 print(f'The data exists {dst_gpath}, but is corrupted. Recomputing')
                 dst_gpath.delete()
                 pass
             else:
                 ref = None
 
     if not needs_recompute:
-        if verbose:
+        if verbose > 2:
             print('cache hit dst = {!r}'.format(dst))
         return dst
 
     if align_method == 'pixel_crop':
         raise NotImplementedError('no longer supported')
 
     if align_method == 'orthorectify':
@@ -2146,17 +2062,14 @@
             '\n* dst_gpath = {!r}'.format(dst_gpath))
 
     error_logfile = None
     # Uncomment to suppress warnings for debug purposes
     #
     # error_logfile = '/dev/null'
 
-    # TODO: add a timeout argument to the gdal calls and pass down the asset
-    # timeout.
-
     # Note: these methods take care of retries and checking that the
     # data is valid.
     force_spatial_res = None
     if asset_config.force_min_gsd is not None:
         if 'approx_meter_gsd' in first_obj:
             approx_meter_gsd = first_obj['approx_meter_gsd']
         else:
@@ -2180,37 +2093,38 @@
 
         if approx_meter_gsd is not None and approx_meter_gsd < asset_config.force_min_gsd:
             # Only setting if needed to avoid needless warping if the
             # 'approximate_meter_gsd' value is slightly different from
             # what GDAL computes at the time of warping
             force_spatial_res = asset_config.force_min_gsd
 
+    cooldown = asset_config.cooldown
+    gdal_verbose = 0 if verbose < 2 else verbose
+
+    gdalkw = dict(
+        space_box=space_box,
+        local_epsg=local_epsg,
+        rpcs=rpcs, nodata=nodata,
+        tries=asset_config.tries,
+        cooldown=cooldown,
+        error_logfile=error_logfile,
+        verbose=gdal_verbose,
+        force_spatial_res=force_spatial_res,
+        eager=not asset_config.hack_lazy,
+        warp_memory='1500',
+        gdal_cachemax='1500',
+        num_threads='2',
+    )
+
     if len(input_gpaths) > 1:
         in_fpaths = input_gpaths
-        commands = util_gdal.gdal_multi_warp(
-            in_fpaths, out_fpath, space_box=space_box,
-            local_epsg=local_epsg, rpcs=rpcs,
-            nodata=nodata, tries=asset_config.tries,
-            error_logfile=error_logfile,
-            verbose=0 if verbose < 2 else verbose,
-            force_spatial_res=force_spatial_res,
-            eager=not asset_config.hack_lazy,
-        )
+        commands = util_gdal.gdal_multi_warp(in_fpaths, out_fpath, **gdalkw)
     else:
         in_fpath = input_gpaths[0]
-        commands = util_gdal.gdal_single_warp(
-            in_fpath, out_fpath,
-            space_box=space_box, local_epsg=local_epsg,
-            rpcs=rpcs, nodata=nodata,
-            tries=asset_config.tries,
-            error_logfile=error_logfile,
-            verbose=0 if verbose < 2 else verbose,
-            force_spatial_res=force_spatial_res,
-            eager=not asset_config.hack_lazy,
-        )
+        commands = util_gdal.gdal_single_warp(in_fpath, out_fpath, **gdalkw)
     if asset_config.hack_lazy:
         # The lazy hack means we are just building the commands
         dst['commands'] = commands
     if verbose > 2:
         print('finish gdal warp dst_gpath = {!r}'.format(dst_gpath))
     return dst
 
@@ -2316,15 +2230,14 @@
 
 
 class SkipImage(Exception):
     ...
 
 
 __config__ = CocoAlignGeotiffConfig
-__config__ = CocoAlignGeotiffConfig
 
 
 if __name__ == '__main__':
     """
     CommandLine:
         python -m watch.cli.coco_align --help
     """
```

### Comparing `geowatch-0.6.3/watch/cli/coco_average_features.py` & `geowatch-0.6.6/watch/cli/coco_average_features.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/coco_clean_geotiffs.py` & `geowatch-0.6.6/watch/cli/coco_clean_geotiffs.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,68 +14,69 @@
         inplace. Make a copy of your dataset if there is any chance you need to
         go back. The underlying kwcoco file is not modified.
 
     Usage:
         # It is a good idea to do a dry run first to check for issues
         # This can be done at a smaller scale for speed.
         DVC_DATA_DPATH=$(geowatch_dvc --tags='phase2_data' --hardware=auto)
-        smartwatch clean_geotiffs \
+        geowatch clean_geotiffs \
             --src "$DVC_DATA_DPATH/Drop4-BAS/data.kwcoco.json" \
             --channels="red|green|blue|nir|swir16|swir22" \
             --prefilter_channels="red" \
             --min_region_size=256 \
             --nodata_value=-9999 \
             --workers="min(2,avail)" \
             --probe_scale=0.5 \
             --dry=True
 
         # Then execute a real run at full scale - optionally with a probe scale
-        smartwatch clean_geotiffs \
+        geowatch clean_geotiffs \
             --src "$DVC_DATA_DPATH/Drop4-BAS/data_vali.kwcoco.json" \
             --channels="red|green|blue|nir|swir16|swir22" \
             --prefilter_channels="red" \
             --min_region_size=256 \
             --nodata_value=-9999 \
             --workers="min(2,avail)" \
             --probe_scale=None \
             --dry=False
 
 
     Ignore:
 
-        smartwatch clean_geotiffs \
+        geowatch clean_geotiffs \
             --src=data.kwcoco.zip --dry=True --workers=8  \
             --probe_scale=0.25 --prefilter_channels=pan --channels=pan
 
-        smartwatch clean_geotiffs \
+        geowatch clean_geotiffs \
             --dry=False --workers=2  \
             --probe_scale=0.0625 --prefilter_channels="pan" \
             --channels="pan" \
             --src=data.kwcoco.zip
 
-        smartwatch clean_geotiffs \
+        geowatch clean_geotiffs \
             --dry=False --workers=avail  \
             --probe_scale=0.0625 --prefilter_channels="red" \
             --channels="red|green|blue|nir|swir16|swir22" \
             --src=data.kwcoco.zip
 
-        smartwatch clean_geotiffs \
+        geowatch clean_geotiffs \
             --dry=False --workers=avail  \
             --probe_scale=0.25 --prefilter_channels="swir22" \
             --channels="swir16|swir22" \
             --src=imgonly-BR_R005.kwcoco.json
 
     """
     src = scfg.Value(None, position=1, help='input coco dataset')
 
     workers = scfg.Value(0, type=str, help='number of workers')
 
-    channels = scfg.Value('red|green|blue|nir|swir16|swir22', help=ub.paragraph(
+    channels = scfg.Value('*', help=ub.paragraph(
         '''
-        The channels to apply nodata fixes to.
+        The channels to apply nodata fixes to. A value of * means all channels
+        except the excluded ones.
         '''))
 
     exclude_channels = scfg.Value('quality|cloudmask', help=ub.paragraph(
         '''
         Channels to never apply fixes to.
         '''))
 
@@ -119,14 +120,16 @@
 
     use_fix_stamps = scfg.Value(False, help=ub.paragraph(
         '''
         if True, write a file next to every file that was fixed so we dont need
         to check it again.
         '''))
 
+    export_bad_fpath = scfg.Value(None, help='if True, export paths to bad files to this newline separated file, also works in dry mode')
+
     dry = scfg.Value(False, help='if True, only do a dry run. Report issues but do not fix them')
 
 
 __config__ = CleanGeotiffConfig
 
 
 def main(cmdline=1, **kwargs):
@@ -180,15 +183,15 @@
         >>> kwplot.autompl()
         >>> kwplot.imshow(canvas1, pnum=(1, 2, 1), title='before')
         >>> kwplot.imshow(canvas2, pnum=(1, 2, 2), title='after')
     """
     from watch.utils import util_parallel
     import kwcoco
 
-    config = CleanGeotiffConfig.cli(cmdline=cmdline, data=kwargs)
+    config = CleanGeotiffConfig.cli(cmdline=cmdline, data=kwargs, strict=True)
     import rich
     rich.print('config = {}'.format(ub.urepr(config, nl=1)))
 
     print('Loading dataset')
     coco_dset = kwcoco.CocoDataset.coerce(config['src'])
 
     workers = util_parallel.coerce_num_workers(config['workers'])
@@ -222,14 +225,22 @@
         'nodata_value': config['nodata_value'],
     }
 
     print('Grabbing coco images')
     coco_imgs = coco_dset.images().coco_images
     print('About to start looping')
 
+    if config.export_bad_fpath is not None:
+        export_fpath = ub.Path(config.export_bad_fpath)
+        with open(export_fpath, 'w'):
+            ...
+        export_file = open(export_fpath, 'a')
+    else:
+        export_file = None
+
     from watch.utils import util_progress
     mprog = util_progress.ProgressManager(backend='progiter')
     # mprog = util_progress.ProgressManager(backend='rich')
     with mprog, jobs:
         print('In the with statement')
         mprog.update_info('Looking for geotiff issues')
 
@@ -298,14 +309,16 @@
             needs_fix = list(needs_fix)
         else:
             needs_fix = iter(needs_fix)
 
         if not config['dry']:
             correct_nodata_value = config['nodata_value']
             for asset_summary in mprog.new(needs_fix, desc='Cleaning identified issues'):
+                if export_file is not None:
+                    export_file.write(asset_summary['fpath'] + '\n')
                 fpath = ub.Path(asset_summary['fpath'])
                 fix_geotiff_ondisk(asset_summary,
                                    correct_nodata_value=correct_nodata_value)
                 if config['use_fix_stamps']:
                     # Mark that fixes have been applied to this asset
                     import json
                     fix_fpath = fpath.augment(tail='.fixes.stamp')
@@ -314,17 +327,22 @@
                     else:
                         fixes = []
                     new_fixes = ub.udict(asset_summary) & {'band_idxs'}
                     fixes.append(new_fixes)
                     fix_fpath.write_text(json.dumps(fixes))
         else:
             for asset_summary in mprog.new(needs_fix, desc='Dry run: identifying issues'):
+                if export_file is not None:
+                    export_file.write(asset_summary['fpath'] + '\n')
                 print(asset_summary['fpath'])
                 ...
 
+    if export_file is not None:
+        export_file.close()
+
     # if 0:
     #     import xdev
     #     import kwplot
     #     kwplot.autompl()
 
     #     nonzero_chans = []
     #     for image_summary in has_nonzeros:
@@ -352,15 +370,17 @@
     multiple bands for fixable nodata values.
 
     Args:
         coco_img : the coco image to check
 
         channels : the channels to check
 
-        prefilter_channels : the channels to check first for efficiency
+        prefilter_channels :
+            the channels to check first for efficiency. If they do not exist,
+            then the all channels are checked.
 
         possible_nodata_values (set[int]):
             the values that may be nodata if known
 
         scale :
             use a downscaled overview to speed up the computation via
             approximation. Returns results at this scale. DO NOT USE RIGHT NOW.
```

### Comparing `geowatch-0.6.3/watch/cli/coco_combine_features.py` & `geowatch-0.6.6/watch/cli/coco_combine_features.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/coco_crop_tracks.py` & `geowatch-0.6.6/watch/cli/coco_crop_tracks.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,17 @@
 
 
     TODO:
         - [ ] option to merge overlapping regions?
 """
 import scriptconfig as scfg
 import ubelt as ub
-# import xdev
 
 
-class CocoCropTrackConfig(scfg.Config):
+class CocoCropTrackConfig(scfg.DataConfig):
     """
     Create a dataset of aligned temporal sequences around objects of interest
     in an unstructured collection of annotated geotiffs.
 
     High Level Steps:
         * Find a set of geospatial AOIs
         * For each AOI find all images that overlap
@@ -104,16 +103,16 @@
         dst = dvc_dpath / 'Cropped-Drop2-TA1-2022-02-15/data.kwcoco.json'
         cmdline = 0
         include_sensors = ['WV']
         kwargs = dict(src=src, dst=dst, include_sensors=include_sensors)
         kwargs['workers'] = 8
     """
     import kwcoco
-    config = CocoCropTrackConfig(cmdline=cmdline, data=kwargs)
-    print('config = {}'.format(ub.urepr(dict(config), nl=1)))
+    config = CocoCropTrackConfig.cli(cmdline=cmdline, data=kwargs, strict=True)
+    print('config = {}'.format(ub.urepr(config, nl=1)))
     src = config['src']
     dst = ub.Path(config['dst'])
     dst_bundle_dpath = dst.parent
 
     print('load = {}'.format(ub.urepr(src, nl=1)))
     if config['sqlmode']:
         coco_dset = kwcoco.CocoSqlDatabase.coerce(src)
```

### Comparing `geowatch-0.6.3/watch/cli/coco_reformat_channels.py` & `geowatch-0.6.6/watch/cli/coco_reformat_channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ubelt as ub
 import scriptconfig as scfg
 import os
 
 
-class CocoReformatChannels(scfg.Config):
+class CocoReformatChannels(scfg.DataConfig):
     """
     Helper to remove channels from a coco file and reformat predictions from
     float32 to int16.
     """
     __default__ = {
         'src': scfg.Value(None, help='path to coco dataset to read and rewrite'),
 
@@ -58,17 +58,17 @@
         >>> new_coco_img = reformatted_dset.coco_image(gid)
         >>> import numpy as np
         >>> new_pred1 = np.nan_to_num(new_coco_img.imdelay('salient').finalize())
         >>> #assert np.allclose(new_pred1, new_pred2)
         >>> #new_pred2 = new_coco_img.imdelay('salient').finalize(dequantize=False)
         >>> #assert new_pred2.dtype.kind == 'i'
     """
-    config = CocoReformatChannels.cli(data=kwargs, cmdline=cmdline)
+    config = CocoReformatChannels.cli(data=kwargs, cmdline=cmdline, strict=True)
     import kwcoco
-    print('config = {}'.format(ub.urepr(dict(config), nl=1)))
+    print('config = {}'.format(ub.urepr(config, nl=1)))
     dset = kwcoco.CocoDataset.coerce(config['src'])
 
     to_quantize = kwcoco.ChannelSpec.coerce('' if config['quantize'] is None else config['quantize']).fuse()
     to_remove = kwcoco.ChannelSpec.coerce('' if config['remove'] is None else config['remove']).fuse()
 
     tasks = []
     for coco_img in dset.images().coco_images:
```

### Comparing `geowatch-0.6.3/watch/cli/coco_remove_bad_images.py` & `geowatch-0.6.6/watch/cli/coco_remove_bad_images.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/coco_shard.py` & `geowatch-0.6.6/watch/cli/coco_shard.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 UNUSED AND UNDEVELOEPD
 """
 import ubelt as ub
 import scriptconfig as scfg
 
 
-class CocoShardConfig(scfg.Config):
+class CocoShardConfig(scfg.DataConfig):
     """
     Shards a kwcoco dataset into multiple subparts
 
     UNUSED AND UNDEVELOEPD
     """
     __default__ = {
         'src': scfg.Value(None, help='input dataset to split', position=1),
@@ -35,15 +35,15 @@
         >>>     'src': dset.fpath,
         >>>     'max_shard_size': 2,
         >>> }
         >>> cmdline = False
         >>> main(cmdline, **kw)
     """
     import kwcoco
-    config = CocoShardConfig(kw, cmdline=cmdline)
+    config = CocoShardConfig.cli(data=kw, cmdline=cmdline, strict=True)
     print('config = {}'.format(ub.urepr(dict(config), nl=1)))
 
     if config['src'] is None:
         raise Exception('must specify source: {}'.format(config['src']))
 
     dst_pattern = config['dst_pattern']
     num_shards = config['num_shards']
```

### Comparing `geowatch-0.6.3/watch/cli/coco_spectra.py` & `geowatch-0.6.6/watch/cli/coco_spectra.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/coco_time_combine.py` & `geowatch-0.6.6/watch/cli/coco_time_combine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 """
 
 SeeAlso:
-    ~/code/watch/dev/poc/prepare_time_combined_dataset.py
+    ~/code/watch/watch/cli/queue_cli/prepare_time_combined_dataset.py
 
 
 CommandLine:
     DVC_DATA_DPATH=$(geowatch_dvc --tags='phase2_data' --hardware=auto)
 
     python -m watch.cli.coco_time_combine \
         --input_kwcoco_fpath="$DVC_DATA_DPATH/Drop6/imgonly-KR_R002.kwcoco.zip" \
@@ -983,15 +983,53 @@
                                     scale_asset_from_stitchspace=scale_asset_from_vid)
     stitch_manager.finalize_image(gid)
     final_img = tmp_dset.imgs[gid]
 
     return final_img
 
 
-def filter_image_ids_by_season(coco_dset, image_ids, filtered_seasons):
+def filter_image_ids_by_season(coco_dset, image_ids, filtered_seasons, ignore_winter_torrid_zone=True):
+    """Filter a sequence of image ids by season and geolocation.
+
+    Args:
+        coco_dset (kwcoco.CocoDataset): A KWCOCO dataset object.
+        image_ids (List(int)): A list of image ids that belong in coco_dset.
+        filtered_seasons (str | List(str) | None): Which seasons to not include in the
+             returned image ids.
+        ignore_winter_torrid_zone (bool, optional): Do not filter images within the 
+            Torrid region when winter is one of the filtered seasons. Defaults to True.
+
+    Raises:
+        ValueError: Check if the filtered seasons varible is a correctable type.
+        ValueError: Check if one of the filtered seasons is not a valid season.
+
+    Returns:
+        List[int]: A list of filtered image ids. Should never be longer than the input
+             image ids.
+
+    Example:
+        >>> # 0: Baseline run.
+        >>> # xdoctest: +REQUIRES(env:DEVEL_TEST)
+        >>> from watch.cli.coco_time_combine import *  # NOQA
+        >>> import watch
+        >>> data_dvc_dpath = watch.find_dvc_dpath(tags='phase2_data', hardware='auto')
+        >>> # Load KWCOCO dataset.
+        >>> input_kwcoco_fpath = data_dvc_dpath / 'Drop6/imgonly-AE_C001.kwcoco.json'
+        >>> coco_dset = kwcoco.CocoDataset(input_kwcoco_fpath)
+        >>> image_ids = coco_dset.images().gids
+        >>> ignore_torrid_regions_gids = filter_image_ids_by_season(coco_dset, 
+        >>>                                image_ids, 
+        >>>                                filtered_seasons='winter', 
+        >>>                                ignore_winter_torrid_zone=True)
+        >>> all_filtered_gids = filter_image_ids_by_season(coco_dset, 
+        >>>                       image_ids, 
+        >>>                       filtered_seasons='winter', 
+        >>>                       ignore_winter_torrid_zone=True)
+        >>> assert len(all_filtered_gids) > len(ignore_torrid_regions_gids)
+    """
     from watch.utils import util_time
     hemipshere_to_season_map = {
         'northern': {
             'spring': [3, 4, 5],
             'summer': [6, 7, 8],
             'fall': [9, 10, 11],
             'winter': [12, 1, 2]
@@ -1000,54 +1038,84 @@
             'spring': [9, 10, 11],
             'summer': [12, 1, 2],
             'fall': [3, 4, 5],
             'winter': [6, 7, 8]
         }
     }
 
+    # Check if there are any images to filter.
     if len(image_ids) == 0:
         print('WARNING: No images to filter.')
         return []
 
-    if not isinstance(filtered_seasons, list):
+    # Check type of filtered_seasons variable and try to convert to list.
+    if isinstance(filtered_seasons, str):
         filtered_seasons = [filtered_seasons]
+    elif filtered_seasons is None:
+        filtered_seasons = []
+    elif isinstance(filtered_seasons, list):
+        pass
+    else:
+        raise ValueError(f'Filtered seasons must be a list or string. Got "{type(filtered_seasons)}" type.')
 
+    # Get seasons to filter (invalid seasons).
     filtered_seasons = set(filtered_seasons)
     valid_seasons = {'spring', 'summer', 'fall', 'winter'}
 
     invalid_seasons = filtered_seasons - valid_seasons
     if invalid_seasons:
         raise ValueError(f'Invalid seasons: {invalid_seasons}')
 
     # Get hemisphere of region.
     coco_img = coco_dset.coco_image(image_ids[0])
-    lon, _ = coco_img.img['geos_corners']['coordinates'][0][0]
+    import numpy as np
+    geo_corner_coords = np.asarray(coco_img.img['geos_corners']['coordinates'])
+    center_coord = geo_corner_coords.mean(axis=1)[0]
+    _, lat = center_coord[0], center_coord[1]
 
-    if lon > 0:
+    # Check if the latitude is in the northern or southern hemisphere.
+    if lat > 0:
         hemisphere = 'northern'
     else:
         hemisphere = 'southern'
 
+    # Check if the region is within the torrid zone.
+    # Torrid zone is generally warm and less likely to contain snow.
+    # https://en.wikipedia.org/wiki/Geographical_zone
+    # https://www.toppr.com/guides/chemistry/environmental-chemistry/torrid-zone/
+    # Should technically be 23.5 but bumpping up to 27 to include AE regions
+    within_torrid_zone = abs(lat) < 27
+
     month_to_season_map = {}
     for season, months in hemipshere_to_season_map[hemisphere].items():
         for month in months:
             month_to_season_map[month] = season
 
     final_image_ids = []
     for image_id in image_ids:
         coco_img = coco_dset.coco_image(image_id)
 
-        # Get month.
+        # Get month image was taken in.
         dt = util_time.coerce_datetime(coco_img['date_captured'])
         month = dt.month
 
-        # Get season of month.
+        # Get season of month (depends on northern or southern hemisphere).
         img_season = month_to_season_map[month]
-        if img_season not in filtered_seasons:
+
+        # Do not filter image if ALL conditions are met:
+        # 1) We are not removing images within the torrid zone during winter,
+        # 2) the region latitude is within the torrid zone (|lat| < 23.5),
+        # 3) winter is in the filtered seasons,
+        # 4) the image was captured during winter.
+        if ignore_winter_torrid_zone and within_torrid_zone and (img_season == 'winter') and ("winter" in filtered_seasons):
             final_image_ids.append(image_id)
+        else:
+            # Check if the season is not in the filtered seasons.
+            if img_season not in filtered_seasons:
+                final_image_ids.append(image_id)
 
     return final_image_ids
 
 
 __config__ = TimeCombineConfig
 
 if __name__ == '__main__':
```

### Comparing `geowatch-0.6.3/watch/cli/coco_update_geotiff_metadata.py` & `geowatch-0.6.6/watch/cli/coco_update_geotiff_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ubelt as ub
 import scriptconfig as scfg
 # import numpy as np
 # import kwimage
 
 
-class UpdateGeotiffMetadataConfig(scfg.Config):
+class UpdateGeotiffMetadataConfig(scfg.DataConfig):
     """
     Simplified version of coco-add-watch-fields that only ensures that geotiff
     metadata is propogated to all auxiliary assets within an image.
 
     Modifies the underlying images on disk.  Does not modify the kwcoco file.
     """
     __default__ = {
@@ -71,15 +71,16 @@
         from watch.cli.coco_update_geotiff_metadata import *  # NOQA
         import watch
         dvc_dpath = watch.find_smart_dvc_dpath()
         base_fpath = dvc_dpath / 'Aligned-Drop3-TA1-2022-03-10/combo_LM.kwcoco.json'
         base_fpath = dvc_dpath / 'Aligned-Drop3-TA1-2022-03-10/dzyne_landcover.kwcoco.json'
         kwargs = {'src': base_fpath}
     """
-    config = UpdateGeotiffMetadataConfig(kwargs, cmdline=True)
+    config = UpdateGeotiffMetadataConfig.cli(data=kwargs, cmdline=cmdline,
+                                             strict=True)
 
     from watch.utils import kwcoco_extensions
     import kwcoco
     coco_dset = kwcoco.CocoDataset.coerce(config['src'])
 
     valid_gids = kwcoco_extensions.filter_image_ids(
         coco_dset,
```

### Comparing `geowatch-0.6.3/watch/cli/coco_visualize_videos.py` & `geowatch-0.6.6/watch/cli/coco_visualize_videos.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     python -m watch.cli.coco_visualize_videos --src=$KWCOCO_FPATH --viz_dpath=$VIZ_DPATH --zoom_to_tracks=True --start_frame=1 --num_frames=5 --animate=True
 """
 import scriptconfig as scfg
 import ubelt as ub
 
 
-class CocoVisualizeConfig(scfg.Config):
+class CocoVisualizeConfig(scfg.DataConfig):
     """
     Visualizes annotations on kwcoco video frames on each band
 
     CommandLine:
         # Point to your kwcoco file
         DVC_DPATH=$HOME/data/dvc-repos/smart_watch_dvc
         COCO_FPATH=$DVC_DPATH/drop1-S2-L8-aligned/data.kwcoco.json
@@ -221,25 +221,27 @@
     Ignore:
         src = ub.expandpath('$HOME/data/dvc-repos/smart_watch_dvc/drop1-S2-L8-aligned/data.kwcoco.json')
         cmdline = False
         kwargs = {
             'src': src,
         }
     """
+    config = CocoVisualizeConfig.cli(data=kwargs, cmdline=cmdline and
+                                     {'strict': True}, strict=True)
     from watch.utils import util_parallel
     from watch.utils import util_resources
     from watch.utils import kwcoco_extensions
     import kwcoco
     import kwarray
     import rich
     import numpy as np
-    config = CocoVisualizeConfig(data=kwargs, cmdline=cmdline and {'strict': True})
+    rich.print('config = {}'.format(ub.urepr(dict(config), nl=2)))
+
     space = config['space']
     channels = config['channels']
-    rich.print('config = {}'.format(ub.urepr(dict(config), nl=2)))
 
     if config['smart']:
         if config['workers'] == 'auto':
             config['workers'] = 'avail'
         if config['animate'] == 'auto':
             config['animate'] = True
         if config['stack'] == 'auto':
@@ -372,15 +374,16 @@
                     keep.append(coco_img.img['id'])
             else:
                 if requested_channels & code:
                     keep.append(coco_img.img['id'])
         rich.print(f'Filtered {len(coco_images) - len(keep)} images without requested channels. Keeping {len(keep)}')
         selected_gids = keep
 
-    rich.print(f'Will write to: [link={viz_dpath}]{viz_dpath}[/link]')
+    viz_dpath_abs = viz_dpath.absolute()
+    rich.print(f'Will write to: [link={viz_dpath_abs}]{viz_dpath_abs}[/link]')
 
     video_names = []
     for vidid, video in prog:
 
         sub_dpath = viz_dpath / video['name']
 
         gids = coco_dset.index.vidid_to_gids[vidid]
@@ -532,15 +535,15 @@
                 job.result()
             except SkipFrame:
                 ...
 
         pool.jobs.clear()
 
     pman.__exit__(None, None, None)
-    rich.print(f'Wrote images to: [link={viz_dpath}]{viz_dpath}[/link]')
+    rich.print(f'Wrote images to: [link={viz_dpath_abs}]{viz_dpath_abs}[/link]')
 
     if config['animate']:
         # TODO: develop this idea more
         # Try to parse out an animation config
         import scriptconfig as scfg
         from watch.utils import util_yaml
 
@@ -567,24 +570,33 @@
         # Hack: pretend that stack is a channel even though it is not.
         if config['stack']:
             if not channels:
                 channels = 'stack'
             else:
                 channels = channels + ',stack'
 
-        animate_visualizations.animate_visualizations(
+        outputs = animate_visualizations.animate_visualizations(
             viz_dpath=viz_dpath,
             channels=channels,
             video_names=video_names,
             draw_imgs=config['draw_imgs'],
             draw_anns=config['draw_anns'],
             workers=max_workers,
             zoom_to_tracks=config['zoom_to_tracks'],
             **animate_config,
         )
+        # Links for summaries
+        type_to_anis = ub.group_items(outputs, lambda x: x['type'])
+        for ani_type, items in type_to_anis.items():
+            summary_fpath = (viz_dpath / ('_' + ani_type)).ensuredir()
+            for item in items:
+                fpath = ub.Path(item['fpath'])
+                dst = summary_fpath / fpath.name
+                ub.symlink(fpath, dst)
+
         # Terminal fixup
         import sys
         if sys.stdout.isatty():
             ub.cmd('stty sane', verbose=3)
 
 
 class SkipFrame(Exception):
```

### Comparing `geowatch-0.6.3/watch/cli/concat_kwcoco_videos.py` & `geowatch-0.6.6/watch/cli/concat_kwcoco_videos.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/crop_sites_to_regions.py` & `geowatch-0.6.6/watch/cli/crop_sites_to_regions.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/dag_cli/run_bas_datagen.py` & `geowatch-0.6.6/watch/cli/dag_cli/run_bas_datagen.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/dag_cli/run_bas_fusion.py` & `geowatch-0.6.6/watch/cli/dag_cli/run_bas_fusion.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/dag_cli/run_dino_sv.py` & `geowatch-0.6.6/watch/cli/dag_cli/run_dino_sv.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/dag_cli/run_dzyne_parallel_site_vali.py` & `geowatch-0.6.6/watch/cli/dag_cli/run_dzyne_parallel_site_vali.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/dag_cli/run_pseudolive_consolidate.py` & `geowatch-0.6.6/watch/cli/dag_cli/run_pseudolive_consolidate.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/dag_cli/run_psuedolive_copy_previous.py` & `geowatch-0.6.6/watch/cli/dag_cli/run_psuedolive_copy_previous.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/dag_cli/run_sc_datagen.py` & `geowatch-0.6.6/watch/cli/dag_cli/run_sc_datagen.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/dag_cli/run_sc_fusion.py` & `geowatch-0.6.6/watch/cli/dag_cli/run_sc_fusion.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/dag_cli/run_sv_datagen.py` & `geowatch-0.6.6/watch/cli/dag_cli/run_sv_datagen.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/dag_cli/run_teamfeat_invariants.py` & `geowatch-0.6.6/watch/cli/dag_cli/run_teamfeat_invariants.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/dag_cli/run_teamfeat_landcover.py` & `geowatch-0.6.6/watch/cli/dag_cli/run_teamfeat_landcover.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/extend_sc_sites.py` & `geowatch-0.6.6/watch/cli/extend_sc_sites.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/find_dvc.py` & `geowatch-0.6.6/watch/cli/find_dvc.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     echo "DVC_DATA_DPATH = $DVC_DATA_DPATH"
     echo "DVC_EXPT_DPATH = $DVC_EXPT_DPATH"
 
 """
 import scriptconfig as scfg
 
 
-class FindDVCConfig(scfg.Config):
+class FindDVCConfig(scfg.DataConfig):
     """
     Command line helper to find the path to the watch DVC repo
 
     Example Usage:
         # List currently known directories
         geowatch_dvc list
 
@@ -92,15 +92,15 @@
 
     @staticmethod
     def main(cmdline=True, **kwargs):
         from watch.utils import util_data
         from rich import print
         import ubelt as ub
 
-        cli_config = FindDVCConfig(data=kwargs, cmdline=cmdline)
+        cli_config = FindDVCConfig.cli(data=kwargs, cmdline=cmdline, strict=True)
         config = dict(cli_config)
 
         command = config.pop('command')
         verbose = config.pop('verbose')
         must_exist = config.pop('must_exist')
         if must_exist == 'auto':
             must_exist = command == 'find'
```

### Comparing `geowatch-0.6.3/watch/cli/geojson_site_stats.py` & `geowatch-0.6.6/watch/cli/geojson_site_stats.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/geotiffs_to_kwcoco.py` & `geowatch-0.6.6/watch/cli/geotiffs_to_kwcoco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/gifify.py` & `geowatch-0.6.6/watch/cli/gifify.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/kwcoco_to_geojson.py` & `geowatch-0.6.6/watch/cli/kwcoco_to_geojson.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,35 +91,35 @@
     #
     # or
     #
     # in_file = None
     # in_file : scfg.Value[help='Input KWCOCO to convert', position=1]
 
     in_file = scfg.Value(None, required=True, help='Input KWCOCO to convert',
-                         position=1)
+                         position=1, alias=['input_kwcoco'])
 
     out_kwcoco = scfg.Value(None, help=ub.paragraph(
             '''
             The file path to write the "tracked" kwcoco file to.
             '''))
 
     out_sites_dir = scfg.Value(None, help=ub.paragraph(
         '''
         The directory where site model geojson files will be written.
-        '''))
+        '''), alias=['output_sites_dpath'])
 
     out_site_summaries_dir = scfg.Value(None, help=ub.paragraph(
         '''
         The directory path where site summary geojson files will be written.
         '''))
 
     out_sites_fpath = scfg.Value(None, help=ub.paragraph(
         '''
         The file path where a manifest of all site models will be written.
-        '''))
+        '''), alias=['output_site_manifest_fpath'])
 
     out_site_summaries_fpath = scfg.Value(None, help=ub.paragraph(
         '''
         The file path where a manifest of all site summary geojson files will
         be written.
         '''))
 
@@ -172,14 +172,16 @@
             Each summary found will be added to in_file as
             'Site Boundary' annotations.
             '''), group='behavior')
     clear_annots = scfg.Value(False, isflag=True, help=ub.paragraph(
             '''
             Clears all annotations before running tracking, so it starts
             from a clean slate.
+            TODO: perhaps name to something that takes the value overwrite or
+            append?
             '''), group='behavior')
     append_mode = scfg.Value(False, isflag=True, help=ub.paragraph(
             '''
             Append sites to existing region GeoJSON.
             '''), group='behavior')
 
     boundary_region = scfg.Value(None, help=ub.paragraph(
```

### Comparing `geowatch-0.6.3/watch/cli/merge_region_models.py` & `geowatch-0.6.6/watch/cli/merge_region_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,35 +2,32 @@
 """
 import re
 import ubelt as ub
 import scriptconfig as scfg
 import json
 
 
-class MergeRegionModelConfig(scfg.Config):
+class MergeRegionModelConfig(scfg.DataConfig):
     """
     Combine the specific features from multiple region files into a single one.
     """
     __default__ = {
-        'src':
-        scfg.Value([],
-                   help='paths to input geojson region files',
-                   nargs='+',
-                   position=1),
-        'dst':
-        scfg.Value(None, help='path to combined multi-region file'),
-        'match_type':
-        scfg.Value('region',
-                   help=ub.paragraph('''
+        'src': scfg.Value([], nargs='+', position=1,
+                          help='paths to input geojson region files'),
+
+        'dst': scfg.Value(None, help='path to combined multi-region file'),
+
+        'match_type': scfg.Value('region', help=ub.paragraph(
+            '''
             regex that filters results to only contain features where
             properties.type match.
             ''')),
-        'match_subtype':
-        scfg.Value('site',
-                   help=ub.paragraph('''
+
+        'match_subtype': scfg.Value('site', help=ub.paragraph(
+            '''
             regex that filters results to include subregion features as
             metadata inside regions, where properties.type match.
             ''')),
     }
     epilog = r"""
     Example Usage:
 
@@ -62,16 +59,16 @@
         >>> region_fpath = os.path.join(dvc_repo, 'drop1/region_models')
         >>> json_paths = list(glob.glob(os.path.join(region_fpath, '*.geojson')))
         >>> kwargs = {'src': json_paths}
         >>> main(**kwargs)
 
     """
     import geojson
-    config = MergeRegionModelConfig(data=kwargs, cmdline=cmdline)
-    # print('config = {}'.format(ub.urepr(dict(config), nl=1)))
+    config = MergeRegionModelConfig.cli(data=kwargs, cmdline=cmdline, strict=True)
+    print('config = {}'.format(ub.urepr(config, nl=1)))
 
     json_paths = config['src']
     output_fpath = config['dst']
 
     combo = combine_region_models(json_paths, config['match_type'],
                                   config['match_subtype'])
```

### Comparing `geowatch-0.6.3/watch/cli/prepare_splits.py` & `geowatch-0.6.6/watch/cli/prepare_splits.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,24 +28,22 @@
 
 """
 
 import scriptconfig as scfg
 import ubelt as ub
 
 
-class PrepareSplitsConfig(scfg.Config):
+class PrepareSplitsConfig(scfg.DataConfig):
     """
     This generates the bash commands necessary to split a base kwcoco file into
     the standard train / validation splits.
 
     Ignore:
         base_fpath = 'imganns*.kwcoco.*'
     """
-    __fuzzy_hyphens__ = 1
-
     __default__ = {
         'base_fpath': scfg.Value(None, nargs='+', help='base coco file to split or a globstring in constructive mode', position=1),
 
         'virtualenv_cmd': scfg.Value(None, type=str, help=ub.paragraph(
             '''
             Command to start the appropriate virtual environment if your bashrc
             does not start it by default.''')),
@@ -55,15 +53,15 @@
         'backend': scfg.Value('tmux', help='can be serial, tmux, or slurm. Using tmux is recommended.'),
         'with_textual': scfg.Value('auto', help='setting for cmd-queue monitoring'),
         'other_session_handler': scfg.Value('ask', help='for tmux backend only. How to handle conflicting sessions. Can be ask, kill, or ignore, or auto'),
 
         'constructive_mode': scfg.Value(False, help='if True use the new constructive mode'),
 
         'verbose': scfg.Value(1, help=''),
-        'workers': scfg.Value(2, help=''),
+        'workers': scfg.Value(2, help='', alias=['tmux_workers']),
 
         'suffix': scfg.Value('', help='suffix for the output split filenames'),
     }
 
 
 # TODO: should be some sort of external file we read / define
 VALI_REGIONS_SPLITS = {
@@ -232,16 +230,15 @@
     The idea is that we should have a lightweight scheduler.  I think something
     fairly minimal can be implemented with tmux, but it would be nice to have a
     more robust slurm extension.
 
     TODO:
         - [ ] Option to just dump the serial bash script that does everything.
     """
-    config = PrepareSplitsConfig(cmdline=cmdline)
-    config.update(kwargs)
+    config = PrepareSplitsConfig.cli(data=kwargs, cmdline=cmdline, strict=True)
     print('config = {}'.format(ub.urepr(dict(config), nl=1)))
 
     if config['base_fpath'] == 'auto':
         # Auto hack.
         raise NotImplementedError
         import watch
         dvc_dpath = watch.find_smart_dvc_dpath()
```

### Comparing `geowatch-0.6.3/watch/cli/prepare_ta2_dataset.py` & `geowatch-0.6.6/watch/cli/prepare_ta2_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,18 @@
         'force_min_gsd': scfg.Value(None, group='align'),
         'align_keep': scfg.Value('img', choices=['img', 'img-roi', 'none', None], help='if the coco align script caches or recomputes images / rois', group='align'),
         'force_nodata': scfg.Value(None, help='if specified, forces nodata to this value', group='align'),
 
         'splits': scfg.Value(False, isflag=1, help='if True do splits'),
 
         'region_globstr': scfg.Value('annotations/region_models', help='region model globstr (relative to the dvc path, unless absolute or prefixed by "./")'),
-        'site_globstr': scfg.Value('annotations/site_models', help='site model globstr (relative to the dvc path, unless absolute or prefixed by "./")'),
+        'site_globstr': scfg.Value(
+            None,
+            # 'annotations/site_models',
+            help='site model globstr (relative to the dvc path, unless absolute or prefixed by "./")'),
 
         'propogate_strategy': scfg.Value('NEW-SMART', help='changes propogation behavior'),
 
         'remove_broken': scfg.Value(True, isflag=1, help='if True, will remove any image that fails population (e.g. caused by a 404)'),
 
         'cache': scfg.Value(1, isflag=1, help='If 1 or 0 globally enable/disable caching. If a comma separated list of strings, only cache those stages', group='queue-related'),
         'skip_existing': scfg.Value(False, help='Unlike cache=1, which checks for file existence at runtime, this will explicitly not submit any job with a product that already exist', group='queue-related'),
@@ -468,15 +471,15 @@
             },
             out_paths={
                 'uncropped_catalog_fpath': uncropped_catalog_fpath,
             },
             stage='catalog',
         )
 
-        uncropped_kwcoco_fpath = uncropped_dpath / f'data_{s3_name}.kwcoco.json'
+        uncropped_kwcoco_fpath = uncropped_dpath / f'data_{s3_name}.kwcoco.zip'
         uncropped_kwcoco_fpath = uncropped_kwcoco_fpath.shrinkuser(home='$HOME')
 
         convert_options = []
         if collated:
             convert_options.append('--from-collated')
         if config['ignore_duplicates']:
             convert_options.append('--ignore_duplicates')
@@ -498,15 +501,15 @@
             },
             out_paths={
                 'uncropped_kwcoco_fpath': uncropped_kwcoco_fpath,
             },
             stage='uncropped_kwcoco',
         )
 
-        uncropped_fielded_kwcoco_fpath = uncropped_dpath / f'data_{s3_name}_fielded.kwcoco.json'
+        uncropped_fielded_kwcoco_fpath = uncropped_dpath / f'data_{s3_name}_fielded.kwcoco.zip'
         uncropped_fielded_kwcoco_fpath = uncropped_fielded_kwcoco_fpath.shrinkuser(home='$HOME')
 
         add_fields_job = pipeline.submit(command=ub.codeblock(
             rf'''
             {job_environ_str}python -m watch.cli.coco_add_watch_fields \
                 --src "{uncropped_kwcoco_fpath}" \
                 --dst "{uncropped_fielded_kwcoco_fpath}" \
@@ -538,26 +541,26 @@
         # TODO: make use of region_id_to_site_fpaths
         # to build a better site globstr (might need to write a tempoaray file
         # to point to)
         final_site_globstr = _coerce_globstr(config['site_globstr'])
         for info in uncropped_fielded_jobs:
             toalign_info = info.copy()
             name = toalign_info['name'] = info['name']
-            toalign_info['aligned_imgonly_fpath'] = aligned_kwcoco_bundle / f'imgonly-{name}.kwcoco.json'
-            toalign_info['aligned_imganns_fpath'] = aligned_kwcoco_bundle / f'imganns-{name}.kwcoco.json'
+            toalign_info['aligned_imgonly_fpath'] = aligned_kwcoco_bundle / f'imgonly-{name}.kwcoco.zip'
+            toalign_info['aligned_imganns_fpath'] = aligned_kwcoco_bundle / f'imganns-{name}.kwcoco.zip'
             # TODO: take only the corresponding set of site models here.
             toalign_info['site_globstr'] = final_site_globstr
             toalign_info['region_globstr'] = info['region_globstr']
             alignment_input_jobs.append(toalign_info)
     else:
         # Do a noop for this case? Or make it fast in kwcoco itself?
         uncropped_coco_paths = [d['uncropped_fielded_fpath'] for d in uncropped_fielded_jobs]
         union_depends_jobs = [d['job'] for d in uncropped_fielded_jobs]
         union_suffix = ub.hash_data([p.name for p in uncropped_coco_paths])[0:8]
-        uncropped_final_kwcoco_fpath = uncropped_dpath / f'data_{union_suffix}.kwcoco.json'
+        uncropped_final_kwcoco_fpath = uncropped_dpath / f'data_{union_suffix}.kwcoco.zip'
         uncropped_final_kwcoco_fpath = uncropped_final_kwcoco_fpath.shrinkuser(home='$HOME')
         uncropped_multi_src_part = ' '.join(['"{}"'.format(p) for p in uncropped_coco_paths])
         union_job = pipeline.submit(command=ub.codeblock(
             rf'''
             # COMBINE Uncropped datasets
             {job_environ_str}python -m kwcoco union \
                 --src {uncropped_multi_src_part} \
@@ -573,16 +576,16 @@
         )
         uncropped_final_jobs = [union_job]
 
         final_site_globstr = _coerce_globstr(config['site_globstr'])
         alignment_input_jobs = [{
             'name': f'align-{union_suffix}',
             'uncropped_fielded_fpath': uncropped_final_kwcoco_fpath,
-            'aligned_imgonly_fpath': aligned_kwcoco_bundle / 'imgonly.kwcoco.json',
-            'aligned_imganns_fpath': aligned_kwcoco_bundle / 'imganns.kwcoco.json',
+            'aligned_imgonly_fpath': aligned_kwcoco_bundle / 'imgonly.kwcoco.zip',
+            'aligned_imganns_fpath': aligned_kwcoco_bundle / 'imganns.kwcoco.zip',
             'region_globstr': final_region_globstr,
             'site_globstr': final_site_globstr,
             'job': uncropped_final_jobs,
         }]
 
     alignment_jobs = []
     for info in alignment_input_jobs:
@@ -790,15 +793,15 @@
         from watch.cli import prepare_splits
         prepare_splits._submit_split_jobs(
             aligned_final_fpath, queue, depends=[aligned_final_jobs])
 
     # TODO: Can start the DVC add of the region subdirectories here
     ub.codeblock(
         '''
-        7z a splits.zip data*.kwcoco.json
+        7z a splits.zip data*.kwcoco.zip
 
         ls */WV
         ls */L8
         ls */S2
         ls */*.json
         dvc add *.zip
         dvc add */WV */L8 */S2 */*.json *.zip
@@ -814,15 +817,15 @@
         */*.json
         ''')
 
     # pipeline.submit(ub.codeblock(
     #     '''
     #     DVC_DPATH=$(geowatch_dvc)
     #     python -m watch.cli.prepare_splits \
-    #         --base_fpath=$DVC_DPATH/Drop2-Aligned-TA1-2022-02-15/data.kwcoco.json \
+    #         --base_fpath=$DVC_DPATH/Drop2-Aligned-TA1-2022-02-15/data.kwcoco.zip \
     #         --run=1 --serial=True
     #     '''))
 
     config.run_queue(queue)
 
     # if config.rprint:
     #     queue.print_graph()
@@ -836,15 +839,15 @@
     # TODO: team features
     """
     DATASET_CODE=Aligned-Drop2-TA1-2022-03-07
     DVC_DPATH=$(geowatch_dvc)
     DATASET_CODE=Drop2-Aligned-TA1-2022-02-15
     KWCOCO_BUNDLE_DPATH=$DVC_DPATH/$DATASET_CODE
     python -m watch.cli.prepare_teamfeats \
-        --base_fpath=$KWCOCO_BUNDLE_DPATH/data.kwcoco.json \
+        --base_fpath=$KWCOCO_BUNDLE_DPATH/data.kwcoco.zip \
         --gres=0, \
         --with_depth=0 \
         --with_landcover=0 \
         --with_invariants=0 \
         --with_materials=1 \
         --depth_workers=auto \
         --do_splits=1  --cache=1 --run=0
@@ -859,17 +862,17 @@
 
 # #region_models=$dvc_dpath'/annotations/region_models/*.geojson'
 # region_models=$dvc_dpath/annotations/region_models/kr_r002.geojson
 # # helper variables
 # uncropped_dpath=$dvc_dpath/$uncropped_bundle_name
 # uncropped_query_dpath=$uncropped_dpath/_query/items
 # uncropped_ingress_dpath=$uncropped_dpath/ingress
-# uncropped_kwcoco_fpath=$uncropped_dpath/data.kwcoco.json
+# uncropped_kwcoco_fpath=$uncropped_dpath/data.kwcoco.zip
 # aligned_kwcoco_bundle=$dvc_dpath/$aligned_bundle_name
-# aligned_kwcoco_fpath=$aligned_kwcoco_bundle/data.kwcoco.json
+# aligned_kwcoco_fpath=$aligned_kwcoco_bundle/data.kwcoco.zip
 # uncropped_query_fpath=$uncropped_query_dpath/$query_basename
 # uncropped_catalog_fpath=$uncropped_ingress_dpath/catalog.json
 
 # export AWS_DEFAULT_PROFILE=iarpa
 #     pass
```

### Comparing `geowatch-0.6.3/watch/cli/prepare_teamfeats.py` & `geowatch-0.6.6/watch/cli/prepare_teamfeats.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,26 +389,27 @@
         task = {}
         task['output_fpath'] = outputs['cold']
         task['gpus'] = 0
         task['command'] = ub.codeblock(
             fr'''
             python -m watch.tasks.cold.predict \
                 --coco_fpath="{base_fpath}" \
+                --out_dpath="{base_fpath.parent}" \
                 --mod_coco_fpath="{task['output_fpath']}" \
                 --sensors='L8' \
                 --adj_cloud=False \
                 --method='COLD' \
                 --prob=0.99 \
                 --conse=6 \
                 --cm_interval=60 \
                 --year_lowbound=None \
                 --year_highbound=None \
                 --coefs=cv,rmse,a0,a1,b1,c1 \
                 --coefs_bands=0,1,2,3,4,5 \
-                --timestamp=True \
+                --timestamp=False \
                 --combine=False \
                 --resolution=30GSD \
                 --workermode="{config.cold_workermode}" \
                 --workers="{config.cold_workers}"
             ''')
         # --coefs=cv,a0,a1,b1,c1,rmse \
         combo_code_parts.append(codes[key])
```

### Comparing `geowatch-0.6.3/watch/cli/pseudolive_consolidate.py` & `geowatch-0.6.6/watch/cli/pseudolive_consolidate.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/reproject_annotations.py` & `geowatch-0.6.6/watch/cli/reproject_annotations.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/run_metrics_framework.py` & `geowatch-0.6.6/watch/cli/run_metrics_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/split_videos.py` & `geowatch-0.6.6/watch/cli/split_videos.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/stac_search.py` & `geowatch-0.6.6/watch/cli/stac_search.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/ta1_stac_to_kwcoco.py` & `geowatch-0.6.6/watch/cli/ta1_stac_to_kwcoco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/torch_model_stats.py` & `geowatch-0.6.6/watch/cli/torch_model_stats.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/validate_annotation_schemas.py` & `geowatch-0.6.6/watch/cli/validate_annotation_schemas.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/cli/watch_coco_stats.py` & `geowatch-0.6.6/watch/cli/watch_coco_stats.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/__init__.py` & `geowatch-0.6.6/watch/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/demo_region.py` & `geowatch-0.6.6/watch/demo/demo_region.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/dummy_demodata.py` & `geowatch-0.6.6/watch/demo/dummy_demodata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/landsat_demodata.py` & `geowatch-0.6.6/watch/demo/landsat_demodata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/metrics_demo/demo_rendering.py` & `geowatch-0.6.6/watch/demo/metrics_demo/demo_rendering.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/metrics_demo/demo_truth.py` & `geowatch-0.6.6/watch/demo/metrics_demo/demo_truth.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/metrics_demo/demo_utils.py` & `geowatch-0.6.6/watch/demo/metrics_demo/demo_utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/metrics_demo/generate_demodata.py` & `geowatch-0.6.6/watch/demo/metrics_demo/generate_demodata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/metrics_demo/site_perterbing.py` & `geowatch-0.6.6/watch/demo/metrics_demo/site_perterbing.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/nitf_demodata.py` & `geowatch-0.6.6/watch/demo/nitf_demodata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/sentinel2_demodata.py` & `geowatch-0.6.6/watch/demo/sentinel2_demodata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/smart_kwcoco_demodata.py` & `geowatch-0.6.6/watch/demo/smart_kwcoco_demodata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/demo/stac_demo.py` & `geowatch-0.6.6/watch/demo/stac_demo.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/geoannots/__init__.py` & `geowatch-0.6.6/watch/geoannots/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/geoannots/geococo_objects.py` & `geowatch-0.6.6/watch/geoannots/geococo_objects.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/geoannots/geomodels.py` & `geowatch-0.6.6/watch/geoannots/geomodels.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,72 @@
 """
-Geojson object oriented interface for region and site models
+Geojson object oriented interface for region and site models.
+
+This defines two classes ``SiteModel`` and ``RegionModel``, both of which
+inherit from ``geojson.FeatureCollection``, so all geojson operations are
+valid, but these classes contain extra convenience methods for loading,
+dumping, manipulating, validating, and inspecting the data.
+
+A non exhaustive list of convenience methods / properties of note are shared by
+both site and region models are:
+
+    * dumps - convert to a geojson string
+
+    * pandas - convert to a geopandas data frame
+
+    * coerce_multiple - read multiple geojson files at once.
+
+    * header - a quick way to access the singular header row (region for region models and site for site models).
+
+    * body_features - any row that is not a header is a body feature (site_summaries for region models and observations for site models).
+
+    * validate - checks the site/region model against the schema.
+
+    * random - classmethod to make a random instance of the site / region model for testing
+
+New region model specific convenience methods / properties are:
+
+    * site_summaries
+    * region_id
+    * pandas_summaries
+    * pandas_region
+
+New site model specific convenience methods / properties are:
+
+    * observations
+    * pandas_observations
+    * as_summary
+    * region_id
+    * site_id
+    * status
 
 SeeAlso:
     ../rc/registry.py
+
+The following example illustrates how to read region / site models efficiently
+
+Example:
+    >>> # xdoctest: +REQUIRES(env:HAS_DVC)
+    >>> import watch
+    >>> dvc_data_dpath = watch.find_dvc_dpath(tags='phase2_data', hardware='auto')
+    >>> region_models_dpath = dvc_data_dpath / 'annotations/drop6/region_models'
+    >>> site_models_dpath = dvc_data_dpath / 'annotations/drop6/site_models'
+    >>> from watch.geoannots import geomodels
+    >>> region_models = list(geomodels.RegionModel.coerce_multiple(region_models_dpath))
+    >>> site_models = list(geomodels.SiteModel.coerce_multiple(site_models_dpath, workers=8))
+    >>> print(f'Number of region models: {len(region_models)}')
+    >>> print(f'Number of site models: {len(site_models)}')
+    >>> # Quick demo of associating sites to regions
+    >>> region_id_to_sites = ub.group_items(site_models, key=lambda s: s.header['properties']['region_id'])
+    >>> region_id_to_num_sites = ub.udict(region_id_to_sites).map_values(len)
+    >>> print('region_id_to_num_sites = {}'.format(ub.urepr(region_id_to_num_sites, nl=1)))
+    >>> # It is also easy to convert these models to geopandas
+    >>> region_model = region_models[0]
+    >>> gdf = region_model.pandas()
+    >>> print(gdf)
 """
 import ubelt as ub
 import geopandas as gpd
 import geojson
 import jsonschema
 import copy
 from watch.utils import util_time
@@ -33,17 +93,32 @@
         return copy.deepcopy(self)
 
     def dumps(self, **kw):
         import json
         return json.dumps(self, **kw)
 
     @classmethod
-    def coerce_multiple(cls, data):
+    def coerce_multiple(cls, data, allow_raw=False, workers=0, mode='thread',
+                        verbose=1, desc=None):
+        """
+        Load multiple geojson files
+
+        Args:
+            arg (str | PathLike | List[str | PathLike]):
+                an argument that is coerceable to one or more geojson files.
+
+            **kwargs: see :func:`util_gis.coerce_geojson_datas`
+
+        Yields:
+            Self
+        """
         from watch.utils import util_gis
-        infos = list(util_gis.coerce_geojson_datas(data, format='json'))
+        infos = list(util_gis.coerce_geojson_datas(
+            data, format='json', allow_raw=allow_raw, workers=workers,
+            mode=mode, verbose=verbose, desc=desc))
         for info in infos:
             yield cls(**info['data'])
 
     @classmethod
     def coerce(cls, data):
         import os
         if isinstance(data, cls):
@@ -337,14 +412,18 @@
             summary = header.copy()
             summary['properties'] = summary['properties'].copy()
             assert summary['properties']['type'] == 'site'
             summary['properties']['type'] = 'site_summary'
             return SiteSummary(**summary)
 
     @property
+    def region_id(self):
+        return self.header['properties']['region_id']
+
+    @property
     def site_id(self):
         return self.header['properties']['site_id']
 
     @property
     def status(self):
         return self.header['properties']['status']
 
@@ -357,16 +436,23 @@
             if geom.geom_type in {'MultiPolygon', 'Polygon'}:
                 make_valid(geom)
             else:
                 geom = geom.buffer(3).convex_hull
                 geom = MultiPolygon([geom])
             feat['geometry'] = geom.__geo_interface__
 
+    def fix_sensor_names(self):
+        for feat in self.observations():
+            prop = feat['properties']
+            if prop.get('sensor_name') == 'WorldView 1':
+                prop['sensor_name'] = 'WorldView'
+
     def fixup(self):
         self.clamp_scores()
+        self.fix_sensor_names()
         # self.fix_geom()
 
     def clamp_scores(self):
         for feat in self.features:
             fprop = feat['properties']
             fprop['score'] = float(max(min(1, fprop['score']), 0))
```

### Comparing `geowatch-0.6.3/watch/gis/__init__.py` & `geowatch-0.6.6/watch/gis/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/gis/digital_globe.py` & `geowatch-0.6.6/watch/gis/digital_globe.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/gis/elevation.py` & `geowatch-0.6.6/watch/gis/elevation.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/gis/geotiff.py` & `geowatch-0.6.6/watch/gis/geotiff.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 from watch import exceptions
 
 try:
     from xdev import profile
 except Exception:
     profile = ub.identity
 
+import xdev
+xdev.make_warnings_print_tracebacks()
+
 
 @profile
 def geotiff_metadata(gpath, elevation='gtop30', strict=False,
                      supress_warnings=False):
     """
     Extract all relevant metadata we know how to extract.
 
@@ -202,19 +205,19 @@
         >>> info = geotiff_crs_info(gpath)
         >>> print('info = {}'.format(ub.urepr(info, nl=1, sort=False)))
         >>> assert not info['is_rpc']
         >>> assert info['img_shape'] == (512, 512)
 
         tf = info['wgs84_to_wld']
     """
-    from watch.utils import util_gdal
-    from osgeo import gdal
-    from osgeo import osr
     import affine
     import kwimage
+    from watch.utils import util_gdal
+    gdal = util_gdal.import_gdal()
+    osr = util_gdal.import_osr()
 
     info = {}
     ref = util_gdal.GdalDataset.coerce(gpath_or_ref)
 
     if 0:
         # TODO: is it more efficient to use a gdal info call?  Do we get all
         # the information we need from it so we can serialize the data?
@@ -524,16 +527,17 @@
 
 def make_crs_info_object(osr_crs):
     """
     Args:
         osr_crs (osr.SpatialReference): an osr object from gdal
 
     Example:
-        >>> from osgeo import osr
         >>> from watch.gis.geotiff import *  # NOQA
+        >>> from watch.utils import util_gdal
+        >>> osr = util_gdal.import_osr()
         >>> osr_crs = osr.SpatialReference()
         >>> osr_crs.ImportFromEPSG(4326)
         >>> crs_info = make_crs_info_object(osr_crs)
         >>> print('crs_info = {}'.format(ub.urepr(crs_info, nl=1)))
         >>> osr_crs = osr.SpatialReference()
         >>> osr_crs.ImportFromEPSG(4326)
         >>> osr_crs.SetAxisMappingStrategy(osr.OAMS_TRADITIONAL_GIS_ORDER)
@@ -568,15 +572,16 @@
         * OAMS_AUTHORITY_COMPLIANT means that the data axis will be
             identical to the CRS axis. This is the default value when
             instantiating OGRSpatialReference
 
         * OAMS_CUSTOM means that the data axis are customly defined with
             SetDataAxisToSRSAxisMapping
     """
-    from osgeo import osr
+    from watch.utils import util_gdal
+    osr = util_gdal.import_osr()
     if axis_mapping_int == osr.OAMS_TRADITIONAL_GIS_ORDER:
         axis_mapping = 'OAMS_TRADITIONAL_GIS_ORDER'
     elif axis_mapping_int == osr.OAMS_AUTHORITY_COMPLIANT:
         axis_mapping = 'OAMS_AUTHORITY_COMPLIANT'
     elif axis_mapping_int == osr.OAMS_CUSTOM:
         axis_mapping = 'OAMS_CUSTOM'
     else:
@@ -819,15 +824,16 @@
 
         def _is_rgb(gpath):
             # fallback for 'channels'
             # often, a gtiff is a TCI that was postprocessed in some way that destroys
             # the original naming convention
             #
             # this opens the image to check for that case as a fallback
-            from osgeo import gdal
+            from watch.utils import util_gdal
+            gdal = util_gdal.import_gdal()
             info = gdal.Info(gpath, format='json')
             if len(info['bands']) == 3:
                 # TODO sometimes colorInterpretation is stripped, but it's still RGB
                 # should this return True for any gpath with 3 bands?
                 if [b['colorInterpretation'] for b in info['bands']] == ['Red', 'Green', 'Blue']:
                     return True
             return False
```

### Comparing `geowatch-0.6.3/watch/gis/sensors/sentinel2.py` & `geowatch-0.6.6/watch/gis/sensors/sentinel2.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/gis/spatial_reference.py` & `geowatch-0.6.6/watch/gis/spatial_reference.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/heuristics.py` & `geowatch-0.6.6/watch/heuristics.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,108 +18,253 @@
 HEURISTIC_END_STATES = {
     'Post Construction'
 }
 
 
 # # FIXME: Hard-coded category aliases.
 # https://smartgitlab.com/TE/standards
-# # The correct way to handle these would be to have some information in the
-# # kwcoco category dictionary that specifies how the categories should be
-# # interpreted.
-# _HEURISTIC_CATEGORIES = {
-#     'background': {'background', 'No Activity', 'Post Construction'},
-#     'pre_background': {'No Activity'},
-#     'post_background': {'Post Construction'},
-#     'ignore': {'ignore', 'Unknown', 'clouds'},
-# }
 
 
-# TODO: ensure consistency with IARPA?
-# https://smartgitlab.com/TE/annotations/-/wikis/Annotation-Status-Types
-# https://smartgitlab.com/TE/metrics-and-test-framework/-/blob/main/iarpa_smart_metrics/evaluation.py#L1205
-# NOTE: A "Status" is not a category.
-# It indicates what sort of annotation detail is available.
+"""
+Status Data Info
+================
+
+The following is a long-form table, where list-items are rows and keys are
+columns to describe how to interpret IARPA annotation status labels in
+different cases. More information on status labels can be found in
+[TEAnnotStatus]_ and in our internal fork [KWAnnotStatus]_.
+
+
+Column Info:
+    * status:
+        the name of the site status label
+
+    * color:
+        what color to use for this status in visualizations. These are
+        mostly taken from [EvalMetricColors]_, but in cases where they are
+        undefined we make them up.
+
+    * kwcoco_catname:
+        what category to map this status to in the kwcoco dataset (and thus
+        what will be learned), Note: a status is different than a phase label,
+        and annotations with phase labels may overwrite the kwcoco category
+        defined here. This is used in geowatch reproject.
+
+    * positive_match_confusion
+        This is the label the truth is given when it has some match in our set
+        of positive predictions.  Denote what type of confusion a truth status
+        incurs when it is matched.
+
+
+The following code prints a concice version of this table and shows a legend
+with colors.
+
+.. code:: python
+
+    from watch.heuristics import *  # NOQA
+    import pandas as pd
+    import rich
+    df = pd.DataFrame(HUERISTIC_STATUS_DATA)
+    rich.print(df.to_string())
+
+    import kwplot
+    kwplot.autompl()
+    status_to_color = {r['status']: r['color'] for r in HUERISTIC_STATUS_DATA}
+    img = kwplot.make_legend_img(status_to_color, dpi=300)
+    kwplot.imshow(img, fnum=1)
+
+
+References
+----------
+.. [TEAnnotStatus] https://smartgitlab.com/TE/annotations/-/wikis/Annotation-Status-Types
+.. [KWAnnotStatus] https://gitlab.kitware.com/smart/annotations-wiki/-/blob/main/Annotation-Status-Types.md
+.. [EvalMetricColors] https://smartgitlab.com/TE/metrics-and-test-framework/-/blob/main/iarpa_smart_metrics/evaluation.py#L1205
+
+"""
 HUERISTIC_STATUS_DATA = [
-    {'name': 'seen', 'color': 'cyan'},
-    {'name': 'train', 'color': 'cyan'},
+    ### Misc Rows
+    {
+        'status': 'seen',
+        'color': 'cyan',
+        'kwcoco_catname': None,
+        'positive_match_confusion': 'gt_seen',
+    },
+    {
+        'status': 'train',
+        'color': 'cyan',
+        'kwcoco_catname': None,
+        'positive_match_confusion': 'gt_seen',
+    },
 
-    {'name': 'ignore', 'color': 'lightsalmon'},
+    ### Ignore Rows
+    {
+        'status': 'ignore',
+        'color': 'lightsalmon',
+        'kwcoco_catname': 'ignore',
+        'positive_match_confusion': 'gt_ignore',
+    },
 
+    ### Negative Rows
     # Note: 'colors for these status labels are undefined, using neutral gray
-    {'name': 'negative', 'color': 'gray'},
-    {'name': 'negative_unbounded', 'color': 'gray'},
+    {
+        'status': 'negative',
+        'color': 'gray',
+        'kwcoco_catname': 'negative',
+        'positive_match_confusion': 'gt_false_pos',
+    },
+    {
+        'status': 'negative_unbounded',
+        'color': 'gray',
+        'kwcoco_catname': 'negative',
+        'positive_match_confusion': 'gt_false_pos',
+    },
 
-    {'name': 'positive_excluded', 'color': 'gray'},
+    ### Positive Rows
+    {
+        'status': 'positive_annotated',
+        'color': 'black',
+        # Requires a category phase label, do not use status to map
+        'kwcoco_catname': None,
+        'positive_match_confusion': 'gt_true_pos',
+    },
+    {
+        'status': 'positive_annotated_static',
+        'color': 'black',
+        # Requires a category phase label, do not use status to map
+        'kwcoco_catname': None,
+        'positive_match_confusion': 'gt_true_pos',
+    },
+    {
+        'status': 'positive_excluded',
+        'color': 'gray',
+        # This is positive, but is not "big" enough
+        'kwcoco_catname': 'ignore',
+        'positive_match_confusion': 'gt_false_pos',
+    },
+    {
+        'status': 'positive_partial',
+        'color': 'black',
+        'kwcoco_catname': 'positive',
+        'positive_match_confusion': 'gt_true_pos',
+    },
+    {
+        'status': 'positive_pending',
+        'color': 'black',
+        'kwcoco_catname': 'positive',
+        'positive_match_confusion': 'gt_true_pos',
+    },
 
-    {'name': 'positive_annotated', 'color': 'black'},
-    {'name': 'positive_annotated_static', 'color': 'black'},
-    {'name': 'positive_partial', 'color': 'black'},
-    {'name': 'positive_pending', 'color': 'black'},
+    {
+        'status': 'positive_unbounded',
+        'color': 'darkviolet',
+        'kwcoco_catname': 'positive',   # Start or end date might not be defined
+        'positive_match_confusion': 'gt_positive_unbounded',
+    },
 
-    {'name': 'positive_unbounded', 'color': 'darkviolet'},
+    ### Transcient Rows
+    {
+        'status': 'transient_positive',
+        'color': 'steelblue',
+        'kwcoco_catname': 'transient',
+    },
+    {
+        'status': 'transient_negative',
+        'color': 'rust',
+        'kwcoco_catname': 'negative',
+    },
+    {
+        'status': 'transient_excluded',
+        'kwcoco_catname': 'ignore',
+        'color': 'lightsalmon',
+    },
+    {
+        'status': 'transient_ignore',
+        'kwcoco_catname': 'ignore',
+        'color': 'lightsalmon',
+    },
+    {
+        'status': 'transient_pending',
+        'kwcoco_catname': 'ignore',
+        'color': 'lightsalmon',
+    },
 
-    # TODO? Add alias of pending for "positive_pending"? For QFabric?
+    ### Prediction Rows
 
-    {'name': 'system_confirmed', 'color': 'kitware_blue'},
+    # TODO? Add alias of pending for "positive_pending"? For QFabric?
+    {
+        'status': 'system_confirmed',
+        'color': 'kitware_blue'
+    },
 ]
 
+# Backwards compat
+for row in HUERISTIC_STATUS_DATA:
+    row['name'] = row['status']
+
+
+# Convinience mappings used in reproject annotations
+PHASE_STATUS_TO_KWCOCO_CATNAME = {
+    row['name']: row['kwcoco_catname'] for row in HUERISTIC_STATUS_DATA
+    if 'kwcoco_catname' in row
+}
 
+# TODO: delete if the above longform table works well.
 # "Positive Match Confusion" is the label the truth is given when it has some
 # match in our set of positive predictions.  Denote what type of confusion a
 # truth status incurs when it is matched.
-PHASE_STATUS_TO_MATCHED_CONFUSION = {
-    'seen'                      : 'gt_seen',
-    'train'                     : 'gt_seen',
+# PHASE_STATUS_TO_MATCHED_CONFUSION = {
+#     'seen'                      : 'gt_seen',
+#     'train'                     : 'gt_seen',
 
-    'ignore'                    : 'gt_ignore',
+#     'ignore'                    : 'gt_ignore',
 
-    'negative'                  : 'gt_false_pos',
-    'negative_unbounded'        : 'gt_false_pos',
+#     'negative'                  : 'gt_false_pos',
+#     'negative_unbounded'        : 'gt_false_pos',
 
-    'positive_excluded'         : 'gt_false_pos',
+#     'positive_excluded'         : 'gt_false_pos',
 
-    'positive_annotated'        : 'gt_true_pos',
-    'positive_annotated_static' : 'gt_true_pos',
-    'positive_partial'          : 'gt_true_pos',
-    'positive_pending'          : 'gt_true_pos',
+#     'positive_annotated'        : 'gt_true_pos',
+#     'positive_annotated_static' : 'gt_true_pos',
+#     'positive_partial'          : 'gt_true_pos',
+#     'positive_pending'          : 'gt_true_pos',
 
-    'positive_unbounded'        : 'gt_positive_unbounded',
+#     'positive_unbounded'        : 'gt_positive_unbounded',
 
-}
+# }
 
 # Mapping of annotation status to the kwcoco category name
 # Used in project annotations
-PHASE_STATUS_TO_KWCOCO_CATNAME = {
-    'seen'                     : None,
-    'train'                    : None,
-
-    'ignore'                    : 'ignore',
+# PHASE_STATUS_TO_KWCOCO_CATNAME = {
+#     'seen'                     : None,
+#     'train'                    : None,
+
+#     'ignore'                    : 'ignore',
+
+#     'negative'                  : 'negative',
+#     'negative_unbounded'        : 'negative',
+
+#     'positive_annotated'        : None,  # This must have a category already do not map
+#     'positive_annotated_static' : None,  # This must have a category already do not map
+#     'positive_excluded'         : 'ignore',  # This is positive, but is not "big" enough
+#     'positive_partial'          : 'positive',  # Does not have phase labels
+#     'positive_pending'          : 'positive',  # Does not have phase labels
 
-    'negative'                  : 'negative',
-    'negative_unbounded'        : 'negative',
-
-    'positive_annotated'        : None,  # This must have a category already do not map
-    'positive_annotated_static' : None,  # This must have a category already do not map
-    'positive_excluded'         : 'ignore',  # This is positive, but is not "big" enough
-    'positive_partial'          : 'positive',  # Does not have phase labels
-    'positive_pending'          : 'positive',  # Does not have phase labels
-
-    'positive_unbounded'        : 'positive',  # Start or end date might not be defined
-}
+#     'positive_unbounded'        : 'positive',  # Start or end date might not be defined
+# }
 
-IARPA_STATUS_TO_INFO = {row['name']: row for row in HUERISTIC_STATUS_DATA}
+IARPA_STATUS_TO_INFO = {row['status']: row for row in HUERISTIC_STATUS_DATA}
 
 # update HUERISTIC_STATUS_DATA
-for name, row in IARPA_STATUS_TO_INFO.items():
-    if name in PHASE_STATUS_TO_KWCOCO_CATNAME:
-        row['kwcoco_catname'] = PHASE_STATUS_TO_KWCOCO_CATNAME[name]
-
-for name, row in IARPA_STATUS_TO_INFO.items():
-    if name in PHASE_STATUS_TO_MATCHED_CONFUSION:
-        row['positive_match_confusion'] = PHASE_STATUS_TO_MATCHED_CONFUSION[name]
+# for status, row in IARPA_STATUS_TO_INFO.items():
+#     if status in PHASE_STATUS_TO_KWCOCO_CATNAME:
+#         row['kwcoco_catname'] = PHASE_STATUS_TO_KWCOCO_CATNAME[status]
+
+# for status, row in IARPA_STATUS_TO_INFO.items():
+#     if status in PHASE_STATUS_TO_MATCHED_CONFUSION:
+#         row['positive_match_confusion'] = PHASE_STATUS_TO_MATCHED_CONFUSION[status]
 
 
 if 0:
     import pandas as pd
     print(pd.DataFrame(HUERISTIC_STATUS_DATA).to_string())
 
 
@@ -821,10 +966,10 @@
 # Mapping from our sensor names to the official T&E sensor names
 TE_SENSOR_NAMES = {
     'WV': 'WorldView',
     'S2': 'Sentinel-2',
     'LE': 'Landsat 7',
     'LC': 'Landsat 8',
     'L8': 'Landsat 8',
-    'WV1': 'WorldView 1',
+    'WV1': 'WorldView',
     'PD': 'Planet',
 }
```

### Comparing `geowatch-0.6.3/watch/mlops/__main__.py` & `geowatch-0.6.6/watch/mlops/__main__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/mlops/_notebook.py` & `geowatch-0.6.6/watch/mlops/_notebook.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 
 
 def _debug_roi_issue():
     import watch
     from watch.mlops.aggregate import AggregateLoader
     expt_dvc_dpath = watch.find_dvc_dpath(tags='phase2_expt', hardware='auto')
     loader = AggregateLoader(
-        pipeline='bas_building_vali',
+        pipeline='bas_depth_vali',
+        # pipeline='bas_building_vali',
         target=[
-            expt_dvc_dpath / '_toothbrush_split6_landcover_MeanYear10GSD-V2',
+            expt_dvc_dpath / '_mlops_test_depth_pcd',
+            # expt_dvc_dpath / '_toothbrush_split6_landcover_MeanYear10GSD-V2',
         ])
     eval_type_to_aggregator = loader.coerce_aggregators()
     pxl_agg = eval_type_to_aggregator['bas_pxl_eval']
     poly_agg = eval_type_to_aggregator['bas_poly_eval']
     sv_poly_agg = eval_type_to_aggregator['sv_poly_eval']
 
     # poly_agg.build_macro_tables(rois)
@@ -27,15 +29,15 @@
     print(ub.urepr(ub.udict(sv_poly_agg.macro_compatible).map_values(len)))
     print(ub.urepr(ub.udict(poly_agg.macro_compatible).map_values(len)))
 
     agg = sv_poly_agg
     # rois = 'KR_R001,KR_R002,CH_R001,NZ_R001,BR_R002'.split(',')
     # rois = 'KR_R001,KR_R002,CH_R001,NZ_R001,BR_R002,AE_R001'.split(',')
     rois = 'KR_R002,CH_R001,NZ_R001'.split(',')
-    # rois = ['KR_R002']
+    rois = ['KR_R002']
     # agg.build_macro_tables(rois)
 
     flags = agg.table['params.sv_crop.crop_src_fpath'].isnull()
     subagg = agg.compress(~flags)
     subagg.build_macro_tables(rois)
     _ = subagg.report_best()
 
@@ -145,17 +147,36 @@
 
         out_dpath = ub.Path('./high-tpr')
         eval_links = (out_dpath / 'eval_links').ensuredir()
         for _, row in high_tpr_agg.table.iterrows():
             node_dpath = ub.Path(row['fpath']).parent
             link_fpath = eval_links / (row['region_id'] + '_' + node_dpath.name)
             ub.symlink(node_dpath, link_fpath)
-
             ...
 
+    if 0:
+        # Inspect one of the best ones.
+        ###
+        out_dpath = ub.Path('./chosen')
+        root_dpath = expt_dvc_dpath / '_toothbrush_split6_landcover_MeanYear10GSD-V2/'
+        out_dpath = root_dpath / '_custom'
+        max_id = macro['metrics.sv_poly_eval.bas_f1'].idxmax()
+        chosen_param_hashid = macro.loc[max_id]['param_hashid']
+
+        chosen_agg = agg.filterto(param_hashids=[chosen_param_hashid])
+        _ = chosen_agg.report_best()
+        print(ub.repr2(chosen_agg.table['fpath'].tolist()))
+        eval_links = (out_dpath / 'eval_links').ensuredir()
+        for _, row in chosen_agg.table.iterrows():
+            node_dpath = ub.Path(row['fpath']).parent
+            link_fpath = eval_links / (row['region_id'] + '_' + node_dpath.name)
+            ub.symlink(node_dpath, link_fpath)
+
+
+
     agg.table['resolved_params.sv_crop.src'].unique()
 
     bad_values['resolved_params.sv_crop.src'].unique()
     good_values['resolved_params.sv_crop.src'].unique()
 
     bad_values = agg.table[flags]
     good_values = agg.table[~flags]
```

### Comparing `geowatch-0.6.3/watch/mlops/aggregate.py` & `geowatch-0.6.6/watch/mlops/aggregate.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 from scriptconfig import DataConfig, Value
 
 try:
     from xdev import profile
 except ImportError:
     profile = ub.identity
 
+# import xdev
+# xdev.make_warnings_print_tracebacks()
+
 
 class AggregateLoader(DataConfig):
     """
     Just the part of the config related to loading
     """
 
     target = Value(None, help=ub.paragraph(
@@ -1383,16 +1386,19 @@
 
         # For each unique set of effective parameters compute a hashid
         param_cols = ub.oset(effective_params.columns).difference(agg.test_dset_cols)
         param_cols = list(param_cols - {'region_id', 'node'})
         hashids_v1 = pd.Series([None] * len(agg.index), index=agg.index.index)
         # hashids_v0 = pd.Series([None] * len(agg.index), index=agg.index.index)
         hashid_to_params = {}
+        try:
+            list(effective_params.groupby(param_cols, dropna=False))
+        except Exception:
+            effective_params = effective_params.applymap(lambda x: str(x) if isinstance(x, list) else x)
         for param_vals, group in effective_params.groupby(param_cols, dropna=False):
-
             # Further subdivide the group so each row only computes its hash
             # with the parameters that were included in its row
             for param_flags, subgroup in is_param_included.loc[group.index].groupby(param_cols, dropna=False):
                 valid_param_cols = list(ub.compress(param_cols, param_flags))
                 valid_param_vals = list(ub.compress(param_vals, param_flags))
                 unique_params = ub.dzip(valid_param_cols, valid_param_vals)
                 hashid = hash_param(unique_params, version=1)
```

### Comparing `geowatch-0.6.3/watch/mlops/aggregate_loader.py` & `geowatch-0.6.6/watch/mlops/aggregate_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -377,14 +377,19 @@
         fpath = node_dpath / 'pred_boxes.kwcoco.zip'
         flat_resolved = _generalized_process_flat_resolved(fpath, node_process_name, node_type)
 
     elif node_type in {'sv_dino_filter'}:
         node_process_name = 'watch.tasks.dino_detector.building_validator'
         fpath = node_dpath / 'out_site_manifest.json'
         flat_resolved = _generalized_process_flat_resolved(fpath, node_process_name, node_type)
+
+    elif node_type in {'sv_depth_filter'}:
+        node_process_name = 'watch.tasks.depth_pcd.score_tracks'
+        fpath = node_dpath / 'sv_depth_out_site_manifest.json'
+        flat_resolved = _generalized_process_flat_resolved(fpath, node_process_name, node_type)
     else:
         raise NotImplementedError(node_type)
 
     predecessor_dpath = node_dpath / '.pred'
     for predecessor_node_type_dpath in predecessor_dpath.glob('*'):
         # predecessor_node_type = predecessor_node_type_dpath.name
         for predecessor_node_dpath in predecessor_node_type_dpath.glob('*'):
```

### Comparing `geowatch-0.6.3/watch/mlops/confusion_visualization.py` & `geowatch-0.6.6/watch/mlops/confusion_visualization.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/mlops/confusor_analysis.py` & `geowatch-0.6.6/watch/mlops/confusor_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,31 @@
 
 def main(cmdline=1, **kwargs):
     """
     CommandLine:
         xdoctest -m /home/joncrall/code/watch/watch/mlops/confusor_analysis.py main
         HAS_DVC=1 xdoctest -m watch.mlops.confusor_analysis main:0
 
+    Ignore:
+        from ubelt import Path
+        kwargs = {
+        'detections_fpath' : '/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_toothbrush_split6_landcover_MeanYear10GSD-V2/_custom/eval_links/KR_R002_sv_poly_eval_id_e865e066/KR_R002/overall/bas/detections_tau=0.2_rho=0.5_min_area=0.csv',
+        'proposals_fpath'  : '/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_toothbrush_split6_landcover_MeanYear10GSD-V2/_custom/eval_links/KR_R002_sv_poly_eval_id_e865e066/KR_R002/overall/bas/proposals_tau=0.2_rho=0.5_min_area=0.csv',
+        'src_kwcoco'       :
+            '/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_toothbrush_split6_landcover_MeanYear10GSD-V2/_custom/eval_links/KR_R002_sv_poly_eval_id_e865e066/.pred/sv_dino_filter/sv_dino_filter_id_32928a74/.pred/sv_dino_boxes/sv_dino_boxes_id_8de62349/.pred/sv_crop/sv_crop_id_64ea2fe6/.pred/bas_poly/bas_poly_id_efa920a0//.pred/bas_pxl/bas_pxl_id_fe488803//pred.kwcoco.zip',
+            'dst_kwcoco'       : '/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_toothbrush_split6_landcover_MeanYear10GSD-V2/_custom/eval_links/KR_R002_sv_poly_eval_id_e865e066/analysis/confusion_analysis/bas_confusion.kwcoco.zip',
+            'pred_sites'       : '/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_toothbrush_split6_landcover_MeanYear10GSD-V2/_custom/eval_links/KR_R002_sv_poly_eval_id_e865e066/.pred/sv_dino_filter/sv_dino_filter_id_32928a74/out_sites',
+            'bas_metric_dpath' : Path('/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_toothbrush_split6_landcover_MeanYear10GSD-V2/_custom/eval_links/KR_R002_sv_poly_eval_id_e865e066/KR_R002/overall/bas'),
+            'region_id'        : 'KR_R002',
+            'true_site_dpath'  : Path('/home/joncrall/remote/toothbrush/data/dvc-repos/smart_data_dvc-ssd/annotations/drop6/site_models'),
+            'true_region_dpath': Path('/home/joncrall/remote/toothbrush/data/dvc-repos/smart_data_dvc-ssd/annotations/drop6/region_models'),
+            'performer_id'     : 'kit',
+            'out_dpath'        : Path('/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_toothbrush_split6_landcover_MeanYear10GSD-V2/_custom/eval_links/KR_R002_sv_poly_eval_id_e865e066/analysis/confusion_analysis'),
+            }
+
     Example:
         >>> # xdoctest: +REQUIRES(env:HAS_DVC)
         >>> from watch.mlops.confusor_analysis import *  # NOQA
         >>> import watch
         >>> data_dvc_dpath = watch.find_dvc_dpath(tags='phase2_data', hardware='auto')
         >>> region_id = 'NZ_R001'
         >>> true_site_dpath = data_dvc_dpath / 'annotations/drop6/site_models'
@@ -105,14 +122,19 @@
     config.proposals_fpath = ub.Path(config.proposals_fpath)
     assert config.proposals_fpath.exists()
     assert config.detections_fpath.exists()
 
     assign1 = pd.read_csv(config.detections_fpath)
     assign2 = pd.read_csv(config.proposals_fpath)
 
+    rich.print(assign1)
+    rich.print(assign2)
+    rich.print(f'{len(assign1)=}')
+    rich.print(f'{len(assign2)=}')
+
     needs_recompute = any('_seq_' in m or m.startswith('seq_') for m in assign2['site model'] if m)
     assert not needs_recompute
 
     def fix_site_id(site_id):
         # Hack because idk why the metrics code does this.
         if site_id.startswith('_'):
             site_id = region_id + site_id
@@ -192,55 +214,57 @@
     """
 
     # Add the confusion info as misc data in new site files and reproject them
     # onto the truth for visualization.
     # pred_sites_fpath = poly_pred_dpath / 'sites_manifest.json'
     # assert pred_sites_fpath.exists()
     # pred_site_fpaths = list(util_gis.coerce_geojson_paths(pred_sites_fpath))
+    from watch.geoannots.geomodels import SiteModel, SiteModelCollection, RegionModel
+    import json
 
     rm_files = list(true_region_dpath.glob(region_id + '*.geojson'))
-
     gt_files = list(true_site_dpath.glob(region_id + '*.geojson'))
     sm_files = pred_site_fpaths
-    true_site_infos = list(util_gis.coerce_geojson_datas(gt_files, format='json'))
-    pred_site_infos = list(util_gis.coerce_geojson_datas(sm_files, format='json'))
-    orig_region_infos = list(util_gis.coerce_geojson_datas(rm_files, format='json'))
-    assert len(orig_region_infos) == 1
+
+    true_sites = SiteModelCollection(list(SiteModel.coerce_multiple(gt_files)))
+    pred_sites = SiteModelCollection(list(SiteModel.coerce_multiple(sm_files)))
+
+    orig_regions = list(RegionModel.coerce_multiple(rm_files))
+    if len(orig_regions) != 1:
+        raise AssertionError(f'Got {orig_regions=}')
 
     # Ensure all site data has misc-info
     # Ensure all data cast to site models
-    from watch.geoannots.geomodels import SiteModel, SiteModelCollection, RegionModel
-    import json
 
-    true_region_model = RegionModel(orig_region_infos[0]['data'])
+    true_region_model = orig_regions[0]
 
-    for info in it.chain(pred_site_infos, true_site_infos):
-        info['data'] = SiteModel(**info['data'])
-        info['data'].header['properties'].setdefault('misc_info', {})
+    for site in it.chain(pred_sites, true_sites):
+        site.header['properties'].setdefault('misc_info', {})
 
-    id_to_true_data = {ub.Path(d['fpath']).stem: d for d in true_site_infos}
-    id_to_pred_data = {ub.Path(d['fpath']).stem: d for d in pred_site_infos}
+    id_to_true_site = {s.site_id: s for s in true_sites}
+    id_to_pred_site = {s.site_id: s for s in pred_sites}
 
     # Add confusion metadata to predicted and truth models
     # https://gis.stackexchange.com/questions/346518/opening-geojson-style-properties-in-qgis
     for row in true_confusion_rows:
-        info = id_to_true_data[row['true_site_id']]
-        info['data'].header['properties']['misc_info']['confusion'] = row
+        site = id_to_true_site[row['true_site_id']]
+        site.header['properties']['misc_info']['confusion'] = row
     for row in pred_confusion_rows:
-        info = id_to_pred_data[row['pred_site_id']]
-        info['data'].header['properties']['misc_info']['confusion'] = row
-
-    pred_sites = SiteModelCollection([d['data'] for d in pred_site_infos])
-    true_sites = SiteModelCollection([d['data'] for d in true_site_infos])
+        site = id_to_pred_site[row['pred_site_id']]
+        site.header['properties']['misc_info']['confusion'] = row
 
     VALIDATE = 1
     if VALIDATE:
         all_models = SiteModelCollection(pred_sites + true_sites)
         all_models.fixup()
-        all_models.validate(workers=8)
+        all_models.validate(workers=0)
+        # for sm in all_models:
+        #     assert sm.header['geometry']['type'] == 'Polygon'
+        #     sm.validate()
+        # ...
 
     pred_region_model = pred_sites.as_region_model(region=true_region_model.header)
     pred_df = pred_region_model.pandas_summaries()
     true_df = true_region_model.pandas_summaries()
     idx1_to_idx2 = util_gis.geopandas_pairwise_overlaps(pred_df, true_df)
 
     # Find predicted annotations that have no truth overlap
@@ -251,21 +275,21 @@
     for true_site in true_sites:
         misc = true_site.header['properties']['misc_info']
         if misc['confusion']['type'] in 'gt_false_neg':
             hard_positive_site_ids.append(true_site.header['properties']['site_id'])
 
     hard_negative_sites = []
     for site_id in cand_df['site_id']:
-        pred_site = id_to_pred_data[site_id]['data']
+        pred_site = id_to_pred_site[site_id]
         misc = pred_site.header['properties']['misc_info']
         if misc['confusion']['type'] in 'sm_completely_wrong':
             hard_negative_sites.append(pred_site.deepcopy())
 
     orig_site_num = int(true_df['site_id'].max().split('_')[-1])
-    base_site_num = max(900, orig_site_num)
+    base_site_num = max(700, orig_site_num)
     for num, hard_neg in enumerate(hard_negative_sites, start=base_site_num):
         header_prop = hard_neg.header['properties']
         header_prop['site_id'] = region_id + f'_{num:04d}'
         header_prop['status'] = 'negative'
         header_prop['model_content'] = 'annotation'
         header_prop['misc_info'].pop('confusion', None)
         header_prop['misc_info']['kwcoco'] = {'weight': 1.5}
@@ -314,21 +338,21 @@
         text = json.dumps(new_site, indent='    ')
         fpath.write_text(text)
 
     # Dump confusion categorized site models to disk
     cfsn_dpath = config.out_dpath / 'confusion_sites'
     true_cfsn_dpath = (cfsn_dpath / 'true').ensuredir()
     pred_cfsn_dpath = (cfsn_dpath / 'pred').ensuredir()
-    for pred_site_id, pred_site in id_to_pred_data.items():
+    for pred_site_id, pred_site in id_to_pred_site.items():
         fpath = pred_cfsn_dpath / (pred_site_id + '.geojson')
-        text = json.dumps(pred_site['data'], indent='    ')
+        text = json.dumps(pred_site, indent='    ')
         fpath.write_text(text)
-    for true_site_id, true_site in id_to_true_data.items():
+    for true_site_id, true_site in id_to_true_site.items():
         fpath = true_cfsn_dpath / (true_site_id + '.geojson')
-        text = json.dumps(true_site['data'], indent='    ')
+        text = json.dumps(true_site, indent='    ')
         fpath.write_text(text)
 
     # Need to build site summaries from site models.
 
     # Write a new "enriched truth" file that reweights false negatives add
     # false positive as hard negatives.
 
@@ -341,32 +365,26 @@
             dst=new_coco_fpath,
             site_models=enriched_sites_dpath,
             region_models=enriched_region_dpath,
             workers=2,
         )
         reproject_annotations.main(cmdline=0, **common_kwargs)
 
-        if 0:
+        if 1:
             # Project confusion site models onto kwcoco for visualization
             import kwcoco
             from watch.cli import reproject_annotations
             src_dset = kwcoco.CocoDataset(config.src_kwcoco)
             dst_dset = src_dset.copy()
             dst_dset.fpath = config.dst_kwcoco
             dst_dset.clear_annotations()
-            true_site_infos2 = list(util_gis.coerce_geojson_datas(
-                id_to_true_data.values(), format='dataframe', allow_raw=True))
-            pred_site_infos2 = list(util_gis.coerce_geojson_datas(
-                id_to_pred_data.values(), format='dataframe', allow_raw=True))
-
-            for info in pred_site_infos2:
-                site_df = info['data']
+            true_site_infos2 = [s.pandas() for s in id_to_true_site.values()]
+            pred_site_infos2 = [s.pandas() for s in id_to_pred_site.values()]
 
-            for info in true_site_infos2:
-                site_df = info['data']
+            for site_df in true_site_infos2:
                 reproject_annotations.validate_site_dataframe(site_df)
 
             dst_dset.clear_annotations()
             common_kwargs = ub.udict(
                 clear_existing=False,
                 src=dst_dset,
                 dst='return',
@@ -396,15 +414,15 @@
             dst_dset = reproject_annotations.main(cmdline=0, **pred_kwargs)
             repr3 = str(dst_dset.annots())
             print(f'repr1={repr1}')
             print(f'repr2={repr2}')
             print(f'repr3={repr3}')
 
             set(dst_dset.annots().lookup('role', None))
-            set([x['role'] for x in dst_dset.annots().lookup('misc_info', None)])
+            set([x.get('role', None) for x in dst_dset.annots().lookup('misc_info', None)])
             # dst_dset.annots().take([0, 1, 2])
             viz_dpath = cfsn_dpath
             summary_visualization(dst_dset, viz_dpath)
             rich.print(f'Viz Dpath: [link={viz_dpath}]{viz_dpath}[/link]')
 
 
 def summary_visualization(dst_dset, viz_dpath):
@@ -492,21 +510,25 @@
 
             track_summaries = []
             from shapely.ops import unary_union
             for (role, tid), groupx in zip(unique_tids, groupxs):
                 track_dets = all_dets.take(groupx)
                 misc_info = track_dets.data['misc_info'][0]
                 row = misc_info.copy()
-                # row['role'] = role
+                row['role'] = role
+                row['confusion_color'] = row['confusion']['color']
                 # assert row['role'] == role
                 sh_poly = unary_union([p.to_shapely() for p in track_dets.data['segmentations']])
                 kw_poly = kwimage.MultiPolygon.from_shapely(sh_poly)
                 row['poly'] = kw_poly
                 track_summaries.append(row)
 
+            role_to_summary = ub.udict(ub.group_items(track_summaries, key=lambda x: x.get('role', None)))
+            print(ub.udict(role_to_summary).map_values(len))
+
             # canvas = kwplot.make_heatmask(util_kwimage.exactly_1channel(mean_heatmap), cmap='magma')[:, :, 0:3]
 
             old_canvas = kwimage.normalize_intensity(oldest_img, axis=2)
             new_canvas = kwimage.normalize_intensity(newest_img, axis=2)
 
             current = running.current()
             mean_heatmap = current['mean']
@@ -533,27 +555,24 @@
                 'avg': {
                     'true': canvas.copy(),
                     'pred': canvas.copy(),
                     'cfsn': canvas.copy(),
                 },
             }
 
-            role_to_summary = ub.udict(ub.group_items(track_summaries, key=lambda x: x['role']))
-            print(ub.udict(role_to_summary).map_values(len))
-
             alpha = 0.6
 
-            for row in ub.ProgIter(role_to_summary['true_confusion']):
+            for row in ub.ProgIter(role_to_summary.get('true_confusion', [])):
                 for k1, v1 in canvases.items():
                     v1['true'] = row['poly'].draw_on(v1['true'], fill=False, edgecolor=row['confusion_color'], alpha=alpha)
                     v1['cfsn'] = row['poly'].draw_on(v1['cfsn'], fill=False, edgecolor=row['confusion_color'], alpha=alpha)
                 # row['poly'].draw_on(canvas_true, fill=False, edgecolor=row['confusion_color'])
                 # row['poly'].draw_on(canvas_cfsn, fill=False, edgecolor=row['confusion_color'])
 
-            for row in ub.ProgIter(role_to_summary['pred_confusion']):
+            for row in ub.ProgIter(role_to_summary.get('pred_confusion', [])):
                 for k1, v1 in canvases.items():
                     v1['pred'] = row['poly'].draw_on(v1['pred'], fill=False, edgecolor=row['confusion_color'], alpha=alpha)
                     v1['cfsn'] = row['poly'].draw_on(v1['cfsn'], fill=False, edgecolor=row['confusion_color'], alpha=alpha)
                 # row['poly'].draw_on(canvas_pred, fill=False, edgecolor=row['confusion_color'])
                 # row['poly'].draw_on(canvas_cfsn, fill=False, edgecolor=row['confusion_color'])
 
             for k1, v1 in canvases.items():
```

### Comparing `geowatch-0.6.3/watch/mlops/manager.py` & `geowatch-0.6.6/watch/mlops/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,28 @@
     python -m watch.mlops.manager "status" --dataset_codes Drop4-SC
 
     python -m watch.mlops.manager "list" --dataset_codes Drop4-BAS
     python -m watch.mlops.manager "list" --dataset_codes Aligned-Drop4-2022-08-08-TA1-S2-WV-PD-ACC
     python -m watch.mlops.manager "list" --dataset_codes Drop6 Drop4-BAS
     python -m watch.mlops.manager "list" --dataset_codes Drop6-MeanYear10GSD
     python -m watch.mlops.manager "list" --dataset_codes Drop6 Drop6-MeanYear10GSD-V2
+    python -m watch.mlops.manager "list" --dataset_codes Drop6 Drop6-MedianSummer10GSD
 
     python -m watch.mlops.manager "push packages" --dataset_codes Drop6-MeanYear10GSD --yes
     python -m watch.mlops.manager "push packages" --dataset_codes Drop6-MeanYear10GSD-V2 --yes
+    python -m watch.mlops.manager "push packages" --dataset_codes Drop6-MedianSummer10GSD --yes
+    python -m watch.mlops.manager "push packages" --dataset_codes Drop6-NoWinterMedian10GSD --yes
 
     python -m watch.mlops.manager "status" --dataset_codes Drop6-MeanYear10GSD-V2
     python -m watch.mlops.manager "pull packages" --dataset_codes Drop6-MeanYear10GSD --yes
     python -m watch.mlops.manager "pull packages" --dataset_codes Drop6-MeanYear10GSD-V2 --yes
+    python -m watch.mlops.manager "pull packages" --dataset_codes Drop6-MedianSummer10GSD --yes
+    python -m watch.mlops.manager "pull packages" --dataset_codes Drop6-NoWinterMedian10GSD --yes
+
+    python -m watch.mlops.manager "pull packages" --dataset_codes Drop6-MeanYear10GSD-V2 --yes
 
     # On training machine
     python -m watch.mlops.manager "push packages" --dataset_codes Drop6
     python -m watch.mlops.manager "push packages" --dataset_codes "Aligned-Drop4-2022-08-08-TA1-S2-WV-PD-ACC"
 
     # On testing machine
     python -m watch.mlops.manager "pull packages" --dataset_codes Drop6
@@ -157,24 +164,26 @@
     # if config['dataset_codes'] is None:
     #     dataset_codes = heuristics.DATASET_CODES
     # else:
     dataset_codes = config['dataset_codes']
 
     if config['expt_dvc_dpath'] == 'auto':
         from watch import heuristics
-        config['expt_dvc_dpath'] = heuristics.auto_expt_dvc()
+        expt_dvc_dpath = heuristics.auto_expt_dvc()
+        config['expt_dvc_dpath'] = expt_dvc_dpath
 
     expt_dvc_dpath = config['expt_dvc_dpath']
+    print('expt_dvc_dpath = {}'.format(ub.urepr(expt_dvc_dpath, nl=1)))
 
     manager = DVCExptManager(
         expt_dvc_dpath, dvc_remote=dvc_remote, dataset_codes=dataset_codes,
         model_pattern=config['model_pattern'])
 
     if 'pull' in actions:
-        manager.pull(targets)
+        manager.pull(targets, yes=config.yes)
 
     if 'add' in actions and 'packages' in targets:
         manager.add_packages(yes=config.yes)
 
     if 'push' in actions and 'packages' in targets:
         manager.push_packages(yes=config.yes)
```

### Comparing `geowatch-0.6.3/watch/mlops/old/expt_manager.py` & `geowatch-0.6.6/watch/mlops/old/expt_manager.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/mlops/old/expt_report.py` & `geowatch-0.6.6/watch/mlops/old/expt_report.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/mlops/old/expt_state.py` & `geowatch-0.6.6/watch/mlops/old/expt_state.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/mlops/old/old_pipeline_nodes.py` & `geowatch-0.6.6/watch/mlops/old/old_pipeline_nodes.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/mlops/old/old_plots.py` & `geowatch-0.6.6/watch/mlops/old/old_plots.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/mlops/old/pipeline_v1.py` & `geowatch-0.6.6/watch/mlops/old/pipeline_v1.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/mlops/old/plots.py` & `geowatch-0.6.6/watch/mlops/old/plots.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/mlops/pipeline_nodes.py` & `geowatch-0.6.6/watch/mlops/pipeline_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -849,21 +849,31 @@
                  resources=None,
                  in_paths=None,
                  out_paths=None,
                  group_dname=None,
                  #node_dname=None,
                  root_dpath=None,
                  config=None,
+                 node_dpath=None,  # overwrites configured node dapth
+                 group_dpath=None,  # overwrites configured node dapth
                  _overwrite_node_dpath=None,  # overwrites the configured node dpath
                  _overwrite_group_dpath=None,  # overwrites the configured group dpath
                  _no_outarg=False,
                  **aliases):
         if aliases:
             if 'command' in aliases:
                 executable = aliases['command']
+
+        if node_dpath is not None:
+            _overwrite_node_dpath = node_dpath
+        if group_dpath is not None:
+            _overwrite_group_dpath = group_dpath
+
+        del node_dpath
+        del group_dpath
         del aliases
 
         if name is None and executable is not None:
             name = 'unnamed_process_node_' + str(id(self))  # ub.hash_data(executable)[0:8]
 
         args = locals()
         fallbacks = {
@@ -1294,14 +1304,25 @@
         """
         if len(self.final_out_paths) == 0:
             # Can only cache if we know what output paths are
             return False
         # return all(self.out_paths.map_values(lambda p: p.exists()).values())
         return all(ub.Path(p).expand().exists() for p in self.final_out_paths.values())
 
+    @memoize_configured_property
+    @profile
+    def outputs_exist(self) -> bool:
+        """
+        Alias for does_exist
+
+        Check if all of the output paths that would be written by this node
+        already exists.
+        """
+        return self.does_exist
+
     def _raw_command(self):
         command = self.command
         if not isinstance(command, str):
             assert callable(command)
             command = command()
         return command
```

### Comparing `geowatch-0.6.3/watch/mlops/repackager.py` & `geowatch-0.6.6/watch/mlops/repackager.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/mlops/schedule_evaluation.py` & `geowatch-0.6.6/watch/mlops/schedule_evaluation.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/mlops/smart_global_helper.py` & `geowatch-0.6.6/watch/mlops/smart_global_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -517,14 +517,35 @@
                 'bas_pxl.chip_dims': '[196, 196]',
                 'bas_poly.thresh': 0.33,
                 'bas_poly.moving_window_size': 'None',
                 'bas_poly.min_area_square_meters': 7200.0,
                 'bas_poly.norm_ord': float('inf'),
                 'bas_poly.poly_merge_method': 'v2',
                 'task': 'BAS',
+            },
+
+            {
+                'delivery': 'Eval11',
+                'bas_pxl.package_fpath': 'models/fusion/Drop6-MeanYear10GSD-V2/packages/Drop6_TCombo1Year_BAS_10GSD_V2_landcover_split6_V47/Drop6_TCombo1Year_BAS_10GSD_V2_landcover_split6_V47_epoch47_step3026.pt',
+                'bas_pxl.chip_dims': '[196, 196]',
+                'bas_pxl.time_sampling': 'soft4',
+                'bas_pxl.tta_fliprot': 3,
+                'bas_pxl.tta_time': 3,
+                'bas_poly.thresh': 0.425,
+                'bas_poly.time_thresh': 0.8,
+                'bas_poly.inner_window_size': '1y',
+                'bas_poly.inner_agg_fn': 'mean',
+                'bas_poly.agg_fn': 'probs',
+                'bas_poly.moving_window_size': 'None',
+                'bas_poly.polygon_simplify_tolerance': 1,
+                'bas_poly.norm_ord': float('inf'),
+                'bas_poly.poly_merge_method': 'v2',
+                'bas_poly.min_area_square_meters': 7200.0,
+                'bas_poly.max_area_square_meters': 8000000.0,
+                'task': 'BAS',
             }
         ]
 
         ## SC
         # delivered_model_params += [
         #     {
         #         'name': 'Drop4_SC_RGB_scratch_V002_epoch=99-step=50300-v1.pt.pt',
```

### Comparing `geowatch-0.6.3/watch/mlops/smart_pipeline.py` & `geowatch-0.6.6/watch/mlops/smart_pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -702,14 +702,82 @@
     }
 
     out_paths = {
         'crop_dst_fpath': 'sv_crop.kwcoco.zip'
     }
 
 
+class SV_DepthFilter(ProcessNode):
+    """
+    Node for DZYNEs high res depth-based parallel change detector
+
+    Example:
+        >>> from watch.mlops import smart_pipeline
+        >>> self = node = smart_pipeline.SV_DepthFilter(root_dpath='/ROOT/DPATH/')
+        >>> node.configure({
+        >>>     'input_kwcoco': 'foo.kwcoco',
+        >>>     'input_region': 'region.geojson',
+        >>>     'input_sites': 'input_sites',
+        >>>     #'output_sites_dpath': 'I_WANT_OUT_SITES_HERE',
+        >>>     'output_region_fpath': 'I_WANT_OUT_REGIONS_HERE',
+        >>>     'output_site_manifest_fpath': 'I_WANT_SITE_MANIFESTS_HERE',
+        >>> })
+        >>> print('self.template_out_paths = {}'.format(ub.urepr(self.template_out_paths, nl=1)))
+        >>> print('self.final_out_paths = {}'.format(ub.urepr(self.final_out_paths, nl=1)))
+        >>> print(node.command())
+
+    Example:
+        >>> from watch.mlops import smart_pipeline
+        >>> self = node = smart_pipeline.SV_DepthFilter(node_dpath='/MY/OUPUT/DIR/')
+        >>> node.configure({
+        >>>     'input_kwcoco': 'foo.kwcoco',
+        >>>     'input_region': 'region.geojson',
+        >>>     'input_sites': 'sites/*.geojson',
+        >>>     'model_fpath': 'models/depth_pcd/basicModel2.h5',
+        >>> })
+        >>> print('self.template_out_paths = {}'.format(ub.urepr(self.template_out_paths, nl=1)))
+        >>> print('self.final_out_paths = {}'.format(ub.urepr(self.final_out_paths, nl=1)))
+        >>> print(node.command())
+    """
+    name = 'sv_depth_filter'
+    executable = 'python -m watch.tasks.depth_pcd.score_tracks'
+    group_dname = PREDICT_NAME
+
+    in_paths = {
+        'input_kwcoco',
+        'input_region',
+        'input_sites',
+    }
+    out_paths = {
+        'output_region_fpath': 'sv_depth_out_region.geojson',
+        'output_sites_dpath': 'sv_depth_out_sites',
+        'output_site_manifest_fpath': 'sv_depth_out_site_manifest.json',
+    }
+
+    algo_params = {
+        'threshold': 0.4,
+        'model_fpath': None,
+    }
+
+    @profile
+    def command(self):
+        # Not sure why final-config doesn't have everything
+        config = (ub.udict(self.final_config) | self.final_algo_config) | self.final_perf_config
+        config_argstr = self._make_argstr(config)
+        command = ub.codeblock(
+            r'''
+            {executable} \
+                {config_argstr}
+            ''').format(
+                executable=self.executable,
+                config_argstr=config_argstr,
+            )
+        return command
+
+
 class DinoBoxDetector(ProcessNode):
     """
     Used for both site cropping and validation-cropping
 
     Example:
         >>> node = DinoBoxDetector(root_dpath='/root/dpath/')
         >>> node.configure({
@@ -777,21 +845,21 @@
             ''').format(**fmtkw)
         return command
 
 
 # from watch.tasks.dino_detector import building_validator  # NOQA
 # ub.udict(building_validator.BuildingValidatorConfig.__default__)
 
-class DinoBuildingFilter(ProcessNode):
+class SV_DinoFilter(ProcessNode):
     """
     Used for both site cropping and validation-cropping
 
     Example:
         >>> from watch.mlops.smart_pipeline import *  # NOQA
-        >>> self = node = DinoBuildingFilter(root_dpath='/ROOT/DPATH/')
+        >>> self = node = SV_DinoFilter(root_dpath='/ROOT/DPATH/')
         >>> node.configure({
         >>>     'input_kwcoco': 'foo.kwcoco',
         >>>     'input_region': 'region.geojson',
         >>>     'input_sites': 'input_sites',
         >>>     #'output_sites_dpath': 'I_WANT_OUT_SITES_HERE',
         >>>     'output_region_fpath': 'I_WANT_OUT_REGIONS_HERE',
         >>>     'output_site_manifest_fpath': 'I_WANT_SITE_MANIFESTS_HERE',
@@ -913,15 +981,16 @@
             nodes['sc_poly_viz'],
         ),
     )
     return nodes
 
 
 def make_smart_pipeline_nodes(with_bas=True, building_validation=False,
-                              site_crops=True, with_sc=True):
+                              depth_validation=True, site_crops=True,
+                              with_sc=True):
     nodes = {}
 
     sc_input_region = None
     sc_input_kwcoco = None
     bas_input_kwcoco = None
 
     true_regions = None
@@ -940,37 +1009,48 @@
 
         # By default SC will use the same input as BAS
         sc_input_kwcoco = sc_input_kwcoco
 
         true_regions = nodes['bas_poly_eval'].inputs['true_region_dpath']
         true_sites = nodes['bas_poly_eval'].inputs['true_site_dpath']
 
-    if building_validation:
-        nodes['sv_crop'] = SV_Cropping()
+    with_sv = building_validation or depth_validation
 
+    if with_sv:
+        nodes['sv_crop'] = SV_Cropping()
         if bas_input_kwcoco is not None:
             bas_output_region.connect(nodes['sv_crop'].inputs['regions'])
             bas_input_kwcoco.connect(nodes['sv_crop'].inputs['crop_src_fpath'])
-
-        nodes['sv_dino_boxes'] = DinoBoxDetector()
-        nodes['sv_crop'].outputs['crop_dst_fpath'].connect(nodes['sv_dino_boxes'].inputs['coco_fpath'])
-
-        nodes['sv_dino_filter'] = DinoBuildingFilter()
-        nodes['sv_dino_boxes'].outputs['out_coco_fpath'].connect(nodes['sv_dino_filter'].inputs['input_kwcoco'])
-        bas_output_region.connect(nodes['sv_dino_filter'].inputs['input_region'])
-        bas_output_sites.connect(nodes['sv_dino_filter'].inputs['input_sites'])
-
-        # If we have a validation step, use those as inputs to SC instead
-        sv_output_region = nodes['sv_dino_filter'].outputs['output_region_fpath']
-        sv_output_sites = nodes['sv_dino_filter'].outputs['output_sites_dpath']
+        sv_output_kwcoco = nodes['sv_crop'].outputs['crop_dst_fpath']
+        sv_region = bas_output_region
+        sv_sites = bas_output_sites
+
+        if building_validation:
+            nodes['sv_dino_boxes'] = DinoBoxDetector()
+            nodes['sv_dino_filter'] = SV_DinoFilter()
+            sv_output_kwcoco.connect(nodes['sv_dino_boxes'].inputs['coco_fpath'])
+            nodes['sv_dino_boxes'].outputs['out_coco_fpath'].connect(nodes['sv_dino_filter'].inputs['input_kwcoco'])
+            sv_region.connect(nodes['sv_dino_filter'].inputs['input_region'])
+            sv_sites.connect(nodes['sv_dino_filter'].inputs['input_sites'])
+            sv_region = nodes['sv_dino_filter'].outputs['output_region_fpath']
+            sv_sites = nodes['sv_dino_filter'].outputs['output_sites_dpath']
+
+        if depth_validation:
+            nodes['sv_depth_filter'] = SV_DepthFilter()
+            sv_output_kwcoco.connect(nodes['sv_depth_filter'].inputs['input_kwcoco'])
+            sv_region.connect(nodes['sv_depth_filter'].inputs['input_region'])
+            sv_sites.connect(nodes['sv_depth_filter'].inputs['input_sites'])
+            sv_region = nodes['sv_depth_filter'].outputs['output_region_fpath']
+            sv_sites = nodes['sv_depth_filter'].outputs['output_sites_dpath']
 
         # Add an evaluation step after bas validation
         nodes['sv_poly_eval'] = PolygonEvaluation(name='sv_poly_eval')
-        sv_output_sites.connect(nodes['sv_poly_eval'].inputs['sites_fpath'])
-        sc_input_region = sv_output_region
+        sv_sites.connect(nodes['sv_poly_eval'].inputs['sites_fpath'])
+        # If we have a validation step, use those as inputs to SC
+        sc_input_region = sv_region
 
         if true_regions is not None:
             true_regions.connect(nodes['sv_poly_eval'].inputs['true_region_dpath'])
             true_sites.connect(nodes['sv_poly_eval'].inputs['true_site_dpath'])
 
     if site_crops:
         nodes['sc_crop'] = SC_Cropping()
@@ -1001,28 +1081,31 @@
     Get an unconfigured instance of the SMART pipeline
 
     CommandLine:
         xdoctest -m watch.mlops.smart_pipeline make_smart_pipeline
 
     Example:
         >>> from watch.mlops.smart_pipeline import *  # NOQA
-        >>> dag = make_smart_pipeline('bas_building_vali')
+        >>> dag = make_smart_pipeline('bas_depth_vali')
         >>> dag.print_graphs()
     """
     from watch.mlops.pipeline_nodes import PipelineDAG
     from functools import partial
     node_makers = {
         'joint_bas_sc': partial(make_smart_pipeline_nodes, site_crops=True),
         'joint_bas_sc_nocrop': partial(make_smart_pipeline_nodes, site_crops=False),
         'crop_sc': partial(make_smart_pipeline_nodes, with_bas=False, site_crops=True),
         'sc': sc_nodes,
         'bas': bas_nodes,
         'bas_building_vali': partial(make_smart_pipeline_nodes, with_bas=True,
                                      building_validation=True,
                                      site_crops=False, with_sc=False),
+        'bas_depth_vali': partial(make_smart_pipeline_nodes, with_bas=True,
+                                  depth_validation=True,
+                                  site_crops=False, with_sc=False),
     }
     make_nodes = node_makers[name]
     nodes = make_nodes()
     dag = PipelineDAG(nodes)
     dag.build_nx_graphs()
     return dag
```

### Comparing `geowatch-0.6.3/watch/mlops/smart_result_parser.py` & `geowatch-0.6.6/watch/mlops/smart_result_parser.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/monkey/_monkey_fbeta.py` & `geowatch-0.6.6/watch/monkey/_monkey_fbeta.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/monkey/monkey_albumentations.py` & `geowatch-0.6.6/watch/monkey/monkey_albumentations.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/monkey/monkey_lightning.py` & `geowatch-0.6.6/watch/monkey/monkey_lightning.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/monkey/monkey_torch.py` & `geowatch-0.6.6/watch/monkey/monkey_torch.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/monkey/monkey_torchmetrics.py` & `geowatch-0.6.6/watch/monkey/monkey_torchmetrics.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/rc/__init__.py` & `geowatch-0.6.6/watch/rc/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/rc/registry.py` & `geowatch-0.6.6/watch/rc/registry.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/stac/_notebook.py` & `geowatch-0.6.6/watch/stac/_notebook.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/stac/stac_search_builder.py` & `geowatch-0.6.6/watch/stac/stac_search_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         https://smartgitlab.com/TE/evaluations/-/wikis/Accenture-TA-1-Processing-Status
 """
 import os
 import ubelt as ub
 import scriptconfig as scfg
 
 
-class StacSearchBuilderConfig(scfg.Config):
+class StacSearchBuilderConfig(scfg.DataConfig):
     """
     Helper to create STAC search json queries
     """
     default = {
         'start_date': scfg.Value(None, help='iso starting date'),
         'end_date': scfg.Value(None, help='iso ending date'),
         'cloud_cover': scfg.Value(10, help='maximum cloud cover percentage'),
@@ -251,14 +251,24 @@
 # https://www.drivendata.org/competitions/143/tick-tick-bloom/page/650/#sentinel-2-1
 # https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2
 _PUBLIC_L2_PRODUCTS['planetarycomputer'] = {
     'collections': ['landsat-c2-l2', 'sentinel-2-l2a'],
     "endpoint": "https://planetarycomputer.microsoft.com/api/stac/v1",
 }
 
+_PUBLIC_L2_PRODUCTS['planetarycomputer_l8'] = {
+    'collections': ['landsat-c2-l2'],
+    "endpoint": "https://planetarycomputer.microsoft.com/api/stac/v1",
+}
+
+_PUBLIC_L2_PRODUCTS['planetarycomputer_s2'] = {
+    'collections': ['sentinel-2-l2a'],
+    "endpoint": "https://planetarycomputer.microsoft.com/api/stac/v1",
+}
+
 
 _PUBLIC_ARD_PRODUCTS = {
     # https://stacindex.org/catalogs/usgs-landsat-collection-2-api#/
     # Surface Reflectance
     'landsat-c2ard-sr': {
         # Note: AWS_REQUEST_PAYER='requester' is required to grab the data
         "collections": ["landsat-c2ard-sr"],
@@ -491,15 +501,16 @@
         >>>     'start_date': '2017-01-01',
         >>>     'end_date': '2020-01-01',
         >>>     'sensors': 'L2-S2',
         >>> }
         >>> main(cmdline=cmdline, **kwargs)
     """
     import json
-    config = StacSearchBuilderConfig(cmdline=cmdline, data=kwargs)
+    config = StacSearchBuilderConfig.cli(cmdline=cmdline, data=kwargs,
+                                         strict=True)
 
     search_json = build_search_json(**ub.compatible(config, build_search_json))
     text = json.dumps(search_json, indent='    ')
 
     if config['out_fpath'] is not None:
         out_fpath = ub.Path(config['out_fpath'])
         out_fpath.write_text(text)
```

### Comparing `geowatch-0.6.3/watch/stac/util_stac.py` & `geowatch-0.6.6/watch/stac/util_stac.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/__init__.py` & `geowatch-0.6.6/watch/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/cold/assemble_cold_result_kwcoco.py` & `geowatch-0.6.6/watch/tasks/cold/assemble_cold_result_kwcoco.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from datetime import datetime as datetime_cls
 import json
 import kwcoco
 import kwimage
 import scriptconfig as scfg
 import ubelt as ub
 import logging
-import shutil
 import gc
 try:
     from xdev import profile
 except ImportError:
     from ubelt import identity as profile
 
 logger = logging.getLogger(__name__)
@@ -78,20 +77,20 @@
         TEST_COLD=1 xdoctest -m watch.tasks.cold.assemble_cold_result_kwcoco assemble_main
 
     Example:
     >>> # xdoctest: +REQUIRES(env:TEST_COLD)
     >>> from watch.tasks.cold.assemble_cold_result_kwcoco import assemble_main
     >>> from watch.tasks.cold.assemble_cold_result_kwcoco import *
     >>> kwargs= dict(
-    >>>    stack_path = "/home/jws18003/data/dvc-repos/smart_data_dvc/Drop6/_pycold_combine/stacked/KR_R001/",
-    >>>    reccg_path = "/home/jws18003/data/dvc-repos/smart_data_dvc/Drop6/_pycold_combine/reccg/KR_R001/",
-    >>>    coco_fpath = ub.Path('/home/jws18003/data/dvc-repos/smart_data_dvc/Drop6/data_vali_split1_KR_R001.kwcoco.json'),
-    >>>    mod_coco_fpath = ub.Path('/home/jws18003/data/dvc-repos/smart_data_dvc/Drop6/_pycold_combine/test.json'),
-    >>>    meta_fpath = '/home/jws18003/data/dvc-repos/smart_data_dvc/Drop6/_pycold_combine/stacked/KR_R001/block_x9_y9/crop_20210807T010000Z_N37.643680E128.649453_N37.683356E128.734073_L8_0.json',
-    >>>    combined_coco_fpath = ub.Path('/home/jws18003/data/dvc-repos/smart_data_dvc/Drop6_MeanYear/data_vali_split1_KR_R001_MeanYear.kwcoco.json'),
+    >>>    stack_path = "/gpfs/scratchfs1/zhz18039/jws18003/new-repos/smart_data_dvc2/Drop6-MeanYear10GSD-V2/_pycold/stacked/KR_R001/",
+    >>>    reccg_path = "/gpfs/scratchfs1/zhz18039/jws18003/new-repos/smart_data_dvc2/Drop6-MeanYear10GSD-V2/_pycold/reccg/KR_R001/",
+    >>>    coco_fpath = ub.Path('/gpfs/scratchfs1/zhz18039/jws18003/new-repos/smart_data_dvc2/Drop6/imgonly-KR_R001.kwcoco.json'),
+    >>>    mod_coco_fpath = ub.Path('/gpfs/scratchfs1/zhz18039/jws18003/new-repos/smart_data_dvc2/Drop6/imgonly_KR_R001_cold.kwcoco.zip'),
+    >>>    meta_fpath = '/gpfs/scratchfs1/zhz18039/jws18003/new-repos/smart_data_dvc2/Drop6-MeanYear10GSD-V2/_pycold/stacked/KR_R001/block_x10_y1/crop_20140115T020000Z_N37.643680E128.649453_N37.683356E128.734073_L8_0.json',
+    >>>    combined_coco_fpath = ub.Path('/gpfs/scratchfs1/zhz18039/jws18003/new-repos/smart_data_dvc2/Drop6-MeanYear10GSD-V2/imgonly-KR_R001.kwcoco.zip'),
     >>>    coefs = 'cv,rmse,a0,a1,b1,c1',
     >>>    year_lowbound = None,
     >>>    year_highbound = None,
     >>>    coefs_bands = '0,1,2,3,4,5',
     >>>    timestamp = False,
     >>>    combine = True,
     >>>    sensors = 'L8',
@@ -181,16 +180,15 @@
     img_dates = []
     img_names = []
 
     # read metadata and
     for meta in meta_files:
         meta_config = json.loads((block_folder / meta).read_text())
         ordinal_date = meta_config['ordinal_date']
-        # img_name = meta_config['image_name'] + '.npy'
-        img_name = meta_config['image_name']
+        img_name = meta_config['image_name']  # + '.npy'
         img_dates.append(ordinal_date)
         img_names.append(img_name)
 
     if year_lowbound is None:
         year_low_ordinal = min(img_dates)
         year_lowbound = pd.Timestamp.fromordinal(year_low_ordinal).year
     else:
@@ -229,15 +227,14 @@
             coco_img_name = coco_image.img['name']
             timestamp_local = datetime_cls.fromtimestamp(ts, tz=tz)
             timestamp_utc = timestamp_local.astimezone(pytz.utc)
             ordinal = timestamp_utc.toordinal()
             ordinal_dates.append(ordinal)
             img_names.append(coco_img_name)
         ordinal_day_list = ordinal_dates
-
     else:
         # Get only the first ordinal date of each year
         first_ordinal_dates = []
         first_img_names = []
         last_year = None
         for ordinal_day, img_name in zip(img_dates, img_names):
             year = pd.Timestamp.fromordinal(ordinal_day).year
@@ -247,15 +244,14 @@
                 last_year = year
 
         ordinal_day_list = first_ordinal_dates
         img_names = first_img_names
 
     # assemble
     logger.info('Generating COLD output geotiff')
-
     if coefs is not None:
         day_iter = range(len(ordinal_day_list))
         if pman is not None:
             day_iter = pman.progiter(day_iter, total=len(ordinal_day_list))
         for day in day_iter:
             tmp_map_blocks = [np.load(
                 tmp_path / f'tmp_coefmap_block{x + 1}_{ordinal_day_list[day]}.npy')
@@ -295,69 +291,111 @@
 
             # for x in range(n_blocks):
                 # TODO: would be nice to have a structure that controls these
                 # name formats so we can use padded inter suffixes for nicer
                 # sorting, or nest files to keep folder sizes small
 
     # Remove tmp files
-    shutil.rmtree(tmp_path)
+    # shutil.rmtree(tmp_path)
 
     logger.info('Starting adding new asset to kwcoco json')
     if combine:
         output_coco_dset = combined_coco_dset
+        for image_id in output_coco_dset.images():
+            combined_coco_image: kwcoco.CocoImage = output_coco_dset.coco_image(image_id)
+            coco_image: kwcoco.CocoImage = coco_dset.coco_image(image_id)
+            image_name = coco_image.img['name']
+
+            asset_w = vid_w
+            asset_h = vid_h
+
+            for band_name in band_names:
+                for coef in coef_names:
+                    band = BAND_INFO[band_name]
+                    new_fpath = out_path / f'{image_name}_{band}_{method}_{coef}.tif'
+                    if new_fpath.exists():
+                        channels = kwcoco.ChannelSpec.coerce(f'{band}_{method}_{coef}')
+                        print('exist', new_fpath)
+                        # COLD output was wrote based on transform information of
+                        # coco_dset, so it aligned to a scaled video space.
+                        warp_img_from_vid = combined_coco_image.warp_img_from_vid
+
+                        if resolution is None:
+                            scale_asset_from_vid = (1., 1.)
+                        else:
+                            scale_asset_from_vid = combined_coco_image._scalefactor_for_resolution(
+                                space='video', resolution=resolution)
+                        warp_asset_from_vid = kwimage.Affine.scale(scale_asset_from_vid)
+                        warp_vid_from_asset = warp_asset_from_vid.inv()
+                        warp_img_from_asset = warp_img_from_vid @ warp_vid_from_asset
+
+                        # Use the CocoImage helper which will augment the coco dictionary with
+                        # your information.
+                        combined_coco_image.add_asset(
+                            file_name=new_fpath,
+                            channels=channels,
+                            width=asset_w,
+                            height=asset_h,
+                            warp_aux_to_img=warp_img_from_asset)
+                        print(f'Added to the asset {new_fpath}')
+                        logger.info(f'Added to the asset {new_fpath}')
     else:
         output_coco_dset = coco_dset
+        for image_id in output_coco_dset.images():
+            # Create a CocoImage object for each image.
+            coco_image: kwcoco.CocoImage = output_coco_dset.coco_image(image_id)
+            image_name = coco_image.img['name']
 
-    for image_id in output_coco_dset.images():
-        combined_coco_image: kwcoco.CocoImage = output_coco_dset.coco_image(image_id)
-        coco_image: kwcoco.CocoImage = output_coco_dset.coco_image(image_id)
-        image_name = coco_image.img['name']
-
-        asset_w = vid_w
-        asset_h = vid_h
-
-        for band_name in band_names:
-            for coef in coef_names:
-                band = BAND_INFO[band_name]
-                new_fpath = out_path / f'{image_name}_{band}_{method}_{coef}.tif'
-                if new_fpath.exists():
-                    channels = kwcoco.ChannelSpec.coerce(f'{band}_{method}_{coef}')
-
-                    # COLD output was wrote based on transform information of
-                    # coco_dset, so it aligned to a scaled video space.
-                    warp_img_from_vid = combined_coco_image.warp_img_from_vid
-
-                    if resolution is None:
-                        scale_asset_from_vid = (1., 1.)
-                    else:
-                        scale_asset_from_vid = combined_coco_image._scalefactor_for_resolution(
-                            space='video', resolution=resolution)
-                    warp_asset_from_vid = kwimage.Affine.scale(scale_asset_from_vid)
-                    warp_vid_from_asset = warp_asset_from_vid.inv()
-                    warp_img_from_asset = warp_img_from_vid @ warp_vid_from_asset
-
-                    # Use the CocoImage helper which will augment the coco dictionary with
-                    # your information.
-                    combined_coco_image.add_asset(
-                        file_name=new_fpath,
-                        channels=channels,
-                        width=asset_w,
-                        height=asset_h,
-                        warp_aux_to_img=warp_img_from_asset)
-                    logger.info(f'Added to the asset {new_fpath}')
+            asset_w = vid_w
+            asset_h = vid_h
+
+            for band_name in band_names:
+                for coef in coef_names:
+                    band = BAND_INFO[band_name]
+                    new_fpath = out_path / f'{image_name}_{band}_{method}_{coef}.tif'
+                    if new_fpath.exists():
+                        channels = kwcoco.ChannelSpec.coerce(f'{band}_{method}_{coef}')
+
+                        # COLD output was wrote based on transform information of
+                        # coco_dset, so it aligned to a scaled video space.
+                        warp_img_from_vid = coco_image.warp_img_from_vid
+
+                        if resolution is None:
+                            scale_asset_from_vid = (1., 1.)
+                        else:
+                            scale_asset_from_vid = coco_image._scalefactor_for_resolution(
+                                space='video', resolution=resolution)
+                        warp_asset_from_vid = kwimage.Affine.scale(scale_asset_from_vid)
+                        warp_vid_from_asset = warp_asset_from_vid.inv()
+                        warp_img_from_asset = warp_img_from_vid @ warp_vid_from_asset
+
+                        # Use the CocoImage helper which will augment the coco dictionary with
+                        # your information.
+                        print(new_fpath)
+                        coco_image.add_asset(os.fspath(new_fpath),
+                                                channels=channels, width=asset_w,
+                                                height=asset_h,
+                                                warp_aux_to_img=warp_img_from_asset)
+
+                        logger.info(f'Added to the asset {new_fpath}')
 
     if proc_context is not None:
         context_info = proc_context.stop()
         output_coco_dset.dataset['info'].append(context_info)
 
     # Write a modified kwcoco.json file
     logger.info(f'Writing kwcoco file to: {mod_coco_fpath}')
-    output_coco_dset.fpath = mod_coco_fpath
-    output_coco_dset._ensure_json_serializable()
-    output_coco_dset.dump()
+    if combine:
+        combined_coco_dset.fpath = mod_coco_fpath
+        combined_coco_dset._ensure_json_serializable()
+        combined_coco_dset.dump()
+    else:
+        coco_dset.fpath = mod_coco_fpath
+        coco_dset._ensure_json_serializable()
+        coco_dset.dump()
     logger.info(f'Finished writing kwcoco file to: {mod_coco_fpath}')
 
     gc.collect()
 
 
 @profile
 def get_gdal_transform(coco_dset, sensor_name, resolution=None):
```

### Comparing `geowatch-0.6.3/watch/tasks/cold/export_change_map.py` & `geowatch-0.6.6/watch/tasks/cold/export_change_map.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/cold/export_cold_result_kwcoco.py` & `geowatch-0.6.6/watch/tasks/cold/export_cold_result_kwcoco.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,18 +89,18 @@
     Example:
     >>> # xdoctest: +REQUIRES(env:TEST_COLD)
     >>> from watch.tasks.cold.export_cold_result_kwcoco import export_cold_main
     >>> from watch.tasks.cold.export_cold_result_kwcoco import *
     >>> kwargs= dict(
     >>>    rank = 0,
     >>>    n_cores = 1,
-    >>>    stack_path = "/home/jws18003/data/dvc-repos/smart_data_dvc/Drop6/_pycold_combine/stacked/KR_R001/",
-    >>>    reccg_path = "/home/jws18003/data/dvc-repos/smart_data_dvc/Drop6/_pycold_combine/reccg/KR_R001/",
-    >>>    meta_fpath = '/home/jws18003/data/dvc-repos/smart_data_dvc/Drop6/_pycold_combine/stacked/KR_R001/block_x9_y9/crop_20210807T010000Z_N37.643680E128.649453_N37.683356E128.734073_L8_0.json',
-    >>>    combined_coco_fpath = "/home/jws18003/data/dvc-repos/smart_data_dvc/Drop6_MeanYear/data_vali_split1_KR_R001_MeanYear.kwcoco.json",
+    >>>    stack_path = "/gpfs/scratchfs1/zhz18039/jws18003/new-repos/smart_data_dvc2/Drop6-MeanYear10GSD-V2/_pycold_combine2/stacked/KR_R001/",
+    >>>    reccg_path = "/gpfs/scratchfs1/zhz18039/jws18003/new-repos/smart_data_dvc2/Drop6-MeanYear10GSD-V2/_pycold_combine2/reccg/KR_R001/",
+    >>>    meta_fpath = '/gpfs/scratchfs1/zhz18039/jws18003/new-repos/smart_data_dvc2/Drop6-MeanYear10GSD-V2/_pycold_combine2/stacked/KR_R001/block_x10_y1/crop_20140115T020000Z_N37.643680E128.649453_N37.683356E128.734073_L8_0.json',
+    >>>    combined_coco_fpath = "/gpfs/scratchfs1/zhz18039/jws18003/new-repos/smart_data_dvc2/Drop6-MeanYear10GSD-V2/imgonly-KR_R001.kwcoco.zip",
     >>>    coefs = 'cv,rmse,a0,a1,b1,c1',
     >>>    year_lowbound = None,
     >>>    year_highbound = None,
     >>>    coefs_bands = '0,1,2,3,4,5',
     >>>    timestamp = False,
     >>>    combine = True,
     >>>    )
@@ -241,14 +241,25 @@
     img_dates, img_names = zip(*filter(lambda x: x[0] < year_high_ordinal,
                                        zip(img_dates, img_names)))
 
     img_dates = sorted(img_dates)
     img_names = sorted(img_names)
     if timestamp:
         ordinal_day_list = img_dates
+    if not timestamp:
+        first_ordinal_dates = []
+        first_img_names = []
+        last_year = None
+        for ordinal_day, img_name in zip(img_dates, img_names):
+            year = pd.Timestamp.fromordinal(ordinal_day).year
+            if year != last_year:
+                first_ordinal_dates.append(ordinal_day)
+                first_img_names.append(img_name)
+                last_year = year
+        ordinal_day_list = first_ordinal_dates
     if combine:
         combined_coco_dset = kwcoco.CocoDataset(combined_coco_fpath)
 
         # filter by sensors
         all_images = combined_coco_dset.images(list(ub.flatten(combined_coco_dset.videos().images)))
         flags = [s in sensors for s in all_images.lookup('sensor_coarse')]
         all_images = all_images.compress(flags)
@@ -265,27 +276,14 @@
             july_first = datetime_mod.date(timestamp_utc.year, 7, 1).toordinal()
             ordinal = timestamp_utc.toordinal()
             ordinal_dates.append(ordinal)
             ordinal_dates_july_first.append(july_first)
 
         ordinal_day_list = ordinal_dates
 
-        # Back up
-    if not timestamp:
-        first_ordinal_dates = []
-        first_img_names = []
-        last_year = None
-        for ordinal_day, img_name in zip(img_dates, img_names):
-            year = pd.Timestamp.fromordinal(ordinal_day).year
-            if year != last_year:
-                first_ordinal_dates.append(ordinal_day)
-                first_img_names.append(img_name)
-                last_year = year
-        ordinal_day_list = first_ordinal_dates
-
     ranks_percore = int(np.ceil(n_blocks / n_cores))
     i_iter = range(ranks_percore)
     if pman is not None:
         i_iter = pman.progiter(i_iter, total=ranks_percore,
                                desc=f'Export COLD \\[rank {rank}]', transient=True)
 
     for i in i_iter:
```

### Comparing `geowatch-0.6.3/watch/tasks/cold/predict.py` & `geowatch-0.6.6/watch/tasks/cold/predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,73 +82,61 @@
 
     smartwatch visualize \
         "$DATA_DVC_DPATH"/Drop6-SMALL/_pycold/imgonly-KR_R001-cold.fixed.kwcoco.zip \
         --channels="L8:(red|green|blue,red_COLD_cv|green_COLD_cv|blue_COLD_cv)" \
         --exclude_sensors="S2" \
         --smart=True --skip_aggressive=True
 
-    ####################
-    ### FULL REGION TEST
-    ####################
+    #######################
+    ### FULL REGION TEST-V1
+    #######################
 
     DATA_DVC_DPATH=$(geowatch_dvc --tags=phase2_data --hardware="auto")
     EXPT_DVC_DPATH=$(geowatch_dvc --tags=phase2_expt --hardware="auto")
     python -m watch.tasks.cold.predict \
         --coco_fpath="$DATA_DVC_DPATH/Drop6/imgonly-KR_R001.kwcoco.json" \
         --combined_coco_fpath="$DATA_DVC_DPATH/Drop6-MeanYear10GSD-V2/imgonly-KR_R001.kwcoco.zip" \
-        --out_dpath="$DATA_DVC_DPATH/Drop6-MeanYear10GSD-V2/_pycold_combine" \
-        --mod_coco_fpath="$DATA_DVC_DPATH/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold.kwcoco.zip" \
+        --out_dpath="$DATA_DVC_DPATH/Drop6-MeanYear10GSD-V2/_pycold_combine_V1" \
+        --mod_coco_fpath="$DATA_DVC_DPATH/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold-V1.kwcoco.zip" \
         --sensors='L8' \
         --adj_cloud=False \
         --method='COLD' \
         --prob=0.99 \
         --conse=6 \
         --cm_interval=60 \
         --year_lowbound=None \
         --year_highbound=None \
         --coefs=cv,rmse,a0,a1,b1,c1 \
         --coefs_bands=0,1,2,3,4,5 \
-        --timestamp=True \
+        --timestamp=False \
         --combine=True \
         --resolution='10GSD' \
         --workermode='serial' \
         --workers=0
 
-    kwcoco stats "$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold.kwcoco.zip
-    geowatch stats "$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold.kwcoco.zip
-
-    # Fix path problem because we wrote a different directory
-    # TODO: fix this script so the output always uses absolute paths?
-    # or at least doesn't write invalid data that needs fixing?
-    DATA_DVC_DPATH=$(geowatch_dvc --tags=phase2_data --hardware="auto")
-    kwcoco reroot \
-        --src="$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold.kwcoco.zip \
-        --dst="$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold_fixed.kwcoco.zip \
-        --absolute=True
-
-        --old_prefix="KR_R001" --new_prefix="../KR_R001"
-
-    DATA_DVC_DPATH=$(geowatch_dvc --tags=phase2_data --hardware="auto")
-    kwcoco validate "$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold_fixed.kwcoco.zip
+    kwcoco stats "$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold-V1.kwcoco.zip
+    geowatch stats "$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold-V1.kwcoco.zip
+    kwcoco validate "$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold-V1.kwcoco.zip
 
     smartwatch visualize \
-        "$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold.kwcoco.zip \
+        "$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold-V1.kwcoco.zip \
         --channels="L8:(red|green|blue,red_COLD_a1|green_COLD_a1|blue_COLD_a1,red_COLD_cv|green_COLD_cv|blue_COLD_cv,red_COLD_rmse|green_COLD_rmse|blue_COLD_rmse)" \
+        --exclude_sensors=WV,PD,S2 \
         --smart=True
 
-    ####################
+    #######################
     ### FULL REGION TEST V2
-    ####################
+    #######################
 
-    DATA_DVC_DPATH=$(smartwatch_dvc --tags=phase2_data --hardware="auto")
-    EXPT_DVC_DPATH=$(smartwatch_dvc --tags=phase2_expt --hardware="auto")
+    DATA_DVC_DPATH=$(geowatch_dvc --tags=phase2_data --hardware="auto")
+    EXPT_DVC_DPATH=$(geowatch_dvc --tags=phase2_expt --hardware="auto")
     python -m watch.tasks.cold.predict \
         --coco_fpath="$DATA_DVC_DPATH/Drop6/imgonly-KR_R001.kwcoco.json" \
-        --combined_coco_fpath="$DATA_DVC_DPATH/Drop6/imgonly-KR_R001.kwcoco.json" \
-        --out_dpath="$DATA_DVC_DPATH/Drop6/_pycold_combine" \
+        --out_dpath="$DATA_DVC_DPATH/Drop6/_pycold_combine_V2" \
+        --mod_coco_fpath="$DATA_DVC_DPATH/Drop6/imgonly_KR_R001_cold-V2.kwcoco.zip" \
         --sensors='L8' \
         --adj_cloud=False \
         --method='COLD' \
         --prob=0.99 \
         --conse=6 \
         --cm_interval=60 \
         --year_lowbound=None \
@@ -157,40 +145,58 @@
         --coefs_bands=0,1,2,3,4,5 \
         --timestamp=False \
         --combine=False \
         --resolution='10GSD' \
         --workermode='serial' \
         --workers=0
 
+    kwcoco stats "$DATA_DVC_DPATH/Drop6/imgonly_KR_R001_cold-V2.kwcoco.zip"
+    geowatch stats "$DATA_DVC_DPATH/Drop6/imgonly_KR_R001_cold-V2.kwcoco.zip"
+    kwcoco validate "$DATA_DVC_DPATH/Drop6/imgonly_KR_R001_cold-V2.kwcoco.zip"
+
+    DATA_DVC_DPATH=$(smartwatch_dvc --tags=phase2_data --hardware="auto")
+    smartwatch visualize \
+        "$DATA_DVC_DPATH/Drop6/imgonly_KR_R001_cold-V2.kwcoco.zip" \
+        --channels="L8:(red|green|blue,red_COLD_a1|green_COLD_a1|blue_COLD_a1,red_COLD_cv|green_COLD_cv|blue_COLD_cv,red_COLD_rmse|green_COLD_rmse|blue_COLD_rmse)" \
+        --exclude_sensors=WV,PD,S2 \
+        --smart=True
 
     ########################
     ### MULTIPLE REGION TEST
     ########################
     DVC_DATA_DPATH=$(geowatch_dvc --tags='phase2_data' --hardware=auto)
 
+    "$BUNDLE_DPATH"/imganns-*BR_[RC]*.kwcoco.zip \
+    "$BUNDLE_DPATH"/imganns-*KR_[RC]*.kwcoco.zip \
+    "$BUNDLE_DPATH"/imganns-*NZ_[RC]*.kwcoco.zip \
+    "$BUNDLE_DPATH"/imganns-*US_[RC]*.kwcoco.zip \
+
     echo "$DVC_DATA_DPATH"
     BUNDLE_DPATH=$DVC_DATA_DPATH/Drop6
     python -m watch.cli.prepare_teamfeats \
         --base_fpath \
-            "$BUNDLE_DPATH"/imganns-*BR_R*.kwcoco.zip \
-            "$BUNDLE_DPATH"/imganns-*KR_R*.kwcoco.zip \
-            "$BUNDLE_DPATH"/imganns-*NZ_R*.kwcoco.zip \
-            "$BUNDLE_DPATH"/imganns-*US_R*.kwcoco.zip \
-        --expt_dpath="$DVC_EXPT_DPATH" \
+            "$BUNDLE_DPATH"/imganns-*AE_[RC]*.kwcoco.zip \
+            "$BUNDLE_DPATH"/imganns-*BH_[RC]*.kwcoco.zip \
+            "$BUNDLE_DPATH"/imganns-*CH_[RC]*.kwcoco.zip \
+            "$BUNDLE_DPATH"/imganns-*LT_[RC]*.kwcoco.zip \
+            "$BUNDLE_DPATH"/imganns-*NZ_[RC]*.kwcoco.zip \
+            "$BUNDLE_DPATH"/imganns-*PE_[RC]*.kwcoco.zip \
+            "$BUNDLE_DPATH"/imganns-*QA_[RC]*.kwcoco.zip \
+            "$BUNDLE_DPATH"/imganns-*SA_[RC]*.kwcoco.zip \
+            "$BUNDLE_DPATH"/imganns-*US_C*.kwcoco.zip \
         --with_cold=1 \
         --with_landcover=0 \
         --with_materials=0 \
         --with_invariants=0 \
         --with_depth=0 \
-        --do_splits=0 \
         --skip_existing=1 \
         --cold_workers=8 \
         --cold_workermode=thread \
-        --workers=2 \
-        --backend=tmux --run=1
+        --tmux_workers=2 \
+        --backend=tmux --run=0
 """
 import scriptconfig as scfg
 import ubelt as ub
 import json
 import logging
 import shutil
```

### Comparing `geowatch-0.6.3/watch/tasks/cold/prepare_ard.py` & `geowatch-0.6.6/watch/tasks/cold/prepare_ard.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/cold/prepare_kwcoco.py` & `geowatch-0.6.6/watch/tasks/cold/prepare_kwcoco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/cold/tile_processing.py` & `geowatch-0.6.6/watch/tasks/cold/tile_processing.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/cold/tile_processing_kwcoco.py` & `geowatch-0.6.6/watch/tasks/cold/tile_processing_kwcoco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/depth/backbone.py` & `geowatch-0.6.6/watch/tasks/depth/backbone.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/depth/config.json` & `geowatch-0.6.6/watch/tasks/depth/config.json`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/depth/datasets.py` & `geowatch-0.6.6/watch/tasks/depth/datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/depth/demo_transform.py` & `geowatch-0.6.6/watch/tasks/depth/demo_transform.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/depth/dzyne_img_util.py` & `geowatch-0.6.6/watch/tasks/depth/dzyne_img_util.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/depth/pl_highres_verify.py` & `geowatch-0.6.6/watch/tasks/depth/pl_highres_verify.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/depth/predict.py` & `geowatch-0.6.6/watch/tasks/depth/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/depth/utils.py` & `geowatch-0.6.6/watch/tasks/depth/utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/depthPCD/model.py` & `geowatch-0.6.6/watch/tasks/depth_pcd/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     import os
     os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 
     # Monkey patch in deeplab2 to sys.path
     try:
         PARENT_DPATH = ub.Path(__file__).parent
     except NameError:
-        from watch.tasks import depthPCD as parent_package
+        from watch.tasks import depth_pcd as parent_package
         PARENT_DPATH = ub.Path(parent_package.__file__).parent
 
     TPL_DPATH = PARENT_DPATH / 'tpl'
 
     import sys
     if TPL_DPATH not in sys.path:
         # Ideally we would use the PythonPathContext to ensure we do not
@@ -33,16 +33,16 @@
     from tensorflow.keras.layers import Layer, Dense, concatenate, Conv2D, \
         BatchNormalization, \
         GlobalAveragePooling2D, Dropout
     from tensorflow.keras.models import Model, Sequential
     import cv2
     import numpy as np
     # import sys
-    # sys.path.append('watch/tasks/depthPCD')
-    # sys.path.append('watch/tasks/depthPCD/deeplab2')
+    # sys.path.append('watch/tasks/depth_pcd')
+    # sys.path.append('watch/tasks/depth_pcd/deeplab2')
 
 
 img_size = 400
 
 
 def normalize(im, q=5, r=128):
     imr = cv2.resize(im, (r, r))
@@ -54,15 +54,15 @@
     im[im > 1] = 1
     im[im < 0] = 0
     im = im * 255
     im = cv2.resize(im, (img_size, img_size))
     return im
 
 
-def getModel(proto='watch/tasks/depthPCD/deeplab2/max_deeplab_s_backbone_os16.textproto'):
+def getModel(proto='watch/tasks/depth_pcd/deeplab2/max_deeplab_s_backbone_os16.textproto'):
     options = config_pb2.ExperimentOptions()
 
     with tf.io.gfile.GFile(proto) as f:
         text_format.Parse(f.read(), options)
 
     model = DeepLab(options)
     i = tf.keras.Input([img_size, img_size, 3], batch_size=1)
```

### Comparing `geowatch-0.6.3/watch/tasks/dino_detector/building_validator.py` & `geowatch-0.6.6/watch/tasks/dino_detector/building_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     """
     Ignore:
         from watch.tasks.dino_detector.building_validator import *  # NOQA
         NODE_DPATH = '/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_mlops_eval10_baseline/pred/flat/buildings/buildings_id_fd298dba'
         from watch.utils.partial_format import fsubtemplate
         coco_fpath = fsubtemplate('$NODE_DPATH/pred_boxes.kwcoco.zip')
         from watch.utils.util_path import coerce_patterned_paths
-        site_summary = ub.Path(fsubtemplate('$NODE_DPATH/.pred/valicrop/*/.pred/bas_poly/*/site_summaries_manifest.json'))
+        site_summary = ub.Path(fsubtemplate('$NODE_DPATH/.pred/sv_crop/*/.pred/bas_poly/*/site_summaries_manifest.json'))
         site_summary = coerce_patterned_paths(site_summary)[0]
 
         output_region_fpath = ub.Path(fsubtemplate('$NODE_DPATH/filtered_site_summaries.geojson'))
 
         kwargs = {
             'input_kwcoco': coco_fpath,
             'input_region': site_summary,
@@ -291,29 +291,31 @@
             f'sites with paths {len(sites_with_paths)} are not the same as '
             f'sites with summaries {len(sites_with_summary)}')
 
     # Copy the filtered site models over to the output directory
     keep_site_fpaths = site_to_site_fpath.subdict(accept_sites)
     output_sites_dpath = ub.Path(config.output_sites_dpath)
     output_sites_dpath.ensuredir()
+    out_site_fpaths = []
     for old_fpath in keep_site_fpaths.values():
         new_fpath = output_sites_dpath / old_fpath.name
         old_fpath.copy(new_fpath, overwrite=True)
+        out_site_fpaths.append(new_fpath)
 
     new_region_model = geomodels.RegionModel.from_features(
         [region_model.header] + list(new_summaries))
 
     output_region_fpath.parent.ensuredir()
     with safer.open(output_region_fpath, 'w', temp_file=not ub.WIN32) as file:
         json.dump(new_region_model, file, indent=4)
 
     proc_context.stop()
 
     if config.output_site_manifest_fpath is not None:
-        filter_output['files'] = [os.fspath(output_region_fpath)]
+        filter_output['files'] = [os.fspath(p) for p in out_site_fpaths]
         print(f'Write filtered site result to {config.output_site_manifest_fpath}')
         with safer.open(config.output_site_manifest_fpath, 'w', temp_file=not ub.WIN32) as file:
             json.dump(filter_output, file, indent=4)
 
 
 def building_in_image_features(coco_img, site_id, config):
     import numpy as np
@@ -451,19 +453,19 @@
             bas_poly_eval.true_site_dpath: $DVC_DATA_DPATH/annotations/drop6/site_models
             bas_poly_eval.true_region_dpath: $DVC_DATA_DPATH/annotations/drop6/region_models
             bas_pxl.enabled: 1
             bas_pxl_eval.enabled: 1
             bas_poly.enabled: 1
             bas_poly_eval.enabled: 1
             bas_poly_viz.enabled: 0
-            valicrop.enabled: 1
-            valicrop.minimum_size: "256x256@2GSD"
-            valicrop.num_start_frames: 3
-            valicrop.num_end_frames: 3
-            valicrop.context_factor: 1.5
+            sv_crop.enabled: 1
+            sv_crop.minimum_size: "256x256@2GSD"
+            sv_crop.num_start_frames: 3
+            sv_crop.num_end_frames: 3
+            sv_crop.context_factor: 1.5
             sv_dino_boxes.enabled: 1
             sv_dino_boxes.package_fpath: $DVC_EXPT_DPATH/models/kitware/xview_dino.pt
             sv_dino_boxes.window_dims:
                 - 256
                 - 512
                 - 768
                 - 1024
@@ -492,25 +494,25 @@
                 - 0.2
                 - 0.25
                 - 0.3
                 # - 0.4
                 - 0.5
         submatrices:
             - bas_pxl.test_dataset: $DVC_DATA_DPATH/Drop6-MeanYear10GSD-V2/imganns-KR_R001.kwcoco.zip
-              valicrop.crop_src_fpath: $DVC_DATA_DPATH/Drop6/imgonly-KR_R001.kwcoco.json
+              sv_crop.crop_src_fpath: $DVC_DATA_DPATH/Drop6/imgonly-KR_R001.kwcoco.json
             - bas_pxl.test_dataset: $DVC_DATA_DPATH/Drop6-MeanYear10GSD-V2/imganns-KR_R002.kwcoco.zip
-              valicrop.crop_src_fpath: $DVC_DATA_DPATH/Drop6/imgonly-KR_R002.kwcoco.json
+              sv_crop.crop_src_fpath: $DVC_DATA_DPATH/Drop6/imgonly-KR_R002.kwcoco.json
             - bas_pxl.test_dataset: $DVC_DATA_DPATH/Drop6-MeanYear10GSD-V2/imganns-BR_R002.kwcoco.zip
-              valicrop.crop_src_fpath: $DVC_DATA_DPATH/Drop6/imgonly-BR_R002.kwcoco.json
+              sv_crop.crop_src_fpath: $DVC_DATA_DPATH/Drop6/imgonly-BR_R002.kwcoco.json
             - bas_pxl.test_dataset: $DVC_DATA_DPATH/Drop6-MeanYear10GSD-V2/imganns-CH_R001.kwcoco.zip
-              valicrop.crop_src_fpath: $DVC_DATA_DPATH/Drop6/imgonly-CH_R001.kwcoco.json
+              sv_crop.crop_src_fpath: $DVC_DATA_DPATH/Drop6/imgonly-CH_R001.kwcoco.json
             - bas_pxl.test_dataset: $DVC_DATA_DPATH/Drop6-MeanYear10GSD-V2/imganns-NZ_R001.kwcoco.zip
-              valicrop.crop_src_fpath: $DVC_DATA_DPATH/Drop6/imgonly-NZ_R001.kwcoco.json
+              sv_crop.crop_src_fpath: $DVC_DATA_DPATH/Drop6/imgonly-NZ_R001.kwcoco.json
             - bas_pxl.test_dataset: $DVC_DATA_DPATH/Drop6-MeanYear10GSD-V2/imganns-AE_R001.kwcoco.zip
-              valicrop.crop_src_fpath: $DVC_DATA_DPATH/Drop6/imgonly-AE_R001.kwcoco.json
+              sv_crop.crop_src_fpath: $DVC_DATA_DPATH/Drop6/imgonly-AE_R001.kwcoco.json
         " \
         --root_dpath="$DVC_EXPT_DPATH/_mlops_eval10_baseline" \
         --devices="0," --tmux_workers=8 \
         --backend=tmux --queue_name "_mlops_eval10_baseline" \
         --pipeline=bas_building_vali --skip_existing=1 \
         --run=1
 
@@ -537,15 +539,15 @@
 
 
 
         print_models: True
 
 geowatch align \
     --src "/home/joncrall/remote/toothbrush/data/dvc-repos/smart_data_dvc-ssd/Drop6/imgonly-KR_R001.kwcoco.json" \
-    --dst "/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_mlops_eval10_baseline/pred/flat/valicrop/valicrop_id_2e8c8dc3/valicrop.kwcoco.zip" \
+    --dst "/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_mlops_eval10_baseline/pred/flat/sv_crop/valicrop_id_2e8c8dc3/sv_crop.kwcoco.zip" \
     --regions="/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_mlops_eval10_baseline/pred/flat/bas_poly/bas_poly_id_dc32b2a6/site_summaries_manifest.json" \
     --site_summary=True \
     --verbose="1" \
     --workers="32" \
     --aux_workers="4" \
     --debug_valid_regions="False" \
     --visualize="False" \
@@ -558,22 +560,22 @@
     --include_sensors="WV" \
     --force_nodata="-9999" \
     --rpc_align_method="orthorectify" \
     --target_gsd="2" \
     --force_min_gsd="2" \
     --convexify_regions="True"
 
-geowatch visualize /home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_mlops_eval10_baseline/pred/flat/valicrop/valicrop_id_2e8c8dc3/valicrop.kwcoco.zip --smart
+geowatch visualize /home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_mlops_eval10_baseline/pred/flat/sv_crop/valicrop_id_2e8c8dc3/sv_crop.kwcoco.zip --smart
 
-python ~/code/watch/dev/wip/grid_sitevali_crops.py /home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_mlops_eval10_baseline/pred/flat/valicrop/valicrop_id_2e8c8dc3/_viz_*
+python ~/code/watch/dev/wip/grid_sitevali_crops.py /home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_mlops_eval10_baseline/pred/flat/sv_crop/valicrop_id_2e8c8dc3/_viz_*
 
 
 python -m watch.tasks.dino_detector.predict \
     --package_fpath="/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/models/kitware/xview_dino.pt" \
-    --coco_fpath="/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_mlops_eval10_baseline/pred/flat/valicrop/valicrop_id_2e8c8dc3/valicrop.kwcoco.zip" \
+    --coco_fpath="/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_mlops_eval10_baseline/pred/flat/sv_crop/valicrop_id_2e8c8dc3/sv_crop.kwcoco.zip" \
     --out_coco_fpath="/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_mlops_eval10_baseline/pred/flat/buildings/buildings_id_61b8c2c7/pred_boxes.kwcoco.zip" \
     --device="0" \
     --data_workers="2" \
     --fixed_resolution="1.0GSD" \
     --window_dims="2048" \
     --batch_size="1"
 
@@ -589,15 +591,15 @@
 
 NODE_DPATH=/home/joncrall/remote/toothbrush/data/dvc-repos/smart_expt_dvc/_mlops_eval10_baseline/pred/flat/buildings/buildings_id_fd298dba
 DVC_DATA_DPATH=$(geowatch_dvc --tags='phase2_data' --hardware=auto)
 
 geowatch reproject \
         --src "$NODE_DPATH/pred_boxes.kwcoco.zip" \
         --dst "$NODE_DPATH/pred_boxes_with_polys.kwcoco.zip" \
-        --region_models "$NODE_DPATH/.pred/valicrop/*/.pred/bas_poly/*/site_summaries_manifest.json" \
+        --region_models "$NODE_DPATH/.pred/sv_crop/*/.pred/bas_poly/*/site_summaries_manifest.json" \
         --status_to_catname="{system_confirmed: positive}" \
         --role=pred_poly \
         --validate_checks=False \
         --clear_existing=False
 
 geowatch reproject \
         --src "$NODE_DPATH/pred_boxes_with_polys.kwcoco.zip" \
@@ -617,15 +619,15 @@
 
 python ~/code/watch/dev/wip/grid_sitevali_crops.py \
     --sub=_anns \
     $NODE_DPATH/_vizme
 
 python -m watch.tasks.dino_detector.building_validator \
     --input_kwcoco "$NODE_DPATH/pred_boxes.kwcoco.zip" \
-    --input_region $NODE_DPATH/.pred/valicrop/*/.pred/bas_poly/*/site_summaries_manifest.json \
+    --input_region $NODE_DPATH/.pred/sv_crop/*/.pred/bas_poly/*/site_summaries_manifest.json \
     --output_region_fpath "$NODE_DPATH/filtered_summaries.json" \
     --box_isect_threshold 0.1 \
     --box_score_threshold 0.1 \
     --start_max_score 0.0 \
     --end_min_score 0.3
 
 python -m watch.tasks.dino_detector.building_validator \
```

### Comparing `geowatch-0.6.3/watch/tasks/dino_detector/predict.py` & `geowatch-0.6.6/watch/tasks/dino_detector/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/__init__.py` & `geowatch-0.6.6/watch/tasks/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/aggregate_results.py` & `geowatch-0.6.6/watch/tasks/fusion/aggregate_results.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/architectures/segmenter_decoder.py` & `geowatch-0.6.6/watch/tasks/fusion/architectures/segmenter_decoder.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/architectures/sits.py` & `geowatch-0.6.6/watch/tasks/fusion/architectures/sits.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/architectures/transformer.py` & `geowatch-0.6.6/watch/tasks/fusion/architectures/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -962,14 +962,16 @@
         'p2w': dict(n_layers=2, embedding_size=128, n_heads=8),
 
         'p3': dict(n_layers=3, embedding_size=128, n_heads=4),
         'p4': dict(n_layers=4, embedding_size=128, n_heads=4),
 
         'p8': dict(n_layers=8, embedding_size=128, n_heads=4),
         'p16': dict(n_layers=16, embedding_size=128, n_heads=4),
+        'p24': dict(n_layers=24, embedding_size=128, n_heads=4),
+        'p32': dict(n_layers=32, embedding_size=128, n_heads=4),
 
         'b8': dict(n_layers=8, embedding_size=384, n_heads=4),
         'n12': dict(n_layers=12, embedding_size=128, n_heads=4),
         't12': dict(n_layers=12, embedding_size=192, n_heads=4),
         't24': dict(n_layers=24, embedding_size=192, n_heads=4),
         's12': dict(n_layers=12, embedding_size=384, n_heads=8),
         's24': dict(n_layers=24, embedding_size=384, n_heads=8),
```

### Comparing `geowatch-0.6.3/watch/tasks/fusion/architectures/unet_blur.py` & `geowatch-0.6.6/watch/tasks/fusion/architectures/unet_blur.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/architectures/wu_mae.py` & `geowatch-0.6.6/watch/tasks/fusion/architectures/wu_mae.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/coco_stitcher.py` & `geowatch-0.6.6/watch/tasks/fusion/coco_stitcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,14 +493,15 @@
         """
         Finalizes the stitcher for this image, deletes it, and adds
         its hard and/or soft predictions to the CocoDataset.
 
         Args:
             gid (int): the image-id to finalize
         """
+        import os
         # Remove this image from the managed set.
         img = self.result_dataset.index.imgs[gid]
 
         self._ready_gids.difference_update({gid})
 
         try:
             # stitcher = self.image_stitchers.get(gid)
@@ -635,27 +636,39 @@
                 if self.expected_minmax is None:
                     old_min, old_max = None, None
                 else:
                     old_min, old_max = self.expected_minmax
                 quant_probs, quantization = quantize_image(
                     final_probs, old_min=old_min, old_max=old_max,
                     quantize_dtype=quantize_dtype)
+                write_data = quant_probs
                 aux['quantization'] = quantization
             else:
+                write_data = final_probs
                 quantization = None
 
             if self.prob_format != 'png':
                 write_kwargs['metadata'] = {
                     'quantization': quantization,
                 }
 
-            kwimage.imwrite(
-                str(new_fpath), final_probs, space=None, backend=imwrite_backend,
-                **write_kwargs,
-            )
+            try:
+                kwimage.imwrite(
+                    os.fspath(new_fpath), write_data, space=None, backend=imwrite_backend,
+                    **write_kwargs,
+                )
+            except Exception as ex:
+                print()
+                print('ERROR ex = {}'.format(ub.urepr(ex, nl=1)))
+                print('new_fpath = {}'.format(ub.urepr(new_fpath, nl=1)))
+                print(f'imwrite_backend={imwrite_backend}')
+                print(f'write_data.shape={write_data.shape}')
+                print(f'write_data.dtype={write_data.dtype}')
+                print(f'write_kwargs={write_kwargs}')
+                raise
 
         if self.write_preds:
             from watch.tasks.tracking.utils import mask_to_polygons
             ub.schedule_deprecation(
                 'watch', 'write_preds', 'needs a different abstraction.',
                 deprecate='now')
             # NOTE: The typical pipeline will never do this.
```

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/_notebook.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/_notebook.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/batch_visualization.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/batch_visualization.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/data_augment.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/data_augment.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/data_utils.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/data_utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/demos_for_slides.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/demos_for_slides.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/kwcoco_datamodule.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/kwcoco_datamodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import scriptconfig as scfg
 
 from watch.utils import util_globals
 from watch.utils import util_parallel
 from watch.tasks.fusion import utils
 from watch.tasks.fusion.datamodules.kwcoco_dataset import KWCocoVideoDatasetConfig, KWCocoVideoDataset
 
-from typing import Dict, List  # NOQA
+from typing import Dict
 
 try:
     import xdev
     profile = xdev.profile
 except Exception:
     profile = ub.identity
 
@@ -32,17 +32,17 @@
     The scriptconfig class is not used directly as it normally would be here.
     Instead we use it as a convinience to minimize lightning boilerplate later
     when it constructs its own argparse object, and for handling arguments
     passed directly to the KWCocoDataModule
 
     In the future this might be convertable to, or handled by omegaconfig
     """
-    train_dataset = scfg.Value(None, help='path to the train kwcoco file')
-    vali_dataset = scfg.Value(None, help='path to the validation kwcoco file')
-    test_dataset = scfg.Value(None, help='path to the test kwcoco file')
+    train_dataset = scfg.Value(None, help='path to the train kwcoco file', group='datasets')
+    vali_dataset = scfg.Value(None, help='path to the validation kwcoco file', group='datasets')
+    test_dataset = scfg.Value(None, help='path to the test kwcoco file', group='datasets')
 
     batch_size = scfg.Value(4, type=int, help=None)
 
     normalize_inputs = scfg.Value(True, help=ub.paragraph(
             '''
             if True, computes the mean/std for this dataset on each mode
             so this can be passed to the model.
@@ -52,32 +52,41 @@
 
     num_workers = scfg.Value(4, type=str, alias=['workers'], help=ub.paragraph(
             '''
             number of background workers. Can be auto or an avail
             expression.
             '''))
 
+    request_rlimit_nofile = scfg.Value('auto', help=ub.paragraph(
+        '''
+        As a convinience, on Linux systems this automatically requests that
+        ulimit raises the maximum number of open files allowed. Auto currently
+        simply sets this to 8192, so use a number higher than this if you run
+        into too many open file errors, or set your ulimit explicitly before
+        running this software.
+        '''), group='resources')
+
     torch_sharing_strategy = scfg.Value('default', help=ub.paragraph(
             '''
             Torch multiprocessing sharing strategy. Can be 'default',
             "file_descriptor", "file_system". On linux, the default is
             "file_descriptor". See https://pytorch.org/docs/stable/multi
             processing.html#sharing-strategies for descriptions of
             options. When using sqlview=True, using "file_system" can
             help prevent the "received 0 items of ancdata" Error. It is
             unclear why using "file_descriptor" fails in this case for
             some datasets.
-            '''))
+            '''), group='resources')
 
     torch_start_method = scfg.Value('default', help=ub.paragraph(
             '''
             Torch multiprocessing sharing strategy. Can be "default",
             "fork", "spawn", "forkserver". The default method on Linux
             is "spawn".
-            '''))
+            '''), group='resources')
 
     sqlview = scfg.Value(False, help=ub.paragraph(
             '''
             If False, reads the COCO dataset as a json file. Otherwise
             it can be sqlite or postgresql to cache json file in an SQL
             database for faster responce times and lower memory
             footprint.
@@ -289,14 +298,15 @@
         if self.verbose:
             print('Setup DataModule: stage = {!r}'.format(stage))
 
         util_globals.configure_global_attributes(**{
             'num_workers': self.num_workers,
             'torch_sharing_strategy': self.torch_sharing_strategy,
             'torch_start_method': self.torch_start_method,
+            'request_rlimit_nofile': self.request_rlimit_nofile,
         })
         sqlview = self.config['sqlview']
 
         # Clear existing coco datasets so a reload occurs (should never happen
         # if the user doesnt touch `self.did_setup`).
         self.coco_datasets.clear()
         # make a temp mapping from train/vali/test to the specified coco inputs
```

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/kwcoco_dataset.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/kwcoco_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/qa_bands.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/qa_bands.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/smart_mixins.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/smart_mixins.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/spacetime_grid_builder.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/spacetime_grid_builder.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/__init__.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/_notebook.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/_notebook.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/affinity.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/affinity.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/plots.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/plots.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/sampler.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/sampler.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/time_kernel_grammar.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/time_kernel_grammar.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/utils.py` & `geowatch-0.6.6/watch/tasks/fusion/datamodules/temporal_sampling/utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/evaluate.py` & `geowatch-0.6.6/watch/tasks/fusion/evaluate.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/fit.py` & `geowatch-0.6.6/watch/tasks/fusion/fit.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/fit_lightning.py` & `geowatch-0.6.6/watch/tasks/fusion/fit_lightning.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/methods/__init__.py` & `geowatch-0.6.6/watch/tasks/fusion/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/methods/channelwise_transformer.py` & `geowatch-0.6.6/watch/tasks/fusion/methods/channelwise_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,18 @@
         the original O(n^2) method. 'performer' - a linear
         approximation. 'reformer' - a LSH approximation.
         '''))
     multimodal_reduce = scfg.Value('max', help=ub.paragraph(
         '''
         operation used to combine multiple modes from the same timestep
         '''))
+    rescale_nans = scfg.Value(None, help=ub.paragraph(
+        '''
+        Method used to rescale nan input values. Can be perframe or None.
+        '''))
 
 
 class MultimodalTransformer(pl.LightningModule, WatchModuleMixins):
     """
     CommandLine:
         xdoctest -m watch.tasks.fusion.methods.channelwise_transformer MultimodalTransformer
 
@@ -384,14 +388,22 @@
         else:
             RAW_CHANS = None
         print(f'RAW_CHANS={RAW_CHANS}')
         MODAL_AGREEMENT_CHANS = self.hparams.stream_channels
         print(f'MODAL_AGREEMENT_CHANS={MODAL_AGREEMENT_CHANS}')
         print(f'self.hparams.tokenizer={self.hparams.tokenizer}')
 
+        self.rescale_nan_method = self.hparams.rescale_nans
+        if self.rescale_nan_method == 'perframe':
+            ...
+        elif self.rescale_nan_method is None:
+            ...
+        else:
+            raise KeyError(f'Unknown: {self.rescale_nan_method}')
+
         self.tokenizer = self.hparams.tokenizer
         self.sensor_channel_tokenizers = RobustModuleDict()
 
         # Unique sensor modes obviously isn't very correct here.
         # We should fix that, but let's hack it so it at least
         # includes all sensor modes we probably will need.
         if input_stats is not None:
@@ -1481,15 +1493,32 @@
                     for _c in sorted(self.input_norms[_s].keys()):
                         print(f'{_s=!r} {_c=!r}')
                 raise
             # self.sensor_channel_tokenizers[]
 
         # After input normalization happens, replace nans with zeros
         # which is effectively imputing the dataset mean
-        mode_val = mode_val.nan_to_num_()
+
+        try:
+            rescale_nan_method = self.rescale_nan_method
+        except AttributeError:
+            rescale_nan_method = None
+
+        if rescale_nan_method is None:
+            mode_val = mode_val.nan_to_num_()
+        elif rescale_nan_method == 'perframe':
+            # Do a dropout-like rescaling to the nan input values.
+            num_nan = mode_val.isnan()
+            num_total = mode_val.numel()
+            p = min((num_nan / num_total), 1 - 1e-5)
+            mode_val = mode_val.nan_to_num_()
+            rescale_factor = 1 / (1 - p)
+            mode_val *= rescale_factor
+        else:
+            raise AssertionError
 
         # Lookup the "tokenizing" network for this type of input
         sensor_chan_tokenizer = self.sensor_channel_tokenizers[sensor][chan_code]
 
         # Is it worth gathering and stacking items in batches here?
 
         # Reduce spatial dimension and normalize the number of
```

### Comparing `geowatch-0.6.3/watch/tasks/fusion/methods/heterogeneous.py` & `geowatch-0.6.6/watch/tasks/fusion/methods/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/methods/network_modules.py` & `geowatch-0.6.6/watch/tasks/fusion/methods/network_modules.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/methods/noop_model.py` & `geowatch-0.6.6/watch/tasks/fusion/methods/noop_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/methods/unet_baseline.py` & `geowatch-0.6.6/watch/tasks/fusion/methods/unet_baseline.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/methods/watch_module_mixins.py` & `geowatch-0.6.6/watch/tasks/fusion/methods/watch_module_mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,20 @@
                 W2 = width_distri.sample()
 
                 modes = {
                     'pan': rng.rand(1, H0, W0).astype("float32"),
                     'red|green|blue': rng.rand(3, H1, W1).astype("float32"),
                     'nir|swir16|swir22': rng.rand(3, H2, W2).astype("float32"),
                 }
+
+                # Add in channels the model exepcts
+                for stream in self.input_sensorchan.streams():
+                    C = stream.chans.numel()
+                    modes[stream.chans.spec] = rng.rand(C, H1, W1).astype("float32")
+
                 frame = {}
                 if time_index == 0:
                     frame['change'] = None
                     frame['change_weights'] = None
                     frame['change_output_dims'] = None
                 else:
                     frame['change'] = rng.randint(low=0, high=1, size=(H0, W0))
```

### Comparing `geowatch-0.6.3/watch/tasks/fusion/organize.py` & `geowatch-0.6.6/watch/tasks/fusion/organize.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/fusion/predict.py` & `geowatch-0.6.6/watch/tasks/fusion/predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,19 +292,20 @@
         head_classes = ['change']
         head_keep_idxs = [
             idx for idx, catname in enumerate(head_classes)
             if catname not in ignore_classes]
         head_keep_classes = list(ub.take(head_classes, head_keep_idxs))
         chan_code = '|'.join(head_keep_classes)
         task_keep_indices[task_name] = head_keep_idxs
-        print('task_name = {!r}'.format(task_name))
-        print('head_classes = {!r}'.format(head_classes))
-        print('head_keep_classes = {!r}'.format(head_keep_classes))
-        print('chan_code = {!r}'.format(chan_code))
-        print('head_keep_idxs = {!r}'.format(head_keep_idxs))
+        if 0:
+            print('task_name = {!r}'.format(task_name))
+            print('head_classes = {!r}'.format(head_classes))
+            print('head_keep_classes = {!r}'.format(head_keep_classes))
+            print('chan_code = {!r}'.format(chan_code))
+            print('head_keep_idxs = {!r}'.format(head_keep_idxs))
         stitch_managers[task_name] = CocoStitchingManager(
             result_dataset,
             chan_code=chan_code,
             short_code='pred_' + task_name,
             num_bands=len(head_keep_classes),
             **stitcher_common_kw,
         )
@@ -324,19 +325,20 @@
         head_classes = method.classes
         head_keep_idxs = [
             idx for idx, catname in enumerate(head_classes)
             if catname not in ignore_classes]
         head_keep_classes = list(ub.take(head_classes, head_keep_idxs))
         task_keep_indices[task_name] = head_keep_idxs
         chan_code = '|'.join(list(head_keep_classes))
-        print('task_name = {!r}'.format(task_name))
-        print('head_classes = {!r}'.format(head_classes))
-        print('head_keep_classes = {!r}'.format(head_keep_classes))
-        print('chan_code = {!r}'.format(chan_code))
-        print('head_keep_idxs = {!r}'.format(head_keep_idxs))
+        if 0:
+            print('task_name = {!r}'.format(task_name))
+            print('head_classes = {!r}'.format(head_classes))
+            print('head_keep_classes = {!r}'.format(head_keep_classes))
+            print('chan_code = {!r}'.format(chan_code))
+            print('head_keep_idxs = {!r}'.format(head_keep_idxs))
         stitch_managers[task_name] = CocoStitchingManager(
             result_dataset,
             chan_code=chan_code,
             short_code='pred_' + task_name,
             polygon_categories=foreground_classes,
             num_bands=len(head_keep_classes),
             **stitcher_common_kw,
@@ -349,19 +351,20 @@
         head_classes = ['not_salient', 'salient']
         head_keep_idxs = [
             idx for idx, catname in enumerate(head_classes)
             if catname not in ignore_classes]
         head_keep_classes = list(ub.take(head_classes, head_keep_idxs))
         task_keep_indices[task_name] = head_keep_idxs
         chan_code = '|'.join(head_keep_classes)
-        print('task_name = {!r}'.format(task_name))
-        print('head_classes = {!r}'.format(head_classes))
-        print('head_keep_classes = {!r}'.format(head_keep_classes))
-        print('chan_code = {!r}'.format(chan_code))
-        print('head_keep_idxs = {!r}'.format(head_keep_idxs))
+        if 0:
+            print('task_name = {!r}'.format(task_name))
+            print('head_classes = {!r}'.format(head_classes))
+            print('head_keep_classes = {!r}'.format(head_keep_classes))
+            print('chan_code = {!r}'.format(chan_code))
+            print('head_keep_idxs = {!r}'.format(head_keep_idxs))
         stitch_managers[task_name] = CocoStitchingManager(
             result_dataset,
             chan_code=chan_code,
             short_code='pred_' + task_name,
             polygon_categories=['salient'],
             num_bands=len(head_keep_classes),
             **stitcher_common_kw,
```

### Comparing `geowatch-0.6.3/watch/tasks/fusion/production.py` & `geowatch-0.6.6/watch/tasks/fusion/production.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """
 These are the current models that should be considered for use in production.
 This also contains metadata about what data the models expect to run on.
 (This should also be contained in the model metadata itself).
 
 Production code exists here:
     https://gitlab.kitware.com/smart/watch/-/blob/dev/eval3-integration/scripts/run_bas_fusion_eval3_for_baseline.py
+
+SeeAlso:
+    ~/code/watch/watch/mlops/smart_global_helper.py
 """
 
 
 PRODUCTION_MODELS = [
     {
         'name': 'BAS_smt_it_stm_p8_TUNE_L1_RAW_v58_epoch=3-step=81135',
         'gsd': 10.0,
```

### Comparing `geowatch-0.6.3/watch/tasks/fusion/utils.py` & `geowatch-0.6.6/watch/tasks/fusion/utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/invariants/change.py` & `geowatch-0.6.6/watch/tasks/invariants/change.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/invariants/data/datasets.py` & `geowatch-0.6.6/watch/tasks/invariants/data/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,31 +433,33 @@
                 valid_coco_poly = None
                 sh_valid_poly = kw_poly_img.warp(warp_vid_from_img).to_shapely()  # shapely.geometry.Polygon
 
         # Sample valid offset boxes until the conditions are met
         rng = kwarray.ensure_rng(None)
         offset_box = None
         attempts = 0
-        while offset_box is None:
-            attempts += 1
-            offset_box = kwimage.Boxes([[0, 0, img_width, img_height]], 'ltrb')
-            offset_x = rng.randint(0, max(vid_width - img_width, 1))
-            offset_y = rng.randint(0, max(vid_height - img_height, 1))
-            offset_box = offset_box.translate((offset_x, offset_y))
-            if attempts > 10:
-                # Give up
-                break
-            sh_box = offset_box.to_shapely()[0]
-            orig_overlap = sh_space_box.intersection(sh_box).area / sh_space_box.area
-            if orig_overlap > 0.001:
-                offset_box = None
-            if sh_valid_poly is not None:
-                valid_frac = sh_valid_poly.intersection(sh_box).area / sh_box.area
-                if valid_frac < 0.5:
+        with warnings.catch_warnings():
+            warnings.filterwarnings('ignore', 'invalid value encountered in intersection')
+            while offset_box is None:
+                attempts += 1
+                offset_box = kwimage.Boxes([[0, 0, img_width, img_height]], 'ltrb')
+                offset_x = rng.randint(0, max(vid_width - img_width, 1))
+                offset_y = rng.randint(0, max(vid_height - img_height, 1))
+                offset_box = offset_box.translate((offset_x, offset_y))
+                if attempts > 10:
+                    # Give up
+                    break
+                sh_box = offset_box.to_shapely()[0]
+                orig_overlap = sh_space_box.intersection(sh_box).area / sh_space_box.area
+                if orig_overlap > 0.001:
                     offset_box = None
+                if sh_valid_poly is not None:
+                    valid_frac = sh_valid_poly.intersection(sh_box).area / sh_box.area
+                    if valid_frac < 0.5:
+                        offset_box = None
 
         # Create a new target for the offset region
         offset_tr = target.copy()
         offset_tr['channels'] = self.bands
         offset_tr['space_slice'] = offset_box.astype(int).to_slices()[0]
         return offset_tr
```

### Comparing `geowatch-0.6.3/watch/tasks/invariants/data/multi_image_datasets.py` & `geowatch-0.6.6/watch/tasks/invariants/data/multi_image_datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/invariants/data/other_datasets.py` & `geowatch-0.6.6/watch/tasks/invariants/data/other_datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/invariants/fit.py` & `geowatch-0.6.6/watch/tasks/invariants/fit.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/invariants/fit_segment.py` & `geowatch-0.6.6/watch/tasks/invariants/fit_segment.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/invariants/iarpa_dataset.py` & `geowatch-0.6.6/watch/tasks/invariants/iarpa_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/invariants/predict.py` & `geowatch-0.6.6/watch/tasks/invariants/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,16 @@
         >>> argv += ['--do_pca', '1']
         >>> args = InvariantPredictConfig.cli(argv=argv)
         >>> self = Predictor(args)
         >>> self.forward(args)
     """
 
     def __init__(self, args):
+        # import xdev
+        # xdev.make_warnings_print_tracebacks()
 
         # TODO: Add a cache flag. If cache==1, Determine what images we have
         # already predicted for and then take a kwcoco subset containing
         # the cache misses. See dzyne and rutgers predictors for example
         # implementations.
 
         # Doesnt work?
@@ -285,28 +287,31 @@
             self.dataset, num_workers=self.workers,
             batch_size=self.batch_size, shuffle=False)
         num_batches = len(loader)
 
         # Start background processes
         # Build a task queue for background write results workers
         from watch.utils import util_parallel
+        from watch.utils import util_progress
         writer_queue = util_parallel.BlockingJobQueue(max_workers=self.io_workers)
         self.stitch_manager.writer_queue = writer_queue
 
         self.proc_context.start()
 
         self.proc_context.add_disk_info(ub.Path(self.output_dset.fpath).parent)
         self.output_dset.dataset.setdefault('info', [])
         self.output_dset.dataset['info'].append(self.proc_context.obj)
 
         print('Evaluating and saving features')
 
-        with torch.set_grad_enabled(False):
+        pman = util_progress.ProgressManager()
+
+        with torch.set_grad_enabled(False), pman:
             seen_images = set()
-            prog = ub.ProgIter(enumerate(loader), total=num_batches, desc='Compute features', verbose=1)
+            prog = pman.progiter(enumerate(loader), total=num_batches, desc='Compute invariants', verbose=1)
             for idx, batch in prog:
                 save_feat = []
                 save_feat2 = []
 
                 # Handle input nans
                 img1 = batch['image1']
                 img2 = batch['image2']
@@ -419,15 +424,15 @@
                     dsize=outspace_dsize,
                     scale=scale_outspace_from_vid)
 
             print('Finalize already compelted jobs')
             writer_queue.wait_until_finished(desc='Finalize submitted jobs')
 
             # Finalize everything else that hasn't completed
-            for gid in ub.ProgIter(list(self.stitch_manager.image_stitchers.keys()), desc='submit loose write jobs'):
+            for gid in pman.progiter(list(self.stitch_manager.image_stitchers.keys()), desc='submit loose write jobs'):
                 if gid not in seen_images:
                     seen_images.add(gid)
                     self.stitch_manager.submit_finalize_image(gid)
                     # writer_queue.submit(self.stitch_manager.finalize, gid)
 
             print('Finalize loose jobs')
             writer_queue.wait_until_finished()
```

### Comparing `geowatch-0.6.3/watch/tasks/invariants/pretext_model.py` & `geowatch-0.6.6/watch/tasks/invariants/pretext_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/invariants/segmentation_model.py` & `geowatch-0.6.6/watch/tasks/invariants/segmentation_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/landcover/datasets.py` & `geowatch-0.6.6/watch/tasks/landcover/datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/landcover/detector.py` & `geowatch-0.6.6/watch/tasks/landcover/detector.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/landcover/model_info.py` & `geowatch-0.6.6/watch/tasks/landcover/model_info.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/landcover/nets.py` & `geowatch-0.6.6/watch/tasks/landcover/nets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/landcover/predict.py` & `geowatch-0.6.6/watch/tasks/landcover/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/metrics/merge_iarpa_metrics.py` & `geowatch-0.6.6/watch/tasks/metrics/merge_iarpa_metrics.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/metrics/viz_sc_results.py` & `geowatch-0.6.6/watch/tasks/metrics/viz_sc_results.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/__init__.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/base_dataset.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/iarpa_kwdataset.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/datasets/iarpa_kwdataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/iarpa_sc_kwdataset.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/datasets/iarpa_sc_kwdataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/peo_dataset.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/datasets/peo_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/__init__.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/apnb.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/apnb.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/base_model.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/base_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/discritizers.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/discritizers.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/dynamic_unet.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/dynamic_unet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/early_fusion_framework.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/early_fusion_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/early_fusion_mat_framework.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/early_fusion_mat_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/late_fusion_framework.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/late_fusion_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/mat_ed_framework.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/mat_ed_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/patch_transformer.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/patch_transformer.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/patch_transformer_framework.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/patch_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/peri_resnet.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/peri_resnet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/pos_embedding.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/pos_embedding.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/resnet.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/resnet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/self_attention.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/self_attention.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/siamese_feature_diff_model.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/siamese_feature_diff_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/siamese_fusion_model.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/siamese_fusion_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/simple_cnn_encoder.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/simple_cnn_encoder.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/simple_decoder.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/simple_decoder.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/timesformer.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/timesformer.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/unet.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/unet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/unet_lstm.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/unet_lstm.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/vit.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/models/vit.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/predict.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/predict_sc.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/predict_sc.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_misc.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/utils/util_misc.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_model.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/utils/util_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_paths.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/utils/util_paths.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_visualize.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_change_detection/utils/util_visualize.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/__init__.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/bigearthnet.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/bigearthnet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/deepglobe.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/deepglobe.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/dynamicearthnet.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/dynamicearthnet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/hrscd.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/hrscd.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/iarpa_contrastive_dataset.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/iarpa_contrastive_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/iarpa_dataset.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/iarpa_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/inria.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/inria.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/s2_self.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/s2_self.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/s2mcp.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/s2mcp.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/spacenet.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/spacenet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/spacenet2.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/spacenet2.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/sysucd.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/datasets/sysucd.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/bigearthnet_finetune.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/bigearthnet_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/change_vector_analysis.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/change_vector_analysis.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/cluster_labeling.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/cluster_labeling.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/compare_vw_maps.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/compare_vw_maps.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/deepglobe_finetune.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/deepglobe_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/deepglobe_train_val.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/deepglobe_train_val.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/dynamicearthnet_finetune.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/dynamicearthnet_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/evaluation_method_comparison.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/evaluation_method_comparison.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/hrscd_finetune.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/hrscd_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/iarpa_finetune.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/iarpa_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/inria_finetune.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/inria_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/moco_train.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/moco_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/moco_unsupervised_material.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/moco_unsupervised_material.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/mt_material_clustering_tranfer_learn.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/mt_material_clustering_tranfer_learn.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/multi_temporal_material_clustering.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/multi_temporal_material_clustering.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_fine_tune.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/onera_fine_tune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune2.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune2.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_patch_train.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/onera_patch_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_train.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/onera_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_net.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_net.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet_enc.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet_enc.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/setr_train.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/setr_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/shallow_seg_train.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/shallow_seg_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/sim_contrastive_train.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/sim_contrastive_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/spacenet2_finetune.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/spacenet2_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/supervised_clustering.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/supervised_clustering.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/sysu_patch_train.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/experiments/sysu_patch_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/__init__.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/canny_edge.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/canny_edge.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/deeplab.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/deeplab.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/deeplabWS.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/deeplabWS.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/deeplab_diff.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/deeplab_diff.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/encoding.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/encoding.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/gci.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/gci.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/linear_classifier.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/linear_classifier.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/losses.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/losses.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/moco.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/moco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/quantizer.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/quantizer.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnet.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/resnet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnetGNWS.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/resnetGNWS.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnet_classification_finetune.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/resnet_classification_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnet_enc.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/resnet_enc.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/sg.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/sg.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/shallow_seg.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/shallow_seg.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/supcon.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/supcon.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/tex_refine.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/tex_refine.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/transformer_model.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/transformer_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/transformer_seg.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/models/transformer_seg.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/predict.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/predict_patchwise.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/predict_patchwise.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/predict_test.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/predict_test.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/scripts/filter_by_sensor.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/scripts/filter_by_sensor.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/scripts/labelbox2coco.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/scripts/labelbox2coco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/convert_sysucd_to_kwcoco.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/utils/convert_sysucd_to_kwcoco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/cva.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/utils/cva.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/eval_utils.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/utils.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/visualization.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/__init__.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/base_dataset.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/image_dataset.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/datasets/image_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/material_pixel_dataset.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/datasets/material_pixel_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/models/material_mlp.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/models/material_mlp.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/predict.py` & `geowatch-0.6.6/watch/tasks/rutgers_material_seg_v2/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/sam/predict.py` & `geowatch-0.6.6/watch/tasks/sam/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/tracking/__init__.py` & `geowatch-0.6.6/watch/tasks/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/tracking/from_heatmap.py` & `geowatch-0.6.6/watch/tasks/tracking/from_heatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -986,26 +986,33 @@
         inner_window_size = None
 
     if isinstance(moving_window_size, float) and math.isnan(moving_window_size):
         moving_window_size = None
 
     if isinstance(inner_window_size, str):
         # TODO: generalize if needed
-        assert inner_agg_fn == 'mean'
         assert heatmap_dates is not None
+
+        if inner_agg_fn == 'mean':
+            inner_ord = 1
+        elif inner_agg_fn == 'max':
+            inner_ord = float('inf')
+        else:
+            raise NotImplementedError(inner_agg_fn)
+
         # Do inner aggregation before outer aggregation
         from watch.utils import util_time
         import kwarray
         delta = util_time.coerce_timedelta(inner_window_size).total_seconds()
         image_unixtimes = np.array([d.timestamp() for d in heatmap_dates])
         bucket_ids = (image_unixtimes // delta).astype(int)
         unique_ids, groupxs = kwarray.group_indices(bucket_ids)
         new_heatmaps = []
         for idxs in groupxs:
-            inner = _norm(heatmaps[idxs], norm_ord=1)
+            inner = _norm(heatmaps[idxs], norm_ord=inner_ord)
             new_heatmaps.append(inner)
         new_heatmaps = np.array(new_heatmaps)
         heatmaps = new_heatmaps
     else:
         if inner_window_size is not None:
             raise NotImplementedError(
                 'only temporal deltas for inner agg window for now')
```

### Comparing `geowatch-0.6.3/watch/tasks/tracking/from_polygon.py` & `geowatch-0.6.6/watch/tasks/tracking/from_polygon.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/tracking/normalize.py` & `geowatch-0.6.6/watch/tasks/tracking/normalize.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/tracking/phase.py` & `geowatch-0.6.6/watch/tasks/tracking/phase.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/tracking/utils.py` & `geowatch-0.6.6/watch/tasks/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/tracking/visualize.py` & `geowatch-0.6.6/watch/tasks/tracking/visualize.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/drop0_datasets.py` & `geowatch-0.6.6/watch/tasks/uky_temporal_prediction/drop0_datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/fit.py` & `geowatch-0.6.6/watch/tasks/uky_temporal_prediction/fit.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/resnets.py` & `geowatch-0.6.6/watch/tasks/uky_temporal_prediction/models/resnets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/unet.py` & `geowatch-0.6.6/watch/tasks/uky_temporal_prediction/models/unet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/unet_blur.py` & `geowatch-0.6.6/watch/tasks/uky_temporal_prediction/models/unet_blur.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/predict.py` & `geowatch-0.6.6/watch/tasks/uky_temporal_prediction/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/create_splits.py` & `geowatch-0.6.6/watch/tasks/uky_temporal_prediction/spacenet/data/create_splits.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/create_splits_unmasked.py` & `geowatch-0.6.6/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/create_splits_unmasked.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/datasets.py` & `geowatch-0.6.6/watch/tasks/uky_temporal_prediction/spacenet/datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/time_sort_S7.py` & `geowatch-0.6.6/watch/tasks/uky_temporal_prediction/time_sort_S7.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/time_sort_module.py` & `geowatch-0.6.6/watch/tasks/uky_temporal_prediction/time_sort_module.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/utils.py` & `geowatch-0.6.6/watch/tasks/uky_temporal_prediction/utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/__init__.py` & `geowatch-0.6.6/watch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/configargparse_ext.py` & `geowatch-0.6.6/watch/utils/configargparse_ext.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/ext_monai.py` & `geowatch-0.6.6/watch/utils/ext_monai.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     def __init__(
         self,
         include_background: bool = True,
         to_onehot_y: bool = False,
         gamma: float = 2.0,
         weight: Optional[Union[Sequence[float], float, int, torch.Tensor]] = None,
         reduction: Union[LossReduction, str] = LossReduction.MEAN,
+        ohem_ratio: Optional[float] = None,
     ) -> None:
         """
         Args:
             include_background: if False, channel index 0 (background category) is excluded from the calculation.
             to_onehot_y: whether to convert `y` into the one-hot format. Defaults to False.
             gamma: value of the exponent gamma in the definition of the Focal loss.
             weight: weights to apply to the voxels of each class. If None no weights are applied.
@@ -90,28 +91,30 @@
                 The value/values should be no less than 0. Defaults to None.
             reduction: {``"none"``, ``"mean"``, ``"sum"``}
                 Specifies the reduction to apply to the output. Defaults to ``"mean"``.
 
                 - ``"none"``: no reduction will be applied.
                 - ``"mean"``: the sum of the output will be divided by the number of elements in the output.
                 - ``"sum"``: the output will be summed.
+            ohem_ratio: whether to use OHEM (online hard example mining) to train the model. Defaults to None aka inactive.
 
         Example:
             >>> import torch
             >>> #from monai.losses import FocalLoss
             >>> pred = torch.tensor([[1, 0], [0, 1], [1, 0]], dtype=torch.float32)
             >>> grnd = torch.tensor([[0], [1], [0]], dtype=torch.int64)
             >>> fl = FocalLoss(to_onehot_y=True)
             >>> fl(pred, grnd)
         """
         super().__init__(reduction=LossReduction(reduction).value)
         self.include_background = include_background
         self.to_onehot_y = to_onehot_y
         self.gamma = gamma
         self.weight: Optional[Union[Sequence[float], float, int, torch.Tensor]] = weight
+        self.ohem_ratio = ohem_ratio
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         """
         Args:
             input: the shape should be BNH[WD], where N is the number of classes.
                 The input should be the original logits since it will be transformed by
                 a sigmoid in the forward function.
@@ -181,14 +184,25 @@
             ce = ce * at
 
         # Compute the loss mini-batch.
         # (1-p_t)^gamma * log(p_t) with reduced chance of overflow
         p = F.logsigmoid(-i * (t * 2.0 - 1.0))
         flat_loss: torch.Tensor = (p * self.gamma).exp() * ce
 
+        if self.ohem_ratio is not None:
+            # Compute Online Hard Example Mining (OHEM) loss based on "slow" method from
+            # https://arxiv.org/pdf/1604.03540.pdf
+
+            ## Find the top k% of regions with the highest loss and create a binary mask
+            ## to zero out the loss for the low loss regions.
+            mask = _ohem_mask(ce, self.ohem_ratio)
+
+            ## Apply the mask to the loss regions.
+            ce = ce * mask
+
         # Previously there was a mean over the last dimension, which did not
         # return a compatible BCE loss. To maintain backwards compatible
         # behavior we have a flag that performs this extra step, disable or
         # parameterize if necessary. (Or justify why the mean should be there)
         average_spatial_dims = True
 
         if self.reduction == LossReduction.SUM.value:
@@ -395,14 +409,21 @@
             input: the shape should be BNH[WD].
             target: the shape should be BNH[WD].
             mask: the shape should B1H[WD] or 11H[WD].
         """
         return self.spatial_weighted(input=input, target=target, mask=mask)
 
 
+def _ohem_mask(loss, ohem_ratio):
+    with torch.no_grad():
+        values, _ = torch.topk(loss.reshape(-1),
+                               int(loss.nelement() * ohem_ratio))
+        mask = loss >= values[-1]
+    return mask.float()
+
 # class GeneralizedDiceLoss(_Loss):
 #     """
 #     Compute the generalised Dice loss defined in:
 
 #         Sudre, C. et. al. (2017) Generalised Dice overlap as a deep learning
 #         loss function for highly unbalanced segmentations. DLMIA 2017.
 
@@ -926,14 +947,15 @@
         smooth_nr: float = 1e-5,
         smooth_dr: float = 1e-5,
         batch: bool = False,
         gamma: float = 2.0,
         focal_weight: Optional[Union[Sequence[float], float, int, torch.Tensor]] = None,
         lambda_dice: float = 1.0,
         lambda_focal: float = 1.0,
+        ohem_ratio_focal: Optional[float] = None,
     ) -> None:
         """
         Args:
             ``gamma``, ``focal_weight`` and ``lambda_focal`` are only used for focal loss.
             ``include_background``, ``to_onehot_y``and ``reduction`` are used for both losses
             and other parameters are only used for dice loss.
             include_background: if False channel index 0 (background category) is excluded from the calculation.
@@ -963,14 +985,16 @@
             focal_weight: weights to apply to the voxels of each class. If None no weights are applied.
                 The input can be a single value (same weight for all classes), a sequence of values (the length
                 of the sequence should be the same as the number of classes).
             lambda_dice: the trade-off weight value for dice loss. The value should be no less than 0.0.
                 Defaults to 1.0.
             lambda_focal: the trade-off weight value for focal loss. The value should be no less than 0.0.
                 Defaults to 1.0.
+            ohem_ratio_focal: Whether to use OHEM (online hard example mining) to train
+                the model during focal loss. Defaults to None aka inactive.
 
         """
         super().__init__()
         self.dice = DiceLoss(
             include_background=include_background,
             to_onehot_y=to_onehot_y,
             sigmoid=sigmoid,
@@ -985,14 +1009,15 @@
         )
         self.focal = FocalLoss(
             include_background=include_background,
             to_onehot_y=to_onehot_y,
             gamma=gamma,
             weight=focal_weight,
             reduction=reduction,
+            ohem_ratio=ohem_ratio_focal,
         )
         if lambda_dice < 0.0:
             raise ValueError("lambda_dice should be no less than 0.0.")
         if lambda_focal < 0.0:
             raise ValueError("lambda_focal should be no less than 0.0.")
         self.lambda_dice = lambda_dice
         self.lambda_focal = lambda_focal
```

### Comparing `geowatch-0.6.3/watch/utils/ijson_ext.py` & `geowatch-0.6.6/watch/utils/ijson_ext.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/kwcoco_extensions.py` & `geowatch-0.6.6/watch/utils/kwcoco_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,15 @@
         >>> dvc_dpath = find_smart_dvc_dpath()
         >>> coco_fpath = dvc_dpath / 'drop1-S2-L8-aligned/data.kwcoco.json'
         >>> coco_dset = kwcoco.CocoDataset(coco_fpath)
         >>> coco_populate_geo_heuristics(coco_dset, overwrite=True, workers=12,
         >>>                              keep_geotiff_metadata=False,
         >>>                              mode='process')
     """
+    import rich
     gids = coco_dset.images(gids)._ids
     # Cant multiprocess because of SwigPyObjects... bleh
     # keep_geotiff_metadata must be False to use mode=process
     keep_geotiff_metadata = kw.get('keep_geotiff_metadata', False)
     if keep_geotiff_metadata and mode == 'process':
         raise NotImplementedError(ub.paragraph(
             '''
@@ -260,21 +261,27 @@
             known_errors = [
                 has_404,
                 has_acc_problem,
                 connection_reset,
             ]
             if any(known_errors):
                 broken_image_ids.append(gid)
+                print('')
+                rich.print('[yellow]WARNING: KNOWN ERROR IN GEO HEURISTICS')
                 print(f'ex={ex!r}')
                 print(f'ex={ex}')
                 print(f'ex.__dict__={ex.__dict__}')
             else:
+                print('')
+                rich.print('[red]ERROR: UNKNOWN ERROR IN GEO HEURISTICS')
                 print(f'ex={ex!r}')
                 print(f'ex={ex}')
                 print(f'ex.__dict__={ex.__dict__}')
+                coco_img = coco_dset.coco_image(gid)
+                print('coco_img = {}'.format(ub.urepr(coco_img.img, nl=3)))
                 raise
         else:
             if mode == 'process':
                 # for multiprocessing
                 real_img = coco_dset.index.imgs[gid]
                 real_img.update(img)
     if broken_image_ids:
```

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/_jsonargparse_ext_ge_4_21.py` & `geowatch-0.6.6/watch/utils/lightning_ext/_jsonargparse_ext_ge_4_21.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/_jsonargparse_ext_lt_4_21.py` & `geowatch-0.6.6/watch/utils/lightning_ext/_jsonargparse_ext_lt_4_21.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/argparse_ext.py` & `geowatch-0.6.6/watch/utils/lightning_ext/argparse_ext.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/__init__.py` & `geowatch-0.6.6/watch/utils/lightning_ext/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/auto_resumer.py` & `geowatch-0.6.6/watch/utils/lightning_ext/callbacks/auto_resumer.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/batch_plotter.py` & `geowatch-0.6.6/watch/utils/lightning_ext/callbacks/batch_plotter.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/packager.py` & `geowatch-0.6.6/watch/utils/lightning_ext/callbacks/packager.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/state_logger.py` & `geowatch-0.6.6/watch/utils/lightning_ext/callbacks/state_logger.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/tensorboard_plotter.py` & `geowatch-0.6.6/watch/utils/lightning_ext/callbacks/tensorboard_plotter.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/text_logger.py` & `geowatch-0.6.6/watch/utils/lightning_ext/callbacks/text_logger.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/demo.py` & `geowatch-0.6.6/watch/utils/lightning_ext/demo.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/lightning_cli_ext.py` & `geowatch-0.6.6/watch/utils/lightning_ext/lightning_cli_ext.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/old_parser_devices.py` & `geowatch-0.6.6/watch/utils/lightning_ext/old_parser_devices.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/lightning_ext/util_device.py` & `geowatch-0.6.6/watch/utils/lightning_ext/util_device.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/partial_format.py` & `geowatch-0.6.6/watch/utils/partial_format.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/process_context.py` & `geowatch-0.6.6/watch/utils/process_context.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/result_analysis.py` & `geowatch-0.6.6/watch/utils/result_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -823,17 +823,20 @@
             else:
                 alternative = "two-sided"
 
             ind_kw = dict(
                 equal_var=False,
                 alternative=alternative,
             )
-            ttest_ind_result = scipy.stats.ttest_ind(
-                metric_vals1, metric_vals2, **ind_kw
-            )
+            with warnings.catch_warnings():
+                warnings.filterwarnings('ignore', 'Degrees of freedom', category=RuntimeWarning)
+                warnings.filterwarnings('ignore', 'invalid value', category=RuntimeWarning)
+                ttest_ind_result = scipy.stats.ttest_ind(
+                    metric_vals1, metric_vals2, **ind_kw
+                )
 
             if 0:
                 from benchmarker.benchmarker import stats_dict
 
                 stats1 = stats_dict(metric_vals1)
                 stats2 = stats_dict(metric_vals2)
                 scipy.stats.ttest_ind_from_stats(
```

### Comparing `geowatch-0.6.3/watch/utils/reverse_hashid.py` & `geowatch-0.6.6/watch/utils/reverse_hashid.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/simple_dvc.py` & `geowatch-0.6.6/watch/utils/simple_dvc.py`

 * *Files 14% similar despite different names*

```diff
@@ -98,33 +98,43 @@
         return self.dvc_root
 
     def _ensure_remote(self, remote):
         if remote is None:
             remote = self.remote
         return remote
 
+    def _resolve_root_and_relative_paths(self, paths):
+        # try:
+        #     dvc_root = self._ensure_root(paths)
+        #     rel_paths = [os.fspath(p.relative_to(dvc_root)) for p in paths]
+        # except Exception as ex:
+        #     print(f'ex={ex}')
+        # Handle symlinks: https://dvc.org/doc/user-guide/troubleshooting#add-symlink
+        # not sure if this is safe
+        dvc_root = self._ensure_root(paths).resolve()
+        # Note: this could resolve the symlink to the dvc cache which we dont want
+        # rel_paths = [os.fspath(p.resolve().relative_to(dvc_root)) for p in paths]
+        # Fixed version?
+        parent_resolved = [p.parent.resolve() / p.name for p in paths]
+        rel_paths = [os.fspath(p.relative_to(dvc_root)) for p in parent_resolved]
+
+        return dvc_root, rel_paths
+
     def add(self, path, verbose=0):
         """
         Args:
             path (str | PathLike | Iterable[str | PathLike]):
                 a single or multiple paths to add
         """
         from dvc import main as dvc_main
         paths = list(map(ub.Path, _ensure_iterable(path)))
         if len(paths) == 0:
             print('No paths to add')
             return
-        if 1:
-            # Handle symlinks: https://dvc.org/doc/user-guide/troubleshooting#add-symlink
-            # not sure if this is safe
-            dvc_root = self._ensure_root(paths).resolve()
-            rel_paths = [os.fspath(p.resolve().relative_to(dvc_root)) for p in paths]
-        else:
-            dvc_root = self._ensure_root(paths)
-            rel_paths = [os.fspath(p.relative_to(dvc_root)) for p in paths]
+        dvc_root, rel_paths = self._resolve_root_and_relative_paths(paths)
         with util_path.ChDir(dvc_root):
             dvc_command = ['add'] + rel_paths
             extra_args = self._verbose_extra_args(verbose)
             dvc_command = dvc_command + extra_args
             ret = dvc_main.main(dvc_command)
         if ret != 0:
             raise Exception('Failed to add files')
@@ -135,16 +145,15 @@
 
     def check_ignore(self, path, details=0, verbose=0):
         from dvc import main as dvc_main
         paths = list(map(ub.Path, _ensure_iterable(path)))
         if len(paths) == 0:
             print('No paths to add')
             return
-        dvc_root = self._ensure_root(paths)
-        rel_paths = [os.fspath(p.relative_to(dvc_root)) for p in paths]
+        dvc_root, rel_paths = self._resolve_root_and_relative_paths(paths)
         with util_path.ChDir(dvc_root):
             dvc_command = ['check-ignore'] + rel_paths
             if details:
                 dvc_command += ['--details']
             extra_args = self._verbose_extra_args(verbose)
             dvc_command = dvc_command + extra_args
             ret = dvc_main.main(dvc_command)
@@ -219,31 +228,31 @@
         """
         from dvc import main as dvc_main
         paths = list(map(ub.Path, _ensure_iterable(path)))
         if len(paths) == 0:
             print('No paths to push')
             return
         remote = self._ensure_remote(remote)
-        dvc_root = self._ensure_root(paths)
+        dvc_root, rel_paths = self._resolve_root_and_relative_paths(paths)
         extra_args = self._remote_extra_args(remote, recursive, jobs, verbose)
         with util_path.ChDir(dvc_root):
-            dvc_command = ['push'] + extra_args + [str(p.relative_to(dvc_root)) for p in paths]
+            dvc_command = ['push'] + extra_args + [str(p) for p in rel_paths]
             dvc_main.main(dvc_command)
 
     def pull(self, path, remote=None, recursive=False, jobs=None, verbose=0):
         from dvc import main as dvc_main
         paths = list(map(ub.Path, _ensure_iterable(path)))
         if len(paths) == 0:
             print('No paths to pull')
             return
         remote = self._ensure_remote(remote)
-        dvc_root = self._ensure_root(paths)
+        dvc_root, rel_paths = self._resolve_root_and_relative_paths(paths)
         extra_args = self._remote_extra_args(remote, recursive, jobs, verbose)
         with util_path.ChDir(dvc_root):
-            dvc_command = ['pull'] + extra_args + [str(p.relative_to(dvc_root)) for p in paths]
+            dvc_command = ['pull'] + extra_args + [str(p) for p in rel_paths]
             dvc_main.main(dvc_command)
 
     def request(self, path, remote=None):
         """
         Requests to ensure that a specific file from DVC exists.
 
         Any files that do not exist, check to see if there is an associated
@@ -255,30 +264,29 @@
                 one or more file paths that should have an associated .dvc
                 sidecar file.
         """
         paths = list(map(ub.Path, _ensure_iterable(path)))
         missing_data = [path for path in paths if not path.exists()]
 
         if missing_data:
-            dvc_root = self._ensure_root(paths)
+            dvc_root, rel_paths = self._resolve_root_and_relative_paths(missing_data)
 
-            def _find_sidecar(path):
-                first_cand = path.augment(stem=path.name, ext='.dvc')
+            def _find_sidecar(rel_path):
+                first_cand = dvc_root / rel_path.augment(stem=rel_path.name, ext='.dvc')
                 if first_cand.exists():
                     return first_cand
-                rel_path = path.relative_to(dvc_root)
                 rel_parts = rel_path.parts
                 for i in reversed(range(len(rel_parts))):
                     parts = rel_parts[0:i]
                     cand_dat = dvc_root.joinpath(*parts)
                     cand_dvc = cand_dat.augment(stem=cand_dat.name, ext='.dvc')
                     if cand_dvc.exists():
                         return cand_dvc
 
-            to_pull = [_find_sidecar(path) for path in missing_data]
+            to_pull = [_find_sidecar(rel_path) for rel_path in rel_paths]
             missing_sidecar = [dvc_fpath for dvc_fpath in to_pull if not dvc_fpath.exists()]
 
             if missing_sidecar:
                 if len(missing_sidecar) < 10:
                     print(f'missing_sidecar={missing_sidecar}')
                 raise Exception(f'There were {len(missing_sidecar)} / {len(paths)} missing sidecar files')
 
@@ -287,16 +295,15 @@
 
     def unprotect(self, path):
         from dvc import main as dvc_main
         paths = list(map(ub.Path, _ensure_iterable(path)))
         if len(paths) == 0:
             print('No paths to unprotect')
             return
-        dvc_root = self._ensure_root(paths)
-        rel_paths = [os.fspath(p.relative_to(dvc_root)) for p in paths]
+        dvc_root, rel_paths = self._resolve_root_and_relative_paths(paths)
         with util_path.ChDir(dvc_root):
             dvc_command = ['unprotect'] + rel_paths
             dvc_main.main(dvc_command)
 
     def is_tracked(self, path):
         path = ub.Path(path)
         tracker_fpath = self.find_file_tracker(path)
```

### Comparing `geowatch-0.6.3/watch/utils/slugify_ext.py` & `geowatch-0.6.6/watch/utils/slugify_ext.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_bands.py` & `geowatch-0.6.6/watch/utils/util_bands.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_codes.py` & `geowatch-0.6.6/watch/utils/util_codes.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_data.py` & `geowatch-0.6.6/watch/utils/util_data.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_dotdict.py` & `geowatch-0.6.6/watch/utils/util_dotdict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_environ.py` & `geowatch-0.6.6/watch/utils/util_environ.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_framework.py` & `geowatch-0.6.6/watch/utils/util_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_gdal.py` & `geowatch-0.6.6/watch/utils/util_gdal.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     https://trac.osgeo.org/gdal/wiki/ConfigOptions#GDAL_PAM_ENABLED
     https://gdal.org/drivers/raster/gtiff.html#georeferencing
 """
 import kwimage
 import os
 import ubelt as ub
 import subprocess
+import functools
 import retry
 
 
 GDAL_VIRTUAL_FILESYSTEM_PREFIX = '/vsi'
 
 # https://gdal.org/user/virtual_file_systems.
 # GDAL_VIRTUAL_FILESYSTEMS = [
@@ -57,29 +58,44 @@
 #     {'prefix': 'vsimem', 'type': None},
 #     {'prefix': 'vsisubfile', 'type': None},
 #     {'prefix': 'vsisparse', 'type': None},
 #     {'prefix': 'vsicrypt', 'type': None},
 # ]
 
 
+@functools.cache
+def import_gdal():
+    from osgeo import gdal
+    if not getattr(gdal, '_UserHasSpecifiedIfUsingExceptions', lambda: False)():
+        gdal.UseExceptions()
+    return gdal
+
+
+@functools.cache
+def import_osr():
+    from osgeo import osr
+    if not getattr(osr, '_UserHasSpecifiedIfUsingExceptions', lambda: False)():
+        osr.UseExceptions()
+    return osr
+
+
 class DummyLogger:
     def warning(self, msg, *args):
         print(msg % args)
 
 
 def _demo_geoimg_with_nodata():
     """
     Example:
         fpath = _demo_geoimg_with_nodata()
         self = LazyGDalFrameFile.demo()
 
     """
     import numpy as np
-    from osgeo import osr
-    # gdal.UseExceptions()
+    osr = import_osr()
 
     # Make a dummy geotiff
     imdata = kwimage.grab_test_image('airport')
     dpath = ub.Path.appdir('watch/test/geotiff').ensuredir()
     geo_fpath = dpath / 'dummy_geotiff.tif'
 
     # compute dummy values for a geotransform to CRS84
@@ -278,15 +294,16 @@
         self['-of'] = 'COG'
         self.options['-co']['OVERVIEWS'] = str(overviews)
         self.options['-co']['BLOCKSIZE'] = str(blocksize)
         self.options['-co']['COMPRESS'] = compress
 
 
 def gdal_single_translate(in_fpath, out_fpath, pixel_box=None, blocksize=256,
-                          compress='DEFLATE', tries=1, verbose=0, eager=True):
+                          compress='DEFLATE', tries=1, cooldown=1, verbose=0,
+                          eager=True, gdal_cachemax=None, num_threads=None):
     """
     Crops geotiffs using pixels
 
     Args:
         in_fpath (PathLike): geotiff to translate
 
         out_fpath (PathLike): output geotiff
@@ -295,14 +312,16 @@
 
         blocksize (int): COG tile size
 
         compress (str): gdal compression
 
         verbose (int): verbosity level
 
+        cooldown (int): number of seconds to wait (i.e. "cool-down") between tries
+
         eager (bool):
             if True, executes the command, if False returns a list of all the
             bash commands that would be executed, suitable for use in a command
             queue.
 
     CommandLine:
         xdoctest -m watch.utils.util_gdal gdal_single_translate
@@ -366,30 +385,34 @@
     tmp_fpath = ub.Path(ub.augpath(out_fpath, prefix='.tmptrans.'))
 
     builder = GDalCommandBuilder('gdal_translate')
     # builder['--debug'] = 'off'
     builder.set_cog_options(compress=compress, blocksize=blocksize)
     # Use the new COG output driver
     # Perf options
-    if 1:
+    if gdal_cachemax is not None:
         # TODO: these probably should be environment variables?
-        builder.options['--config']['GDAL_CACHEMAX'] = '15%'
-        builder.options['-co']['NUM_THREADS'] = 'ALL_CPUS'
+        # '1500'  # '15%'
+        builder.options['--config']['GDAL_CACHEMAX'] = str(gdal_cachemax)
+
+    if num_threads is not None:
+        builder.options['-co']['NUM_THREADS'] = str(num_threads)  # 'ALL_CPUS'
 
     if pixel_box is not None:
         xoff, yoff, xsize, ysize = pixel_box.to_xywh().data[0]
         builder['-srcwin'] = [f'{xoff}', f'{yoff}', f'{xsize}', f'{ysize}']
 
     builder.append(f'{in_fpath}')
     builder.append(f'{tmp_fpath}')
     gdal_translate_command = builder.finalize()
 
     if eager:
         _execute_gdal_command_with_checks(
-            gdal_translate_command, tmp_fpath, tries=tries, verbose=verbose)
+            gdal_translate_command, tmp_fpath, tries=tries, cooldown=cooldown,
+            verbose=verbose)
         os.rename(tmp_fpath, out_fpath)
     else:
         commands = [
             gdal_translate_command,
             f'mv "{tmp_fpath}" "{out_fpath}"',
         ]
         return commands
@@ -407,15 +430,20 @@
                      as_vrt=False,
                      use_te_geoidgrid=False,
                      dem_fpath=None,
                      error_logfile=None,
                      tries=1,
                      verbose=0,
                      force_spatial_res=None,
-                     eager=True):
+                     eager=True,
+                     cooldown=1,
+                     use_tempfile=True,
+                     gdal_cachemax=None,
+                     num_threads=None,
+                     warp_memory=None):
     r"""
     Wrapper around gdalwarp
 
     Args:
         in_fpath (PathLike): input geotiff path
 
         out_fpath (PathLike): output geotiff path
@@ -456,14 +484,16 @@
             resolution for output images.
 
         eager (bool):
             if True, executes the command, if False returns a list of all the
             bash commands that would be executed, suitable for use in a command
             queue.
 
+        cooldown (int): number of seconds to wait (i.e. "cool-down") between tries
+
     Returns:
         None | List[str]:
             Nothing if executing the command. If eager=False, returns the
             commands that would have been executed.
 
     Notes:
         In gdalwarp:
@@ -574,16 +604,21 @@
     if as_vrt:
         builder['-of'] = 'VRT'
     else:
         builder.set_cog_options(compress=compress, blocksize=blocksize,
                                 overviews='AUTO')
 
     if space_box is not None:
+
         # Data is from geo-pandas so this should be traditional order
-        lonmin, latmin, lonmax, latmax = space_box.data[0]
+        ltrb = space_box.to_ltrb()
+        if isinstance(ltrb, kwimage.Box):
+            lonmin, latmin, lonmax, latmax = ltrb.data
+        else:
+            lonmin, latmin, lonmax, latmax = ltrb.data[0]
         ymin, xmin, ymax, xmax = latmin, lonmin, latmax, lonmax
 
         # Coordinate Reference System of the "te" crop coordinates
         # te_srs = spatial reference of query points
         # This means space_box currently MUST be in CRS84
         # crop_coordinate_srs = 'epsg:4326'
         crop_coordinate_srs = f'epsg:{box_epsg}'
@@ -635,45 +670,59 @@
     #     config_options['GDAL_CACHEMAX'] = '15%'
     #     common_options['NUM_THREADS'] = 'ALL_CPUS'
     #     warp_options['NUM_THREADS'] = '1'
     #     builder.options['-wo']['NUM_THREADS'] = '1'
     # else:
     # GDAL_CACHEMAX is in megabytes
     # https://gdal.org/programs/gdalwarp.html#cmdoption-gdalwarp-wm
-    warp_memory = '1500'
-    builder['-wm'] = str(warp_memory)
-    builder.options['-co']['NUM_THREADS'] = '2'
-    builder.options['--config']['GDAL_CACHEMAX'] = '1500'
+    if warp_memory is not None:
+        builder['-wm'] = str(warp_memory)
+    if num_threads is not None:
+        builder.options['-co']['NUM_THREADS'] = str(num_threads)
+    if gdal_cachemax is not None:
+        builder.options['--config']['GDAL_CACHEMAX'] = str(gdal_cachemax)
 
     builder.append(in_fpath)
-    builder.append(tmp_out_fpath)
+    if use_tempfile:
+        dst_fpath = tmp_out_fpath
+        builder.append(tmp_out_fpath)
+    else:
+        dst_fpath = out_fpath
+        builder.append(out_fpath)
 
     gdal_warp_command = builder.finalize()
 
     # Execute the command with checks to ensure gdal doesnt fail
     if eager:
         _execute_gdal_command_with_checks(
-            gdal_warp_command, tmp_out_fpath, tries=tries, verbose=verbose)
-        os.rename(tmp_out_fpath, out_fpath)
+            gdal_warp_command, dst_fpath, tries=tries, verbose=verbose,
+            cooldown=cooldown)
+        if use_tempfile:
+            os.rename(tmp_out_fpath, out_fpath)
     else:
-        commands = [
-            gdal_warp_command,
-            f'mv "{tmp_out_fpath}" "{out_fpath}"',
-        ]
+        commands = [gdal_warp_command]
+        if use_tempfile:
+            commands += [
+                f'mv "{tmp_out_fpath}" "{out_fpath}"'
+            ]
         return commands
 
 
-def gdal_multi_warp(in_fpaths, out_fpath, nodata=None, tries=1, blocksize=256,
-                    compress='DEFLATE', error_logfile=None,
+def gdal_multi_warp(in_fpaths, out_fpath, nodata=None, tries=1, cooldown=1,
+                    blocksize=256, compress='DEFLATE', error_logfile=None,
                     _intermediate_vrt=False, verbose=0,
                     return_intermediate=False, force_spatial_res=None,
-                    eager=True, **kwargs):
+                    eager=True, gdal_cachemax=None, num_threads=None,
+                    warp_memory=None, **kwargs):
     """
     See gdal_single_warp() for args
 
+    NOTE: it is important to set the nodata argument for gdalmerge [SO187522]_
+    if you want to preserver them.
+
     Example:
         >>> # xdoctest: +REQUIRES(--slow)
         >>> # Uses data from the data cube with extra=1
         >>> from watch.utils.util_gdal import *  # NOQA
         >>> import ubelt as ub
         >>> cube, region_df = SimpleDataCube.demo(with_region=True, extra=True)
         >>> local_epsg = 32635
@@ -729,14 +778,17 @@
         >>> print('commands = {}'.format(ub.urepr(commands, nl=1)))
 
     Returns:
         None | List[str]:
             Nothing if executing the command. If eager=False, returns the
             commands that would have been executed.
 
+    References:
+        .. [SO187522] https://gis.stackexchange.com/questions/187522/keep-nodata-values-when-using-gdal-merge
+
     Ignore:
         import os
         import kwimage
         raw_in_fpaths = [
             '/vsis3/smart-data-accenture/ta-1/ta1-s2-acc/17/S/QD/2017/4/9/S2A_17SQD_20170409_0_L1C_ACC/S2A_17SQD_20170409_0_L1C_ACC_B02.tif',
             '/vsis3/smart-data-accenture/ta-1/ta1-s2-acc/18/S/TJ/2017/4/9/S2A_18STJ_20170409_0_L1C_ACC/S2A_18STJ_20170409_0_L1C_ACC_B02.tif',
         ]
@@ -773,19 +825,23 @@
     # Destination so ctrl+c doesn't break everything
     tmp_out_fpath = ub.augpath(out_fpath, prefix='.tmpmerge.')
 
     single_warp_kwargs = kwargs.copy()
     single_warp_kwargs['compress'] = compress
     single_warp_kwargs['blocksize'] = blocksize
     single_warp_kwargs['tries'] = tries
+    single_warp_kwargs['cooldown'] = cooldown
     single_warp_kwargs['nodata'] = nodata
     single_warp_kwargs['verbose'] = verbose
     single_warp_kwargs['error_logfile'] = error_logfile
     single_warp_kwargs['force_spatial_res'] = force_spatial_res
     single_warp_kwargs['eager'] = eager
+    single_warp_kwargs['gdal_cachemax'] = gdal_cachemax
+    single_warp_kwargs['warp_memory'] = warp_memory
+    single_warp_kwargs['num_threads'] = num_threads
     # Delay the actual execution of the partial warps until merge is called.
 
     commands = []
 
     if _intermediate_vrt:
         # Not using the intermediate VRT is faster.
         # Building the VRT requires network calls, so might as well
@@ -828,52 +884,61 @@
         warped_gpaths = warped_gpaths[::-1]
     else:
         # Last image is copied over earlier ones, but we expect first image to
         # be the primary one, so reverse order
         warped_gpaths = warped_gpaths[::-1]
 
     builder = GDalCommandBuilder('gdal_merge.py')
-    builder.options['-co']['NUM_THREADS'] = '2'
-    builder.options['--config']['GDAL_CACHEMAX'] = '1500'
+    if num_threads is not None:
+        builder.options['-co']['NUM_THREADS'] = str(num_threads)
+    if gdal_cachemax is not None:
+        builder.options['--config']['GDAL_CACHEMAX'] = str(gdal_cachemax)
     # builder.set_cog_options()
     if error_logfile is not None:
         builder.options['--config']['CPL_LOG'] = error_logfile
     if nodata is not None:
         builder['-n'] = str(nodata)
+        builder['-a_nodata'] = str(nodata)
+        builder['-init'] = str(nodata)
     builder['-o'] = tmp_out_fpath
     builder.extend(warped_gpaths)
 
     gdal_merge_cmd = builder.finalize()
 
     if eager:
         _execute_gdal_command_with_checks(
-            gdal_merge_cmd, tmp_out_fpath, tries=tries, verbose=verbose)
+            gdal_merge_cmd, tmp_out_fpath, tries=tries, cooldown=cooldown,
+            verbose=verbose)
     else:
         commands.append(gdal_merge_cmd)
 
     # Merge does not output cogs, we need to do another call to make that
     # happen
     tmp_out_fpath2 = ub.augpath(out_fpath, prefix='.tmpcog.')
     _cmd = gdal_single_translate(tmp_out_fpath, tmp_out_fpath2,
                                  compress=compress, blocksize=blocksize,
-                                 verbose=verbose, eager=eager)
+                                 verbose=verbose, eager=eager, tries=tries,
+                                 cooldown=cooldown,
+                                 gdal_cachemax=gdal_cachemax,
+                                 num_threads=num_threads)
     if eager:
         ub.Path(tmp_out_fpath).delete()
         os.rename(tmp_out_fpath2, out_fpath)
     else:
         commands.extend(_cmd)
         commands.append(f'rm "{tmp_out_fpath}"')
         commands.append(f'mv "{tmp_out_fpath2}" "{out_fpath}"')
 
     if not eager:
         return commands
 
 
-def _execute_gdal_command_with_checks(command, out_fpath, tries=1, shell=False,
-                                      check_after=True, verbose=0):
+def _execute_gdal_command_with_checks(command, out_fpath, tries=1, cooldown=1,
+                                      shell=False, check_after=True,
+                                      verbose=0):
     """
     Given a gdal command and the expected file that it should produce
     try to execute a few times and check that it produced a valid result.
     """
 
     def _execute_command():
         cmd_info = ub.cmd(command, check=True, verbose=verbose, shell=shell)
@@ -886,15 +951,15 @@
                 raise
         return cmd_info
     got = -1
     try:
         logger = DummyLogger()
         got = retry.api.retry_call(
             _execute_command,
-            tries=tries, delay=1, exceptions=(
+            tries=tries, delay=cooldown, exceptions=(
                 subprocess.CalledProcessError, FileNotFoundError,
                 RuntimeError),
             logger=logger)
     except subprocess.CalledProcessError as ex:
         if verbose:
             print('\n\nCOMMAND FAILED: {!r}'.format(ex.cmd))
             print(ex.stdout)
@@ -927,15 +992,15 @@
 
     Example:
         >>> from watch.utils.util_gdal import *
         >>> drivers = list_gdal_drivers()
         >>> print('drivers = {}'.format(ub.urepr(drivers, nl=1)))
         >>> assert ('GTiff', 'GeoTIFF', ['tif', 'tiff']) in drivers
     """
-    from osgeo import gdal
+    gdal = import_gdal()
     result = []
     for idx in range(gdal.GetDriverCount()):
         driver = gdal.GetDriver(idx)
         if driver:
             metadata = driver.GetMetadata()
             if metadata.get(gdal.DCAP_CREATE) == 'YES' and metadata.get(
                     gdal.DCAP_RASTER) == 'YES':
@@ -1106,19 +1171,29 @@
         Do not call this method directly. Use `GdalDataset.open`
         """
         self.__ref = __ref  # This is a private variable
         self._path = _path
         self._str_mode = _str_mode
 
     @classmethod
-    def open(cls, path, mode='r', virtual_retries=3):
+    def open(cls, path, mode='r', virtual_retries=3, cooldown=0.1):
         """
-        Create a new dataset
+        Create a new dataset in read or write mode.
+
+        Args:
+            path (str | PathLike): the path or URI to open
+            mode (str): either 'r' for read only or 'w+' for update mode.
+            virtual_retries (int): number of times to attempt to open the
+                dataset when the URI points to a non-local resource
+            cooldown (float): seconds between retry attempts
+
+        Returns:
+            GdalDataset
         """
-        from osgeo import gdal
+        gdal = import_gdal()
         _path = os.fspath(path)
 
         if isinstance(mode, str):
             # https://mkyong.com/python/python-difference-between-r-w-and-a-in-open/
             if mode in {'readonly', 'r'}:
                 mode = gdal.GA_ReadOnly
             elif mode == {'update', 'w+'}:
@@ -1140,36 +1215,35 @@
                 # gdal.GetLastErrorType()
                 # gdal.GetLastErrorNo()
                 msg = gdal.GetLastErrorMsg()
                 raise RuntimeError(msg + f' for {_path}')
         except Exception:
             import time
             if _path.startswith(GDAL_VIRTUAL_FILESYSTEM_PREFIX):
-                wait_time = 0.1
                 for _ in range(virtual_retries):
                     try:
                         __ref = gdal.Open(_path, mode)
                         if __ref is None:
                             msg = gdal.GetLastErrorMsg()
                             raise RuntimeError(msg + f' for {_path}')
                     except Exception:
-                        time.sleep(wait_time)
+                        time.sleep(cooldown)
                     else:
                         break
             if __ref is None:
                 raise
         self = cls(__ref, _path, _str_mode)
         return self
 
     @classmethod
     def coerce(cls, data, mode=None, **kwargs):
         """
         Ensures the underlying object is a gdal dataset.
         """
-        from osgeo import gdal
+        gdal = import_gdal()
         import pathlib
         if mode is None:
             mode = gdal.GA_ReadOnly
         if isinstance(data, str):
             ref = cls.open(data, mode, **kwargs)
         elif isinstance(data, pathlib.Path):
             ref = cls.open(data, mode, **kwargs)
@@ -1238,25 +1312,25 @@
         """
         Exiting the context manager forces the gdal object closed.
         """
         self.close()
 
     def info(self):
         """
-        Information similar to gdalinfo
+        Information similar to gdalinfo (in json format)
         """
         # https://gdal.org/api/python/osgeo.gdal.html#osgeo.gdal.AsyncReader
         # osgeo.gdal.InfoOptions(options=None, format='text', deserialize=True,
         #                computeMinMax=False, reportHistograms=False,
         #                reportProj4=False, stats=False, approxStats=False,
         #                computeChecksum=False, showGCPs=True, showMetadata=True,
         #                showRAT=True, showColorTable=True, listMDD=False,
         #                showFileList=True, allMetadata=False,
         #                extraMDDomains=None, wktFormat=None)
-        from osgeo import gdal
+        gdal = import_gdal()
         info = gdal.Info(self, format='json', allMetadata=True, listMDD=True)
         # info = gdal.Info(self)
         # info = gdal.Info(self, allMetadata=True, listMDD=True)
         return info
 
     def get_overview_info(self):
         """
@@ -1271,11 +1345,10 @@
         return overview_counts
 
     def get_all_metadata(self):
         """
         References:
             https://gdal.org/user/raster_data_model.html
         """
-
         domain_to_metadata = {}
         for domain in self.GetMetadataDomainList():
             domain_to_metadata[domain] = self.GetMetadata(domain)
```

### Comparing `geowatch-0.6.3/watch/utils/util_girder.py` & `geowatch-0.6.6/watch/utils/util_girder.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_gis.py` & `geowatch-0.6.6/watch/utils/util_gis.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_globals.py` & `geowatch-0.6.6/watch/utils/util_globals.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,31 +14,34 @@
         config (dict): exected to contain certain special keys.
 
             * "workers" with an integer value equal to the number of dataloader
                 processes.
 
             * "torch_sharing_strategy" to specify the torch multiprocessing backend
 
-        **kw: can also be used to specify config items
+            * "request_rlimit_nofile"
+                the maximum number of open files to request ulimit raise the
+                soft limit to.
 
     Modules we currently hack:
         * cv2 - fix thread count
         * torch sharing strategy
 
     References:
         https://pytorch.org/docs/stable/multiprocessing.html#torch.multiprocessing.get_all_sharing_strategies
     """
 
     num_workers = config.get('num_workers', None)
     num_workers = coerce_num_workers(num_workers)
     if num_workers is not None and num_workers > 0:
         import cv2
         cv2.setNumThreads(0)
-        request_nofile_limits()
-        want_shm_per_worker = 0.5
+        request_rlimit_nofile = config.get('request_rlimit_nofile', 'auto')
+        request_nofile_limits(request_rlimit_nofile=request_rlimit_nofile)
+        want_shm_per_worker = 0.5  # gibibytes
         want_shm = want_shm_per_worker * num_workers
         try:
             check_shm_limits(want_shm)
         except IOError as ex:
             import warnings
             warnings.warn(str(ex))
```

### Comparing `geowatch-0.6.3/watch/utils/util_hardware.py` & `geowatch-0.6.6/watch/utils/util_hardware.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_iter.py` & `geowatch-0.6.6/watch/utils/util_iter.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_json.py` & `geowatch-0.6.6/watch/utils/util_json.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_kwarray.py` & `geowatch-0.6.6/watch/utils/util_kwarray.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_kwimage.py` & `geowatch-0.6.6/watch/utils/util_kwimage.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_kwplot.py` & `geowatch-0.6.6/watch/utils/util_kwplot.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_locks.py` & `geowatch-0.6.6/watch/utils/util_locks.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_logging.py` & `geowatch-0.6.6/watch/utils/util_logging.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_nesting.py` & `geowatch-0.6.6/watch/utils/util_nesting.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_netharn.py` & `geowatch-0.6.6/watch/utils/util_netharn.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_nvidia.py` & `geowatch-0.6.6/watch/utils/util_nvidia.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_pandas.py` & `geowatch-0.6.6/watch/utils/util_pandas.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_parallel.py` & `geowatch-0.6.6/watch/utils/util_parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         >>> print(coerce_num_workers('all'))
         >>> print(coerce_num_workers('avail'))
         >>> print(coerce_num_workers('auto'))
         >>> print(coerce_num_workers('all-2'))
         >>> print(coerce_num_workers('avail-2'))
         >>> print(coerce_num_workers('all/2'))
         >>> print(coerce_num_workers('min(all,2)'))
-        >>> print(coerce_num_workers('[max(all,2)][0]'))
+        >>> #print(coerce_num_workers('[max(all,2)][0]'))
         >>> import pytest
         >>> with pytest.raises(Exception):
         >>>     print(coerce_num_workers('all + 1' + (' + 1' * 100)))
         >>> total_cpus = coerce_num_workers('all')
         >>> assert coerce_num_workers('all-2') == max(total_cpus - 2, 0)
         >>> assert coerce_num_workers('all-100') == max(total_cpus - 100, 0)
         >>> assert coerce_num_workers('avail') <= coerce_num_workers('all')
```

### Comparing `geowatch-0.6.3/watch/utils/util_param_grid.py` & `geowatch-0.6.6/watch/utils/util_param_grid.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_path.py` & `geowatch-0.6.6/watch/utils/util_path.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_pattern.py` & `geowatch-0.6.6/watch/utils/util_pattern.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_progress.py` & `geowatch-0.6.6/watch/utils/util_progress.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_raster.py` & `geowatch-0.6.6/watch/utils/util_raster.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_regex.py` & `geowatch-0.6.6/watch/utils/util_regex.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_resolution.py` & `geowatch-0.6.6/watch/utils/util_resolution.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_resources.py` & `geowatch-0.6.6/watch/utils/util_resources.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Utilities to configure / inspect system resources
 """
 
 
-def request_nofile_limits(requested_limit='auto'):
+def request_nofile_limits(request_rlimit_nofile='auto', requested_limit=None):
     """
     Attempts to increase the limit of open file descriptors on the system.
 
+    Does nothing on non-linux operating systems.
+
     Args:
-        requested_limit (int | str):
+        request_rlimit_nofile (int | str):
             attempt to increase rlimit_nofile to this number of open files,
-            if auto, uses a hueristic
+            if auto, uses a hueristic, which currently defaults to 8192.
 
     Ignore:
         # Helpful file descriptor monitor script:
         watch -x bash -c '
             PROC_ID_LIST=($(ps -a | grep python | awk '"'"'{print $1}'"'"' ))
             for PROC_ID in "${PROC_ID_LIST[@]}"; do
                 NUM_OPEN_FILES=$(lsof -p $PROC_ID | wc -l)
@@ -32,46 +34,59 @@
         ulimit -S -n 8192
 
     Example:
         >>> from watch.utils import util_resources
         >>> util_resources.request_nofile_limits()
     """
     import ubelt as ub
+
+    if requested_limit is not None:
+        ub.schedule_deprecation(
+            'watch', 'requested_limit', 'arg',
+            migration='Use request_rlimit_nofile instead',
+            deprecate='0.6.4', error='0.7.0', remove='0.8.0')
+        request_rlimit_nofile = requested_limit
+
     if ub.LINUX:
         import resource
-        if isinstance(requested_limit, str):
-            if requested_limit == 'auto':
-                requested_limit = 8192
+        if isinstance(request_rlimit_nofile, str):
+            if request_rlimit_nofile == 'auto':
+                request_rlimit_nofile = 8192
             else:
-                raise KeyError(requested_limit)
+                raise KeyError(request_rlimit_nofile)
         soft, hard = resource.getrlimit(resource.RLIMIT_NOFILE)
-        if requested_limit > soft:
-            print('Requesting FileLimit = {!r}'.format(requested_limit))
+        if request_rlimit_nofile > soft:
+            print('Requesting FileLimit = {!r}'.format(request_rlimit_nofile))
             print(' * Before FileLimit: soft={}, hard={}'.format(soft, hard))
             try:
-                resource.setrlimit(resource.RLIMIT_NOFILE, (requested_limit, hard))
+                resource.setrlimit(resource.RLIMIT_NOFILE, (request_rlimit_nofile, hard))
             except Exception as ex:
                 print(f'ERROR ex={ex}')
             soft, hard = resource.getrlimit(resource.RLIMIT_NOFILE)
             print(' * After FileLimit: soft={}, hard={}'.format(soft, hard))
 
 
 def check_shm_limits(threshold_gibibytes=1):
     """
     When running training in docker you may need more shared memory than
     its default provide. Warns if shared memory is not above a threshold.
 
+    Args:
+        threshold_gibibytes (float):
+            The amount of shared memory we want to have access to.
+
     Notes:
-        Running docker run with `--shm-size=32768m` increases shm to 32GB
+        Running docker run with ``--shm-size=32768m`` increases shm to 32GB
 
     Raises:
         IOError: if the system does not have a /dev/shm device.
 
     References:
-        https://stackoverflow.com/questions/30210362/how-to-increase-the-size-of-the-dev-shm-in-docker-container
+        .. [SO30210362] https://stackoverflow.com/questions/30210362/how-to-increase-the-size-of-the-dev-shm-in-docker-container
+        .. [SO58804022] https://stackoverflow.com/questions/58804022/how-to-resize-dev-shm
     """
     import ubelt as ub
     import psutil
 
     shm = ub.Path('/dev/shm')
     if shm.exists():
         usage = psutil.disk_usage(shm)
@@ -80,16 +95,26 @@
         raise IOError('Dont know how to check shm size on this system')
 
     # shm_gigabytes = (shm_bytes / 10 ** 9)
     shm_gibibytes = (shm_bytes / 2 ** 30)
 
     if shm_gibibytes < threshold_gibibytes:
         import warnings
+        import math
+        thresh_mb = math.ceil(threshold_gibibytes * (2 ** 30 / 10 ** 6))
         print(f'shm_gibibytes={shm_gibibytes}')
-        warnings.warn('Likely do not have enough /dev/shm space')
+        warnings.warn(ub.paragraph(
+            f'''
+            Likely do not have enough /dev/shm space.
+            Current /dev/shm space is {shm_gibibytes} GiB,
+            but we requested {threshold_gibibytes} GiB.
+            Changing the size of /dev/shm of a host machine requires system
+            level configuration. For docker images you can call docker run
+            with --shm-size={thresh_mb}m.
+            '''))
 
     if 0:
         disk_parts = psutil.disk_partitions(all=True)
         # Note sure if there is a way to find candidates that could be
         # /dev/shm or if it is ever the case that it doesnt exist.
         import pandas as pd
         rows = []
```

### Comparing `geowatch-0.6.3/watch/utils/util_rgdc.py` & `geowatch-0.6.6/watch/utils/util_rgdc.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_s3.py` & `geowatch-0.6.6/watch/utils/util_s3.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_stringalgo.py` & `geowatch-0.6.6/watch/utils/util_stringalgo.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_time.py` & `geowatch-0.6.6/watch/utils/util_time.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_torchmetrics.py` & `geowatch-0.6.6/watch/utils/util_torchmetrics.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_windows.py` & `geowatch-0.6.6/watch/utils/util_windows.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.3/watch/utils/util_yaml.py` & `geowatch-0.6.6/watch/utils/util_yaml.py`

 * *Files identical despite different names*

