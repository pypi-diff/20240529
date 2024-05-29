# Comparing `tmp/sheeprl-0.5.6.tar.gz` & `tmp/sheeprl-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheeprl-0.5.6.tar", last modified: Tue May 28 09:23:27 2024, max compression
+gzip compressed data, was "sheeprl-0.5.7.tar", last modified: Wed May 29 09:40:53 2024, max compression
```

## Comparing `sheeprl-0.5.6.tar` & `sheeprl-0.5.7.tar`

### file list

```diff
@@ -1,269 +1,269 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.554382 sheeprl-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-28 09:23:23.000000 sheeprl-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 09:23:23.000000 sheeprl-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-28 09:23:27.554382 sheeprl-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24648 2024-05-28 09:23:23.000000 sheeprl-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.510382 sheeprl-0.5.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-28 09:23:23.000000 sheeprl-0.5.6/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.510382 sheeprl-0.5.6/hydra_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-28 09:23:23.000000 sheeprl-0.5.6/hydra_plugins/sheeprl_search_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-28 09:23:23.000000 sheeprl-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:23:27.554382 sheeprl-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-28 09:23:23.000000 sheeprl-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.510382 sheeprl-0.5.6/sheeprl/
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.510382 sheeprl-0.5.6/sheeprl/algos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.514382 sheeprl-0.5.6/sheeprl/algos/a2c/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/a2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17056 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/a2c/a2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/a2c/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/a2c/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/a2c/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/a2c/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.514382 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    37013 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/dreamer_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.514382 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50079 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    37705 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/dreamer_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.518382 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57473 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    36001 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/dreamer_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/dreamer_v3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.518382 sheeprl-0.5.6/sheeprl/algos/droq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/droq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/droq/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    19322 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/droq/droq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/droq/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/droq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.518382 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    39226 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/p2e_dv1_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)    20966 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/p2e_dv1_finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.518382 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    45740 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/p2e_dv2_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)    22312 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/p2e_dv2_finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.522382 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    50773 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/p2e_dv3_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)    22684 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/p2e_dv3_finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/p2e_dv3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.522382 sheeprl-0.5.6/sheeprl/algos/ppo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    20232 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/ppo.py
--rw-r--r--   0 runner    (1001) docker     (127)    29492 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/ppo_decoupled.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.522382 sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    23826 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/ppo_recurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.526382 sheeprl-0.5.6/sheeprl/algos/sac/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/sac.py
--rw-r--r--   0 runner    (1001) docker     (127)    25840 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/sac_decoupled.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.526382 sheeprl-0.5.6/sheeprl/algos/sac_ae/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac_ae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24357 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac_ae/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac_ae/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    22522 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac_ae/sac_ae.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/algos/sac_ae/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/available_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    20399 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.526382 sheeprl-0.5.6/sheeprl/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.530382 sheeprl-0.5.6/sheeprl/configs/algo/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/a2c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3_L.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3_M.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3_S.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3_XL.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3_XS.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/droq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/p2e_dv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/p2e_dv2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/p2e_dv3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/ppo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/ppo_decoupled.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/ppo_recurrent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/sac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/sac_ae.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/algo/sac_decoupled.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.530382 sheeprl-0.5.6/sheeprl/configs/buffer/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/buffer/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.530382 sheeprl-0.5.6/sheeprl/configs/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/checkpoint/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.530382 sheeprl-0.5.6/sheeprl/configs/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/distribution/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.534382 sheeprl-0.5.6/sheeprl/configs/env/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/atari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/crafter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/diambra.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/dmc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/dummy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/gym.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/minecraft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/minedojo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/minerl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/minerl_obtain_diamond.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/minerl_obtain_iron_pickaxe.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/mujoco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env/super_mario_bros.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/env_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/eval_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.538382 sheeprl-0.5.6/sheeprl/configs/exp/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/a2c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/a2c_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v1_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2_crafter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_100k_boxing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_100k_ms_pacman.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_L_doapp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_L_navigate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_XL_crafter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_dmc_cartpole_swingup_sparse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_minedojo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_super_mario_bros.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/droq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv1_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv1_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv2_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv2_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_fntn_L_doapp_64px_gray_combo_discrete_5Mstps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/ppo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/ppo_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/ppo_decoupled.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/ppo_recurrent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/ppo_super_mario_bros.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/sac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/sac_ae.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/sac_benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/exp/sac_decoupled.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.538382 sheeprl-0.5.6/sheeprl/configs/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/fabric/ddp-cpu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/fabric/ddp-cuda.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/fabric/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.538382 sheeprl-0.5.6/sheeprl/configs/hydra/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/hydra/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.542382 sheeprl-0.5.6/sheeprl/configs/logger/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/logger/mlflow.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/logger/tensorboard.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.542382 sheeprl-0.5.6/sheeprl/configs/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/metric/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.542382 sheeprl-0.5.6/sheeprl/configs/model_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/a2c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/dreamer_v1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/dreamer_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/dreamer_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/droq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv1_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv1_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv2_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv2_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv3_exploration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv3_finetuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/ppo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/ppo_recurrent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/sac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager/sac_ae.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/model_manager_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.542382 sheeprl-0.5.6/sheeprl/configs/optim/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/optim/adam.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/optim/rmsprop.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/optim/rmsprop_tf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/configs/optim/sgd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.542382 sheeprl-0.5.6/sheeprl/data/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54229 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/data/buffers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.546382 sheeprl-0.5.6/sheeprl/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/crafter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/diambra.py
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/dmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/minedojo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/minerl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.546382 sheeprl-0.5.6/sheeprl/envs/minerl_envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/minerl_envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/minerl_envs/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/minerl_envs/navigate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/minerl_envs/obtain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/super_mario_bros.py
--rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/envs/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.546382 sheeprl-0.5.6/sheeprl/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21610 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.546382 sheeprl-0.5.6/sheeprl/optim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/optim/rmsprop_tf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.550382 sheeprl-0.5.6/sheeprl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/memmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    17999 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-28 09:23:23.000000 sheeprl-0.5.6/sheeprl/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:23:27.550382 sheeprl-0.5.6/sheeprl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-28 09:23:27.000000 sheeprl-0.5.6/sheeprl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-05-28 09:23:27.000000 sheeprl-0.5.6/sheeprl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:23:27.000000 sheeprl-0.5.6/sheeprl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-28 09:23:27.000000 sheeprl-0.5.6/sheeprl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-28 09:23:27.000000 sheeprl-0.5.6/sheeprl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 09:23:27.000000 sheeprl-0.5.6/sheeprl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.577332 sheeprl-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-29 09:40:48.000000 sheeprl-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-29 09:40:48.000000 sheeprl-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-29 09:40:53.577332 sheeprl-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24648 2024-05-29 09:40:48.000000 sheeprl-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.537332 sheeprl-0.5.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-29 09:40:48.000000 sheeprl-0.5.7/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.537332 sheeprl-0.5.7/hydra_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-29 09:40:48.000000 sheeprl-0.5.7/hydra_plugins/sheeprl_search_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-29 09:40:48.000000 sheeprl-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:40:53.577332 sheeprl-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-29 09:40:48.000000 sheeprl-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.541332 sheeprl-0.5.7/sheeprl/
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.541332 sheeprl-0.5.7/sheeprl/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.541332 sheeprl-0.5.7/sheeprl/algos/a2c/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/a2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17064 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/a2c/a2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/a2c/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/a2c/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/a2c/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/a2c/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.541332 sheeprl-0.5.7/sheeprl/algos/dreamer_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v1/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37013 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v1/dreamer_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v1/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v1/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.545332 sheeprl-0.5.7/sheeprl/algos/dreamer_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50079 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v2/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37705 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v2/dreamer_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v2/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v2/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.545332 sheeprl-0.5.7/sheeprl/algos/dreamer_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57473 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v3/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36001 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v3/dreamer_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v3/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v3/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/dreamer_v3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.545332 sheeprl-0.5.7/sheeprl/algos/droq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/droq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/droq/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19322 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/droq/droq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/droq/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/droq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.545332 sheeprl-0.5.7/sheeprl/algos/p2e_dv1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv1/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv1/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39226 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv1/p2e_dv1_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20966 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv1/p2e_dv1_finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.549332 sheeprl-0.5.7/sheeprl/algos/p2e_dv2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv2/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv2/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45740 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv2/p2e_dv2_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22312 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv2/p2e_dv2_finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.549332 sheeprl-0.5.7/sheeprl/algos/p2e_dv3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv3/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv3/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50773 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv3/p2e_dv3_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22684 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv3/p2e_dv3_finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/p2e_dv3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.549332 sheeprl-0.5.7/sheeprl/algos/ppo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/ppo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/ppo/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/ppo/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/ppo/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20240 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/ppo/ppo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29492 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/ppo/ppo_decoupled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/ppo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.553332 sheeprl-0.5.7/sheeprl/algos/ppo_recurrent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/ppo_recurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/ppo_recurrent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/ppo_recurrent/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23834 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/ppo_recurrent/ppo_recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/ppo_recurrent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.553332 sheeprl-0.5.7/sheeprl/algos/sac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/sac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/sac/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/sac/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/sac/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/sac/sac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25840 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/sac/sac_decoupled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/sac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.553332 sheeprl-0.5.7/sheeprl/algos/sac_ae/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/sac_ae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24357 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/sac_ae/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/sac_ae/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22522 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/sac_ae/sac_ae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/algos/sac_ae/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/available_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20399 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.553332 sheeprl-0.5.7/sheeprl/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.557332 sheeprl-0.5.7/sheeprl/configs/algo/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/a2c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/dreamer_v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/dreamer_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/dreamer_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/dreamer_v3_L.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/dreamer_v3_M.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/dreamer_v3_S.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/dreamer_v3_XL.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/dreamer_v3_XS.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/droq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/p2e_dv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/p2e_dv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/p2e_dv3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/ppo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/ppo_decoupled.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/ppo_recurrent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/sac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/sac_ae.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/algo/sac_decoupled.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.557332 sheeprl-0.5.7/sheeprl/configs/buffer/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/buffer/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.557332 sheeprl-0.5.7/sheeprl/configs/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/checkpoint/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.557332 sheeprl-0.5.7/sheeprl/configs/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/distribution/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.561332 sheeprl-0.5.7/sheeprl/configs/env/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/atari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/crafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/diambra.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/dmc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/dummy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/gym.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/minecraft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/minedojo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/minerl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/minerl_obtain_diamond.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/minerl_obtain_iron_pickaxe.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/mujoco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env/super_mario_bros.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/env_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/eval_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.565332 sheeprl-0.5.7/sheeprl/configs/exp/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/a2c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/a2c_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v1_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v2_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v2_crafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_100k_boxing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_100k_ms_pacman.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_L_doapp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_L_navigate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_XL_crafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_dmc_cartpole_swingup_sparse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_minedojo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_super_mario_bros.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/droq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv1_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv1_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv2_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv2_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv3_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv3_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv3_fntn_L_doapp_64px_gray_combo_discrete_5Mstps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/ppo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/ppo_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/ppo_decoupled.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/ppo_recurrent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/ppo_super_mario_bros.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/sac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/sac_ae.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/sac_benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/exp/sac_decoupled.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.565332 sheeprl-0.5.7/sheeprl/configs/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/fabric/ddp-cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/fabric/ddp-cuda.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/fabric/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.565332 sheeprl-0.5.7/sheeprl/configs/hydra/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/hydra/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.565332 sheeprl-0.5.7/sheeprl/configs/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/logger/mlflow.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/logger/tensorboard.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.565332 sheeprl-0.5.7/sheeprl/configs/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/metric/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.569332 sheeprl-0.5.7/sheeprl/configs/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/a2c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/dreamer_v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/dreamer_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/dreamer_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/droq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/p2e_dv1_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/p2e_dv1_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/p2e_dv2_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/p2e_dv2_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/p2e_dv3_exploration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/p2e_dv3_finetuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/ppo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/ppo_recurrent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/sac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager/sac_ae.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/model_manager_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.569332 sheeprl-0.5.7/sheeprl/configs/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/optim/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/optim/rmsprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/optim/rmsprop_tf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/configs/optim/sgd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.569332 sheeprl-0.5.7/sheeprl/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54229 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/data/buffers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.573332 sheeprl-0.5.7/sheeprl/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/crafter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/diambra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/dmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/minedojo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/minerl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.573332 sheeprl-0.5.7/sheeprl/envs/minerl_envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/minerl_envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/minerl_envs/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/minerl_envs/navigate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/minerl_envs/obtain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/super_mario_bros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/envs/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.573332 sheeprl-0.5.7/sheeprl/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21610 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.573332 sheeprl-0.5.7/sheeprl/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/optim/rmsprop_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.573332 sheeprl-0.5.7/sheeprl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/memmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17999 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-29 09:40:48.000000 sheeprl-0.5.7/sheeprl/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:40:53.573332 sheeprl-0.5.7/sheeprl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-29 09:40:53.000000 sheeprl-0.5.7/sheeprl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-05-29 09:40:53.000000 sheeprl-0.5.7/sheeprl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:40:53.000000 sheeprl-0.5.7/sheeprl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-29 09:40:53.000000 sheeprl-0.5.7/sheeprl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-29 09:40:53.000000 sheeprl-0.5.7/sheeprl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 09:40:53.000000 sheeprl-0.5.7/sheeprl.egg-info/top_level.txt
```

### Comparing `sheeprl-0.5.6/LICENSE` & `sheeprl-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/PKG-INFO` & `sheeprl-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheeprl
-Version: 0.5.6
+Version: 0.5.7
 Summary: High-quality, single file and distributed implementation of Deep Reinforcement Learning algorithms with production-friendly features
 Author-email: Federico Belotti <federico.belotti@orobix.com>, Davide Angioni <davide.angioni@orobix.com>, Refik Can Malli <refikcan.malli@orobix.com>, Michele Milesi <michele.milesi@orobix.com>
 Maintainer-email: Federico Belotti <federico.belotti@orobix.com>, Davide Angioni <davide.angioni@orobix.com>, Refik Can Malli <refikcan.malli@orobix.com>, Michele Milesi <michele.milesi@orobix.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `sheeprl-0.5.6/README.md` & `sheeprl-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/docs/README.md` & `sheeprl-0.5.7/docs/README.md`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/hydra_plugins/sheeprl_search_path.py` & `sheeprl-0.5.7/hydra_plugins/sheeprl_search_path.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/pyproject.toml` & `sheeprl-0.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 # -> Level 4# This one isn't too hard to get passing, but return on investment is lower
 no_implicit_reexport = false
 # This one can be tricky to get passing if you use a lot of untyped libraries
 warn_return_any = false
 
 
 [tool.bumpver]
