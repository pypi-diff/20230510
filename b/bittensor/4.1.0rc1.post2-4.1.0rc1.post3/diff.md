# Comparing `tmp/bittensor-4.1.0rc1.post2.tar.gz` & `tmp/bittensor-4.1.0rc1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-4.1.0rc1.post2.tar", last modified: Tue May  2 20:38:49 2023, max compression
+gzip compressed data, was "bittensor-4.1.0rc1.post3.tar", last modified: Wed May 10 19:12:58 2023, max compression
```

## Comparing `bittensor-4.1.0rc1.post2.tar` & `bittensor-4.1.0rc1.post3.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/
--rw-rw-r--   0 root         (0) root         (0)     1087 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4907 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3359 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.464254 bittensor-4.1.0rc1.post2/bin/
--rwxrwxr-x   0 root         (0) root         (0)     1297 2022-10-11 20:24:30.000000 bittensor-4.1.0rc1.post2/bin/btcli
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.464254 bittensor-4.1.0rc1.post2/bittensor/
--rw-rw-r--   0 root         (0) root         (0)    14544 2023-05-02 20:38:21.000000 bittensor-4.1.0rc1.post2/bittensor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.464254 bittensor-4.1.0rc1.post2/bittensor/_axon/
--rw-rw-r--   0 root         (0) root         (0)    17744 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_axon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.464254 bittensor-4.1.0rc1.post2/bittensor/_cli/
--rw-rw-r--   0 root         (0) root         (0)     6688 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3983 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/cli_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.464254 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/
--rw-rw-r--   0 root         (0) root         (0)      649 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    25104 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/delegates.py
--rw-rw-r--   0 root         (0) root         (0)     7571 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/inspect.py
--rw-rw-r--   0 root         (0) root         (0)     3911 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/list.py
--rw-rw-r--   0 root         (0) root         (0)     7193 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/metagraph.py
--rw-rw-r--   0 root         (0) root         (0)     7008 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/misc.py
--rw-rw-r--   0 root         (0) root         (0)    16429 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/overview.py
--rw-rw-r--   0 root         (0) root         (0)     7587 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/register.py
--rw-rw-r--   0 root         (0) root         (0)    11039 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/stake.py
--rw-rw-r--   0 root         (0) root         (0)     4349 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/transfer.py
--rw-rw-r--   0 root         (0) root         (0)    11156 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/unstake.py
--rw-rw-r--   0 root         (0) root         (0)     7733 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/utils.py
--rw-rw-r--   0 root         (0) root         (0)    17664 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/wallets.py
--rw-rw-r--   0 root         (0) root         (0)     4705 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_cli/commands/weights.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_config/
--rw-rw-r--   0 root         (0) root         (0)     6034 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5957 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_config/config_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_dataset/
--rw-rw-r--   0 root         (0) root         (0)    10966 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_dataset/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    27097 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_dataset/dataset_impl.py
--rw-rw-r--   0 root         (0) root         (0)     5467 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_dataset/dataset_mock.py
--rw-rw-r--   0 root         (0) root         (0)     3623 2022-10-11 20:17:46.000000 bittensor-4.1.0rc1.post2/bittensor/_dataset/thread_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_dendrite/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-02 20:35:22.000000 bittensor-4.1.0rc1.post2/bittensor/_dendrite/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10383 2023-05-02 18:29:38.000000 bittensor-4.1.0rc1.post2/bittensor/_dendrite/dendrite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_dendrite/text_prompting/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-02 20:35:24.000000 bittensor-4.1.0rc1.post2/bittensor/_dendrite/text_prompting/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7962 2023-05-02 18:29:38.000000 bittensor-4.1.0rc1.post2/bittensor/_dendrite/text_prompting/dendrite.py
--rw-rw-r--   0 root         (0) root         (0)     5195 2023-05-02 18:29:38.000000 bittensor-4.1.0rc1.post2/bittensor/_dendrite/text_prompting/dendrite_pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_ipfs/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/bittensor/_ipfs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2907 2023-02-21 20:04:30.000000 bittensor-4.1.0rc1.post2/bittensor/_ipfs/ipfs_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_keyfile/
--rw-rw-r--   0 root         (0) root         (0)     1894 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/bittensor/_keyfile/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    22266 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_keyfile/keyfile_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_logging/
--rw-rw-r--   0 root         (0) root         (0)    13107 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_metagraph/
--rw-rw-r--   0 root         (0) root         (0)    12460 2023-05-02 18:29:38.000000 bittensor-4.1.0rc1.post2/bittensor/_metagraph/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_prometheus/
--rw-rw-r--   0 root         (0) root         (0)     8118 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_prometheus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_proto/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/bittensor/_proto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    30214 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_proto/bittensor_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     4422 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_proto/bittensor_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_serializer/
--rw-rw-r--   0 root         (0) root         (0)     6078 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_serializer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10782 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_serializer/serializer_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_subtensor/
--rw-rw-r--   0 root         (0) root         (0)    14289 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    26232 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/chain_data.py
--rw-rw-r--   0 root         (0) root         (0)     2351 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/
--rw-rw-r--   0 root         (0) root         (0)     1126 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17164 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/delegation.py
--rw-rw-r--   0 root         (0) root         (0)    27011 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/log_utilities.py
--rw-rw-r--   0 root         (0) root         (0)     6056 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/prometheus.py
--rw-rw-r--   0 root         (0) root         (0)    14454 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/registration.py
--rw-rw-r--   0 root         (0) root         (0)    10152 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/serving.py
--rw-rw-r--   0 root         (0) root         (0)     6387 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/set_weights.py
--rw-rw-r--   0 root         (0) root         (0)    18492 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/staking.py
--rw-rw-r--   0 root         (0) root         (0)     7595 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/transfer.py
--rw-rw-r--   0 root         (0) root         (0)    15591 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/unstaking.py
--rw-rw-r--   0 root         (0) root         (0)    45559 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/subtensor_impl.py
--rw-rw-r--   0 root         (0) root         (0)    18974 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/_subtensor/subtensor_mock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_synapse/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-02 20:33:22.000000 bittensor-4.1.0rc1.post2/bittensor/_synapse/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6777 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_synapse/synapse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_synapse/text_prompting/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-02 20:34:23.000000 bittensor-4.1.0rc1.post2/bittensor/_synapse/text_prompting/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10714 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_synapse/text_prompting/miner.py
--rw-rw-r--   0 root         (0) root         (0)     5258 2023-05-02 18:29:38.000000 bittensor-4.1.0rc1.post2/bittensor/_synapse/text_prompting/synapse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_threadpool/
--rw-rw-r--   0 root         (0) root         (0)     4517 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_threadpool/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8631 2022-11-24 17:43:32.000000 bittensor-4.1.0rc1.post2/bittensor/_threadpool/priority_thread_pool_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_tokenizer/
--rw-rw-r--   0 root         (0) root         (0)     2500 2022-10-11 20:17:46.000000 bittensor-4.1.0rc1.post2/bittensor/_tokenizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/_wallet/
--rw-rw-r--   0 root         (0) root         (0)     7293 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/_wallet/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    41712 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/_wallet/wallet_impl.py
--rw-rw-r--   0 root         (0) root         (0)     2287 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/bittensor/_wallet/wallet_mock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/bittensor/utils/
--rw-rw-r--   0 root         (0) root         (0)     8575 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3443 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/utils/_register_cuda.py
--rw-rw-r--   0 root         (0) root         (0)     8711 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/utils/balance.py
--rw-rw-r--   0 root         (0) root         (0)     4457 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/utils/codes.py
--rw-rw-r--   0 root         (0) root         (0)      518 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/utils/formatting.py
--rw-rw-r--   0 root         (0) root         (0)     8017 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/utils/networking.py
--rw-rw-r--   0 root         (0) root         (0)    36116 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/utils/registration.py
--rw-rw-r--   0 root         (0) root         (0)    33174 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post2/bittensor/utils/registratrion_old.py
--rw-rw-r--   0 root         (0) root         (0)     3373 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/bittensor/utils/stats.py
--rw-rw-r--   0 root         (0) root         (0)      630 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post2/bittensor/utils/test_utils.py
--rw-rw-r--   0 root         (0) root         (0)    75481 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post2/bittensor/utils/tokenizer_utils.py
--rw-rw-r--   0 root         (0) root         (0)     9986 2023-05-02 18:29:32.000000 bittensor-4.1.0rc1.post2/bittensor/utils/weight_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:38:49.464254 bittensor-4.1.0rc1.post2/bittensor.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     4907 2023-05-02 20:38:49.000000 bittensor-4.1.0rc1.post2/bittensor.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3005 2023-05-02 20:38:49.000000 bittensor-4.1.0rc1.post2/bittensor.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-05-02 20:38:49.000000 bittensor-4.1.0rc1.post2/bittensor.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)     1027 2023-05-02 20:38:49.000000 bittensor-4.1.0rc1.post2/bittensor.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       10 2023-05-02 20:38:49.000000 bittensor-4.1.0rc1.post2/bittensor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 20:38:49.468254 bittensor-4.1.0rc1.post2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3436 2023-05-02 18:50:29.000000 bittensor-4.1.0rc1.post2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/
+-rw-rw-r--   0 root         (0) root         (0)     1087 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4917 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3369 2023-05-10 19:11:39.000000 bittensor-4.1.0rc1.post3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bin/
+-rwxrwxr-x   0 root         (0) root         (0)     1297 2022-10-11 20:24:30.000000 bittensor-4.1.0rc1.post3/bin/btcli
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/
+-rw-rw-r--   0 root         (0) root         (0)    15549 2023-05-10 19:12:46.000000 bittensor-4.1.0rc1.post3/bittensor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_axon/
+-rw-rw-r--   0 root         (0) root         (0)    17744 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_axon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_cli/
+-rw-rw-r--   0 root         (0) root         (0)     6688 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3983 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/cli_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/
+-rw-rw-r--   0 root         (0) root         (0)      649 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    25104 2023-05-04 15:20:44.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/delegates.py
+-rw-rw-r--   0 root         (0) root         (0)     7571 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/inspect.py
+-rw-rw-r--   0 root         (0) root         (0)     3911 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/list.py
+-rw-rw-r--   0 root         (0) root         (0)     7407 2023-05-10 19:11:39.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/metagraph.py
+-rw-rw-r--   0 root         (0) root         (0)     7008 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/misc.py
+-rw-rw-r--   0 root         (0) root         (0)    16429 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/overview.py
+-rw-rw-r--   0 root         (0) root         (0)     7587 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/register.py
+-rw-rw-r--   0 root         (0) root         (0)    11039 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/stake.py
+-rw-rw-r--   0 root         (0) root         (0)     4349 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/transfer.py
+-rw-rw-r--   0 root         (0) root         (0)    11156 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/unstake.py
+-rw-rw-r--   0 root         (0) root         (0)     7733 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    17664 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/wallets.py
+-rw-rw-r--   0 root         (0) root         (0)     4705 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_cli/commands/weights.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_config/
+-rw-rw-r--   0 root         (0) root         (0)     6034 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5957 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_config/config_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_dataset/
+-rw-rw-r--   0 root         (0) root         (0)    10966 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_dataset/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    27097 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_dataset/dataset_impl.py
+-rw-rw-r--   0 root         (0) root         (0)     5467 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_dataset/dataset_mock.py
+-rw-rw-r--   0 root         (0) root         (0)     3623 2022-10-11 20:17:46.000000 bittensor-4.1.0rc1.post3/bittensor/_dataset/thread_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_dendrite/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_dendrite/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10220 2023-05-10 19:11:39.000000 bittensor-4.1.0rc1.post3/bittensor/_dendrite/dendrite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_dendrite/text_prompting/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_dendrite/text_prompting/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10897 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_dendrite/text_prompting/dendrite.py
+-rw-rw-r--   0 root         (0) root         (0)     5195 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_dendrite/text_prompting/dendrite_pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_ipfs/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/bittensor/_ipfs/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2907 2023-02-21 20:04:30.000000 bittensor-4.1.0rc1.post3/bittensor/_ipfs/ipfs_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_keyfile/
+-rw-rw-r--   0 root         (0) root         (0)     1894 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/bittensor/_keyfile/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22266 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_keyfile/keyfile_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_logging/
+-rw-rw-r--   0 root         (0) root         (0)    13107 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_metagraph/
+-rw-rw-r--   0 root         (0) root         (0)    12489 2023-05-10 19:11:39.000000 bittensor-4.1.0rc1.post3/bittensor/_metagraph/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_prometheus/
+-rw-rw-r--   0 root         (0) root         (0)     8118 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_prometheus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_proto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/bittensor/_proto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    37015 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_proto/bittensor_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6201 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_proto/bittensor_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_serializer/
+-rw-rw-r--   0 root         (0) root         (0)     6078 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_serializer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10782 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_serializer/serializer_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor/_subtensor/
+-rw-rw-r--   0 root         (0) root         (0)    14289 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    26232 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/chain_data.py
+-rw-rw-r--   0 root         (0) root         (0)     2351 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/
+-rw-rw-r--   0 root         (0) root         (0)     1126 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    17164 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/delegation.py
+-rw-rw-r--   0 root         (0) root         (0)    27011 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/log_utilities.py
+-rw-rw-r--   0 root         (0) root         (0)     6056 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/prometheus.py
+-rw-rw-r--   0 root         (0) root         (0)    14454 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/registration.py
+-rw-rw-r--   0 root         (0) root         (0)    10152 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/serving.py
+-rw-rw-r--   0 root         (0) root         (0)     6387 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/set_weights.py
+-rw-rw-r--   0 root         (0) root         (0)    18492 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/staking.py
+-rw-rw-r--   0 root         (0) root         (0)     7595 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/transfer.py
+-rw-rw-r--   0 root         (0) root         (0)    15591 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/unstaking.py
+-rw-rw-r--   0 root         (0) root         (0)    45559 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/subtensor_impl.py
+-rw-rw-r--   0 root         (0) root         (0)    18974 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/_subtensor/subtensor_mock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/_synapse/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_synapse/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6777 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_synapse/synapse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/_synapse/text_prompting/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_synapse/text_prompting/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10714 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_synapse/text_prompting/miner.py
+-rw-rw-r--   0 root         (0) root         (0)     7346 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_synapse/text_prompting/synapse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/_threadpool/
+-rw-rw-r--   0 root         (0) root         (0)     4517 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_threadpool/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8631 2022-11-24 17:43:32.000000 bittensor-4.1.0rc1.post3/bittensor/_threadpool/priority_thread_pool_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/_tokenizer/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2022-10-11 20:17:46.000000 bittensor-4.1.0rc1.post3/bittensor/_tokenizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/_wallet/
+-rw-rw-r--   0 root         (0) root         (0)     7293 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/_wallet/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    41712 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/_wallet/wallet_impl.py
+-rw-rw-r--   0 root         (0) root         (0)     2287 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/bittensor/_wallet/wallet_mock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/bittensor/utils/
+-rw-rw-r--   0 root         (0) root         (0)     8575 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3443 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/utils/_register_cuda.py
+-rw-rw-r--   0 root         (0) root         (0)     8711 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/utils/balance.py
+-rw-rw-r--   0 root         (0) root         (0)     4457 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/utils/codes.py
+-rw-rw-r--   0 root         (0) root         (0)      518 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/utils/formatting.py
+-rw-rw-r--   0 root         (0) root         (0)     8017 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/utils/networking.py
+-rw-rw-r--   0 root         (0) root         (0)    36116 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/utils/registration.py
+-rw-rw-r--   0 root         (0) root         (0)    33174 2023-04-20 18:56:12.000000 bittensor-4.1.0rc1.post3/bittensor/utils/registratrion_old.py
+-rw-rw-r--   0 root         (0) root         (0)     3373 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/bittensor/utils/stats.py
+-rw-rw-r--   0 root         (0) root         (0)      630 2022-07-09 15:48:08.000000 bittensor-4.1.0rc1.post3/bittensor/utils/test_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    75481 2023-03-23 20:47:08.000000 bittensor-4.1.0rc1.post3/bittensor/utils/tokenizer_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     9986 2023-05-04 15:30:00.000000 bittensor-4.1.0rc1.post3/bittensor/utils/weight_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:12:58.569312 bittensor-4.1.0rc1.post3/bittensor.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     4917 2023-05-10 19:12:58.000000 bittensor-4.1.0rc1.post3/bittensor.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3005 2023-05-10 19:12:58.000000 bittensor-4.1.0rc1.post3/bittensor.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-10 19:12:58.000000 bittensor-4.1.0rc1.post3/bittensor.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)     1044 2023-05-10 19:12:58.000000 bittensor-4.1.0rc1.post3/bittensor.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       10 2023-05-10 19:12:58.000000 bittensor-4.1.0rc1.post3/bittensor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 19:12:58.573312 bittensor-4.1.0rc1.post3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3436 2023-05-02 18:50:29.000000 bittensor-4.1.0rc1.post3/setup.py
```

### Comparing `bittensor-4.1.0rc1.post2/LICENSE` & `bittensor-4.1.0rc1.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/PKG-INFO` & `bittensor-4.1.0rc1.post3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 4.1.0rc1.post2
+Version: 4.1.0rc1.post3
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
 Description: <div align="center">
         
