# Comparing `tmp/ml-starter-0.0.33.tar.gz` & `tmp/ml-starter-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.33.tar", last modified: Tue May  9 22:50:21 2023, max compression
+gzip compressed data, was "ml-starter-0.0.34.tar", last modified: Wed May 10 03:54:09 2023, max compression
```

## Comparing `ml-starter-0.0.33.tar` & `ml-starter-0.0.34.tar`

### file list

```diff
@@ -1,158 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.059192 ml-starter-0.0.33/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 22:50:09.000000 ml-starter-0.0.33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-09 22:50:09.000000 ml-starter-0.0.33/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 22:50:21.059192 ml-starter-0.0.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-09 22:50:09.000000 ml-starter-0.0.33/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.043192 ml-starter-0.0.33/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.043192 ml-starter-0.0.33/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.043192 ml-starter-0.0.33/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/launchers/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.043192 ml-starter-0.0.33/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12434 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.043192 ml-starter-0.0.33/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.043192 ml-starter-0.0.33/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.047191 ml-starter-0.0.33/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.047191 ml-starter-0.0.33/ml/models/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/models/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41250 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/models/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    60677 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/models/pretrained/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.047191 ml-starter-0.0.33/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.047191 ml-starter-0.0.33/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.047191 ml-starter-0.0.33/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.051192 ml-starter-0.0.33/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.051192 ml-starter-0.0.33/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.051192 ml-starter-0.0.33/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.051192 ml-starter-0.0.33/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.051192 ml-starter-0.0.33/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.051192 ml-starter-0.0.33/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.051192 ml-starter-0.0.33/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.055192 ml-starter-0.0.33/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.055192 ml-starter-0.0.33/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-09 22:50:09.000000 ml-starter-0.0.33/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:50:21.055192 ml-starter-0.0.33/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 22:50:21.000000 ml-starter-0.0.33/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-09 22:50:21.000000 ml-starter-0.0.33/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:50:21.000000 ml-starter-0.0.33/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-09 22:50:21.000000 ml-starter-0.0.33/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-09 22:50:21.000000 ml-starter-0.0.33/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-09 22:50:09.000000 ml-starter-0.0.33/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 22:50:09.000000 ml-starter-0.0.33/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-09 22:50:09.000000 ml-starter-0.0.33/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 22:50:09.000000 ml-starter-0.0.33/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 22:50:21.059192 ml-starter-0.0.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-09 22:50:09.000000 ml-starter-0.0.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.717642 ml-starter-0.0.34/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 03:53:54.000000 ml-starter-0.0.34/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 03:53:54.000000 ml-starter-0.0.34/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-10 03:54:09.717642 ml-starter-0.0.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-10 03:53:54.000000 ml-starter-0.0.34/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.689642 ml-starter-0.0.34/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.693642 ml-starter-0.0.34/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.693642 ml-starter-0.0.34/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/launchers/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.693642 ml-starter-0.0.34/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12434 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.697642 ml-starter-0.0.34/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.697642 ml-starter-0.0.34/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.697642 ml-starter-0.0.34/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23565 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.697642 ml-starter-0.0.34/ml/models/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/models/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41234 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/models/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31736 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/models/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60669 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/models/pretrained/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.701642 ml-starter-0.0.34/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.701642 ml-starter-0.0.34/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.701642 ml-starter-0.0.34/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.705642 ml-starter-0.0.34/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.705642 ml-starter-0.0.34/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.705642 ml-starter-0.0.34/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.705642 ml-starter-0.0.34/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.705642 ml-starter-0.0.34/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.709642 ml-starter-0.0.34/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.709642 ml-starter-0.0.34/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.713642 ml-starter-0.0.34/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.717642 ml-starter-0.0.34/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-10 03:53:54.000000 ml-starter-0.0.34/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:09.717642 ml-starter-0.0.34/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-10 03:54:09.000000 ml-starter-0.0.34/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-10 03:54:09.000000 ml-starter-0.0.34/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:54:09.000000 ml-starter-0.0.34/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-10 03:54:09.000000 ml-starter-0.0.34/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-10 03:54:09.000000 ml-starter-0.0.34/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-10 03:53:54.000000 ml-starter-0.0.34/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-10 03:53:54.000000 ml-starter-0.0.34/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 03:53:54.000000 ml-starter-0.0.34/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 03:53:54.000000 ml-starter-0.0.34/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 03:54:09.721642 ml-starter-0.0.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-10 03:53:54.000000 ml-starter-0.0.34/setup.py
```

### Comparing `ml-starter-0.0.33/LICENSE` & `ml-starter-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/PKG-INFO` & `ml-starter-0.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.33
+Version: 0.0.34
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.33/README.md` & `ml-starter-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/api.py` & `ml-starter-0.0.34/ml/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,18 +85,19 @@
     "InitializationType",
     "instantiate_config",
     "is_debugging",
     "is_distributed",
     "is_master",
     "LearnedPositionalEmbeddings",
     "load_model_and_task",