-current_version = "0.5.6"
+current_version = "0.5.7"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "v{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `sheeprl-0.5.6/setup.py` & `sheeprl-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/__init__.py` & `sheeprl-0.5.7/sheeprl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # fmt: on
 
 # Needed because MineRL 0.4.4 is not compatible with the latest version of numpy
 np.float = np.float32
 np.int = np.int64
 np.bool = bool
 
-__version__ = "0.5.6"
+__version__ = "0.5.7"
 
 
 # Replace `moviepy.decorators.use_clip_fps_by_default` method to work with python 3.8, 3.9, and 3.10
 import moviepy.decorators
 
 
 # Taken from https://github.com/Zulko/moviepy/blob/master/moviepy/decorators.py#L118
```

### Comparing `sheeprl-0.5.6/sheeprl/algos/a2c/a2c.py` & `sheeprl-0.5.7/sheeprl/algos/a2c/a2c.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     next_obs = envs.reset(seed=cfg.seed)[0]  # [N_envs, N_obs]
     for k in obs_keys:
         step_data[k] = next_obs[k][np.newaxis]
 
     for iter_num in range(1, total_iters + 1):
         with torch.inference_mode():
             for _ in range(0, cfg.algo.rollout_steps):
-                policy_step += policy_steps_per_iter
+                policy_step += cfg.env.num_envs * world_size
 
                 # Measure environment interaction time: this considers both the model forward
                 # to get the action given the observation and the time taken into the environment
                 with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                     # Sample an action given the observation received by the environment
                     # This calls the `forward` method of the PyTorch module, escaping from Fabric
                     # because we don't want this to be a synchronization point