@@ -31,15 +31,15 @@
         Bittensor is a mining network, similar to Bitcoin, that includes built-in incentives designed to encourage miners to provide value by hosting trained or training machine learning models. These models can be queried by clients seeking inference over inputs, such as token-based text generations or numerical embeddings from a large foundation model like GPT-NeoX-20B.
         
         Token-based incentives are designed to drive the network's growth and distribute the value generated by the network directly to the individuals producing that value, without intermediaries. The network is open to all participants, and no individual or group has full control over what is learned, who can profit from it, or who can access it.
         
         To learn more about Bittensor, please read our [paper](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU/view).
         
         # Install
-        Three ways to install Bittensor
+        There are three ways to install Bittensor
         
         1. Through the installer:
         ```
         $ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/opentensor/bittensor/master/scripts/install.sh)"
         ```
         
         2. With pip:
```

### Comparing `bittensor-4.1.0rc1.post2/README.md` & `bittensor-4.1.0rc1.post3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 Bittensor is a mining network, similar to Bitcoin, that includes built-in incentives designed to encourage miners to provide value by hosting trained or training machine learning models. These models can be queried by clients seeking inference over inputs, such as token-based text generations or numerical embeddings from a large foundation model like GPT-NeoX-20B.
 
 Token-based incentives are designed to drive the network's growth and distribute the value generated by the network directly to the individuals producing that value, without intermediaries. The network is open to all participants, and no individual or group has full control over what is learned, who can profit from it, or who can access it.
 
 To learn more about Bittensor, please read our [paper](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU/view).
 
 # Install
