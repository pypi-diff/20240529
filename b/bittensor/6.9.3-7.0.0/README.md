# Comparing `tmp/bittensor-6.9.3.tar.gz` & `tmp/bittensor-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-6.9.3.tar", last modified: Tue Mar 12 21:55:13 2024, max compression
+gzip compressed data, was "bittensor-7.0.0.tar", last modified: Wed May 29 18:47:28 2024, max compression
```

## Comparing `bittensor-6.9.3.tar` & `bittensor-7.0.0.tar`

### file list

```diff
@@ -1,107 +1,86 @@
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.926277 bittensor-6.9.3/
--rw-r--r--   0 alashaabana   (501) staff       (20)     1087 2022-12-14 19:12:32.000000 bittensor-6.9.3/LICENSE
--rw-r--r--   0 alashaabana   (501) staff       (20)    18529 2024-03-12 21:55:13.926085 bittensor-6.9.3/PKG-INFO
--rw-r--r--   0 alashaabana   (501) staff       (20)    17503 2024-02-26 16:25:46.000000 bittensor-6.9.3/README.md
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.912416 bittensor-6.9.3/bin/
--rwxr-xr-x   0 alashaabana   (501) staff       (20)     2012 2024-01-15 19:02:35.000000 bittensor-6.9.3/bin/btcli
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.915516 bittensor-6.9.3/bittensor/
--rw-r--r--   0 alashaabana   (501) staff       (20)     7480 2024-03-12 21:25:56.000000 bittensor-6.9.3/bittensor/__init__.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    67213 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/axon.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    11584 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/btlogging.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    38877 2024-03-12 21:25:56.000000 bittensor-6.9.3/bittensor/chain_data.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    11194 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/cli.py
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.918824 bittensor-6.9.3/bittensor/commands/
--rw-r--r--   0 alashaabana   (501) staff       (20)     3913 2024-01-15 19:02:35.000000 bittensor-6.9.3/bittensor/commands/__init__.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    38241 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/commands/delegates.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    13519 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/identity.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    11154 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/inspect.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     4926 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/list.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    10770 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/commands/metagraph.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     5096 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/misc.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    25743 2024-03-12 21:25:56.000000 bittensor-6.9.3/bittensor/commands/network.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    30254 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/overview.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    25769 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/register.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    28679 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/root.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    23862 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/senate.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    23616 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/stake.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     5781 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/transfer.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    13182 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/unstake.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     9078 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/utils.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    41540 2024-03-12 21:25:56.000000 bittensor-6.9.3/bittensor/commands/wallets.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    14128 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/config.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    37824 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/dendrite.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     4283 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/errors.py
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.920532 bittensor-6.9.3/bittensor/extrinsics/
--rw-r--r--   0 alashaabana   (501) staff       (20)     1120 2023-10-02 18:12:13.000000 bittensor-6.9.3/bittensor/extrinsics/__init__.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    14777 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/extrinsics/delegation.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     8768 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/extrinsics/network.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     6046 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/extrinsics/prometheus.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    20397 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/extrinsics/registration.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     8992 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/extrinsics/root.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    11054 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/extrinsics/senate.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    11140 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/extrinsics/serving.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     5644 2024-03-07 16:45:01.000000 bittensor-6.9.3/bittensor/extrinsics/set_weights.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    19314 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/extrinsics/staking.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     6640 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/extrinsics/transfer.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    16331 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/extrinsics/unstaking.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    32032 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/keyfile.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    47097 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/metagraph.py
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.921085 bittensor-6.9.3/bittensor/mock/
--rw-r--r--   0 alashaabana   (501) staff       (20)     1186 2023-10-02 18:12:13.000000 bittensor-6.9.3/bittensor/mock/__init__.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     3216 2023-10-02 18:12:13.000000 bittensor-6.9.3/bittensor/mock/keyfile_mock.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    51880 2024-03-12 21:25:56.000000 bittensor-6.9.3/bittensor/mock/subtensor_mock.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     5030 2023-10-02 18:12:13.000000 bittensor-6.9.3/bittensor/mock/wallet_mock.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     6981 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/stream.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     3283 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/subnets.py
--rw-r--r--   0 alashaabana   (501) staff       (20)   194474 2024-03-12 21:25:56.000000 bittensor-6.9.3/bittensor/subtensor.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    35031 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/synapse.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     6891 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/tensor.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    10401 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/threadpool.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     1510 2023-10-02 18:12:13.000000 bittensor-6.9.3/bittensor/types.py
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.922254 bittensor-6.9.3/bittensor/utils/
--rw-r--r--   0 alashaabana   (501) staff       (20)     7560 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/utils/__init__.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     3527 2023-12-22 21:03:26.000000 bittensor-6.9.3/bittensor/utils/_register_cuda.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    10075 2023-10-02 18:12:13.000000 bittensor-6.9.3/bittensor/utils/balance.py
--rw-r--r--   0 alashaabana   (501) staff       (20)      553 2023-09-25 14:12:29.000000 bittensor-6.9.3/bittensor/utils/formatting.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     5784 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/utils/networking.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    37774 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/utils/registration.py
--rw-r--r--   0 alashaabana   (501) staff       (20)      630 2023-07-04 20:47:55.000000 bittensor-6.9.3/bittensor/utils/test_utils.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     6327 2023-12-22 21:03:26.000000 bittensor-6.9.3/bittensor/utils/wallet_utils.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    11141 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/utils/weight_utils.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    33414 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/wallet.py
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.916179 bittensor-6.9.3/bittensor.egg-info/
--rw-r--r--   0 alashaabana   (501) staff       (20)    18529 2024-03-12 21:55:13.000000 bittensor-6.9.3/bittensor.egg-info/PKG-INFO
--rw-r--r--   0 alashaabana   (501) staff       (20)     2700 2024-03-12 21:55:13.000000 bittensor-6.9.3/bittensor.egg-info/SOURCES.txt
--rw-r--r--   0 alashaabana   (501) staff       (20)        1 2024-03-12 21:55:13.000000 bittensor-6.9.3/bittensor.egg-info/dependency_links.txt
--rw-r--r--   0 alashaabana   (501) staff       (20)      730 2024-03-12 21:55:13.000000 bittensor-6.9.3/bittensor.egg-info/requires.txt
--rw-r--r--   0 alashaabana   (501) staff       (20)       16 2024-03-12 21:55:13.000000 bittensor-6.9.3/bittensor.egg-info/top_level.txt
--rw-r--r--   0 alashaabana   (501) staff       (20)       38 2024-03-12 21:55:13.926324 bittensor-6.9.3/setup.cfg
--rw-r--r--   0 alashaabana   (501) staff       (20)     3705 2023-10-02 18:12:13.000000 bittensor-6.9.3/setup.py
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.922391 bittensor-6.9.3/tests/
--rw-r--r--   0 alashaabana   (501) staff       (20)     1202 2023-10-02 18:12:13.000000 bittensor-6.9.3/tests/__init__.py
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.922641 bittensor-6.9.3/tests/helpers/
--rw-r--r--   0 alashaabana   (501) staff       (20)     1308 2023-10-02 18:12:13.000000 bittensor-6.9.3/tests/helpers/__init__.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     5565 2023-10-02 18:12:13.000000 bittensor-6.9.3/tests/helpers/helpers.py
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.923304 bittensor-6.9.3/tests/integration_tests/
--rw-r--r--   0 alashaabana   (501) staff       (20)        0 2023-07-20 18:02:20.000000 bittensor-6.9.3/tests/integration_tests/__init__.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    86929 2024-03-11 16:59:34.000000 bittensor-6.9.3/tests/integration_tests/test_cli.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    49428 2024-01-15 19:02:35.000000 bittensor-6.9.3/tests/integration_tests/test_cli_no_network.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     3450 2023-10-02 18:12:13.000000 bittensor-6.9.3/tests/integration_tests/test_metagraph_integration.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    23150 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/integration_tests/test_subtensor_integration.py
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.925187 bittensor-6.9.3/tests/unit_tests/
--rw-r--r--   0 alashaabana   (501) staff       (20)        0 2023-07-20 18:02:20.000000 bittensor-6.9.3/tests/unit_tests/__init__.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     8119 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/test_axon.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    15306 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/test_chain_data.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     8228 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/test_dendrite.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    21841 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/test_keyfile.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     5969 2024-03-11 16:59:34.000000 bittensor-6.9.3/tests/unit_tests/test_metagraph.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     5605 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/test_subtensor.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     7559 2023-10-30 23:32:38.000000 bittensor-6.9.3/tests/unit_tests/test_synapse.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     5648 2023-10-02 18:12:13.000000 bittensor-6.9.3/tests/unit_tests/test_tensor.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    17894 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/test_wallet.py
-drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.925881 bittensor-6.9.3/tests/unit_tests/utils/
--rw-r--r--   0 alashaabana   (501) staff       (20)        0 2023-10-02 18:12:13.000000 bittensor-6.9.3/tests/unit_tests/utils/__init__.py
--rw-r--r--   0 alashaabana   (501) staff       (20)    15327 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/utils/test_balance.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     5390 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/utils/test_networking.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     9661 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/utils/test_utils.py
--rw-r--r--   0 alashaabana   (501) staff       (20)     9661 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/utils/test_weight_utils.py
+drwxr-xr-x   0 ibraheem   (502) staff       (20)        0 2024-05-29 18:47:28.767206 bittensor-7.0.0/
+-rw-r--r--   0 ibraheem   (502) staff       (20)     1087 2024-05-29 16:48:37.000000 bittensor-7.0.0/LICENSE
+-rw-r--r--   0 ibraheem   (502) staff       (20)    18932 2024-05-29 18:47:28.766964 bittensor-7.0.0/PKG-INFO
+-rw-r--r--   0 ibraheem   (502) staff       (20)    17883 2024-05-29 18:32:25.000000 bittensor-7.0.0/README.md
+drwxr-xr-x   0 ibraheem   (502) staff       (20)        0 2024-05-29 18:47:28.745713 bittensor-7.0.0/bin/
+-rwxr-xr-x   0 ibraheem   (502) staff       (20)     2012 2024-05-29 16:48:37.000000 bittensor-7.0.0/bin/btcli
+drwxr-xr-x   0 ibraheem   (502) staff       (20)        0 2024-05-29 18:47:28.750476 bittensor-7.0.0/bittensor/
+-rw-r--r--   0 ibraheem   (502) staff       (20)     9224 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/__init__.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    67196 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/axon.py
+drwxr-xr-x   0 ibraheem   (502) staff       (20)        0 2024-05-29 18:47:28.753758 bittensor-7.0.0/bittensor/btlogging/
+-rw-r--r--   0 ibraheem   (502) staff       (20)     1466 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/btlogging/__init__.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     1529 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/btlogging/defines.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     7019 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/btlogging/format.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     3807 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/btlogging/helpers.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    17751 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/btlogging/loggingmachine.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    43524 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/chain_data.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    12392 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/cli.py
+drwxr-xr-x   0 ibraheem   (502) staff       (20)        0 2024-05-29 18:47:28.760391 bittensor-7.0.0/bittensor/commands/
+-rw-r--r--   0 ibraheem   (502) staff       (20)     3933 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/commands/__init__.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    42629 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/commands/delegates.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    13519 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/commands/identity.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    11154 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/commands/inspect.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     4926 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/commands/list.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    10770 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/commands/metagraph.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     5096 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/commands/misc.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    25743 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/commands/network.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    31474 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/commands/overview.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    25949 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/commands/register.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    28525 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/commands/root.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    23862 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/commands/senate.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    23616 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/commands/stake.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     5781 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/commands/transfer.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    13369 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/commands/unstake.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     9122 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/commands/utils.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    41533 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/commands/wallets.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    15260 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/config.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    38412 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/dendrite.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     4410 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/errors.py
+drwxr-xr-x   0 ibraheem   (502) staff       (20)        0 2024-05-29 18:47:28.762941 bittensor-7.0.0/bittensor/extrinsics/
+-rw-r--r--   0 ibraheem   (502) staff       (20)     1120 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/extrinsics/__init__.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    19011 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/extrinsics/delegation.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     8768 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/extrinsics/network.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     6047 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/extrinsics/prometheus.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    20731 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/extrinsics/registration.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     9317 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/extrinsics/root.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    11038 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/extrinsics/senate.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    11141 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/extrinsics/serving.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     6016 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/extrinsics/set_weights.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    19314 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/extrinsics/staking.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     6640 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/extrinsics/transfer.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    17413 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/extrinsics/unstaking.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    32484 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/keyfile.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    59052 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/metagraph.py
+drwxr-xr-x   0 ibraheem   (502) staff       (20)        0 2024-05-29 18:47:28.764493 bittensor-7.0.0/bittensor/mock/
+-rw-r--r--   0 ibraheem   (502) staff       (20)     1186 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/mock/__init__.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     3216 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/mock/keyfile_mock.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    52306 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/mock/subtensor_mock.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     5030 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/mock/wallet_mock.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     6996 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/stream.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     3283 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/subnets.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)   206743 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/subtensor.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    35016 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/synapse.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     8806 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/tensor.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    10504 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/threadpool.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     1510 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/types.py
+drwxr-xr-x   0 ibraheem   (502) staff       (20)        0 2024-05-29 18:47:28.766720 bittensor-7.0.0/bittensor/utils/
+-rw-r--r--   0 ibraheem   (502) staff       (20)     9119 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/utils/__init__.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     3527 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/utils/_register_cuda.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    10075 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/utils/balance.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)      553 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/utils/formatting.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     5784 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/utils/networking.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    39892 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/utils/registration.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     5304 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/utils/subtensor.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)      630 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/utils/test_utils.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     3100 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/utils/version.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)     6327 2024-05-29 16:48:37.000000 bittensor-7.0.0/bittensor/utils/wallet_utils.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    13028 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/utils/weight_utils.py
+-rw-r--r--   0 ibraheem   (502) staff       (20)    33529 2024-05-29 18:32:25.000000 bittensor-7.0.0/bittensor/wallet.py
+drwxr-xr-x   0 ibraheem   (502) staff       (20)        0 2024-05-29 18:47:28.753176 bittensor-7.0.0/bittensor.egg-info/
+-rw-r--r--   0 ibraheem   (502) staff       (20)    18932 2024-05-29 18:47:28.000000 bittensor-7.0.0/bittensor.egg-info/PKG-INFO
+-rw-r--r--   0 ibraheem   (502) staff       (20)     2073 2024-05-29 18:47:28.000000 bittensor-7.0.0/bittensor.egg-info/SOURCES.txt
+-rw-r--r--   0 ibraheem   (502) staff       (20)        1 2024-05-29 18:47:28.000000 bittensor-7.0.0/bittensor.egg-info/dependency_links.txt
+-rw-r--r--   0 ibraheem   (502) staff       (20)      863 2024-05-29 18:47:28.000000 bittensor-7.0.0/bittensor.egg-info/requires.txt
+-rw-r--r--   0 ibraheem   (502) staff       (20)       10 2024-05-29 18:47:28.000000 bittensor-7.0.0/bittensor.egg-info/top_level.txt
+-rw-r--r--   0 ibraheem   (502) staff       (20)       38 2024-05-29 18:47:28.767250 bittensor-7.0.0/setup.cfg
+-rw-r--r--   0 ibraheem   (502) staff       (20)     3785 2024-05-29 18:32:25.000000 bittensor-7.0.0/setup.py
```

### Comparing `bittensor-6.9.3/LICENSE` & `bittensor-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/PKG-INFO` & `bittensor-7.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 6.9.3
+Version: 7.0.0
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: torch
 License-File: LICENSE
 
 <div align="center">
 
 # **Bittensor** <!-- omit in toc -->
 [![Discord Chat](https://img.shields.io/discord/308323056592486420.svg)](https://discord.gg/bittensor)
 [![PyPI version](https://badge.fury.io/py/bittensor.svg)](https://badge.fury.io/py/bittensor)
@@ -244,14 +245,19 @@
 btcli --print-completion zsh >> ~/.zshrc    # For Zsh
 source ~/.bashrc  # Reload Bash configuration to take effect
 ```
 
 # The Bittensor Package
 The bittensor package contains data structures for interacting with the bittensor ecosystem, writing miners, validators and querying the network. Additionally, it provides many utilities for efficient serialization of Tensors over the wire, performing data analysis of the network, and other useful utilities.
 
+In the 7.0.0 release, we have removed `torch` by default. However, you can still use `torch` by setting the environment variable
+`USE_TORCH=1` and making sure that you have installed the `torch` library. 
+You can install `torch` by running `pip install bittensor[torch]` (if installing via PyPI), or by running `pip install -e ".[torch]"` (if installing from source). 
+We will not be adding any new functionality based on torch.
+
 Wallet: Interface over locally stored bittensor hot + coldkey styled wallets. 
 ```python
 import bittensor
 # Bittensor's wallet maintenance class.
 wallet = bittensor.wallet() 
 # Access the hotkey
 wallet.hotkey 
@@ -296,15 +302,15 @@
 metagraph.load()
 ```
 
 Synapse: Responsible for defining the protocol definition between axon servers and dendrite clients
 ```python
 class Topk( bittensor.Synapse ):
     topk: int = 2  # Number of "top" elements to select
-    input: bittensor.Tensor = pydantic.Field(..., allow_mutation=False)  # Ensure that input cannot be set on the server side. 
+    input: bittensor.Tensor = pydantic.Field(..., frozen=True)  # Ensure that input cannot be set on the server side. 
     v: bittensor.Tensor = None
     i: bittensor.Tensor = None
 
 def topk( synapse: Topk ) -> Topk:
     v, i = torch.topk( synapse.input.deserialize(), k = synapse.topk ) 
     synapse.v = bittensor.Tensor.serialize( v )
     synapse.i = bittensor.Tensor.serialize( i )
@@ -352,16 +358,16 @@
     forward_fn = forward_my_synapse, 
     verify_fn=verify_my_synapse,
     blacklist_fn = blacklist_my_synapse,
     priority_fn = prioritize_my_synape
 ).start()
 ```     
 
-Dendrite: Inheriting from PyTorch's Module class, represents the abstracted implementation of a network client module designed 
-to send requests to those endpoints to receive inputs.
+Dendrite: Represents the abstracted implementation of a network client module
+designed to send requests to those endpoints to receive inputs.
 
 Example:
 ```python
 dendrite_obj = dendrite( wallet = bittensor.wallet() )
 # pings the axon endpoint
 await d( <axon> )
 # ping multiple axon endpoints
```

### Comparing `bittensor-6.9.3/README.md` & `bittensor-7.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,19 @@
 btcli --print-completion zsh >> ~/.zshrc    # For Zsh
 source ~/.bashrc  # Reload Bash configuration to take effect
 ```
 
 # The Bittensor Package
 The bittensor package contains data structures for interacting with the bittensor ecosystem, writing miners, validators and querying the network. Additionally, it provides many utilities for efficient serialization of Tensors over the wire, performing data analysis of the network, and other useful utilities.
 
+In the 7.0.0 release, we have removed `torch` by default. However, you can still use `torch` by setting the environment variable
+`USE_TORCH=1` and making sure that you have installed the `torch` library. 
+You can install `torch` by running `pip install bittensor[torch]` (if installing via PyPI), or by running `pip install -e ".[torch]"` (if installing from source). 
+We will not be adding any new functionality based on torch.
+
 Wallet: Interface over locally stored bittensor hot + coldkey styled wallets. 
 ```python
 import bittensor
 # Bittensor's wallet maintenance class.
 wallet = bittensor.wallet() 
 # Access the hotkey
 wallet.hotkey 
@@ -269,15 +274,15 @@
 metagraph.load()
 ```
 
 Synapse: Responsible for defining the protocol definition between axon servers and dendrite clients
 ```python
 class Topk( bittensor.Synapse ):
     topk: int = 2  # Number of "top" elements to select
-    input: bittensor.Tensor = pydantic.Field(..., allow_mutation=False)  # Ensure that input cannot be set on the server side. 
+    input: bittensor.Tensor = pydantic.Field(..., frozen=True)  # Ensure that input cannot be set on the server side. 
     v: bittensor.Tensor = None
     i: bittensor.Tensor = None
 
 def topk( synapse: Topk ) -> Topk:
     v, i = torch.topk( synapse.input.deserialize(), k = synapse.topk ) 
     synapse.v = bittensor.Tensor.serialize( v )
     synapse.i = bittensor.Tensor.serialize( i )
@@ -325,16 +330,16 @@
     forward_fn = forward_my_synapse, 
     verify_fn=verify_my_synapse,
     blacklist_fn = blacklist_my_synapse,
     priority_fn = prioritize_my_synape
 ).start()
 ```     
 
-Dendrite: Inheriting from PyTorch's Module class, represents the abstracted implementation of a network client module designed 
-to send requests to those endpoints to receive inputs.
+Dendrite: Represents the abstracted implementation of a network client module
+designed to send requests to those endpoints to receive inputs.
 
 Example:
 ```python
 dendrite_obj = dendrite( wallet = bittensor.wallet() )
 # pings the axon endpoint
 await d( <axon> )
 # ping multiple axon endpoints
```

### Comparing `bittensor-6.9.3/bin/btcli` & `bittensor-7.0.0/bin/btcli`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/axon.py` & `bittensor-7.0.0/bittensor/axon.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,37 +16,37 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-import os
-import uuid
+import argparse
+import asyncio
+import contextlib
 import copy
+import inspect
 import json
+import os
+import threading
 import time
-import asyncio
-import inspect
-import uvicorn
-import argparse
 import traceback
-import threading
-import bittensor
-import contextlib
-
+import uuid
 from inspect import signature, Signature, Parameter
+from typing import List, Optional, Tuple, Callable, Any, Dict
+
+import uvicorn
+from fastapi import FastAPI, APIRouter, Depends
 from fastapi.responses import JSONResponse
-from substrateinterface import Keypair
-from fastapi import FastAPI, APIRouter, Request, Response, Depends
-from starlette.responses import Response
-from starlette.requests import Request
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
-from typing import List, Optional, Tuple, Callable, Any, Dict
+from starlette.requests import Request
+from starlette.responses import Response
+from substrateinterface import Keypair
 
+import bittensor
 from bittensor.errors import (
     InvalidRequestNameError,
     SynapseDendriteNoneException,
     SynapseParsingError,
     UnknownSynapseError,
     NotVerifiedException,
     BlacklistedException,
@@ -563,15 +563,15 @@
         self.priority_fns[request_name] = priority_fn
         self.verify_fns[request_name] = (
             verify_fn or self.default_verify
         )  # Use 'default_verify' if 'verify_fn' is None
         self.forward_fns[request_name] = forward_fn
 
         # Parse required hash fields from the forward function protocol defaults
-        required_hash_fields = request_class.__dict__["__fields__"][
+        required_hash_fields = request_class.__dict__["model_fields"][
             "required_hash_fields"
         ].default
         self.required_hash_fields[request_name] = required_hash_fields
 
         return self
 
     @classmethod
```

### Comparing `bittensor-6.9.3/bittensor/chain_data.py` & `bittensor-7.0.0/bittensor/chain_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
-import torch
 import bittensor
-
 import json
 from enum import Enum
 from dataclasses import dataclass, asdict
 from scalecodec.types import GenericCall
 from typing import List, Tuple, Dict, Optional, Any, TypedDict, Union
 from scalecodec.base import RuntimeConfiguration, ScaleBytes
 from scalecodec.type_registry import load_type_registry_preset
 from scalecodec.utils.ss58 import ss58_encode
 
 from .utils import networking as net, U16_MAX, U16_NORMALIZED_FLOAT
 from .utils.balance import Balance
+from .utils.registration import torch, use_torch
 
 custom_rpc_type_registry = {
     "types": {
         "SubnetInfo": {
             "type": "struct",
             "type_mapping": [
                 ["netuid", "Compact<u16>"],
@@ -261,24 +260,51 @@
             ip=net.int_to_ip(int(neuron_info["axon_info"]["ip"])),
             port=neuron_info["axon_info"]["port"],
             ip_type=neuron_info["axon_info"]["ip_type"],
             hotkey=neuron_info["hotkey"],
             coldkey=neuron_info["coldkey"],
         )
 
-    def to_parameter_dict(self) -> "torch.nn.ParameterDict":
-        r"""Returns a torch tensor of the subnet info."""
-        return torch.nn.ParameterDict(self.__dict__)
+    def _to_parameter_dict(
+        self, return_type: str
+    ) -> Union[dict[str, Union[int, str]], "torch.nn.ParameterDict"]:
+        if return_type == "torch":
+            return torch.nn.ParameterDict(self.__dict__)
+        else:
+            return self.__dict__
+
+    def to_parameter_dict(
+        self,
+    ) -> Union[dict[str, Union[int, str]], "torch.nn.ParameterDict"]:
+        """Returns a torch tensor or dict of the subnet info, depending on the USE_TORCH flag set"""
+        if use_torch():
+            return self._to_parameter_dict("torch")
+        else:
+            return self._to_parameter_dict("numpy")
+
+    @classmethod
+    def _from_parameter_dict(
+        cls,
+        parameter_dict: Union[dict[str, Any], "torch.nn.ParameterDict"],
+        return_type: str,
+    ) -> "AxonInfo":
+        if return_type == "torch":
+            return cls(**dict(parameter_dict))
+        else:
+            return cls(**parameter_dict)
 
     @classmethod
     def from_parameter_dict(
-        cls, parameter_dict: "torch.nn.ParameterDict"
+        cls, parameter_dict: Union[dict[str, Any], "torch.nn.ParameterDict"]
     ) -> "AxonInfo":
-        r"""Returns an axon_info object from a torch parameter_dict."""
-        return cls(**dict(parameter_dict))
+        """Returns an axon_info object from a torch parameter_dict or a parameter dict."""
+        if use_torch():
+            return cls._from_parameter_dict(parameter_dict, "torch")
+        else:
+            return cls._from_parameter_dict(parameter_dict, "numpy")
 
 
 class ChainDataType(Enum):
     NeuronInfo = 1
     SubnetInfo = 2
     DelegateInfo = 3
     NeuronInfoLite = 4
@@ -693,15 +719,27 @@
 
         return cls(**prometheus_info_decoded)
 
 
 @dataclass
 class DelegateInfo:
     r"""
-    Dataclass for delegate info.
+    Dataclass for delegate information.
+
+    Args:
+        hotkey_ss58 (str): Hotkey of the delegate for which the information is being fetched.
+        total_stake (int): Total stake of the delegate.
+        nominators (list[Tuple[str, int]]): List of nominators of the delegate and their stake.
+        take (float): Take of the delegate as a percentage.
+        owner_ss58 (str): Coldkey of the owner.
+        registrations (list[int]): List of subnets that the delegate is registered on.
+        validator_permits (list[int]): List of subnets that the delegate is allowed to validate on.
+        return_per_1000 (int): Return per 1000 TAO, for the delegate over a day.
+        total_daily_return (int): Total daily return of the delegate.
+
     """
 
     hotkey_ss58: str  # Hotkey of delegate
     total_stake: Balance  # Total stake of the delegate
     nominators: List[
         Tuple[str, Balance]
     ]  # List of nominators of the delegate and their stake
@@ -825,15 +863,15 @@
 
     @classmethod
     def list_of_tuple_from_vec_u8(
         cls, vec_u8: List[int]
     ) -> Dict[str, List["StakeInfo"]]:
         r"""Returns a list of StakeInfo objects from a ``vec_u8``."""
         decoded: Optional[
-            List[Tuple(str, List[object])]
+            list[tuple[str, list[object]]]
         ] = from_scale_encoding_using_type_string(
             input=vec_u8, type_string="Vec<(AccountId, Vec<StakeInfo>)>"
         )
 
         if decoded is None:
             return {}
 
@@ -938,25 +976,50 @@
                 for netuid, req in decoded["network_connect"]
             },
             emission_value=decoded["emission_values"],
             burn=Balance.from_rao(decoded["burn"]),
             owner_ss58=ss58_encode(decoded["owner"], bittensor.__ss58_format__),
         )
 
-    def to_parameter_dict(self) -> "torch.nn.ParameterDict":
-        r"""Returns a torch tensor of the subnet info."""
-        return torch.nn.ParameterDict(self.__dict__)
+    def _to_parameter_dict(
+        self, return_type: str
+    ) -> Union[dict[str, Any], "torch.nn.ParameterDict"]:
+        if return_type == "torch":
+            return torch.nn.ParameterDict(self.__dict__)
+        else:
+            return self.__dict__
+
+    def to_parameter_dict(self) -> Union[dict[str, Any], "torch.nn.ParameterDict"]:
+        """Returns a torch tensor or dict of the subnet info."""
+        if use_torch():
+            return self._to_parameter_dict("torch")
+        else:
+            return self._to_parameter_dict("numpy")
 
     @classmethod
-    def from_parameter_dict(
+    def _from_parameter_dict_torch(
         cls, parameter_dict: "torch.nn.ParameterDict"
     ) -> "SubnetInfo":
-        r"""Returns a SubnetInfo object from a torch parameter_dict."""
+        """Returns a SubnetInfo object from a torch parameter_dict."""
         return cls(**dict(parameter_dict))
 
+    @classmethod
+    def _from_parameter_dict_numpy(cls, parameter_dict: dict[str, Any]) -> "SubnetInfo":
+        r"""Returns a SubnetInfo object from a parameter_dict."""
+        return cls(**parameter_dict)
+
+    @classmethod
+    def from_parameter_dict(
+        cls, parameter_dict: Union[dict[str, Any], "torch.nn.ParameterDict"]
+    ) -> "SubnetInfo":
+        if use_torch():
+            return cls._from_parameter_dict_torch(parameter_dict)
+        else:
+            return cls._from_parameter_dict_numpy(parameter_dict)
+
 
 @dataclass
 class SubnetHyperparameters:
     r"""
     Dataclass for subnet hyperparameters.
     """
 
@@ -1034,25 +1097,54 @@
             max_validators=decoded["max_validators"],
             serving_rate_limit=decoded["serving_rate_limit"],
             bonds_moving_avg=decoded["bonds_moving_avg"],
             adjustment_alpha=decoded["adjustment_alpha"],
             difficulty=decoded["difficulty"],
         )
 
-    def to_parameter_dict(self) -> "torch.nn.ParameterDict":
-        r"""Returns a torch tensor of the subnet hyperparameters."""
-        return torch.nn.ParameterDict(self.__dict__)
+    def _to_parameter_dict_torch(
+        self, return_type: str
+    ) -> Union[dict[str, Union[int, float, bool]], "torch.nn.ParameterDict"]:
+        if return_type == "torch":
+            return torch.nn.ParameterDict(self.__dict__)
+        else:
+            return self.__dict__
+
+    def to_parameter_dict(
+        self,
+    ) -> Union[dict[str, Union[int, float, bool]], "torch.nn.ParameterDict"]:
+        """Returns a torch tensor or dict of the subnet hyperparameters."""
+        if use_torch():
+            return self._to_parameter_dict_torch("torch")
+        else:
+            return self._to_parameter_dict_torch("numpy")
 
     @classmethod
-    def from_parameter_dict(
+    def _from_parameter_dict_torch(
         cls, parameter_dict: "torch.nn.ParameterDict"
-    ) -> "SubnetInfo":
-        r"""Returns a SubnetHyperparameters object from a torch parameter_dict."""
+    ) -> "SubnetHyperparameters":
+        """Returns a SubnetHyperparameters object from a torch parameter_dict."""
         return cls(**dict(parameter_dict))
 
+    @classmethod
+    def _from_parameter_dict_numpy(
+        cls, parameter_dict: dict[str, Any]
+    ) -> "SubnetHyperparameters":
+        """Returns a SubnetHyperparameters object from a parameter_dict."""
+        return cls(**parameter_dict)
+
+    @classmethod
+    def from_parameter_dict(
+        cls, parameter_dict: Union[dict[str, Any], "torch.nn.ParameterDict"]
+    ) -> "SubnetHyperparameters":
+        if use_torch():
+            return cls._from_parameter_dict_torch(parameter_dict)
+        else:
+            return cls._from_parameter_dict_numpy(parameter_dict)
+
 
 @dataclass
 class IPInfo:
     r"""
     Dataclass for associated IP Info.
     """
 
@@ -1099,23 +1191,53 @@
         r"""Returns a SubnetInfo object from a decoded IPInfo dictionary."""
         return IPInfo(
             ip=bittensor.utils.networking.int_to_ip(decoded["ip"]),
             ip_type=decoded["ip_type_and_protocol"] >> 4,
             protocol=decoded["ip_type_and_protocol"] & 0xF,
         )
 
-    def to_parameter_dict(self) -> "torch.nn.ParameterDict":
-        r"""Returns a torch tensor of the subnet info."""
-        return torch.nn.ParameterDict(self.__dict__)
+    def _to_parameter_dict(
+        self, return_type: str
+    ) -> Union[dict[str, Union[str, int]], "torch.nn.ParameterDict"]:
+        """Returns a torch tensor of the subnet info."""
+        if return_type == "torch":
+            return torch.nn.ParameterDict(self.__dict__)
+        else:
+            return self.__dict__
+
+    def to_parameter_dict(
+        self,
+    ) -> Union[dict[str, Union[str, int]], "torch.nn.ParameterDict"]:
+        """Returns a torch tensor or dict of the subnet IP info."""
+        if use_torch():
+            return self._to_parameter_dict("torch")
+        else:
+            return self._to_parameter_dict("numpy")
 
     @classmethod
-    def from_parameter_dict(cls, parameter_dict: "torch.nn.ParameterDict") -> "IPInfo":
-        r"""Returns a IPInfo object from a torch parameter_dict."""
+    def _from_parameter_dict_torch(
+        cls, parameter_dict: "torch.nn.ParameterDict"
+    ) -> "IPInfo":
+        """Returns a IPInfo object from a torch parameter_dict."""
         return cls(**dict(parameter_dict))
 
+    @classmethod
+    def _from_parameter_dict_numpy(cls, parameter_dict: dict[str, Any]) -> "IPInfo":
+        """Returns a IPInfo object from a parameter_dict."""
+        return cls(**parameter_dict)
+
+    @classmethod
+    def from_parameter_dict(
+        cls, parameter_dict: Union[dict[str, Any], "torch.nn.ParameterDict"]
+    ) -> "IPInfo":
+        if use_torch():
+            return cls._from_parameter_dict_torch(parameter_dict)
+        else:
+            return cls._from_parameter_dict_numpy(parameter_dict)
+
 
 # Senate / Proposal data
 
 
 class ProposalVoteData(TypedDict):
     index: int
     threshold: int
```

### Comparing `bittensor-6.9.3/bittensor/cli.py` & `bittensor-7.0.0/bittensor/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,62 @@
 # DEALINGS IN THE SOFTWARE.
 
 import sys
 import shtab
 import argparse
 import bittensor
 from typing import List, Optional
-from .commands import *
+from .commands import (
+    AutocompleteCommand,
+    DelegateStakeCommand,
+    DelegateUnstakeCommand,
+    GetIdentityCommand,
+    GetWalletHistoryCommand,
+    InspectCommand,
+    ListCommand,
+    ListDelegatesCommand,
+    MetagraphCommand,
+    MyDelegatesCommand,
+    NewColdkeyCommand,
+    NewHotkeyCommand,
+    NominateCommand,
+    OverviewCommand,
+    PowRegisterCommand,
+    ProposalsCommand,
+    RegenColdkeyCommand,
+    RegenColdkeypubCommand,
+    RegenHotkeyCommand,
+    RegisterCommand,
+    RegisterSubnetworkCommand,
+    RootGetWeightsCommand,
+    RootList,
+    RootRegisterCommand,
+    RootSetBoostCommand,
+    RootSetSlashCommand,
+    RootSetWeightsCommand,
+    RunFaucetCommand,
+    SenateCommand,
+    SetIdentityCommand,
+    SetTakeCommand,
+    StakeCommand,
+    StakeShow,
+    SubnetGetHyperparamsCommand,
+    SubnetHyperparamsCommand,
+    SubnetListCommand,
+    SubnetLockCostCommand,
+    SubnetSudoCommand,
+    SwapHotkeyCommand,
+    TransferCommand,
+    UnStakeCommand,
+    UpdateCommand,
+    UpdateWalletCommand,
+    VoteCommand,
+    WalletBalanceCommand,
+    WalletCreateCommand,
+)
 
 # Create a console instance for CLI display.
 console = bittensor.__console__
 
 ALIAS_TO_COMMAND = {
     "subnets": "subnets",
     "root": "root",
@@ -71,14 +118,15 @@
             "get_weights": RootGetWeightsCommand,
             "boost": RootSetBoostCommand,
             "slash": RootSetSlashCommand,
             "senate_vote": VoteCommand,
             "senate": SenateCommand,
             "register": RootRegisterCommand,
             "proposals": ProposalsCommand,
+            "set_take": SetTakeCommand,
             "delegate": DelegateStakeCommand,
             "undelegate": DelegateUnstakeCommand,
             "my_delegates": MyDelegatesCommand,
             "list_delegates": ListDelegatesCommand,
             "nominate": NominateCommand,
         },
     },
@@ -196,16 +244,16 @@
 
         # Check if the config is valid.
         cli.check_config(self.config)
 
         # If no_version_checking is not set or set as False in the config, version checking is done.
         if not self.config.get("no_version_checking", d=True):
             try:
-                bittensor.utils.version_checking()
-            except:
+                bittensor.utils.check_version()
+            except bittensor.utils.VersionCheckError:
                 # If version checking fails, inform user with an exception.
                 raise RuntimeError(
                     "To avoid internet-based version checking, pass --no_version_checking while running the CLI."
                 )
 
     @staticmethod
     def __create_parser__() -> "argparse.ArgumentParser":
@@ -279,15 +327,15 @@
         # Check if command exists, if so, run the corresponding check_config.
         # If command doesn't exist, inform user and exit the program.
         if config.command in COMMANDS:
             command = config.command
             command_data = COMMANDS[command]
 
             if isinstance(command_data, dict):
-                if config["subcommand"] != None:
+                if config["subcommand"] is not None:
                     command_data["commands"][config["subcommand"]].check_config(config)
                 else:
                     console.print(
                         f":cross_mark:[red]Missing subcommand for: {config.command}[/red]"
                     )
                     sys.exit(1)
             else:
@@ -298,14 +346,15 @@
 
     def run(self):
         """
         Executes the command from the configuration.
         """
         # Check for print-completion argument
         if self.config.print_completion:
+            parser = cli.__create_parser__()
             shell = self.config.print_completion
             print(shtab.complete(parser, shell))
             return
 
         # Check if command exists, if so, run the corresponding method.
         # If command doesn't exist, inform user and exit the program.
         command = self.config.command
```

### Comparing `bittensor-6.9.3/bittensor/commands/__init__.py` & `bittensor-7.0.0/bittensor/commands/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 )
 from .delegates import (
     NominateCommand,
     ListDelegatesCommand,
     DelegateStakeCommand,
     DelegateUnstakeCommand,
     MyDelegatesCommand,
+    SetTakeCommand,
 )
 from .wallets import (
     NewColdkeyCommand,
     NewHotkeyCommand,
     RegenColdkeyCommand,
     RegenColdkeypubCommand,
     RegenHotkeyCommand,
```

### Comparing `bittensor-6.9.3/bittensor/commands/delegates.py` & `bittensor-7.0.0/bittensor/commands/delegates.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,32 +11,29 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-import sys
-import os
 import argparse
-import bittensor
-from typing import List, Optional
-from rich.table import Table
-from rich.prompt import Prompt
-from rich.prompt import Confirm
+import os
+import sys
+from typing import List, Dict, Optional
+
 from rich.console import Text
-from tqdm import tqdm
+from rich.prompt import Prompt, FloatPrompt, Confirm
+from rich.table import Table
 from substrateinterface.exceptions import SubstrateRequestException
-from .utils import get_delegates_details, DelegatesDetails
-from .identity import SetIdentityCommand
-from . import defaults
+from tqdm import tqdm
 
-import os
 import bittensor
-from typing import List, Dict, Optional
+from . import defaults
+from .identity import SetIdentityCommand
+from .utils import get_delegates_details, DelegatesDetails
 
 
 def _get_coldkey_wallets_for_path(path: str) -> List["bittensor.wallet"]:
     try:
         wallet_names = next(os.walk(os.path.expanduser(path)))[1]
         return [bittensor.wallet(path=path, name=name) for name in wallet_names]
     except StopIteration:
@@ -56,47 +53,48 @@
 ):
     """
     Displays a formatted table of Bittensor network delegates with detailed statistics to the console.
 
     The table is sorted by total stake in descending order and provides
     a snapshot of delegate performance and status, helping users make informed decisions for staking or nominating.
 
-    This is a helper function that is called by the :func:`list_delegates` and :func:`my_delegates`, and is not intended to be used directly in user code unless specifically required.
+    This is a helper function that is called by the :func:`list_delegates` and :func:`my_delegates`, and is not intended
+    to be used directly in user code unless specifically required.
 
     Args:
-        - delegates (List[bittensor.DelegateInfo]): A list of delegate information objects to be displayed.
-        - prev_delegates (Optional[List[bittensor.DelegateInfo]]): A list of delegate information objects from a previous state, used to calculate changes in stake. Defaults to ``None``.
-        - width (Optional[int]): The width of the console output table. Defaults to ``None``, which will make the table expand to the maximum width of the console.
+        delegates (List[bittensor.DelegateInfo]): A list of delegate information objects to be displayed.
+        prev_delegates (Optional[List[bittensor.DelegateInfo]]): A list of delegate information objects from a previous state, used to calculate changes in stake. Defaults to ``None``.
+        width (Optional[int]): The width of the console output table. Defaults to ``None``, which will make the table expand to the maximum width of the console.
 
-    The output table includes the following columns:
+    The output table contains the following columns:
 
     - INDEX: The numerical index of the delegate.
     - DELEGATE: The name of the delegate.
     - SS58: The truncated SS58 address of the delegate.
     - NOMINATORS: The number of nominators supporting the delegate.
     - DELEGATE STAKE(τ): The stake that is directly delegated to the delegate.
     - TOTAL STAKE(τ): The total stake held by the delegate, including nominators' stake.
     - CHANGE/(4h): The percentage change in the delegate's stake over the past 4 hours.
-    - SUBNETS: A list of subnets the delegate is registered with.
     - VPERMIT: Validator permits held by the delegate for the subnets.
+    - TAKE: The percentage of the delegate's earnings taken by the network.
     - NOMINATOR/(24h)/kτ: The earnings per 1000 τ staked by nominators in the last 24 hours.
     - DELEGATE/(24h): The earnings of the delegate in the last 24 hours.
     - Desc: A brief description provided by the delegate.
 
     Usage:
-        This function is typically used within the Bittensor CLI to show current delegate
-        options to users who are considering where to stake their tokens.
+        This function is typically used within the Bittensor CLI to show current delegate options to users who are considering where to stake their tokens.
 
     Example usage::
 
         show_delegates(current_delegates, previous_delegates, width=80)
 
     Note:
         This function is primarily for display purposes within a command-line interface and does
-        not return any values. It relies on the `rich <https://github.com/Textualize/rich>`_ Python library to render the table in the
+        not return any values. It relies on the `rich <https://github.com/Textualize/rich>`_ Python library to render
+        the table in the
         console.
     """
 
     delegates.sort(key=lambda delegate: delegate.total_stake, reverse=True)
     prev_delegates_dict = {}
     if prev_delegates is not None:
         for prev_delegate in prev_delegates:
@@ -192,25 +190,37 @@
                     )
                 else:
                     rate_change_in_stake_str = "[grey0]0%[/grey0]"
         else:
             rate_change_in_stake_str = "[grey0]NA[/grey0]"
 
         table.add_row(
+            # INDEX
             str(i),
+            # DELEGATE
             Text(delegate_name, style=f"link {delegate_url}"),
+            # SS58
             f"{delegate.hotkey_ss58:8.8}...",
+            # NOMINATORS
             str(len([nom for nom in delegate.nominators if nom[1].rao > 0])),
+            # DELEGATE STAKE
             f"{owner_stake!s:13.13}",
+            # TOTAL STAKE
             f"{delegate.total_stake!s:13.13}",
+            # CHANGE/(4h)
             rate_change_in_stake_str,
+            # VPERMIT
             str(delegate.registrations),
+            # TAKE
             f"{delegate.take * 100:.1f}%",
-            f"{bittensor.Balance.from_tao( delegate.total_daily_return.tao * (1000/ ( 0.001 + delegate.total_stake.tao ) ))!s:6.6}",
-            f"{bittensor.Balance.from_tao( delegate.total_daily_return.tao * (0.18) ) !s:6.6}",
+            # NOMINATOR/(24h)/k
+            f"{bittensor.Balance.from_tao( delegate.total_daily_return.tao * (1000/ (0.001 + delegate.total_stake.tao)))!s:6.6}",
+            # DELEGATE/(24h)
+            f"{bittensor.Balance.from_tao(delegate.total_daily_return.tao * 0.18) !s:6.6}",
+            # Desc
             str(delegate_description),
             end_section=True,
         )
     bittensor.__console__.print(table)
 
 
 class DelegateStakeCommand:
@@ -221,26 +231,31 @@
 
     Optional Arguments:
         - ``wallet.name``: The name of the wallet to use for the command.
         - ``delegate_ss58key``: The ``SS58`` address of the delegate to stake to.
         - ``amount``: The amount of Tao to stake.
         - ``all``: If specified, the command stakes all available Tao.
 
-    The command interacts with the user to determine the delegate and the amount of Tao to be staked. If the ``--all`` flag is used, it delegates the entire available balance.
+    The command interacts with the user to determine the delegate and the amount of Tao to be staked. If the ``--all``
+    flag is used, it delegates the entire available balance.
 
     Usage:
-        The user must specify the delegate's SS58 address and the amount of Tao to stake. The function sends a transaction to the subtensor network to delegate the specified amount to the chosen delegate. These values are prompted if not provided.
+        The user must specify the delegate's SS58 address and the amount of Tao to stake. The function sends a
+        transaction to the subtensor network to delegate the specified amount to the chosen delegate. These values are
+        prompted if not provided.
 
     Example usage::
 
         btcli delegate --delegate_ss58key <SS58_ADDRESS> --amount <AMOUNT>
         btcli delegate --delegate_ss58key <SS58_ADDRESS> --all
 
     Note:
-        This command modifies the blockchain state and may incur transaction fees. It requires user confirmation and interaction, and is designed to be used within the Bittensor CLI environment. The user should ensure the delegate's address and the amount to be staked are correct before executing the command.
+        This command modifies the blockchain state and may incur transaction fees. It requires user confirmation and
+        interaction, and is designed to be used within the Bittensor CLI environment. The user should ensure the
+        delegate's address and the amount to be staked are correct before executing the command.
     """
 
     @staticmethod
     def run(cli: "bittensor.cli"):
         """Delegates stake to a chain delegate."""
         try:
             config = cli.config.copy()
@@ -340,36 +355,42 @@
                     sys.exit()
             else:
                 config.stake_all = True
 
 
 class DelegateUnstakeCommand:
     """
-    Executes the ``undelegate`` command, allowing users to withdraw their staked Tao from a delegate on the Bittensor network.
+    Executes the ``undelegate`` command, allowing users to withdraw their staked Tao from a delegate on the Bittensor
+    network.
 
     This process is known as "undelegating" and it reverses the delegation process, freeing up the staked tokens.
 
     Optional Arguments:
         - ``wallet.name``: The name of the wallet to use for the command.
         - ``delegate_ss58key``: The ``SS58`` address of the delegate to undelegate from.
         - ``amount``: The amount of Tao to undelegate.
         - ``all``: If specified, the command undelegates all staked Tao from the delegate.
 
-    The command prompts the user for the amount of Tao to undelegate and the ``SS58`` address of the delegate from which to undelegate. If the ``--all`` flag is used, it will attempt to undelegate the entire staked amount from the specified delegate.
+    The command prompts the user for the amount of Tao to undelegate and the ``SS58`` address of the delegate from which
+    to undelegate. If the ``--all`` flag is used, it will attempt to undelegate the entire staked amount from the
+    specified delegate.
 
     Usage:
-        The user must provide the delegate's SS58 address and the amount of Tao to undelegate. The function will then send a transaction to the Bittensor network to process the undelegation.
+        The user must provide the delegate's SS58 address and the amount of Tao to undelegate. The function will then
+        send a transaction to the Bittensor network to process the undelegation.
 
     Example usage::
 
         btcli undelegate --delegate_ss58key <SS58_ADDRESS> --amount <AMOUNT>
         btcli undelegate --delegate_ss58key <SS58_ADDRESS> --all
 
     Note:
-        This command can result in a change to the blockchain state and may incur transaction fees. It is interactive and requires confirmation from the user before proceeding. It should be used with care as undelegating can affect the delegate's total stake and
+        This command can result in a change to the blockchain state and may incur transaction fees. It is interactive
+        and requires confirmation from the user before proceeding. It should be used with care as undelegating can
+        affect the delegate's total stake and
         potentially the user's staking rewards.
     """
 
     @staticmethod
     def run(cli: "bittensor.cli"):
         """Undelegates stake from a chain delegate."""
         try:
@@ -379,17 +400,17 @@
             )
             DelegateUnstakeCommand._run(cli, subtensor)
         finally:
             if "subtensor" in locals():
                 subtensor.close()
                 bittensor.logging.debug("closing subtensor connection")
 
-    def _run(cli: "bittensor.cli", subtensor: "bittensor.subtensor"):
+    def _run(self: "bittensor.cli", subtensor: "bittensor.subtensor"):
         """Undelegates stake from a chain delegate."""
-        config = cli.config.copy()
+        config = self.config.copy()
         wallet = bittensor.wallet(config=config)
         subtensor.undelegate(
             wallet=wallet,
             delegate_ss58=config.get("delegate_ss58key"),
             amount=config.get("amount"),
             wait_for_inclusion=True,
             prompt=not config.no_prompt,
@@ -477,15 +498,15 @@
                 config.unstake_all = True
 
 
 class ListDelegatesCommand:
     """
     Displays a formatted table of Bittensor network delegates, providing a comprehensive overview of delegate statistics and information.
 
-    This table helps users make informed decisions on which delegates to allocate their Tao stake.
+    This table helps users make informed decisions on which delegates to allocate their TAO stake.
 
     Optional Arguments:
         - ``wallet.name``: The name of the wallet to use for the command.
         - ``subtensor.network``: The name of the network to use for the command.
 
     The table columns include:
 
@@ -498,50 +519,56 @@
     - CHANGE/(4h): The percentage change in the delegate's stake over the last four hours.
     - SUBNETS: The subnets to which the delegate is registered.
     - VPERMIT: Indicates the subnets for which the delegate has validator permits.
     - NOMINATOR/(24h)/kτ: The earnings per 1000 τ staked by nominators in the last 24 hours.
     - DELEGATE/(24h): The total earnings of the delegate in the last 24 hours.
     - DESCRIPTION: A brief description of the delegate's purpose and operations.
 
-    Sorting is done based on the ``TOTAL STAKE`` column in descending order. Changes in stake are highlighted: increases in green and decreases in red. Entries with no previous data are marked with ``NA``. Each delegate's name is a hyperlink to their respective URL, if available.
+    Sorting is done based on the ``TOTAL STAKE`` column in descending order. Changes in stake are highlighted:
+    increases in green and decreases in red. Entries with no previous data are marked with ``NA``. Each delegate's name
+    is a hyperlink to their respective URL, if available.
 
     Example usage::
 
         btcli root list_delegates
         btcli root list_delegates --wallet.name my_wallet
         btcli root list_delegates --subtensor.network finney # can also be `test` or `local`
 
     Note:
-        This function is part of the Bittensor CLI tools and is intended for use within a console application. It prints directly to the console and does not return any value.
+        This function is part of the Bittensor CLI tools and is intended for use within a console application. It prints
+        directly to the console and does not return any value.
     """
 
     @staticmethod
     def run(cli: "bittensor.cli"):
         r"""
         List all delegates on the network.
         """
         try:
+            cli.config.subtensor.network = "archive"
+            cli.config.subtensor.chain_endpoint = (
+                "wss://archive.chain.opentensor.ai:443"
+            )
             subtensor: "bittensor.subtensor" = bittensor.subtensor(
                 config=cli.config, log_verbose=False
             )
             ListDelegatesCommand._run(cli, subtensor)
         finally:
             if "subtensor" in locals():
                 subtensor.close()
                 bittensor.logging.debug("closing subtensor connection")
 
     @staticmethod
     def _run(cli: "bittensor.cli", subtensor: "bittensor.subtensor"):
         r"""
         List all delegates on the network.
         """
-        cli.config.subtensor.network = "archive"
-        cli.config.subtensor.chain_endpoint = "wss://archive.chain.opentensor.ai:443"
         with bittensor.__console__.status(":satellite: Loading delegates..."):
-            delegates: bittensor.DelegateInfo = subtensor.get_delegates()
+            delegates: list[bittensor.DelegateInfo] = subtensor.get_delegates()
+
             try:
                 prev_delegates = subtensor.get_delegates(max(0, subtensor.block - 1200))
             except SubstrateRequestException:
                 prev_delegates = None
 
         if prev_delegates is None:
             bittensor.__console__.print(
@@ -566,37 +593,41 @@
         pass
 
 
 class NominateCommand:
     """
     Executes the ``nominate`` command, which facilitates a wallet to become a delegate on the Bittensor network.
 
-    This command handles the nomination process, including wallet unlocking and verification of the hotkey's current delegate status.
+    This command handles the nomination process, including wallet unlocking and verification of the hotkey's current
+    delegate status.
 
     The command performs several checks:
 
     - Verifies that the hotkey is not already a delegate to prevent redundant nominations.
     - Tries to nominate the wallet and reports success or failure.
 
     Upon success, the wallet's hotkey is registered as a delegate on the network.
 
     Optional Arguments:
         - ``wallet.name``: The name of the wallet to use for the command.
         - ``wallet.hotkey``: The name of the hotkey to use for the command.
 
     Usage:
-        To run the command, the user must have a configured wallet with both hotkey and coldkey. If the wallet is not already nominated, this command will initiate the process.
+        To run the command, the user must have a configured wallet with both hotkey and coldkey. If the wallet is not
+        already nominated, this command will initiate the process.
 
     Example usage::
 
         btcli root nominate
         btcli root nominate --wallet.name my_wallet --wallet.hotkey my_hotkey
 
     Note:
-        This function is intended to be used as a CLI command. It prints the outcome directly to the console and does not return any value. It should not be called programmatically in user code due to its interactive nature and side effects on the network state.
+        This function is intended to be used as a CLI command. It prints the outcome directly to the console and does
+        not return any value. It should not be called programmatically in user code due to its interactive nature and
+        side effects on the network state.
     """
 
     @staticmethod
     def run(cli: "bittensor.cli"):
         r"""Nominate wallet."""
         try:
             subtensor: "bittensor.subtensor" = bittensor.subtensor(
@@ -680,15 +711,16 @@
         if not config.is_set("wallet.hotkey") and not config.no_prompt:
             hotkey = Prompt.ask("Enter hotkey name", default=defaults.wallet.hotkey)
             config.wallet.hotkey = str(hotkey)
 
 
 class MyDelegatesCommand:
     """
-    Executes the ``my_delegates`` command within the Bittensor CLI, which retrieves and displays a table of delegated stakes from a user's wallet(s) to various delegates on the Bittensor network.
+    Executes the ``my_delegates`` command within the Bittensor CLI, which retrieves and displays a table of delegated
+    stakes from a user's wallet(s) to various delegates on the Bittensor network.
 
     The command provides detailed insights into the user's
     staking activities and the performance of their chosen delegates.
 
     Optional Arguments:
         - ``wallet.name``: The name of the wallet to use for the command.
         - ``all``: If specified, the command aggregates information across all wallets.
@@ -707,15 +739,17 @@
     - VPERMIT: Validator permits held by the delegate for various subnets.
     - 24h/kτ: Earnings per 1000 Tao staked over the last 24 hours.
     - Desc: A description of the delegate.
 
     The command also sums and prints the total amount of Tao delegated across all wallets.
 
     Usage:
-        The command can be run as part of the Bittensor CLI suite of tools and requires no parameters if a single wallet is used. If multiple wallets are present, the ``--all`` flag can be specified to aggregate information across all wallets.
+        The command can be run as part of the Bittensor CLI suite of tools and requires no parameters if a single wallet
+        is used. If multiple wallets are present, the ``--all`` flag can be specified to aggregate information across
+        all wallets.
 
     Example usage::
 
         btcli my_delegates
         btcli my_delegates --all
         btcli my_delegates --wallet.name my_wallet
 
@@ -737,15 +771,15 @@
                 subtensor.close()
                 bittensor.logging.debug("closing subtensor connection")
 
     @staticmethod
     def _run(cli: "bittensor.cli", subtensor: "bittensor.subtensor"):
         """Delegates stake to a chain delegate."""
         config = cli.config.copy()
-        if config.get("all", d=None) == True:
+        if config.get("all", d=None):
             wallets = _get_coldkey_wallets_for_path(config.wallet.path)
         else:
             wallets = [bittensor.wallet(config=config)]
 
         table = Table(show_footer=True, pad_edge=False, box=None, expand=True)
         table.add_column(
             "[overline white]Wallet", footer_style="overline white", style="bold white"
@@ -887,7 +921,121 @@
         if (
             not config.get("all", d=None)
             and not config.is_set("wallet.name")
             and not config.no_prompt
         ):
             wallet_name = Prompt.ask("Enter wallet name", default=defaults.wallet.name)
             config.wallet.name = str(wallet_name)
+
+
+class SetTakeCommand:
+    """
+    Executes the ``set_take`` command, which sets the delegate take.
+
+    The command performs several checks:
+
+        1. Hotkey is already a delegate
+        2. New take value is within 0-18% range
+
+    Optional Arguments:
+        - ``take``: The new take value
+        - ``wallet.name``: The name of the wallet to use for the command.
+        - ``wallet.hotkey``: The name of the hotkey to use for the command.
+
+    Usage:
+        To run the command, the user must have a configured wallet with both hotkey and coldkey. Also, the hotkey should already be a delegate.
+
+    Example usage::
+        btcli root set_take --wallet.name my_wallet --wallet.hotkey my_hotkey
+
+    Note:
+        This function can be used to update the takes individually for every subnet
+    """
+
+    @staticmethod
+    def run(cli: "bittensor.cli"):
+        r"""Set delegate take."""
+        try:
+            subtensor: "bittensor.subtensor" = bittensor.subtensor(
+                config=cli.config, log_verbose=False
+            )
+            SetTakeCommand._run(cli, subtensor)
+        finally:
+            if "subtensor" in locals():
+                subtensor.close()
+                bittensor.logging.debug("closing subtensor connection")
+
+    @staticmethod
+    def _run(cli: "bittensor.cli", subtensor: "bittensor.subtensor"):
+        r"""Set delegate take."""
+        config = cli.config.copy()
+        wallet = bittensor.wallet(config=cli.config)
+
+        # Unlock the wallet.
+        wallet.hotkey
+        wallet.coldkey
+
+        # Check if the hotkey is not a delegate.
+        if not subtensor.is_hotkey_delegate(wallet.hotkey.ss58_address):
+            bittensor.__console__.print(
+                "Aborting: Hotkey {} is NOT a delegate.".format(
+                    wallet.hotkey.ss58_address
+                )
+            )
+            return
+
+        # Prompt user for take value.
+        new_take_str = config.get("take")
+        if new_take_str == None:
+            new_take = FloatPrompt.ask(f"Enter take value (0.18 for 18%)")
+        else:
+            new_take = float(new_take_str)
+
+        if new_take > 0.18:
+            bittensor.__console__.print("ERROR: Take value should not exceed 18%")
+            return
+
+        result: bool = subtensor.set_take(
+            wallet=wallet,
+            delegate_ss58=wallet.hotkey.ss58_address,
+            take=new_take,
+        )
+        if not result:
+            bittensor.__console__.print("Could not set the take")
+        else:
+            # Check if we are a delegate.
+            is_delegate: bool = subtensor.is_hotkey_delegate(wallet.hotkey.ss58_address)
+            if not is_delegate:
+                bittensor.__console__.print(
+                    "Could not set the take [white]{}[/white]".format(subtensor.network)
+                )
+                return
+            bittensor.__console__.print(
+                "Successfully set the take on [white]{}[/white]".format(
+                    subtensor.network
+                )
+            )
+
+    @staticmethod
+    def add_args(parser: argparse.ArgumentParser):
+        set_take_parser = parser.add_parser(
+            "set_take", help="""Set take for delegate"""
+        )
+        set_take_parser.add_argument(
+            "--take",
+            dest="take",
+            type=float,
+            required=False,
+            help="""Take as a float number""",
+        )
+        bittensor.wallet.add_args(set_take_parser)
+        bittensor.subtensor.add_args(set_take_parser)
+
+    @staticmethod
+    def check_config(config: "bittensor.config"):
+        if not config.is_set("wallet.name") and not config.no_prompt:
+            wallet_name = Prompt.ask("Enter wallet name", default=defaults.wallet.name)
+            config.wallet.name = str(wallet_name)
+
+        if not config.is_set("wallet.hotkey") and not config.no_prompt:
+            hotkey = Prompt.ask("Enter hotkey name", default=defaults.wallet.hotkey)
+            config.wallet.hotkey = str(hotkey)
```

### Comparing `bittensor-6.9.3/bittensor/commands/identity.py` & `bittensor-7.0.0/bittensor/commands/identity.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/commands/inspect.py` & `bittensor-7.0.0/bittensor/commands/inspect.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
             "[overline white]Stake", footer_style="overline white", style="green"
         )
         table.add_column(
             "[overline white]Emission", footer_style="overline white", style="green"
         )
         for wallet in tqdm(wallets):
             delegates: List[
-                Tuple(bittensor.DelegateInfo, bittensor.Balance)
+                Tuple[bittensor.DelegateInfo, bittensor.Balance]
             ] = subtensor.get_delegated(coldkey_ss58=wallet.coldkeypub.ss58_address)
             if not wallet.coldkeypub_file.exists_on_device():
                 continue
             cold_balance = subtensor.get_balance(wallet.coldkeypub.ss58_address)
             table.add_row(wallet.name, str(cold_balance), "", "", "", "", "", "", "")
             for dele, staked in delegates:
                 if dele.hotkey_ss58 in registered_delegate_info:
```

### Comparing `bittensor-6.9.3/bittensor/commands/list.py` & `bittensor-7.0.0/bittensor/commands/list.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/commands/metagraph.py` & `bittensor-7.0.0/bittensor/commands/metagraph.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/commands/misc.py` & `bittensor-7.0.0/bittensor/commands/misc.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/commands/network.py` & `bittensor-7.0.0/bittensor/commands/network.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/commands/overview.py` & `bittensor-7.0.0/bittensor/commands/overview.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,23 +86,20 @@
             )
             OverviewCommand._run(cli, subtensor)
         finally:
             if "subtensor" in locals():
                 subtensor.close()
                 bittensor.logging.debug("closing subtensor connection")
 
-    def _run(cli: "bittensor.cli", subtensor: "bittensor.subtensor"):
-        r"""Prints an overview for the wallet's colkey."""
-        console = bittensor.__console__
-        wallet = bittensor.wallet(config=cli.config)
-
-        all_hotkeys = []
-        total_balance = bittensor.Balance(0)
-
-        # We are printing for every coldkey.
+    @staticmethod
+    def _get_total_balance(
+        total_balance: "bittensor.Balance",
+        subtensor: "bittensor.subtensor",
+        cli: "bittensor.cli",
+    ) -> Tuple[List["bittensor.wallet"], "bittensor.Balance"]:
         if cli.config.get("all", d=None):
             cold_wallets = get_coldkey_wallets_for_path(cli.config.wallet.path)
             for cold_wallet in tqdm(cold_wallets, desc="Pulling balances"):
                 if (
                     cold_wallet.coldkeypub_file.exists_on_device()
                     and not cold_wallet.coldkeypub_file.is_encrypted()
                 ):
@@ -118,34 +115,90 @@
                 and not coldkey_wallet.coldkeypub_file.is_encrypted()
             ):
                 total_balance = subtensor.get_balance(
                     coldkey_wallet.coldkeypub.ss58_address
                 )
             if not coldkey_wallet.coldkeypub_file.exists_on_device():
                 console.print("[bold red]No wallets found.")
-                return
+                return [], None
             all_hotkeys = get_hotkey_wallets_for_wallet(coldkey_wallet)
 
-        # We are printing for a select number of hotkeys from all_hotkeys.
+        return all_hotkeys, total_balance
+
+    @staticmethod
+    def _get_hotkeys(
+        cli: "bittensor.cli", all_hotkeys: List["bittensor.wallet"]
+    ) -> List["bittensor.wallet"]:
+        if not cli.config.get("all_hotkeys", False):
+            # We are only showing hotkeys that are specified.
+            all_hotkeys = [
+                hotkey
+                for hotkey in all_hotkeys
+                if hotkey.hotkey_str in cli.config.hotkeys
+            ]
+        else:
+            # We are excluding the specified hotkeys from all_hotkeys.
+            all_hotkeys = [
+                hotkey
+                for hotkey in all_hotkeys
+                if hotkey.hotkey_str not in cli.config.hotkeys
+            ]
+        return all_hotkeys
+
+    @staticmethod
+    def _get_key_address(all_hotkeys: List["bittensor.wallet"]):
+        hotkey_coldkey_to_hotkey_wallet = {}
+        for hotkey_wallet in all_hotkeys:
+            if hotkey_wallet.hotkey.ss58_address not in hotkey_coldkey_to_hotkey_wallet:
+                hotkey_coldkey_to_hotkey_wallet[hotkey_wallet.hotkey.ss58_address] = {}
+
+            hotkey_coldkey_to_hotkey_wallet[hotkey_wallet.hotkey.ss58_address][
+                hotkey_wallet.coldkeypub.ss58_address
+            ] = hotkey_wallet
+
+        all_hotkey_addresses = list(hotkey_coldkey_to_hotkey_wallet.keys())
+
+        return all_hotkey_addresses, hotkey_coldkey_to_hotkey_wallet
 
-        if cli.config.get("hotkeys", []):
-            if not cli.config.get("all_hotkeys", False):
-                # We are only showing hotkeys that are specified.
-                all_hotkeys = [
-                    hotkey
-                    for hotkey in all_hotkeys
-                    if hotkey.hotkey_str in cli.config.hotkeys
-                ]
+    @staticmethod
+    def _process_neuron_results(
+        results: List[Tuple[int, List["bittensor.NeuronInfoLite"], Optional[str]]],
+        neurons: Dict[str, List["bittensor.NeuronInfoLite"]],
+        netuids: List[int],
+    ) -> Dict[str, List["bittensor.NeuronInfoLite"]]:
+        for result in results:
+            netuid, neurons_result, err_msg = result
+            if err_msg is not None:
+                console.print(f"netuid '{netuid}': {err_msg}")
+
+            if len(neurons_result) == 0:
+                # Remove netuid from overview if no neurons are found.
+                netuids.remove(netuid)
+                del neurons[str(netuid)]
             else:
-                # We are excluding the specified hotkeys from all_hotkeys.
-                all_hotkeys = [
-                    hotkey
-                    for hotkey in all_hotkeys
-                    if hotkey.hotkey_str not in cli.config.hotkeys
-                ]
+                # Add neurons to overview.
+                neurons[str(netuid)] = neurons_result
+        return neurons
+
+    def _run(cli: "bittensor.cli", subtensor: "bittensor.subtensor"):
+        r"""Prints an overview for the wallet's colkey."""
+        console = bittensor.__console__
+        wallet = bittensor.wallet(config=cli.config)
+
+        all_hotkeys = []
+        total_balance = bittensor.Balance(0)
+
+        # We are printing for every coldkey.
+        all_hotkeys, total_balance = OverviewCommand._get_total_balance(
+            total_balance, subtensor, cli
+        )
+
+        # We are printing for a select number of hotkeys from all_hotkeys.
+        if cli.config.get("hotkeys"):
+            all_hotkeys = OverviewCommand._get_hotkeys(cli, all_hotkeys)
 
         # Check we have keys to display.
         if len(all_hotkeys) == 0:
             console.print("[red]No wallets found.[/red]")
             return
 
         # Pull neuron info for all keys.
@@ -157,29 +210,24 @@
             cli, subtensor, netuids, all_hotkeys
         )
         bittensor.logging.debug(f"Netuids to check: {netuids}")
 
         for netuid in netuids:
             neurons[str(netuid)] = []
 
-        all_wallet_names = set([wallet.name for wallet in all_hotkeys])
+        all_wallet_names = {wallet.name for wallet in all_hotkeys}
         all_coldkey_wallets = [
             bittensor.wallet(name=wallet_name) for wallet_name in all_wallet_names
         ]
 
-        hotkey_coldkey_to_hotkey_wallet = {}
-        for hotkey_wallet in all_hotkeys:
-            if hotkey_wallet.hotkey.ss58_address not in hotkey_coldkey_to_hotkey_wallet:
-                hotkey_coldkey_to_hotkey_wallet[hotkey_wallet.hotkey.ss58_address] = {}
-
-            hotkey_coldkey_to_hotkey_wallet[hotkey_wallet.hotkey.ss58_address][
-                hotkey_wallet.coldkeypub.ss58_address
-            ] = hotkey_wallet
+        (
+            all_hotkey_addresses,
+            hotkey_coldkey_to_hotkey_wallet,
+        ) = OverviewCommand._get_key_address(all_hotkeys)
 
-        all_hotkey_addresses = list(hotkey_coldkey_to_hotkey_wallet.keys())
         with console.status(
             ":satellite: Syncing with chain: [white]{}[/white] ...".format(
                 cli.config.subtensor.get(
                     "network", bittensor.defaults.subtensor.network
                 )
             )
         ):
@@ -194,26 +242,17 @@
             with ProcessPoolExecutor(max_workers=max(len(netuids), 5)) as executor:
                 results = executor.map(
                     OverviewCommand._get_neurons_for_netuid,
                     [(copy_config, netuid, all_hotkey_addresses) for netuid in netuids],
                 )
                 executor.shutdown(wait=True)  # wait for all complete
 
-                for result in results:
-                    netuid, neurons_result, err_msg = result
-                    if err_msg is not None:
-                        console.print(f"netuid '{netuid}': {err_msg}")
-
-                    if len(neurons_result) == 0:
-                        # Remove netuid from overview if no neurons are found.
-                        netuids.remove(netuid)
-                        del neurons[str(netuid)]
-                    else:
-                        # Add neurons to overview.
-                        neurons[str(netuid)] = neurons_result
+                neurons = OverviewCommand._process_neuron_results(
+                    results, neurons, netuids
+                )
 
             total_coldkey_stake_from_metagraph = defaultdict(
                 lambda: bittensor.Balance(0.0)
             )
             checked_hotkeys = set()
             for neuron_list in neurons.values():
                 for neuron in neuron_list:
@@ -245,15 +284,15 @@
                 coldkeys_to_check.append(coldkey_wallet)
                 alerts_table.add_row(
                     "Found {} stake with coldkey {} that is not registered.".format(
                         difference, coldkey_wallet.coldkeypub.ss58_address
                     )
                 )
 
-            if len(coldkeys_to_check) > 0:
+            if coldkeys_to_check:
                 # We have some stake that is not with a registered hotkey.
                 if "-1" not in neurons:
                     neurons["-1"] = []
 
             # Use process pool to check each coldkey wallet for de-registered stake.
             with ProcessPoolExecutor(
                 max_workers=max(len(coldkeys_to_check), 5)
@@ -290,15 +329,15 @@
                     # Add this hotkey to the wallets dict
                     wallet_ = bittensor.wallet(
                         name=wallet,
                     )
                     wallet_.hotkey_ss58 = hotkey_addr
                     wallet.hotkey_str = hotkey_addr[:5]  # Max length of 5 characters
                     # Indicates a hotkey not on local machine but exists in stake_info obj on-chain
-                    if hotkey_coldkey_to_hotkey_wallet.get(hotkey_addr) == None:
+                    if hotkey_coldkey_to_hotkey_wallet.get(hotkey_addr) is None:
                         hotkey_coldkey_to_hotkey_wallet[hotkey_addr] = {}
                     hotkey_coldkey_to_hotkey_wallet[hotkey_addr][
                         coldkey_wallet.coldkeypub.ss58_address
                     ] = wallet_
 
                 # Add neurons to overview.
                 neurons["-1"].extend(de_registered_neurons)
```

### Comparing `bittensor-6.9.3/bittensor/commands/register.py` & `bittensor-7.0.0/bittensor/commands/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         # Verify subnet exists
         if not subtensor.subnet_exists(netuid=cli.config.netuid):
             bittensor.__console__.print(
                 f"[red]Subnet {cli.config.netuid} does not exist[/red]"
             )
             sys.exit(1)
 
-        subtensor.register(
+        registered = subtensor.register(
             wallet=wallet,
             netuid=cli.config.netuid,
             prompt=not cli.config.no_prompt,
             tpb=cli.config.pow_register.cuda.get("tpb", None),
             update_interval=cli.config.pow_register.get("update_interval", None),
             num_processes=cli.config.pow_register.get("num_processes", None),
             cuda=cli.config.pow_register.cuda.get(
@@ -230,14 +230,16 @@
             output_in_place=cli.config.pow_register.get(
                 "output_in_place", defaults.pow_register.output_in_place
             ),
             log_verbose=cli.config.pow_register.get(
                 "verbose", defaults.pow_register.verbose
             ),
         )
+        if not registered:
+            sys.exit(1)
 
     @staticmethod
     def add_args(parser: argparse.ArgumentParser):
         register_parser = parser.add_parser(
             "pow_register", help="""Register a wallet to a network using PoW."""
         )
         register_parser.add_argument(
@@ -404,15 +406,15 @@
                 subtensor.close()
                 bittensor.logging.debug("closing subtensor connection")
 
     @staticmethod
     def _run(cli: "bittensor.cli", subtensor: "bittensor.subtensor"):
         r"""Register neuron."""
         wallet = bittensor.wallet(config=cli.config)
-        subtensor.run_faucet(
+        success = subtensor.run_faucet(
             wallet=wallet,
             prompt=not cli.config.no_prompt,
             tpb=cli.config.pow_register.cuda.get("tpb", None),
             update_interval=cli.config.pow_register.get("update_interval", None),
             num_processes=cli.config.pow_register.get("num_processes", None),
             cuda=cli.config.pow_register.cuda.get(
                 "use_cuda", defaults.pow_register.cuda.use_cuda
@@ -421,14 +423,17 @@
             output_in_place=cli.config.pow_register.get(
                 "output_in_place", defaults.pow_register.output_in_place
             ),
             log_verbose=cli.config.pow_register.get(
                 "verbose", defaults.pow_register.verbose
             ),
         )
+        if not success:
+            bittensor.logging.error("Faucet run failed.")
+            sys.exit(1)
 
     @staticmethod
     def add_args(parser: argparse.ArgumentParser):
         run_faucet_parser = parser.add_parser(
             "faucet", help="""Perform PoW to receieve test TAO in your wallet."""
         )
         run_faucet_parser.add_argument(
```

### Comparing `bittensor-6.9.3/bittensor/commands/root.py` & `bittensor-7.0.0/bittensor/commands/root.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import re
-import torch
 import typing
 import argparse
 import numpy as np
 import bittensor
 from typing import List, Optional, Dict
 from rich.prompt import Prompt
 from rich.table import Table
@@ -279,15 +278,14 @@
                 subtensor.close()
                 bittensor.logging.debug("closing subtensor connection")
 
     @staticmethod
     def _run(cli: "bittensor.cli", subtensor: "bittensor.subtensor"):
         r"""Set weights for root network."""
         wallet = bittensor.wallet(config=cli.config)
-        subnets: List[bittensor.SubnetInfo] = subtensor.get_all_subnets_info()
 
         root = subtensor.metagraph(0, lite=False)
         try:
             my_uid = root.hotkeys.index(wallet.hotkey.ss58_address)
         except ValueError:
             bittensor.__console__.print(
                 "Wallet hotkey: {} not found in root metagraph".format(wallet.hotkey)
@@ -297,15 +295,15 @@
         prev_weight = my_weights[cli.config.netuid]
         new_weight = prev_weight + cli.config.amount
 
         bittensor.__console__.print(
             f"Boosting weight for netuid {cli.config.netuid} from {prev_weight} -> {new_weight}"
         )
         my_weights[cli.config.netuid] = new_weight
-        all_netuids = torch.tensor(list(range(len(my_weights))))
+        all_netuids = np.arange(len(my_weights))
 
         bittensor.__console__.print("Setting root weights...")
         subtensor.root_set_weights(
             wallet=wallet,
             netuids=all_netuids,
             weights=my_weights,
             version_key=0,
@@ -397,15 +395,14 @@
             if "subtensor" in locals():
                 subtensor.close()
                 bittensor.logging.debug("closing subtensor connection")
 
     @staticmethod
     def _run(cli: "bittensor.cli", subtensor: "bittensor.subtensor"):
         wallet = bittensor.wallet(config=cli.config)
-        subnets: List[bittensor.SubnetInfo] = subtensor.get_all_subnets_info()
 
         bittensor.__console__.print(
             "Slashing weight for subnet: {} by amount: {}".format(
                 cli.config.netuid, cli.config.amount
             )
         )
         root = subtensor.metagraph(0, lite=False)
@@ -415,15 +412,15 @@
             bittensor.__console__.print(
                 "Wallet hotkey: {} not found in root metagraph".format(wallet.hotkey)
             )
             exit()
         my_weights = root.weights[my_uid]
         my_weights[cli.config.netuid] -= cli.config.amount
         my_weights[my_weights < 0] = 0  # Ensure weights don't go negative
-        all_netuids = torch.tensor(list(range(len(my_weights))))
+        all_netuids = np.arange(len(my_weights))
 
         subtensor.root_set_weights(
             wallet=wallet,
             netuids=all_netuids,
             weights=my_weights,
             version_key=0,
             prompt=not cli.config.no_prompt,
@@ -516,21 +513,21 @@
                     )
                 )
                 + " ..."
             )
             cli.config.weights = Prompt.ask(f"Enter weights (e.g. {example})")
 
         # Parse from string
-        netuids = torch.tensor(
-            list(map(int, re.split(r"[ ,]+", cli.config.netuids))), dtype=torch.long
-        )
-        weights = torch.tensor(
-            list(map(float, re.split(r"[ ,]+", cli.config.weights))),
-            dtype=torch.float32,
-        )
+        matched_netuids = list(map(int, re.split(r"[ ,]+", cli.config.netuids)))
+        netuids = np.array(matched_netuids, dtype=np.int64)
+
+        matched_weights = [
+            float(weight) for weight in re.split(r"[ ,]+", cli.config.weights)
+        ]
+        weights = np.array(matched_weights, dtype=np.float32)
 
         # Run the set weights operation.
         subtensor.root_set_weights(
             wallet=wallet,
             netuids=netuids,
             weights=weights,
             version_key=0,
```

### Comparing `bittensor-6.9.3/bittensor/commands/senate.py` & `bittensor-7.0.0/bittensor/commands/senate.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/commands/stake.py` & `bittensor-7.0.0/bittensor/commands/stake.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/commands/transfer.py` & `bittensor-7.0.0/bittensor/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/commands/unstake.py` & `bittensor-7.0.0/bittensor/commands/unstake.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,30 +81,31 @@
             hotkeys: str = ""
             if config.get("all_hotkeys"):
                 hotkeys = "all hotkeys"
             elif config.get("hotkeys"):
                 hotkeys = str(config.hotkeys).replace("[", "").replace("]", "")
             else:
                 hotkeys = str(config.wallet.hotkey)
-            if not Confirm.ask(
-                "Unstake all Tao from: [bold]'{}'[/bold]?".format(hotkeys)
-            ):
-                amount = Prompt.ask("Enter Tao amount to unstake")
-                config.unstake_all = False
-                try:
-                    config.amount = float(amount)
-                except ValueError:
-                    console.print(
-                        ":cross_mark:[red] Invalid Tao amount[/red] [bold white]{}[/bold white]".format(
-                            amount
-                        )
-                    )
-                    sys.exit()
-            else:
+            if config.no_prompt:
                 config.unstake_all = True
+            else:
+                # I really don't like this logic flow. It can be a bit confusing to read for something
+                # as serious as unstaking all.
+                if Confirm.ask(f"Unstake all Tao from: [bold]'{hotkeys}'[/bold]?"):
+                    config.unstake_all = True
+                else:
+                    config.unstake_all = False
+                    amount = Prompt.ask("Enter Tao amount to unstake")
+                    try:
+                        config.amount = float(amount)
+                    except ValueError:
+                        console.print(
+                            f":cross_mark:[red] Invalid Tao amount[/red] [bold white]{amount}[/bold white]"
+                        )
+                        sys.exit()
 
     @staticmethod
     def add_args(command_parser):
         unstake_parser = command_parser.add_parser(
             "remove",
             help="""Remove stake from the specified hotkey into the coldkey balance.""",
         )
```

### Comparing `bittensor-6.9.3/bittensor/commands/utils.py` & `bittensor-7.0.0/bittensor/commands/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import sys
 import os
-import torch
 import bittensor
+import requests
+from bittensor.utils.registration import torch
 from typing import List, Dict, Any, Optional
 from rich.prompt import Confirm, PromptBase
-import requests
 from dataclasses import dataclass
 from . import defaults
 
 console = bittensor.__console__
 
 
 class IntListPrompt(PromptBase):
@@ -74,17 +74,17 @@
                 config.netuid = int(netuid)
             except:
                 raise ValueError('netuid must be an integer or "None" (if applicable)')
 
 
 def check_for_cuda_reg_config(config: "bittensor.config") -> None:
     """Checks, when CUDA is available, if the user would like to register with their CUDA device."""
-    if torch.cuda.is_available():
+    if torch and torch.cuda.is_available():
         if not config.no_prompt:
-            if config.pow_register.cuda.get("use_cuda") == None:  # flag not set
+            if config.pow_register.cuda.get("use_cuda") is None:  # flag not set
                 # Ask about cuda registration only if a CUDA device is available.
                 cuda = Confirm.ask("Detected CUDA device, use CUDA for registration?\n")
                 config.pow_register.cuda.use_cuda = cuda
 
             # Only ask about which CUDA device if the user has more than one CUDA device.
             if (
                 config.pow_register.cuda.use_cuda
```

### Comparing `bittensor-6.9.3/bittensor/commands/wallets.py` & `bittensor-7.0.0/bittensor/commands/wallets.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,18 +62,16 @@
         json_password: Optional[str] = None
         if cli.config.get("json"):
             file_name: str = cli.config.get("json")
             if not os.path.exists(file_name) or not os.path.isfile(file_name):
                 raise ValueError("File {} does not exist".format(file_name))
             with open(cli.config.get("json"), "r") as f:
                 json_str = f.read()
-
             # Password can be "", assume if None
             json_password = cli.config.get("json_password", "")
-
         wallet.regenerate_coldkey(
             mnemonic=cli.config.mnemonic,
             seed=cli.config.seed,
             json=(json_str, json_password),
             use_password=cli.config.use_password,
             overwrite=cli.config.overwrite_coldkey,
         )
@@ -142,15 +140,15 @@
             dest="use_password",
             action="store_false",
             help="""Set off protects the generated bittensor key with a password.""",
         )
         regen_coldkey_parser.add_argument(
             "--overwrite_coldkey",
             default=False,
-            action="store_false",
+            action="store_true",
             help="""Overwrite the old coldkey with the newly generated coldkey""",
         )
         bittensor.wallet.add_args(regen_coldkey_parser)
         bittensor.subtensor.add_args(regen_coldkey_parser)
 
 
 class RegenColdkeypubCommand:
@@ -439,15 +437,15 @@
             "--no_password",
             dest="use_password",
             action="store_false",
             help="""Set off protects the generated bittensor key with a password.""",
         )
         new_hotkey_parser.add_argument(
             "--overwrite_hotkey",
-            action="store_false",
+            action="store_true",
             default=False,
             help="""Overwrite the old hotkey with the newly generated hotkey""",
         )
         bittensor.wallet.add_args(new_hotkey_parser)
         bittensor.subtensor.add_args(new_hotkey_parser)
 
 
@@ -514,15 +512,15 @@
             "--no_password",
             dest="use_password",
             action="store_false",
             help="""Set off protects the generated bittensor key with a password.""",
         )
         new_coldkey_parser.add_argument(
             "--overwrite_coldkey",
-            action="store_false",
+            action="store_true",
             default=False,
             help="""Overwrite the old coldkey with the newly generated coldkey""",
         )
         bittensor.wallet.add_args(new_coldkey_parser)
         bittensor.subtensor.add_args(new_coldkey_parser)
 
 
@@ -598,21 +596,21 @@
             "--no_password",
             dest="use_password",
             action="store_false",
             help="""Set off protects the generated bittensor key with a password.""",
         )
         new_coldkey_parser.add_argument(
             "--overwrite_coldkey",
-            action="store_false",
+            action="store_true",
             default=False,
             help="""Overwrite the old coldkey with the newly generated coldkey""",
         )
         new_coldkey_parser.add_argument(
             "--overwrite_hotkey",
-            action="store_false",
+            action="store_true",
             default=False,
             help="""Overwrite the old hotkey with the newly generated hotkey""",
         )
         bittensor.wallet.add_args(new_coldkey_parser)
         bittensor.subtensor.add_args(new_coldkey_parser)
```

### Comparing `bittensor-6.9.3/bittensor/config.py` & `bittensor-7.0.0/bittensor/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -119,14 +119,22 @@
             # this can fail if --no_version_checking has already been added.
             pass
 
         # Get args from argv if not passed in.
         if args == None:
             args = sys.argv[1:]
 
+        # Check for missing required arguments before proceeding
+        missing_required_args = self.__check_for_missing_required_args(parser, args)
+        if missing_required_args:
+            # Handle missing required arguments gracefully
+            raise ValueError(
+                f"Missing required arguments: {', '.join(missing_required_args)}"
+            )
+
         # 1.1 Optionally load defaults if the --config is set.
         try:
             config_file_path = (
                 str(os.getcwd())
                 + "/"
                 + vars(parser.parse_known_args(args)[0])["config"]
             )
@@ -369,14 +377,31 @@
         Returns a boolean indicating whether the parameter has been set or is still the default.
         """
         if param_name not in self.get("__is_set"):
             return False
         else:
             return self.get("__is_set")[param_name]
 
+    def __check_for_missing_required_args(
+        self, parser: argparse.ArgumentParser, args: List[str]
+    ) -> List[str]:
+        required_args = self.__get_required_args_from_parser(parser)
+        missing_args = [arg for arg in required_args if not any(arg in s for s in args)]
+        return missing_args
+
+    @staticmethod
+    def __get_required_args_from_parser(parser: argparse.ArgumentParser) -> List[str]:
+        required_args = []
+        for action in parser._actions:
+            if action.required:
+                # Prefix the argument with '--' if it's a long argument, or '-' if it's short
+                prefix = "--" if len(action.dest) > 1 else "-"
+                required_args.append(prefix + action.dest)
+        return required_args
+
 
 T = TypeVar("T", bound="DefaultConfig")
 
 
 class DefaultConfig(config):
     """
     A Config with a set of default values.
```

### Comparing `bittensor-6.9.3/bittensor/dendrite.py` & `bittensor-7.0.0/bittensor/dendrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 # DEALINGS IN THE SOFTWARE.
 
 from __future__ import annotations
 
 import asyncio
 import uuid
 import time
-import torch
 import aiohttp
 import bittensor
-from typing import Union, Optional, List, Union, AsyncGenerator, Any
+from typing import Optional, List, Union, AsyncGenerator, Any
+from bittensor.utils.registration import torch, use_torch
 
 
-class dendrite(torch.nn.Module):
+class DendriteMixin:
     """
-    The Dendrite class, inheriting from PyTorch's Module class, represents the abstracted implementation of a network client module.
+    The Dendrite class represents the abstracted implementation of a network client module.
 
     In the brain analogy, dendrites receive signals
     from other neurons (in this case, network servers or axons), and the Dendrite class here is designed
     to send requests to those endpoint to recieve inputs.
 
     This class includes a wallet or keypair used for signing messages, and methods for making
     HTTP requests to the network servers. It also provides functionalities such as logging
@@ -101,15 +101,15 @@
         Initializes the Dendrite object, setting up essential properties.
 
         Args:
             wallet (Optional[Union['bittensor.wallet', 'bittensor.keypair']], optional):
                 The user's wallet or keypair used for signing messages. Defaults to ``None``, in which case a new :func:`bittensor.wallet().hotkey` is generated and used.
         """
         # Initialize the parent class
-        super(dendrite, self).__init__()
+        super(DendriteMixin, self).__init__()
 
         # Unique identifier for the instance
         self.uuid = str(uuid.uuid1())
 
         # Get the external IP
         self.external_ip = bittensor.utils.networking.get_external_ip()
 
@@ -440,23 +440,23 @@
                     data chunks. In non-streaming mode, a Synapse or StreamingSynapse object is returned
                     containing the response.
                 """
                 if is_stream:
                     # If in streaming mode, return the async_generator
                     return self.call_stream(
                         target_axon=target_axon,
-                        synapse=synapse.copy(),  # type: ignore
+                        synapse=synapse.model_copy(),  # type: ignore
                         timeout=timeout,
                         deserialize=deserialize,
                     )
                 else:
                     # If not in streaming mode, simply call the axon and get the response.
                     return await self.call(
                         target_axon=target_axon,
-                        synapse=synapse.copy(),  # type: ignore
+                        synapse=synapse.model_copy(),  # type: ignore
                         timeout=timeout,
                         deserialize=deserialize,
                     )
 
             # If run_async flag is False, get responses one by one.
             if not run_async:
                 return [
@@ -515,15 +515,15 @@
             # Log outgoing request
             self._log_outgoing_request(synapse)
 
             # Make the HTTP POST request
             async with (await self.session).post(
                 url,
                 headers=synapse.to_headers(),
-                json=synapse.dict(),
+                json=synapse.model_dump(),
                 timeout=timeout,
             ) as response:
                 # Extract the JSON response from the server
                 json_response = await response.json()
                 # Process the server response and fill synapse
                 self.process_server_response(response, json_response, synapse)
 
@@ -597,15 +597,15 @@
             # Log outgoing request
             self._log_outgoing_request(synapse)
 
             # Make the HTTP POST request
             async with (await self.session).post(
                 url,
                 headers=synapse.to_headers(),
-                json=synapse.dict(),
+                json=synapse.model_dump(),
                 timeout=timeout,
             ) as response:
                 # Use synapse subclass' process_streaming_response method to yield the response chunks
                 async for chunk in synapse.process_streaming_response(response):  # type: ignore
                     yield chunk  # Yield each chunk as it's processed
                 json_response = synapse.extract_response_json(response)
 
@@ -694,41 +694,41 @@
         Raises:
             None: But errors in attribute setting are silently ignored.
         """
         # Check if the server responded with a successful status code
         if server_response.status == 200:
             # If the response is successful, overwrite local synapse state with
             # server's state only if the protocol allows mutation. To prevent overwrites,
-            # the protocol must set allow_mutation = False
+            # the protocol must set Frozen = True
             server_synapse = local_synapse.__class__(**json_response)
-            for key in local_synapse.dict().keys():
+            for key in local_synapse.model_dump().keys():
                 try:
                     # Set the attribute in the local synapse from the corresponding
                     # attribute in the server synapse
                     setattr(local_synapse, key, getattr(server_synapse, key))
                 except:
                     # Ignore errors during attribute setting
                     pass
 
         # Extract server headers and overwrite None values in local synapse headers
         server_headers = bittensor.Synapse.from_headers(server_response.headers)  # type: ignore
 
         # Merge dendrite headers
         local_synapse.dendrite.__dict__.update(
             {
-                **local_synapse.dendrite.dict(exclude_none=True),  # type: ignore
-                **server_headers.dendrite.dict(exclude_none=True),  # type: ignore
+                **local_synapse.dendrite.model_dump(exclude_none=True),  # type: ignore
+                **server_headers.dendrite.model_dump(exclude_none=True),  # type: ignore
             }
         )
 
         # Merge axon headers
         local_synapse.axon.__dict__.update(
             {
-                **local_synapse.axon.dict(exclude_none=True),  # type: ignore
-                **server_headers.axon.dict(exclude_none=True),  # type: ignore
+                **local_synapse.axon.model_dump(exclude_none=True),  # type: ignore
+                **server_headers.axon.model_dump(exclude_none=True),  # type: ignore
             }
         )
 
         # Update the status code and status message of the dendrite to match the axon
         local_synapse.dendrite.status_code = local_synapse.axon.status_code  # type: ignore
         local_synapse.dendrite.status_message = local_synapse.axon.status_message  # type: ignore
 
@@ -802,7 +802,28 @@
         Usage::
 
             dendrite = Dendrite()
             # ... some operations ...
             del dendrite  # This will implicitly invoke the __del__ method and close the session.
         """
         self.close_session()
+
+
+# For back-compatibility with torch
+BaseModel: Union["torch.nn.Module", object] = torch.nn.Module if use_torch() else object
+
+
+class dendrite(DendriteMixin, BaseModel):  # type: ignore
+    def __init__(
+        self, wallet: Optional[Union[bittensor.wallet, bittensor.Keypair]] = None
+    ):
+        if use_torch():
+            torch.nn.Module.__init__(self)
+        DendriteMixin.__init__(self, wallet)
+
+
+if not use_torch():
+
+    async def call(self, *args, **kwargs):
+        return await self.forward(*args, **kwargs)
+
+    dendrite.__call__ = call
```

### Comparing `bittensor-6.9.3/bittensor/errors.py` & `bittensor-7.0.0/bittensor/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,20 @@
 
 class NominationError(ChainTransactionError):
     r"""Error raised when a nomination transaction fails."""
 
     pass
 
 
+class TakeError(ChainTransactionError):
+    r"""Error raised when a increase / decrease take transaction fails."""
+
+    pass
+
+
 class TransferError(ChainTransactionError):
     r"""Error raised when a transfer transaction fails."""
 
     pass
 
 
 class RegistrationError(ChainTransactionError):
```

### Comparing `bittensor-6.9.3/bittensor/extrinsics/__init__.py` & `bittensor-7.0.0/bittensor/extrinsics/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/extrinsics/delegation.py` & `bittensor-7.0.0/bittensor/extrinsics/delegation.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,23 +12,29 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
+import logging
 import bittensor
-from ..errors import *
+from ..errors import (
+    NominationError,
+    NotDelegateError,
+    NotRegisteredError,
+    StakeError,
+    TakeError,
+)
 from rich.prompt import Confirm
 from typing import Union, Optional
 from bittensor.utils.balance import Balance
+from bittensor.btlogging.defines import BITTENSOR_LOGGER_NAME
 
-from loguru import logger
-
-logger = logger.opt(colors=True)
+logger = logging.getLogger(BITTENSOR_LOGGER_NAME)
 
 
 def nominate_extrinsic(
     subtensor: "bittensor.subtensor",
     wallet: "bittensor.wallet",
     wait_for_finalization: bool = False,
     wait_for_inclusion: bool = True,
@@ -65,33 +71,33 @@
 
             if success == True:
                 bittensor.__console__.print(
                     ":white_heavy_check_mark: [green]Finalized[/green]"
                 )
                 bittensor.logging.success(
                     prefix="Become Delegate",
-                    sufix="<green>Finalized: </green>" + str(success),
+                    suffix="<green>Finalized: </green>" + str(success),
                 )
 
             # Raises NominationError if False
             return success
 
         except Exception as e:
             bittensor.__console__.print(
                 ":cross_mark: [red]Failed[/red]: error:{}".format(e)
             )
             bittensor.logging.warning(
-                prefix="Set weights", sufix="<red>Failed: </red>" + str(e)
+                prefix="Set weights", suffix="<red>Failed: </red>" + str(e)
             )
         except NominationError as e:
             bittensor.__console__.print(
                 ":cross_mark: [red]Failed[/red]: error:{}".format(e)
             )
             bittensor.logging.warning(
-                prefix="Set weights", sufix="<red>Failed: </red>" + str(e)
+                prefix="Set weights", suffix="<red>Failed: </red>" + str(e)
             )
 
     return False
 
 
 def delegate_extrinsic(
     subtensor: "bittensor.subtensor",
@@ -353,7 +359,134 @@
                 wallet.hotkey_str
             )
         )
         return False
     except StakeError as e:
         bittensor.__console__.print(":cross_mark: [red]Stake Error: {}[/red]".format(e))
         return False
+
+
+def decrease_take_extrinsic(
+    subtensor: "bittensor.subtensor",
+    wallet: "bittensor.wallet",
+    hotkey_ss58: Optional[str] = None,
+    take: int = 0,
+    wait_for_finalization: bool = False,
+    wait_for_inclusion: bool = True,
+) -> bool:
+    r"""Decrease delegate take for the hotkey.
+
+    Args:
+        wallet (bittensor.wallet):
+            Bittensor wallet object.
+        hotkey_ss58 (Optional[str]):
+            The ``ss58`` address of the hotkey account to stake to defaults to the wallet's hotkey.
+        take (float):
+            The ``take`` of the hotkey.
+    Returns:
+        success (bool): ``True`` if the transaction was successful.
+    """
+    # Unlock the coldkey.
+    wallet.coldkey
+    wallet.hotkey
+
+    with bittensor.__console__.status(
+        ":satellite: Sending decrease_take_extrinsic call on [white]{}[/white] ...".format(
+            subtensor.network
+        )
+    ):
+        try:
+            success = subtensor._do_decrease_take(
+                wallet=wallet,
+                hotkey_ss58=hotkey_ss58,
+                take=take,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+
+            if success == True:
+                bittensor.__console__.print(
+                    ":white_heavy_check_mark: [green]Finalized[/green]"
+                )
+                bittensor.logging.success(
+                    prefix="Decrease Delegate Take",
+                    sufix="<green>Finalized: </green>" + str(success),
+                )
+
+            return success
+
+        except (TakeError, Exception) as e:
+            bittensor.__console__.print(
+                ":cross_mark: [red]Failed[/red]: error:{}".format(e)
+            )
+            bittensor.logging.warning(
+                prefix="Set weights", sufix="<red>Failed: </red>" + str(e)
+            )
+
+    return False
+
+
+def increase_take_extrinsic(
+    subtensor: "bittensor.subtensor",
+    wallet: "bittensor.wallet",
+    hotkey_ss58: Optional[str] = None,
+    take: int = 0,
+    wait_for_finalization: bool = False,
+    wait_for_inclusion: bool = True,
+) -> bool:
+    r"""Increase delegate take for the hotkey.
+
+    Args:
+        wallet (bittensor.wallet):
+            Bittensor wallet object.
+        hotkey_ss58 (Optional[str]):
+            The ``ss58`` address of the hotkey account to stake to defaults to the wallet's hotkey.
+        take (float):
+            The ``take`` of the hotkey.
+    Returns:
+        success (bool): ``True`` if the transaction was successful.
+    """
+    # Unlock the coldkey.
+    wallet.coldkey
+    wallet.hotkey
+
+    with bittensor.__console__.status(
+        ":satellite: Sending increase_take_extrinsic call on [white]{}[/white] ...".format(
+            subtensor.network
+        )
+    ):
+        try:
+            success = subtensor._do_increase_take(
+                wallet=wallet,
+                hotkey_ss58=hotkey_ss58,
+                take=take,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+
+            if success == True:
+                bittensor.__console__.print(
+                    ":white_heavy_check_mark: [green]Finalized[/green]"
+                )
+                bittensor.logging.success(
+                    prefix="Increase Delegate Take",
+                    sufix="<green>Finalized: </green>" + str(success),
+                )
+
+            return success
+
+        except Exception as e:
+            bittensor.__console__.print(
+                ":cross_mark: [red]Failed[/red]: error:{}".format(e)
+            )
+            bittensor.logging.warning(
+                prefix="Set weights", sufix="<red>Failed: </red>" + str(e)
+            )
+        except TakeError as e:
+            bittensor.__console__.print(
+                ":cross_mark: [red]Failed[/red]: error:{}".format(e)
+            )
+            bittensor.logging.warning(
+                prefix="Set weights", sufix="<red>Failed: </red>" + str(e)
+            )
+
+    return False
```

### Comparing `bittensor-6.9.3/bittensor/extrinsics/network.py` & `bittensor-7.0.0/bittensor/extrinsics/network.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/extrinsics/prometheus.py` & `bittensor-7.0.0/bittensor/extrinsics/prometheus.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             external_ip = net.get_external_ip()
             bittensor.__console__.print(
                 ":white_heavy_check_mark: [green]Found external ip: {}[/green]".format(
                     external_ip
                 )
             )
             bittensor.logging.success(
-                prefix="External IP", sufix="<blue>{}</blue>".format(external_ip)
+                prefix="External IP", suffix="<blue>{}</blue>".format(external_ip)
             )
         except Exception as E:
             raise RuntimeError(
                 "Unable to attain your external ip. Check your internet connection. error: {}".format(
                     E
                 )
             ) from E
```

### Comparing `bittensor-6.9.3/bittensor/extrinsics/registration.py` & `bittensor-7.0.0/bittensor/extrinsics/registration.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import bittensor
-
-import torch
 import time
 from rich.prompt import Confirm
 from typing import List, Union, Optional, Tuple
-from bittensor.utils.registration import POWSolution, create_pow
+from bittensor.utils.registration import (
+    POWSolution,
+    create_pow,
+    torch,
+    log_no_torch_error,
+)
 
 
 def register_extrinsic(
     subtensor: "bittensor.subtensor",
     wallet: "bittensor.wallet",
     netuid: int,
     wait_for_inclusion: bool = False,
@@ -98,25 +101,29 @@
                 wallet.hotkey.ss58_address,
                 wallet.coldkeypub.ss58_address,
                 subtensor.network,
             )
         ):
             return False
 
+    if not torch:
+        log_no_torch_error()
+        return False
+
     # Attempt rolling registration.
     attempts = 1
     while True:
         bittensor.__console__.print(
             ":satellite: Registering...({}/{})".format(attempts, max_allowed_attempts)
         )
         # Solve latest POW.
         if cuda:
             if not torch.cuda.is_available():
                 if prompt:
-                    bittensor.__console__.error("CUDA is not available.")
+                    bittensor.__console__.print("CUDA is not available.")
                 return False
             pow_result: Optional[POWSolution] = create_pow(
                 subtensor,
                 wallet,
                 netuid,
                 output_in_place,
                 cuda=cuda,
@@ -284,15 +291,15 @@
         )
 
         if success != True or success == False:
             bittensor.__console__.print(
                 ":cross_mark: [red]Failed[/red]: error:{}".format(err_msg)
             )
             time.sleep(0.5)
-
+            return False
         # Successful registration, final check for neuron and pubkey
         else:
             bittensor.__console__.print(":satellite: Checking Balance...")
             block = subtensor.get_current_block()
             new_balance = subtensor.get_balance(
                 wallet.coldkeypub.ss58_address, block=block
             )
@@ -311,14 +318,15 @@
                 )
                 return True
             else:
                 # neuron not found, try again
                 bittensor.__console__.print(
                     ":cross_mark: [red]Unknown error. Neuron not found.[/red]"
                 )
+                return False
 
 
 class MaxSuccessException(Exception):
     pass
 
 
 class MaxAttemptsException(Exception):
@@ -335,15 +343,15 @@
     output_in_place: bool = True,
     cuda: bool = False,
     dev_id: Union[List[int], int] = 0,
     tpb: int = 256,
     num_processes: Optional[int] = None,
     update_interval: Optional[int] = None,
     log_verbose: bool = False,
-) -> bool:
+) -> Tuple[bool, str]:
     r"""Runs a continual POW to get a faucet of TAO on the test net.
 
     Args:
         wallet (bittensor.wallet):
             Bittensor wallet object.
         prompt (bool):
             If ``true``, the call waits for confirmation from the user before proceeding.
@@ -372,35 +380,39 @@
     if prompt:
         if not Confirm.ask(
             "Run Faucet ?\n coldkey:    [bold white]{}[/bold white]\n network:    [bold white]{}[/bold white]".format(
                 wallet.coldkeypub.ss58_address,
                 subtensor.network,
             )
         ):
-            return False
+            return False, ""
+
+    if not torch:
+        log_no_torch_error()
+        return False, "Requires torch"
 
     # Unlock coldkey
     wallet.coldkey
 
     # Get previous balance.
     old_balance = subtensor.get_balance(wallet.coldkeypub.ss58_address)
 
     # Attempt rolling registration.
     attempts = 1
     successes = 1
     while True:
         try:
             pow_result = None
-            while pow_result == None or pow_result.is_stale(subtensor=subtensor):
+            while pow_result is None or pow_result.is_stale(subtensor=subtensor):
                 # Solve latest POW.
                 if cuda:
                     if not torch.cuda.is_available():
                         if prompt:
-                            bittensor.__console__.error("CUDA is not available.")
-                        return False
+                            bittensor.__console__.print("CUDA is not available.")
+                        return False, "CUDA is not available."
                     pow_result: Optional[POWSolution] = create_pow(
                         subtensor,
                         wallet,
                         -1,
                         output_in_place,
                         cuda=cuda,
                         dev_id=dev_id,
@@ -495,12 +507,14 @@
         )
 
         if success != True or success == False:
             bittensor.__console__.print(
                 ":cross_mark: [red]Failed[/red]: error:{}".format(err_msg)
             )
             time.sleep(0.5)
+            return False
 
         else:
             bittensor.__console__.print(
                 f"Hotkey {wallet.hotkey} swapped for new hotkey: {new_wallet.hotkey}"
             )
+            return True
```

### Comparing `bittensor-6.9.3/bittensor/extrinsics/root.py` & `bittensor-7.0.0/bittensor/extrinsics/root.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import bittensor
 
 import time
-import torch
+import logging
+import numpy as np
+from numpy.typing import NDArray
 from rich.prompt import Confirm
-from typing import Union
+from typing import Union, List
 import bittensor.utils.weight_utils as weight_utils
+from bittensor.btlogging.defines import BITTENSOR_LOGGER_NAME
+from bittensor.utils.registration import torch, legacy_torch_api_compat
 
-from loguru import logger
-
-logger = logger.opt(colors=True)
+logger = logging.getLogger(BITTENSOR_LOGGER_NAME)
 
 
 def root_register_extrinsic(
     subtensor: "bittensor.subtensor",
     wallet: "bittensor.wallet",
     wait_for_inclusion: bool = False,
     wait_for_finalization: bool = True,
@@ -94,63 +96,65 @@
             else:
                 # neuron not found, try again
                 bittensor.__console__.print(
                     ":cross_mark: [red]Unknown error. Neuron not found.[/red]"
                 )
 
 
+@legacy_torch_api_compat
 def set_root_weights_extrinsic(
     subtensor: "bittensor.subtensor",
     wallet: "bittensor.wallet",
-    netuids: Union[torch.LongTensor, list],
-    weights: Union[torch.FloatTensor, list],
+    netuids: Union[NDArray[np.int64], "torch.LongTensor", List[int]],
+    weights: Union[NDArray[np.float32], "torch.FloatTensor", List[float]],
     version_key: int = 0,
     wait_for_inclusion: bool = False,
     wait_for_finalization: bool = False,
     prompt: bool = False,
 ) -> bool:
     r"""Sets the given weights and values on chain for wallet hotkey account.
 
     Args:
         wallet (bittensor.wallet):
             Bittensor wallet object.
-        netuids (List[int]):
+        netuids (Union[NDArray[np.int64], torch.LongTensor, List[int]]):
             The ``netuid`` of the subnet to set weights for.
-        weights ( Union[torch.FloatTensor, list]):
+        weights (Union[NDArray[np.float32], torch.FloatTensor, list]):
             Weights to set. These must be ``float`` s and must correspond to the passed ``netuid`` s.
         version_key (int):
             The version key of the validator.
         wait_for_inclusion (bool):
             If set, waits for the extrinsic to enter a block before returning ``true``, or returns ``false`` if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             If set, waits for the extrinsic to be finalized on the chain before returning ``true``, or returns ``false`` if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If ``true``, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
             Flag is ``true`` if extrinsic was finalized or uncluded in the block. If we did not wait for finalization / inclusion, the response is ``true``.
     """
+
     # First convert types.
     if isinstance(netuids, list):
-        netuids = torch.tensor(netuids, dtype=torch.int64)
+        netuids = np.array(netuids, dtype=np.int64)
     if isinstance(weights, list):
-        weights = torch.tensor(weights, dtype=torch.float32)
+        weights = np.array(weights, dtype=np.float32)
 
     # Get weight restrictions.
     min_allowed_weights = subtensor.min_allowed_weights(netuid=0)
     max_weight_limit = subtensor.max_weight_limit(netuid=0)
 
     # Get non zero values.
-    non_zero_weight_idx = torch.argwhere(weights > 0).squeeze(dim=1)
+    non_zero_weight_idx = np.argwhere(weights > 0).squeeze(axis=1)
     non_zero_weight_uids = netuids[non_zero_weight_idx]
     non_zero_weights = weights[non_zero_weight_idx]
-    if non_zero_weights.numel() < min_allowed_weights:
+    if non_zero_weights.size < min_allowed_weights:
         raise ValueError(
             "The minimum number of weights required to set weights is {}, got {}".format(
-                min_allowed_weights, non_zero_weights.numel()
+                min_allowed_weights, non_zero_weights.size
             )
         )
 
     # Normalize the weights to max value.
     formatted_weights = bittensor.utils.weight_utils.normalize_max_weight(
         x=weights, limit=max_weight_limit
     )
@@ -187,35 +191,35 @@
             )
 
             bittensor.__console__.print(success, error_message)
 
             if not wait_for_finalization and not wait_for_inclusion:
                 return True
 
-            if success == True:
+            if success is True:
                 bittensor.__console__.print(
                     ":white_heavy_check_mark: [green]Finalized[/green]"
                 )
                 bittensor.logging.success(
                     prefix="Set weights",
-                    sufix="<green>Finalized: </green>" + str(success),
+                    suffix="<green>Finalized: </green>" + str(success),
                 )
                 return True
             else:
                 bittensor.__console__.print(
                     ":cross_mark: [red]Failed[/red]: error:{}".format(error_message)
                 )
                 bittensor.logging.warning(
                     prefix="Set weights",
-                    sufix="<red>Failed: </red>" + str(error_message),
+                    suffix="<red>Failed: </red>" + str(error_message),
                 )
                 return False
 
         except Exception as e:
-            # TODO( devs ): lets remove all of the bittensor.__console__ calls and replace with loguru.
+            # TODO( devs ): lets remove all of the bittensor.__console__ calls and replace with the bittensor logger.
             bittensor.__console__.print(
                 ":cross_mark: [red]Failed[/red]: error:{}".format(e)
             )
             bittensor.logging.warning(
-                prefix="Set weights", sufix="<red>Failed: </red>" + str(e)
+                prefix="Set weights", suffix="<red>Failed: </red>" + str(e)
             )
             return False
```

### Comparing `bittensor-6.9.3/bittensor/extrinsics/senate.py` & `bittensor-7.0.0/bittensor/extrinsics/senate.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     proposal_hash: str,
     proposal_idx: int,
     vote: bool,
     wait_for_inclusion: bool = False,
     wait_for_finalization: bool = True,
     prompt: bool = False,
 ) -> bool:
-    r"""Removes the wallet from chain for senate voting.
+    r"""Votes ayes or nays on proposals.
 
     Args:
         wallet (bittensor.wallet):
             Bittensor wallet object.
         wait_for_inclusion (bool):
             If set, waits for the extrinsic to enter a block before returning ``true``, or returns ``false`` if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
```

### Comparing `bittensor-6.9.3/bittensor/extrinsics/serving.py` & `bittensor-7.0.0/bittensor/extrinsics/serving.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             external_ip = net.get_external_ip()
             bittensor.__console__.print(
                 ":white_heavy_check_mark: [green]Found external ip: {}[/green]".format(
                     external_ip
                 )
             )
             bittensor.logging.success(
-                prefix="External IP", sufix="<blue>{}</blue>".format(external_ip)
+                prefix="External IP", suffix="<blue>{}</blue>".format(external_ip)
             )
         except Exception as E:
             raise RuntimeError(
                 "Unable to attain your external ip. Check your internet connection. error: {}".format(
                     E
                 )
             ) from E
```

### Comparing `bittensor-6.9.3/bittensor/extrinsics/set_weights.py` & `bittensor-7.0.0/bittensor/extrinsics/set_weights.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,66 +14,73 @@
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import bittensor
 
-import torch
+import logging
+import numpy as np
+from numpy.typing import NDArray
 from rich.prompt import Confirm
 from typing import Union, Tuple
 import bittensor.utils.weight_utils as weight_utils
+from bittensor.btlogging.defines import BITTENSOR_LOGGER_NAME
+from bittensor.utils.registration import torch, use_torch
 
-from loguru import logger
-
-logger = logger.opt(colors=True)
+logger = logging.getLogger(BITTENSOR_LOGGER_NAME)
 
 
 def set_weights_extrinsic(
     subtensor: "bittensor.subtensor",
     wallet: "bittensor.wallet",
     netuid: int,
-    uids: Union[torch.LongTensor, list],
-    weights: Union[torch.FloatTensor, list],
+    uids: Union[NDArray[np.int64], "torch.LongTensor", list],
+    weights: Union[NDArray[np.float32], "torch.FloatTensor", list],
     version_key: int = 0,
     wait_for_inclusion: bool = False,
     wait_for_finalization: bool = False,
     prompt: bool = False,
 ) -> Tuple[bool, str]:
     r"""Sets the given weights and values on chain for wallet hotkey account.
 
     Args:
         subtensor_endpoint (bittensor.subtensor):
             Subtensor endpoint to use.
         wallet (bittensor.wallet):
             Bittensor wallet object.
         netuid (int):
             The ``netuid`` of the subnet to set weights for.
-        uids (Union[torch.LongTensor, list]):
+        uids (Union[NDArray[np.int64], torch.LongTensor, list]):
             The ``uint64`` uids of destination neurons.
-        weights ( Union[torch.FloatTensor, list]):
+        weights (Union[NDArray[np.float32], torch.FloatTensor, list]):
             The weights to set. These must be ``float`` s and correspond to the passed ``uid`` s.
         version_key (int):
             The version key of the validator.
         wait_for_inclusion (bool):
             If set, waits for the extrinsic to enter a block before returning ``true``, or returns ``false`` if the extrinsic fails to enter the block within the timeout.
         wait_for_finalization (bool):
             If set, waits for the extrinsic to be finalized on the chain before returning ``true``, or returns ``false`` if the extrinsic fails to be finalized within the timeout.
         prompt (bool):
             If ``true``, the call waits for confirmation from the user before proceeding.
     Returns:
         success (bool):
             Flag is ``true`` if extrinsic was finalized or uncluded in the block. If we did not wait for finalization / inclusion, the response is ``true``.
     """
-
     # First convert types.
-    if isinstance(uids, list):
-        uids = torch.tensor(uids, dtype=torch.int64)
-    if isinstance(weights, list):
-        weights = torch.tensor(weights, dtype=torch.float32)
+    if use_torch():
+        if isinstance(uids, list):
+            uids = torch.tensor(uids, dtype=torch.int64)
+        if isinstance(weights, list):
+            weights = torch.tensor(weights, dtype=torch.float32)
+    else:
+        if isinstance(uids, list):
+            uids = np.array(uids, dtype=np.int64)
+        if isinstance(weights, list):
+            weights = np.array(weights, dtype=np.float32)
 
     # Reformat and normalize.
     weight_uids, weight_vals = weight_utils.convert_weights_and_uids_for_emit(
         uids, weights
     )
 
     # Ask before moving on.
@@ -104,29 +111,28 @@
 
             if success == True:
                 bittensor.__console__.print(
                     ":white_heavy_check_mark: [green]Finalized[/green]"
                 )
                 bittensor.logging.success(
                     prefix="Set weights",
-                    sufix="<green>Finalized: </green>" + str(success),
+                    suffix="<green>Finalized: </green>" + str(success),
                 )
                 return True, "Successfully set weights and Finalized."
             else:
                 bittensor.__console__.print(
                     ":cross_mark: [red]Failed[/red]: error:{}".format(error_message)
                 )
                 bittensor.logging.warning(
                     prefix="Set weights",
-                    sufix="<red>Failed: </red>" + str(error_message),
+                    suffix="<red>Failed: </red>" + str(error_message),
                 )
                 return False, error_message
 
         except Exception as e:
-            # TODO( devs ): lets remove all of the bittensor.__console__ calls and replace with loguru.
             bittensor.__console__.print(
                 ":cross_mark: [red]Failed[/red]: error:{}".format(e)
             )
             bittensor.logging.warning(
-                prefix="Set weights", sufix="<red>Failed: </red>" + str(e)
+                prefix="Set weights", suffix="<red>Failed: </red>" + str(e)
             )
             return False, str(e)
```

### Comparing `bittensor-6.9.3/bittensor/extrinsics/staking.py` & `bittensor-7.0.0/bittensor/extrinsics/staking.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/extrinsics/transfer.py` & `bittensor-7.0.0/bittensor/extrinsics/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/extrinsics/unstaking.py` & `bittensor-7.0.0/bittensor/extrinsics/unstaking.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,40 @@
         wait_for_inclusion=wait_for_inclusion,
         wait_for_finalization=wait_for_finalization,
     )
 
     return success
 
 
+def check_threshold_amount(
+    subtensor: "bittensor.subtensor", unstaking_balance: Balance
+) -> bool:
+    """
+    Checks if the unstaking amount is above the threshold or 0
+
+    Args:
+        unstaking_balance (Balance):
+            the balance to check for threshold limits.
+
+    Returns:
+        success (bool):
+            ``true`` if the unstaking is above the threshold or 0, or ``false`` if the
+                unstaking is below the threshold, but not 0.
+    """
+    min_req_stake: Balance = subtensor.get_minimum_required_stake()
+
+    if min_req_stake > unstaking_balance > 0:
+        bittensor.__console__.print(
+            f":cross_mark: [red]Unstaking balance of {unstaking_balance} less than minimum of {min_req_stake} TAO[/red]"
+        )
+        return False
+    else:
+        return True
+
+
 def unstake_extrinsic(
     subtensor: "bittensor.subtensor",
     wallet: "bittensor.wallet",
     hotkey_ss58: Optional[str] = None,
     amount: Optional[Union[Balance, float]] = None,
     wait_for_inclusion: bool = True,
     wait_for_finalization: bool = False,
@@ -130,14 +156,19 @@
         bittensor.__console__.print(
             ":cross_mark: [red]Not enough stake[/red]: [green]{}[/green] to unstake: [blue]{}[/blue] from hotkey: [white]{}[/white]".format(
                 stake_on_uid, unstaking_balance, wallet.hotkey_str
             )
         )
         return False
 
+    if not check_threshold_amount(
+        subtensor=subtensor, unstaking_balance=unstaking_balance
+    ):
+        return False
+
     # Ask before moving on.
     if prompt:
         if not Confirm.ask(
             "Do you want to unstake:\n[bold white]  amount: {}\n  hotkey: {}[/bold white ]?".format(
                 unstaking_balance, wallet.hotkey_str
             )
         ):
@@ -301,14 +332,19 @@
             bittensor.__console__.print(
                 ":cross_mark: [red]Not enough stake[/red]: [green]{}[/green] to unstake: [blue]{}[/blue] from hotkey: [white]{}[/white]".format(
                     stake_on_uid, unstaking_balance, wallet.hotkey_str
                 )
             )
             continue
 
+        if not check_threshold_amount(
+            subtensor=subtensor, unstaking_balance=unstaking_balance
+        ):
+            return False
+
         # Ask before moving on.
         if prompt:
             if not Confirm.ask(
                 "Do you want to unstake:\n[bold white]  amount: {}\n  hotkey: {}[/bold white ]?".format(
                     unstaking_balance, wallet.hotkey_str
                 )
             ):
```

### Comparing `bittensor-6.9.3/bittensor/keyfile.py` & `bittensor-7.0.0/bittensor/keyfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         keypair (bittensor.Keypair): The keypair object to be serialized.
     Returns:
         data (bytes): Serialized keypair data.
     """
     json_data = {
         "accountId": "0x" + keypair.public_key.hex() if keypair.public_key else None,
         "publicKey": "0x" + keypair.public_key.hex() if keypair.public_key else None,
+        "privateKey": "0x" + keypair.private_key.hex() if keypair.private_key else None,
         "secretPhrase": keypair.mnemonic if keypair.mnemonic else None,
         "secretSeed": (
             "0x"
             + (
                 keypair.seed_hex
                 if isinstance(keypair.seed_hex, str)
                 else keypair.seed_hex.hex()
@@ -86,33 +87,40 @@
     except:
         string_value = str(keyfile_data)
         if string_value[:2] == "0x":
             string_value = ss58_encode(string_value)
             keyfile_dict = {
                 "accountId": None,
                 "publicKey": None,
+                "privateKey": None,
                 "secretPhrase": None,
                 "secretSeed": None,
                 "ss58Address": string_value,
             }
         else:
             raise bittensor.KeyFileError(
                 "Keypair could not be created from keyfile data: {}".format(
                     string_value
                 )
             )
 
     if "secretSeed" in keyfile_dict and keyfile_dict["secretSeed"] is not None:
         return bittensor.Keypair.create_from_seed(keyfile_dict["secretSeed"])
 
-    if "secretPhrase" in keyfile_dict and keyfile_dict["secretPhrase"] is not None:
+    elif "secretPhrase" in keyfile_dict and keyfile_dict["secretPhrase"] is not None:
         return bittensor.Keypair.create_from_mnemonic(
             mnemonic=keyfile_dict["secretPhrase"]
         )
 
+    elif keyfile_dict.get("privateKey", None) is not None:
+        # May have the above dict keys also, but we want to preserve the first two
+        return bittensor.Keypair.create_from_private_key(
+            keyfile_dict["privateKey"], ss58_format=bittensor.__ss58_format__
+        )
+
     if "ss58Address" in keyfile_dict and keyfile_dict["ss58Address"] is not None:
         return bittensor.Keypair(ss58_address=keyfile_dict["ss58Address"])
 
     else:
         raise bittensor.KeyFileError(
             "Keypair could not be created from keyfile data: {}".format(keyfile_dict)
         )
@@ -264,21 +272,20 @@
     """Retrieves the cold key password from the environment variables.
 
     Args:
         coldkey_name (str): The name of the cold key.
     Returns:
         password (str): The password retrieved from the environment variables, or ``None`` if not found.
     """
-    for env_var in os.environ:
-        if env_var.upper().startswith("BT_COLD_PW_") and env_var.upper().endswith(
-            coldkey_name.upper()
-        ):
-            return os.getenv(env_var)
-
-    return None
+    envs = {
+        normalized_env_name: env_value
+        for env_name, env_value in os.environ.items()
+        if (normalized_env_name := env_name.upper()).startswith("BT_COLD_PW_")
+    }
+    return envs.get(f"BT_COLD_PW_{coldkey_name.upper()}")
 
 
 def decrypt_keyfile_data(
     keyfile_data: bytes, password: str = None, coldkey_name: Optional[str] = None
 ) -> bytes:
     """Decrypts the passed keyfile data using ansible vault.
```

### Comparing `bittensor-6.9.3/bittensor/metagraph.py` & `bittensor-7.0.0/bittensor/metagraph.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,45 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
+from abc import ABC, abstractmethod
 import os
-import torch
+import pickle
+import numpy as np
+from numpy.typing import NDArray
 import bittensor
 from os import listdir
 from os.path import join
-from typing import List, Optional
+from typing import List, Optional, Union, Tuple
 
 from bittensor.chain_data import AxonInfo
+from bittensor.utils.registration import torch, use_torch
+
+METAGRAPH_STATE_DICT_NDARRAY_KEYS = [
+    "version",
+    "n",
+    "block",
+    "stake",
+    "total_stake",
+    "ranks",
+    "trust",
+    "consensus",
+    "validator_trust",
+    "incentive",
+    "emission",
+    "dividends",
+    "active",
+    "last_update",
+    "validator_permit",
+    "uids",
+]
 
 
 def get_save_dir(network: str, netuid: int) -> str:
     """
     Return directory path from ``network`` and ``netuid``.
 
     Args:
@@ -66,30 +89,30 @@
             pass
     if not latest_file_full_path:
         raise ValueError(f"Metagraph not found at: {dir_path}")
     else:
         return latest_file_full_path
 
 
-class metagraph(torch.nn.Module):
+class MetagraphMixin(ABC):
     """
     The metagraph class is a core component of the Bittensor network, representing the neural graph that forms the backbone of the decentralized machine learning system.
 
     The metagraph is a dynamic representation of the network's state, capturing the interconnectedness and attributes of neurons (participants) in the Bittensor ecosystem. This class is not just a static structure but a live reflection of the network, constantly updated and synchronized with the state of the blockchain.
 
     In Bittensor, neurons are akin to nodes in a distributed system, each contributing computational resources and participating in the network's collective intelligence. The metagraph tracks various attributes of these neurons, such as stake, trust, and consensus, which are crucial for the network's incentive mechanisms and the Yuma Consensus algorithm as outlined in the `NeurIPS paper <https://bittensor.com/pdfs/academia/NeurIPS_DAO_Workshop_2022_3_3.pdf>`_. These attributes
     govern how neurons interact, how they are incentivized, and their roles within the network's
     decision-making processes.
 
     Args:
         netuid (int): A unique identifier that distinguishes between different instances or versions of the Bittensor network.
         network (str): The name of the network, signifying specific configurations or iterations within the Bittensor ecosystem.
-        version (torch.nn.parameter.Parameter): The version number of the network, formatted for compatibility with PyTorch models, integral for tracking network updates.
-        n (torch.nn.Parameter): The total number of neurons in the network, reflecting its size and complexity.
-        block (torch.nn.Parameter): The current block number in the blockchain, crucial for synchronizing with the network's latest state.
+        version (NDArray): The version number of the network, integral for tracking network updates.
+        n (NDArray): The total number of neurons in the network, reflecting its size and complexity.
+        block (NDArray): The current block number in the blockchain, crucial for synchronizing with the network's latest state.
         stake: Represents the cryptocurrency staked by neurons, impacting their influence and earnings within the network.
         total_stake: The cumulative stake across all neurons.
         ranks: Neuron rankings as per the Yuma Consensus algorithm, influencing their incentive distribution and network authority.
         trust: Scores indicating the reliability of neurons, mainly miners, within the network's operational context.
         consensus: Scores reflecting each neuron's alignment with the network's collective decisions.
         validator_trust: Trust scores for validator neurons, crucial for network security and validation.
         incentive: Rewards allocated to neurons, particularly miners, for their network contributions.
@@ -123,153 +146,175 @@
             ...
 
         Maintaining a local copy of hotkeys for querying and interacting with network entities::
 
             hotkeys = deepcopy(metagraph.hotkeys)
     """
 
+    netuid: int
+    network: str
+    version: Union["torch.nn.Parameter", Tuple[NDArray]]
+    n: Union["torch.nn.Parameter", NDArray]
+    block: Union["torch.nn.Parameter", NDArray]
+    stake: Union["torch.nn.Parameter", NDArray]
+    total_stake: Union["torch.nn.Parameter", NDArray]
+    ranks: Union["torch.nn.Parameter", NDArray]
+    trust: Union["torch.nn.Parameter", NDArray]
+    consensus: Union["torch.nn.Parameter", NDArray]
+    validator_trust: Union["torch.nn.Parameter", NDArray]
+    incentive: Union["torch.nn.Parameter", NDArray]
+    emission: Union["torch.nn.Parameter", NDArray]
+    dividends: Union["torch.nn.Parameter", NDArray]
+    active: Union["torch.nn.Parameter", NDArray]
+    last_update: Union["torch.nn.Parameter", NDArray]
+    validator_permit: Union["torch.nn.Parameter", NDArray]
+    weights: Union["torch.nn.Parameter", NDArray]
+    bonds: Union["torch.nn.Parameter", NDArray]
+    uids: Union["torch.nn.Parameter", NDArray]
+    axons: List[AxonInfo]
+
     @property
-    def S(self) -> torch.nn.Parameter:
+    def S(self) -> Union[NDArray, "torch.nn.Parameter"]:
         """
         Represents the stake of each neuron in the Bittensor network. Stake is an important concept in the
         Bittensor ecosystem, signifying the amount of network weight (or “stake”) each neuron holds,
         represented on a digital ledger. The stake influences a neuron's ability to contribute to and benefit
         from the network, playing a crucial role in the distribution of incentives and decision-making processes.
 
         Returns:
-            torch.nn.Parameter: A tensor representing the stake of each neuron in the network. Higher values signify a greater stake held by the respective neuron.
+            NDArray: A tensor representing the stake of each neuron in the network. Higher values signify a greater stake held by the respective neuron.
         """
         return self.total_stake
 
     @property
-    def R(self) -> torch.nn.Parameter:
+    def R(self) -> Union[NDArray, "torch.nn.Parameter"]:
         """
         Contains the ranks of neurons in the Bittensor network. Ranks are determined by the network based
         on each neuron's performance and contributions. Higher ranks typically indicate a greater level of
         contribution or performance by a neuron. These ranks are crucial in determining the distribution of
         incentives within the network, with higher-ranked neurons receiving more incentive.
 
         Returns:
-            torch.nn.Parameter: A tensor where each element represents the rank of a neuron. Higher values indicate higher ranks within the network.
+            NDArray: A tensor where each element represents the rank of a neuron. Higher values indicate higher ranks within the network.
         """
         return self.ranks
 
     @property
-    def I(self) -> torch.nn.Parameter:
+    def I(self) -> Union[NDArray, "torch.nn.Parameter"]:
         """
         Incentive values of neurons represent the rewards they receive for their contributions to the network.
         The Bittensor network employs an incentive mechanism that rewards neurons based on their
         informational value, stake, and consensus with other peers. This ensures that the most valuable and
         trusted contributions are incentivized.
 
         Returns:
-            torch.nn.Parameter: A tensor of incentive values, indicating the rewards or benefits accrued by each neuron based on their contributions and network consensus.
+            NDArray: A tensor of incentive values, indicating the rewards or benefits accrued by each neuron based on their contributions and network consensus.
         """
         return self.incentive
 
     @property
-    def E(self) -> torch.nn.Parameter:
+    def E(self) -> Union[NDArray, "torch.nn.Parameter"]:
         """
         Denotes the emission values of neurons in the Bittensor network. Emissions refer to the distribution or
         release of rewards (often in the form of cryptocurrency) to neurons, typically based on their stake and
         performance. This mechanism is central to the network's incentive model, ensuring that active and
         contributing neurons are appropriately rewarded.
 
         Returns:
-            torch.nn.Parameter: A tensor where each element represents the emission value for a neuron, indicating the amount of reward distributed to that neuron.
+            NDArray: A tensor where each element represents the emission value for a neuron, indicating the amount of reward distributed to that neuron.
         """
         return self.emission
 
     @property
-    def C(self) -> torch.nn.Parameter:
+    def C(self) -> Union[NDArray, "torch.nn.Parameter"]:
         """
         Represents the consensus values of neurons in the Bittensor network. Consensus is a measure of how
         much a neuron's contributions are trusted and agreed upon by the majority of the network. It is
         calculated based on a staked weighted trust system, where the network leverages the collective
         judgment of all participating peers. Higher consensus values indicate that a neuron's contributions
         are more widely trusted and valued across the network.
 
         Returns:
-            torch.nn.Parameter: A tensor of consensus values, where each element reflects the level of trust and agreement a neuron has achieved within the network.
+            NDArray: A tensor of consensus values, where each element reflects the level of trust and agreement a neuron has achieved within the network.
 
         """
         return self.consensus
 
     @property
-    def T(self) -> torch.nn.Parameter:
+    def T(self) -> Union[NDArray, "torch.nn.Parameter"]:
         """
         Represents the trust values assigned to each neuron in the Bittensor network. Trust is a key metric that
         reflects the reliability and reputation of a neuron based on its past behavior and contributions. It is
         an essential aspect of the network's functioning, influencing decision-making processes and interactions
         between neurons.
 
         The trust matrix is inferred from the network's inter-peer weights, indicating the level of trust each neuron
         has in others. A higher value in the trust matrix suggests a stronger trust relationship between neurons.
 
         Returns:
-            torch.nn.Parameter: A tensor of trust values, where each element represents the trust level of a neuron. Higher values denote a higher level of trust within the network.
+            NDArray: A tensor of trust values, where each element represents the trust level of a neuron. Higher values denote a higher level of trust within the network.
         """
         return self.trust
 
     @property
-    def Tv(self) -> torch.nn.Parameter:
+    def Tv(self) -> Union[NDArray, "torch.nn.Parameter"]:
         """
         Contains the validator trust values of neurons in the Bittensor network. Validator trust is specifically
         associated with neurons that act as validators within the network. This specialized form of trust reflects
         the validators' reliability and integrity in their role, which is crucial for maintaining the network's
         stability and security.
 
         Validator trust values are particularly important for the network's consensus and validation processes,
         determining the validators' influence and responsibilities in these critical functions.
 
         Returns:
-            torch.nn.Parameter: A tensor of validator trust values, specifically applicable to neurons serving as validators, where higher values denote greater trustworthiness in their validation roles.
+            NDArray: A tensor of validator trust values, specifically applicable to neurons serving as validators, where higher values denote greater trustworthiness in their validation roles.
         """
         return self.validator_trust
 
     @property
-    def D(self) -> torch.nn.Parameter:
+    def D(self) -> Union[NDArray, "torch.nn.Parameter"]:
         """
         Represents the dividends received by neurons in the Bittensor network. Dividends are a form of reward or
         distribution, typically given to neurons based on their stake, performance, and contribution to the network.
         They are an integral part of the network's incentive structure, encouraging active and beneficial participation.
 
         Returns:
-            torch.nn.Parameter: A tensor of dividend values, where each element indicates the dividends received by a neuron, reflecting their share of network rewards.
+            NDArray: A tensor of dividend values, where each element indicates the dividends received by a neuron, reflecting their share of network rewards.
         """
         return self.dividends
 
     @property
-    def B(self) -> torch.nn.Parameter:
+    def B(self) -> Union[NDArray, "torch.nn.Parameter"]:
         """
         Bonds in the Bittensor network represent a speculative reward mechanism where neurons can accumulate
         bonds in other neurons. Bonds are akin to investments or stakes in other neurons, reflecting a belief in
         their future value or performance. This mechanism encourages correct weighting and collaboration
         among neurons while providing an additional layer of incentive.
 
         Returns:
-            torch.nn.Parameter: A tensor representing the bonds held by each neuron, where each value signifies the proportion of bonds owned by one neuron in another.
+            NDArray: A tensor representing the bonds held by each neuron, where each value signifies the proportion of bonds owned by one neuron in another.
         """
         return self.bonds
 
     @property
-    def W(self) -> torch.nn.Parameter:
+    def W(self) -> Union[NDArray, "torch.nn.Parameter"]:
         """
         Represents the weights assigned to each neuron in the Bittensor network. In the context of Bittensor,
         weights are crucial for determining the influence and interaction between neurons. Each neuron is responsible
         for setting its weights, which are then recorded on a digital ledger. These weights are reflective of the
         neuron's assessment or judgment of other neurons in the network.
 
         The weight matrix :math:`W = [w_{ij}]` is a key component of the network's architecture, where the :math:`i^{th}` row is set by
         neuron :math:`i` and represents its weights towards other neurons. These weights influence the ranking and incentive
         mechanisms within the network. Higher weights from a neuron towards another can imply greater trust or value
         placed on that neuron's contributions.
 
         Returns:
-            torch.nn.Parameter: A tensor of inter-peer weights, where each element :math:`w_{ij}` represents the weight assigned by neuron :math:`i` to neuron :math:`j`. This matrix is fundamental to the network's functioning, influencing the distribution of incentives and the inter-neuronal dynamics.
+            NDArray: A tensor of inter-peer weights, where each element :math:`w_{ij}` represents the weight assigned by neuron :math:`i` to neuron :math:`j`. This matrix is fundamental to the network's functioning, influencing the distribution of incentives and the inter-neuronal dynamics.
         """
         return self.weights
 
     @property
     def hotkeys(self) -> List[str]:
         """
         Represents a list of ``hotkeys`` for each neuron in the Bittensor network.
@@ -316,14 +361,33 @@
         Note:
             While IP addresses are a basic aspect of network communication, specific details about their use in
             the Bittensor network may not be covered in the `NeurIPS paper <https://bittensor.com/pdfs/academia/NeurIPS_DAO_Workshop_2022_3_3.pdf>`_. They are, however, integral to the
             functioning of any distributed network.
         """
         return [axon.ip_str() for axon in self.axons]
 
+    @abstractmethod
+    def __init__(
+        self, netuid: int, network: str = "finney", lite: bool = True, sync: bool = True
+    ):
+        """
+        Initializes a new instance of the metagraph object, setting up the basic structure and parameters based on the provided arguments.
+        This method is the entry point for creating a metagraph object,
+        which is a central component in representing the state of the Bittensor network.
+        Args:
+            netuid (int): The unique identifier for the network, distinguishing this instance of the metagraph within potentially multiple network configurations.
+            network (str): The name of the network, which can indicate specific configurations or versions of the Bittensor network.
+            lite (bool): A flag indicating whether to use a lite version of the metagraph. The lite version may contain less detailed information but can be quicker to initialize and sync.
+            sync (bool): A flag indicating whether to synchronize the metagraph with the network upon initialization. Synchronization involves updating the metagraph's parameters to reflect the current state of the network.
+        Example:
+            Initializing a metagraph object for the Bittensor network with a specific network UID::
+                metagraph = metagraph(netuid=123, network="finney", lite=True, sync=True)
+        """
+        pass
+
     def __str__(self) -> str:
         """
         Provides a human-readable string representation of the metagraph object. This representation includes key identifiers and attributes of the metagraph, making it easier to quickly understand
         the state and configuration of the metagraph in a simple format.
 
         Returns:
             str: A string that succinctly represents the metagraph, including its network UID, the total number of neurons (n), the current block number, and the network's name. This format is particularly useful for logging, debugging, and displaying the metagraph in a concise manner.
@@ -376,95 +440,38 @@
             "netuid": self.netuid,
             "n": self.n.item(),
             "block": self.block.item(),
             "network": self.network,
             "version": bittensor.__version__,
         }
 
-    def __init__(
-        self, netuid: int, network: str = "finney", lite: bool = True, sync: bool = True
-    ):
-        """
-        Initializes a new instance of the metagraph object, setting up the basic structure and parameters based on the provided arguments.
-
-        This method is the entry point for creating a metagraph object,
-        which is a central component in representing the state of the Bittensor network.
-
-        Args:
-            netuid (int): The unique identifier for the network, distinguishing this instance of the metagraph within potentially multiple network configurations.
-            network (str): The name of the network, which can indicate specific configurations or versions of the Bittensor network.
-            lite (bool): A flag indicating whether to use a lite version of the metagraph. The lite version may contain less detailed information but can be quicker to initialize and sync.
-            sync (bool): A flag indicating whether to synchronize the metagraph with the network upon initialization. Synchronization involves updating the metagraph's parameters to reflect the current state of the network.
-
-        Example:
-            Initializing a metagraph object for the Bittensor network with a specific network UID::
-
-                metagraph = metagraph(netuid=123, network="finney", lite=True, sync=True)
-        """
-        super(metagraph, self).__init__()
-        self.netuid = netuid
-        self.network = network
-        self.version = torch.nn.Parameter(
-            torch.tensor([bittensor.__version_as_int__], dtype=torch.int64),
-            requires_grad=False,
-        )
-        self.n: torch.nn.Parameter = torch.nn.Parameter(
-            torch.tensor([0], dtype=torch.int64), requires_grad=False
-        )
-        self.block: torch.nn.Parameter = torch.nn.Parameter(
-            torch.tensor([0], dtype=torch.int64), requires_grad=False
-        )
-        self.stake = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.float32), requires_grad=False
-        )
-        self.total_stake: torch.nn.Parameter = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.float32), requires_grad=False
-        )
-        self.ranks: torch.nn.Parameter = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.float32), requires_grad=False
-        )
-        self.trust: torch.nn.Parameter = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.float32), requires_grad=False
-        )
-        self.consensus: torch.nn.Parameter = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.float32), requires_grad=False
-        )
-        self.validator_trust: torch.nn.Parameter = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.float32), requires_grad=False
-        )
-        self.incentive: torch.nn.Parameter = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.float32), requires_grad=False
-        )
-        self.emission: torch.nn.Parameter = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.float32), requires_grad=False
-        )
-        self.dividends: torch.nn.Parameter = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.float32), requires_grad=False
-        )
-        self.active = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.int64), requires_grad=False
-        )
-        self.last_update = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.int64), requires_grad=False
-        )
-        self.validator_permit = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.bool), requires_grad=False
-        )
-        self.weights: torch.nn.Parameter = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.float32), requires_grad=False
-        )
-        self.bonds: torch.nn.Parameter = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.int64), requires_grad=False
-        )
-        self.uids = torch.nn.Parameter(
-            torch.tensor([], dtype=torch.int64), requires_grad=False
-        )
-        self.axons: List[AxonInfo] = []
-        if sync:
-            self.sync(block=None, lite=lite)
+    def state_dict(self):
+        return {
+            "netuid": self.netuid,
+            "network": self.network,
+            "version": self.version,
+            "n": self.n,
+            "block": self.block,
+            "stake": self.stake,
+            "total_stake": self.total_stake,
+            "ranks": self.ranks,
+            "trust": self.trust,
+            "consensus": self.consensus,
+            "validator_trust": self.validator_trust,
+            "incentive": self.incentive,
+            "emission": self.emission,
+            "dividends": self.dividends,
+            "active": self.active,
+            "last_update": self.last_update,
+            "validator_permit": self.validator_permit,
+            "weights": self.weights,
+            "bonds": self.bonds,
+            "uids": self.uids,
+            "axons": self.axons,
+        }
 
     def sync(
         self,
         block: Optional[int] = None,
         lite: bool = True,
         subtensor: Optional["bittensor.subtensor"] = None,
     ):
@@ -568,97 +575,37 @@
         # TODO: Check and test the conditions for assigning neurons
         if lite:
             self.neurons = subtensor.neurons_lite(block=block, netuid=self.netuid)
         else:
             self.neurons = subtensor.neurons(block=block, netuid=self.netuid)
         self.lite = lite
 
-    def _set_metagraph_attributes(self, block, subtensor):
-        """
-        Sets various attributes of the metagraph based on the latest network data fetched from the subtensor.
-
-        This method updates parameters like the number of neurons, block number, stakes, trusts, ranks, and other neuron-specific information.
-
-        Args:
-            block: The block number for which the metagraph attributes need to be set. If ``None``, the latest block data is used.
-            subtensor: The subtensor instance used for fetching the latest network data.
-
-        Internal Usage:
-            Used internally during the sync process to update the metagraph's attributes::
-
-                self._set_metagraph_attributes(block, subtensor)
-        """
-        # TODO: Check and test the setting of each attribute
-        self.n = self._create_tensor(len(self.neurons), dtype=torch.int64)
-        self.version = self._create_tensor(
-            [bittensor.__version_as_int__], dtype=torch.int64
-        )
-        self.block = self._create_tensor(
-            block if block else subtensor.block, dtype=torch.int64
-        )
-        self.uids = self._create_tensor(
-            [neuron.uid for neuron in self.neurons], dtype=torch.int64
-        )
-        self.trust = self._create_tensor(
-            [neuron.trust for neuron in self.neurons], dtype=torch.float32
-        )
-        self.consensus = self._create_tensor(
-            [neuron.consensus for neuron in self.neurons], dtype=torch.float32
-        )
-        self.incentive = self._create_tensor(
-            [neuron.incentive for neuron in self.neurons], dtype=torch.float32
-        )
-        self.dividends = self._create_tensor(
-            [neuron.dividends for neuron in self.neurons], dtype=torch.float32
-        )
-        self.ranks = self._create_tensor(
-            [neuron.rank for neuron in self.neurons], dtype=torch.float32
-        )
-        self.emission = self._create_tensor(
-            [neuron.emission for neuron in self.neurons], dtype=torch.float32
-        )
-        self.active = self._create_tensor(
-            [neuron.active for neuron in self.neurons], dtype=torch.int64
-        )
-        self.last_update = self._create_tensor(
-            [neuron.last_update for neuron in self.neurons], dtype=torch.int64
-        )
-        self.validator_permit = self._create_tensor(
-            [neuron.validator_permit for neuron in self.neurons], dtype=torch.bool
-        )
-        self.validator_trust = self._create_tensor(
-            [neuron.validator_trust for neuron in self.neurons], dtype=torch.float32
-        )
-        self.total_stake = self._create_tensor(
-            [neuron.total_stake.tao for neuron in self.neurons], dtype=torch.float32
-        )
-        self.stake = self._create_tensor(
-            [neuron.stake for neuron in self.neurons], dtype=torch.float32
-        )
-        self.axons = [n.axon_info for n in self.neurons]
-
-    def _create_tensor(self, data, dtype) -> torch.nn.Parameter:
+    @staticmethod
+    def _create_tensor(data, dtype) -> Union[NDArray, "torch.nn.Parameter"]:
         """
-        Creates a tensor parameter with the given data and data type. This method is a utility function used internally to encapsulate data into a PyTorch tensor, making it compatible with the metagraph's PyTorch
-        model structure.
+        Creates a numpy array with the given data and data type. This method is a utility function used internally to encapsulate data into a np.array, making it compatible with the metagraph's numpy model structure.
 
         Args:
             data: The data to be included in the tensor. This could be any numeric data, like stakes, ranks, etc.
-            dtype: The data type for the tensor, typically a PyTorch data type like ``torch.float32`` or ``torch.int64``.
+            dtype: The data type for the tensor, typically a numpy data type like ``np.float32`` or ``np.int64``.
 
         Returns:
             A tensor parameter encapsulating the provided data.
 
         Internal Usage:
             Used internally to create tensor parameters for various metagraph attributes::
 
-                self.stake = self._create_tensor(neuron_stakes, dtype=torch.float32)
+                self.stake = self._create_tensor(neuron_stakes, dtype=np.float32)
         """
         # TODO: Check and test the creation of tensor
-        return torch.nn.Parameter(torch.tensor(data, dtype=dtype), requires_grad=False)
+        return (
+            torch.nn.Parameter(torch.tensor(data, dtype=dtype), requires_grad=False)
+            if use_torch()
+            else np.array(data, dtype=dtype)
+        )
 
     def _set_weights_and_bonds(self, subtensor: Optional[bittensor.subtensor] = None):
         """
         Computes and sets the weights and bonds for each neuron in the metagraph. This method is responsible for processing the raw weight and bond data obtained from the network and converting it into a structured format suitable for the metagraph model.
 
         Args:
             subtensor: The subtensor instance used for fetching weights and bonds data. If ``None``, the weights and bonds are not updated.
@@ -677,15 +624,17 @@
             self.weights = self._process_weights_or_bonds(
                 [neuron.weights for neuron in self.neurons], "weights"
             )
             self.bonds = self._process_weights_or_bonds(
                 [neuron.bonds for neuron in self.neurons], "bonds"
             )
 
-    def _process_weights_or_bonds(self, data, attribute: str) -> torch.nn.Parameter:
+    def _process_weights_or_bonds(
+        self, data, attribute: str
+    ) -> Union[NDArray, "torch.nn.Parameter"]:
         """
         Processes the raw weights or bonds data and converts it into a structured tensor format. This method handles the transformation of neuron connection data (``weights`` or ``bonds``) from a list or other unstructured format into a tensor that can be utilized within the metagraph model.
 
         Args:
             data: The raw weights or bonds data to be processed. This data typically comes from the subtensor.
             attribute: A string indicating whether the data is ``weights`` or ``bonds``, which determines the specific processing steps to be applied.
 
@@ -696,44 +645,61 @@
             Used internally to process and set weights or bonds for the neurons::
 
                 self.weights = self._process_weights_or_bonds(raw_weights_data, "weights")
         """
         data_array = []
         for item in data:
             if len(item) == 0:
-                data_array.append(torch.zeros(len(self.neurons)))
+                if use_torch():
+                    data_array.append(torch.zeros(len(self.neurons)))  # type: ignore
+                else:
+                    data_array.append(np.zeros(len(self.neurons), dtype=np.float32))  # type: ignore
             else:
                 uids, values = zip(*item)
                 # TODO: Validate and test the conversion of uids and values to tensor
                 if attribute == "weights":
                     data_array.append(
                         bittensor.utils.weight_utils.convert_weight_uids_and_vals_to_tensor(
-                            len(self.neurons), list(uids), list(values)
+                            len(self.neurons), list(uids), list(values)  # type: ignore
                         )
                     )
                 else:
                     data_array.append(
-                        bittensor.utils.weight_utils.convert_bond_uids_and_vals_to_tensor(
+                        bittensor.utils.weight_utils.convert_bond_uids_and_vals_to_tensor(  # type: ignore
                             len(self.neurons), list(uids), list(values)
+                        ).astype(
+                            np.float32
                         )
                     )
-        tensor_param = (
-            torch.nn.Parameter(torch.stack(data_array), requires_grad=False)
-            if len(data_array)
-            else torch.nn.Parameter()
+        tensor_param: Union["torch.nn.Parameter", NDArray] = (
+            (
+                torch.nn.Parameter(torch.stack(data_array), requires_grad=False)
+                if len(data_array)
+                else torch.nn.Parameter()
+            )
+            if use_torch()
+            else (
+                np.stack(data_array)
+                if len(data_array)
+                else np.array([], dtype=np.float32)
+            )
         )
         if len(data_array) == 0:
             bittensor.logging.warning(
                 f"Empty {attribute}_array on metagraph.sync(). The '{attribute}' tensor is empty."
             )
         return tensor_param
 
+    @abstractmethod
+    def _set_metagraph_attributes(self, block, subtensor):
+        pass
+
     def _process_root_weights(
         self, data, attribute: str, subtensor: bittensor.subtensor
-    ) -> torch.nn.Parameter:
+    ) -> Union[NDArray, "torch.nn.Parameter"]:
         """
         Specifically processes the root weights data for the metagraph. This method is similar to :func:`_process_weights_or_bonds` but is tailored for processing root weights, which have a different structure and significance in the network.
 
         Args:
             data: The raw root weights data to be processed.
             attribute: A string indicating the attribute type, here it's typically ``weights``.
             subtensor: The subtensor instance used for additional data and context needed in processing.
@@ -750,36 +716,47 @@
 
         """
         data_array = []
         n_subnets = subtensor.get_total_subnets() or 0
         subnets = subtensor.get_subnets()
         for item in data:
             if len(item) == 0:
-                data_array.append(torch.zeros(n_subnets))
+                if use_torch():
+                    data_array.append(torch.zeros(n_subnets))
+                else:
+                    data_array.append(np.zeros(n_subnets, dtype=np.float32))  # type: ignore
             else:
                 uids, values = zip(*item)
                 # TODO: Validate and test the conversion of uids and values to tensor
                 data_array.append(
-                    bittensor.utils.weight_utils.convert_root_weight_uids_and_vals_to_tensor(
+                    bittensor.utils.weight_utils.convert_root_weight_uids_and_vals_to_tensor(  # type: ignore
                         n_subnets, list(uids), list(values), subnets
                     )
                 )
 
-        tensor_param = (
-            torch.nn.Parameter(torch.stack(data_array), requires_grad=False)
-            if len(data_array)
-            else torch.nn.Parameter()
+        tensor_param: Union[NDArray, "torch.nn.Parameter"] = (
+            (
+                torch.nn.Parameter(torch.stack(data_array), requires_grad=False)
+                if len(data_array)
+                else torch.nn.Parameter()
+            )
+            if use_torch()
+            else (
+                np.stack(data_array)
+                if len(data_array)
+                else np.array([], dtype=np.float32)
+            )
         )
         if len(data_array) == 0:
             bittensor.logging.warning(
                 f"Empty {attribute}_array on metagraph.sync(). The '{attribute}' tensor is empty."
             )
         return tensor_param
 
-    def save(self) -> "metagraph":
+    def save(self) -> "metagraph":  # type: ignore
         """
         Saves the current state of the metagraph to a file on disk. This function is crucial for persisting the current state of the network's metagraph, which can later be reloaded or analyzed. The save operation includes all neuron attributes and parameters, ensuring a complete snapshot of the metagraph's state.
 
         Returns:
             metagraph: The metagraph instance after saving its state.
 
         Example:
@@ -795,19 +772,27 @@
 
             If using a custom save path::
 
                 metagraph.load_from_path(dir_path)
         """
         save_directory = get_save_dir(self.network, self.netuid)
         os.makedirs(save_directory, exist_ok=True)
-        graph_file = save_directory + f"/block-{self.block.item()}.pt"
-        state_dict = self.state_dict()
-        state_dict["axons"] = self.axons
-        torch.save(state_dict, graph_file)
-        state_dict = torch.load(graph_file)
+        if use_torch():
+            graph_filename = f"{save_directory}/block-{self.block.item()}.pt"
+            state_dict = self.state_dict()
+            state_dict["axons"] = self.axons
+            torch.save(state_dict, graph_filename)
+            state_dict = torch.load(
+                graph_filename
+            )  # verifies that the file can be loaded correctly
+        else:
+            graph_filename = f"{save_directory}/block-{self.block.item()}.pt"
+            state_dict = self.state_dict()
+            with open(graph_filename, "wb") as graph_file:
+                pickle.dump(state_dict, graph_file)
         return self
 
     def load(self):
         """
         Loads the state of the metagraph from the default save directory. This method is instrumental for restoring the metagraph to its last saved state. It automatically identifies the save directory based on the ``network`` and ``netuid`` properties of the metagraph, locates the latest block file in that directory, and loads all metagraph parameters from it.
 
         This functionality is particularly beneficial when continuity in the state of the metagraph is necessary
@@ -827,15 +812,16 @@
             After this operation, the metagraph's parameters and neuron data are restored to their state at the time of the last save in the default directory.
 
         Note:
             The default save directory is determined based on the metagraph's ``network`` and ``netuid`` attributes. It is important to ensure that these attributes are set correctly and that the default save directory contains the appropriate state files for the metagraph.
         """
         self.load_from_path(get_save_dir(self.network, self.netuid))
 
-    def load_from_path(self, dir_path: str) -> "metagraph":
+    @abstractmethod
+    def load_from_path(self, dir_path: str) -> "metagraph":  # type: ignore
         """
         Loads the state of the metagraph from a specified directory path. This method is crucial for restoring the metagraph to a specific state based on saved data. It locates the latest block file in the given
         directory and loads all metagraph parameters from it. This is particularly useful for analyses that require historical states of the network or for restoring previous states of the metagraph in different
         execution environments.
 
         The method first identifies the latest block file in the specified directory, then loads the metagraph state including neuron attributes and parameters from this file. This ensures that the metagraph is accurately reconstituted to reflect the network state at the time of the saved block.
 
@@ -854,14 +840,164 @@
             The metagraph is now restored to the state it was in at the time of the latest saved block in the specified directory.
 
         Note:
             This method assumes that the state files in the specified directory are correctly formatted and
             contain valid data for the metagraph. It is essential to ensure that the directory path and the
             state files within it are accurate and consistent with the expected metagraph structure.
         """
+        pass
+
+
+BaseClass: Union["torch.nn.Module", object] = torch.nn.Module if use_torch() else object
+
+
+class TorchMetaGraph(MetagraphMixin, BaseClass):  # type: ignore
+    def __init__(
+        self, netuid: int, network: str = "finney", lite: bool = True, sync: bool = True
+    ):
+        """
+        Initializes a new instance of the metagraph object, setting up the basic structure and parameters based on the provided arguments.
+        This method is the entry point for creating a metagraph object,
+        which is a central component in representing the state of the Bittensor network.
+        Args:
+            netuid (int): The unique identifier for the network, distinguishing this instance of the metagraph within potentially multiple network configurations.
+            network (str): The name of the network, which can indicate specific configurations or versions of the Bittensor network.
+            lite (bool): A flag indicating whether to use a lite version of the metagraph. The lite version may contain less detailed information but can be quicker to initialize and sync.
+            sync (bool): A flag indicating whether to synchronize the metagraph with the network upon initialization. Synchronization involves updating the metagraph's parameters to reflect the current state of the network.
+        Example:
+            Initializing a metagraph object for the Bittensor network with a specific network UID::
+                metagraph = metagraph(netuid=123, network="finney", lite=True, sync=True)
+        """
+        torch.nn.Module.__init__(self)
+        MetagraphMixin.__init__(self, netuid, network, lite, sync)
+        self.netuid = netuid
+        self.network = network
+        self.version = torch.nn.Parameter(
+            torch.tensor([bittensor.__version_as_int__], dtype=torch.int64),
+            requires_grad=False,
+        )
+        self.n: torch.nn.Parameter = torch.nn.Parameter(
+            torch.tensor([0], dtype=torch.int64), requires_grad=False
+        )
+        self.block: torch.nn.Parameter = torch.nn.Parameter(
+            torch.tensor([0], dtype=torch.int64), requires_grad=False
+        )
+        self.stake = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.float32), requires_grad=False
+        )
+        self.total_stake: torch.nn.Parameter = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.float32), requires_grad=False
+        )
+        self.ranks: torch.nn.Parameter = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.float32), requires_grad=False
+        )
+        self.trust: torch.nn.Parameter = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.float32), requires_grad=False
+        )
+        self.consensus: torch.nn.Parameter = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.float32), requires_grad=False
+        )
+        self.validator_trust: torch.nn.Parameter = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.float32), requires_grad=False
+        )
+        self.incentive: torch.nn.Parameter = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.float32), requires_grad=False
+        )
+        self.emission: torch.nn.Parameter = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.float32), requires_grad=False
+        )
+        self.dividends: torch.nn.Parameter = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.float32), requires_grad=False
+        )
+        self.active = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.int64), requires_grad=False
+        )
+        self.last_update = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.int64), requires_grad=False
+        )
+        self.validator_permit = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.bool), requires_grad=False
+        )
+        self.weights: torch.nn.Parameter = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.float32), requires_grad=False
+        )
+        self.bonds: torch.nn.Parameter = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.int64), requires_grad=False
+        )
+        self.uids = torch.nn.Parameter(
+            torch.tensor([], dtype=torch.int64), requires_grad=False
+        )
+        self.axons: List[AxonInfo] = []
+        if sync:
+            self.sync(block=None, lite=lite)
+
+    def _set_metagraph_attributes(self, block, subtensor):
+        """
+        Sets various attributes of the metagraph based on the latest network data fetched from the subtensor.
+
+        This method updates parameters like the number of neurons, block number, stakes, trusts, ranks, and other neuron-specific information.
+
+        Args:
+            block: The block number for which the metagraph attributes need to be set. If ``None``, the latest block data is used.
+            subtensor: The subtensor instance used for fetching the latest network data.
+
+        Internal Usage:
+            Used internally during the sync process to update the metagraph's attributes::
+
+                self._set_metagraph_attributes(block, subtensor)
+        """
+        self.n = self._create_tensor(len(self.neurons), dtype=torch.int64)
+        self.version = self._create_tensor(
+            [bittensor.__version_as_int__], dtype=torch.int64
+        )
+        self.block = self._create_tensor(
+            block if block else subtensor.block, dtype=torch.int64
+        )
+        self.uids = self._create_tensor(
+            [neuron.uid for neuron in self.neurons], dtype=torch.int64
+        )
+        self.trust = self._create_tensor(
+            [neuron.trust for neuron in self.neurons], dtype=torch.float32
+        )
+        self.consensus = self._create_tensor(
+            [neuron.consensus for neuron in self.neurons], dtype=torch.float32
+        )
+        self.incentive = self._create_tensor(
+            [neuron.incentive for neuron in self.neurons], dtype=torch.float32
+        )
+        self.dividends = self._create_tensor(
+            [neuron.dividends for neuron in self.neurons], dtype=torch.float32
+        )
+        self.ranks = self._create_tensor(
+            [neuron.rank for neuron in self.neurons], dtype=torch.float32
+        )
+        self.emission = self._create_tensor(
+            [neuron.emission for neuron in self.neurons], dtype=torch.float32
+        )
+        self.active = self._create_tensor(
+            [neuron.active for neuron in self.neurons], dtype=torch.int64
+        )
+        self.last_update = self._create_tensor(
+            [neuron.last_update for neuron in self.neurons], dtype=torch.int64
+        )
+        self.validator_permit = self._create_tensor(
+            [neuron.validator_permit for neuron in self.neurons], dtype=torch.bool
+        )
+        self.validator_trust = self._create_tensor(
+            [neuron.validator_trust for neuron in self.neurons], dtype=torch.float32
+        )
+        self.total_stake = self._create_tensor(
+            [neuron.total_stake.tao for neuron in self.neurons], dtype=torch.float32
+        )
+        self.stake = self._create_tensor(
+            [neuron.stake for neuron in self.neurons], dtype=torch.float32
+        )
+        self.axons = [n.axon_info for n in self.neurons]
+
+    def load_from_path(self, dir_path: str) -> "metagraph":  # type: ignore
         graph_file = latest_block_path(dir_path)
         state_dict = torch.load(graph_file)
         self.n = torch.nn.Parameter(state_dict["n"], requires_grad=False)
         self.block = torch.nn.Parameter(state_dict["block"], requires_grad=False)
         self.uids = torch.nn.Parameter(state_dict["uids"], requires_grad=False)
         self.stake = torch.nn.Parameter(state_dict["stake"], requires_grad=False)
         self.total_stake = torch.nn.Parameter(
@@ -894,7 +1030,152 @@
         if "weights" in state_dict:
             self.weights = torch.nn.Parameter(
                 state_dict["weights"], requires_grad=False
             )
         if "bonds" in state_dict:
             self.bonds = torch.nn.Parameter(state_dict["bonds"], requires_grad=False)
         return self
+
+
+class NonTorchMetagraph(MetagraphMixin):
+    def __init__(
+        self, netuid: int, network: str = "finney", lite: bool = True, sync: bool = True
+    ):
+        # super(metagraph, self).__init__()
+        MetagraphMixin.__init__(self, netuid, network, lite, sync)
+
+        self.netuid = netuid
+        self.network = network
+        self.version = (np.array([bittensor.__version_as_int__], dtype=np.int64),)
+        self.n = np.array([0], dtype=np.int64)
+        self.block = np.array([0], dtype=np.int64)
+        self.stake = np.array([], dtype=np.float32)
+        self.total_stake = np.array([], dtype=np.float32)
+        self.ranks = np.array([], dtype=np.float32)
+        self.trust = np.array([], dtype=np.float32)
+        self.consensus = np.array([], dtype=np.float32)
+        self.validator_trust = np.array([], dtype=np.float32)
+        self.incentive = np.array([], dtype=np.float32)
+        self.emission = np.array([], dtype=np.float32)
+        self.dividends = np.array([], dtype=np.float32)
+        self.active = np.array([], dtype=np.int64)
+        self.last_update = np.array([], dtype=np.int64)
+        self.validator_permit = np.array([], dtype=bool)
+        self.weights = np.array([], dtype=np.float32)
+        self.bonds = np.array([], dtype=np.int64)
+        self.uids = np.array([], dtype=np.int64)
+        self.axons: List[AxonInfo] = []
+        if sync:
+            self.sync(block=None, lite=lite)
+
+    def _set_metagraph_attributes(self, block, subtensor):
+        """
+        Sets various attributes of the metagraph based on the latest network data fetched from the subtensor.
+
+        This method updates parameters like the number of neurons, block number, stakes, trusts, ranks, and other neuron-specific information.
+
+        Args:
+            block: The block number for which the metagraph attributes need to be set. If ``None``, the latest block data is used.
+            subtensor: The subtensor instance used for fetching the latest network data.
+
+        Internal Usage:
+            Used internally during the sync process to update the metagraph's attributes::
+
+                self._set_metagraph_attributes(block, subtensor)
+        """
+        # TODO: Check and test the setting of each attribute
+        self.n = self._create_tensor(len(self.neurons), dtype=np.int64)
+        self.version = self._create_tensor(
+            [bittensor.__version_as_int__], dtype=np.int64
+        )
+        self.block = self._create_tensor(
+            block if block else subtensor.block, dtype=np.int64
+        )
+        self.uids = self._create_tensor(
+            [neuron.uid for neuron in self.neurons], dtype=np.int64
+        )
+        self.trust = self._create_tensor(
+            [neuron.trust for neuron in self.neurons], dtype=np.float32
+        )
+        self.consensus = self._create_tensor(
+            [neuron.consensus for neuron in self.neurons], dtype=np.float32
+        )
+        self.incentive = self._create_tensor(
+            [neuron.incentive for neuron in self.neurons], dtype=np.float32
+        )
+        self.dividends = self._create_tensor(
+            [neuron.dividends for neuron in self.neurons], dtype=np.float32
+        )
+        self.ranks = self._create_tensor(
+            [neuron.rank for neuron in self.neurons], dtype=np.float32
+        )
+        self.emission = self._create_tensor(
+            [neuron.emission for neuron in self.neurons], dtype=np.float32
+        )
+        self.active = self._create_tensor(
+            [neuron.active for neuron in self.neurons], dtype=np.int64
+        )
+        self.last_update = self._create_tensor(
+            [neuron.last_update for neuron in self.neurons], dtype=np.int64
+        )
+        self.validator_permit = self._create_tensor(
+            [neuron.validator_permit for neuron in self.neurons], dtype=bool
+        )
+        self.validator_trust = self._create_tensor(
+            [neuron.validator_trust for neuron in self.neurons], dtype=np.float32
+        )
+        self.total_stake = self._create_tensor(
+            [neuron.total_stake.tao for neuron in self.neurons], dtype=np.float32
+        )
+        self.stake = self._create_tensor(
+            [neuron.stake for neuron in self.neurons], dtype=np.float32
+        )
+        self.axons = [n.axon_info for n in self.neurons]
+
+    def load_from_path(self, dir_path: str) -> "metagraph":  # type: ignore
+        graph_filename = latest_block_path(dir_path)
+        try:
+            with open(graph_filename, "rb") as graph_file:
+                state_dict = pickle.load(graph_file)
+        except pickle.UnpicklingError:
+            bittensor.__console__.print(
+                "Unable to load file. Attempting to restore metagraph using torch."
+            )
+            bittensor.__console__.print(
+                ":warning:[yellow]Warning:[/yellow] This functionality exists to load "
+                "metagraph state from legacy saves, but will not be supported in the future."
+            )
+            try:
+                import torch as real_torch
+
+                state_dict = real_torch.load(graph_filename)
+                for key in METAGRAPH_STATE_DICT_NDARRAY_KEYS:
+                    state_dict[key] = state_dict[key].detach().numpy()
+                del real_torch
+            except (RuntimeError, ImportError):
+                bittensor.__console__.print("Unable to load file. It may be corrupted.")
+                raise
+
+        self.n = state_dict["n"]
+        self.block = state_dict["block"]
+        self.uids = state_dict["uids"]
+        self.stake = state_dict["stake"]
+        self.total_stake = state_dict["total_stake"]
+        self.ranks = state_dict["ranks"]
+        self.trust = state_dict["trust"]
+        self.consensus = state_dict["consensus"]
+        self.validator_trust = state_dict["validator_trust"]
+        self.incentive = state_dict["incentive"]
+        self.emission = state_dict["emission"]
+        self.dividends = state_dict["dividends"]
+        self.active = state_dict["active"]
+        self.last_update = state_dict["last_update"]
+        self.validator_permit = state_dict["validator_permit"]
+        self.axons = state_dict["axons"]
+        if "weights" in state_dict:
+            self.weights = state_dict["weights"]
+        if "bonds" in state_dict:
+            self.bonds = state_dict["bonds"]
+        return self
+
+
+metagraph = TorchMetaGraph if use_torch() else NonTorchMetagraph
```

### Comparing `bittensor-6.9.3/bittensor/mock/__init__.py` & `bittensor-7.0.0/bittensor/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/mock/keyfile_mock.py` & `bittensor-7.0.0/bittensor/mock/keyfile_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/mock/subtensor_mock.py` & `bittensor-7.0.0/bittensor/mock/subtensor_mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     NeuronInfo,
     NeuronInfoLite,
     PrometheusInfo,
     DelegateInfo,
     SubnetInfo,
     AxonInfo,
 )
-from ..errors import *
+from ..errors import ChainQueryError
 from ..subtensor import subtensor
 from ..utils import RAOPERTAO, U16_NORMALIZED_FLOAT
 from ..utils.balance import Balance
 from ..utils.registration import POWSolution
 
 from typing import TypedDict
 
@@ -1301,14 +1301,26 @@
 
         self.chain_state["System"]["Account"][wallet.coldkeypub.ss58_address]["data"][
             "free"
         ][self.block_number] = (bal + amount).rao
 
         return True
 
+    @staticmethod
+    def min_required_stake():
+        """
+        As the minimum required stake may change, this method allows us to dynamically
+        update the amount in the mock without updating the tests
+        """
+        # valid minimum threshold as of 2024/05/01
+        return 100_000_000  # RAO
+
+    def get_minimum_required_stake(self):
+        return Balance.from_rao(self.min_required_stake())
+
     def get_delegate_by_hotkey(
         self, hotkey_ss58: str, block: Optional[int] = None
     ) -> Optional["DelegateInfo"]:
         subtensor_state = self.chain_state["SubtensorModule"]
 
         if hotkey_ss58 not in subtensor_state["Delegates"]:
             return None
```

### Comparing `bittensor-6.9.3/bittensor/mock/wallet_mock.py` & `bittensor-7.0.0/bittensor/mock/wallet_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/stream.py` & `bittensor-7.0.0/bittensor/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from aiohttp import ClientResponse
 import bittensor
 
 from starlette.responses import StreamingResponse as _StreamingResponse
 from starlette.types import Send, Receive, Scope
 from typing import Callable, Awaitable
-from pydantic import BaseModel
+from pydantic import ConfigDict, BaseModel
 from abc import ABC, abstractmethod
 
 
 class BTStreamingResponseModel(BaseModel):
     """
     :func:`BTStreamingResponseModel` is a Pydantic model that encapsulates the token streamer callable for Pydantic validation.
     It is used within the :func:`StreamingSynapse` class to create a :func:`BTStreamingResponse` object, which is responsible for handling
@@ -32,16 +32,15 @@
 class StreamingSynapse(bittensor.Synapse, ABC):
     """
     The :func:`StreamingSynapse` class is designed to be subclassed for handling streaming responses in the Bittensor network.
     It provides abstract methods that must be implemented by the subclass to deserialize, process streaming responses,
     and extract JSON data. It also includes a method to create a streaming response object.
     """
 
-    class Config:
-        validate_assignment = True
+    model_config = ConfigDict(validate_assignment=True)
 
     class BTStreamingResponse(_StreamingResponse):
         """
         :func:`BTStreamingResponse` is a specialized subclass of the Starlette StreamingResponse designed to handle the streaming
         of tokens within the Bittensor network. It is used internally by the StreamingSynapse class to manage the response
         streaming process, including sending headers and calling the token streamer provided by the subclass.
```

### Comparing `bittensor-6.9.3/bittensor/subnets.py` & `bittensor-7.0.0/bittensor/subnets.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/subtensor.py` & `bittensor-7.0.0/bittensor/subtensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,101 +12,131 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-import os
+"""
+The ``bittensor.subtensor`` module in Bittensor serves as a crucial interface for interacting with the Bittensor
+blockchain, facilitating a range of operations essential for the decentralized machine learning network.
+"""
+import argparse
 import copy
+import functools
+import socket
 import time
-import torch
-import argparse
-import bittensor
-import scalecodec
+from typing import List, Dict, Union, Optional, Tuple, TypedDict, Any, TypeVar
 
+import numpy as np
+import scalecodec
+from numpy.typing import NDArray
 from retry import retry
-from loguru import logger
-from typing import List, Dict, Union, Optional, Tuple, TypedDict, Any, TypeVar
-from substrateinterface.base import QueryMapResult, SubstrateInterface, ExtrinsicReceipt
-from substrateinterface.exceptions import SubstrateRequestException
 from scalecodec.base import RuntimeConfiguration
+from scalecodec.exceptions import RemainingScaleBytesNotEmptyException
 from scalecodec.type_registry import load_type_registry_preset
 from scalecodec.types import GenericCall
+from substrateinterface.base import QueryMapResult, SubstrateInterface, ExtrinsicReceipt
+from substrateinterface.exceptions import SubstrateRequestException
+
 
-# Local imports.
+import bittensor
+from bittensor.utils import torch
+from bittensor.btlogging import logging as _logger
 from .chain_data import (
     NeuronInfo,
     DelegateInfo,
     PrometheusInfo,
     SubnetInfo,
     SubnetHyperparameters,
     StakeInfo,
     NeuronInfoLite,
     AxonInfo,
     ProposalVoteData,
     IPInfo,
     custom_rpc_type_registry,
 )
-from .errors import *
+from .errors import IdentityError, NominationError, StakeError, TakeError
+from .extrinsics.delegation import (
+    delegate_extrinsic,
+    nominate_extrinsic,
+    undelegate_extrinsic,
+    increase_take_extrinsic,
+    decrease_take_extrinsic,
+)
 from .extrinsics.network import (
     register_subnetwork_extrinsic,
     set_hyperparameter_extrinsic,
 )
-from .extrinsics.staking import add_stake_extrinsic, add_stake_multiple_extrinsic
-from .extrinsics.unstaking import unstake_extrinsic, unstake_multiple_extrinsic
-from .extrinsics.serving import (
-    serve_extrinsic,
-    serve_axon_extrinsic,
-    publish_metadata,
-    get_metadata,
-)
+from .extrinsics.prometheus import prometheus_extrinsic
 from .extrinsics.registration import (
     register_extrinsic,
     burned_register_extrinsic,
     run_faucet_extrinsic,
     swap_hotkey_extrinsic,
 )
-from .extrinsics.transfer import transfer_extrinsic
-from .extrinsics.set_weights import set_weights_extrinsic
-from .extrinsics.prometheus import prometheus_extrinsic
-from .extrinsics.delegation import (
-    delegate_extrinsic,
-    nominate_extrinsic,
-    undelegate_extrinsic,
-)
+from .extrinsics.root import root_register_extrinsic, set_root_weights_extrinsic
 from .extrinsics.senate import (
     register_senate_extrinsic,
     leave_senate_extrinsic,
     vote_senate_extrinsic,
 )
-from .extrinsics.root import root_register_extrinsic, set_root_weights_extrinsic
+from .extrinsics.serving import (
+    serve_extrinsic,
+    serve_axon_extrinsic,
+    publish_metadata,
+    get_metadata,
+)
+from .extrinsics.set_weights import set_weights_extrinsic
+from .extrinsics.staking import add_stake_extrinsic, add_stake_multiple_extrinsic
+from .extrinsics.transfer import transfer_extrinsic
+from .extrinsics.unstaking import unstake_extrinsic, unstake_multiple_extrinsic
 from .types import AxonServeCallParams, PrometheusServeCallParams
-from .utils import U16_NORMALIZED_FLOAT, ss58_to_vec_u8, U64_NORMALIZED_FLOAT
+from .utils import (
+    U16_NORMALIZED_FLOAT,
+    ss58_to_vec_u8,
+    U64_NORMALIZED_FLOAT,
+    networking,
+)
 from .utils.balance import Balance
 from .utils.registration import POWSolution
+from .utils.subtensor import get_subtensor_errors
+from .utils.registration import legacy_torch_api_compat
 
-logger = logger.opt(colors=True)
 
 KEY_NONCE: Dict[str, int] = {}
 
 T = TypeVar("T")
 
+#######
+# Monkey patch in caching the convert_type_string method
+#######
+if hasattr(RuntimeConfiguration, "convert_type_string"):
+    original_convert_type_string = RuntimeConfiguration.convert_type_string
+
+    @functools.lru_cache(maxsize=None)
+    def convert_type_string(cls, name):
+        return original_convert_type_string(name)
+
+    RuntimeConfiguration.convert_type_string = convert_type_string
+#######
+
 
 class ParamWithTypes(TypedDict):
     name: str  # Name of the parameter.
     type: str  # ScaleType string of the parameter.
 
 
 class subtensor:
     """
-    The Subtensor class in Bittensor serves as a crucial interface for interacting with the Bittensor blockchain, facilitating a range of operations essential for the decentralized machine learning network.
+    The Subtensor class in Bittensor serves as a crucial interface for interacting with the Bittensor blockchain,
+    facilitating a range of operations essential for the decentralized machine learning network.
 
-    This class enables neurons (network participants) to engage in activities such as registering on the network, managing
-    staked weights, setting inter-neuronal weights, and participating in consensus mechanisms.
+    This class enables neurons (network participants) to engage in activities such as registering on the network,
+    managing staked weights, setting inter-neuronal weights, and participating in consensus mechanisms.
 
     The Bittensor network operates on a digital ledger where each neuron holds stakes (S) and learns a set
     of inter-peer weights (W). These weights, set by the neurons themselves, play a critical role in determining
     the ranking and incentive mechanisms within the network. Higher-ranked neurons, as determined by their
     contributions and trust within the network, receive more incentives.
 
     The Subtensor class connects to various Bittensor networks like the main ``finney`` network or local test
@@ -116,16 +146,18 @@
 
     Additionally, Bittensor introduces a speculation-based reward mechanism in the form of bonds (B), allowing
     neurons to accumulate bonds in other neurons, speculating on their future value. This mechanism aligns
     with market-based speculation, incentivizing neurons to make judicious decisions in their inter-neuronal
     investments.
 
     Args:
-        network (str): The name of the Bittensor network (e.g., 'finney', 'test', 'archive', 'local') the instance is connected to, determining the blockchain interaction context.
-        chain_endpoint (str): The blockchain node endpoint URL, enabling direct communication with the Bittensor blockchain for transaction processing and data retrieval.
+        network (str): The name of the Bittensor network (e.g., 'finney', 'test', 'archive', 'local') the instance is
+            connected to, determining the blockchain interaction context.
+        chain_endpoint (str): The blockchain node endpoint URL, enabling direct communication with the Bittensor
+            blockchain for transaction processing and data retrieval.
 
     Example Usage::
 
         # Connect to the main Bittensor network (Finney).
         finney_subtensor = subtensor(network='finney')
 
         # Close websocket connection with the Bittensor network.
@@ -145,88 +177,228 @@
         success = finney_subtensor.delegate(wallet=wallet, delegate_ss58=other_neuron_ss58, amount=bond_amount)
 
         # Get the metagraph for a specific subnet using given subtensor connection
         metagraph = subtensor.metagraph(netuid=netuid)
 
     By facilitating these operations, the Subtensor class is instrumental in maintaining the decentralized
     intelligence and dynamic learning environment of the Bittensor network, as envisioned in its foundational
-    principles and mechanisms described in the `NeurIPS paper <https://bittensor.com/pdfs/academia/NeurIPS_DAO_Workshop_2022_3_3.pdf>`_. paper.
+    principles and mechanisms described in the `NeurIPS paper
+    <https://bittensor.com/pdfs/academia/NeurIPS_DAO_Workshop_2022_3_3.pdf>`_. paper.
     """
 
+    def __init__(
+        self,
+        network: Optional[str] = None,
+        config: Optional[bittensor.config] = None,
+        _mock: bool = False,
+        log_verbose: bool = True,
+    ) -> None:
+        """
+        Initializes a Subtensor interface for interacting with the Bittensor blockchain.
+
+        NOTE:
+            Currently subtensor defaults to the ``finney`` network. This will change in a future release.
+
+        We strongly encourage users to run their own local subtensor node whenever possible. This increases
+        decentralization and resilience of the network. In a future release, local subtensor will become the
+        default and the fallback to ``finney`` removed. Please plan ahead for this change. We will provide detailed
+        instructions on how to run a local subtensor node in the documentation in a subsequent release.
+
+        Args:
+            network (str, optional): The network name to connect to (e.g., ``finney``, ``local``). This can also be the
+                chain endpoint (e.g., ``wss://entrypoint-finney.opentensor.ai:443``) and will be correctly parsed into
+                the network and chain endpoint. If not specified, defaults to the main Bittensor network.
+            config (bittensor.config, optional): Configuration object for the subtensor. If not provided, a default
+                configuration is used.
+            _mock (bool, optional): If set to ``True``, uses a mocked connection for testing purposes.
+
+        This initialization sets up the connection to the specified Bittensor network, allowing for various
+        blockchain operations such as neuron registration, stake management, and setting weights.
+
+        """
+        # Determine config.subtensor.chain_endpoint and config.subtensor.network config.
+        # If chain_endpoint is set, we override the network flag, otherwise, the chain_endpoint is assigned by the
+        # network.
+        # Argument importance: network > chain_endpoint > config.subtensor.chain_endpoint > config.subtensor.network
+
+        # Check if network is a config object. (Single argument passed as first positional)
+        if isinstance(network, bittensor.config):
+            if network.subtensor is None:
+                _logger.warning(
+                    "If passing a bittensor config object, it must not be empty. Using default subtensor config."
+                )
+                config = None
+            else:
+                config = network
+            network = None
+
+        if config is None:
+            config = subtensor.config()
+        self.config = copy.deepcopy(config)  # type: ignore
+
+        # Setup config.subtensor.network and config.subtensor.chain_endpoint
+        self.chain_endpoint, self.network = subtensor.setup_config(network, config)  # type: ignore
+
+        if (
+            self.network == "finney"
+            or self.chain_endpoint == bittensor.__finney_entrypoint__
+        ) and log_verbose:
+            _logger.info(
+                f"You are connecting to {self.network} network with endpoint {self.chain_endpoint}."
+            )
+            _logger.warning(
+                "We strongly encourage running a local subtensor node whenever possible. "
+                "This increases decentralization and resilience of the network."
+            )
+            _logger.warning(
+                "In a future release, local subtensor will become the default endpoint. "
+                "To get ahead of this change, please run a local subtensor node and point to it."
+            )
+
+        # Attempt to connect to chosen endpoint. Fallback to finney if local unavailable.
+        try:
+            # Set up params.
+            self.substrate = SubstrateInterface(
+                ss58_format=bittensor.__ss58_format__,
+                use_remote_preset=True,
+                url=self.chain_endpoint,
+                type_registry=bittensor.__type_registry__,
+            )
+        except ConnectionRefusedError as e:
+            _logger.error(
+                f"Could not connect to {self.network} network with {self.chain_endpoint} chain endpoint. Exiting...",
+            )
+            _logger.info(
+                "You can check if you have connectivity by running this command: nc -vz localhost "
+                f"{self.chain_endpoint.split(':')[2]}"
+            )
+            exit(1)
+            # TODO (edu/phil): Advise to run local subtensor and point to dev docs.
+
+        try:
+            self.substrate.websocket.settimeout(600)
+        # except:
+        #     bittensor.logging.warning("Could not set websocket timeout.")
+        except AttributeError as e:
+            _logger.warning(f"AttributeError: {e}")
+        except TypeError as e:
+            _logger.warning(f"TypeError: {e}")
+        except (socket.error, OSError) as e:
+            _logger.warning(f"Socket error: {e}")
+
+        if log_verbose:
+            _logger.info(
+                f"Connected to {self.network} network and {self.chain_endpoint}."
+            )
+
+        self._subtensor_errors: Dict[str, Dict[str, str]] = {}
+
+    def __str__(self) -> str:
+        if self.network == self.chain_endpoint:
+            # Connecting to chain endpoint without network known.
+            return "subtensor({})".format(self.chain_endpoint)
+        else:
+            # Connecting to network with endpoint known.
+            return "subtensor({}, {})".format(self.network, self.chain_endpoint)
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
     @staticmethod
-    def config() -> "bittensor.config":
+    def config() -> bittensor.config:
+        """
+        Creates and returns a Bittensor configuration object.
+
+        Returns:
+            config (bittensor.config): A Bittensor configuration object configured with arguments added by the
+                `subtensor.add_args` method.
+        """
         parser = argparse.ArgumentParser()
         subtensor.add_args(parser)
         return bittensor.config(parser, args=[])
 
     @classmethod
     def help(cls):
-        """Print help to stdout"""
+        """Print help to stdout."""
         parser = argparse.ArgumentParser()
         cls.add_args(parser)
         print(cls.__new__.__doc__)
         parser.print_help()
 
     @classmethod
     def add_args(cls, parser: argparse.ArgumentParser, prefix: Optional[str] = None):
+        """
+        Adds command-line arguments to the provided ArgumentParser for configuring the Subtensor settings.
+
+        Args:
+            parser (argparse.ArgumentParser): The ArgumentParser object to which the Subtensor arguments will be added.
+            prefix (Optional[str]): An optional prefix for the argument names. If provided, the prefix is prepended to
+                each argument name.
+
+        Arguments added:
+            --subtensor.network: The Subtensor network flag. Possible values are 'finney', 'test', 'archive', and
+                'local'. Overrides the chain endpoint if set.
+            --subtensor.chain_endpoint: The Subtensor chain endpoint flag. If set, it overrides the network flag.
+            --subtensor._mock: If true, uses a mocked connection to the chain.
+
+        Example:
+            parser = argparse.ArgumentParser()
+            Subtensor.add_args(parser)
+        """
         prefix_str = "" if prefix is None else f"{prefix}."
         try:
-            default_network = os.getenv("BT_SUBTENSOR_NETWORK") or "finney"
-            default_chain_endpoint = (
-                os.getenv("BT_SUBTENSOR_CHAIN_ENDPOINT")
-                or bittensor.__finney_entrypoint__
-            )
+            default_network = bittensor.__networks__[1]
+            default_chain_endpoint = bittensor.__finney_entrypoint__
+
             parser.add_argument(
-                "--" + prefix_str + "subtensor.network",
+                f"--{prefix_str}subtensor.network",
                 default=default_network,
                 type=str,
                 help="""The subtensor network flag. The likely choices are:
                                         -- finney (main network)
                                         -- test (test network)
                                         -- archive (archive network +300 blocks)
                                         -- local (local running network)
                                     If this option is set it overloads subtensor.chain_endpoint with
                                     an entry point node from that network.
                                     """,
             )
             parser.add_argument(
-                "--" + prefix_str + "subtensor.chain_endpoint",
+                f"--{prefix_str}subtensor.chain_endpoint",
                 default=default_chain_endpoint,
                 type=str,
-                help="""The subtensor endpoint flag. If set, overrides the --network flag.
-                                    """,
+                help="""The subtensor endpoint flag. If set, overrides the --network flag.""",
             )
             parser.add_argument(
-                "--" + prefix_str + "subtensor._mock",
+                f"--{prefix_str}subtensor._mock",
                 default=False,
                 type=bool,
-                help="""If true, uses a mocked connection to the chain.
-                                    """,
+                help="""If true, uses a mocked connection to the chain.""",
             )
 
         except argparse.ArgumentError:
             # re-parsing arguments.
             pass
 
     @staticmethod
     def determine_chain_endpoint_and_network(network: str):
         """Determines the chain endpoint and network from the passed network or chain_endpoint.
 
         Args:
-            network (str): The network flag. The choices are: ``-- finney`` (main network), ``-- archive`` (archive network +300 blocks), ``-- local`` (local running network), ``-- test`` (test network).
-            chain_endpoint (str): The chain endpoint flag. If set, overrides the network argument.
+            network (str): The network flag. The choices are: ``-- finney`` (main network), ``-- archive``
+                (archive network +300 blocks), ``-- local`` (local running network), ``-- test`` (test network).
         Returns:
             network (str): The network flag.
             chain_endpoint (str): The chain endpoint flag. If set, overrides the ``network`` argument.
         """
         if network is None:
             return None, None
         if network in ["finney", "local", "test", "archive"]:
             if network == "finney":
-                # Kiru Finney stagin network.
+                # Kiru Finney staging network.
                 return network, bittensor.__finney_entrypoint__
             elif network == "local":
                 return network, bittensor.__local_entrypoint__
             elif network == "test":
                 return network, bittensor.__finney_test_entrypoint__
             elif network == "archive":
                 return network, bittensor.__archive_entrypoint__
@@ -249,15 +421,34 @@
             elif "127.0.0.1" in network or "localhost" in network:
                 return "local", network
             else:
                 return "unknown", network
 
     @staticmethod
     def setup_config(network: str, config: bittensor.config):
-        if network != None:
+        """
+        Sets up and returns the configuration for the Subtensor network and endpoint.
+
+        This method determines the appropriate network and chain endpoint based on the provided network string or
+        configuration object. It evaluates the network and endpoint in the following order of precedence:
+        1. Provided network string.
+        2. Configured chain endpoint in the `config` object.
+        3. Configured network in the `config` object.
+        4. Default chain endpoint.
+        5. Default network.
+
+        Args:
+            network (str): The name of the Subtensor network. If None, the network and endpoint will be determined from
+                the `config` object.
+            config (bittensor.config): The configuration object containing the network and chain endpoint settings.
+
+        Returns:
+            tuple: A tuple containing the formatted WebSocket endpoint URL and the evaluated network name.
+        """
+        if network is not None:
             (
                 evaluated_network,
                 evaluated_endpoint,
             ) = subtensor.determine_chain_endpoint_and_network(network)
         else:
             if config.get("__is_set", {}).get("subtensor.chain_endpoint"):
                 (
@@ -296,169 +487,40 @@
                     evaluated_network,
                     evaluated_endpoint,
                 ) = subtensor.determine_chain_endpoint_and_network(
                     bittensor.defaults.subtensor.network
                 )
 
         return (
-            bittensor.utils.networking.get_formatted_ws_endpoint_url(
-                evaluated_endpoint
-            ),
+            networking.get_formatted_ws_endpoint_url(evaluated_endpoint),
             evaluated_network,
         )
 
-    def __init__(
-        self,
-        network: Optional[str] = None,
-        config: Optional[bittensor.config] = None,
-        _mock: bool = False,
-        log_verbose: bool = True,
-    ) -> None:
-        """
-        Initializes a Subtensor interface for interacting with the Bittensor blockchain.
-
-        NOTE:
-            Currently subtensor defaults to the ``finney`` network. This will change in a future release.
-
-        We strongly encourage users to run their own local subtensor node whenever possible. This increases
-        decentralization and resilience of the network. In a future release, local subtensor will become the
-        default and the fallback to ``finney`` removed. Please plan ahead for this change. We will provide detailed
-        instructions on how to run a local subtensor node in the documentation in a subsequent release.
-
-        Args:
-            network (str, optional): The network name to connect to (e.g., ``finney``, ``local``). This can also be the chain endpoint (e.g., ``wss://entrypoint-finney.opentensor.ai:443``) and will be correctly parsed into the network and chain endpoint. If not specified, defaults to the main Bittensor network.
-            config (bittensor.config, optional): Configuration object for the subtensor. If not provided, a default configuration is used.
-            _mock (bool, optional): If set to ``True``, uses a mocked connection for testing purposes.
-
-        This initialization sets up the connection to the specified Bittensor network, allowing for various
-        blockchain operations such as neuron registration, stake management, and setting weights.
-
-        """
-        # Determine config.subtensor.chain_endpoint and config.subtensor.network config.
-        # If chain_endpoint is set, we override the network flag, otherwise, the chain_endpoint is assigned by the network.
-        # Argument importance: network > chain_endpoint > config.subtensor.chain_endpoint > config.subtensor.network
-
-        # Check if network is a config object. (Single argument passed as first positional)
-        if isinstance(network, bittensor.config):
-            if network.subtensor is None:
-                bittensor.logging.warning(
-                    "If passing a bittensor config object, it must not be empty. Using default subtensor config."
-                )
-                config = None
-            else:
-                config = network
-            network = None
-
-        if config is None:
-            config = subtensor.config()
-        self.config = copy.deepcopy(config)  # type: ignore
-
-        # Setup config.subtensor.network and config.subtensor.chain_endpoint
-        self.chain_endpoint, self.network = subtensor.setup_config(network, config)  # type: ignore
-
-        if (
-            self.network == "finney"
-            or self.chain_endpoint == bittensor.__finney_entrypoint__
-        ) and log_verbose:
-            bittensor.logging.info(
-                f"You are connecting to {self.network} network with endpoint {self.chain_endpoint}."
-            )
-            bittensor.logging.warning(
-                "We strongly encourage running a local subtensor node whenever possible. "
-                "This increases decentralization and resilience of the network."
-            )
-            bittensor.logging.warning(
-                "In a future release, local subtensor will become the default endpoint. "
-                "To get ahead of this change, please run a local subtensor node and point to it."
-            )
-
-        # Returns a mocked connection with a background chain connection.
-        self.config.subtensor._mock = (
-            _mock
-            if _mock != None
-            else self.config.subtensor.get("_mock", bittensor.defaults.subtensor._mock)
-        )
-        if (
-            self.config.subtensor._mock
-        ):  # TODO: review this doesn't appear to be used anywhere.
-            config.subtensor._mock = True
-            return bittensor.MockSubtensor()  # type: ignore
-
-        # Attempt to connect to chosen endpoint. Fallback to finney if local unavailable.
-        try:
-            # Set up params.
-            self.substrate = SubstrateInterface(
-                ss58_format=bittensor.__ss58_format__,
-                use_remote_preset=True,
-                url=self.chain_endpoint,
-                type_registry=bittensor.__type_registry__,
-            )
-        except ConnectionRefusedError as e:
-            bittensor.logging.error(
-                f"Could not connect to {self.network} network with {self.chain_endpoint} chain endpoint. Exiting..."
-            )
-            bittensor.logging.info(
-                f"You can check if you have connectivity by runing this command: nc -vz localhost {self.chain_endpoint.split(':')[2]}"
-            )
-            exit(1)
-            # TODO (edu/phil): Advise to run local subtensor and point to dev docs.
-
-        try:
-            self.substrate.websocket.settimeout(600)
-        except:
-            bittensor.logging.warning("Could not set websocket timeout.")
-
-        if log_verbose:
-            bittensor.logging.info(
-                f"Connected to {self.network} network and {self.chain_endpoint}."
-            )
-
-    def __str__(self) -> str:
-        if self.network == self.chain_endpoint:
-            # Connecting to chain endpoint without network known.
-            return "subtensor({})".format(self.chain_endpoint)
-        else:
-            # Connecting to network with endpoint known.
-            return "subtensor({}, {})".format(self.network, self.chain_endpoint)
-
-    def __repr__(self) -> str:
-        return self.__str__()
-
-    ####################
-    #### SubstrateInterface related
-    ####################
-    def connect_websocket(self):
-        """
-        (Re)creates the websocket connection, if the URL contains a 'ws' or 'wss' scheme
-        """
-        self.subtensor.connect_websocket
-
     def close(self):
-        """
-        Cleans up resources for this subtensor instance like active websocket connection and active extensions
-        """
+        """Cleans up resources for this subtensor instance like active websocket connection and active extensions."""
         self.substrate.close()
 
-    #####################
-    #### Delegation #####
-    #####################
+    ##############
+    # Delegation #
+    ##############
     def nominate(
         self,
-        wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
         wait_for_finalization: bool = False,
         wait_for_inclusion: bool = True,
     ) -> bool:
         """
         Becomes a delegate for the hotkey associated with the given wallet. This method is used to nominate
         a neuron (identified by the hotkey in the wallet) as a delegate on the Bittensor network, allowing it
         to participate in consensus and validation processes.
 
         Args:
             wallet (bittensor.wallet): The wallet containing the hotkey to be nominated.
-            wait_for_finalization (bool, optional): If ``True``, waits until the transaction is finalized on the blockchain.
+            wait_for_finalization (bool, optional): If ``True``, waits until the transaction is finalized on the
+                blockchain.
             wait_for_inclusion (bool, optional): If ``True``, waits until the transaction is included in a block.
 
         Returns:
             bool: ``True`` if the nomination process is successful, ``False`` otherwise.
 
         This function is a key part of the decentralized governance mechanism of Bittensor, allowing for the
         dynamic selection and participation of validators in the network's consensus process.
@@ -468,30 +530,34 @@
             wallet=wallet,
             wait_for_finalization=wait_for_finalization,
             wait_for_inclusion=wait_for_inclusion,
         )
 
     def delegate(
         self,
-        wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
         delegate_ss58: Optional[str] = None,
         amount: Optional[Union[Balance, float]] = None,
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
         """
         Becomes a delegate for the hotkey associated with the given wallet. This method is used to nominate
         a neuron (identified by the hotkey in the wallet) as a delegate on the Bittensor network, allowing it
         to participate in consensus and validation processes.
 
         Args:
             wallet (bittensor.wallet): The wallet containing the hotkey to be nominated.
-            wait_for_finalization (bool, optional): If ``True``, waits until the transaction is finalized on the blockchain.
+            delegate_ss58 (Optional[str]): The ``SS58`` address of the delegate neuron.
+            amount (Union[Balance, float]): The amount of TAO to undelegate.
+            wait_for_finalization (bool, optional): If ``True``, waits until the transaction is finalized on the
+                blockchain.
             wait_for_inclusion (bool, optional): If ``True``, waits until the transaction is included in a block.
+            prompt (bool, optional): If ``True``, prompts for user confirmation before proceeding.
 
         Returns:
             bool: ``True`` if the nomination process is successful, False otherwise.
 
         This function is a key part of the decentralized governance mechanism of Bittensor, allowing for the
         dynamic selection and participation of validators in the network's consensus process.
         """
@@ -503,15 +569,15 @@
             wait_for_inclusion=wait_for_inclusion,
             wait_for_finalization=wait_for_finalization,
             prompt=prompt,
         )
 
     def undelegate(
         self,
-        wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
         delegate_ss58: Optional[str] = None,
         amount: Optional[Union[Balance, float]] = None,
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
         """
@@ -538,17 +604,82 @@
             delegate_ss58=delegate_ss58,
             amount=amount,
             wait_for_inclusion=wait_for_inclusion,
             wait_for_finalization=wait_for_finalization,
             prompt=prompt,
         )
 
+    def set_take(
+        self,
+        wallet: bittensor.wallet,
+        delegate_ss58: Optional[str] = None,
+        take: float = 0.0,
+        wait_for_inclusion: bool = True,
+        wait_for_finalization: bool = False,
+    ) -> bool:
+        """
+        Set delegate hotkey take
+        Args:
+            wallet (bittensor.wallet): The wallet containing the hotkey to be nominated.
+            delegate_ss58 (str, optional): Hotkey
+            take (float): Delegate take on subnet ID
+            wait_for_finalization (bool, optional): If ``True``, waits until the transaction is finalized on the
+                blockchain.
+            wait_for_inclusion (bool, optional): If ``True``, waits until the transaction is included in a block.
+
+        Returns:
+            bool: ``True`` if the process is successful, False otherwise.
+
+        This function is a key part of the decentralized governance mechanism of Bittensor, allowing for the
+        dynamic selection and participation of validators in the network's consensus process.
+        """
+        # Ensure delegate_ss58 is not None
+        if delegate_ss58 is None:
+            raise ValueError("delegate_ss58 cannot be None")
+
+        # Calculate u16 representation of the take
+        takeu16 = int(take * 0xFFFF)
+
+        # Check if the new take is greater or lower than existing take or if existing is set
+        delegate = self.get_delegate_by_hotkey(delegate_ss58)
+        current_take = None
+        if delegate is not None:
+            current_take = int(float(delegate.take) * 65535.0)
+
+        if takeu16 == current_take:
+            bittensor.__console__.print("Nothing to do, take hasn't changed")
+            return True
+        if current_take is None or current_take < takeu16:
+            bittensor.__console__.print(
+                "Current take is either not set or is lower than the new one. Will use increase_take"
+            )
+            return increase_take_extrinsic(
+                subtensor=self,
+                wallet=wallet,
+                hotkey_ss58=delegate_ss58,
+                take=takeu16,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+        else:
+            bittensor.__console__.print(
+                "Current take is higher than the new one. Will use decrease_take"
+            )
+            return decrease_take_extrinsic(
+                subtensor=self,
+                wallet=wallet,
+                hotkey_ss58=delegate_ss58,
+                take=takeu16,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+
     def send_extrinsic(
         self,
-        wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
         module: str,
         function: str,
         params: dict,
         period: int = 5,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = False,
         max_retries: int = 3,
@@ -587,14 +718,15 @@
 
         nonce = KEY_NONCE[hotkey]
 
         # <3 parity tech
         old_init_runtime = self.substrate.init_runtime
         self.substrate.init_runtime = lambda: None
         self.substrate.init_runtime = old_init_runtime
+        response = None
 
         for attempt in range(1, max_retries + 1):
             try:
                 # Create the extrinsic with new nonce
                 extrinsic = self.substrate.create_signed_extrinsic(
                     call=call,
                     keypair=wallet.hotkey,
@@ -626,53 +758,51 @@
                     nonce = nonce + 1
                     continue
 
             # This dies because user is spamming... incr and try again
             except SubstrateRequestException as e:
                 if "Priority is too low" in e.args[0]["message"]:
                     wait = min(wait_time * attempt, max_wait)
-                    bittensor.logging.warning(
+                    _logger.warning(
                         f"Priority is too low, retrying with new nonce: {nonce} in {wait} seconds."
                     )
                     nonce = nonce + 1
                     time.sleep(wait)
                     continue
                 else:
-                    bittensor.logging.error(f"Error sending extrinsic: {e}")
+                    _logger.error(f"Error sending extrinsic: {e}")
                     response = None
 
         return response
 
-    #####################
-    #### Set Weights ####
-    #####################
+    ###############
+    # Set Weights #
+    ###############
     def set_weights(
         self,
-        wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
         netuid: int,
-        uids: Union[torch.LongTensor, list],
-        weights: Union[torch.FloatTensor, list],
+        uids: Union[NDArray[np.int64], "torch.LongTensor", list],
+        weights: Union[NDArray[np.float32], "torch.FloatTensor", list],
         version_key: int = bittensor.__version_as_int__,
-        uid: Optional[int] = None,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = False,
         prompt: bool = False,
         max_retries: int = 5,
     ) -> Tuple[bool, str]:
         """
         Sets the inter-neuronal weights for the specified neuron. This process involves specifying the
         influence or trust a neuron places on other neurons in the network, which is a fundamental aspect
         of Bittensor's decentralized learning architecture.
 
         Args:
             wallet (bittensor.wallet): The wallet associated with the neuron setting the weights.
             netuid (int): The unique identifier of the subnet.
-            uid (int): Unique identifier for the caller on the subnet specified by `netuid`.
-            uids (Union[torch.LongTensor, list]): The list of neuron UIDs that the weights are being set for.
-            weights (Union[torch.FloatTensor, list]): The corresponding weights to be set for each UID.
+            uids (Union[NDArray[np.int64], torch.LongTensor, list]): The list of neuron UIDs that the weights are being set for.
+            weights (Union[NDArray[np.float32], torch.FloatTensor, list]): The corresponding weights to be set for each UID.
             version_key (int, optional): Version key for compatibility with the network.
             wait_for_inclusion (bool, optional): Waits for the transaction to be included in a block.
             wait_for_finalization (bool, optional): Waits for the transaction to be finalized on the blockchain.
             prompt (bool, optional): If ``True``, prompts for user confirmation before proceeding.
             max_retries (int, optional): The number of maximum attempts to set weights. (Default: 5)
 
         Returns:
@@ -699,23 +829,23 @@
                     weights=weights,
                     version_key=version_key,
                     wait_for_inclusion=wait_for_inclusion,
                     wait_for_finalization=wait_for_finalization,
                     prompt=prompt,
                 )
             except Exception as e:
-                bittensor.logging.error(f"Error setting weights: {e}")
+                _logger.error(f"Error setting weights: {e}")
             finally:
                 retries += 1
 
         return success, message
 
     def _do_set_weights(
         self,
-        wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
         uids: List[int],
         vals: List[int],
         netuid: int,
         version_key: int = bittensor.__version_as_int__,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = False,
     ) -> Tuple[bool, Optional[str]]:  # (success, error_message)
@@ -736,56 +866,55 @@
         Returns:
             Tuple[bool, Optional[str]]: A tuple containing a success flag and an optional error message.
 
         This method is vital for the dynamic weighting mechanism in Bittensor, where neurons adjust their
         trust in other neurons based on observed performance and contributions.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=1, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                call = substrate.compose_call(
-                    call_module="SubtensorModule",
-                    call_function="set_weights",
-                    call_params={
-                        "dests": uids,
-                        "weights": vals,
-                        "netuid": netuid,
-                        "version_key": version_key,
-                    },
-                )
-                # Period dictates how long the extrinsic will stay as part of waiting pool
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call,
-                    keypair=wallet.hotkey,
-                    era={"period": 5},
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
-                # We only wait here if we expect finalization.
-                if not wait_for_finalization and not wait_for_inclusion:
-                    return True, "Not waiting for finalziation or inclusion."
-
-                response.process_events()
-                if response.is_success:
-                    return True, "Successfully set weights."
-                else:
-                    return False, response.error_message
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="set_weights",
+                call_params={
+                    "dests": uids,
+                    "weights": vals,
+                    "netuid": netuid,
+                    "version_key": version_key,
+                },
+            )
+            # Period dictates how long the extrinsic will stay as part of waiting pool
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call,
+                keypair=wallet.hotkey,
+                era={"period": 5},
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+            # We only wait here if we expect finalization.
+            if not wait_for_finalization and not wait_for_inclusion:
+                return True, "Not waiting for finalization or inclusion."
+
+            response.process_events()
+            if response.is_success:
+                return True, "Successfully set weights."
+            else:
+                return False, response.error_message
 
         return make_substrate_call_with_retry()
 
-    ######################
-    #### Registration ####
-    ######################
+    ################
+    # Registration #
+    ################
     def register(
         self,
-        wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
         netuid: int,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
         prompt: bool = False,
         max_allowed_attempts: int = 3,
         output_in_place: bool = True,
         cuda: bool = False,
@@ -800,16 +929,27 @@
         is a critical step for a neuron to become an active participant in the network, enabling
         it to stake, set weights, and receive incentives.
 
         Args:
             wallet (bittensor.wallet): The wallet associated with the neuron to be registered.
             netuid (int): The unique identifier of the subnet.
             wait_for_inclusion (bool, optional): Waits for the transaction to be included in a block.
+                Defaults to `False`.
             wait_for_finalization (bool, optional): Waits for the transaction to be finalized on the blockchain.
-            Other arguments: Various optional parameters to customize the registration process.
+                 Defaults to `True`.
+            prompt (bool, optional): If ``True``, prompts for user confirmation before proceeding.
+            max_allowed_attempts (int): Maximum number of attempts to register the wallet.
+            output_in_place (bool): If true, prints the progress of the proof of work to the console in-place. Meaning
+                the progress is printed on the same lines. Defaults to `True`.
+            cuda (bool): If ``true``, the wallet should be registered using CUDA device(s). Defaults to `False`.
+            dev_id (Union[List[int], int]): The CUDA device id to use, or a list of device ids. Defaults to `0` (zero).
+            tpb (int): The number of threads per block (CUDA). Default to `256`.
+            num_processes (Optional[int]): The number of processes to use to register. Default to `None`.
+            update_interval (Optional[int]): The number of nonces to solve between updates.  Default to `None`.
+            log_verbose (bool): If ``true``, the registration process will log more information.  Default to `False`.
 
         Returns:
             bool: ``True`` if the registration is successful, False otherwise.
 
         This function facilitates the entry of new neurons into the network, supporting the decentralized
         growth and scalability of the Bittensor ecosystem.
         """
@@ -828,33 +968,49 @@
             num_processes=num_processes,
             update_interval=update_interval,
             log_verbose=log_verbose,
         )
 
     def swap_hotkey(
         self,
-        wallet: "bittensor.wallet",
-        new_wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
+        new_wallet: bittensor.wallet,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
         prompt: bool = False,
     ) -> bool:
-        """Swaps an old hotkey to a new hotkey."""
+        """
+        Swaps an old hotkey with a new hotkey for the specified wallet.
+
+        This method initiates an extrinsic to change the hotkey associated with a wallet to a new hotkey. It provides
+        options to wait for inclusion and finalization of the transaction, and to prompt the user for confirmation.
+
+        Args:
+            wallet (bittensor.wallet): The wallet whose hotkey is to be swapped.
+            new_wallet (bittensor.wallet): The new wallet with the hotkey to be set.
+            wait_for_inclusion (bool): Whether to wait for the transaction to be included in a block.
+                Default is `False`.
+            wait_for_finalization (bool): Whether to wait for the transaction to be finalized. Default is `True`.
+            prompt (bool): Whether to prompt the user for confirmation before proceeding. Default is `False`.
+
+        Returns:
+            bool: True if the hotkey swap was successful, False otherwise.
+        """
         return swap_hotkey_extrinsic(
             subtensor=self,
             wallet=wallet,
             new_wallet=new_wallet,
             wait_for_inclusion=wait_for_inclusion,
             wait_for_finalization=wait_for_finalization,
             prompt=prompt,
         )
 
     def run_faucet(
         self,
-        wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
         prompt: bool = False,
         max_allowed_attempts: int = 3,
         output_in_place: bool = True,
         cuda: bool = False,
         dev_id: Union[List[int], int] = 0,
@@ -866,59 +1022,76 @@
         """
         Facilitates a faucet transaction, allowing new neurons to receive an initial amount of TAO
         for participating in the network. This function is particularly useful for newcomers to the
         Bittensor network, enabling them to start with a small stake on testnet only.
 
         Args:
             wallet (bittensor.wallet): The wallet for which the faucet transaction is to be run.
-            Other arguments: Various optional parameters to customize the faucet transaction process.
+            wait_for_inclusion (bool, optional): Waits for the transaction to be included in a block.
+                Defaults to `False`.
+            wait_for_finalization (bool, optional): Waits for the transaction to be finalized on the blockchain.
+                 Defaults to `True`.
+            prompt (bool, optional): If ``True``, prompts for user confirmation before proceeding.
+            max_allowed_attempts (int): Maximum number of attempts to register the wallet.
+            output_in_place (bool): If true, prints the progress of the proof of work to the console in-place. Meaning
+                the progress is printed on the same lines. Defaults to `True`.
+            cuda (bool): If ``true``, the wallet should be registered using CUDA device(s). Defaults to `False`.
+            dev_id (Union[List[int], int]): The CUDA device id to use, or a list of device ids. Defaults to `0` (zero).
+            tpb (int): The number of threads per block (CUDA). Default to `256`.
+            num_processes (Optional[int]): The number of processes to use to register. Default to `None`.
+            update_interval (Optional[int]): The number of nonces to solve between updates.  Default to `None`.
+            log_verbose (bool): If ``true``, the registration process will log more information.  Default to `False`.
 
         Returns:
             bool: ``True`` if the faucet transaction is successful, False otherwise.
 
         This function is part of Bittensor's onboarding process, ensuring that new neurons have
         the necessary resources to begin their journey in the decentralized AI network.
 
         Note:
-            This is for testnet ONLY and is disabled currently. You must build your own staging subtensor chain with the ``--features pow-faucet`` argument to enable this.
+            This is for testnet ONLY and is disabled currently. You must build your own staging subtensor chain with the
+            ``--features pow-faucet`` argument to enable this.
         """
-        return run_faucet_extrinsic(
+        result, _ = run_faucet_extrinsic(
             subtensor=self,
             wallet=wallet,
             wait_for_inclusion=wait_for_inclusion,
             wait_for_finalization=wait_for_finalization,
             prompt=prompt,
             max_allowed_attempts=max_allowed_attempts,
             output_in_place=output_in_place,
             cuda=cuda,
             dev_id=dev_id,
             tpb=tpb,
             num_processes=num_processes,
             update_interval=update_interval,
             log_verbose=log_verbose,
         )
+        return result
 
     def burned_register(
         self,
-        wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
         netuid: int,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
         prompt: bool = False,
     ) -> bool:
         """
         Registers a neuron on the Bittensor network by recycling TAO. This method of registration
         involves recycling TAO tokens, allowing them to be re-mined by performing work on the network.
 
         Args:
             wallet (bittensor.wallet): The wallet associated with the neuron to be registered.
             netuid (int): The unique identifier of the subnet.
             wait_for_inclusion (bool, optional): Waits for the transaction to be included in a block.
+                Defaults to `False`.
             wait_for_finalization (bool, optional): Waits for the transaction to be finalized on the blockchain.
-            prompt (bool, optional): If ``True``, prompts for user confirmation before proceeding.
+                Defaults to `True`.
+            prompt (bool, optional): If ``True``, prompts for user confirmation before proceeding. Defaults to `False`.
 
         Returns:
             bool: ``True`` if the registration is successful, False otherwise.
         """
         return burned_register_extrinsic(
             subtensor=self,
             wallet=wallet,
@@ -927,161 +1100,193 @@
             wait_for_finalization=wait_for_finalization,
             prompt=prompt,
         )
 
     def _do_pow_register(
         self,
         netuid: int,
-        wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
         pow_result: POWSolution,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
     ) -> Tuple[bool, Optional[str]]:
         """Sends a (POW) register extrinsic to the chain.
 
         Args:
             netuid (int): The subnet to register on.
             wallet (bittensor.wallet): The wallet to register.
             pow_result (POWSolution): The PoW result to register.
-            wait_for_inclusion (bool): If ``true``, waits for the extrinsic to be included in a block.
-            wait_for_finalization (bool): If ``true``, waits for the extrinsic to be finalized.
+            wait_for_inclusion (bool): If ``True``, waits for the extrinsic to be included in a block.
+                Default to `False`.
+            wait_for_finalization (bool): If ``True``, waits for the extrinsic to be finalized. Default to `True`.
+
         Returns:
             success (bool): ``True`` if the extrinsic was included in a block.
-            error (Optional[str]): ``None`` on success or not waiting for inclusion/finalization, otherwise the error message.
+            error (Optional[str]): ``None`` on success or not waiting for inclusion/finalization, otherwise the error
+                message.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=1, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                # create extrinsic call
-                call = substrate.compose_call(
-                    call_module="SubtensorModule",
-                    call_function="register",
-                    call_params={
-                        "netuid": netuid,
-                        "block_number": pow_result.block_number,
-                        "nonce": pow_result.nonce,
-                        "work": [int(byte_) for byte_ in pow_result.seal],
-                        "hotkey": wallet.hotkey.ss58_address,
-                        "coldkey": wallet.coldkeypub.ss58_address,
-                    },
-                )
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call, keypair=wallet.hotkey
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
-
-                # We only wait here if we expect finalization.
-                if not wait_for_finalization and not wait_for_inclusion:
-                    return True, None
+            # create extrinsic call
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="register",
+                call_params={
+                    "netuid": netuid,
+                    "block_number": pow_result.block_number,
+                    "nonce": pow_result.nonce,
+                    "work": [int(byte_) for byte_ in pow_result.seal],
+                    "hotkey": wallet.hotkey.ss58_address,
+                    "coldkey": wallet.coldkeypub.ss58_address,
+                },
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.hotkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
 
-                # process if registration successful, try again if pow is still valid
-                response.process_events()
-                if not response.is_success:
-                    return False, response.error_message
-                # Successful registration
-                else:
-                    return True, None
+            # We only wait here if we expect finalization.
+            if not wait_for_finalization and not wait_for_inclusion:
+                return True, None
+
+            # process if registration successful, try again if pow is still valid
+            response.process_events()
+            if not response.is_success:
+                return False, response.error_message
+            # Successful registration
+            else:
+                return True, None
 
         return make_substrate_call_with_retry()
 
     def _do_burned_register(
         self,
         netuid: int,
-        wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
     ) -> Tuple[bool, Optional[str]]:
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
-        def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                # create extrinsic call
-                call = substrate.compose_call(
-                    call_module="SubtensorModule",
-                    call_function="burned_register",
-                    call_params={
-                        "netuid": netuid,
-                        "hotkey": wallet.hotkey.ss58_address,
-                    },
-                )
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call, keypair=wallet.coldkey
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
+        """
+        Performs a burned register extrinsic call to the Subtensor chain.
 
-                # We only wait here if we expect finalization.
-                if not wait_for_finalization and not wait_for_inclusion:
-                    return True
+        This method sends a registration transaction to the Subtensor blockchain using the burned register mechanism. It
+        retries the call up to three times with exponential backoff in case of failures.
 
-                # process if registration successful, try again if pow is still valid
-                response.process_events()
-                if not response.is_success:
-                    return False, response.error_message
-                # Successful registration
-                else:
-                    return True, None
+        Args:
+            netuid (int): The network unique identifier to register on.
+            wallet (bittensor.wallet): The wallet to be registered.
+            wait_for_inclusion (bool): Whether to wait for the transaction to be included in a block. Default is False.
+            wait_for_finalization (bool): Whether to wait for the transaction to be finalized. Default is True.
+
+        Returns:
+            Tuple[bool, Optional[str]]: A tuple containing a boolean indicating success or failure, and an optional
+                error message.
+        """
+
+        @retry(delay=1, tries=3, backoff=2, max_delay=4, logger=_logger)
+        def make_substrate_call_with_retry():
+            # create extrinsic call
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="burned_register",
+                call_params={
+                    "netuid": netuid,
+                    "hotkey": wallet.hotkey.ss58_address,
+                },
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.coldkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+
+            # We only wait here if we expect finalization.
+            if not wait_for_finalization and not wait_for_inclusion:
+                return True, None
+
+            # process if registration successful, try again if pow is still valid
+            response.process_events()
+            if not response.is_success:
+                return False, response.error_message
+            # Successful registration
+            else:
+                return True, None
 
         return make_substrate_call_with_retry()
 
     def _do_swap_hotkey(
         self,
-        wallet: "bittensor.wallet",
-        new_wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
+        new_wallet: bittensor.wallet,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
     ) -> Tuple[bool, Optional[str]]:
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
-        def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                # create extrinsic call
-                call = substrate.compose_call(
-                    call_module="SubtensorModule",
-                    call_function="swap_hotkey",
-                    call_params={
-                        "hotkey": wallet.hotkey.ss58_address,
-                        "new_hotkey": new_wallet.hotkey.ss58_address,
-                    },
-                )
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call, keypair=wallet.coldkey
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
+        """
+        Performs a hotkey swap extrinsic call to the Subtensor chain.
 
-                # We only wait here if we expect finalization.
-                if not wait_for_finalization and not wait_for_inclusion:
-                    return True
+        Args:
+            wallet (bittensor.wallet): The wallet whose hotkey is to be swapped.
+            new_wallet (bittensor.wallet): The wallet with the new hotkey to be set.
+            wait_for_inclusion (bool): Whether to wait for the transaction to be included in a block. Default is
+            `False`.
+            wait_for_finalization (bool): Whether to wait for the transaction to be finalized. Default is `True`.
 
-                # process if registration successful, try again if pow is still valid
-                response.process_events()
-                if not response.is_success:
-                    return False, response.error_message
-                # Successful registration
-                else:
-                    return True, None
+        Returns:
+            Tuple[bool, Optional[str]]: A tuple containing a boolean indicating success or failure, and an optional
+                error message.
+        """
+
+        @retry(delay=1, tries=3, backoff=2, max_delay=4, logger=_logger)
+        def make_substrate_call_with_retry():
+            # create extrinsic call
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="swap_hotkey",
+                call_params={
+                    "hotkey": wallet.hotkey.ss58_address,
+                    "new_hotkey": new_wallet.hotkey.ss58_address,
+                },
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.coldkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+
+            # We only wait here if we expect finalization.
+            if not wait_for_finalization and not wait_for_inclusion:
+                return True, None
+
+            # process if registration successful, try again if pow is still valid
+            response.process_events()
+            if not response.is_success:
+                return False, response.error_message
+            # Successful registration
+            else:
+                return True, None
 
         return make_substrate_call_with_retry()
 
-    ##################
-    #### Transfer ####
-    ##################
+    ############
+    # Transfer #
+    ############
     def transfer(
         self,
-        wallet: "bittensor.wallet",
+        wallet: bittensor.wallet,
         dest: str,
         amount: Union[Balance, float],
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
         """
@@ -1094,15 +1299,15 @@
             dest (str): The destination public key address.
             amount (Union[Balance, float]): The amount of TAO to be transferred.
             wait_for_inclusion (bool, optional): Waits for the transaction to be included in a block.
             wait_for_finalization (bool, optional): Waits for the transaction to be finalized on the blockchain.
             prompt (bool, optional): If ``True``, prompts for user confirmation before proceeding.
 
         Returns:
-            bool: ``True`` if the transfer is successful, False otherwise.
+            transfer_extrinsic (bool): ``True`` if the transfer is successful, False otherwise.
 
         This function is essential for the fluid movement of tokens in the network, supporting
         various economic activities such as staking, delegation, and reward distribution.
         """
         return transfer_extrinsic(
             subtensor=self,
             wallet=wallet,
@@ -1110,59 +1315,69 @@
             amount=amount,
             wait_for_inclusion=wait_for_inclusion,
             wait_for_finalization=wait_for_finalization,
             prompt=prompt,
         )
 
     def get_transfer_fee(
-        self, wallet: "bittensor.wallet", dest: str, value: Union[Balance, float, int]
+        self, wallet: bittensor.wallet, dest: str, value: Union[Balance, float, int]
     ) -> Balance:
         """
         Calculates the transaction fee for transferring tokens from a wallet to a specified destination address.
         This function simulates the transfer to estimate the associated cost, taking into account the current
         network conditions and transaction complexity.
 
         Args:
             wallet (bittensor.wallet): The wallet from which the transfer is initiated.
             dest (str): The ``SS58`` address of the destination account.
-            value (Union[Balance, float, int]): The amount of tokens to be transferred, specified as a Balance object, or in Tao (float) or Rao (int) units.
+            value (Union[Balance, float, int]): The amount of tokens to be transferred, specified as a Balance object,
+                or in Tao (float) or Rao (int) units.
 
         Returns:
             Balance: The estimated transaction fee for the transfer, represented as a Balance object.
 
         Estimating the transfer fee is essential for planning and executing token transactions, ensuring that the
         wallet has sufficient funds to cover both the transfer amount and the associated costs. This function
         provides a crucial tool for managing financial operations within the Bittensor network.
         """
         if isinstance(value, float):
-            transfer_balance = Balance.from_tao(value)
+            value = Balance.from_tao(value)
         elif isinstance(value, int):
-            transfer_balance = Balance.from_rao(value)
+            value = Balance.from_rao(value)
 
-        with self.substrate as substrate:
-            call = substrate.compose_call(
+        if isinstance(value, Balance):
+            call = self.substrate.compose_call(
                 call_module="Balances",
-                call_function="transfer",
-                call_params={"dest": dest, "value": transfer_balance.rao},
+                call_function="transfer_allow_death",
+                call_params={"dest": dest, "value": value.rao},
             )
 
             try:
-                payment_info = substrate.get_payment_info(
+                payment_info = self.substrate.get_payment_info(
                     call=call, keypair=wallet.coldkeypub
                 )
             except Exception as e:
                 bittensor.__console__.print(
                     ":cross_mark: [red]Failed to get payment info[/red]:[bold white]\n  {}[/bold white]".format(
                         e
                     )
                 )
-                payment_info = {"partialFee": 2e7}  # assume  0.02 Tao
+                payment_info = {"partialFee": int(2e7)}  # assume  0.02 Tao
 
-        fee = Balance.from_rao(payment_info["partialFee"])
-        return fee
+            fee = Balance.from_rao(payment_info["partialFee"])
+            return fee
+        else:
+            fee = Balance.from_rao(int(2e7))
+            _logger.error(
+                "To calculate the transaction fee, the value must be Balance, float, or int. Received type: %s. Fee "
+                "is %s",
+                type(value),
+                2e7,
+            )
+            return fee
 
     def _do_transfer(
         self,
         wallet: "bittensor.wallet",
         dest: str,
         transfer_balance: Balance,
         wait_for_inclusion: bool = True,
@@ -1178,41 +1393,40 @@
             wait_for_finalization (bool): If ``true``, waits for finalization.
         Returns:
             success (bool): ``True`` if transfer was successful.
             block_hash (str): Block hash of the transfer. On success and if wait_for_ finalization/inclusion is ``True``.
             error (str): Error message if transfer failed.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                call = substrate.compose_call(
-                    call_module="Balances",
-                    call_function="transfer",
-                    call_params={"dest": dest, "value": transfer_balance.rao},
-                )
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call, keypair=wallet.coldkey
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
-                # We only wait here if we expect finalization.
-                if not wait_for_finalization and not wait_for_inclusion:
-                    return True, None, None
-
-                # Otherwise continue with finalization.
-                response.process_events()
-                if response.is_success:
-                    block_hash = response.block_hash
-                    return True, block_hash, None
-                else:
-                    return False, None, response.error_message
+            call = self.substrate.compose_call(
+                call_module="Balances",
+                call_function="transfer_allow_death",
+                call_params={"dest": dest, "value": transfer_balance.rao},
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.coldkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+            # We only wait here if we expect finalization.
+            if not wait_for_finalization and not wait_for_inclusion:
+                return True, None, None
+
+            # Otherwise continue with finalization.
+            response.process_events()
+            if response.is_success:
+                block_hash = response.block_hash
+                return True, block_hash, None
+            else:
+                return False, None, response.error_message
 
         return make_substrate_call_with_retry()
 
     def get_existential_deposit(self, block: Optional[int] = None) -> Optional[Balance]:
         """
         Retrieves the existential deposit amount for the Bittensor blockchain. The existential deposit
         is the minimum amount of TAO required for an account to exist on the blockchain. Accounts with
@@ -1413,38 +1627,37 @@
         Returns:
             Tuple[bool, Optional[str]]: A tuple containing a success flag and an optional error message.
 
         This function is crucial for initializing and announcing a neuron's Axon service on the network,
         enhancing the decentralized computation capabilities of Bittensor.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                call = substrate.compose_call(
-                    call_module="SubtensorModule",
-                    call_function="serve_axon",
-                    call_params=call_params,
-                )
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call, keypair=wallet.hotkey
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
-                if wait_for_inclusion or wait_for_finalization:
-                    response.process_events()
-                    if response.is_success:
-                        return True, None
-                    else:
-                        return False, response.error_message
-                else:
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="serve_axon",
+                call_params=call_params,
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.hotkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+            if wait_for_inclusion or wait_for_finalization:
+                response.process_events()
+                if response.is_success:
                     return True, None
+                else:
+                    return False, response.error_message
+            else:
+                return True, None
 
         return make_substrate_call_with_retry()
 
     def serve_prometheus(
         self,
         wallet: "bittensor.wallet",
         port: int,
@@ -1476,38 +1689,37 @@
             wait_for_inclusion (bool): If ``true``, waits for inclusion.
             wait_for_finalization (bool): If ``true``, waits for finalization.
         Returns:
             success (bool): ``True`` if serve prometheus was successful.
             error (:func:`Optional[str]`): Error message if serve prometheus failed, ``None`` otherwise.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                call = substrate.compose_call(
-                    call_module="SubtensorModule",
-                    call_function="serve_prometheus",
-                    call_params=call_params,
-                )
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call, keypair=wallet.hotkey
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
-                if wait_for_inclusion or wait_for_finalization:
-                    response.process_events()
-                    if response.is_success:
-                        return True, None
-                    else:
-                        return False, response.error_message
-                else:
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="serve_prometheus",
+                call_params=call_params,
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.hotkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+            if wait_for_inclusion or wait_for_finalization:
+                response.process_events()
+                if response.is_success:
                     return True, None
+                else:
+                    return False, response.error_message
+            else:
+                return True, None
 
         return make_substrate_call_with_retry()
 
     def _do_associate_ips(
         self,
         wallet: "bittensor.wallet",
         ip_info_list: List[IPInfo],
@@ -1526,41 +1738,40 @@
             wait_for_finalization (bool): If ``true``, waits for finalization.
 
         Returns:
             success (bool): ``True`` if associate IPs was successful.
             error (:func:`Optional[str]`): Error message if associate IPs failed, None otherwise.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                call = substrate.compose_call(
-                    call_module="SubtensorModule",
-                    call_function="associate_ips",
-                    call_params={
-                        "ip_info_list": [ip_info.encode() for ip_info in ip_info_list],
-                        "netuid": netuid,
-                    },
-                )
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call, keypair=wallet.hotkey
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
-                if wait_for_inclusion or wait_for_finalization:
-                    response.process_events()
-                    if response.is_success:
-                        return True, None
-                    else:
-                        return False, response.error_message
-                else:
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="associate_ips",
+                call_params={
+                    "ip_info_list": [ip_info.encode() for ip_info in ip_info_list],
+                    "netuid": netuid,
+                },
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.hotkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+            if wait_for_inclusion or wait_for_finalization:
+                response.process_events()
+                if response.is_success:
                     return True, None
+                else:
+                    return False, response.error_message
+            else:
+                return True, None
 
         return make_substrate_call_with_retry()
 
     #################
     #### Staking ####
     #################
     def add_stake(
@@ -1656,39 +1867,38 @@
             wait_for_finalization (bool): If ``true``, waits for finalization before returning.
         Returns:
             success (bool): ``True`` if the extrinsic was successful.
         Raises:
             StakeError: If the extrinsic failed.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                call = substrate.compose_call(
-                    call_module="SubtensorModule",
-                    call_function="add_stake",
-                    call_params={"hotkey": hotkey_ss58, "amount_staked": amount.rao},
-                )
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call, keypair=wallet.coldkey
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
-                # We only wait here if we expect finalization.
-                if not wait_for_finalization and not wait_for_inclusion:
-                    return True
-
-                response.process_events()
-                if response.is_success:
-                    return True
-                else:
-                    raise StakeError(response.error_message)
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="add_stake",
+                call_params={"hotkey": hotkey_ss58, "amount_staked": amount.rao},
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.coldkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+            # We only wait here if we expect finalization.
+            if not wait_for_finalization and not wait_for_inclusion:
+                return True
+
+            response.process_events()
+            if response.is_success:
+                return True
+            else:
+                raise StakeError(response.error_message)
 
         return make_substrate_call_with_retry()
 
     ###################
     #### Unstaking ####
     ###################
     def unstake_multiple(
@@ -1783,39 +1993,38 @@
             wait_for_finalization (bool): If ``true``, waits for finalization before returning.
         Returns:
             success (bool): ``True`` if the extrinsic was successful.
         Raises:
             StakeError: If the extrinsic failed.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                call = substrate.compose_call(
-                    call_module="SubtensorModule",
-                    call_function="remove_stake",
-                    call_params={"hotkey": hotkey_ss58, "amount_unstaked": amount.rao},
-                )
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call, keypair=wallet.coldkey
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
-                # We only wait here if we expect finalization.
-                if not wait_for_finalization and not wait_for_inclusion:
-                    return True
-
-                response.process_events()
-                if response.is_success:
-                    return True
-                else:
-                    raise StakeError(response.error_message)
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="remove_stake",
+                call_params={"hotkey": hotkey_ss58, "amount_unstaked": amount.rao},
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.coldkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+            # We only wait here if we expect finalization.
+            if not wait_for_finalization and not wait_for_inclusion:
+                return True
+
+            response.process_events()
+            if response.is_success:
+                return True
+            else:
+                raise StakeError(response.error_message)
 
         return make_substrate_call_with_retry()
 
     ################
     #### Senate ####
     ################
 
@@ -2102,64 +2311,64 @@
 
     def _do_root_register(
         self,
         wallet: "bittensor.wallet",
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = True,
     ) -> Tuple[bool, Optional[str]]:
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                # create extrinsic call
-                call = substrate.compose_call(
-                    call_module="SubtensorModule",
-                    call_function="root_register",
-                    call_params={"hotkey": wallet.hotkey.ss58_address},
-                )
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call, keypair=wallet.coldkey
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
-
-                # We only wait here if we expect finalization.
-                if not wait_for_finalization and not wait_for_inclusion:
-                    return True
+            # create extrinsic call
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="root_register",
+                call_params={"hotkey": wallet.hotkey.ss58_address},
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.coldkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
 
-                # process if registration successful, try again if pow is still valid
-                response.process_events()
-                if not response.is_success:
-                    return False, response.error_message
-                # Successful registration
-                else:
-                    return True, None
+            # We only wait here if we expect finalization.
+            if not wait_for_finalization and not wait_for_inclusion:
+                return True
+
+            # process if registration successful, try again if pow is still valid
+            response.process_events()
+            if not response.is_success:
+                return False, response.error_message
+            # Successful registration
+            else:
+                return True, None
 
         return make_substrate_call_with_retry()
 
+    @legacy_torch_api_compat
     def root_set_weights(
         self,
         wallet: "bittensor.wallet",
-        netuids: Union[torch.LongTensor, list],
-        weights: Union[torch.FloatTensor, list],
+        netuids: Union[NDArray[np.int64], "torch.LongTensor", list],
+        weights: Union[NDArray[np.float32], "torch.FloatTensor", list],
         version_key: int = 0,
         wait_for_inclusion: bool = False,
         wait_for_finalization: bool = False,
         prompt: bool = False,
     ) -> bool:
         """
         Sets the weights for neurons on the root network. This action is crucial for defining the influence
         and interactions of neurons at the root level of the Bittensor network.
 
         Args:
             wallet (bittensor.wallet): The wallet associated with the neuron setting the weights.
-            netuids (Union[torch.LongTensor, list]): The list of neuron UIDs for which weights are being set.
-            weights (Union[torch.FloatTensor, list]): The corresponding weights to be set for each UID.
+            netuids (Union[NDArray[np.int64], torch.LongTensor, list]): The list of neuron UIDs for which weights are being set.
+            weights (Union[NDArray[np.float32], torch.FloatTensor, list]): The corresponding weights to be set for each UID.
             version_key (int, optional): Version key for compatibility with the network.
             wait_for_inclusion (bool, optional): Waits for the transaction to be included in a block.
             wait_for_finalization (bool, optional): Waits for the transaction to be finalized on the blockchain.
             prompt (bool, optional): If ``True``, prompts for user confirmation before proceeding.
 
         Returns:
             bool: ``True`` if the setting of root-level weights is successful, False otherwise.
@@ -2204,25 +2413,24 @@
         Returns:
             Optional[object]: An object containing the identity information of the neuron if found, ``None`` otherwise.
 
         The identity information can include various attributes such as the neuron's stake, rank, and other
         network-specific details, providing insights into the neuron's role and status within the Bittensor network.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                return substrate.query(
-                    module="Registry",
-                    storage_function="IdentityOf",
-                    params=[key],
-                    block_hash=(
-                        None if block is None else substrate.get_block_hash(block)
-                    ),
-                )
+            return self.substrate.query(
+                module="Registry",
+                storage_function="IdentityOf",
+                params=[key],
+                block_hash=(
+                    None if block is None else self.substrate.get_block_hash(block)
+                ),
+            )
 
         identity_info = make_substrate_call_with_retry()
         return bittensor.utils.wallet_utils.decode_hex_identity_dict(
             identity_info.value["info"]
         )
 
     def update_identity(
@@ -2255,49 +2463,48 @@
         """
         if identified is None:
             identified = wallet.coldkey.ss58_address
 
         call_params = bittensor.utils.wallet_utils.create_identity_dict(**params)
         call_params["identified"] = identified
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                call = substrate.compose_call(
-                    call_module="Registry",
-                    call_function="set_identity",
-                    call_params=call_params,
-                )
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call, keypair=wallet.coldkey
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
-                # We only wait here if we expect finalization.
-                if not wait_for_finalization and not wait_for_inclusion:
-                    return True
-                response.process_events()
-                if response.is_success:
-                    return True
-                else:
-                    raise IdentityError(response.error_message)
+            call = self.substrate.compose_call(
+                call_module="Registry",
+                call_function="set_identity",
+                call_params=call_params,
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.coldkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+            # We only wait here if we expect finalization.
+            if not wait_for_finalization and not wait_for_inclusion:
+                return True
+            response.process_events()
+            if response.is_success:
+                return True
+            else:
+                raise IdentityError(response.error_message)
 
         return make_substrate_call_with_retry()
 
     """ Make some commitment on-chain about arbitary data """
 
     def commit(self, wallet, netuid: int, data: str):
         publish_metadata(self, wallet, netuid, f"Raw{len(data)}", data.encode())
 
     def get_commitment(self, netuid: int, uid: int, block: Optional[int] = None) -> str:
         metagraph = self.metagraph(netuid)
-        hotkey = metagraph.hotkeys[uid]
+        hotkey = metagraph.hotkeys[uid]  # type: ignore
 
         metadata = get_metadata(self, netuid, hotkey, block)
         commitment = metadata["info"]["fields"][0]  # type: ignore
         hex_data = commitment[list(commitment.keys())[0]][2:]  # type: ignore
 
         return bytes.fromhex(hex_data).decode()
 
@@ -2325,25 +2532,24 @@
         Returns:
             Optional[object]: An object containing the requested data if found, ``None`` otherwise.
 
         This query function is essential for accessing detailed information about the network and its neurons,
         providing valuable insights into the state and dynamics of the Bittensor ecosystem.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                return substrate.query(
-                    module="SubtensorModule",
-                    storage_function=name,
-                    params=params,
-                    block_hash=(
-                        None if block is None else substrate.get_block_hash(block)
-                    ),
-                )
+            return self.substrate.query(
+                module="SubtensorModule",
+                storage_function=name,
+                params=params,
+                block_hash=(
+                    None if block is None else self.substrate.get_block_hash(block)
+                ),
+            )
 
         return make_substrate_call_with_retry()
 
     """ Queries subtensor map storage with params and block. """
 
     def query_map_subtensor(
         self,
@@ -2363,25 +2569,24 @@
         Returns:
             QueryMapResult: An object containing the map-like data structure, or ``None`` if not found.
 
         This function is particularly useful for analyzing and understanding complex network structures and
         relationships within the Bittensor ecosystem, such as inter-neuronal connections and stake distributions.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                return substrate.query_map(
-                    module="SubtensorModule",
-                    storage_function=name,
-                    params=params,
-                    block_hash=(
-                        None if block is None else substrate.get_block_hash(block)
-                    ),
-                )
+            return self.substrate.query_map(
+                module="SubtensorModule",
+                storage_function=name,
+                params=params,
+                block_hash=(
+                    None if block is None else self.substrate.get_block_hash(block)
+                ),
+            )
 
         return make_substrate_call_with_retry()
 
     def query_constant(
         self, module_name: str, constant_name: str, block: Optional[int] = None
     ) -> Optional[object]:
         """
@@ -2398,24 +2603,23 @@
             Optional[object]: The value of the constant if found, ``None`` otherwise.
 
         Constants queried through this function can include critical network parameters such as inflation rates,
         consensus rules, or validation thresholds, providing a deeper understanding of the Bittensor network's
         operational parameters.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                return substrate.get_constant(
-                    module_name=module_name,
-                    constant_name=constant_name,
-                    block_hash=(
-                        None if block is None else substrate.get_block_hash(block)
-                    ),
-                )
+            return self.substrate.get_constant(
+                module_name=module_name,
+                constant_name=constant_name,
+                block_hash=(
+                    None if block is None else self.substrate.get_block_hash(block)
+                ),
+            )
 
         return make_substrate_call_with_retry()
 
     """ Queries any module storage with params and block. """
 
     def query_module(
         self,
@@ -2438,25 +2642,24 @@
         Returns:
             Optional[object]: An object containing the requested data if found, ``None`` otherwise.
 
         This versatile query function is key to accessing a wide range of data and insights from different
         parts of the Bittensor blockchain, enhancing the understanding and analysis of the network's state and dynamics.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                return substrate.query(
-                    module=module,
-                    storage_function=name,
-                    params=params,
-                    block_hash=(
-                        None if block is None else substrate.get_block_hash(block)
-                    ),
-                )
+            return self.substrate.query(
+                module=module,
+                storage_function=name,
+                params=params,
+                block_hash=(
+                    None if block is None else self.substrate.get_block_hash(block)
+                ),
+            )
 
         return make_substrate_call_with_retry()
 
     """ Queries any module map storage with params and block. """
 
     def query_map(
         self,
@@ -2478,25 +2681,24 @@
         Returns:
             Optional[object]: A data structure representing the map storage if found, ``None`` otherwise.
 
         This function is particularly useful for retrieving detailed and structured data from various blockchain
         modules, offering insights into the network's state and the relationships between its different components.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                return substrate.query_map(
-                    module=module,
-                    storage_function=name,
-                    params=params,
-                    block_hash=(
-                        None if block is None else substrate.get_block_hash(block)
-                    ),
-                )
+            return self.substrate.query_map(
+                module=module,
+                storage_function=name,
+                params=params,
+                block_hash=(
+                    None if block is None else self.substrate.get_block_hash(block)
+                ),
+            )
 
         return make_substrate_call_with_retry()
 
     def state_call(
         self,
         method: str,
         data: str,
@@ -2514,22 +2716,21 @@
         Returns:
             Optional[object]: The result of the state call if successful, ``None`` otherwise.
 
         The state call function provides a more direct and flexible way of querying blockchain data,
         useful for specific use cases where standard queries are insufficient.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                block_hash = None if block is None else substrate.get_block_hash(block)
-                params = [method, data]
-                if block_hash:
-                    params = params + [block_hash]
-                return substrate.rpc_request(method="state_call", params=params)
+            block_hash = None if block is None else self.substrate.get_block_hash(block)
+            params = [method, data]
+            if block_hash:
+                params = params + [block_hash]
+            return self.substrate.rpc_request(method="state_call", params=params)
 
         return make_substrate_call_with_retry()
 
     def query_runtime_api(
         self,
         runtime_api: str,
         method: str,
@@ -3018,15 +3219,15 @@
     def get_axon_info(
         self, netuid: int, hotkey_ss58: str, block: Optional[int] = None
     ) -> Optional[AxonInfo]:
         """Returns the axon information for this hotkey account"""
         result = self.query_subtensor("Axons", block, [netuid, hotkey_ss58])
         if result is not None and hasattr(result, "value"):
             return AxonInfo(
-                ip=bittensor.utils.networking.int_to_ip(result.value["ip"]),
+                ip=networking.int_to_ip(result.value["ip"]),
                 ip_type=result.value["ip_type"],
                 port=result.value["port"],
                 protocol=result.value["protocol"],
                 version=result.value["version"],
                 placeholder1=result.value["placeholder1"],
                 placeholder2=result.value["placeholder2"],
                 hotkey=hotkey_ss58,
@@ -3038,26 +3239,26 @@
     def get_prometheus_info(
         self, netuid: int, hotkey_ss58: str, block: Optional[int] = None
     ) -> Optional[PrometheusInfo]:
         """Returns the prometheus information for this hotkey account"""
         result = self.query_subtensor("Prometheus", block, [netuid, hotkey_ss58])
         if result is not None:
             return PrometheusInfo(
-                ip=bittensor.utils.networking.int_to_ip(result.value["ip"]),
+                ip=networking.int_to_ip(result.value["ip"]),
                 ip_type=result.value["ip_type"],
                 port=result.value["port"],
                 version=result.value["version"],
                 block=result.value["block"],
             )
         else:
             return None
 
-    ###########################
-    #### Global Parameters ####
-    ###########################
+    #####################
+    # Global Parameters #
+    #####################
 
     @property
     def block(self) -> int:
         r"""Returns current chain block.
         Returns:
             block (int):
                 Current chain block.
@@ -3105,15 +3306,15 @@
         return Balance.from_rao(_result.value)
 
     def serving_rate_limit(
         self, netuid: int, block: Optional[int] = None
     ) -> Optional[int]:
         """
         Retrieves the serving rate limit for a specific subnet within the Bittensor network.
-        This rate limit determines the maximum number of requests a neuron can serve within a given time frame.
+        This rate limit determines how often you can change your node's IP address on the blockchain. Expressed in number of blocks. Applies to both subnet validator and subnet miner nodes. Used when you move your node to a new machine.
 
         Args:
             netuid (int): The unique identifier of the subnet.
             block (Optional[int], optional): The blockchain block number at which to perform the query.
 
         Returns:
             Optional[int]: The serving rate limit of the subnet if it exists, ``None`` otherwise.
@@ -3307,25 +3508,24 @@
         Returns:
             List[SubnetInfo]: A list of SubnetInfo objects, each containing detailed information about a subnet.
 
         Gaining insights into the subnets' details assists in understanding the network's composition,
         the roles of different subnets, and their unique features.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                block_hash = None if block is None else substrate.get_block_hash(block)
-                params = []
-                if block_hash:
-                    params = params + [block_hash]
-                return substrate.rpc_request(
-                    method="subnetInfo_getSubnetsInfo",  # custom rpc method
-                    params=params,
-                )
+            block_hash = None if block is None else self.substrate.get_block_hash(block)
+            params = []
+            if block_hash:
+                params = params + [block_hash]
+            return self.substrate.rpc_request(
+                method="subnetInfo_getSubnetsInfo",  # custom rpc method
+                params=params,
+            )
 
         json_body = make_substrate_call_with_retry()
         result = json_body["result"]
 
         if result in (None, []):
             return []
 
@@ -3345,25 +3545,24 @@
         Returns:
             Optional[SubnetInfo]: Detailed information about the subnet, or ``None`` if not found.
 
         This function is essential for neurons and stakeholders interested in the specifics of a particular
         subnet, including its governance, performance, and role within the broader network.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                block_hash = None if block is None else substrate.get_block_hash(block)
-                params = [netuid]
-                if block_hash:
-                    params = params + [block_hash]
-                return substrate.rpc_request(
-                    method="subnetInfo_getSubnetInfo",  # custom rpc method
-                    params=params,
-                )
+            block_hash = None if block is None else self.substrate.get_block_hash(block)
+            params = [netuid]
+            if block_hash:
+                params = params + [block_hash]
+            return self.substrate.rpc_request(
+                method="subnetInfo_getSubnetInfo",  # custom rpc method
+                params=params,
+            )
 
         json_body = make_substrate_call_with_retry()
         result = json_body["result"]
 
         if result in (None, []):
             return None
 
@@ -3506,61 +3705,58 @@
         Returns:
             Optional[DelegateInfo]: Detailed information about the delegate neuron, ``None`` if not found.
 
         This function is essential for understanding the roles and influence of delegate neurons within
         the Bittensor network's consensus and governance structures.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry(encoded_hotkey: List[int]):
-            with self.substrate as substrate:
-                block_hash = None if block == None else substrate.get_block_hash(block)
-                params = [encoded_hotkey]
-                if block_hash:
-                    params = params + [block_hash]
-                return substrate.rpc_request(
-                    method="delegateInfo_getDelegate",  # custom rpc method
-                    params=params,
-                )
+            block_hash = None if block == None else self.substrate.get_block_hash(block)
+            params = [encoded_hotkey]
+            if block_hash:
+                params = params + [block_hash]
+            return self.substrate.rpc_request(
+                method="delegateInfo_getDelegate",  # custom rpc method
+                params=params,
+            )
 
         encoded_hotkey = ss58_to_vec_u8(hotkey_ss58)
         json_body = make_substrate_call_with_retry(encoded_hotkey)
         result = json_body["result"]
 
         if result in (None, []):
             return None
 
         return DelegateInfo.from_vec_u8(result)
 
     def get_delegates(self, block: Optional[int] = None) -> List[DelegateInfo]:
         """
-        Retrieves a list of all delegate neurons within the Bittensor network. This function provides an
-        overview of the neurons that are actively involved in the network's delegation system.
+        Retrieves a list of all delegate neurons within the Bittensor network. This function provides an overview of the neurons that are actively involved in the network's delegation system.
+
+        Analyzing the delegate population offers insights into the network's governance dynamics and the distribution of trust and responsibility among participating neurons.
 
         Args:
             block (Optional[int], optional): The blockchain block number for the query.
 
         Returns:
             List[DelegateInfo]: A list of DelegateInfo objects detailing each delegate's characteristics.
 
-        Analyzing the delegate population offers insights into the network's governance dynamics and the
-        distribution of trust and responsibility among participating neurons.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=1, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                block_hash = None if block == None else substrate.get_block_hash(block)
-                params = []
-                if block_hash:
-                    params = params + [block_hash]
-                return substrate.rpc_request(
-                    method="delegateInfo_getDelegates",  # custom rpc method
-                    params=params,
-                )
+            block_hash = None if block is None else self.substrate.get_block_hash(block)
+            params = []
+            if block_hash:
+                params.extend([block_hash])
+            return self.substrate.rpc_request(
+                method="delegateInfo_getDelegates",  # custom rpc method
+                params=params,
+            )
 
         json_body = make_substrate_call_with_retry()
         result = json_body["result"]
 
         if result in (None, []):
             return []
 
@@ -3580,25 +3776,24 @@
         Returns:
             List[Tuple[DelegateInfo, Balance]]: A list of tuples, each containing a delegate's information and staked amount.
 
         This function is important for account holders to understand their stake allocations and their
         involvement in the network's delegation and consensus mechanisms.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry(encoded_coldkey: List[int]):
-            with self.substrate as substrate:
-                block_hash = None if block == None else substrate.get_block_hash(block)
-                params = [encoded_coldkey]
-                if block_hash:
-                    params = params + [block_hash]
-                return substrate.rpc_request(
-                    method="delegateInfo_getDelegated",  # custom rpc method
-                    params=params,
-                )
+            block_hash = None if block == None else self.substrate.get_block_hash(block)
+            params = [encoded_coldkey]
+            if block_hash:
+                params = params + [block_hash]
+            return self.substrate.rpc_request(
+                method="delegateInfo_getDelegated",  # custom rpc method
+                params=params,
+            )
 
         encoded_coldkey = ss58_to_vec_u8(coldkey_ss58)
         json_body = make_substrate_call_with_retry(encoded_coldkey)
         result = json_body["result"]
 
         if result in (None, []):
             return []
@@ -3680,14 +3875,26 @@
         if hex_bytes_result.startswith("0x"):
             bytes_result = bytes.fromhex(hex_bytes_result[2:])
         else:
             bytes_result = bytes.fromhex(hex_bytes_result)
 
         return StakeInfo.list_of_tuple_from_vec_u8(bytes_result)  # type: ignore
 
+    def get_minimum_required_stake(
+        self,
+    ):
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
+        def make_substrate_call_with_retry():
+            return self.substrate.query(
+                module="SubtensorModule", storage_function="NominatorMinRequiredStake"
+            )
+
+        result = make_substrate_call_with_retry()
+        return Balance.from_rao(result.decode())
+
     ########################################
     #### Neuron information per subnet ####
     ########################################
 
     def is_hotkey_registered_any(
         self, hotkey_ss58: str, block: Optional[int] = None
     ) -> bool:
@@ -3928,24 +4135,23 @@
 
         This function is crucial for analyzing individual neurons' contributions and status within a specific
         subnet, offering insights into their roles in the network's consensus and validation mechanisms.
         """
         if uid is None:
             return NeuronInfo._null_neuron()
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                block_hash = None if block == None else substrate.get_block_hash(block)
-                params = [netuid, uid]
-                if block_hash:
-                    params = params + [block_hash]
-                return substrate.rpc_request(
-                    method="neuronInfo_getNeuron", params=params  # custom rpc method
-                )
+            block_hash = None if block == None else self.substrate.get_block_hash(block)
+            params = [netuid, uid]
+            if block_hash:
+                params = params + [block_hash]
+            return self.substrate.rpc_request(
+                method="neuronInfo_getNeuron", params=params  # custom rpc method
+            )
 
         json_body = make_substrate_call_with_retry()
         result = json_body["result"]
 
         if result in (None, []):
             return NeuronInfo._null_neuron()
 
@@ -4060,15 +4266,15 @@
         return NeuronInfoLite.list_from_vec_u8(bytes_result)  # type: ignore
 
     def metagraph(
         self,
         netuid: int,
         lite: bool = True,
         block: Optional[int] = None,
-    ) -> "bittensor.metagraph":
+    ) -> "bittensor.metagraph":  # type: ignore
         """
         Returns a synced metagraph for a specified subnet within the Bittensor network. The metagraph
         represents the network's structure, including neuron connections and interactions.
 
         Args:
             netuid (int): The network UID of the subnet to query.
             lite (bool, default=True): If true, returns a metagraph using a lightweight sync (no weights, no bonds).
@@ -4239,92 +4445,165 @@
         self,
         wallet: "bittensor.wallet",
         delegate_ss58: str,
         amount: "Balance",
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
     ) -> bool:
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                call = substrate.compose_call(
-                    call_module="SubtensorModule",
-                    call_function="add_stake",
-                    call_params={"hotkey": delegate_ss58, "amount_staked": amount.rao},
-                )
-                extrinsic = substrate.create_signed_extrinsic(
-                    call=call, keypair=wallet.coldkey
-                )
-                response = substrate.submit_extrinsic(
-                    extrinsic,
-                    wait_for_inclusion=wait_for_inclusion,
-                    wait_for_finalization=wait_for_finalization,
-                )
-                # We only wait here if we expect finalization.
-                if not wait_for_finalization and not wait_for_inclusion:
-                    return True
-                response.process_events()
-                if response.is_success:
-                    return True
-                else:
-                    raise StakeError(response.error_message)
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="add_stake",
+                call_params={"hotkey": delegate_ss58, "amount_staked": amount.rao},
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.coldkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+            # We only wait here if we expect finalization.
+            if not wait_for_finalization and not wait_for_inclusion:
+                return True
+            response.process_events()
+            if response.is_success:
+                return True
+            else:
+                raise StakeError(response.error_message)
 
         return make_substrate_call_with_retry()
 
     def _do_undelegation(
         self,
         wallet: "bittensor.wallet",
         delegate_ss58: str,
         amount: "Balance",
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
     ) -> bool:
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
+        def make_substrate_call_with_retry():
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="remove_stake",
+                call_params={
+                    "hotkey": delegate_ss58,
+                    "amount_unstaked": amount.rao,
+                },
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.coldkey
+            )
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+            # We only wait here if we expect finalization.
+            if not wait_for_finalization and not wait_for_inclusion:
+                return True
+            response.process_events()
+            if response.is_success:
+                return True
+            else:
+                raise StakeError(response.error_message)
+
+        return make_substrate_call_with_retry()
+
+    def _do_nominate(
+        self,
+        wallet: "bittensor.wallet",
+        wait_for_inclusion: bool = True,
+        wait_for_finalization: bool = False,
+    ) -> bool:
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
+        def make_substrate_call_with_retry():
+            call = self.substrate.compose_call(
+                call_module="SubtensorModule",
+                call_function="become_delegate",
+                call_params={"hotkey": wallet.hotkey.ss58_address},
+            )
+            extrinsic = self.substrate.create_signed_extrinsic(
+                call=call, keypair=wallet.coldkey
+            )  # sign with coldkey
+            response = self.substrate.submit_extrinsic(
+                extrinsic,
+                wait_for_inclusion=wait_for_inclusion,
+                wait_for_finalization=wait_for_finalization,
+            )
+            # We only wait here if we expect finalization.
+            if not wait_for_finalization and not wait_for_inclusion:
+                return True
+            response.process_events()
+            if response.is_success:
+                return True
+            else:
+                raise NominationError(response.error_message)
+
+        return make_substrate_call_with_retry()
+
+    def _do_increase_take(
+        self,
+        wallet: "bittensor.wallet",
+        hotkey_ss58: str,
+        take: int,
+        wait_for_inclusion: bool = True,
+        wait_for_finalization: bool = False,
+    ) -> bool:
         @retry(delay=2, tries=3, backoff=2, max_delay=4)
         def make_substrate_call_with_retry():
             with self.substrate as substrate:
                 call = substrate.compose_call(
                     call_module="SubtensorModule",
-                    call_function="remove_stake",
+                    call_function="increase_take",
                     call_params={
-                        "hotkey": delegate_ss58,
-                        "amount_unstaked": amount.rao,
+                        "hotkey": hotkey_ss58,
+                        "take": take,
                     },
                 )
                 extrinsic = substrate.create_signed_extrinsic(
                     call=call, keypair=wallet.coldkey
-                )
+                )  # sign with coldkey
                 response = substrate.submit_extrinsic(
                     extrinsic,
                     wait_for_inclusion=wait_for_inclusion,
                     wait_for_finalization=wait_for_finalization,
                 )
                 # We only wait here if we expect finalization.
                 if not wait_for_finalization and not wait_for_inclusion:
                     return True
                 response.process_events()
                 if response.is_success:
                     return True
                 else:
-                    raise StakeError(response.error_message)
+                    raise TakeError(response.error_message)
 
         return make_substrate_call_with_retry()
 
-    def _do_nominate(
+    def _do_decrease_take(
         self,
         wallet: "bittensor.wallet",
+        hotkey_ss58: str,
+        take: int,
         wait_for_inclusion: bool = True,
         wait_for_finalization: bool = False,
     ) -> bool:
         @retry(delay=2, tries=3, backoff=2, max_delay=4)
         def make_substrate_call_with_retry():
             with self.substrate as substrate:
                 call = substrate.compose_call(
                     call_module="SubtensorModule",
-                    call_function="become_delegate",
-                    call_params={"hotkey": wallet.hotkey.ss58_address},
+                    call_function="decrease_take",
+                    call_params={
+                        "hotkey": hotkey_ss58,
+                        "take": take,
+                    },
                 )
                 extrinsic = substrate.create_signed_extrinsic(
                     call=call, keypair=wallet.coldkey
                 )  # sign with coldkey
                 response = substrate.submit_extrinsic(
                     extrinsic,
                     wait_for_inclusion=wait_for_inclusion,
@@ -4333,15 +4612,15 @@
                 # We only wait here if we expect finalization.
                 if not wait_for_finalization and not wait_for_inclusion:
                     return True
                 response.process_events()
                 if response.is_success:
                     return True
                 else:
-                    raise NominationError(response.error_message)
+                    raise TakeError(response.error_message)
 
         return make_substrate_call_with_retry()
 
     ################
     #### Legacy ####
     ################
 
@@ -4358,30 +4637,29 @@
             Balance: The account balance at the specified block, represented as a Balance object.
 
         This function is important for monitoring account holdings and managing financial transactions
         within the Bittensor ecosystem. It helps in assessing the economic status and capacity of network participants.
         """
         try:
 
-            @retry(delay=2, tries=3, backoff=2, max_delay=4)
+            @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
             def make_substrate_call_with_retry():
-                with self.substrate as substrate:
-                    return substrate.query(
-                        module="System",
-                        storage_function="Account",
-                        params=[address],
-                        block_hash=(
-                            None if block is None else substrate.get_block_hash(block)
-                        ),
-                    )
+                return self.substrate.query(
+                    module="System",
+                    storage_function="Account",
+                    params=[address],
+                    block_hash=(
+                        None if block is None else self.substrate.get_block_hash(block)
+                    ),
+                )
 
             result = make_substrate_call_with_retry()
-        except scalecodec.exceptions.RemainingScaleBytesNotEmptyException:
-            bittensor.logging.error(
-                "Your wallet it legacy formatted, you need to run btcli stake --ammount 0 to reformat it."
+        except RemainingScaleBytesNotEmptyException:
+            _logger.error(
+                "Received a corrupted message. This likely points to an error with the network or subnet."
             )
             return Balance(1000)
         return Balance(result.value["data"]["free"])
 
     def get_current_block(self) -> int:
         """
         Returns the current block number on the Bittensor blockchain. This function provides the latest block
@@ -4390,18 +4668,17 @@
         Returns:
             int: The current chain block number.
 
         Knowing the current block number is essential for querying real-time data and performing time-sensitive
         operations on the blockchain. It serves as a reference point for network activities and data synchronization.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                return substrate.get_block_number(None)
+            return self.substrate.get_block_number(None)
 
         return make_substrate_call_with_retry()
 
     def get_balances(self, block: Optional[int] = None) -> Dict[str, Balance]:
         """
         Retrieves the token balances of all accounts within the Bittensor network as of a specific blockchain block.
         This function provides a comprehensive view of the token distribution among different accounts.
@@ -4412,24 +4689,23 @@
         Returns:
             Dict[str, Balance]: A dictionary mapping each account's ``ss58`` address to its balance.
 
         This function is valuable for analyzing the overall economic landscape of the Bittensor network,
         including the distribution of financial resources and the financial status of network participants.
         """
 
-        @retry(delay=2, tries=3, backoff=2, max_delay=4)
+        @retry(delay=2, tries=3, backoff=2, max_delay=4, logger=_logger)
         def make_substrate_call_with_retry():
-            with self.substrate as substrate:
-                return substrate.query_map(
-                    module="System",
-                    storage_function="Account",
-                    block_hash=(
-                        None if block is None else substrate.get_block_hash(block)
-                    ),
-                )
+            return self.substrate.query_map(
+                module="System",
+                storage_function="Account",
+                block_hash=(
+                    None if block is None else self.substrate.get_block_hash(block)
+                ),
+            )
 
         result = make_substrate_call_with_retry()
         return_dict = {}
         for r in result:
             bal = Balance(int(r[1]["data"]["free"].value))
             return_dict[r[0].value] = bal
         return return_dict
@@ -4473,7 +4749,24 @@
             str: The cryptographic hash of the specified block.
 
         The block hash is a fundamental aspect of blockchain technology, providing a secure reference to
         each block's data. It is crucial for verifying transactions, ensuring data consistency, and
         maintaining the trustworthiness of the blockchain.
         """
         return self.substrate.get_block_hash(block_id=block_id)
+
+    def get_error_info_by_index(self, error_index: int) -> Tuple[str, str]:
+        """Returns the error name and description from the Subtensor error list."""
+
+        unknown_error = ("Unknown Error", "")
+
+        if not self._subtensor_errors:
+            self._subtensor_errors = get_subtensor_errors(self.substrate)
+
+        name, description = self._subtensor_errors.get(str(error_index), unknown_error)
+
+        if name == unknown_error[0]:
+            _logger.warning(
+                f"Subtensor returned an error with an unknown index: {error_index}"
+            )
+
+        return name, description
```

### Comparing `bittensor-6.9.3/bittensor/synapse.py` & `bittensor-7.0.0/bittensor/synapse.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,21 @@
 # DEALINGS IN THE SOFTWARE.
 
 
 import base64
 import json
 import sys
 
-import pydantic
-from pydantic.schema import schema
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+    Field,
+    field_validator,
+    model_validator,
+)
 import bittensor
 from typing import Optional, List, Any, Dict
 
 
 def get_size(obj, seen=None) -> int:
     """
     Recursively finds size of objects.
@@ -88,15 +93,15 @@
     Returns:
         float or None: The converted float, or ``None`` if the input was ``None``.
 
     """
     return float(raw) if raw != None else raw  # type: ignore
 
 
-class TerminalInfo(pydantic.BaseModel):
+class TerminalInfo(BaseModel):
     """
     TerminalInfo encapsulates detailed information about a network synapse (node) involved in a communication process.
 
     This class serves as a metadata carrier,
     providing essential details about the state and configuration of a terminal during network interactions. This is a crucial class in the Bittensor framework.
 
     The TerminalInfo class contains information such as HTTP status codes and messages, processing times,
@@ -140,120 +145,123 @@
         processing_duration = terminal_info.process_time
 
         # TerminalInfo can be used to monitor and verify network interactions, ensuring proper communication and security within the Bittensor network.
 
     TerminalInfo plays a pivotal role in providing transparency and control over network operations, making it an indispensable tool for developers and users interacting with the Bittensor ecosystem.
     """
 
-    class Config:
-        validate_assignment = True
+    model_config = ConfigDict(validate_assignment=True)
 
     # The HTTP status code from: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status
-    status_code: Optional[int] = pydantic.Field(
+    status_code: Optional[int] = Field(
         title="status_code",
         description="The HTTP status code from: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status",
-        examples=200,
+        examples=[200],
         default=None,
-        allow_mutation=True,
+        frozen=False,
     )
-    _extract_status_code = pydantic.validator(
-        "status_code", pre=True, allow_reuse=True
-    )(cast_int)
 
     # The HTTP status code from: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status
-    status_message: Optional[str] = pydantic.Field(
+    status_message: Optional[str] = Field(
         title="status_message",
         description="The status_message associated with the status_code",
-        examples="Success",
+        examples=["Success"],
         default=None,
-        allow_mutation=True,
+        frozen=False,
     )
 
     # Process time on this terminal side of call
-    process_time: Optional[float] = pydantic.Field(
+    process_time: Optional[float] = Field(
         title="process_time",
         description="Process time on this terminal side of call",
-        examples=0.1,
+        examples=[0.1],
         default=None,
-        allow_mutation=True,
+        frozen=False,
     )
-    _extract_process_time = pydantic.validator(
-        "process_time", pre=True, allow_reuse=True
-    )(cast_float)
 
     # The terminal ip.
-    ip: Optional[str] = pydantic.Field(
+    ip: Optional[str] = Field(
         title="ip",
-        description="The ip of the axon recieving the request.",
-        examples="198.123.23.1",
+        description="The ip of the axon receiving the request.",
+        examples=["198.123.23.1"],
         default=None,
-        allow_mutation=True,
+        frozen=False,
     )
 
     # The host port of the terminal.
-    port: Optional[int] = pydantic.Field(
+    port: Optional[int] = Field(
         title="port",
         description="The port of the terminal.",
-        examples="9282",
+        examples=["9282"],
         default=None,
-        allow_mutation=True,
+        frozen=False,
     )
-    _extract_port = pydantic.validator("port", pre=True, allow_reuse=True)(cast_int)
 
     # The bittensor version on the terminal as an int.
-    version: Optional[int] = pydantic.Field(
+    version: Optional[int] = Field(
         title="version",
         description="The bittensor version on the axon as str(int)",
-        examples=111,
+        examples=[111],
         default=None,
-        allow_mutation=True,
-    )
-    _extract_version = pydantic.validator("version", pre=True, allow_reuse=True)(
-        cast_int
+        frozen=False,
     )
 
-    # A unique monotonically increasing integer nonce associate with the terminal
-    nonce: Optional[int] = pydantic.Field(
+    # A Unix timestamp to associate with the terminal
+    nonce: Optional[int] = Field(
         title="nonce",
-        description="A unique monotonically increasing integer nonce associate with the terminal generated from time.monotonic_ns()",
-        examples=111111,
+        description="A Unix timestamp that prevents replay attacks",
+        examples=[111111],
         default=None,
-        allow_mutation=True,
+        frozen=False,
     )
-    _extract_nonce = pydantic.validator("nonce", pre=True, allow_reuse=True)(cast_int)
 
     # A unique identifier associated with the terminal, set on the axon side.
-    uuid: Optional[str] = pydantic.Field(
+    uuid: Optional[str] = Field(
         title="uuid",
         description="A unique identifier associated with the terminal",
-        examples="5ecbd69c-1cec-11ee-b0dc-e29ce36fec1a",
+        examples=["5ecbd69c-1cec-11ee-b0dc-e29ce36fec1a"],
         default=None,
-        allow_mutation=True,
+        frozen=False,
     )
 
     # The bittensor version on the terminal as an int.
-    hotkey: Optional[str] = pydantic.Field(
+    hotkey: Optional[str] = Field(
         title="hotkey",
         description="The ss58 encoded hotkey string of the terminal wallet.",
-        examples="5EnjDGNqqWnuL2HCAdxeEtN2oqtXZw6BMBe936Kfy2PFz1J1",
+        examples=["5EnjDGNqqWnuL2HCAdxeEtN2oqtXZw6BMBe936Kfy2PFz1J1"],
         default=None,
-        allow_mutation=True,
+        frozen=False,
     )
 
     # A signature verifying the tuple (axon_nonce, axon_hotkey, dendrite_hotkey, axon_uuid)
-    signature: Optional[str] = pydantic.Field(
+    signature: Optional[str] = Field(
         title="signature",
         description="A signature verifying the tuple (nonce, axon_hotkey, dendrite_hotkey, uuid)",
-        examples="0x0813029319030129u4120u10841824y0182u091u230912u",
+        examples=["0x0813029319030129u4120u10841824y0182u091u230912u"],
         default=None,
-        allow_mutation=True,
+        frozen=False,
     )
 
+    # Extract the process time on this terminal side of call as a float
+    _extract_process_time = field_validator("process_time", mode="before")(cast_float)
+
+    # Extract the host port of the terminal as an int
+    _extract_port = field_validator("port", mode="before")(cast_int)
+
+    # Extract the bittensor version on the terminal as an int.
+    _extract_version = field_validator("version", mode="before")(cast_int)
+
+    # Extract the Unix timestamp associated with the terminal as an int
+    _extract_nonce = field_validator("nonce", mode="before")(cast_int)
 
-class Synapse(pydantic.BaseModel):
+    # Extract the HTTP status code as an int
+    _extract_status_code = field_validator("status_code", mode="before")(cast_int)
+
+
+class Synapse(BaseModel):
     """
     Represents a Synapse in the Bittensor network, serving as a communication schema between neurons (nodes).
 
     Synapses ensure the format and correctness of transmission tensors according to the Bittensor protocol.
     Each Synapse type is tailored for a specific machine learning (ML) task, following unique compression and
     communication processes. This helps maintain sanitized, correct, and useful information flow across the network.
 
@@ -311,15 +319,15 @@
         # Setting properties and input
         synapse.timeout = 15.0
         synapse.name = "MySynapse"
         # Not setting fields that are not defined in your synapse class will result in an error, e.g.:
         synapse.dummy_input = 1 # This will raise an error because dummy_input is not defined in the Synapse class
 
         # Get a dictionary of headers and body from the synapse instance
-        synapse_dict = synapse.json()
+        synapse_dict = synapse.model_dump_json()
 
         # Get a dictionary of headers from the synapse instance
         headers = synapse.to_headers()
 
         # Reconstruct the synapse from headers using the classmethod 'from_headers'
         synapse = Synapse.from_headers(headers)
 
@@ -353,16 +361,15 @@
         parse_headers_to_inputs: Parses headers to construct an inputs dictionary.
         from_headers: Creates an instance from a headers dictionary.
 
     This class is a cornerstone in the Bittensor framework, providing the necessary tools for secure, efficient, and
     standardized communication in a decentralized environment.
     """
 
-    class Config:
-        validate_assignment = True
+    model_config = ConfigDict(validate_assignment=True)
 
     def deserialize(self) -> "Synapse":
         """
         Deserializes the Synapse object.
 
         This method is intended to be overridden by subclasses for custom deserialization logic.
         In the context of the Synapse superclass, this method simply returns the instance itself.
@@ -383,116 +390,113 @@
                     # Custom deserialization logic
                     # For example, decoding a base64 encoded string in 'additional_data'
                     if self.additional_data:
                         self.additional_data = base64.b64decode(self.additional_data).decode('utf-8')
                     return self
 
             serialized_data = '{"additional_data": "SGVsbG8gV29ybGQ="}'  # Base64 for 'Hello World'
-            custom_synapse = CustomSynapse.parse_raw(serialized_data)
+            custom_synapse = CustomSynapse.model_validate_json(serialized_data)
             deserialized_synapse = custom_synapse.deserialize()
 
             # deserialized_synapse.additional_data would now be 'Hello World'
 
         Returns:
             Synapse: The deserialized Synapse object. In this default implementation, it returns the object itself.
         """
         return self
 
-    @pydantic.root_validator(pre=True)
+    @model_validator(mode="before")
     def set_name_type(cls, values) -> dict:
         values["name"] = cls.__name__  # type: ignore
         return values
 
     # Defines the http route name which is set on axon.attach( callable( request: RequestName ))
-    name: Optional[str] = pydantic.Field(
+    name: Optional[str] = Field(
         title="name",
         description="Defines the http route name which is set on axon.attach( callable( request: RequestName ))",
-        examples="Forward",
-        allow_mutation=True,
+        examples=["Forward"],
+        frozen=False,
         default=None,
         repr=False,
     )
 
     # The call timeout, set by the dendrite terminal.
-    timeout: Optional[float] = pydantic.Field(
+    timeout: Optional[float] = Field(
         title="timeout",
         description="Defines the total query length.",
-        examples=12.0,
+        examples=[12.0],
         default=12.0,
-        allow_mutation=True,
+        frozen=False,
         repr=False,
     )
-    _extract_timeout = pydantic.validator("timeout", pre=True, allow_reuse=True)(
-        cast_float
-    )
 
     # The call timeout, set by the dendrite terminal.
-    total_size: Optional[int] = pydantic.Field(
+    total_size: Optional[int] = Field(
         title="total_size",
         description="Total size of request body in bytes.",
-        examples=1000,
+        examples=[1000],
         default=0,
-        allow_mutation=True,
+        frozen=False,
         repr=False,
     )
-    _extract_total_size = pydantic.validator("total_size", pre=True, allow_reuse=True)(
-        cast_int
-    )
 
     # The call timeout, set by the dendrite terminal.
-    header_size: Optional[int] = pydantic.Field(
+    header_size: Optional[int] = Field(
         title="header_size",
         description="Size of request header in bytes.",
-        examples=1000,
+        examples=[1000],
         default=0,
-        allow_mutation=True,
+        frozen=False,
         repr=False,
     )
-    _extract_header_size = pydantic.validator(
-        "header_size", pre=True, allow_reuse=True
-    )(cast_int)
 
     # The dendrite Terminal Information.
-    dendrite: Optional[TerminalInfo] = pydantic.Field(
+    dendrite: Optional[TerminalInfo] = Field(
         title="dendrite",
         description="Dendrite Terminal Information",
-        examples="bittensor.TerminalInfo",
+        examples=["bittensor.TerminalInfo"],
         default=TerminalInfo(),
-        allow_mutation=True,
+        frozen=False,
         repr=False,
     )
 
     # A axon terminal information
-    axon: Optional[TerminalInfo] = pydantic.Field(
+    axon: Optional[TerminalInfo] = Field(
         title="axon",
         description="Axon Terminal Information",
-        examples="bittensor.TerminalInfo",
+        examples=["bittensor.TerminalInfo"],
         default=TerminalInfo(),
-        allow_mutation=True,
+        frozen=False,
         repr=False,
     )
 
-    computed_body_hash: Optional[str] = pydantic.Field(
+    computed_body_hash: Optional[str] = Field(
         title="computed_body_hash",
         description="The computed body hash of the request.",
-        examples="0x0813029319030129u4120u10841824y0182u091u230912u",
+        examples=["0x0813029319030129u4120u10841824y0182u091u230912u"],
         default="",
-        allow_mutation=False,
+        frozen=True,
         repr=False,
     )
 
-    required_hash_fields: Optional[List[str]] = pydantic.Field(
+    required_hash_fields: Optional[List[str]] = Field(
         title="required_hash_fields",
         description="The list of required fields to compute the body hash.",
         examples=["roles", "messages"],
         default=[],
-        allow_mutation=False,
+        frozen=True,
         repr=False,
     )
 
+    _extract_total_size = field_validator("total_size", mode="before")(cast_int)
+
+    _extract_header_size = field_validator("header_size", mode="before")(cast_int)
+
+    _extract_timeout = field_validator("timeout", mode="before")(cast_float)
+
     def __setattr__(self, name: str, value: Any):
         """
         Override the :func:`__setattr__` method to make the ``required_hash_fields`` property read-only.
 
         This is a security mechanism such that the ``required_hash_fields`` property cannot be
         overridden by the user or malicious code.
         """
@@ -576,14 +580,21 @@
         which is the HTTP status code for unauthorized access.
 
         Returns:
             bool: ``True`` if dendrite's status code is ``401``, ``False`` otherwise.
         """
         return self.dendrite is not None and self.dendrite.status_code == 401
 
+    def get_required_fields(self):
+        """
+        Get the required fields from the model's JSON schema.
+        """
+        schema = self.__class__.model_json_schema()
+        return schema.get("required", [])
+
     def to_headers(self) -> dict:
         """
         Converts the state of a Synapse instance into a dictionary of HTTP headers.
 
         This method is essential for
         packaging Synapse data for network transmission in the Bittensor framework, ensuring that each key aspect of
         the Synapse is represented in a format suitable for HTTP communication.
@@ -608,36 +619,34 @@
         headers = {"name": self.name, "timeout": str(self.timeout)}
 
         # Adding headers for 'axon' and 'dendrite' if they are not None
         if self.axon:
             headers.update(
                 {
                     f"bt_header_axon_{k}": str(v)
-                    for k, v in self.axon.dict().items()
+                    for k, v in self.axon.model_dump().items()
                     if v is not None
                 }
             )
         if self.dendrite:
             headers.update(
                 {
                     f"bt_header_dendrite_{k}": str(v)
-                    for k, v in self.dendrite.dict().items()
+                    for k, v in self.dendrite.model_dump().items()
                     if v is not None
                 }
             )
 
         # Getting the fields of the instance
-        instance_fields = self.dict()
+        instance_fields = self.model_dump()
 
         # Iterating over the fields of the instance
         for field, value in instance_fields.items():
             # If the object is not optional, serializing it, encoding it, and adding it to the headers
-            required = schema([self.__class__])["definitions"][self.name].get(
-                "required"
-            )
+            required = self.get_required_fields()
 
             # Skipping the field if it's already in the headers or its value is None
             if field in headers or value is None:
                 continue
 
             elif required and field in required:
                 try:
@@ -683,15 +692,15 @@
         Returns:
             str: The SHA3-256 hash as a hexadecimal string, providing a fingerprint of the Synapse instance's data for integrity checks.
         """
         # Hash the body for verification
         hashes = []
 
         # Getting the fields of the instance
-        instance_fields = self.dict()
+        instance_fields = self.model_dump()
 
         for field, value in instance_fields.items():
             # If the field is required in the subclass schema, hash and add it.
             if (
                 self.required_hash_fields is not None
                 and field in self.required_hash_fields
             ):
```

### Comparing `bittensor-6.9.3/bittensor/tensor.py` & `bittensor-7.0.0/bittensor/tensor.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,64 +12,104 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-import numpy
-import torch
+import numpy as np
 import base64
 import msgpack
-import pydantic
 import msgpack_numpy
 from typing import Optional, Union, List
+from bittensor.utils.registration import torch, use_torch
+from pydantic import ConfigDict, BaseModel, Field, field_validator
 
-TORCH_DTYPES = {
-    "torch.float16": torch.float16,
-    "torch.float32": torch.float32,
-    "torch.float64": torch.float64,
-    "torch.uint8": torch.uint8,
-    "torch.int16": torch.int16,
-    "torch.int8": torch.int8,
-    "torch.int32": torch.int32,
-    "torch.int64": torch.int64,
-    "torch.bool": torch.bool,
-}
 
+class DTypes(dict):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.torch: bool = False
+        self.update(
+            {
+                "float16": np.float16,
+                "float32": np.float32,
+                "float64": np.float64,
+                "uint8": np.uint8,
+                "int16": np.int16,
+                "int8": np.int8,
+                "int32": np.int32,
+                "int64": np.int64,
+                "bool": bool,
+            }
+        )
 
-def cast_dtype(raw: Union[None, torch.dtype, str]) -> str:
-    """
-    Casts the raw value to a string representing the `torch data type <https://pytorch.org/docs/stable/tensor_attributes.html>`_.
+    def __getitem__(self, key):
+        self._add_torch()
+        return super().__getitem__(key)
+
+    def __contains__(self, key):
+        self._add_torch()
+        return super().__contains__(key)
+
+    def _add_torch(self):
+        if self.torch is False:
+            torch_dtypes = {
+                "torch.float16": torch.float16,
+                "torch.float32": torch.float32,
+                "torch.float64": torch.float64,
+                "torch.uint8": torch.uint8,
+                "torch.int16": torch.int16,
+                "torch.int8": torch.int8,
+                "torch.int32": torch.int32,
+                "torch.int64": torch.int64,
+                "torch.bool": torch.bool,
+            }
+            self.update(torch_dtypes)
+            self.torch = True
+
+
+dtypes = DTypes()
+
+
+def cast_dtype(raw: Union[None, np.dtype, "torch.dtype", str]) -> Optional[str]:
+    """
+    Casts the raw value to a string representing the
+    `numpy data type <https://numpy.org/doc/stable/user/basics.types.html>`_, or the
+    `torch data type <https://pytorch.org/docs/stable/tensor_attributes.html>`_ if using torch.
 
     Args:
-        raw (Union[None, torch.dtype, str]): The raw value to cast.
+        raw (Union[None, numpy.dtype, torch.dtype, str]): The raw value to cast.
 
     Returns:
-        str: The string representing the torch data type.
+        str: The string representing the numpy/torch data type.
 
     Raises:
         Exception: If the raw value is of an invalid type.
     """
     if not raw:
         return None
-    if isinstance(raw, torch.dtype):
-        return TORCH_DTYPES[raw]
+    if use_torch() and isinstance(raw, torch.dtype):
+        return dtypes[raw]
+    elif isinstance(raw, np.dtype):
+        return dtypes[raw]
     elif isinstance(raw, str):
-        assert (
-            raw in TORCH_DTYPES
-        ), f"{str} not a valid torch type in dict {TORCH_DTYPES}"
-        return raw
+        if use_torch():
+            assert raw in dtypes, f"{raw} not a valid torch type in dict {dtypes}"
+            return raw
+        else:
+            assert raw in dtypes, f"{raw} not a valid numpy type in dict {dtypes}"
+            return raw
     else:
         raise Exception(
-            f"{raw} of type {type(raw)} does not have a valid type in Union[None, torch.dtype, str]"
+            f"{raw} of type {type(raw)} does not have a valid type in Union[None, numpy.dtype, torch.dtype, str]"
         )
 
 
-def cast_shape(raw: Union[None, List[int], str]) -> str:
+def cast_shape(raw: Union[None, List[int], str]) -> Optional[Union[str, list]]:
     """
     Casts the raw value to a string representing the tensor shape.
 
     Args:
         raw (Union[None, List[int], str]): The raw value to cast.
 
     Returns:
@@ -77,123 +117,134 @@
 
     Raises:
         Exception: If the raw value is of an invalid type or if the list elements are not of type int.
     """
     if not raw:
         return None
     elif isinstance(raw, list):
-        if len(raw) == 0:
-            return raw
-        elif isinstance(raw[0], int):
+        if len(raw) == 0 or isinstance(raw[0], int):
             return raw
         else:
             raise Exception(f"{raw} list elements are not of type int")
     elif isinstance(raw, str):
         shape = list(map(int, raw.split("[")[1].split("]")[0].split(",")))
         return shape
     else:
         raise Exception(
             f"{raw} of type {type(raw)} does not have a valid type in Union[None, List[int], str]"
         )
 
 
 class tensor:
-    def __new__(cls, tensor: Union[list, numpy.ndarray, torch.Tensor]):
-        if isinstance(tensor, list):
-            tensor = torch.tensor(tensor)
-        elif isinstance(tensor, numpy.ndarray):
-            tensor = torch.tensor(tensor)
-        return Tensor.serialize(tensor=tensor)
+    def __new__(cls, tensor: Union[list, np.ndarray, "torch.Tensor"]):
+        if isinstance(tensor, list) or isinstance(tensor, np.ndarray):
+            tensor = torch.tensor(tensor) if use_torch() else np.array(tensor)
+        return Tensor.serialize(tensor_=tensor)
 
 
-class Tensor(pydantic.BaseModel):
+class Tensor(BaseModel):
     """
     Represents a Tensor object.
 
     Args:
         buffer (Optional[str]): Tensor buffer data.
         dtype (str): Tensor data type.
         shape (List[int]): Tensor shape.
     """
 
-    class Config:
-        validate_assignment = True
+    model_config = ConfigDict(validate_assignment=True)
 
-    def tensor(self) -> torch.Tensor:
+    def tensor(self) -> Union[np.ndarray, "torch.Tensor"]:
         return self.deserialize()
 
     def tolist(self) -> List[object]:
         return self.deserialize().tolist()
 
     def numpy(self) -> "numpy.ndarray":
-        return self.deserialize().detach().numpy()
+        return (
+            self.deserialize().detach().numpy() if use_torch() else self.deserialize()
+        )
 
-    def deserialize(self) -> "torch.Tensor":
+    def deserialize(self) -> Union["np.ndarray", "torch.Tensor"]:
         """
         Deserializes the Tensor object.
 
         Returns:
-            torch.Tensor: The deserialized tensor object.
+            np.array or torch.Tensor: The deserialized tensor object.
 
         Raises:
             Exception: If the deserialization process encounters an error.
         """
         shape = tuple(self.shape)
         buffer_bytes = base64.b64decode(self.buffer.encode("utf-8"))
         numpy_object = msgpack.unpackb(
             buffer_bytes, object_hook=msgpack_numpy.decode
         ).copy()
-        torch_object = torch.as_tensor(numpy_object)
-        # Reshape does not work for (0) or [0]
-        if not (len(shape) == 1 and shape[0] == 0):
-            torch_object = torch_object.reshape(shape)
-        return torch_object.type(TORCH_DTYPES[self.dtype])
+        if use_torch():
+            torch_object = torch.as_tensor(numpy_object)
+            # Reshape does not work for (0) or [0]
+            if not (len(shape) == 1 and shape[0] == 0):
+                torch_object = torch_object.reshape(shape)
+            return torch_object.type(dtypes[self.dtype])
+        else:
+            # Reshape does not work for (0) or [0]
+            if not (len(shape) == 1 and shape[0] == 0):
+                numpy_object = numpy_object.reshape(shape)
+            return numpy_object.astype(dtypes[self.dtype])
 
     @staticmethod
-    def serialize(tensor: "torch.Tensor") -> "Tensor":
+    def serialize(tensor_: Union["np.ndarray", "torch.Tensor"]) -> "Tensor":
         """
         Serializes the given tensor.
 
         Args:
-            tensor (torch.Tensor): The tensor to serialize.
+            tensor_ (np.array or torch.Tensor): The tensor to serialize.
 
         Returns:
             Tensor: The serialized tensor.
 
         Raises:
             Exception: If the serialization process encounters an error.
         """
-        dtype = str(tensor.dtype)
-        shape = list(tensor.shape)
+        dtype = str(tensor_.dtype)
+        shape = list(tensor_.shape)
         if len(shape) == 0:
             shape = [0]
-        torch_numpy = tensor.cpu().detach().numpy().copy()
+        tensor__ = tensor_.cpu().detach().numpy().copy() if use_torch() else tensor_
         data_buffer = base64.b64encode(
-            msgpack.packb(torch_numpy, default=msgpack_numpy.encode)
+            msgpack.packb(tensor__, default=msgpack_numpy.encode)
         ).decode("utf-8")
         return Tensor(buffer=data_buffer, shape=shape, dtype=dtype)
 
-    buffer: Optional[str] = pydantic.Field(
+    # Represents the tensor buffer data.
+    buffer: Optional[str] = Field(
+        default=None,
         title="buffer",
         description="Tensor buffer data. This field stores the serialized representation of the tensor data.",
-        examples="0x321e13edqwds231231231232131",
-        allow_mutation=False,
+        examples=["0x321e13edqwds231231231232131"],
+        frozen=True,
         repr=False,
-    )  # Represents the tensor buffer data.
+    )
 
-    dtype: str = pydantic.Field(
+    # Represents the data type of the tensor.
+    dtype: str = Field(
         title="dtype",
-        description="Tensor data type. This field specifies the data type of the tensor, such as torch.float32 or torch.int64.",
-        examples="torch.float32",
-        allow_mutation=False,
+        description="Tensor data type. This field specifies the data type of the tensor, such as numpy.float32 or torch.int64.",
+        examples=["np.float32"],
+        frozen=True,
         repr=True,
-    )  # Represents the data type of the tensor.
-    _extract_dtype = pydantic.validator("dtype", pre=True, allow_reuse=True)(cast_dtype)
+    )
 
-    shape: List[int] = pydantic.Field(
+    # Represents the shape of the tensor.
+    shape: List[int] = Field(
         title="shape",
         description="Tensor shape. This field defines the dimensions of the tensor as a list of integers, such as [10, 10] for a 2D tensor with shape (10, 10).",
-        examples="[10,10]",
-        allow_mutation=False,
+        examples=[10, 10],
+        frozen=True,
         repr=True,
-    )  # Represents the shape of the tensor.
-    _extract_shape = pydantic.validator("shape", pre=True, allow_reuse=True)(cast_shape)
+    )
+
+    # Extract the represented shape of the tensor.
+    _extract_shape = field_validator("shape", mode="before")(cast_shape)
+
+    # Extract the represented data type of the tensor.
+    _extract_dtype = field_validator("dtype", mode="before")(cast_dtype)
```

### Comparing `bittensor-6.9.3/bittensor/threadpool.py` & `bittensor-7.0.0/bittensor/threadpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,37 +7,41 @@
 
 import os
 import sys
 import time
 import queue
 import random
 import weakref
+import logging
 import argparse
 import bittensor
 import itertools
 import threading
 
-from loguru import logger
 from typing import Callable
 from concurrent.futures import _base
 
+from bittensor.btlogging.defines import BITTENSOR_LOGGER_NAME
+
 # Workers are created as daemon threads. This is done to allow the interpreter
 # to exit when there are still idle threads in a ThreadPoolExecutor's thread
 # pool (i.e. shutdown() was not called). However, allowing workers to die with
 # the interpreter has two undesirable properties:
 #   - The workers would still be running during interpreter shutdown,
 #     meaning that they would fail in unpredictable ways.
 #   - The workers could be killed while evaluating a work item, which could
 #     be bad if the callable being evaluated has external side-effects e.g.
 #     writing to a file.
 #
 # To work around this problem, an exit handler is installed which tells the
 # workers to exit when their work queues are empty and then waits until the
 # threads finish.
 
+logger = logging.getLogger(BITTENSOR_LOGGER_NAME)
+
 _threads_queues = weakref.WeakKeyDictionary()
 _shutdown = False
 
 
 class _WorkItem(object):
     def __init__(self, future, fn, start_time, args, kwargs):
         self.future = future
@@ -217,22 +221,22 @@
                 raise RuntimeError(
                     "cannot schedule new futures after " "interpreter shutdown"
                 )
 
             priority = kwargs.get("priority", random.randint(0, 1000000))
             if priority == 0:
                 priority = random.randint(1, 100)
-            eplison = random.uniform(0, 0.01) * priority
+            epsilon = random.uniform(0, 0.01) * priority
             start_time = time.time()
             if "priority" in kwargs:
                 del kwargs["priority"]
 
             f = _base.Future()
             w = _WorkItem(f, fn, start_time, args, kwargs)
-            self._work_queue.put((-float(priority + eplison), w), block=False)
+            self._work_queue.put((-float(priority + epsilon), w), block=False)
             self._adjust_thread_count()
             return f
 
     submit.__doc__ = _base.Executor.submit.__doc__
 
     def _adjust_thread_count(self):
         # if idle threads are available, don't spin new threads
```

### Comparing `bittensor-6.9.3/bittensor/types.py` & `bittensor-7.0.0/bittensor/types.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/utils/__init__.py` & `bittensor-7.0.0/bittensor/utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # The MIT License (MIT)
 # Copyright © 2022 Opentensor Foundation
 # Copyright © 2023 Opentensor Technologies Inc
+import os
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 # documentation files (the “Software”), to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 # The above copyright notice and this permission notice shall be included in all copies or substantial portions of
@@ -12,84 +13,130 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-from typing import Callable, Union, List, Optional, Dict, Literal
+from typing import Callable, List, Dict, Literal, Tuple
 
 import bittensor
 import hashlib
 import requests
-import torch
 import scalecodec
+import numpy as np
 
 from .wallet_utils import *  # noqa F401
+from .version import version_checking, check_version, VersionCheckError
+from .registration import torch, use_torch
 
 RAOPERTAO = 1e9
 U16_MAX = 65535
 U64_MAX = 18446744073709551615
 
 
 def ss58_to_vec_u8(ss58_address: str) -> List[int]:
     ss58_bytes: bytes = bittensor.utils.ss58_address_to_bytes(ss58_address)
     encoded_address: List[int] = [int(byte) for byte in ss58_bytes]
     return encoded_address
 
 
-def unbiased_topk(values, k, dim=0, sorted=True, largest=True):
-    r"""Selects topk as in torch.topk but does not bias lower indices when values are equal.
+def _unbiased_topk(
+    values: Union[np.ndarray, "torch.Tensor"],
+    k: int,
+    dim=0,
+    sorted=True,
+    largest=True,
+    axis=0,
+    return_type: str = "numpy",
+) -> Union[Tuple[np.ndarray, np.ndarray], Tuple["torch.Tensor", "torch.LongTensor"]]:
+    """Selects topk as in torch.topk but does not bias lower indices when values are equal.
     Args:
-        values: (torch.Tensor)
+        values: (np.ndarray) if using numpy, (torch.Tensor) if using torch:
             Values to index into.
         k: (int):
             Number to take.
+        dim: (int):
+            Dimension to index into (used by Torch)
+        sorted: (bool):
+            Whether to sort indices.
+        largest: (bool):
+            Whether to take the largest value.
+        axis: (int):
+            Axis along which to index into (used by Numpy)
+        return_type: (str):
+            Whether or use torch or numpy approach
 
     Return:
-        topk: (torch.Tensor):
+        topk: (np.ndarray) if using numpy, (torch.Tensor) if using torch:
             topk k values.
-        indices: (torch.LongTensor)
+        indices: (np.ndarray) if using numpy, (torch.LongTensor) if using torch:
             indices of the topk values.
     """
-    permutation = torch.randperm(values.shape[dim])
-    permuted_values = values[permutation]
-    topk, indices = torch.topk(
-        permuted_values, k, dim=dim, sorted=sorted, largest=largest
-    )
-    return topk, permutation[indices]
-
+    if return_type == "torch":
+        permutation = torch.randperm(values.shape[dim])
+        permuted_values = values[permutation]
+        topk, indices = torch.topk(
+            permuted_values, k, dim=dim, sorted=sorted, largest=largest
+        )
+        return topk, permutation[indices]
+    else:
+        if dim != 0 and axis == 0:
+            # Ensures a seamless transition for calls made to this function that specified args by keyword
+            axis = dim
+
+        permutation = np.random.permutation(values.shape[axis])
+        permuted_values = np.take(values, permutation, axis=axis)
+        indices = np.argpartition(permuted_values, -k, axis=axis)[-k:]
+        if not sorted:
+            indices = np.sort(indices, axis=axis)
+        if not largest:
+            indices = indices[::-1]
+        topk = np.take(permuted_values, indices, axis=axis)
+        return topk, permutation[indices]
+
+
+def unbiased_topk(
+    values: Union[np.ndarray, "torch.Tensor"],
+    k: int,
+    dim: int = 0,
+    sorted: bool = True,
+    largest: bool = True,
+    axis: int = 0,
+) -> Union[Tuple[np.ndarray, np.ndarray], Tuple["torch.Tensor", "torch.LongTensor"]]:
+    """Selects topk as in torch.topk but does not bias lower indices when values are equal.
+    Args:
+        values: (np.ndarray) if using numpy, (torch.Tensor) if using torch:
+            Values to index into.
+        k: (int):
+            Number to take.
+        dim: (int):
+            Dimension to index into (used by Torch)
+        sorted: (bool):
+            Whether to sort indices.
+        largest: (bool):
+            Whether to take the largest value.
+        axis: (int):
+            Axis along which to index into (used by Numpy)
 
-def version_checking(timeout: int = 15):
-    try:
-        bittensor.logging.debug(
-            f"Checking latest Bittensor version at: {bittensor.__pipaddress__}"
+    Return:
+        topk: (np.ndarray) if using numpy, (torch.Tensor) if using torch:
+            topk k values.
+        indices: (np.ndarray) if using numpy, (torch.LongTensor) if using torch:
+            indices of the topk values.
+    """
+    if use_torch():
+        return _unbiased_topk(
+            values, k, dim, sorted, largest, axis, return_type="torch"
         )
-        response = requests.get(bittensor.__pipaddress__, timeout=timeout)
-        latest_version = response.json()["info"]["version"]
-        version_split = latest_version.split(".")
-        latest_version_as_int = (
-            (100 * int(version_split[0]))
-            + (10 * int(version_split[1]))
-            + (1 * int(version_split[2]))
+    else:
+        return _unbiased_topk(
+            values, k, dim, sorted, largest, axis, return_type="numpy"
         )
 
-        if latest_version_as_int > bittensor.__version_as_int__:
-            print(
-                "\u001b[33mBittensor Version: Current {}/Latest {}\nPlease update to the latest version at your earliest convenience. "
-                "Run the following command to upgrade:\n\n\u001b[0mpython -m pip install --upgrade bittensor".format(
-                    bittensor.__version__, latest_version
-                )
-            )
-
-    except requests.exceptions.Timeout:
-        bittensor.logging.error("Version check failed due to timeout")
-    except requests.exceptions.RequestException as e:
-        bittensor.logging.error(f"Version check failed due to request failure: {e}")
-
 
 def strtobool_with_default(
     default: bool,
 ) -> Callable[[str], Union[bool, Literal["==SUPRESS=="]]]:
     """
     Creates a strtobool function with a default value.
```

### Comparing `bittensor-6.9.3/bittensor/utils/_register_cuda.py` & `bittensor-7.0.0/bittensor/utils/_register_cuda.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/utils/balance.py` & `bittensor-7.0.0/bittensor/utils/balance.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/utils/formatting.py` & `bittensor-7.0.0/bittensor/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/utils/networking.py` & `bittensor-7.0.0/bittensor/utils/networking.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/utils/registration.py` & `bittensor-7.0.0/bittensor/utils/registration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,107 @@
 import binascii
+import functools
 import hashlib
 import math
 import multiprocessing
 import os
 import random
 import time
+import typing
 from dataclasses import dataclass
 from datetime import timedelta
 from queue import Empty, Full
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import backoff
+import numpy
+
 import bittensor
-import torch
 from Crypto.Hash import keccak
 from rich import console as rich_console
 from rich import status as rich_status
 
 from .formatting import get_human_readable, millify
 from ._register_cuda import solve_cuda
 
 
+def use_torch() -> bool:
+    """Force the use of torch over numpy for certain operations."""
+    return True if os.getenv("USE_TORCH") == "1" else False
+
+
+def legacy_torch_api_compat(func):
+    """
+    Convert function operating on numpy Input&Output to legacy torch Input&Output API if `use_torch()` is True.
+
+    Args:
+        func (function):
+            Function with numpy Input/Output to be decorated.
+    Returns:
+        decorated (function):
+            Decorated function.
+    """
+
+    @functools.wraps(func)
+    def decorated(*args, **kwargs):
+        if use_torch():
+            # if argument is a Torch tensor, convert it to numpy
+            args = [
+                arg.cpu().numpy() if isinstance(arg, torch.Tensor) else arg
+                for arg in args
+            ]
+            kwargs = {
+                key: value.cpu().numpy() if isinstance(value, torch.Tensor) else value
+                for key, value in kwargs.items()
+            }
+        ret = func(*args, **kwargs)
+        if use_torch():
+            # if return value is a numpy array, convert it to Torch tensor
+            if isinstance(ret, numpy.ndarray):
+                ret = torch.from_numpy(ret)
+        return ret
+
+    return decorated
+
+
+@functools.cache
+def _get_real_torch():
+    try:
+        import torch as _real_torch
+    except ImportError:
+        _real_torch = None
+    return _real_torch
+
+
+def log_no_torch_error():
+    bittensor.btlogging.error(
+        "This command requires torch. You can install torch for bittensor"
+        ' with `pip install bittensor[torch]` or `pip install ".[torch]"`'
+        " if installing from source, and then run the command with USE_TORCH=1 {command}"
+    )
+
+
+class LazyLoadedTorch:
+    def __bool__(self):
+        return bool(_get_real_torch())
+
+    def __getattr__(self, name):
+        if real_torch := _get_real_torch():
+            return getattr(real_torch, name)
+        else:
+            log_no_torch_error()
+            raise ImportError("torch not installed")
+
+
+if typing.TYPE_CHECKING:
+    import torch
+else:
+    torch = LazyLoadedTorch()
+
+
 class CUDAException(Exception):
     """An exception raised when an error occurs in the CUDA environment."""
 
     pass
 
 
 def _hex_bytes_to_u8_list(hex_bytes: bytes):
```

### Comparing `bittensor-6.9.3/bittensor/utils/test_utils.py` & `bittensor-7.0.0/bittensor/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/utils/wallet_utils.py` & `bittensor-7.0.0/bittensor/utils/wallet_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.3/bittensor/utils/weight_utils.py` & `bittensor-7.0.0/bittensor/utils/weight_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Conversion for weight between chain representation and torch tensor
+""" Conversion for weight between chain representation and np.array or torch.Tensor
 """
 
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 # documentation files (the “Software”), to deal in the Software without restriction, including without limitation
@@ -14,53 +14,58 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-import torch
+import numpy as np
 import bittensor
-from typing import Tuple, List
+from numpy.typing import NDArray
+from typing import Tuple, List, Union
+from bittensor.utils.registration import torch, use_torch, legacy_torch_api_compat
+
+from bittensor.btlogging import logging
 
 U32_MAX = 4294967295
 U16_MAX = 65535
 
 
+@legacy_torch_api_compat
 def normalize_max_weight(
-    x: torch.FloatTensor, limit: float = 0.1
-) -> "torch.FloatTensor":
+    x: Union[NDArray[np.float32], "torch.FloatTensor"], limit: float = 0.1
+) -> Union[NDArray[np.float32], "torch.FloatTensor"]:
     r"""Normalizes the tensor x so that sum(x) = 1 and the max value is not greater than the limit.
     Args:
-        x (:obj:`torch.FloatTensor`):
+        x (:obj:`np.float32`):
             Tensor to be max_value normalized.
         limit: float:
             Max value after normalization.
     Returns:
-        y (:obj:`torch.FloatTensor`):
+        y (:obj:`np.float32`):
             Normalized x tensor.
     """
     epsilon = 1e-7  # For numerical stability after normalization
 
-    weights = x.clone()
-    values, _ = torch.sort(weights)
+    weights = x.copy()
+    values = np.sort(weights)
 
-    if x.sum() == 0 or len(x) * limit <= 1:
-        return torch.ones_like(x) / x.size(0)
+    if x.sum() == 0 or x.shape[0] * limit <= 1:
+        return np.ones_like(x) / x.shape[0]
     else:
         estimation = values / values.sum()
 
         if estimation.max() <= limit:
             return weights / weights.sum()
 
-        # Find the cumlative sum and sorted tensor
-        cumsum = torch.cumsum(estimation, 0)
+        # Find the cumulative sum and sorted tensor
+        cumsum = np.cumsum(estimation, 0)
 
         # Determine the index of cutoff
-        estimation_sum = torch.tensor(
+        estimation_sum = np.array(
             [(len(values) - i - 1) * estimation[i] for i in range(len(values))]
         )
         n_values = (estimation / (estimation_sum + cumsum + epsilon) < limit).sum()
 
         # Determine the cutoff based on the index
         cutoff_scale = (limit * cumsum[n_values - 1] - epsilon) / (
             1 - (limit * (len(estimation) - n_values))
@@ -73,100 +78,116 @@
         y = weights / weights.sum()
 
         return y
 
 
 def convert_weight_uids_and_vals_to_tensor(
     n: int, uids: List[int], weights: List[int]
-) -> "torch.FloatTensor":
-    r"""Converts weights and uids from chain representation into a torch tensor (inverse operation from convert_weights_and_uids_for_emit)
+) -> Union[NDArray[np.float32], "torch.FloatTensor"]:
+    r"""Converts weights and uids from chain representation into a np.array (inverse operation from convert_weights_and_uids_for_emit)
     Args:
         n: int:
             number of neurons on network.
         uids (:obj:`List[int],`):
             Tensor of uids as destinations for passed weights.
         weights (:obj:`List[int],`):
             Tensor of weights.
     Returns:
-        row_weights ( torch.FloatTensor ):
+        row_weights ( np.float32 or torch.FloatTensor ):
             Converted row weights.
     """
-    row_weights = torch.zeros([n], dtype=torch.float32)
+    row_weights = (
+        torch.zeros([n], dtype=torch.float32)
+        if use_torch()
+        else np.zeros([n], dtype=np.float32)
+    )
     for uid_j, wij in list(zip(uids, weights)):
         row_weights[uid_j] = float(
             wij
         )  # assumes max-upscaled values (w_max = U16_MAX).
     row_sum = row_weights.sum()
     if row_sum > 0:
         row_weights /= row_sum  # normalize
     return row_weights
 
 
 def convert_root_weight_uids_and_vals_to_tensor(
     n: int, uids: List[int], weights: List[int], subnets: List[int]
-) -> "torch.FloatTensor":
-    r"""Converts root weights and uids from chain representation into a torch tensor (inverse operation from convert_weights_and_uids_for_emit)
+) -> Union[NDArray[np.float32], "torch.FloatTensor"]:
+    r"""Converts root weights and uids from chain representation into a np.array or torch FloatTensor (inverse operation from convert_weights_and_uids_for_emit)
     Args:
         n: int:
             number of neurons on network.
         uids (:obj:`List[int],`):
             Tensor of uids as destinations for passed weights.
         weights (:obj:`List[int],`):
             Tensor of weights.
         subnets (:obj:`List[int],`):
             list of subnets on the network
     Returns:
-        row_weights ( torch.FloatTensor ):
+        row_weights ( np.float32 ):
             Converted row weights.
     """
 
-    row_weights = torch.zeros([n], dtype=torch.float32)
+    row_weights = (
+        torch.zeros([n], dtype=torch.float32)
+        if use_torch()
+        else np.zeros([n], dtype=np.float32)
+    )
     for uid_j, wij in list(zip(uids, weights)):
         if uid_j in subnets:
             index_s = subnets.index(uid_j)
+            row_weights[index_s] = float(
+                wij
+            )  # assumes max-upscaled values (w_max = U16_MAX).
         else:
-            raise Exception("Incorrect Subnet {uid_j} in {subnets}")
-        row_weights[index_s] = float(
-            wij
-        )  # assumes max-upscaled values (w_max = U16_MAX).
+            logging.warning(
+                f"Incorrect Subnet uid {uid_j} in Subnets {subnets}. The subnet is unavailable at the moment."
+            )
+            continue
     row_sum = row_weights.sum()
     if row_sum > 0:
         row_weights /= row_sum  # normalize
     return row_weights
 
 
 def convert_bond_uids_and_vals_to_tensor(
     n: int, uids: List[int], bonds: List[int]
-) -> "torch.LongTensor":
-    r"""Converts bond and uids from chain representation into a torch tensor.
+) -> Union[NDArray[np.int64], "torch.LongTensor"]:
+    r"""Converts bond and uids from chain representation into a np.array.
     Args:
         n: int:
             number of neurons on network.
         uids (:obj:`List[int],`):
             Tensor of uids as destinations for passed bonds.
         bonds (:obj:`List[int],`):
             Tensor of bonds.
     Returns:
-        row_bonds ( torch.FloatTensor ):
+        row_bonds ( np.float32 ):
             Converted row bonds.
     """
-    row_bonds = torch.zeros([n], dtype=torch.int64)
+    row_bonds = (
+        torch.zeros([n], dtype=torch.int64)
+        if use_torch()
+        else np.zeros([n], dtype=np.int64)
+    )
     for uid_j, bij in list(zip(uids, bonds)):
         row_bonds[uid_j] = int(bij)
     return row_bonds
 
 
 def convert_weights_and_uids_for_emit(
-    uids: torch.LongTensor, weights: torch.FloatTensor
+    uids: Union[NDArray[np.int64], "torch.LongTensor"],
+    weights: Union[NDArray[np.float32], "torch.FloatTensor"],
 ) -> Tuple[List[int], List[int]]:
     r"""Converts weights into integer u32 representation that sum to MAX_INT_WEIGHT.
     Args:
-        uids (:obj:`torch.LongTensor,`):
+        uids (:obj:`np.int64,`):
             Tensor of uids as destinations for passed weights.
-        weights (:obj:`torch.FloatTensor,`):
+        weights (:obj:`np.float32,`):
             Tensor of weights.
     Returns:
         weight_uids (List[int]):
             Uids as a list.
         weight_vals (List[int]):
             Weights as a list.
     """
@@ -205,77 +226,113 @@
             weight_vals.append(uint16_val)
             weight_uids.append(uid_i)
 
     return weight_uids, weight_vals
 
 
 def process_weights_for_netuid(
-    uids,
-    weights: torch.Tensor,
+    uids: Union[NDArray[np.int64], "torch.Tensor"],
+    weights: Union[NDArray[np.float32], "torch.Tensor"],
     netuid: int,
     subtensor: "bittensor.subtensor",
     metagraph: "bittensor.metagraph" = None,
     exclude_quantile: int = 0,
-) -> torch.FloatTensor:
+) -> Union[
+    Tuple["torch.Tensor", "torch.FloatTensor"],
+    Tuple[NDArray[np.int64], NDArray[np.float32]],
+]:
     bittensor.logging.debug("process_weights_for_netuid()")
     bittensor.logging.debug("weights", weights)
     bittensor.logging.debug("netuid", netuid)
     bittensor.logging.debug("subtensor", subtensor)
     bittensor.logging.debug("metagraph", metagraph)
 
     # Get latest metagraph from chain if metagraph is None.
-    if metagraph == None:
+    if metagraph is None:
         metagraph = subtensor.metagraph(netuid)
 
     # Cast weights to floats.
-    if not isinstance(weights, torch.FloatTensor):
-        weights = weights.type(torch.float32)
+    if not use_torch():
+        if not isinstance(weights, torch.FloatTensor):
+            weights = weights.type(torch.float32)
+    else:
+        if not isinstance(weights, np.float32):
+            weights = weights.astype(np.float32)
 
     # Network configuration parameters from an subtensor.
     # These parameters determine the range of acceptable weights for each neuron.
     quantile = exclude_quantile / U16_MAX
     min_allowed_weights = subtensor.min_allowed_weights(netuid=netuid)
     max_weight_limit = subtensor.max_weight_limit(netuid=netuid)
     bittensor.logging.debug("quantile", quantile)
     bittensor.logging.debug("min_allowed_weights", min_allowed_weights)
     bittensor.logging.debug("max_weight_limit", max_weight_limit)
 
     # Find all non zero weights.
-    non_zero_weight_idx = torch.argwhere(weights > 0).squeeze(dim=1)
+    non_zero_weight_idx = (
+        torch.argwhere(weights > 0).squeeze(dim=1)
+        if use_torch()
+        else np.argwhere(weights > 0).squeeze(axis=1)
+    )
     non_zero_weight_uids = uids[non_zero_weight_idx]
     non_zero_weights = weights[non_zero_weight_idx]
-    if non_zero_weights.numel() == 0 or metagraph.n < min_allowed_weights:
+    nzw_size = non_zero_weights.numel() if use_torch() else non_zero_weights.size
+    if nzw_size == 0 or metagraph.n < min_allowed_weights:
         bittensor.logging.warning("No non-zero weights returning all ones.")
-        final_weights = torch.ones((metagraph.n)).to(metagraph.n) / metagraph.n
+        final_weights = (
+            torch.ones((metagraph.n)).to(metagraph.n) / metagraph.n
+            if use_torch()
+            else np.ones((metagraph.n), dtype=np.int64) / metagraph.n
+        )
         bittensor.logging.debug("final_weights", final_weights)
-        return torch.tensor(list(range(len(final_weights)))), final_weights
+        final_weights_count = (
+            torch.tensor(list(range(len(final_weights))))
+            if use_torch()
+            else np.arange(len(final_weights))
+        )
+        return (
+            (final_weights_count, final_weights)
+            if use_torch()
+            else (final_weights_count, final_weights)
+        )
 
-    elif non_zero_weights.numel() < min_allowed_weights:
+    elif nzw_size < min_allowed_weights:
         bittensor.logging.warning(
             "No non-zero weights less then min allowed weight, returning all ones."
         )
-        # ( const ): Should this be torch.zeros( ( metagraph.n ) ) to reset everyone to build up weight?
+        # ( const ): Should this be np.zeros( ( metagraph.n ) ) to reset everyone to build up weight?
         weights = (
             torch.ones((metagraph.n)).to(metagraph.n) * 1e-5
+            if use_torch()
+            else np.ones((metagraph.n), dtype=np.int64) * 1e-5
         )  # creating minimum even non-zero weights
         weights[non_zero_weight_idx] += non_zero_weights
         bittensor.logging.debug("final_weights", weights)
         normalized_weights = bittensor.utils.weight_utils.normalize_max_weight(
             x=weights, limit=max_weight_limit
         )
-        return torch.tensor(list(range(len(normalized_weights)))), normalized_weights
+        nw_arange = (
+            torch.tensor(list(range(len(normalized_weights))))
+            if use_torch()
+            else np.arange(len(normalized_weights))
+        )
+        return nw_arange, normalized_weights
 
     bittensor.logging.debug("non_zero_weights", non_zero_weights)
 
     # Compute the exclude quantile and find the weights in the lowest quantile
     max_exclude = max(0, len(non_zero_weights) - min_allowed_weights) / len(
         non_zero_weights
     )
     exclude_quantile = min([quantile, max_exclude])
-    lowest_quantile = non_zero_weights.quantile(exclude_quantile)
+    lowest_quantile = (
+        non_zero_weights.quantile(exclude_quantile)
+        if use_torch()
+        else np.quantile(non_zero_weights, exclude_quantile)
+    )
     bittensor.logging.debug("max_exclude", max_exclude)
     bittensor.logging.debug("exclude_quantile", exclude_quantile)
     bittensor.logging.debug("lowest_quantile", lowest_quantile)
 
     # Exclude all weights below the allowed quantile.
     non_zero_weight_uids = non_zero_weight_uids[lowest_quantile <= non_zero_weights]
     non_zero_weights = non_zero_weights[lowest_quantile <= non_zero_weights]
```

### Comparing `bittensor-6.9.3/bittensor/wallet.py` & `bittensor-7.0.0/bittensor/wallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -736,14 +736,16 @@
         json = kwargs.get("json", None)
 
         if mnemonic is None and seed is None and json is None:
             raise ValueError("Must pass either mnemonic, seed, or json")
         if mnemonic is not None:
             if isinstance(mnemonic, str):
                 mnemonic = mnemonic.split()
+            elif isinstance(mnemonic, list) and len(mnemonic) == 1:
+                mnemonic = mnemonic[0].split()
             if len(mnemonic) not in [12, 15, 18, 21, 24]:
                 raise ValueError(
                     "Mnemonic has invalid size. This should be 12,15,18,21 or 24 words"
                 )
             keypair = Keypair.create_from_mnemonic(
                 " ".join(mnemonic), ss58_format=bittensor.__ss58_format__
             )
```

### Comparing `bittensor-6.9.3/bittensor.egg-info/PKG-INFO` & `bittensor-7.0.0/bittensor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 6.9.3
+Version: 7.0.0
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: torch
 License-File: LICENSE
 
 <div align="center">
 
 # **Bittensor** <!-- omit in toc -->
 [![Discord Chat](https://img.shields.io/discord/308323056592486420.svg)](https://discord.gg/bittensor)
 [![PyPI version](https://badge.fury.io/py/bittensor.svg)](https://badge.fury.io/py/bittensor)
@@ -244,14 +245,19 @@
 btcli --print-completion zsh >> ~/.zshrc    # For Zsh
 source ~/.bashrc  # Reload Bash configuration to take effect
 ```
 
 # The Bittensor Package
 The bittensor package contains data structures for interacting with the bittensor ecosystem, writing miners, validators and querying the network. Additionally, it provides many utilities for efficient serialization of Tensors over the wire, performing data analysis of the network, and other useful utilities.
 
+In the 7.0.0 release, we have removed `torch` by default. However, you can still use `torch` by setting the environment variable
+`USE_TORCH=1` and making sure that you have installed the `torch` library. 
+You can install `torch` by running `pip install bittensor[torch]` (if installing via PyPI), or by running `pip install -e ".[torch]"` (if installing from source). 
+We will not be adding any new functionality based on torch.
+
 Wallet: Interface over locally stored bittensor hot + coldkey styled wallets. 
 ```python
 import bittensor
 # Bittensor's wallet maintenance class.
 wallet = bittensor.wallet() 
 # Access the hotkey
 wallet.hotkey 
@@ -296,15 +302,15 @@
 metagraph.load()
 ```
 
 Synapse: Responsible for defining the protocol definition between axon servers and dendrite clients
 ```python
 class Topk( bittensor.Synapse ):
     topk: int = 2  # Number of "top" elements to select
-    input: bittensor.Tensor = pydantic.Field(..., allow_mutation=False)  # Ensure that input cannot be set on the server side. 
+    input: bittensor.Tensor = pydantic.Field(..., frozen=True)  # Ensure that input cannot be set on the server side. 
     v: bittensor.Tensor = None
     i: bittensor.Tensor = None
 
 def topk( synapse: Topk ) -> Topk:
     v, i = torch.topk( synapse.input.deserialize(), k = synapse.topk ) 
     synapse.v = bittensor.Tensor.serialize( v )
     synapse.i = bittensor.Tensor.serialize( i )
@@ -352,16 +358,16 @@
     forward_fn = forward_my_synapse, 
     verify_fn=verify_my_synapse,
     blacklist_fn = blacklist_my_synapse,
     priority_fn = prioritize_my_synape
 ).start()
 ```     
 
-Dendrite: Inheriting from PyTorch's Module class, represents the abstracted implementation of a network client module designed 
-to send requests to those endpoints to receive inputs.
+Dendrite: Represents the abstracted implementation of a network client module
+designed to send requests to those endpoints to receive inputs.
 
 Example:
 ```python
 dendrite_obj = dendrite( wallet = bittensor.wallet() )
 # pings the axon endpoint
 await d( <axon> )
 # ping multiple axon endpoints
```

### Comparing `bittensor-6.9.3/bittensor.egg-info/SOURCES.txt` & `bittensor-7.0.0/bittensor.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 setup.py
 bin/btcli
 bittensor/__init__.py
 bittensor/axon.py
-bittensor/btlogging.py
 bittensor/chain_data.py
 bittensor/cli.py
 bittensor/config.py
 bittensor/dendrite.py
 bittensor/errors.py
 bittensor/keyfile.py
 bittensor/metagraph.py
@@ -21,14 +20,19 @@
 bittensor/types.py
 bittensor/wallet.py
 bittensor.egg-info/PKG-INFO
 bittensor.egg-info/SOURCES.txt
 bittensor.egg-info/dependency_links.txt
 bittensor.egg-info/requires.txt
 bittensor.egg-info/top_level.txt
+bittensor/btlogging/__init__.py
+bittensor/btlogging/defines.py
+bittensor/btlogging/format.py
+bittensor/btlogging/helpers.py
+bittensor/btlogging/loggingmachine.py
 bittensor/commands/__init__.py
 bittensor/commands/delegates.py
 bittensor/commands/identity.py
 bittensor/commands/inspect.py
 bittensor/commands/list.py
 bittensor/commands/metagraph.py
 bittensor/commands/misc.py
@@ -60,33 +64,12 @@
 bittensor/mock/wallet_mock.py
 bittensor/utils/__init__.py
 bittensor/utils/_register_cuda.py
 bittensor/utils/balance.py
 bittensor/utils/formatting.py
 bittensor/utils/networking.py
 bittensor/utils/registration.py
+bittensor/utils/subtensor.py
 bittensor/utils/test_utils.py
+bittensor/utils/version.py
 bittensor/utils/wallet_utils.py
-bittensor/utils/weight_utils.py
-tests/__init__.py
-tests/helpers/__init__.py
-tests/helpers/helpers.py
-tests/integration_tests/__init__.py
-tests/integration_tests/test_cli.py
-tests/integration_tests/test_cli_no_network.py
-tests/integration_tests/test_metagraph_integration.py
-tests/integration_tests/test_subtensor_integration.py
-tests/unit_tests/__init__.py
-tests/unit_tests/test_axon.py
-tests/unit_tests/test_chain_data.py
-tests/unit_tests/test_dendrite.py
-tests/unit_tests/test_keyfile.py
-tests/unit_tests/test_metagraph.py
-tests/unit_tests/test_subtensor.py
-tests/unit_tests/test_synapse.py
-tests/unit_tests/test_tensor.py
-tests/unit_tests/test_wallet.py
-tests/unit_tests/utils/__init__.py
-tests/unit_tests/utils/test_balance.py
-tests/unit_tests/utils/test_networking.py
-tests/unit_tests/utils/test_utils.py
-tests/unit_tests/utils/test_weight_utils.py
+bittensor/utils/weight_utils.py
```

### Comparing `bittensor-6.9.3/bittensor.egg-info/requires.txt` & `bittensor-7.0.0/bittensor.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 aiohttp==3.9.0b0
 ansible==6.7.0
 ansible_vault==2.1.0
 backoff
 black==23.7.0
-cryptography==42.0.0
+certifi==2024.2.2
+colorama==0.4.6
+cryptography==42.0.5
 ddt==1.6.0
+eth-utils<2.3.0
 fuzzywuzzy>=0.18.0
-fastapi==0.99.1
-loguru==0.7.0
+fastapi==0.110.1
 munch==2.5.0
 netaddr
 numpy
 msgpack-numpy-opentensor==0.5.0
 nest_asyncio
+packaging
 pycryptodome<4.0.0,>=3.18.0
 pyyaml
 password_strength
-pydantic!=1.8,!=1.8.1,<2.0.0,>=1.7.4
+pydantic<3,>=2.3
 PyNaCl<=1.5.0,>=1.3.0
 pytest-asyncio
 python-Levenshtein
+python-statemachine==2.1.2
 pytest
 retry
 requests
 rich
 scalecodec==1.2.7
 shtab==1.6.5
 substrate-interface==1.7.5
 termcolor
-torch>=1.13.1
 tqdm
 uvicorn==0.22.0
 wheel
 
 [dev]
+aioresponses==0.7.6
 pytest==7.2.0
 pytest-mock==3.12.0
 pytest-split==0.8.0
 pytest-xdist==3.0.2
 pytest-rerunfailures==10.2
 coveralls==3.3.1
 pytest-cov==4.0.0
 ddt==1.6.0
 hypothesis==6.81.1
 flake8==7.0.0
 mypy==1.8.0
 types-retry==0.9.9.4
+freezegun==1.5.0
+torch>=1.13.1
+factory-boy==3.3.0
+
+[torch]
+torch>=1.13.1
```

### Comparing `bittensor-6.9.3/setup.py` & `bittensor-7.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,22 +12,20 @@
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 from setuptools import setup, find_packages
-from pkg_resources import parse_requirements
 from os import path
 from io import open
 import codecs
 import re
 import os
 import pathlib
-import subprocess
 
 
 def read_requirements(path):
     requirements = []
     git_requirements = []
 
     with pathlib.Path(path).open() as requirements_txt:
@@ -40,14 +38,15 @@
 
     return requirements
 
 
 requirements = read_requirements("requirements/prod.txt")
 extra_requirements_dev = read_requirements("requirements/dev.txt")
 extra_requirements_cubit = read_requirements("requirements/cubit.txt")
+extra_requirements_torch = read_requirements("requirements/torch.txt")
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
@@ -64,34 +63,35 @@
     name="bittensor",
     version=version_string,
     description="bittensor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/opentensor/bittensor",
     author="bittensor.com",
-    packages=find_packages(),
+    packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     author_email="",
     license="MIT",
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     install_requires=requirements,
     extras_require={
         "dev": extra_requirements_dev,
+        "torch": extra_requirements_torch,
     },
     scripts=["bin/btcli"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         # Pick your license as you wish
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
```

### Comparing `bittensor-6.9.3/tests/__init__.py` & `bittensor-7.0.0/bittensor/btlogging/defines.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 # The MIT License (MIT)
-# Copyright © 2022 Yuma Rao
-# Copyright © 2022-2023 Opentensor Foundation
-# Copyright © 2023 Opentensor Technologies Inc
+# Copyright © 2023 OpenTensor Foundation
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 # documentation files (the “Software”), to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 # The above copyright notice and this permission notice shall be included in all copies or substantial portions of
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
+
+"""Btlogging constant definition module."""
+
+BASE_LOG_FORMAT = "%(asctime)s | %(levelname)s | %(message)s"
+TRACE_LOG_FORMAT = (
+    f"%(asctime)s | %(levelname)s | %(name)s:%(filename)s:%(lineno)s | %(message)s"
+)
+DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
+BITTENSOR_LOGGER_NAME = "bittensor"
+DEFAULT_LOG_FILE_NAME = "bittensor.log"
+DEFAULT_MAX_ROTATING_LOG_FILE_SIZE = 25 * 1024 * 1024
+DEFAULT_LOG_BACKUP_COUNT = 10
```