```

### Comparing `sheeprl-0.5.6/sheeprl/algos/a2c/agent.py` & `sheeprl-0.5.7/sheeprl/algos/a2c/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/a2c/evaluate.py` & `sheeprl-0.5.7/sheeprl/algos/a2c/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/a2c/loss.py` & `sheeprl-0.5.7/sheeprl/algos/a2c/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/a2c/utils.py` & `sheeprl-0.5.7/sheeprl/algos/a2c/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v1/agent.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v1/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v1/dreamer_v1.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v1/dreamer_v1.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v1/evaluate.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v1/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v1/loss.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v1/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v1/utils.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v1/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v2/agent.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v2/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v2/dreamer_v2.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v2/dreamer_v2.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v2/evaluate.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v2/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v2/loss.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v2/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v2/utils.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v2/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v3/agent.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v3/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v3/dreamer_v3.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v3/dreamer_v3.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v3/evaluate.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v3/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v3/loss.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v3/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/dreamer_v3/utils.py` & `sheeprl-0.5.7/sheeprl/algos/dreamer_v3/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/droq/agent.py` & `sheeprl-0.5.7/sheeprl/algos/droq/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/droq/droq.py` & `sheeprl-0.5.7/sheeprl/algos/droq/droq.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/droq/evaluate.py` & `sheeprl-0.5.7/sheeprl/algos/droq/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/droq/utils.py` & `sheeprl-0.5.7/sheeprl/algos/droq/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv1/agent.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv1/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv1/evaluate.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv1/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv1/p2e_dv1_exploration.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv1/p2e_dv1_exploration.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv1/p2e_dv1_finetuning.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv1/p2e_dv1_finetuning.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv1/utils.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv1/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv2/agent.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv2/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv2/evaluate.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv2/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv2/p2e_dv2_exploration.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv2/p2e_dv2_exploration.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv2/p2e_dv2_finetuning.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv2/p2e_dv2_finetuning.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv2/utils.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv2/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv3/agent.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv3/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv3/evaluate.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv3/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv3/p2e_dv3_exploration.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv3/p2e_dv3_exploration.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv3/p2e_dv3_finetuning.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv3/p2e_dv3_finetuning.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/p2e_dv3/utils.py` & `sheeprl-0.5.7/sheeprl/algos/p2e_dv3/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/ppo/agent.py` & `sheeprl-0.5.7/sheeprl/algos/ppo/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/ppo/evaluate.py` & `sheeprl-0.5.7/sheeprl/algos/ppo/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/ppo/loss.py` & `sheeprl-0.5.7/sheeprl/algos/ppo/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/ppo/ppo.py` & `sheeprl-0.5.7/sheeprl/algos/ppo/ppo.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         if k in cfg.algo.cnn_keys.encoder:
             next_obs[k] = next_obs[k].reshape(cfg.env.num_envs, -1, *next_obs[k].shape[-2:])
         step_data[k] = next_obs[k][np.newaxis]
 
     for iter_num in range(start_iter, total_iters + 1):
         with torch.inference_mode():
             for _ in range(0, cfg.algo.rollout_steps):