-Three ways to install Bittensor
+There are three ways to install Bittensor
 
 1. Through the installer:
 ```
 $ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/opentensor/bittensor/master/scripts/install.sh)"
 ```
 
 2. With pip:
```

### Comparing `bittensor-4.1.0rc1.post2/bin/btcli` & `bittensor-4.1.0rc1.post3/bin/btcli`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from langchain.llms.base import LLM
 from typing import Optional, List, Mapping, Any, Tuple
 
 import nest_asyncio
 nest_asyncio.apply()
 
 # Bittensor code and protocol version.
-__version__ = '4.1.0-rc1-2'
+__version__ = '4.1.0-rc1-3'
 version_split = __version__.split("-")[0].split(".")
 __version_as_int__ = (100 * int(version_split[0])) + (10 * int(version_split[1])) + (1 * int(version_split[2]))
 __new_signature_version__ = 360
 
 # Turn off rich console locals trace.
 from rich.traceback import install
 install(show_locals=False)
@@ -186,14 +186,16 @@
 from bittensor._ipfs.ipfs_impl import Ipfs as Ipfs
 
 # ---- Errors and Exceptions -----
 from bittensor._keyfile.keyfile_impl import KeyFileError as KeyFileError
 
 from bittensor._proto.bittensor_pb2 import ForwardTextPromptingRequest
 from bittensor._proto.bittensor_pb2 import ForwardTextPromptingResponse
+from bittensor._proto.bittensor_pb2 import MultiForwardTextPromptingRequest
+from bittensor._proto.bittensor_pb2 import MultiForwardTextPromptingResponse
 from bittensor._proto.bittensor_pb2 import BackwardTextPromptingRequest
 from bittensor._proto.bittensor_pb2 import BackwardTextPromptingResponse
 
 # ---- Synapses -----
 from bittensor._synapse.synapse import Synapse
 from bittensor._synapse.synapse import SynapseCall
 from bittensor._synapse.text_prompting.synapse import TextPromptingSynapse
@@ -244,43 +246,48 @@
 __context_prompting_llm = None
 def prompt( 
         content: Union[ str, List[str], List[Dict[ str ,str ]]],
         wallet_name: str = "default",
         hotkey: str = default_prompting_validator_key,
         subtensor_: Optional['Subtensor'] = None,
         axon_: Optional['axon_info'] = None,
+        return_all: bool = False,
     ) -> str:
     global __context_prompting_llm
     if __context_prompting_llm == None:
         __context_prompting_llm = prompting( 
             wallet_name = wallet_name,
             hotkey = hotkey,
             subtensor_ = subtensor_,
             axon_ = axon_,
         )
-    return __context_prompting_llm( content = content )
+    return __context_prompting_llm( content = content, return_all = return_all )
 
 class prompting ( torch.nn.Module ):
     _axon: 'axon_info'
     _dendrite: 'Dendrite'
     _subtensor: 'Subtensor'
     _hotkey: str
     _keypair: 'Keypair'
 
     def __init__(
         self,
         wallet_name: str = "default",
         hotkey: str = default_prompting_validator_key,
         subtensor_: Optional['Subtensor'] = None,
         axon_: Optional['axon_info'] = None,
+        use_coldkey: bool = False
     ):
         super(prompting, self).__init__()
         self._hotkey = hotkey
         self._subtensor = subtensor() if subtensor_ is None else subtensor_
-        self._keypair = wallet( name = wallet_name ).create_if_non_existent().coldkey
+        if use_coldkey:
+            self._keypair = wallet( name = wallet_name ).create_if_non_existent().coldkey
+        else:
+            self._keypair = wallet( name = wallet_name ).create_if_non_existent().hotkey
         
         if axon_ is not None:
             self._axon = axon_
         else:
             self._metagraph = metagraph( 1 )
             self._axon = self._metagraph.axons[ self._metagraph.hotkeys.index( self._hotkey ) ]
         self._dendrite = text_prompting(
@@ -301,35 +308,52 @@
                 raise ValueError('content has invalid type {}'.format( type( content )))
         else:
             raise ValueError('content has invalid type {}'.format( type( content )))
         
     def forward( 
             self,
             content: Union[ str, List[str], List[Dict[ str ,str ]]],
-            timeout: float = 1000,
-            return_call: bool = False
-        ) -> str:
+            timeout: float = 24,
+            return_call: bool = False,
+            return_all: bool = False,
+        ) -> Union[str, List[str]]:
         roles, messages = self.format_content( content )
-        return self._dendrite.forward(
-            roles = roles,
-            messages = messages,
-            timeout = timeout
-        ).completion
+        if not return_all:
+            return self._dendrite.forward(
+                roles = roles,
+                messages = messages,
+                timeout = timeout
+            ).completion
+        else:
+            return self._dendrite.multi_forward(
+                roles = roles,
+                messages = messages,
+                timeout = timeout
+            ).multi_completions
+
        
     async def async_forward( 
             self,
             content: Union[ str, List[str], List[Dict[ str ,str ]]],
-            timeout: float = 1000
-        ):
+            timeout: float = 24,
+            return_all: bool = False,
+        ) -> Union[str, List[str]]:
         roles, messages = self.format_content( content )
-        return await self._dendrite.async_forward(
-            roles = roles,
-            messages = messages,
-            timeout = timeout
-        ).completion
+        if not return_all:
+            return await self._dendrite.async_forward(
+                    roles = roles,
+                    messages = messages,
+                    timeout = timeout
+                ).completion
+        else:
+            return self._dendrite.async_multi_forward(
+                roles = roles,
+                messages = messages,
+                timeout = timeout
+            ).multi_completions
 
 class BittensorLLM(LLM):
     """Wrapper around Bittensor Prompting Subnetwork. 
 This Python file implements the BittensorLLM class, a wrapper around the Bittensor Prompting Subnetwork for easy integration into language models. The class provides a query method to receive responses from the subnetwork for a given user message and an implementation of the _call method to return the best response. The class can be initialized with various parameters such as the wallet name and chain endpoint.
     
     Example:
         .. code-block:: python
```

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_axon/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_axon/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/cli_impl.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/cli_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/delegates.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/delegates.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/inspect.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/list.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/metagraph.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/metagraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,21 @@
     @staticmethod
     def add_args( parser: argparse.ArgumentParser ):
         metagraph_parser = parser.add_parser(
             'metagraph', 
             help='''Metagraph commands'''
         )
         metagraph_parser.add_argument(
+            '--netuid', 
+            dest='netuid', 
+            type=int,
+            help='''Set the netuid to get the metagraph of''',
+            default=False,
+        )
+        metagraph_parser.add_argument(
             '--no_prompt', 
             dest='no_prompt', 
             action='store_true', 
             help='''Set true to avoid prompting the user.''',
             default=False,
         )
         metagraph_parser.add_argument( '--no_version_checking', action='store_true', help='''Set false to stop cli version checking''', default = False )
