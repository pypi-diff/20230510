# Comparing `tmp/ml-starter-0.0.31.tar.gz` & `tmp/ml-starter-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.31.tar", last modified: Mon May  8 13:15:03 2023, max compression
+gzip compressed data, was "ml-starter-0.0.32.tar", last modified: Tue May  9 02:52:06 2023, max compression
```

## Comparing `ml-starter-0.0.31.tar` & `ml-starter-0.0.32.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.231423 ml-starter-0.0.31/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 13:14:46.000000 ml-starter-0.0.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 13:14:46.000000 ml-starter-0.0.31/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-08 13:15:03.231423 ml-starter-0.0.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-08 13:14:46.000000 ml-starter-0.0.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.203423 ml-starter-0.0.31/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.207423 ml-starter-0.0.31/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.207423 ml-starter-0.0.31/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/launchers/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.207423 ml-starter-0.0.31/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12434 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.211423 ml-starter-0.0.31/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.211423 ml-starter-0.0.31/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.211423 ml-starter-0.0.31/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.211423 ml-starter-0.0.31/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.215423 ml-starter-0.0.31/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.215423 ml-starter-0.0.31/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.219423 ml-starter-0.0.31/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.219423 ml-starter-0.0.31/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.219423 ml-starter-0.0.31/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.219423 ml-starter-0.0.31/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.219423 ml-starter-0.0.31/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.219423 ml-starter-0.0.31/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.223423 ml-starter-0.0.31/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.227423 ml-starter-0.0.31/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.231423 ml-starter-0.0.31/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.231423 ml-starter-0.0.31/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-08 13:15:03.000000 ml-starter-0.0.31/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-08 13:15:03.000000 ml-starter-0.0.31/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:15:03.000000 ml-starter-0.0.31/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-08 13:15:03.000000 ml-starter-0.0.31/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-08 13:15:03.000000 ml-starter-0.0.31/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-08 13:14:46.000000 ml-starter-0.0.31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 13:14:46.000000 ml-starter-0.0.31/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-08 13:14:46.000000 ml-starter-0.0.31/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-08 13:14:46.000000 ml-starter-0.0.31/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-08 13:15:03.231423 ml-starter-0.0.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-08 13:14:46.000000 ml-starter-0.0.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.568925 ml-starter-0.0.32/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 02:51:52.000000 ml-starter-0.0.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-09 02:51:52.000000 ml-starter-0.0.32/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 02:52:06.568925 ml-starter-0.0.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-09 02:51:52.000000 ml-starter-0.0.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.540925 ml-starter-0.0.32/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.540925 ml-starter-0.0.32/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.540925 ml-starter-0.0.32/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/launchers/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.544925 ml-starter-0.0.32/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12434 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.544925 ml-starter-0.0.32/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.544925 ml-starter-0.0.32/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.544925 ml-starter-0.0.32/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.548925 ml-starter-0.0.32/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.548925 ml-starter-0.0.32/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.548925 ml-starter-0.0.32/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.552925 ml-starter-0.0.32/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.552925 ml-starter-0.0.32/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.552925 ml-starter-0.0.32/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.552925 ml-starter-0.0.32/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.556925 ml-starter-0.0.32/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.556925 ml-starter-0.0.32/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.560926 ml-starter-0.0.32/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.564926 ml-starter-0.0.32/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.564926 ml-starter-0.0.32/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-09 02:51:52.000000 ml-starter-0.0.32/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:52:06.568925 ml-starter-0.0.32/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 02:52:06.000000 ml-starter-0.0.32/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-09 02:52:06.000000 ml-starter-0.0.32/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 02:52:06.000000 ml-starter-0.0.32/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-09 02:52:06.000000 ml-starter-0.0.32/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-09 02:52:06.000000 ml-starter-0.0.32/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-09 02:51:52.000000 ml-starter-0.0.32/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 02:51:52.000000 ml-starter-0.0.32/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-09 02:51:52.000000 ml-starter-0.0.32/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 02:51:52.000000 ml-starter-0.0.32/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 02:52:06.568925 ml-starter-0.0.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-09 02:51:52.000000 ml-starter-0.0.32/setup.py
```

### Comparing `ml-starter-0.0.31/LICENSE` & `ml-starter-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/PKG-INFO` & `ml-starter-0.0.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.31
+Version: 0.0.32
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.31/README.md` & `ml-starter-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/api.py` & `ml-starter-0.0.32/ml/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     "Batch",
     "cached_object",
     "cast_activation_type",
     "cast_embedding_kind",
     "cast_init_type",
     "cast_norm_type",
     "cast_reduce_type",
+    "check_md5",
+    "check_sha256",
     "ChunkSampler",
     "Clamp",
     "ClippifyDataset",
     "collate_non_null",
     "collate",
     "CollateMode",
     "colorize",