-    "LoRAConv1D",
-    "LoRAConv2D",
-    "LoRAEmbedding",
-    "LoRALinear",
+    "lora",
+    "LoraConv1d",
+    "LoraConv2d",
+    "LoraEmbedding",
+    "LoraLinear",
     "Loss",
     "meta_to_empty_func",
     "MultiIterDataset",
     "NormType",
     "open_atomic",
     "Output",
     "pad_all",
@@ -178,23 +179,16 @@
     LearnedPositionalEmbeddings,
     RotaryEmbeddings,
     SinusoidalEmbeddings,
     cast_embedding_kind,
     get_positional_embeddings,
 )
 from ml.models.init import InitializationType, cast_init_type, init_
-from ml.models.lora import LoRAConv1D, LoRAConv2D, LoRAEmbedding, LoRALinear
-from ml.models.norms import (
-    NormType,
-    cast_norm_type,
-    get_norm_1d,
-    get_norm_2d,
-    get_norm_3d,
-    get_norm_linear,
-)
+from ml.models.lora import LoraConv1d, LoraConv2d, LoraEmbedding, LoraLinear, lora
+from ml.models.norms import NormType, cast_norm_type, get_norm_1d, get_norm_2d, get_norm_3d, get_norm_linear
 from ml.models.pretrained.clip import pretrained_clip
 from ml.models.pretrained.sam import pretrained_sam
 from ml.optimizers.base import BaseOptimizer, BaseOptimizerConfig
 from ml.tasks.base import BaseTask, BaseTaskConfig
 from ml.tasks.datasets import transforms
 from ml.tasks.datasets.async_iterable import AsyncIterableDataset
 from ml.tasks.datasets.clippify import ClippifyDataset