```

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/misc.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/misc.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/overview.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/overview.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/register.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/register.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/stake.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/stake.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/transfer.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/unstake.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/unstake.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/utils.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/wallets.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/wallets.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_cli/commands/weights.py` & `bittensor-4.1.0rc1.post3/bittensor/_cli/commands/weights.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_config/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_config/config_impl.py` & `bittensor-4.1.0rc1.post3/bittensor/_config/config_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_dataset/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_dataset/dataset_impl.py` & `bittensor-4.1.0rc1.post3/bittensor/_dataset/dataset_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_dataset/dataset_mock.py` & `bittensor-4.1.0rc1.post3/bittensor/_dataset/dataset_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_dataset/thread_queue.py` & `bittensor-4.1.0rc1.post3/bittensor/_dataset/thread_queue.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_dendrite/dendrite.py` & `bittensor-4.1.0rc1.post3/bittensor/_dendrite/dendrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,16 +140,14 @@
         ):
         """ Dendrite abstract class
             Args:
                 keypair (:obj:`Union[ 'bittensor.Wallet', 'bittensor.Keypair']`, `required`):
                     bittensor keypair used for signing messages.
                 axon (:obj:Union[`bittensor.axon_info`, 'bittensor.axon'], `required`):   
                     bittensor axon object or its info used to create the connection.
-                external_ip (:obj:`str`, `optional`, defaults to None):
-                    external ip of the machine, if None, will use the ip from the endpoint.
                 grpc_options (:obj:`List[Tuple[str,object]]`, `optional`):
                     grpc options to pass through to channel.
         """
         super(Dendrite, self).__init__()
         self.uuid = str(uuid.uuid1())
         self.uid = uid
         self.keypair = keypair.hotkey if isinstance( keypair, bittensor.Wallet ) else keypair
@@ -244,8 +242,8 @@
             return "Channel closed"
 
 
 
     
 
     
-    
+
```

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_dendrite/text_prompting/dendrite.py` & `bittensor-4.1.0rc1.post3/bittensor/_dendrite/text_prompting/dendrite.py`

 * *Files 18% similar despite different names*

```diff
@@ -72,14 +72,53 @@
         return await self.dendrite.async_backward(
             roles = self.roles,
             messages = self.messages,
             completion = self.completion,
             rewards = [ reward ],
             timeout = self.timeout if timeout is None else bittensor.__blocktime__
         )
+
+
+class MultiDendriteForwardCall( bittensor.DendriteCall ):
+
+    name: str = "text_prompting_multi_forward"
+    is_forward: bool = True
+    multi_completions: List[str] = [""] # To be filled.
+
+    def __init__(
+        self,
+        dendrite: 'bittensor.TextPromptingDendrite',
+        messages: List[str],
+        roles: List[str],
+        timeout: float = bittensor.__blocktime__,
+    ):
+        super().__init__( dendrite = dendrite, timeout = timeout )
+        self.messages = messages
+        self.roles = roles
+        self.packed_messages = [json.dumps({"role": role, "content": message}) for role, message in zip(self.roles, self.messages)]
+
+    def __repr__(self) -> str:
+        return f"MultiDendriteForwardCall( {bittensor.utils.codes.code_to_string(self.return_code)}, to: {self.dest_hotkey[:4]}...{self.dest_hotkey[-4:]}, msg: {self.return_message}, n_completion: {len(self.multi_completions)})"
+    
+    def __str__(self) -> str: return self.__repr__()
+    
+    def get_callable( self ) -> Callable:
+        return bittensor.grpc.TextPromptingStub( self.dendrite.channel ).MultiForward
+
+    def get_request_proto( self ) -> bittensor.proto.MultiForwardTextPromptingRequest:
+        return bittensor.MultiForwardTextPromptingRequest( timeout = self.timeout, messages = self.packed_messages )
+    
+    def apply_response_proto( self, response_proto: bittensor.MultiForwardTextPromptingResponse ):
+        self.multi_completions = response_proto.multi_completions
+        
+    def get_inputs_shape(self) -> torch.Size: 
+        return torch.Size( [len(message) for message in self.packed_messages] )
+
+    def get_outputs_shape(self) -> torch.Size:
+        return torch.Size([ len(self.multi_completions) ] )
     
     
 class DendriteBackwardCall( bittensor.DendriteCall ):
 
     name: str = "text_prompting_backward"
     is_forward: bool = False
     
@@ -155,14 +194,48 @@
             roles = roles,
             timeout = timeout,
         )
         forward_call = await self.apply( dendrite_call = forward_call )
         if return_call: return forward_call
         else: return forward_call.completion
 