@@ -216,15 +218,15 @@
 from ml.trainers.vanilla import VanillaTrainer, VanillaTrainerConfig
 from ml.utils.argparse import from_args, get_args, get_type_from_string
 from ml.utils.atomic import atomic_save, open_atomic
 from ml.utils.augmentation import get_image_mask
 from ml.utils.caching import DictIndex, cached_object
 from ml.utils.checks import assert_no_nans
 from ml.utils.colors import colorize
-from ml.utils.data import get_dataset_split_for_phase, get_dataset_splits, get_worker_info
+from ml.utils.data import check_md5, check_sha256, get_dataset_split_for_phase, get_dataset_splits, get_worker_info
 from ml.utils.datetime import format_timedelta
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.distributed import (
     get_master_addr,
     get_master_port,
     get_random_port,
```

### Comparing `ml-starter-0.0.31/ml/core/config.py` & `ml-starter-0.0.32/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/core/env.py` & `ml-starter-0.0.32/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/core/registry.py` & `ml-starter-0.0.32/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/core/state.py` & `ml-starter-0.0.32/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/launchers/base.py` & `ml-starter-0.0.32/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/launchers/ddp.py` & `ml-starter-0.0.32/ml/launchers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/launchers/slurm.py` & `ml-starter-0.0.32/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/launchers/torchrun.py` & `ml-starter-0.0.32/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/loggers/base.py` & `ml-starter-0.0.32/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/loggers/meter.py` & `ml-starter-0.0.32/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/loggers/multi.py` & `ml-starter-0.0.32/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/loggers/stdout.py` & `ml-starter-0.0.32/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/loggers/tensorboard.py` & `ml-starter-0.0.32/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/lr_schedulers/base.py` & `ml-starter-0.0.32/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.32/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.32/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/lr_schedulers/linear.py` & `ml-starter-0.0.32/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.32/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.32/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/models/activations.py` & `ml-starter-0.0.32/ml/models/activations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,34 @@
+import math
 from typing import Literal, cast, get_args
 
+import torch
 from torch import Tensor, nn
 
 ActivationType = Literal[
     "no_act",
     "relu",
     "relu6",
+    "relu2",
     "clamp6",
     "leaky_relu",
     "elu",
     "celu",
     "selu",
+    "gelu",
+    "gelu_fast",
     "sigmoid",
     "log_sigmoid",
     "hard_sigomid",
     "tanh",
     "softsign",
     "softplus",
     "silu",
     "mish",
+    "swish",
     "hard_swish",
     "soft_shrink",
     "hard_shrink",
     "tanh_shrink",
     "soft_sign",
 ]
 
@@ -62,14 +68,37 @@
 
 
 class Clamp6(Clamp):
     def __init__(self, inplace: bool = False) -> None:
         super().__init__(value=6.0, inplace=inplace)
 
 
+class ReLUSquared(nn.Module):
+    def forward(self, x: Tensor) -> Tensor:
+        relu_applied = nn.functional.relu(x)
+        squared = torch.square(relu_applied)
+        return squared
+
+
+class FastGELU(nn.Module):
+    def forward(self, x: Tensor) -> Tensor:
+        return 0.5 * x * (1.0 + torch.tanh(x * 0.7978845608 * (1.0 + 0.044715 * x * x)))
+
+
+class QuickGELU(nn.Module):
+    def forward(self, x: Tensor) -> Tensor:
+        return x * torch.sigmoid(1.702 * x)
+
+
+class LaplaceActivation(nn.Module):
+    def forward(self, x: Tensor, mu: float = 0.707107, sigma: float = 0.282095) -> Tensor:
+        x = (x - mu).div(sigma * math.sqrt(2.0))
+        return 0.5 * (1.0 + torch.erf(x))
+
+
 def get_activation(act: ActivationType, *, inplace: bool = True) -> nn.Module:
     """Returns an activation function from a keyword string.
 
     Args:
         act: The keyword for the activation function (None for identity)
         inplace: If set, use the inplace version of the activation function
 
@@ -81,39 +110,47 @@
     """
 
     match act:
         case "no_act":
             return nn.Identity()
         case "relu":
             return nn.ReLU(inplace=inplace)
+        case "relu2":
+            return nn.ReLU(inplace=inplace)
         case "relu6":
             return nn.ReLU6(inplace=inplace)
         case "clamp6":
             return Clamp6(inplace=inplace)
         case "leaky_relu":
             return nn.LeakyReLU(inplace=inplace)
         case "elu":
             return nn.ELU(inplace=inplace)
         case "celu":
             return nn.CELU(inplace=inplace)
         case "selu":
             return nn.SELU(inplace=inplace)
+        case "gelu":
+            return nn.GELU()
+        case "gelu_fast":
+            return FastGELU()
+        case "gelu_quick":
+            return QuickGELU()
         case "sigmoid":
             return nn.Sigmoid()
         case "log_sigmoid":
             return nn.LogSigmoid()
         case "hard_sigomid":
             return nn.Hardsigmoid(inplace=inplace)
         case "tanh":
             return nn.Tanh()
         case "softsign":
             return nn.Softsign()
         case "softplus":
             return nn.Softplus()
-        case "silu":
+        case "silu" | "swish":
             return nn.SiLU()
         case "mish":
             return nn.Mish(inplace=inplace)
         case "hard_swish":
             return nn.Hardswish(inplace=inplace)
         case "soft_shrink":
             return nn.Softshrink()
```

### Comparing `ml-starter-0.0.31/ml/models/base.py` & `ml-starter-0.0.32/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/models/embeddings.py` & `ml-starter-0.0.32/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/models/init.py` & `ml-starter-0.0.32/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/models/lora.py` & `ml-starter-0.0.32/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/models/norms.py` & `ml-starter-0.0.32/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/optimizers/adam.py` & `ml-starter-0.0.32/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/optimizers/adamw.py` & `ml-starter-0.0.32/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/optimizers/adan.py` & `ml-starter-0.0.32/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/optimizers/base.py` & `ml-starter-0.0.32/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/optimizers/sgd.py` & `ml-starter-0.0.32/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/optimizers/shampoo.py` & `ml-starter-0.0.32/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/scripts/cli.py` & `ml-starter-0.0.32/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/scripts/stage.py` & `ml-starter-0.0.32/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/scripts/train.py` & `ml-starter-0.0.32/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/base.py` & `ml-starter-0.0.32/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.32/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.32/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/datasets/collate.py` & `ml-starter-0.0.32/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.32/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.32/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.32/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.32/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.32/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/datasets/utils.py` & `ml-starter-0.0.32/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.32/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/environments/base.py` & `ml-starter-0.0.32/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/environments/utils.py` & `ml-starter-0.0.32/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/environments/worker.py` & `ml-starter-0.0.32/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/losses/reduce.py` & `ml-starter-0.0.32/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/rl/base.py` & `ml-starter-0.0.32/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/rl/replay.py` & `ml-starter-0.0.32/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/tasks/sl/base.py` & `ml-starter-0.0.32/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/trainers/base.py` & `ml-starter-0.0.32/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.32/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.32/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.32/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.32/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.32/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.32/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.32/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.32/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/trainers/rl.py` & `ml-starter-0.0.32/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/trainers/sl.py` & `ml-starter-0.0.32/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/trainers/vanilla.py` & `ml-starter-0.0.32/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/argparse.py` & `ml-starter-0.0.32/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/atomic.py` & `ml-starter-0.0.32/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/augmentation.py` & `ml-starter-0.0.32/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/caching.py` & `ml-starter-0.0.32/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/call_train.py` & `ml-starter-0.0.32/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/cli.py` & `ml-starter-0.0.32/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/colors.py` & `ml-starter-0.0.32/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/datetime.py` & `ml-starter-0.0.32/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/device/auto.py` & `ml-starter-0.0.32/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/device/base.py` & `ml-starter-0.0.32/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/device/cpu.py` & `ml-starter-0.0.32/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/device/gpu.py` & `ml-starter-0.0.32/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/device/metal.py` & `ml-starter-0.0.32/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/distributed.py` & `ml-starter-0.0.32/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/image.py` & `ml-starter-0.0.32/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/io.py` & `ml-starter-0.0.32/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/large_models.py` & `ml-starter-0.0.32/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/logging.py` & `ml-starter-0.0.32/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/meter.py` & `ml-starter-0.0.32/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/staging.py` & `ml-starter-0.0.32/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/timer.py` & `ml-starter-0.0.32/ml/utils/timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,27 +63,27 @@
     def close(self) -> None:
         self.stop()
         self._spinner_close = True
         self._thread.join()
 
     def _spinner(self) -> None:
         chars = [colorize(c, "light-yellow") for c in ("|", "/", "-", "\\")]
-        max_line_len = 0
         while not self._spinner_close:
             self._flag.wait()
             start_time = time.time()
             while not self._spinner_stop:
+                max_line_len = 0
                 for char in chars:
                     elapsed_secs = time.time() - start_time
                     line = f"[ {char} {elapsed_secs:.1f} ] {self._text}\r"
                     max_line_len = max(max_line_len, len(line))
                     sys.stderr.write(line)
                     sys.stderr.flush()
                     time.sleep(0.05)
-            sys.stderr.write(" " * max_line_len + "\r")
+                sys.stderr.write(" " * (max_line_len + 1) + "\r")
             self._flag.clear()
 
 
 @functools.lru_cache
 def spinner() -> Spinner:
     return Spinner()
```

### Comparing `ml-starter-0.0.31/ml/utils/torch_distributed.py` & `ml-starter-0.0.32/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml/utils/video.py` & `ml-starter-0.0.32/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.32/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.31
+Version: 0.0.32
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.31/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.32/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/pyproject.toml` & `ml-starter-0.0.32/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.31/setup.py` & `ml-starter-0.0.32/setup.py`

 * *Files identical despite different names*