```

### Comparing `ml-starter-0.0.33/ml/core/common_types.py` & `ml-starter-0.0.34/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/core/config.py` & `ml-starter-0.0.34/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/core/env.py` & `ml-starter-0.0.34/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/core/registry.py` & `ml-starter-0.0.34/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/core/state.py` & `ml-starter-0.0.34/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/launchers/base.py` & `ml-starter-0.0.34/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/launchers/ddp.py` & `ml-starter-0.0.34/ml/launchers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/launchers/slurm.py` & `ml-starter-0.0.34/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/launchers/torchrun.py` & `ml-starter-0.0.34/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/loggers/base.py` & `ml-starter-0.0.34/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/loggers/meter.py` & `ml-starter-0.0.34/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/loggers/multi.py` & `ml-starter-0.0.34/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/loggers/stdout.py` & `ml-starter-0.0.34/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/loggers/tensorboard.py` & `ml-starter-0.0.34/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/lr_schedulers/base.py` & `ml-starter-0.0.34/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.34/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.34/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/lr_schedulers/linear.py` & `ml-starter-0.0.34/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.34/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.34/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/models/activations.py` & `ml-starter-0.0.34/ml/models/activations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,48 @@
+"""Defines a general-purpose API for activation functions.
+
+.. highlight:: python
+.. code-block:: python
+
+    from ml.models.activations import get_activation, cast_activation_type
+
+    model = nn.Sequential(nn.Linear(4, 5), get_activation("relu"))
+
+    # This lets you parametrize the activation function as a string.
+    model = nn.Sequential(nn.Linear(4, 5), get_activation(cast_activation_type(my_activation)))
+
+Choices for the activation functions are:
+
+- ``"no_act"``
+- ``"relu"``
+- ``"relu6"``
+- ``"relu2"``
+- ``"clamp6"``
+- ``"leaky_relu"``
+- ``"elu"``
+- ``"celu"``
+- ``"selu"``
+- ``"gelu"``
+- ``"gelu_fast"``
+- ``"sigmoid"``
+- ``"log_sigmoid"``
+- ``"hard_sigomid"``
+- ``"tanh"``
+- ``"softsign"``
+- ``"softplus"``
+- ``"silu"``
+- ``"mish"``
+- ``"swish"``
+- ``"hard_swish"``
+- ``"soft_shrink"``
+- ``"hard_shrink"``
+- ``"tanh_shrink"``
+- ``"soft_sign"``
+"""
+
 import math
 from typing import Literal, cast, get_args
 
 import torch
 from torch import Tensor, nn
 
 ActivationType = Literal[
```

### Comparing `ml-starter-0.0.33/ml/models/base.py` & `ml-starter-0.0.34/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/models/embeddings.py` & `ml-starter-0.0.34/ml/models/embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,45 @@
+"""Defines a general-purpose API for transformer embedding layers.
+
+.. highlight:: python
+.. code-block:: python
+
+    from ml.models.embeddings import get_positional_embeddings, cast_embedding_kind
+
+    embeddings = get_positional_embeddings(
+        max_tsz=1024,
+        embed_dim=128,
+        kind="sinusoidal",
+        learnable=False,
+    )
+
+    x = torch.arange(3, 5, 8)
+
+    # Time-based positional embeddings - the time tensor supplies the
+    # times for each element in the input.
+    times = torch.randint(0, 1024, (3, 5))
+    y1 = embeddings(x, times=times)
+
+    # Offset-based positional embeddings - the input is assumed to be in
+    # temporal order, and the offset is the offset of the first element.
+    y2 = embeddings(x, offset=1)
+
+    assert y1.shape == y2.shape == x.shape
+
+    # This lets you parametrize the embedding kind as a string.
+    embeddings = get_positional_embeddings(..., kind=cast_embedding_kind(my_kind))
+
+Choices for the embedding kind are:
+
+- ``"identity"``: No positional embeddings are added.
+- ``"learned"``: Positional embeddings are learned.
+- ``"sinusoidal"``: Sinusoidal embeddings.
+- ``"rotary"``: Rotary embeddings (popular for training transformers).
+"""
+
 from typing import Literal, cast, get_args, overload
 
 import torch
 from torch import Tensor, nn
 
 from ml.models.init import InitializationType, init_
```

### Comparing `ml-starter-0.0.33/ml/models/norms.py` & `ml-starter-0.0.34/ml/models/norms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 """Defines general-purpose helper functions for initializing norm layers.
 
-Some pointers:
+.. highlight:: python
+.. code-block:: python
 
-- For networks which need to run efficiently at inference time, batch norm
-  is usually a good idea, since it can be fused with the weights of the
-  convolutional neural network. Similarly, weight norm also achieves this
-  (see `nn.utils.weight_norm`).
-
-This documentation should be updated with a better explanation of different
-types of normalization functions. My usual approach is to just throw everything
-at the wall and see what sticks.
-"""
+    from ml.models.norms import get_norm_linear, get_norm_1d, get_norm_2d, get_norm_3d, cast_norm_type
+
+    linear = nn.Sequential(nn.Linear(32, 32), get_norm_linear("layer", dim=32))
+    conv_1d = nn.Sequential(nn.Conv1d(32, 32, 3), get_norm_1d("layer", dim=32, groups=4))
+    conv_2d = nn.Sequential(nn.Conv2d(32, 32, 3), get_norm_2d("layer", dim=32, groups=4))
+    conv_3d = nn.Sequential(nn.Conv3d(32, 32, 3), get_norm_3d("layer", dim=32, groups=4))
+
+    # This lets you parametrize the norm type as a string.
+    linear = nn.Sequential(nn.Linear(32, 32), get_norm_linear(cast_norm_type(my_norm), dim=32))
 
+Choices for the norm type are:
+
+- ``"no_norm"``: No normalization
+- ``"batch"`` or ``"batch_affine"``: Batch normalization
+- ``"instance"`` or ``"instance_affine"``: Instance normalization
+- ``"group"`` or ``"group_affine"``: Group normalization
+- ``"layer"`` or ``"layer_affine"``: Layer normalization
+
+Note that instance norm and group norm are not available for linear layers.
+"""
 
 from typing import Literal, cast, get_args
 
 import torch
 from torch import Tensor, nn
 
 NormType = Literal[
```

### Comparing `ml-starter-0.0.33/ml/models/pretrained/clip.py` & `ml-starter-0.0.34/ml/models/pretrained/clip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # pylint: disable=too-many-lines
 """Defines a simple API for using OpenAI's pretrained CLIP model.
 
-Usage:
-
 .. highlight:: python
 .. code-block:: python
 
     from ml.models.pretrained.clip import pretrained_clip
 
     full_model = pretrained_clip("RN50", mode="all")
     visual_model = pretrained_clip("RN50", mode="visual")
@@ -168,15 +166,15 @@
         prev_char = char
     return pairs
 
 
 @functools.lru_cache()
 def test_clean_func(lower: bool = True) -> Callable[[str], str]:
     try:
-        import ftfy  # type: ignore[import]
+        import ftfy  # type: ignore
 
     except ImportError:
         logger.warning("Please install ftfy: pip install ftfy")
         ftfy = None
 
     def _clean(text: str) -> str:
         if ftfy is not None:
```

### Comparing `ml-starter-0.0.33/ml/models/pretrained/sam.py` & `ml-starter-0.0.34/ml/models/pretrained/sam.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # pylint: disable=too-many-lines
 """Defines a simple API for using Meta's pretrained Segment Anything model.
 
-Usage:
-
 .. highlight:: python
 .. code-block:: python
 
     from ml.models.pretrained.sam import pretrained_sam
 
     model = pretrained_sam("ViT-B")
     predictor = model.predictor()
```

### Comparing `ml-starter-0.0.33/ml/optimizers/adam.py` & `ml-starter-0.0.34/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/optimizers/adamw.py` & `ml-starter-0.0.34/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/optimizers/adan.py` & `ml-starter-0.0.34/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/optimizers/base.py` & `ml-starter-0.0.34/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/optimizers/sgd.py` & `ml-starter-0.0.34/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/optimizers/shampoo.py` & `ml-starter-0.0.34/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/scripts/cli.py` & `ml-starter-0.0.34/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/scripts/stage.py` & `ml-starter-0.0.34/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/scripts/train.py` & `ml-starter-0.0.34/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/base.py` & `ml-starter-0.0.34/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.34/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.34/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/datasets/collate.py` & `ml-starter-0.0.34/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.34/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.34/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.34/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.34/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.34/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/datasets/utils.py` & `ml-starter-0.0.34/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.34/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/environments/base.py` & `ml-starter-0.0.34/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/environments/utils.py` & `ml-starter-0.0.34/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/environments/worker.py` & `ml-starter-0.0.34/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/losses/reduce.py` & `ml-starter-0.0.34/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/rl/base.py` & `ml-starter-0.0.34/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/rl/replay.py` & `ml-starter-0.0.34/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/tasks/sl/base.py` & `ml-starter-0.0.34/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/trainers/base.py` & `ml-starter-0.0.34/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.34/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.34/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.34/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.34/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.34/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.34/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.34/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.34/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/trainers/rl.py` & `ml-starter-0.0.34/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/trainers/sl.py` & `ml-starter-0.0.34/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/trainers/vanilla.py` & `ml-starter-0.0.34/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/argparse.py` & `ml-starter-0.0.34/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/atomic.py` & `ml-starter-0.0.34/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/augmentation.py` & `ml-starter-0.0.34/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/caching.py` & `ml-starter-0.0.34/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/call_train.py` & `ml-starter-0.0.34/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/cli.py` & `ml-starter-0.0.34/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/colors.py` & `ml-starter-0.0.34/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/data.py` & `ml-starter-0.0.34/ml/utils/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,11 +156,11 @@
     Returns:
         True if the SHA256 matches, False otherwise.
     """
 
     sha256 = hashlib.sha256()
 
     with open(file_path, "rb") as f:
-        for chunk in tqdm.tqdm(iter(lambda: f.read(chunk_size), b""), disabled=not use_tqdm, delay=1.0):
+        for chunk in tqdm.tqdm(iter(lambda: f.read(chunk_size), b""), disable=not use_tqdm, delay=1.0):
             sha256.update(chunk)
 
     return sha256.hexdigest() == hash_str
```

### Comparing `ml-starter-0.0.33/ml/utils/datetime.py` & `ml-starter-0.0.34/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/device/auto.py` & `ml-starter-0.0.34/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/device/base.py` & `ml-starter-0.0.34/ml/utils/device/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,17 @@
         return Prefetcher(functools.partial(cls.sample_to_device), dataloader)
 
     @classmethod
     def module_to(cls, module: nn.Module) -> None:
         module.to(cls.get_device(), cls.get_floating_point_type())
 
     @classmethod
-    def tensor_to(cls, tensor: Tensor) -> Tensor:
+    def tensor_to(cls, tensor: np.ndarray | Tensor) -> Tensor:
+        if isinstance(tensor, np.ndarray):
+            tensor = torch.from_numpy(tensor)
         device = cls.get_device()
         if tensor.is_floating_point():
             return tensor.to(device, cls.get_floating_point_type())
         return tensor.to(device)
 
     @classmethod
     def recursive_apply(cls, item: Any) -> Any:
```

### Comparing `ml-starter-0.0.33/ml/utils/device/cpu.py` & `ml-starter-0.0.34/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/device/gpu.py` & `ml-starter-0.0.34/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/device/metal.py` & `ml-starter-0.0.34/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/distributed.py` & `ml-starter-0.0.34/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/image.py` & `ml-starter-0.0.34/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/io.py` & `ml-starter-0.0.34/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/large_models.py` & `ml-starter-0.0.34/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/logging.py` & `ml-starter-0.0.34/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/meter.py` & `ml-starter-0.0.34/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/staging.py` & `ml-starter-0.0.34/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/timer.py` & `ml-starter-0.0.34/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/torch_distributed.py` & `ml-starter-0.0.34/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml/utils/video.py` & `ml-starter-0.0.34/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.34/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.33
+Version: 0.0.34
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.33/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.34/ml_starter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 ml/models/base.py
 ml/models/embeddings.py
 ml/models/init.py
 ml/models/lora.py
 ml/models/norms.py
 ml/models/pretrained/__init__.py
 ml/models/pretrained/clip.py
+ml/models/pretrained/hubert.py
 ml/models/pretrained/sam.py
 ml/optimizers/__init__.py
 ml/optimizers/adam.py
 ml/optimizers/adamw.py
 ml/optimizers/adan.py
 ml/optimizers/base.py
 ml/optimizers/sgd.py
```

### Comparing `ml-starter-0.0.33/pyproject.toml` & `ml-starter-0.0.34/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.33/setup.py` & `ml-starter-0.0.34/setup.py`

 * *Files identical despite different names*