+    def multi_forward(
+            self,
+            roles: List[ str ] ,
+            messages: List[ str ],
+            timeout: float = bittensor.__blocktime__,
+            return_call:bool = True,
+        ) -> Union[ str, DendriteForwardCall ]:
+        forward_call = MultiDendriteForwardCall(
+            dendrite = self, 
+            messages = messages,
+            roles = roles,
+            timeout = timeout,
+        )
+        response_call = self.loop.run_until_complete( self.apply( dendrite_call = forward_call ) )
+        if return_call: return response_call
+        else: return response_call.multi_completions
+    
+    async def async_multi_forward(
+        self,
+        roles: List[ str ],
+        messages: List[ str ],
+        timeout: float = bittensor.__blocktime__,
+        return_call: bool = True,
+    ) -> Union[ str, DendriteForwardCall ]:
+        forward_call = MultiDendriteForwardCall(
+            dendrite = self, 
+            messages = messages,
+            roles = roles,
+            timeout = timeout,
+        )
+        forward_call = await self.apply( dendrite_call = forward_call )
+        if return_call: return forward_call
+        else: return forward_call.multi_completions
+
     def backward(
             self,
             roles: List[ str ],
             messages: List[ str ],
             completion: str,
             rewards: Union[ List[ float], torch.FloatTensor ],
             timeout: float = bittensor.__blocktime__,
```

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_dendrite/text_prompting/dendrite_pool.py` & `bittensor-4.1.0rc1.post3/bittensor/_dendrite/text_prompting/dendrite_pool.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_ipfs/ipfs_impl.py` & `bittensor-4.1.0rc1.post3/bittensor/_ipfs/ipfs_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_keyfile/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_keyfile/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_keyfile/keyfile_impl.py` & `bittensor-4.1.0rc1.post3/bittensor/_keyfile/keyfile_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_logging/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_metagraph/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_metagraph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,17 +112,17 @@
         self.axons = []
         if sync:
             self.sync( block = None, lite = lite )
 
     def sync ( self, block: Optional[int] = None, lite: bool = True ) -> 'metagraph':
         subtensor = bittensor.subtensor( network = self.network )
         if lite:
-            self.neurons = subtensor.neurons_lite( netuid = self.netuid )
+            self.neurons = subtensor.neurons_lite( block = block, netuid = self.netuid )
         else:
-            self.neurons = subtensor.neurons( netuid = self.netuid )
+            self.neurons = subtensor.neurons(block = block, netuid = self.netuid )
         self.lite = lite
         self.n = torch.nn.Parameter( torch.tensor( len(self.neurons), dtype=torch.int64 ), requires_grad=False )
         self.version = torch.nn.Parameter( torch.tensor( [bittensor.__version_as_int__], dtype=torch.int64 ), requires_grad=False )
         self.block = torch.nn.Parameter( torch.tensor( subtensor.block, dtype=torch.int64 ), requires_grad=False )
         self.uids = torch.nn.Parameter( torch.tensor( [ neuron.uid for neuron in self.neurons ], dtype=torch.int64 ), requires_grad=False )
         self.trust = torch.nn.Parameter( torch.tensor( [ neuron.trust for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
         self.consensus = torch.nn.Parameter( torch.tensor( [ neuron.consensus for neuron in self.neurons ], dtype=torch.float32 ), requires_grad=False )
```

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_prometheus/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_proto/bittensor_pb2.py` & `bittensor-4.1.0rc1.post3/bittensor/_proto/bittensor_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='bittensor/_proto/bittensor.proto',
   package='',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n bittensor/_proto/bittensor.proto\"a\n\x1b\x46orwardTextPromptingRequest\x12\x0f\n\x07version\x18\x01 \x01(\x05\x12\x0e\n\x06hotkey\x18\x02 \x01(\t\x12\x10\n\x08messages\x18\x03 \x03(\t\x12\x0f\n\x07timeout\x18\x04 \x01(\x02\"\x8b\x01\n\x1c\x46orwardTextPromptingResponse\x12\x0f\n\x07version\x18\x01 \x01(\x05\x12\x0e\n\x06hotkey\x18\x02 \x01(\t\x12\x10\n\x08response\x18\x03 \x01(\t\x12\x16\n\x0ereturn_message\x18\x04 \x01(\t\x12 \n\x0breturn_code\x18\x05 \x01(\x0e\x32\x0b.ReturnCode\"\x85\x01\n\x1c\x42\x61\x63kwardTextPromptingRequest\x12\x0f\n\x07version\x18\x01 \x01(\x05\x12\x0e\n\x06hotkey\x18\x02 \x01(\t\x12\x0f\n\x07rewards\x18\x03 \x03(\x02\x12\x10\n\x08messages\x18\x04 \x03(\t\x12\x10\n\x08response\x18\x05 \x01(\t\x12\x0f\n\x07timeout\x18\x06 \x01(\x02\"z\n\x1d\x42\x61\x63kwardTextPromptingResponse\x12\x0f\n\x07version\x18\x01 \x01(\x05\x12\x0e\n\x06hotkey\x18\x02 \x01(\t\x12\x16\n\x0ereturn_message\x18\x04 \x01(\t\x12 \n\x0breturn_code\x18\x05 \x01(\x0e\x32\x0b.ReturnCode\"\xac\x01\n\x06Tensor\x12\x0f\n\x07version\x18\x01 \x01(\x05\x12\x0e\n\x06\x62uffer\x18\x02 \x01(\x0c\x12\r\n\x05shape\x18\x03 \x03(\x03\x12\x1f\n\nserializer\x18\x04 \x01(\x0e\x32\x0b.Serializer\x12 \n\x0btensor_type\x18\x05 \x01(\x0e\x32\x0b.TensorType\x12\x18\n\x05\x64type\x18\x06 \x01(\x0e\x32\t.DataType\x12\x15\n\rrequires_grad\x18\x08 \x01(\x08*\xda\x04\n\nReturnCode\x12\x0c\n\x08NoReturn\x10\x00\x12\x0b\n\x07Success\x10\x01\x12\x0b\n\x07Timeout\x10\x02\x12\x0b\n\x07\x42\x61\x63koff\x10\x03\x12\x0f\n\x0bUnavailable\x10\x04\x12\x12\n\x0eNotImplemented\x10\x05\x12\x10\n\x0c\x45mptyRequest\x10\x06\x12\x11\n\rEmptyResponse\x10\x07\x12\x13\n\x0fInvalidResponse\x10\x08\x12\x12\n\x0eInvalidRequest\x10\t\x12\x19\n\x15RequestShapeException\x10\n\x12\x1a\n\x16ResponseShapeException\x10\x0b\x12!\n\x1dRequestSerializationException\x10\x0c\x12\"\n\x1eResponseSerializationException\x10\r\x12#\n\x1fRequestDeserializationException\x10\x0e\x12$\n ResponseDeserializationException\x10\x0f\x12\x15\n\x11NotServingNucleus\x10\x10\x12\x12\n\x0eNucleusTimeout\x10\x11\x12\x0f\n\x0bNucleusFull\x10\x12\x12\x1e\n\x1aRequestIncompatibleVersion\x10\x13\x12\x1f\n\x1bResponseIncompatibleVersion\x10\x14\x12\x11\n\rSenderUnknown\x10\x15\x12\x14\n\x10UnknownException\x10\x16\x12\x13\n\x0fUnauthenticated\x10\x17\x12\x0f\n\x0b\x42\x61\x64\x45ndpoint\x10\x18\x12\x0f\n\x0b\x42lacklisted\x10\x19*&\n\nSerializer\x12\x0b\n\x07MSGPACK\x10\x00\x12\x0b\n\x07\x43MPPACK\x10\x01*2\n\nTensorType\x12\t\n\x05TORCH\x10\x00\x12\x0e\n\nTENSORFLOW\x10\x01\x12\t\n\x05NUMPY\x10\x02*h\n\x08\x44\x61taType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07\x46LOAT32\x10\x01\x12\x0b\n\x07\x46LOAT64\x10\x02\x12\t\n\x05INT32\x10\x03\x12\t\n\x05INT64\x10\x04\x12\x08\n\x04UTF8\x10\x05\x12\x0b\n\x07\x46LOAT16\x10\x06\x12\x08\n\x04\x42OOL\x10\x07\x32\xa6\x01\n\rTextPrompting\x12H\n\x07\x46orward\x12\x1c.ForwardTextPromptingRequest\x1a\x1d.ForwardTextPromptingResponse\"\x00\x12K\n\x08\x42\x61\x63kward\x12\x1d.BackwardTextPromptingRequest\x1a\x1e.BackwardTextPromptingResponse\"\x00\x62\x06proto3'
+  serialized_pb=b'\n bittensor/_proto/bittensor.proto\"a\n\x1b\x46orwardTextPromptingRequest\x12\x0f\n\x07version\x18\x01 \x01(\x05\x12\x0e\n\x06hotkey\x18\x02 \x01(\t\x12\x10\n\x08messages\x18\x03 \x03(\t\x12\x0f\n\x07timeout\x18\x04 \x01(\x02\"\x8b\x01\n\x1c\x46orwardTextPromptingResponse\x12\x0f\n\x07version\x18\x01 \x01(\x05\x12\x0e\n\x06hotkey\x18\x02 \x01(\t\x12\x10\n\x08response\x18\x03 \x01(\t\x12\x16\n\x0ereturn_message\x18\x04 \x01(\t\x12 \n\x0breturn_code\x18\x05 \x01(\x0e\x32\x0b.ReturnCode\"f\n MultiForwardTextPromptingRequest\x12\x0f\n\x07version\x18\x01 \x01(\x05\x12\x0e\n\x06hotkey\x18\x02 \x01(\t\x12\x10\n\x08messages\x18\x03 \x03(\t\x12\x0f\n\x07timeout\x18\x04 \x01(\x02\"\x99\x01\n!MultiForwardTextPromptingResponse\x12\x0f\n\x07version\x18\x01 \x01(\x05\x12\x0e\n\x06hotkey\x18\x02 \x01(\t\x12\x19\n\x11multi_completions\x18\x03 \x03(\t\x12\x16\n\x0ereturn_message\x18\x04 \x01(\t\x12 \n\x0breturn_code\x18\x05 \x01(\x0e\x32\x0b.ReturnCode\"\x85\x01\n\x1c\x42\x61\x63kwardTextPromptingRequest\x12\x0f\n\x07version\x18\x01 \x01(\x05\x12\x0e\n\x06hotkey\x18\x02 \x01(\t\x12\x0f\n\x07rewards\x18\x03 \x03(\x02\x12\x10\n\x08messages\x18\x04 \x03(\t\x12\x10\n\x08response\x18\x05 \x01(\t\x12\x0f\n\x07timeout\x18\x06 \x01(\x02\"z\n\x1d\x42\x61\x63kwardTextPromptingResponse\x12\x0f\n\x07version\x18\x01 \x01(\x05\x12\x0e\n\x06hotkey\x18\x02 \x01(\t\x12\x16\n\x0ereturn_message\x18\x04 \x01(\t\x12 \n\x0breturn_code\x18\x05 \x01(\x0e\x32\x0b.ReturnCode\"\xac\x01\n\x06Tensor\x12\x0f\n\x07version\x18\x01 \x01(\x05\x12\x0e\n\x06\x62uffer\x18\x02 \x01(\x0c\x12\r\n\x05shape\x18\x03 \x03(\x03\x12\x1f\n\nserializer\x18\x04 \x01(\x0e\x32\x0b.Serializer\x12 \n\x0btensor_type\x18\x05 \x01(\x0e\x32\x0b.TensorType\x12\x18\n\x05\x64type\x18\x06 \x01(\x0e\x32\t.DataType\x12\x15\n\rrequires_grad\x18\x08 \x01(\x08*\xda\x04\n\nReturnCode\x12\x0c\n\x08NoReturn\x10\x00\x12\x0b\n\x07Success\x10\x01\x12\x0b\n\x07Timeout\x10\x02\x12\x0b\n\x07\x42\x61\x63koff\x10\x03\x12\x0f\n\x0bUnavailable\x10\x04\x12\x12\n\x0eNotImplemented\x10\x05\x12\x10\n\x0c\x45mptyRequest\x10\x06\x12\x11\n\rEmptyResponse\x10\x07\x12\x13\n\x0fInvalidResponse\x10\x08\x12\x12\n\x0eInvalidRequest\x10\t\x12\x19\n\x15RequestShapeException\x10\n\x12\x1a\n\x16ResponseShapeException\x10\x0b\x12!\n\x1dRequestSerializationException\x10\x0c\x12\"\n\x1eResponseSerializationException\x10\r\x12#\n\x1fRequestDeserializationException\x10\x0e\x12$\n ResponseDeserializationException\x10\x0f\x12\x15\n\x11NotServingNucleus\x10\x10\x12\x12\n\x0eNucleusTimeout\x10\x11\x12\x0f\n\x0bNucleusFull\x10\x12\x12\x1e\n\x1aRequestIncompatibleVersion\x10\x13\x12\x1f\n\x1bResponseIncompatibleVersion\x10\x14\x12\x11\n\rSenderUnknown\x10\x15\x12\x14\n\x10UnknownException\x10\x16\x12\x13\n\x0fUnauthenticated\x10\x17\x12\x0f\n\x0b\x42\x61\x64\x45ndpoint\x10\x18\x12\x0f\n\x0b\x42lacklisted\x10\x19*&\n\nSerializer\x12\x0b\n\x07MSGPACK\x10\x00\x12\x0b\n\x07\x43MPPACK\x10\x01*2\n\nTensorType\x12\t\n\x05TORCH\x10\x00\x12\x0e\n\nTENSORFLOW\x10\x01\x12\t\n\x05NUMPY\x10\x02*h\n\x08\x44\x61taType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07\x46LOAT32\x10\x01\x12\x0b\n\x07\x46LOAT64\x10\x02\x12\t\n\x05INT32\x10\x03\x12\t\n\x05INT64\x10\x04\x12\x08\n\x04UTF8\x10\x05\x12\x0b\n\x07\x46LOAT16\x10\x06\x12\x08\n\x04\x42OOL\x10\x07\x32\xff\x01\n\rTextPrompting\x12H\n\x07\x46orward\x12\x1c.ForwardTextPromptingRequest\x1a\x1d.ForwardTextPromptingResponse\"\x00\x12W\n\x0cMultiForward\x12!.MultiForwardTextPromptingRequest\x1a\".MultiForwardTextPromptingResponse\"\x00\x12K\n\x08\x42\x61\x63kward\x12\x1d.BackwardTextPromptingRequest\x1a\x1e.BackwardTextPromptingResponse\"\x00\x62\x06proto3'
 )
 
 _RETURNCODE = _descriptor.EnumDescriptor(
   name='ReturnCode',
   full_name='ReturnCode',
   filename=None,
   file=DESCRIPTOR,
@@ -159,16 +159,16 @@
       name='Blacklisted', index=25, number=25,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=713,
-  serialized_end=1315,
+  serialized_start=973,
+  serialized_end=1575,
 )
 _sym_db.RegisterEnumDescriptor(_RETURNCODE)
 
 ReturnCode = enum_type_wrapper.EnumTypeWrapper(_RETURNCODE)
 _SERIALIZER = _descriptor.EnumDescriptor(
   name='Serializer',
   full_name='Serializer',
@@ -185,16 +185,16 @@
       name='CMPPACK', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1317,
-  serialized_end=1355,
+  serialized_start=1577,
+  serialized_end=1615,
 )
 _sym_db.RegisterEnumDescriptor(_SERIALIZER)
 
 Serializer = enum_type_wrapper.EnumTypeWrapper(_SERIALIZER)
 _TENSORTYPE = _descriptor.EnumDescriptor(
   name='TensorType',
   full_name='TensorType',
@@ -216,16 +216,16 @@
       name='NUMPY', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1357,
-  serialized_end=1407,
+  serialized_start=1617,
+  serialized_end=1667,
 )
 _sym_db.RegisterEnumDescriptor(_TENSORTYPE)
 
 TensorType = enum_type_wrapper.EnumTypeWrapper(_TENSORTYPE)
 _DATATYPE = _descriptor.EnumDescriptor(
   name='DataType',
   full_name='DataType',
@@ -272,16 +272,16 @@
       name='BOOL', index=7, number=7,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1409,
-  serialized_end=1513,
+  serialized_start=1669,
+  serialized_end=1773,
 )
 _sym_db.RegisterEnumDescriptor(_DATATYPE)
 
 DataType = enum_type_wrapper.EnumTypeWrapper(_DATATYPE)
 NoReturn = 0
 Success = 1
 Timeout = 2