-                policy_step += policy_steps_per_iter
+                policy_step += cfg.env.num_envs * world_size
 
                 # Measure environment interaction time: this considers both the model forward
                 # to get the action given the observation and the time taken into the environment
                 with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                     # Sample an action given the observation received by the environment
                     torch_obs = prepare_obs(
                         fabric, next_obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs
```

### Comparing `sheeprl-0.5.6/sheeprl/algos/ppo/ppo_decoupled.py` & `sheeprl-0.5.7/sheeprl/algos/ppo/ppo_decoupled.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/ppo/utils.py` & `sheeprl-0.5.7/sheeprl/algos/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/agent.py` & `sheeprl-0.5.7/sheeprl/algos/ppo_recurrent/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/evaluate.py` & `sheeprl-0.5.7/sheeprl/algos/ppo_recurrent/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/ppo_recurrent.py` & `sheeprl-0.5.7/sheeprl/algos/ppo_recurrent/ppo_recurrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
     prev_states = agent.initial_states
     prev_actions = np.zeros((1, cfg.env.num_envs, sum(actions_dim)))
     torch_prev_actions = torch.zeros(1, cfg.env.num_envs, sum(actions_dim), device=device, dtype=torch.float32)
 
     for iter_num in range(start_iter, total_iters + 1):
         with torch.inference_mode():
             for _ in range(0, cfg.algo.rollout_steps):
-                policy_step += policy_steps_per_iter
+                policy_step += cfg.env.num_envs * world_size
 
                 # Measure environment interaction time: this considers both the model forward
                 # to get the action given the observation and the time taken into the environment
                 with timer("Time/env_interaction_time", SumMetric, sync_on_compute=False):
                     # Sample an action given the observation received by the environment
                     # [Seq_len, Batch_size, D] --> [1, num_envs, D]
                     torch_obs = prepare_obs(fabric, obs, cnn_keys=cfg.algo.cnn_keys.encoder, num_envs=cfg.env.num_envs)
```

### Comparing `sheeprl-0.5.6/sheeprl/algos/ppo_recurrent/utils.py` & `sheeprl-0.5.7/sheeprl/algos/ppo_recurrent/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/sac/agent.py` & `sheeprl-0.5.7/sheeprl/algos/sac/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/sac/evaluate.py` & `sheeprl-0.5.7/sheeprl/algos/sac/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/sac/loss.py` & `sheeprl-0.5.7/sheeprl/algos/sac/loss.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/sac/sac.py` & `sheeprl-0.5.7/sheeprl/algos/sac/sac.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/sac/sac_decoupled.py` & `sheeprl-0.5.7/sheeprl/algos/sac/sac_decoupled.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/sac/utils.py` & `sheeprl-0.5.7/sheeprl/algos/sac/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/sac_ae/agent.py` & `sheeprl-0.5.7/sheeprl/algos/sac_ae/agent.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/sac_ae/evaluate.py` & `sheeprl-0.5.7/sheeprl/algos/sac_ae/evaluate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/sac_ae/sac_ae.py` & `sheeprl-0.5.7/sheeprl/algos/sac_ae/sac_ae.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/algos/sac_ae/utils.py` & `sheeprl-0.5.7/sheeprl/algos/sac_ae/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/available_agents.py` & `sheeprl-0.5.7/sheeprl/available_agents.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/cli.py` & `sheeprl-0.5.7/sheeprl/cli.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/algo/a2c.yaml` & `sheeprl-0.5.7/sheeprl/configs/algo/a2c.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v1.yaml` & `sheeprl-0.5.7/sheeprl/configs/algo/dreamer_v1.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v2.yaml` & `sheeprl-0.5.7/sheeprl/configs/algo/dreamer_v2.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/algo/dreamer_v3.yaml` & `sheeprl-0.5.7/sheeprl/configs/algo/dreamer_v3.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/algo/p2e_dv1.yaml` & `sheeprl-0.5.7/sheeprl/configs/algo/p2e_dv1.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/algo/p2e_dv2.yaml` & `sheeprl-0.5.7/sheeprl/configs/algo/p2e_dv2.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/algo/p2e_dv3.yaml` & `sheeprl-0.5.7/sheeprl/configs/algo/p2e_dv3.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/algo/ppo.yaml` & `sheeprl-0.5.7/sheeprl/configs/algo/ppo.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/algo/ppo_recurrent.yaml` & `sheeprl-0.5.7/sheeprl/configs/algo/ppo_recurrent.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/algo/sac.yaml` & `sheeprl-0.5.7/sheeprl/configs/algo/sac.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/algo/sac_ae.yaml` & `sheeprl-0.5.7/sheeprl/configs/algo/sac_ae.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/config.yaml` & `sheeprl-0.5.7/sheeprl/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/env/atari.yaml` & `sheeprl-0.5.7/sheeprl/configs/env/atari.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/env/diambra.yaml` & `sheeprl-0.5.7/sheeprl/configs/env/diambra.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/env/minerl.yaml` & `sheeprl-0.5.7/sheeprl/configs/env/minerl.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/a2c.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/a2c.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/a2c_benchmarks.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/a2c_benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v1.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v1.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v1_benchmarks.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v1_benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v2.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2_benchmarks.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v2_benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2_crafter.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v2_crafter.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v2_ms_pacman.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_L_doapp.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_L_doapp.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_L_doapp_128px_gray_combo_discrete.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_L_navigate.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_L_navigate.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_benchmarks.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_dmc_cartpole_swingup_sparse.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_dmc_cartpole_swingup_sparse.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_dmc_walker_walk.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/dreamer_v3_minedojo.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/dreamer_v3_minedojo.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv1_exploration.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv1_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv1_finetuning.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv1_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv2_exploration.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv2_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv2_finetuning.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv2_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv3_expl_L_doapp_128px_gray_combo_discrete_15Mexpl_20Mstps.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_exploration.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv3_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_finetuning.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv3_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/p2e_dv3_fntn_L_doapp_64px_gray_combo_discrete_5Mstps.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/p2e_dv3_fntn_L_doapp_64px_gray_combo_discrete_5Mstps.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/ppo.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/ppo.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/ppo_benchmarks.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/ppo_benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/ppo_super_mario_bros.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/ppo_super_mario_bros.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/sac.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/sac.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/exp/sac_benchmarks.yaml` & `sheeprl-0.5.7/sheeprl/configs/exp/sac_benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/metric/default.yaml` & `sheeprl-0.5.7/sheeprl/configs/metric/default.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/model_manager/dreamer_v2.yaml` & `sheeprl-0.5.7/sheeprl/configs/model_manager/dreamer_v2.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/model_manager/dreamer_v3.yaml` & `sheeprl-0.5.7/sheeprl/configs/model_manager/dreamer_v3.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv1_exploration.yaml` & `sheeprl-0.5.7/sheeprl/configs/model_manager/p2e_dv1_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv2_exploration.yaml` & `sheeprl-0.5.7/sheeprl/configs/model_manager/p2e_dv2_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv2_finetuning.yaml` & `sheeprl-0.5.7/sheeprl/configs/model_manager/p2e_dv2_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv3_exploration.yaml` & `sheeprl-0.5.7/sheeprl/configs/model_manager/p2e_dv3_exploration.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/configs/model_manager/p2e_dv3_finetuning.yaml` & `sheeprl-0.5.7/sheeprl/configs/model_manager/p2e_dv3_finetuning.yaml`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/data/buffers.py` & `sheeprl-0.5.7/sheeprl/data/buffers.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/envs/crafter.py` & `sheeprl-0.5.7/sheeprl/envs/crafter.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/envs/diambra.py` & `sheeprl-0.5.7/sheeprl/envs/diambra.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/envs/dmc.py` & `sheeprl-0.5.7/sheeprl/envs/dmc.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/envs/dummy.py` & `sheeprl-0.5.7/sheeprl/envs/dummy.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/envs/minedojo.py` & `sheeprl-0.5.7/sheeprl/envs/minedojo.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/envs/minerl.py` & `sheeprl-0.5.7/sheeprl/envs/minerl.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/envs/minerl_envs/backend.py` & `sheeprl-0.5.7/sheeprl/envs/minerl_envs/backend.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/envs/minerl_envs/navigate.py` & `sheeprl-0.5.7/sheeprl/envs/minerl_envs/navigate.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/envs/minerl_envs/obtain.py` & `sheeprl-0.5.7/sheeprl/envs/minerl_envs/obtain.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/envs/super_mario_bros.py` & `sheeprl-0.5.7/sheeprl/envs/super_mario_bros.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/envs/wrappers.py` & `sheeprl-0.5.7/sheeprl/envs/wrappers.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/models/models.py` & `sheeprl-0.5.7/sheeprl/models/models.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/optim/rmsprop_tf.py` & `sheeprl-0.5.7/sheeprl/optim/rmsprop_tf.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/callback.py` & `sheeprl-0.5.7/sheeprl/utils/callback.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/distribution.py` & `sheeprl-0.5.7/sheeprl/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/env.py` & `sheeprl-0.5.7/sheeprl/utils/env.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/fabric.py` & `sheeprl-0.5.7/sheeprl/utils/fabric.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/imports.py` & `sheeprl-0.5.7/sheeprl/utils/imports.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/logger.py` & `sheeprl-0.5.7/sheeprl/utils/logger.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/memmap.py` & `sheeprl-0.5.7/sheeprl/utils/memmap.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/metric.py` & `sheeprl-0.5.7/sheeprl/utils/metric.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/mlflow.py` & `sheeprl-0.5.7/sheeprl/utils/mlflow.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/model.py` & `sheeprl-0.5.7/sheeprl/utils/model.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/registry.py` & `sheeprl-0.5.7/sheeprl/utils/registry.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/timer.py` & `sheeprl-0.5.7/sheeprl/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl/utils/utils.py` & `sheeprl-0.5.7/sheeprl/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl.egg-info/PKG-INFO` & `sheeprl-0.5.7/sheeprl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheeprl
-Version: 0.5.6
+Version: 0.5.7
 Summary: High-quality, single file and distributed implementation of Deep Reinforcement Learning algorithms with production-friendly features
 Author-email: Federico Belotti <federico.belotti@orobix.com>, Davide Angioni <davide.angioni@orobix.com>, Refik Can Malli <refikcan.malli@orobix.com>, Michele Milesi <michele.milesi@orobix.com>
 Maintainer-email: Federico Belotti <federico.belotti@orobix.com>, Davide Angioni <davide.angioni@orobix.com>, Refik Can Malli <refikcan.malli@orobix.com>, Michele Milesi <michele.milesi@orobix.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `sheeprl-0.5.6/sheeprl.egg-info/SOURCES.txt` & `sheeprl-0.5.7/sheeprl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sheeprl-0.5.6/sheeprl.egg-info/requires.txt` & `sheeprl-0.5.7/sheeprl.egg-info/requires.txt`

 * *Files identical despite different names*