@@ -433,14 +433,127 @@
   oneofs=[
   ],
   serialized_start=136,
   serialized_end=275,
 )
 
 
+_MULTIFORWARDTEXTPROMPTINGREQUEST = _descriptor.Descriptor(
+  name='MultiForwardTextPromptingRequest',
+  full_name='MultiForwardTextPromptingRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='version', full_name='MultiForwardTextPromptingRequest.version', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='hotkey', full_name='MultiForwardTextPromptingRequest.hotkey', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='messages', full_name='MultiForwardTextPromptingRequest.messages', index=2,
+      number=3, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='timeout', full_name='MultiForwardTextPromptingRequest.timeout', index=3,
+      number=4, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=277,
+  serialized_end=379,
+)
+
+
+_MULTIFORWARDTEXTPROMPTINGRESPONSE = _descriptor.Descriptor(
+  name='MultiForwardTextPromptingResponse',
+  full_name='MultiForwardTextPromptingResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='version', full_name='MultiForwardTextPromptingResponse.version', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='hotkey', full_name='MultiForwardTextPromptingResponse.hotkey', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='multi_completions', full_name='MultiForwardTextPromptingResponse.multi_completions', index=2,
+      number=3, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='return_message', full_name='MultiForwardTextPromptingResponse.return_message', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='return_code', full_name='MultiForwardTextPromptingResponse.return_code', index=4,
+      number=5, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=382,
+  serialized_end=535,
+)
+
+
 _BACKWARDTEXTPROMPTINGREQUEST = _descriptor.Descriptor(
   name='BackwardTextPromptingRequest',
   full_name='BackwardTextPromptingRequest',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
@@ -495,16 +608,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=278,
-  serialized_end=411,
+  serialized_start=538,
+  serialized_end=671,
 )
 
 
 _BACKWARDTEXTPROMPTINGRESPONSE = _descriptor.Descriptor(
   name='BackwardTextPromptingResponse',
   full_name='BackwardTextPromptingResponse',
   filename=None,
@@ -548,16 +661,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=413,
-  serialized_end=535,
+  serialized_start=673,
+  serialized_end=795,
 )
 
 
 _TENSOR = _descriptor.Descriptor(
   name='Tensor',
   full_name='Tensor',
   filename=None,
@@ -622,25 +735,28 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=538,
-  serialized_end=710,
+  serialized_start=798,
+  serialized_end=970,
 )
 
 _FORWARDTEXTPROMPTINGRESPONSE.fields_by_name['return_code'].enum_type = _RETURNCODE
+_MULTIFORWARDTEXTPROMPTINGRESPONSE.fields_by_name['return_code'].enum_type = _RETURNCODE
 _BACKWARDTEXTPROMPTINGRESPONSE.fields_by_name['return_code'].enum_type = _RETURNCODE
 _TENSOR.fields_by_name['serializer'].enum_type = _SERIALIZER
 _TENSOR.fields_by_name['tensor_type'].enum_type = _TENSORTYPE
 _TENSOR.fields_by_name['dtype'].enum_type = _DATATYPE
 DESCRIPTOR.message_types_by_name['ForwardTextPromptingRequest'] = _FORWARDTEXTPROMPTINGREQUEST
 DESCRIPTOR.message_types_by_name['ForwardTextPromptingResponse'] = _FORWARDTEXTPROMPTINGRESPONSE
+DESCRIPTOR.message_types_by_name['MultiForwardTextPromptingRequest'] = _MULTIFORWARDTEXTPROMPTINGREQUEST
+DESCRIPTOR.message_types_by_name['MultiForwardTextPromptingResponse'] = _MULTIFORWARDTEXTPROMPTINGRESPONSE
 DESCRIPTOR.message_types_by_name['BackwardTextPromptingRequest'] = _BACKWARDTEXTPROMPTINGREQUEST
 DESCRIPTOR.message_types_by_name['BackwardTextPromptingResponse'] = _BACKWARDTEXTPROMPTINGRESPONSE
 DESCRIPTOR.message_types_by_name['Tensor'] = _TENSOR
 DESCRIPTOR.enum_types_by_name['ReturnCode'] = _RETURNCODE
 DESCRIPTOR.enum_types_by_name['Serializer'] = _SERIALIZER
 DESCRIPTOR.enum_types_by_name['TensorType'] = _TENSORTYPE
 DESCRIPTOR.enum_types_by_name['DataType'] = _DATATYPE
@@ -656,14 +772,28 @@
 ForwardTextPromptingResponse = _reflection.GeneratedProtocolMessageType('ForwardTextPromptingResponse', (_message.Message,), {
   'DESCRIPTOR' : _FORWARDTEXTPROMPTINGRESPONSE,
   '__module__' : 'bittensor._proto.bittensor_pb2'
   # @@protoc_insertion_point(class_scope:ForwardTextPromptingResponse)
   })
 _sym_db.RegisterMessage(ForwardTextPromptingResponse)
 
+MultiForwardTextPromptingRequest = _reflection.GeneratedProtocolMessageType('MultiForwardTextPromptingRequest', (_message.Message,), {
+  'DESCRIPTOR' : _MULTIFORWARDTEXTPROMPTINGREQUEST,
+  '__module__' : 'bittensor._proto.bittensor_pb2'
+  # @@protoc_insertion_point(class_scope:MultiForwardTextPromptingRequest)
+  })
+_sym_db.RegisterMessage(MultiForwardTextPromptingRequest)
+
+MultiForwardTextPromptingResponse = _reflection.GeneratedProtocolMessageType('MultiForwardTextPromptingResponse', (_message.Message,), {
+  'DESCRIPTOR' : _MULTIFORWARDTEXTPROMPTINGRESPONSE,
+  '__module__' : 'bittensor._proto.bittensor_pb2'
+  # @@protoc_insertion_point(class_scope:MultiForwardTextPromptingResponse)
+  })
+_sym_db.RegisterMessage(MultiForwardTextPromptingResponse)
+
 BackwardTextPromptingRequest = _reflection.GeneratedProtocolMessageType('BackwardTextPromptingRequest', (_message.Message,), {
   'DESCRIPTOR' : _BACKWARDTEXTPROMPTINGREQUEST,
   '__module__' : 'bittensor._proto.bittensor_pb2'
   # @@protoc_insertion_point(class_scope:BackwardTextPromptingRequest)
   })
 _sym_db.RegisterMessage(BackwardTextPromptingRequest)
 
@@ -686,31 +816,41 @@
 _TEXTPROMPTING = _descriptor.ServiceDescriptor(
   name='TextPrompting',
   full_name='TextPrompting',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=1516,
-  serialized_end=1682,
+  serialized_start=1776,
+  serialized_end=2031,
   methods=[
   _descriptor.MethodDescriptor(
     name='Forward',
     full_name='TextPrompting.Forward',
     index=0,
     containing_service=None,
     input_type=_FORWARDTEXTPROMPTINGREQUEST,
     output_type=_FORWARDTEXTPROMPTINGRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
+    name='MultiForward',
+    full_name='TextPrompting.MultiForward',
+    index=1,
+    containing_service=None,
+    input_type=_MULTIFORWARDTEXTPROMPTINGREQUEST,
+    output_type=_MULTIFORWARDTEXTPROMPTINGRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
     name='Backward',
     full_name='TextPrompting.Backward',
-    index=1,
+    index=2,
     containing_service=None,
     input_type=_BACKWARDTEXTPROMPTINGREQUEST,
     output_type=_BACKWARDTEXTPROMPTINGRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
 ])
```

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_proto/bittensor_pb2_grpc.py` & `bittensor-4.1.0rc1.post3/bittensor/_proto/bittensor_pb2_grpc.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,19 @@
             channel: A grpc.Channel.
         """
         self.Forward = channel.unary_unary(
                 '/TextPrompting/Forward',
                 request_serializer=bittensor_dot___proto_dot_bittensor__pb2.ForwardTextPromptingRequest.SerializeToString,
                 response_deserializer=bittensor_dot___proto_dot_bittensor__pb2.ForwardTextPromptingResponse.FromString,
                 )
+        self.MultiForward = channel.unary_unary(
+                '/TextPrompting/MultiForward',
+                request_serializer=bittensor_dot___proto_dot_bittensor__pb2.MultiForwardTextPromptingRequest.SerializeToString,
+                response_deserializer=bittensor_dot___proto_dot_bittensor__pb2.MultiForwardTextPromptingResponse.FromString,
+                )
         self.Backward = channel.unary_unary(
                 '/TextPrompting/Backward',
                 request_serializer=bittensor_dot___proto_dot_bittensor__pb2.BackwardTextPromptingRequest.SerializeToString,
                 response_deserializer=bittensor_dot___proto_dot_bittensor__pb2.BackwardTextPromptingResponse.FromString,
                 )
 
 
@@ -31,28 +36,39 @@
 
     def Forward(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def MultiForward(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def Backward(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_TextPromptingServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Forward': grpc.unary_unary_rpc_method_handler(
                     servicer.Forward,
                     request_deserializer=bittensor_dot___proto_dot_bittensor__pb2.ForwardTextPromptingRequest.FromString,
                     response_serializer=bittensor_dot___proto_dot_bittensor__pb2.ForwardTextPromptingResponse.SerializeToString,
             ),
+            'MultiForward': grpc.unary_unary_rpc_method_handler(
+                    servicer.MultiForward,
+                    request_deserializer=bittensor_dot___proto_dot_bittensor__pb2.MultiForwardTextPromptingRequest.FromString,
+                    response_serializer=bittensor_dot___proto_dot_bittensor__pb2.MultiForwardTextPromptingResponse.SerializeToString,
+            ),
             'Backward': grpc.unary_unary_rpc_method_handler(
                     servicer.Backward,
                     request_deserializer=bittensor_dot___proto_dot_bittensor__pb2.BackwardTextPromptingRequest.FromString,
                     response_serializer=bittensor_dot___proto_dot_bittensor__pb2.BackwardTextPromptingResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -78,14 +94,31 @@
         return grpc.experimental.unary_unary(request, target, '/TextPrompting/Forward',
             bittensor_dot___proto_dot_bittensor__pb2.ForwardTextPromptingRequest.SerializeToString,
             bittensor_dot___proto_dot_bittensor__pb2.ForwardTextPromptingResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def MultiForward(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/TextPrompting/MultiForward',
+            bittensor_dot___proto_dot_bittensor__pb2.MultiForwardTextPromptingRequest.SerializeToString,
+            bittensor_dot___proto_dot_bittensor__pb2.MultiForwardTextPromptingResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def Backward(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_serializer/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_serializer/serializer_impl.py` & `bittensor-4.1.0rc1.post3/bittensor/_serializer/serializer_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/chain_data.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/chain_data.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/errors.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/errors.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/delegation.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/delegation.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/log_utilities.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/log_utilities.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/prometheus.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/prometheus.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/registration.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/serving.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/serving.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/set_weights.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/set_weights.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/staking.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/staking.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/transfer.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/extrinsics/unstaking.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/extrinsics/unstaking.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/subtensor_impl.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/subtensor_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_subtensor/subtensor_mock.py` & `bittensor-4.1.0rc1.post3/bittensor/_subtensor/subtensor_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_synapse/synapse.py` & `bittensor-4.1.0rc1.post3/bittensor/_synapse/synapse.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_synapse/text_prompting/miner.py` & `bittensor-4.1.0rc1.post3/bittensor/_synapse/text_prompting/miner.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_synapse/text_prompting/synapse.py` & `bittensor-4.1.0rc1.post3/bittensor/_synapse/text_prompting/synapse.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,23 +19,57 @@
 import torch
 import bittensor
 
 from typing import List, Dict, Union, Callable
 from abc import ABC, abstractmethod
 import json
 
+
+class SynapseForwardMulti( bittensor.SynapseCall ):
+    name: str = "text_prompting_forward_multi"
+    is_forward: bool = True
+    multi_completions: List[ str ] = [""]
+
+    def __init__( 
+            self, 
+            synapse: "TextPromptingSynapseMulti", 
+            request_proto: bittensor.proto.MultiForwardTextPromptingRequest,
+            multi_forward_callback: Callable,
+        ):
+        super().__init__( synapse = synapse, request_proto = request_proto )
+        self.messages: List[ Dict[str, str] ] = request_proto.messages
+        self.formatted_messages = [ json.loads(message) for message in self.messages ]
+        self.multi_forward_callback = multi_forward_callback
+
+    def apply( self ):
+        bittensor.logging.trace( "SynapseForward.apply()" )
+        self.multi_completions = self.multi_forward_callback( messages = self.formatted_messages )
+        bittensor.logging.trace( "SynapseForward.apply() = ", self.multi_completions )
+
+    def get_response_proto( self ) -> bittensor.proto.MultiForwardTextPromptingResponse: 
+        bittensor.logging.trace( "SynapseForward.get_response_proto()")
+        return bittensor.MultiForwardTextPromptingResponse( multi_completions = self.multi_completions )
+            
+    def get_inputs_shape(self) -> Union[torch.Size, None]: 
+        bittensor.logging.trace( "SynapseForward.get_inputs_shape()" )
+        return torch.Size( [ len(message) for message in self.messages ] )
+    
+    def get_outputs_shape(self) -> Union[torch.Size, None]: 
+        bittensor.logging.trace( "SynapseForward.get_outputs_shape()" )
+        return torch.Size( [ len(self.multi_completions) ]  )
+
 class SynapseForward( bittensor.SynapseCall ):
     name: str = "text_prompting_forward"
     is_forward: bool = True
     completion: str = ""
 
     def __init__( 
             self, 
             synapse: "TextPromptingSynapse", 
-            request_proto: bittensor.proto.BackwardTextPromptingRequest,
+            request_proto: bittensor.proto.ForwardTextPromptingRequest,
             forward_callback: Callable,
         ):
         super().__init__( synapse = synapse, request_proto = request_proto )
         self.messages = request_proto.messages
         self.formatted_messages = [ json.loads(message) for message in self.messages ]
         self.forward_callback = forward_callback
 
@@ -96,20 +130,27 @@
         super().__init__( axon = axon )
         self.axon = axon
         bittensor.grpc.add_TextPromptingServicer_to_server( self, self.axon.server )
 
     @abstractmethod
     def forward( self, messages: List[Dict[str, str]] ) -> str: ...
 
+    def multi_forward( self, messages: List[Dict[str, str]] ) -> List[ str ]: ...
+
     @abstractmethod
     def backward( self, messages: List[Dict[str, str]], response: str, rewards: torch.FloatTensor ) -> str: ...
 
     def Forward( self, request: bittensor.proto.ForwardTextPromptingRequest, context: grpc.ServicerContext ) -> bittensor.proto.ForwardTextPromptingResponse:
         call = SynapseForward( self, request, self.forward )
         bittensor.logging.trace( 'Forward: {} '.format( call ) )
         return self.apply( call = call ) 
+
+    def MultiForward( self, request: bittensor.proto.MultiForwardTextPromptingRequest, context: grpc.ServicerContext ) -> bittensor.proto.MultiForwardTextPromptingResponse:
+        call = SynapseForwardMulti( self, request, self.multi_forward )
+        bittensor.logging.trace( 'MultiForward: {} '.format( call ) )
+        return self.apply( call = call ) 
                          
     def Backward( self, request: bittensor.proto.BackwardTextPromptingRequest, context: grpc.ServicerContext ) -> bittensor.proto.BackwardTextPromptingResponse:
         call = SynapseBackward( self, request, self.backward )
         bittensor.logging.trace( 'Backward: {}'.format( call ) )
         return self.apply( call = call )
```

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_threadpool/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_threadpool/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_threadpool/priority_thread_pool_impl.py` & `bittensor-4.1.0rc1.post3/bittensor/_threadpool/priority_thread_pool_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_tokenizer/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_wallet/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/_wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_wallet/wallet_impl.py` & `bittensor-4.1.0rc1.post3/bittensor/_wallet/wallet_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/_wallet/wallet_mock.py` & `bittensor-4.1.0rc1.post3/bittensor/_wallet/wallet_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/utils/__init__.py` & `bittensor-4.1.0rc1.post3/bittensor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/utils/_register_cuda.py` & `bittensor-4.1.0rc1.post3/bittensor/utils/_register_cuda.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/utils/balance.py` & `bittensor-4.1.0rc1.post3/bittensor/utils/balance.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/utils/codes.py` & `bittensor-4.1.0rc1.post3/bittensor/utils/codes.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/utils/formatting.py` & `bittensor-4.1.0rc1.post3/bittensor/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/utils/networking.py` & `bittensor-4.1.0rc1.post3/bittensor/utils/networking.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/utils/registration.py` & `bittensor-4.1.0rc1.post3/bittensor/utils/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/utils/registratrion_old.py` & `bittensor-4.1.0rc1.post3/bittensor/utils/registratrion_old.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/utils/stats.py` & `bittensor-4.1.0rc1.post3/bittensor/utils/stats.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/utils/test_utils.py` & `bittensor-4.1.0rc1.post3/bittensor/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/utils/tokenizer_utils.py` & `bittensor-4.1.0rc1.post3/bittensor/utils/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor/utils/weight_utils.py` & `bittensor-4.1.0rc1.post3/bittensor/utils/weight_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor.egg-info/PKG-INFO` & `bittensor-4.1.0rc1.post3/bittensor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 4.1.0rc1.post2
+Version: 4.1.0rc1.post3
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
 Description: <div align="center">
         
@@ -31,15 +31,15 @@
         Bittensor is a mining network, similar to Bitcoin, that includes built-in incentives designed to encourage miners to provide value by hosting trained or training machine learning models. These models can be queried by clients seeking inference over inputs, such as token-based text generations or numerical embeddings from a large foundation model like GPT-NeoX-20B.
         
         Token-based incentives are designed to drive the network's growth and distribute the value generated by the network directly to the individuals producing that value, without intermediaries. The network is open to all participants, and no individual or group has full control over what is learned, who can profit from it, or who can access it.
         
         To learn more about Bittensor, please read our [paper](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU/view).
         
         # Install
-        Three ways to install Bittensor
+        There are three ways to install Bittensor
         
         1. Through the installer:
         ```
         $ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/opentensor/bittensor/master/scripts/install.sh)"
         ```
         
         2. With pip:
```

### Comparing `bittensor-4.1.0rc1.post2/bittensor.egg-info/SOURCES.txt` & `bittensor-4.1.0rc1.post3/bittensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bittensor-4.1.0rc1.post2/bittensor.egg-info/requires.txt` & `bittensor-4.1.0rc1.post3/bittensor.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ansible_vault>=2.1
 argparse==1.4.0
 backoff==2.1.0
 base58==2.0.1
 certifi==2020.11.8
 cryptography==39.0.0
+datasets==2.12.0
 fuzzywuzzy==0.18.0
 google-api-python-client==2.7.0
 grpcio-tools==1.42.0
 grpcio==1.42.0
 hypothesis==6.47.4
 idna==2.10
 jinja2==3.0
```

### Comparing `bittensor-4.1.0rc1.post2/setup.py` & `bittensor-4.1.0rc1.post3/setup.py`

 * *Files identical despite different names*

