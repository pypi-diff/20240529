# Comparing `tmp/eulith_web3-0.22.9.tar.gz` & `tmp/eulith_web3-0.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulith_web3-0.22.9.tar", last modified: Tue Mar 19 21:38:12 2024, max compression
+gzip compressed data, was "eulith_web3-0.27.0.tar", last modified: Wed May 29 19:04:19 2024, max compression
```

## Comparing `eulith_web3-0.22.9.tar` & `eulith_web3-0.27.0.tar`

### file list

```diff
@@ -1,158 +1,147 @@
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.085440 eulith_web3-0.22.9/
--rw-r--r--   0 kristian   (501) staff       (20)    19298 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/LICENSE
--rw-r--r--   0 kristian   (501) staff       (20)     1183 2024-03-19 21:38:12.085235 eulith_web3-0.22.9/PKG-INFO
--rw-r--r--   0 kristian   (501) staff       (20)      483 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/README.md
--rw-r--r--   0 kristian   (501) staff       (20)      641 2024-03-19 20:55:03.000000 eulith_web3-0.22.9/pyproject.toml
--rw-r--r--   0 kristian   (501) staff       (20)       38 2024-03-19 21:38:12.085484 eulith_web3-0.22.9/setup.cfg
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.041323 eulith_web3-0.22.9/src/
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.050831 eulith_web3-0.22.9/src/eulith_web3/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     2622 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/ace.py
--rw-r--r--   0 kristian   (501) staff       (20)     5180 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/asn_dump.py
--rw-r--r--   0 kristian   (501) staff       (20)      273 2024-02-03 00:16:54.000000 eulith_web3-0.22.9/src/eulith_web3/atomic.py
--rw-r--r--   0 kristian   (501) staff       (20)    12539 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/binding_generator.py
--rw-r--r--   0 kristian   (501) staff       (20)      181 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/common.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.060096 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/__init__.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.061515 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/convex/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/convex/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     5939 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/convex/i_booster.py
--rw-r--r--   0 kristian   (501) staff       (20)     3255 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/convex/i_convex_deposits.py
--rw-r--r--   0 kristian   (501) staff       (20)     9648 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/convex/i_reward_staking.py
--rw-r--r--   0 kristian   (501) staff       (20)    11940 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/convex/i_rewards.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.064976 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)    31380 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv.py
--rw-r--r--   0 kristian   (501) staff       (20)    31259 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv_gauge.py
--rw-r--r--   0 kristian   (501) staff       (20)    34191 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo.py
--rw-r--r--   0 kristian   (501) staff       (20)    35219 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo_gauge.py
--rw-r--r--   0 kristian   (501) staff       (20)    34193 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic.py
--rw-r--r--   0 kristian   (501) staff       (20)    35221 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic_gauge.py
--rw-r--r--   0 kristian   (501) staff       (20)    20520 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_three_pool.py
--rw-r--r--   0 kristian   (501) staff       (20)    36477 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_tri_crypto.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.068492 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)    13203 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_glp_manager.py
--rw-r--r--   0 kristian   (501) staff       (20)    17641 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_order_book.py
--rw-r--r--   0 kristian   (501) staff       (20)    40783 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_position_router.py
--rw-r--r--   0 kristian   (501) staff       (20)    20251 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_reader.py
--rw-r--r--   0 kristian   (501) staff       (20)     5755 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_reward_router.py
--rw-r--r--   0 kristian   (501) staff       (20)    13770 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_reward_tracker.py
--rw-r--r--   0 kristian   (501) staff       (20)     8639 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_router.py
--rw-r--r--   0 kristian   (501) staff       (20)    75065 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_vault.py
--rw-r--r--   0 kristian   (501) staff       (20)    15870 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_vault_price_feed.py
--rw-r--r--   0 kristian   (501) staff       (20)    16478 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_vault_utils.py
--rw-r--r--   0 kristian   (501) staff       (20)     7521 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_e_r_c20.py
--rw-r--r--   0 kristian   (501) staff       (20)    12164 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_e_r_c721.py
--rw-r--r--   0 kristian   (501) staff       (20)    14310 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_e_r_c721_enumerable.py
--rw-r--r--   0 kristian   (501) staff       (20)    14065 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_e_r_c721_metadata.py
--rw-r--r--   0 kristian   (501) staff       (20)    14832 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_e_r_c721_permit.py
--rw-r--r--   0 kristian   (501) staff       (20)     9235 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_e_r_c_detailed.py
--rw-r--r--   0 kristian   (501) staff       (20)    43634 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_lending_pool.py
--rw-r--r--   0 kristian   (501) staff       (20)    41038 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_nonfungible_position_manager.py
--rw-r--r--   0 kristian   (501) staff       (20)     1942 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_periphery_immutable_state.py
--rw-r--r--   0 kristian   (501) staff       (20)     3617 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_periphery_payments.py
--rw-r--r--   0 kristian   (501) staff       (20)     2211 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_pool_initializer.py
--rw-r--r--   0 kristian   (501) staff       (20)    11682 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_swap_router.py
--rw-r--r--   0 kristian   (501) staff       (20)    39907 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_uniswap_v3_pool.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.076734 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)      166 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/approx_params.py
--rw-r--r--   0 kristian   (501) staff       (20)      106 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/call3.py
--rw-r--r--   0 kristian   (501) staff       (20)     4720 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_diamond_loupe.py
--rw-r--r--   0 kristian   (501) staff       (20)     3542 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_e_r_c20_permit.py
--rw-r--r--   0 kristian   (501) staff       (20)    58050 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_action_add_remove_liq.py
--rw-r--r--   0 kristian   (501) staff       (20)    29865 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_action_mint_redeem.py
--rw-r--r--   0 kristian   (501) staff       (20)     4934 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_action_misc.py
--rw-r--r--   0 kristian   (501) staff       (20)    10373 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_action_storage_static.py
--rw-r--r--   0 kristian   (501) staff       (20)    22670 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_p_t.py
--rw-r--r--   0 kristian   (501) staff       (20)    29801 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_y_t.py
--rw-r--r--   0 kristian   (501) staff       (20)   144663 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_all_action.py
--rw-r--r--   0 kristian   (501) staff       (20)    13822 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_bulk_seller.py
--rw-r--r--   0 kristian   (501) staff       (20)     2111 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_gauge.py
--rw-r--r--   0 kristian   (501) staff       (20)     2528 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_interest_manager_y_t.py
--rw-r--r--   0 kristian   (501) staff       (20)    30200 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_market.py
--rw-r--r--   0 kristian   (501) staff       (20)     2542 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_market_swap_callback.py
--rw-r--r--   0 kristian   (501) staff       (20)    15287 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_principal_token.py
--rw-r--r--   0 kristian   (501) staff       (20)     3587 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_swap_aggregator.py
--rw-r--r--   0 kristian   (501) staff       (20)    28049 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_yield_token.py
--rw-r--r--   0 kristian   (501) staff       (20)     2418 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_reward_manager.py
--rw-r--r--   0 kristian   (501) staff       (20)    28299 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_standardized_yield.py
--rw-r--r--   0 kristian   (501) staff       (20)      108 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/multi_approval.py
--rw-r--r--   0 kristian   (501) staff       (20)      148 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/swap_data.py
--rw-r--r--   0 kristian   (501) staff       (20)      256 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/token_input.py
--rw-r--r--   0 kristian   (501) staff       (20)      261 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/token_output.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.076967 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/safe/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/safe/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)    92716 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/safe/i_safe.py
--rw-r--r--   0 kristian   (501) staff       (20)     8882 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/contract_bindings/w_e_t_h_interface.py
--rw-r--r--   0 kristian   (501) staff       (20)     1472 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/curve.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.077566 eulith_web3-0.22.9/src/eulith_web3/dydx/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2024-02-03 00:16:54.000000 eulith_web3-0.22.9/src/eulith_web3/dydx/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)      205 2024-02-03 00:16:54.000000 eulith_web3-0.22.9/src/eulith_web3/dydx/dydx.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.078813 eulith_web3-0.22.9/src/eulith_web3/dydx/v3/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2024-02-03 00:16:54.000000 eulith_web3-0.22.9/src/eulith_web3/dydx/v3/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     2628 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/dydx/v3/_core.py
--rw-r--r--   0 kristian   (501) staff       (20)     1494 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/dydx/v3/_eip712.py
--rw-r--r--   0 kristian   (501) staff       (20)     1430 2024-02-03 00:16:54.000000 eulith_web3-0.22.9/src/eulith_web3/dydx/v3/rpc.py
--rw-r--r--   0 kristian   (501) staff       (20)      326 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/dydx/v3/util.py
--rw-r--r--   0 kristian   (501) staff       (20)     3325 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/dydx/v3/v3.py
--rw-r--r--   0 kristian   (501) staff       (20)     4393 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/erc20.py
--rw-r--r--   0 kristian   (501) staff       (20)    49568 2024-03-19 18:45:35.000000 eulith_web3-0.22.9/src/eulith_web3/eulith_service.py
--rw-r--r--   0 kristian   (501) staff       (20)    58541 2024-03-19 18:45:35.000000 eulith_web3-0.22.9/src/eulith_web3/eulith_web3.py
--rw-r--r--   0 kristian   (501) staff       (20)      608 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/exceptions.py
--rw-r--r--   0 kristian   (501) staff       (20)     2620 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/fireblocks.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.079030 eulith_web3-0.22.9/src/eulith_web3/gmx/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2024-02-03 00:16:54.000000 eulith_web3-0.22.9/src/eulith_web3/gmx/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)      664 2024-02-03 00:16:54.000000 eulith_web3-0.22.9/src/eulith_web3/gmx/gmx.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.079331 eulith_web3-0.22.9/src/eulith_web3/gmx/v1/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2024-02-03 00:16:54.000000 eulith_web3-0.22.9/src/eulith_web3/gmx/v1/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)    29189 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/gmx/v1/v1.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.080265 eulith_web3-0.22.9/src/eulith_web3/gmx/v2/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2024-02-03 00:16:54.000000 eulith_web3-0.22.9/src/eulith_web3/gmx/v2/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     3495 2024-02-16 16:28:49.000000 eulith_web3-0.22.9/src/eulith_web3/gmx/v2/rpc.py
--rw-r--r--   0 kristian   (501) staff       (20)     1723 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/gmx/v2/v2.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.081072 eulith_web3-0.22.9/src/eulith_web3/hyperliquid/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2024-03-12 01:50:37.000000 eulith_web3-0.22.9/src/eulith_web3/hyperliquid/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     4069 2024-03-15 03:27:42.000000 eulith_web3-0.22.9/src/eulith_web3/hyperliquid/_eip712.py
--rw-r--r--   0 kristian   (501) staff       (20)     3616 2024-03-15 03:27:42.000000 eulith_web3-0.22.9/src/eulith_web3/hyperliquid/hyperliquid.py
--rw-r--r--   0 kristian   (501) staff       (20)      856 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/hyperliquid/rpc.py
--rw-r--r--   0 kristian   (501) staff       (20)     2225 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/kms.py
--rw-r--r--   0 kristian   (501) staff       (20)     2502 2024-03-19 16:11:25.000000 eulith_web3-0.22.9/src/eulith_web3/ledger.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.083192 eulith_web3-0.22.9/src/eulith_web3/ledger_interface/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/ledger_interface/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     4149 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/ledger_interface/account.py
--rw-r--r--   0 kristian   (501) staff       (20)     6647 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/ledger_interface/comms.py
--rw-r--r--   0 kristian   (501) staff       (20)     2325 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/ledger_interface/constants.py
--rw-r--r--   0 kristian   (501) staff       (20)     3929 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/ledger_interface/exceptions.py
--rw-r--r--   0 kristian   (501) staff       (20)     5230 2024-03-19 16:11:18.000000 eulith_web3-0.22.9/src/eulith_web3/ledger_interface/messages.py
--rw-r--r--   0 kristian   (501) staff       (20)    27708 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/ledger_interface/objects.py
--rw-r--r--   0 kristian   (501) staff       (20)    11115 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/ledger_interface/transactions.py
--rw-r--r--   0 kristian   (501) staff       (20)     6807 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/ledger_interface/utils.py
--rw-r--r--   0 kristian   (501) staff       (20)     2122 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/lightsim.py
--rw-r--r--   0 kristian   (501) staff       (20)     6466 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/pendle.py
--rw-r--r--   0 kristian   (501) staff       (20)      936 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/requests.py
--rw-r--r--   0 kristian   (501) staff       (20)      968 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/response.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.083427 eulith_web3-0.22.9/src/eulith_web3/safe_utils/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/safe_utils/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     1503 2024-03-19 18:45:35.000000 eulith_web3-0.22.9/src/eulith_web3/safe_utils/transaction_data.py
--rw-r--r--   0 kristian   (501) staff       (20)      471 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/signer.py
--rw-r--r--   0 kristian   (501) staff       (20)     7440 2024-03-18 23:31:34.000000 eulith_web3-0.22.9/src/eulith_web3/signing.py
--rw-r--r--   0 kristian   (501) staff       (20)     1250 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/swap.py
--rw-r--r--   0 kristian   (501) staff       (20)     4267 2024-03-19 16:11:39.000000 eulith_web3-0.22.9/src/eulith_web3/trezor.py
--rw-r--r--   0 kristian   (501) staff       (20)     6062 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/uniswap.py
--rw-r--r--   0 kristian   (501) staff       (20)    14005 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/websocket.py
--rw-r--r--   0 kristian   (501) staff       (20)     1624 2023-11-16 20:52:40.000000 eulith_web3-0.22.9/src/eulith_web3/whitelists.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.084438 eulith_web3-0.22.9/src/eulith_web3/whitelists_v2/
--rw-r--r--   0 kristian   (501) staff       (20)      136 2023-12-20 20:05:47.000000 eulith_web3-0.22.9/src/eulith_web3/whitelists_v2/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)      511 2023-12-20 20:05:47.000000 eulith_web3-0.22.9/src/eulith_web3/whitelists_v2/_core.py
--rw-r--r--   0 kristian   (501) staff       (20)     3894 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/src/eulith_web3/whitelists_v2/_eip712.py
--rw-r--r--   0 kristian   (501) staff       (20)     1192 2023-12-20 20:05:47.000000 eulith_web3-0.22.9/src/eulith_web3/whitelists_v2/rpc.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.084958 eulith_web3-0.22.9/src/eulith_web3.egg-info/
--rw-r--r--   0 kristian   (501) staff       (20)     1183 2024-03-19 21:38:12.000000 eulith_web3-0.22.9/src/eulith_web3.egg-info/PKG-INFO
--rw-r--r--   0 kristian   (501) staff       (20)     6169 2024-03-19 21:38:12.000000 eulith_web3-0.22.9/src/eulith_web3.egg-info/SOURCES.txt
--rw-r--r--   0 kristian   (501) staff       (20)        1 2024-03-19 21:38:12.000000 eulith_web3-0.22.9/src/eulith_web3.egg-info/dependency_links.txt
--rw-r--r--   0 kristian   (501) staff       (20)      119 2024-03-19 21:38:12.000000 eulith_web3-0.22.9/src/eulith_web3.egg-info/requires.txt
--rw-r--r--   0 kristian   (501) staff       (20)       12 2024-03-19 21:38:12.000000 eulith_web3-0.22.9/src/eulith_web3.egg-info/top_level.txt
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-03-19 21:38:12.084576 eulith_web3-0.22.9/tests/
--rw-r--r--   0 kristian   (501) staff       (20)      898 2024-03-14 17:08:00.000000 eulith_web3-0.22.9/tests/test_guard.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.919272 eulith_web3-0.27.0/
+-rw-r--r--   0 kristian   (501) staff       (20)    19298 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/LICENSE
+-rw-r--r--   0 kristian   (501) staff       (20)     1183 2024-05-29 19:04:19.919066 eulith_web3-0.27.0/PKG-INFO
+-rw-r--r--   0 kristian   (501) staff       (20)      483 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/README.md
+-rw-r--r--   0 kristian   (501) staff       (20)      641 2024-05-29 00:14:49.000000 eulith_web3-0.27.0/pyproject.toml
+-rw-r--r--   0 kristian   (501) staff       (20)       38 2024-05-29 19:04:19.919312 eulith_web3-0.27.0/setup.cfg
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.883054 eulith_web3-0.27.0/src/
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.892245 eulith_web3-0.27.0/src/eulith_web3/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2785 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/ace.py
+-rw-r--r--   0 kristian   (501) staff       (20)      273 2024-02-03 00:16:54.000000 eulith_web3-0.27.0/src/eulith_web3/atomic.py
+-rw-r--r--   0 kristian   (501) staff       (20)      181 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/common.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.894532 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/__init__.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.895699 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/convex/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/convex/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5977 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/convex/i_booster.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3267 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/convex/i_convex_deposits.py
+-rw-r--r--   0 kristian   (501) staff       (20)     9671 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/convex/i_reward_staking.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11963 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/convex/i_rewards.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.898727 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)    31380 2024-03-14 17:08:00.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv.py
+-rw-r--r--   0 kristian   (501) staff       (20)    31273 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv_gauge.py
+-rw-r--r--   0 kristian   (501) staff       (20)    34191 2024-03-14 17:08:00.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo.py
+-rw-r--r--   0 kristian   (501) staff       (20)    35233 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo_gauge.py
+-rw-r--r--   0 kristian   (501) staff       (20)    34193 2024-03-14 17:08:00.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic.py
+-rw-r--r--   0 kristian   (501) staff       (20)    35235 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic_gauge.py
+-rw-r--r--   0 kristian   (501) staff       (20)    20535 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_three_pool.py
+-rw-r--r--   0 kristian   (501) staff       (20)    36500 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_tri_crypto.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.902167 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)    13226 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_glp_manager.py
+-rw-r--r--   0 kristian   (501) staff       (20)    17665 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_order_book.py
+-rw-r--r--   0 kristian   (501) staff       (20)    40806 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_position_router.py
+-rw-r--r--   0 kristian   (501) staff       (20)    20284 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_reader.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5778 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_reward_router.py
+-rw-r--r--   0 kristian   (501) staff       (20)    13793 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_reward_tracker.py
+-rw-r--r--   0 kristian   (501) staff       (20)     8662 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_router.py
+-rw-r--r--   0 kristian   (501) staff       (20)    75836 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_vault.py
+-rw-r--r--   0 kristian   (501) staff       (20)    15893 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_vault_price_feed.py
+-rw-r--r--   0 kristian   (501) staff       (20)    16506 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_vault_utils.py
+-rw-r--r--   0 kristian   (501) staff       (20)     7521 2024-03-14 17:08:00.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/i_e_r_c20.py
+-rw-r--r--   0 kristian   (501) staff       (20)     9235 2024-03-14 17:08:00.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/i_e_r_c_detailed.py
+-rw-r--r--   0 kristian   (501) staff       (20)    39883 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/i_uniswap_v3_pool.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.909606 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)      178 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/approx_params.py
+-rw-r--r--   0 kristian   (501) staff       (20)      118 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/call3.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4734 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_diamond_loupe.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4012 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_e_r_c20_permit.py
+-rw-r--r--   0 kristian   (501) staff       (20)    57918 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_action_add_remove_liq.py
+-rw-r--r--   0 kristian   (501) staff       (20)    29733 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_action_mint_redeem.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4730 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_action_misc.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10174 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_action_storage_static.py
+-rw-r--r--   0 kristian   (501) staff       (20)    22466 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_p_t.py
+-rw-r--r--   0 kristian   (501) staff       (20)    29597 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_y_t.py
+-rw-r--r--   0 kristian   (501) staff       (20)   144461 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_all_action.py
+-rw-r--r--   0 kristian   (501) staff       (20)    13618 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_bulk_seller.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2123 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_gauge.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1871 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_interest_manager_y_t.py
+-rw-r--r--   0 kristian   (501) staff       (20)    30216 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_market.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2338 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_market_swap_callback.py
+-rw-r--r--   0 kristian   (501) staff       (20)    15083 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_principal_token.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3383 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_swap_aggregator.py
+-rw-r--r--   0 kristian   (501) staff       (20)    27397 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_yield_token.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1761 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_reward_manager.py
+-rw-r--r--   0 kristian   (501) staff       (20)    28100 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_standardized_yield.py
+-rw-r--r--   0 kristian   (501) staff       (20)      120 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/multi_approval.py
+-rw-r--r--   0 kristian   (501) staff       (20)      160 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/swap_data.py
+-rw-r--r--   0 kristian   (501) staff       (20)      195 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/token_input.py
+-rw-r--r--   0 kristian   (501) staff       (20)      200 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/token_output.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.909839 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/safe/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/safe/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)    92742 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/safe/i_safe.py
+-rw-r--r--   0 kristian   (501) staff       (20)     8882 2024-03-14 17:08:00.000000 eulith_web3-0.27.0/src/eulith_web3/contract_bindings/w_e_t_h_interface.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1549 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/curve.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.910601 eulith_web3-0.27.0/src/eulith_web3/dydx/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2024-02-03 00:16:54.000000 eulith_web3-0.27.0/src/eulith_web3/dydx/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)      205 2024-02-03 00:16:54.000000 eulith_web3-0.27.0/src/eulith_web3/dydx/dydx.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.912016 eulith_web3-0.27.0/src/eulith_web3/dydx/v3/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2024-02-03 00:16:54.000000 eulith_web3-0.27.0/src/eulith_web3/dydx/v3/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2853 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/dydx/v3/_core.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1494 2024-03-14 17:08:00.000000 eulith_web3-0.27.0/src/eulith_web3/dydx/v3/_eip712.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1430 2024-02-03 00:16:54.000000 eulith_web3-0.27.0/src/eulith_web3/dydx/v3/rpc.py
+-rw-r--r--   0 kristian   (501) staff       (20)      326 2024-03-14 17:08:00.000000 eulith_web3-0.27.0/src/eulith_web3/dydx/v3/util.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2942 2024-04-03 15:02:37.000000 eulith_web3-0.27.0/src/eulith_web3/dydx/v3/v3.py
+-rw-r--r--   0 kristian   (501) staff       (20)      372 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/eip712_types.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4428 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/erc20.py
+-rw-r--r--   0 kristian   (501) staff       (20)    34003 2024-05-29 00:14:49.000000 eulith_web3-0.27.0/src/eulith_web3/eulith_service.py
+-rw-r--r--   0 kristian   (501) staff       (20)    51279 2024-05-29 00:14:49.000000 eulith_web3-0.27.0/src/eulith_web3/eulith_web3.py
+-rw-r--r--   0 kristian   (501) staff       (20)      646 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/exceptions.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2752 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/fireblocks.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.912343 eulith_web3-0.27.0/src/eulith_web3/gmx/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2024-02-03 00:16:54.000000 eulith_web3-0.27.0/src/eulith_web3/gmx/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)      487 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/gmx/gmx.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.912667 eulith_web3-0.27.0/src/eulith_web3/gmx/v1/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2024-02-03 00:16:54.000000 eulith_web3-0.27.0/src/eulith_web3/gmx/v1/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)    26640 2024-04-03 15:02:37.000000 eulith_web3-0.27.0/src/eulith_web3/gmx/v1/v1.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.913607 eulith_web3-0.27.0/src/eulith_web3/gmx/v2/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2024-02-03 00:16:54.000000 eulith_web3-0.27.0/src/eulith_web3/gmx/v2/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3495 2024-02-16 16:28:49.000000 eulith_web3-0.27.0/src/eulith_web3/gmx/v2/rpc.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1490 2024-04-03 15:02:37.000000 eulith_web3-0.27.0/src/eulith_web3/gmx/v2/v2.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.914524 eulith_web3-0.27.0/src/eulith_web3/hyperliquid/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2024-03-12 01:50:37.000000 eulith_web3-0.27.0/src/eulith_web3/hyperliquid/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4310 2024-04-03 15:02:37.000000 eulith_web3-0.27.0/src/eulith_web3/hyperliquid/_eip712.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3880 2024-04-03 15:02:37.000000 eulith_web3-0.27.0/src/eulith_web3/hyperliquid/hyperliquid.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1256 2024-04-03 15:02:37.000000 eulith_web3-0.27.0/src/eulith_web3/hyperliquid/rpc.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2309 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/kms.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2872 2024-04-03 15:02:37.000000 eulith_web3-0.27.0/src/eulith_web3/ledger.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.916548 eulith_web3-0.27.0/src/eulith_web3/ledger_interface/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/ledger_interface/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4149 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/ledger_interface/account.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6647 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/ledger_interface/comms.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2325 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/ledger_interface/constants.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3929 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/ledger_interface/exceptions.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5230 2024-03-19 16:11:18.000000 eulith_web3-0.27.0/src/eulith_web3/ledger_interface/messages.py
+-rw-r--r--   0 kristian   (501) staff       (20)    27708 2024-03-14 17:08:00.000000 eulith_web3-0.27.0/src/eulith_web3/ledger_interface/objects.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11115 2024-03-14 17:08:00.000000 eulith_web3-0.27.0/src/eulith_web3/ledger_interface/transactions.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6807 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/ledger_interface/utils.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2307 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/lightsim.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5743 2024-04-03 15:02:37.000000 eulith_web3-0.27.0/src/eulith_web3/pendle.py
+-rw-r--r--   0 kristian   (501) staff       (20)      936 2024-03-14 17:08:00.000000 eulith_web3-0.27.0/src/eulith_web3/requests.py
+-rw-r--r--   0 kristian   (501) staff       (20)      984 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/response.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.916783 eulith_web3-0.27.0/src/eulith_web3/safe_utils/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-11-16 20:52:40.000000 eulith_web3-0.27.0/src/eulith_web3/safe_utils/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1649 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/safe_utils/transaction_data.py
+-rw-r--r--   0 kristian   (501) staff       (20)      787 2024-04-03 15:02:37.000000 eulith_web3-0.27.0/src/eulith_web3/signer.py
+-rw-r--r--   0 kristian   (501) staff       (20)     7766 2024-04-03 15:02:37.000000 eulith_web3-0.27.0/src/eulith_web3/signing.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1263 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/swap.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4527 2024-04-03 15:02:37.000000 eulith_web3-0.27.0/src/eulith_web3/trezor.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6115 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/uniswap.py
+-rw-r--r--   0 kristian   (501) staff       (20)    14844 2024-04-03 15:02:37.000000 eulith_web3-0.27.0/src/eulith_web3/websocket.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1745 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/whitelists.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.918070 eulith_web3-0.27.0/src/eulith_web3/whitelists_v2/
+-rw-r--r--   0 kristian   (501) staff       (20)      136 2023-12-20 20:05:47.000000 eulith_web3-0.27.0/src/eulith_web3/whitelists_v2/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)      511 2023-12-20 20:05:47.000000 eulith_web3-0.27.0/src/eulith_web3/whitelists_v2/_core.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4148 2024-03-28 23:19:25.000000 eulith_web3-0.27.0/src/eulith_web3/whitelists_v2/_eip712.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1192 2023-12-20 20:05:47.000000 eulith_web3-0.27.0/src/eulith_web3/whitelists_v2/rpc.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.918781 eulith_web3-0.27.0/src/eulith_web3.egg-info/
+-rw-r--r--   0 kristian   (501) staff       (20)     1183 2024-05-29 19:04:19.000000 eulith_web3-0.27.0/src/eulith_web3.egg-info/PKG-INFO
+-rw-r--r--   0 kristian   (501) staff       (20)     5567 2024-05-29 19:04:19.000000 eulith_web3-0.27.0/src/eulith_web3.egg-info/SOURCES.txt
+-rw-r--r--   0 kristian   (501) staff       (20)        1 2024-05-29 19:04:19.000000 eulith_web3-0.27.0/src/eulith_web3.egg-info/dependency_links.txt
+-rw-r--r--   0 kristian   (501) staff       (20)      119 2024-05-29 19:04:19.000000 eulith_web3-0.27.0/src/eulith_web3.egg-info/requires.txt
+-rw-r--r--   0 kristian   (501) staff       (20)       12 2024-05-29 19:04:19.000000 eulith_web3-0.27.0/src/eulith_web3.egg-info/top_level.txt
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2024-05-29 19:04:19.918291 eulith_web3-0.27.0/tests/
+-rw-r--r--   0 kristian   (501) staff       (20)      898 2024-03-14 17:08:00.000000 eulith_web3-0.27.0/tests/test_guard.py
```

### Comparing `eulith_web3-0.22.9/LICENSE` & `eulith_web3-0.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/PKG-INFO` & `eulith_web3-0.27.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulith_web3
-Version: 0.22.9
+Version: 0.27.0
 Summary: A Web3.py compatible wrapper library for Eulith clients
 Author-email: Eulith Team <kristian@eulith.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `eulith_web3-0.22.9/pyproject.toml` & `eulith_web3-0.27.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [project]
-version = "0.22.9"
+version = "0.27.0"
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 dependencies = ["web3 >= 5.31.1, < 7.0", "boto3", "asn1", "uuid", "requests", "hexbytes", "cytoolz", "botocore", "fireblocks-sdk", "websocket-client", "ledgerblue", "trezor"]
 description = "A Web3.py compatible wrapper library for Eulith clients"
 name = "eulith_web3"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/ace.py` & `eulith_web3-0.27.0/src/eulith_web3/ace.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from dataclasses import dataclass
-from typing import TypedDict
+from typing import Any, Dict, TypedDict
 
 from eth_account.messages import encode_typed_data
 from eth_utils import keccak
 
+from eulith_web3.eip712_types import Eip712Data, Eip712Domain, Eip712Field
+
 
 @dataclass
 class AceImmediateTx:
     chain_id: int
     nonce: int
     max_priority_fee_per_gas: int
     max_fee_per_gas: int
     gas_limit: int
     data: bytes
 
     @classmethod
-    def from_json(cls, data: dict) -> "AceImmediateTx":
+    def from_json(cls, data: Dict[str, Any]) -> "AceImmediateTx":
         return cls(
             chain_id=data["chain_id"],
             nonce=int(data["nonce"], base=16),
             max_priority_fee_per_gas=int(data["max_priority_fee_per_gas"], base=16),
             max_fee_per_gas=int(data["max_fee_per_gas"], base=16),
             gas_limit=int(data["gas_limit"], base=16),
             data=bytes.fromhex(data["data"][2:]),
         )
 
-    def to_json(self) -> dict:
+    def to_json(self) -> Dict[str, Any]:
         return dict(
             chain_id=self.chain_id,
             nonce=hex(self.nonce),
             max_priority_fee_per_gas=hex(self.max_priority_fee_per_gas),
             max_fee_per_gas=hex(self.max_fee_per_gas),
             gas_limit=hex(self.gas_limit),
             data="0x" + self.data.hex(),
@@ -38,46 +40,46 @@
 
 class AcePingResponse(TypedDict):
     ping_time_millis: int
     auth_address: str
     ui_address: str
 
 
-def get_ace_immediate_tx_typed_data(message: AceImmediateTx) -> dict:
+def get_ace_immediate_tx_typed_data(message: AceImmediateTx) -> Eip712Data:
     # Should match the EIP-712 definition in src/ace/immediate_tx.rs
     types = {
         "EIP712Domain": [
-            {"name": "name", "type": "string"},
-            {"name": "version", "type": "string"},
+            Eip712Field(name="name", type="string"),
+            Eip712Field(name="version", type="string"),
         ],
         "AceImmediateTx": [
-            {"name": "chainId", "type": "int64"},
-            {"name": "nonce", "type": "uint256"},
-            {"name": "maxPriorityFeePerGas", "type": "uint256"},
-            {"name": "maxFeePerGas", "type": "uint256"},
-            {"name": "gasLimit", "type": "uint256"},
-            {"name": "data", "type": "bytes"},
+            Eip712Field(name="chainId", type="int64"),
+            Eip712Field(name="nonce", type="uint256"),
+            Eip712Field(name="maxPriorityFeePerGas", type="uint256"),
+            Eip712Field(name="maxFeePerGas", type="uint256"),
+            Eip712Field(name="gasLimit", type="uint256"),
+            Eip712Field(name="data", type="bytes"),
         ],
     }
 
-    payload = {
-        "types": types,
-        "primaryType": "AceImmediateTx",
-        "domain": {"name": "EulithAceImmediateTx", "version": "1"},
-        "message": {
+    payload = Eip712Data(
+        types=types,
+        primaryType="AceImmediateTx",
+        domain=Eip712Domain(name="EulithAceImmediateTx", version="1"),
+        message={
             "chainId": message.chain_id,
             "nonce": message.nonce,
             "maxPriorityFeePerGas": message.max_priority_fee_per_gas,
             "maxFeePerGas": message.max_fee_per_gas,
             "gasLimit": message.gas_limit,
             "data": message.data,
         },
-    }
+    )
 
     return payload
 
 
 def get_ace_immediate_tx_hash(ace_immediate_tx: AceImmediateTx) -> bytes:
     signable_message = encode_typed_data(
-        full_message=get_ace_immediate_tx_typed_data(ace_immediate_tx)
+        full_message=dict(get_ace_immediate_tx_typed_data(ace_immediate_tx))
     )
     return keccak(b"\x19\x01" + signable_message.header + signable_message.body)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/convex/i_booster.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/convex/i_booster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
@@ -104,22 +104,22 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.owner().call()
 
-    def pool_info(self, _pid: int) -> TxParams:
+    def pool_info(self, _pid: int) -> Tuple[str, str, str, str, str, bool]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.poolInfo(_pid).build_transaction()
+        return c.functions.poolInfo(_pid).call()
 
     def set_vote_delegate(
         self, _vote_delegate: str, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/convex/i_convex_deposits.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/convex/i_convex_deposits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/convex/i_reward_staking.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/convex/i_reward_staking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/convex/i_rewards.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/convex/i_rewards.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv_gauge.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv_gauge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
@@ -642,22 +642,22 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.name().call()
 
-    def period(self) -> TxParams:
+    def period(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.period().build_transaction()
+        return c.functions.period().call()
 
     def period_timestamp(self, arg0: int) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
@@ -669,22 +669,22 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.reward_count().call()
 
-    def reward_data(self, arg0: str) -> TxParams:
+    def reward_data(self, arg0: str) -> Tuple[str, str, int, int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.reward_data(arg0).build_transaction()
+        return c.functions.reward_data(arg0).call()
 
     def reward_integral_for(self, arg0: str, arg1: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo_gauge.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo_gauge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
@@ -714,22 +714,22 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.nonces(arg0).call()
 
-    def period(self) -> TxParams:
+    def period(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.period().build_transaction()
+        return c.functions.period().call()
 
     def period_timestamp(self, arg0: int) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
@@ -762,22 +762,22 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.reward_count().call()
 
-    def reward_data(self, arg0: str) -> TxParams:
+    def reward_data(self, arg0: str) -> Tuple[str, str, int, int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.reward_data(arg0).build_transaction()
+        return c.functions.reward_data(arg0).call()
 
     def reward_integral_for(self, arg0: str, arg1: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic_gauge.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic_gauge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
@@ -714,22 +714,22 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.nonces(arg0).call()
 
-    def period(self) -> TxParams:
+    def period(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.period().build_transaction()
+        return c.functions.period().call()
 
     def period_timestamp(self, arg0: int) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
@@ -762,22 +762,22 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.reward_count().call()
 
-    def reward_data(self, arg0: str) -> TxParams:
+    def reward_data(self, arg0: str) -> Tuple[str, str, int, int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.reward_data(arg0).build_transaction()
+        return c.functions.reward_data(arg0).call()
 
     def reward_integral_for(self, arg0: str, arg1: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_three_pool.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_three_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
@@ -346,15 +346,15 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.calc_token_amount(amounts, deposit).call()
 
-    def calc_withdraw_one_coin(self, _token_amount: int, i: None) -> int:
+    def calc_withdraw_one_coin(self, _token_amount: int, i: int) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.calc_withdraw_one_coin(_token_amount, i).call()
@@ -366,16 +366,16 @@
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.coins(arg0).call()
 
     def exchange(
         self,
-        i: None,
-        j: None,
+        i: int,
+        j: int,
         dx: int,
         min_dy: int,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
@@ -436,24 +436,24 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.future_owner().call()
 
-    def get_dy(self, i: None, j: None, dx: int) -> int:
+    def get_dy(self, i: int, j: int, dx: int) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.get_dy(i, j, dx).call()
 
-    def get_dy_underlying(self, i: None, j: None, dx: int) -> int:
+    def get_dy_underlying(self, i: int, j: int, dx: int) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.get_dy_underlying(i, j, dx).call()
@@ -525,15 +525,15 @@
         return c.functions.remove_liquidity_imbalance(
             amounts, max_burn_amount
         ).build_transaction(override_tx_parameters)
 
     def remove_liquidity_one_coin(
         self,
         _token_amount: int,
-        i: None,
+        i: int,
         min_amount: int,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/curve/curve_v2_tri_crypto.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/curve/curve_v2_tri_crypto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_glp_manager.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_glp_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_order_book.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_order_book.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
@@ -390,15 +390,15 @@
             _should_wrap,
         ).build_transaction(override_tx_parameters)
 
     def execute_decrease_order(
         self,
         a0: str,
         a1: int,
-        a2: None,
+        a2: str,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
@@ -407,15 +407,15 @@
             override_tx_parameters
         )
 
     def execute_increase_order(
         self,
         a0: str,
         a1: int,
-        a2: None,
+        a2: str,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
@@ -424,52 +424,52 @@
             override_tx_parameters
         )
 
     def execute_swap_order(
         self,
         a0: str,
         a1: int,
-        a2: None,
+        a2: str,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.executeSwapOrder(a0, a1, a2).build_transaction(
             override_tx_parameters
         )
 
     def get_decrease_order(
         self, _account: str, _order_index: int
-    ) -> (str, int, str, int, bool, int, bool, int):
+    ) -> Tuple[str, int, str, int, bool, int, bool, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getDecreaseOrder(_account, _order_index).call()
 
     def get_increase_order(
         self, _account: str, _order_index: int
-    ) -> (str, int, str, str, int, bool, int, bool, int):
+    ) -> Tuple[str, int, str, str, int, bool, int, bool, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getIncreaseOrder(_account, _order_index).call()
 
     def get_swap_order(
         self, _account: str, _order_index: int
-    ) -> (str, str, str, int, int, int, bool, bool, int):
+    ) -> Tuple[str, str, str, int, int, int, bool, bool, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getSwapOrder(_account, _order_index).call()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_position_router.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_position_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_reader.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
@@ -326,29 +326,29 @@
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
     def get_amount_out(
-        self, _vault: str, _token_in: str, _token_out: str, _amount_in: int
-    ) -> (int, int):
+        self, _vault: Any, _token_in: str, _token_out: str, _amount_in: int
+    ) -> Tuple[int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getAmountOut(
             _vault, _token_in, _token_out, _amount_in
         ).call()
 
     def get_fee_basis_points(
-        self, _vault: str, _token_in: str, _token_out: str, _amount_in: int
-    ) -> (int, int, int):
+        self, _vault: Any, _token_in: str, _token_out: str, _amount_in: int
+    ) -> Tuple[int, int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getFeeBasisPoints(
@@ -375,15 +375,15 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getFundingRates(_vault, _weth, _tokens).call()
 
-    def get_max_amount_in(self, _vault: str, _token_in: str, _token_out: str) -> int:
+    def get_max_amount_in(self, _vault: Any, _token_in: str, _token_out: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getMaxAmountIn(_vault, _token_in, _token_out).call()
@@ -411,15 +411,15 @@
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getPositions(
             _vault, _account, _collateral_tokens, _index_tokens, _is_long
         ).call()
 
-    def get_prices(self, _price_feed: str, _tokens: List[str]) -> List[int]:
+    def get_prices(self, _price_feed: Any, _tokens: List[str]) -> List[int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getPrices(_price_feed, _tokens).call()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_reward_router.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_reward_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_reward_tracker.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_reward_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_router.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_vault.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
@@ -238,14 +238,23 @@
                     {"internalType": "uint256", "name": "", "type": "uint256"},
                 ],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
+                    {"internalType": "uint256", "name": "_sizeDelta", "type": "uint256"}
+                ],
+                "name": "getPositionFee",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [
                     {"internalType": "address", "name": "_token", "type": "address"},
                     {
                         "internalType": "uint256",
                         "name": "_usdgAmount",
                         "type": "uint256",
                     },
                 ],
@@ -1116,15 +1125,15 @@
     def get_delta(
         self,
         _index_token: str,
         _size: int,
         _average_price: int,
         _is_long: bool,
         _last_increased_time: int,
-    ) -> (bool, int):
+    ) -> Tuple[bool, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getDelta(
@@ -1174,25 +1183,34 @@
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getNextFundingRate(_token).call()
 
     def get_position(
         self, _account: str, _collateral_token: str, _index_token: str, _is_long: bool
-    ) -> (int, int, int, int, int, int, bool, int):
+    ) -> Tuple[int, int, int, int, int, int, bool, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getPosition(
             _account, _collateral_token, _index_token, _is_long
         ).call()
 
+    def get_position_fee(self, _size_delta: int) -> int:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.getPositionFee(_size_delta).call()
+
     def get_redemption_amount(self, _token: str, _usdg_amount: int) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
@@ -1758,15 +1776,15 @@
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.setUsdgAmount(_token, _amount).build_transaction(
             override_tx_parameters
         )
 
     def set_vault_utils(
-        self, _vault_utils: str, override_tx_parameters: Optional[TxParams] = None
+        self, _vault_utils: Any, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
@@ -1920,15 +1938,15 @@
     def validate_liquidation(
         self,
         _account: str,
         _collateral_token: str,
         _index_token: str,
         _is_long: bool,
         _raise: bool,
-    ) -> (int, int):
+    ) -> Tuple[int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.validateLiquidation(
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_vault_price_feed.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_vault_price_feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/gmx/i_vault_utils.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/gmx/i_vault_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
@@ -429,15 +429,15 @@
     def validate_liquidation(
         self,
         _account: str,
         _collateral_token: str,
         _index_token: str,
         _is_long: bool,
         _raise: bool,
-    ) -> (int, int):
+    ) -> Tuple[int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.validateLiquidation(
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_e_r_c20.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/i_e_r_c20.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_e_r_c721.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/i_e_r_c_detailed.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Optional, Union
 from eth_typing import Address, ChecksumAddress
-from web3 import Web3
 from web3.types import TxParams
+from web3 import Web3
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class IERC721:
+class IERCDetailed:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
@@ -24,311 +24,232 @@
                         "internalType": "address",
                         "name": "owner",
                         "type": "address",
                     },
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "approved",
+                        "name": "spender",
                         "type": "address",
                     },
                     {
-                        "indexed": True,
+                        "indexed": False,
                         "internalType": "uint256",
-                        "name": "tokenId",
+                        "name": "value",
                         "type": "uint256",
                     },
                 ],
                 "name": "Approval",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "owner",
-                        "type": "address",
-                    },
-                    {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "operator",
-                        "type": "address",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "bool",
-                        "name": "approved",
-                        "type": "bool",
-                    },
-                ],
-                "name": "ApprovalForAll",
-                "type": "event",
-            },
-            {
-                "anonymous": False,
-                "inputs": [
-                    {
-                        "indexed": True,
-                        "internalType": "address",
                         "name": "from",
                         "type": "address",
                     },
                     {
                         "indexed": True,
                         "internalType": "address",
                         "name": "to",
                         "type": "address",
                     },
                     {
-                        "indexed": True,
+                        "indexed": False,
                         "internalType": "uint256",
-                        "name": "tokenId",
+                        "name": "value",
                         "type": "uint256",
                     },
                 ],
                 "name": "Transfer",
                 "type": "event",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
-                ],
-                "name": "approve",
-                "outputs": [],
-                "stateMutability": "nonpayable",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"}
-                ],
-                "name": "balanceOf",
-                "outputs": [
-                    {"internalType": "uint256", "name": "balance", "type": "uint256"}
+                    {"internalType": "address", "name": "owner", "type": "address"},
+                    {"internalType": "address", "name": "spender", "type": "address"},
                 ],
+                "name": "allowance",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"}
-                ],
-                "name": "getApproved",
-                "outputs": [
-                    {"internalType": "address", "name": "operator", "type": "address"}
+                    {"internalType": "address", "name": "spender", "type": "address"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
-                "stateMutability": "view",
+                "name": "approve",
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"},
-                    {"internalType": "address", "name": "operator", "type": "address"},
+                    {"internalType": "address", "name": "account", "type": "address"}
                 ],
-                "name": "isApprovedForAll",
-                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
+                "name": "balanceOf",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"}
-                ],
-                "name": "ownerOf",
-                "outputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"}
-                ],
+                "inputs": [],
+                "name": "decimals",
+                "outputs": [{"internalType": "uint8", "name": "", "type": "uint8"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "from", "type": "address"},
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
-                ],
-                "name": "safeTransferFrom",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "inputs": [],
+                "name": "name",
+                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "from", "type": "address"},
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
-                    {"internalType": "bytes", "name": "data", "type": "bytes"},
-                ],
-                "name": "safeTransferFrom",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "inputs": [],
+                "name": "symbol",
+                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "operator", "type": "address"},
-                    {"internalType": "bool", "name": "_approved", "type": "bool"},
-                ],
-                "name": "setApprovalForAll",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "inputs": [],
+                "name": "totalSupply",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "bytes4", "name": "interfaceId", "type": "bytes4"}
+                    {"internalType": "address", "name": "to", "type": "address"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
-                "name": "supportsInterface",
+                "name": "transfer",
                 "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
-                "stateMutability": "view",
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
                     {"internalType": "address", "name": "from", "type": "address"},
                     {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
                 "name": "transferFrom",
-                "outputs": [],
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def approve(
-        self, to: str, token_id: int, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
+    def allowance(self, owner: str, spender: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.approve(to, token_id).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.allowance(owner, spender).call()
 
-    def balance_of(self, owner: str) -> int:
+    def approve(
+        self,
+        spender: str,
+        amount: int,
+        override_tx_parameters: Optional[TxParams] = None,
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.balanceOf(owner).call()
+        return c.functions.approve(spender, amount).build_transaction(
+            override_tx_parameters
+        )
 
-    def get_approved(self, token_id: int) -> str:
+    def balance_of(self, account: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.getApproved(token_id).call()
+        return c.functions.balanceOf(account).call()
 
-    def is_approved_for_all(self, owner: str, operator: str) -> bool:
+    def decimals(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.isApprovedForAll(owner, operator).call()
+        return c.functions.decimals().call()
 
-    def owner_of(self, token_id: int) -> str:
+    def name(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.ownerOf(token_id).call()
+        return c.functions.name().call()
 
-    def safe_transfer_from(
-        self,
-        _from: str,
-        to: str,
-        token_id: int,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def symbol(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.safeTransferFrom(_from, to, token_id).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.symbol().call()
 
-    def safe_transfer_from(
-        self,
-        _from: str,
-        to: str,
-        token_id: int,
-        data: bytes,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def total_supply(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.safeTransferFrom(
-            _from, to, token_id, data
-        ).build_transaction(override_tx_parameters)
+        return c.functions.totalSupply().call()
 
-    def set_approval_for_all(
-        self,
-        operator: str,
-        _approved: bool,
-        override_tx_parameters: Optional[TxParams] = None,
+    def transfer(
+        self, to: str, amount: int, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.setApprovalForAll(operator, _approved).build_transaction(
+        return c.functions.transfer(to, amount).build_transaction(
             override_tx_parameters
         )
 
-    def supports_interface(self, interface_id: None) -> bool:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.supportsInterface(interface_id).call()
-
     def transfer_from(
         self,
         _from: str,
         to: str,
-        token_id: int,
+        amount: int,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.transferFrom(_from, to, token_id).build_transaction(
+        return c.functions.transferFrom(_from, to, amount).build_transaction(
             override_tx_parameters
         )
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_e_r_c721_enumerable.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_principal_token.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,33 @@
-from typing import Optional, Union
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
+from .multi_approval import MultiApproval
+from .call3 import Call3
+
+
+def serialize_struct(d) -> tuple:
+    if isinstance(d, dict):
+        return tuple(serialize_struct(v) for v in d.values())
+    elif isinstance(d, (list, tuple)):
+        return tuple(serialize_struct(x) for x in d)
+    else:
+        return d
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class IERC721Enumerable:
+class IPPrincipalToken:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
@@ -24,364 +39,378 @@
                         "internalType": "address",
                         "name": "owner",
                         "type": "address",
                     },
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "approved",
+                        "name": "spender",
                         "type": "address",
                     },
                     {
-                        "indexed": True,
+                        "indexed": False,
                         "internalType": "uint256",
-                        "name": "tokenId",
+                        "name": "value",
                         "type": "uint256",
                     },
                 ],
                 "name": "Approval",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "owner",
-                        "type": "address",
-                    },
-                    {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "operator",
-                        "type": "address",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "bool",
-                        "name": "approved",
-                        "type": "bool",
-                    },
-                ],
-                "name": "ApprovalForAll",
-                "type": "event",
-            },
-            {
-                "anonymous": False,
-                "inputs": [
-                    {
-                        "indexed": True,
-                        "internalType": "address",
                         "name": "from",
                         "type": "address",
                     },
                     {
                         "indexed": True,
                         "internalType": "address",
                         "name": "to",
                         "type": "address",
                     },
                     {
-                        "indexed": True,
+                        "indexed": False,
                         "internalType": "uint256",
-                        "name": "tokenId",
+                        "name": "value",
                         "type": "uint256",
                     },
                 ],
                 "name": "Transfer",
                 "type": "event",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
-                ],
-                "name": "approve",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "inputs": [],
+                "name": "SY",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"}
-                ],
-                "name": "balanceOf",
-                "outputs": [
-                    {"internalType": "uint256", "name": "balance", "type": "uint256"}
-                ],
+                "inputs": [],
+                "name": "YT",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"}
-                ],
-                "name": "getApproved",
-                "outputs": [
-                    {"internalType": "address", "name": "operator", "type": "address"}
+                    {"internalType": "address", "name": "owner", "type": "address"},
+                    {"internalType": "address", "name": "spender", "type": "address"},
                 ],
+                "name": "allowance",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"},
-                    {"internalType": "address", "name": "operator", "type": "address"},
+                    {"internalType": "address", "name": "spender", "type": "address"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
-                "name": "isApprovedForAll",
+                "name": "approve",
                 "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
-                "stateMutability": "view",
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"}
-                ],
-                "name": "ownerOf",
-                "outputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"}
+                    {"internalType": "address", "name": "account", "type": "address"}
                 ],
+                "name": "balanceOf",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "from", "type": "address"},
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
+                    {"internalType": "address", "name": "user", "type": "address"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
-                "name": "safeTransferFrom",
+                "name": "burnByYT",
                 "outputs": [],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "from", "type": "address"},
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
-                    {"internalType": "bytes", "name": "data", "type": "bytes"},
-                ],
-                "name": "safeTransferFrom",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "inputs": [],
+                "name": "decimals",
+                "outputs": [{"internalType": "uint8", "name": "", "type": "uint8"}],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "expiry",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "factory",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "operator", "type": "address"},
-                    {"internalType": "bool", "name": "_approved", "type": "bool"},
+                    {"internalType": "address", "name": "_YT", "type": "address"}
                 ],
-                "name": "setApprovalForAll",
+                "name": "initialize",
                 "outputs": [],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "bytes4", "name": "interfaceId", "type": "bytes4"}
-                ],
-                "name": "supportsInterface",
+                "inputs": [],
+                "name": "isExpired",
                 "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "uint256", "name": "index", "type": "uint256"}
+                    {"internalType": "address", "name": "user", "type": "address"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
-                "name": "tokenByIndex",
-                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "name": "mintByYT",
+                "outputs": [],
+                "stateMutability": "nonpayable",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "name",
+                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"},
-                    {"internalType": "uint256", "name": "index", "type": "uint256"},
-                ],
-                "name": "tokenOfOwnerByIndex",
-                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "inputs": [],
+                "name": "symbol",
+                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [],
                 "name": "totalSupply",
                 "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
+                    {"internalType": "address", "name": "to", "type": "address"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
+                ],
+                "name": "transfer",
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
+                "stateMutability": "nonpayable",
+                "type": "function",
+            },
+            {
+                "inputs": [
                     {"internalType": "address", "name": "from", "type": "address"},
                     {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
                 "name": "transferFrom",
-                "outputs": [],
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
+    def s_y(self) -> str:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.SY().call()
+
+    def y_t(self) -> str:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.YT().call()
+
+    def allowance(self, owner: str, spender: str) -> int:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.allowance(owner, spender).call()
+
     def approve(
-        self, to: str, token_id: int, override_tx_parameters: Optional[TxParams] = None
+        self,
+        spender: str,
+        amount: int,
+        override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.approve(to, token_id).build_transaction(
+        return c.functions.approve(spender, amount).build_transaction(
             override_tx_parameters
         )
 
-    def balance_of(self, owner: str) -> int:
+    def balance_of(self, account: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.balanceOf(owner).call()
+        return c.functions.balanceOf(account).call()
 
-    def get_approved(self, token_id: int) -> str:
+    def burn_by_y_t(
+        self, user: str, amount: int, override_tx_parameters: Optional[TxParams] = None
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.getApproved(token_id).call()
+        return c.functions.burnByYT(user, amount).build_transaction(
+            override_tx_parameters
+        )
 
-    def is_approved_for_all(self, owner: str, operator: str) -> bool:
+    def decimals(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.isApprovedForAll(owner, operator).call()
+        return c.functions.decimals().call()
 
-    def owner_of(self, token_id: int) -> str:
+    def expiry(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.ownerOf(token_id).call()
+        return c.functions.expiry().call()
 
-    def safe_transfer_from(
-        self,
-        _from: str,
-        to: str,
-        token_id: int,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def factory(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.safeTransferFrom(_from, to, token_id).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.factory().call()
 
-    def safe_transfer_from(
-        self,
-        _from: str,
-        to: str,
-        token_id: int,
-        data: bytes,
-        override_tx_parameters: Optional[TxParams] = None,
+    def initialize(
+        self, __y_t: str, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.safeTransferFrom(
-            _from, to, token_id, data
-        ).build_transaction(override_tx_parameters)
+        return c.functions.initialize(__y_t).build_transaction(override_tx_parameters)
 
-    def set_approval_for_all(
-        self,
-        operator: str,
-        _approved: bool,
-        override_tx_parameters: Optional[TxParams] = None,
+    def is_expired(self) -> bool:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.isExpired().call()
+
+    def mint_by_y_t(
+        self, user: str, amount: int, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.setApprovalForAll(operator, _approved).build_transaction(
+        return c.functions.mintByYT(user, amount).build_transaction(
             override_tx_parameters
         )
 
-    def supports_interface(self, interface_id: None) -> bool:
+    def name(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.supportsInterface(interface_id).call()
+        return c.functions.name().call()
 
-    def token_by_index(self, index: int) -> int:
+    def symbol(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.tokenByIndex(index).call()
+        return c.functions.symbol().call()
 
-    def token_of_owner_by_index(self, owner: str, index: int) -> int:
+    def total_supply(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.tokenOfOwnerByIndex(owner, index).call()
+        return c.functions.totalSupply().call()
 
-    def total_supply(self) -> int:
+    def transfer(
+        self, to: str, amount: int, override_tx_parameters: Optional[TxParams] = None
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.totalSupply().call()
+        return c.functions.transfer(to, amount).build_transaction(
+            override_tx_parameters
+        )
 
     def transfer_from(
         self,
         _from: str,
         to: str,
-        token_id: int,
+        amount: int,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.transferFrom(_from, to, token_id).build_transaction(
+        return c.functions.transferFrom(_from, to, amount).build_transaction(
             override_tx_parameters
         )
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_e_r_c721_metadata.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_bulk_seller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,384 +1,382 @@
-from typing import Optional, Union
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
+from .multi_approval import MultiApproval
+from .call3 import Call3
+
+
+def serialize_struct(d) -> tuple:
+    if isinstance(d, dict):
+        return tuple(serialize_struct(v) for v in d.values())
+    elif isinstance(d, (list, tuple)):
+        return tuple(serialize_struct(x) for x in d)
+    else:
+        return d
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class IERC721Metadata:
+class IPBulkSeller:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
             {
                 "anonymous": False,
                 "inputs": [
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "owner",
-                        "type": "address",
-                    },
-                    {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "approved",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "newFeeRate",
+                        "type": "uint256",
                     },
                     {
-                        "indexed": True,
+                        "indexed": False,
                         "internalType": "uint256",
-                        "name": "tokenId",
+                        "name": "oldFeeRate",
                         "type": "uint256",
                     },
                 ],
-                "name": "Approval",
+                "name": "FeeRateUpdated",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "owner",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "newRateTokenToSy",
+                        "type": "uint256",
                     },
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "operator",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "newRateSyToToken",
+                        "type": "uint256",
                     },
                     {
                         "indexed": False,
-                        "internalType": "bool",
-                        "name": "approved",
-                        "type": "bool",
+                        "internalType": "uint256",
+                        "name": "oldRateTokenToSy",
+                        "type": "uint256",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "oldRateSyToToken",
+                        "type": "uint256",
                     },
                 ],
-                "name": "ApprovalForAll",
+                "name": "RateUpdated",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "from",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "netSyRedeem",
+                        "type": "uint256",
                     },
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "to",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "netTokenFromSy",
+                        "type": "uint256",
                     },
                     {
-                        "indexed": True,
+                        "indexed": False,
                         "internalType": "uint256",
-                        "name": "tokenId",
+                        "name": "newTokenProp",
+                        "type": "uint256",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "oldTokenProp",
                         "type": "uint256",
                     },
                 ],
-                "name": "Transfer",
+                "name": "ReBalanceSyToToken",
                 "type": "event",
             },
             {
+                "anonymous": False,
                 "inputs": [
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "netTokenDeposit",
+                        "type": "uint256",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "netSyFromToken",
+                        "type": "uint256",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "newTokenProp",
+                        "type": "uint256",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "oldTokenProp",
+                        "type": "uint256",
+                    },
                 ],
-                "name": "approve",
-                "outputs": [],
-                "stateMutability": "nonpayable",
-                "type": "function",
+                "name": "ReBalanceTokenToSy",
+                "type": "event",
             },
             {
+                "anonymous": False,
                 "inputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"}
-                ],
-                "name": "balanceOf",
-                "outputs": [
-                    {"internalType": "uint256", "name": "balance", "type": "uint256"}
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "totalToken",
+                        "type": "uint256",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "totalSy",
+                        "type": "uint256",
+                    },
                 ],
-                "stateMutability": "view",
-                "type": "function",
+                "name": "ReserveUpdated",
+                "type": "event",
             },
             {
+                "anonymous": False,
                 "inputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"}
-                ],
-                "name": "getApproved",
-                "outputs": [
-                    {"internalType": "address", "name": "operator", "type": "address"}
+                    {
+                        "indexed": False,
+                        "internalType": "address",
+                        "name": "receiver",
+                        "type": "address",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "netSyIn",
+                        "type": "uint256",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "netTokenOut",
+                        "type": "uint256",
+                    },
                 ],
-                "stateMutability": "view",
-                "type": "function",
+                "name": "SwapExactSyForToken",
+                "type": "event",
             },
             {
+                "anonymous": False,
                 "inputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"},
-                    {"internalType": "address", "name": "operator", "type": "address"},
+                    {
+                        "indexed": False,
+                        "internalType": "address",
+                        "name": "receiver",
+                        "type": "address",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "netTokenIn",
+                        "type": "uint256",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "netSyOut",
+                        "type": "uint256",
+                    },
                 ],
-                "name": "isApprovedForAll",
-                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
-                "stateMutability": "view",
-                "type": "function",
+                "name": "SwapExactTokenForSy",
+                "type": "event",
             },
             {
                 "inputs": [],
-                "name": "name",
-                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
+                "name": "SY",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"}
-                ],
-                "name": "ownerOf",
+                "inputs": [],
+                "name": "readState",
                 "outputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"}
+                    {
+                        "components": [
+                            {
+                                "internalType": "uint256",
+                                "name": "rateTokenToSy",
+                                "type": "uint256",
+                            },
+                            {
+                                "internalType": "uint256",
+                                "name": "rateSyToToken",
+                                "type": "uint256",
+                            },
+                            {
+                                "internalType": "uint256",
+                                "name": "totalToken",
+                                "type": "uint256",
+                            },
+                            {
+                                "internalType": "uint256",
+                                "name": "totalSy",
+                                "type": "uint256",
+                            },
+                            {
+                                "internalType": "uint256",
+                                "name": "feeRate",
+                                "type": "uint256",
+                            },
+                        ],
+                        "internalType": "struct BulkSellerState",
+                        "name": "",
+                        "type": "tuple",
+                    }
                 ],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "from", "type": "address"},
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
+                    {"internalType": "address", "name": "receiver", "type": "address"},
+                    {"internalType": "uint256", "name": "exactSyIn", "type": "uint256"},
+                    {
+                        "internalType": "uint256",
+                        "name": "minTokenOut",
+                        "type": "uint256",
+                    },
+                    {
+                        "internalType": "bool",
+                        "name": "swapFromInternalBalance",
+                        "type": "bool",
+                    },
                 ],
-                "name": "safeTransferFrom",
-                "outputs": [],
-                "stateMutability": "nonpayable",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "address", "name": "from", "type": "address"},
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
-                    {"internalType": "bytes", "name": "data", "type": "bytes"},
+                "name": "swapExactSyForToken",
+                "outputs": [
+                    {
+                        "internalType": "uint256",
+                        "name": "netTokenOut",
+                        "type": "uint256",
+                    }
                 ],
-                "name": "safeTransferFrom",
-                "outputs": [],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "operator", "type": "address"},
-                    {"internalType": "bool", "name": "_approved", "type": "bool"},
+                    {"internalType": "address", "name": "receiver", "type": "address"},
+                    {
+                        "internalType": "uint256",
+                        "name": "netTokenIn",
+                        "type": "uint256",
+                    },
+                    {"internalType": "uint256", "name": "minSyOut", "type": "uint256"},
                 ],
-                "name": "setApprovalForAll",
-                "outputs": [],
-                "stateMutability": "nonpayable",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "bytes4", "name": "interfaceId", "type": "bytes4"}
+                "name": "swapExactTokenForSy",
+                "outputs": [
+                    {"internalType": "uint256", "name": "netSyOut", "type": "uint256"}
                 ],
-                "name": "supportsInterface",
-                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
-                "stateMutability": "view",
+                "stateMutability": "payable",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "symbol",
-                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
+                "name": "token",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
                 "stateMutability": "view",
                 "type": "function",
             },
-            {
-                "inputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"}
-                ],
-                "name": "tokenURI",
-                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "address", "name": "from", "type": "address"},
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
-                ],
-                "name": "transferFrom",
-                "outputs": [],
-                "stateMutability": "nonpayable",
-                "type": "function",
-            },
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def approve(
-        self, to: str, token_id: int, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
+    def s_y(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.approve(to, token_id).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.SY().call()
 
-    def balance_of(self, owner: str) -> int:
+    def read_state(self) -> tuple:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.balanceOf(owner).call()
+        return c.functions.readState().call()
 
-    def get_approved(self, token_id: int) -> str:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.getApproved(token_id).call()
-
-    def is_approved_for_all(self, owner: str, operator: str) -> bool:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.isApprovedForAll(owner, operator).call()
-
-    def name(self) -> TxParams:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.name().build_transaction()
-
-    def owner_of(self, token_id: int) -> str:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.ownerOf(token_id).call()
-
-    def safe_transfer_from(
-        self,
-        _from: str,
-        to: str,
-        token_id: int,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.safeTransferFrom(_from, to, token_id).build_transaction(
-            override_tx_parameters
-        )
-
-    def safe_transfer_from(
+    def swap_exact_sy_for_token(
         self,
-        _from: str,
-        to: str,
-        token_id: int,
-        data: bytes,
+        receiver: str,
+        exact_sy_in: int,
+        min_token_out: int,
+        swap_from_internal_balance: bool,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.safeTransferFrom(
-            _from, to, token_id, data
+        return c.functions.swapExactSyForToken(
+            receiver, exact_sy_in, min_token_out, swap_from_internal_balance
         ).build_transaction(override_tx_parameters)
 
-    def set_approval_for_all(
+    def swap_exact_token_for_sy(
         self,
-        operator: str,
-        _approved: bool,
+        receiver: str,
+        net_token_in: int,
+        min_sy_out: int,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.setApprovalForAll(operator, _approved).build_transaction(
-            override_tx_parameters
-        )
-
-    def supports_interface(self, interface_id: None) -> bool:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.supportsInterface(interface_id).call()
-
-    def symbol(self) -> TxParams:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.symbol().build_transaction()
-
-    def token_u_r_i(self, token_id: int) -> TxParams:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.tokenURI(token_id).build_transaction()
+        return c.functions.swapExactTokenForSy(
+            receiver, net_token_in, min_sy_out
+        ).build_transaction(override_tx_parameters)
 
-    def transfer_from(
-        self,
-        _from: str,
-        to: str,
-        token_id: int,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def token(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.transferFrom(_from, to, token_id).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.token().call()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_e_r_c_detailed.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/w_e_t_h_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Optional, Union
 from eth_typing import Address, ChecksumAddress
-from web3.types import TxParams
 from web3 import Web3
+from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class IERCDetailed:
+class WETHInterface:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
@@ -93,31 +93,17 @@
                 "name": "balanceOf",
                 "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "decimals",
-                "outputs": [{"internalType": "uint8", "name": "", "type": "uint8"}],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
-                "inputs": [],
-                "name": "name",
-                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
-                "inputs": [],
-                "name": "symbol",
-                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
-                "stateMutability": "view",
+                "name": "deposit",
+                "outputs": [],
+                "stateMutability": "payable",
                 "type": "function",
             },
             {
                 "inputs": [],
                 "name": "totalSupply",
                 "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
@@ -140,14 +126,23 @@
                     {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
                 "name": "transferFrom",
                 "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
+            {
+                "inputs": [
+                    {"internalType": "uint256", "name": "wad", "type": "uint256"}
+                ],
+                "name": "withdraw",
+                "outputs": [],
+                "stateMutability": "nonpayable",
+                "type": "function",
+            },
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
@@ -184,40 +179,22 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.balanceOf(account).call()
 
-    def decimals(self) -> int:
+    def deposit(self, override_tx_parameters: Optional[TxParams] = None) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.decimals().call()
-
-    def name(self) -> str:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.name().call()
-
-    def symbol(self) -> str:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.symbol().call()
+        return c.functions.deposit().build_transaction(override_tx_parameters)
 
     def total_supply(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
@@ -249,7 +226,18 @@
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.transferFrom(_from, to, amount).build_transaction(
             override_tx_parameters
         )
+
+    def withdraw(
+        self, wad: int, override_tx_parameters: Optional[TxParams] = None
+    ) -> TxParams:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.withdraw(wad).build_transaction(override_tx_parameters)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_lending_pool.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/i_uniswap_v3_pool.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1175 +1,1074 @@
-from typing import Optional, Union
+from typing import Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class ILendingPool:
+class IUniswapV3Pool:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "reserve",
+                        "name": "owner",
                         "type": "address",
                     },
                     {
-                        "indexed": False,
-                        "internalType": "address",
-                        "name": "user",
-                        "type": "address",
+                        "indexed": True,
+                        "internalType": "int24",
+                        "name": "tickLower",
+                        "type": "int24",
                     },
                     {
                         "indexed": True,
-                        "internalType": "address",
-                        "name": "onBehalfOf",
-                        "type": "address",
+                        "internalType": "int24",
+                        "name": "tickUpper",
+                        "type": "int24",
                     },
                     {
                         "indexed": False,
-                        "internalType": "uint256",
+                        "internalType": "uint128",
                         "name": "amount",
-                        "type": "uint256",
+                        "type": "uint128",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "borrowRateMode",
+                        "name": "amount0",
                         "type": "uint256",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "borrowRate",
+                        "name": "amount1",
                         "type": "uint256",
                     },
-                    {
-                        "indexed": True,
-                        "internalType": "uint16",
-                        "name": "referral",
-                        "type": "uint16",
-                    },
                 ],
-                "name": "Borrow",
+                "name": "Burn",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "reserve",
+                        "name": "owner",
                         "type": "address",
                     },
                     {
                         "indexed": False,
                         "internalType": "address",
-                        "name": "user",
+                        "name": "recipient",
                         "type": "address",
                     },
                     {
                         "indexed": True,
-                        "internalType": "address",
-                        "name": "onBehalfOf",
-                        "type": "address",
+                        "internalType": "int24",
+                        "name": "tickLower",
+                        "type": "int24",
+                    },
+                    {
+                        "indexed": True,
+                        "internalType": "int24",
+                        "name": "tickUpper",
+                        "type": "int24",
                     },
                     {
                         "indexed": False,
-                        "internalType": "uint256",
-                        "name": "amount",
-                        "type": "uint256",
+                        "internalType": "uint128",
+                        "name": "amount0",
+                        "type": "uint128",
                     },
                     {
-                        "indexed": True,
-                        "internalType": "uint16",
-                        "name": "referral",
-                        "type": "uint16",
+                        "indexed": False,
+                        "internalType": "uint128",
+                        "name": "amount1",
+                        "type": "uint128",
                     },
                 ],
-                "name": "Deposit",
+                "name": "Collect",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "target",
-                        "type": "address",
-                    },
-                    {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "initiator",
+                        "name": "sender",
                         "type": "address",
                     },
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "asset",
+                        "name": "recipient",
                         "type": "address",
                     },
                     {
                         "indexed": False,
-                        "internalType": "uint256",
-                        "name": "amount",
-                        "type": "uint256",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "uint256",
-                        "name": "premium",
-                        "type": "uint256",
+                        "internalType": "uint128",
+                        "name": "amount0",
+                        "type": "uint128",
                     },
                     {
                         "indexed": False,
-                        "internalType": "uint16",
-                        "name": "referralCode",
-                        "type": "uint16",
+                        "internalType": "uint128",
+                        "name": "amount1",
+                        "type": "uint128",
                     },
                 ],
-                "name": "FlashLoan",
+                "name": "CollectProtocol",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "collateralAsset",
-                        "type": "address",
-                    },
-                    {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "debtAsset",
+                        "name": "sender",
                         "type": "address",
                     },
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "user",
+                        "name": "recipient",
                         "type": "address",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "debtToCover",
+                        "name": "amount0",
                         "type": "uint256",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "liquidatedCollateralAmount",
+                        "name": "amount1",
                         "type": "uint256",
                     },
                     {
                         "indexed": False,
-                        "internalType": "address",
-                        "name": "liquidator",
-                        "type": "address",
+                        "internalType": "uint256",
+                        "name": "paid0",
+                        "type": "uint256",
                     },
                     {
                         "indexed": False,
-                        "internalType": "bool",
-                        "name": "receiveAToken",
-                        "type": "bool",
+                        "internalType": "uint256",
+                        "name": "paid1",
+                        "type": "uint256",
                     },
                 ],
-                "name": "LiquidationCall",
+                "name": "Flash",
                 "type": "event",
             },
-            {"anonymous": False, "inputs": [], "name": "Paused", "type": "event"},
             {
                 "anonymous": False,
                 "inputs": [
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "reserve",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint16",
+                        "name": "observationCardinalityNextOld",
+                        "type": "uint16",
                     },
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "user",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint16",
+                        "name": "observationCardinalityNextNew",
+                        "type": "uint16",
                     },
                 ],
-                "name": "RebalanceStableBorrowRate",
+                "name": "IncreaseObservationCardinalityNext",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "reserve",
-                        "type": "address",
-                    },
-                    {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "user",
-                        "type": "address",
-                    },
-                    {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "repayer",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint160",
+                        "name": "sqrtPriceX96",
+                        "type": "uint160",
                     },
                     {
                         "indexed": False,
-                        "internalType": "uint256",
-                        "name": "amount",
-                        "type": "uint256",
+                        "internalType": "int24",
+                        "name": "tick",
+                        "type": "int24",
                     },
                 ],
-                "name": "Repay",
+                "name": "Initialize",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
+                        "indexed": False,
+                        "internalType": "address",
+                        "name": "sender",
+                        "type": "address",
+                    },
+                    {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "reserve",
+                        "name": "owner",
                         "type": "address",
                     },
                     {
-                        "indexed": False,
-                        "internalType": "uint256",
-                        "name": "liquidityRate",
-                        "type": "uint256",
+                        "indexed": True,
+                        "internalType": "int24",
+                        "name": "tickLower",
+                        "type": "int24",
                     },
                     {
-                        "indexed": False,
-                        "internalType": "uint256",
-                        "name": "stableBorrowRate",
-                        "type": "uint256",
+                        "indexed": True,
+                        "internalType": "int24",
+                        "name": "tickUpper",
+                        "type": "int24",
                     },
                     {
                         "indexed": False,
-                        "internalType": "uint256",
-                        "name": "variableBorrowRate",
-                        "type": "uint256",
+                        "internalType": "uint128",
+                        "name": "amount",
+                        "type": "uint128",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "liquidityIndex",
+                        "name": "amount0",
                         "type": "uint256",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "variableBorrowIndex",
+                        "name": "amount1",
                         "type": "uint256",
                     },
                 ],
-                "name": "ReserveDataUpdated",
+                "name": "Mint",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "reserve",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint8",
+                        "name": "feeProtocol0Old",
+                        "type": "uint8",
                     },
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "user",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint8",
+                        "name": "feeProtocol1Old",
+                        "type": "uint8",
                     },
-                ],
-                "name": "ReserveUsedAsCollateralDisabled",
-                "type": "event",
-            },
-            {
-                "anonymous": False,
-                "inputs": [
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "reserve",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint8",
+                        "name": "feeProtocol0New",
+                        "type": "uint8",
                     },
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "user",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint8",
+                        "name": "feeProtocol1New",
+                        "type": "uint8",
                     },
                 ],
-                "name": "ReserveUsedAsCollateralEnabled",
+                "name": "SetFeeProtocol",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "reserve",
+                        "name": "sender",
                         "type": "address",
                     },
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "user",
+                        "name": "recipient",
                         "type": "address",
                     },
                     {
                         "indexed": False,
-                        "internalType": "uint256",
-                        "name": "rateMode",
-                        "type": "uint256",
+                        "internalType": "int256",
+                        "name": "amount0",
+                        "type": "int256",
                     },
-                ],
-                "name": "Swap",
-                "type": "event",
-            },
-            {"anonymous": False, "inputs": [], "name": "Unpaused", "type": "event"},
-            {
-                "anonymous": False,
-                "inputs": [
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "reserve",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "int256",
+                        "name": "amount1",
+                        "type": "int256",
                     },
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "user",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint160",
+                        "name": "sqrtPriceX96",
+                        "type": "uint160",
                     },
                     {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "to",
-                        "type": "address",
+                        "indexed": False,
+                        "internalType": "uint128",
+                        "name": "liquidity",
+                        "type": "uint128",
                     },
                     {
                         "indexed": False,
-                        "internalType": "uint256",
-                        "name": "amount",
-                        "type": "uint256",
+                        "internalType": "int24",
+                        "name": "tick",
+                        "type": "int24",
                     },
                 ],
-                "name": "Withdraw",
+                "name": "Swap",
                 "type": "event",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "asset", "type": "address"},
-                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
-                    {
-                        "internalType": "uint256",
-                        "name": "interestRateMode",
-                        "type": "uint256",
-                    },
-                    {
-                        "internalType": "uint16",
-                        "name": "referralCode",
-                        "type": "uint16",
-                    },
-                    {
-                        "internalType": "address",
-                        "name": "onBehalfOf",
-                        "type": "address",
-                    },
+                    {"internalType": "int24", "name": "tickLower", "type": "int24"},
+                    {"internalType": "int24", "name": "tickUpper", "type": "int24"},
+                    {"internalType": "uint128", "name": "amount", "type": "uint128"},
+                ],
+                "name": "burn",
+                "outputs": [
+                    {"internalType": "uint256", "name": "amount0", "type": "uint256"},
+                    {"internalType": "uint256", "name": "amount1", "type": "uint256"},
                 ],
-                "name": "borrow",
-                "outputs": [],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "asset", "type": "address"},
-                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
+                    {"internalType": "address", "name": "recipient", "type": "address"},
+                    {"internalType": "int24", "name": "tickLower", "type": "int24"},
+                    {"internalType": "int24", "name": "tickUpper", "type": "int24"},
                     {
-                        "internalType": "address",
-                        "name": "onBehalfOf",
-                        "type": "address",
+                        "internalType": "uint128",
+                        "name": "amount0Requested",
+                        "type": "uint128",
                     },
                     {
-                        "internalType": "uint16",
-                        "name": "referralCode",
-                        "type": "uint16",
+                        "internalType": "uint128",
+                        "name": "amount1Requested",
+                        "type": "uint128",
                     },
                 ],
-                "name": "deposit",
-                "outputs": [],
+                "name": "collect",
+                "outputs": [
+                    {"internalType": "uint128", "name": "amount0", "type": "uint128"},
+                    {"internalType": "uint128", "name": "amount1", "type": "uint128"},
+                ],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "asset", "type": "address"},
-                    {"internalType": "address", "name": "from", "type": "address"},
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
+                    {"internalType": "address", "name": "recipient", "type": "address"},
                     {
-                        "internalType": "uint256",
-                        "name": "balanceFromAfter",
-                        "type": "uint256",
+                        "internalType": "uint128",
+                        "name": "amount0Requested",
+                        "type": "uint128",
                     },
                     {
-                        "internalType": "uint256",
-                        "name": "balanceToBefore",
-                        "type": "uint256",
+                        "internalType": "uint128",
+                        "name": "amount1Requested",
+                        "type": "uint128",
                     },
                 ],
-                "name": "finalizeTransfer",
+                "name": "collectProtocol",
+                "outputs": [
+                    {"internalType": "uint128", "name": "amount0", "type": "uint128"},
+                    {"internalType": "uint128", "name": "amount1", "type": "uint128"},
+                ],
+                "stateMutability": "nonpayable",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "factory",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "fee",
+                "outputs": [{"internalType": "uint24", "name": "", "type": "uint24"}],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "feeGrowthGlobal0X128",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "feeGrowthGlobal1X128",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [
+                    {"internalType": "address", "name": "recipient", "type": "address"},
+                    {"internalType": "uint256", "name": "amount0", "type": "uint256"},
+                    {"internalType": "uint256", "name": "amount1", "type": "uint256"},
+                    {"internalType": "bytes", "name": "data", "type": "bytes"},
+                ],
+                "name": "flash",
                 "outputs": [],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
                     {
-                        "internalType": "address",
-                        "name": "receiverAddress",
-                        "type": "address",
-                    },
-                    {
-                        "internalType": "address[]",
-                        "name": "assets",
-                        "type": "address[]",
-                    },
-                    {
-                        "internalType": "uint256[]",
-                        "name": "amounts",
-                        "type": "uint256[]",
-                    },
-                    {"internalType": "uint256[]", "name": "modes", "type": "uint256[]"},
-                    {
-                        "internalType": "address",
-                        "name": "onBehalfOf",
-                        "type": "address",
-                    },
-                    {"internalType": "bytes", "name": "params", "type": "bytes"},
-                    {
                         "internalType": "uint16",
-                        "name": "referralCode",
+                        "name": "observationCardinalityNext",
                         "type": "uint16",
-                    },
+                    }
                 ],
-                "name": "flashLoan",
+                "name": "increaseObservationCardinalityNext",
                 "outputs": [],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
-                "inputs": [],
-                "name": "getAddressesProvider",
-                "outputs": [
+                "inputs": [
                     {
-                        "internalType": "contract ILendingPoolAddressesProvider",
-                        "name": "",
-                        "type": "address",
+                        "internalType": "uint160",
+                        "name": "sqrtPriceX96",
+                        "type": "uint160",
                     }
                 ],
+                "name": "initialize",
+                "outputs": [],
+                "stateMutability": "nonpayable",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "liquidity",
+                "outputs": [{"internalType": "uint128", "name": "", "type": "uint128"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "asset", "type": "address"}
-                ],
-                "name": "getConfiguration",
-                "outputs": [
-                    {
-                        "components": [
-                            {
-                                "internalType": "uint256",
-                                "name": "data",
-                                "type": "uint256",
-                            }
-                        ],
-                        "internalType": "struct DataTypes.ReserveConfigurationMap",
-                        "name": "",
-                        "type": "tuple",
-                    }
-                ],
+                "inputs": [],
+                "name": "maxLiquidityPerTick",
+                "outputs": [{"internalType": "uint128", "name": "", "type": "uint128"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "asset", "type": "address"}
+                    {"internalType": "address", "name": "recipient", "type": "address"},
+                    {"internalType": "int24", "name": "tickLower", "type": "int24"},
+                    {"internalType": "int24", "name": "tickUpper", "type": "int24"},
+                    {"internalType": "uint128", "name": "amount", "type": "uint128"},
+                    {"internalType": "bytes", "name": "data", "type": "bytes"},
                 ],
-                "name": "getReserveData",
+                "name": "mint",
                 "outputs": [
-                    {
-                        "components": [
-                            {
-                                "components": [
-                                    {
-                                        "internalType": "uint256",
-                                        "name": "data",
-                                        "type": "uint256",
-                                    }
-                                ],
-                                "internalType": "struct DataTypes.ReserveConfigurationMap",
-                                "name": "configuration",
-                                "type": "tuple",
-                            },
-                            {
-                                "internalType": "uint128",
-                                "name": "liquidityIndex",
-                                "type": "uint128",
-                            },
-                            {
-                                "internalType": "uint128",
-                                "name": "variableBorrowIndex",
-                                "type": "uint128",
-                            },
-                            {
-                                "internalType": "uint128",
-                                "name": "currentLiquidityRate",
-                                "type": "uint128",
-                            },
-                            {
-                                "internalType": "uint128",
-                                "name": "currentVariableBorrowRate",
-                                "type": "uint128",
-                            },
-                            {
-                                "internalType": "uint128",
-                                "name": "currentStableBorrowRate",
-                                "type": "uint128",
-                            },
-                            {
-                                "internalType": "uint40",
-                                "name": "lastUpdateTimestamp",
-                                "type": "uint40",
-                            },
-                            {
-                                "internalType": "address",
-                                "name": "aTokenAddress",
-                                "type": "address",
-                            },
-                            {
-                                "internalType": "address",
-                                "name": "stableDebtTokenAddress",
-                                "type": "address",
-                            },
-                            {
-                                "internalType": "address",
-                                "name": "variableDebtTokenAddress",
-                                "type": "address",
-                            },
-                            {
-                                "internalType": "address",
-                                "name": "interestRateStrategyAddress",
-                                "type": "address",
-                            },
-                            {"internalType": "uint8", "name": "id", "type": "uint8"},
-                        ],
-                        "internalType": "struct DataTypes.ReserveData",
-                        "name": "",
-                        "type": "tuple",
-                    }
+                    {"internalType": "uint256", "name": "amount0", "type": "uint256"},
+                    {"internalType": "uint256", "name": "amount1", "type": "uint256"},
                 ],
-                "stateMutability": "view",
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "asset", "type": "address"}
+                    {"internalType": "uint256", "name": "index", "type": "uint256"}
+                ],
+                "name": "observations",
+                "outputs": [
+                    {
+                        "internalType": "uint32",
+                        "name": "blockTimestamp",
+                        "type": "uint32",
+                    },
+                    {
+                        "internalType": "int56",
+                        "name": "tickCumulative",
+                        "type": "int56",
+                    },
+                    {
+                        "internalType": "uint160",
+                        "name": "secondsPerLiquidityCumulativeX128",
+                        "type": "uint160",
+                    },
+                    {"internalType": "bool", "name": "initialized", "type": "bool"},
                 ],
-                "name": "getReserveNormalizedIncome",
-                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "asset", "type": "address"}
+                    {
+                        "internalType": "uint32[]",
+                        "name": "secondsAgos",
+                        "type": "uint32[]",
+                    }
                 ],
-                "name": "getReserveNormalizedVariableDebt",
-                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
-                "inputs": [],
-                "name": "getReservesList",
+                "name": "observe",
                 "outputs": [
-                    {"internalType": "address[]", "name": "", "type": "address[]"}
+                    {
+                        "internalType": "int56[]",
+                        "name": "tickCumulatives",
+                        "type": "int56[]",
+                    },
+                    {
+                        "internalType": "uint160[]",
+                        "name": "secondsPerLiquidityCumulativeX128s",
+                        "type": "uint160[]",
+                    },
                 ],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "user", "type": "address"}
+                    {"internalType": "bytes32", "name": "key", "type": "bytes32"}
                 ],
-                "name": "getUserAccountData",
+                "name": "positions",
                 "outputs": [
+                    {"internalType": "uint128", "name": "liquidity", "type": "uint128"},
                     {
                         "internalType": "uint256",
-                        "name": "totalCollateralETH",
-                        "type": "uint256",
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "totalDebtETH",
+                        "name": "feeGrowthInside0LastX128",
                         "type": "uint256",
                     },
                     {
                         "internalType": "uint256",
-                        "name": "availableBorrowsETH",
+                        "name": "feeGrowthInside1LastX128",
                         "type": "uint256",
                     },
                     {
-                        "internalType": "uint256",
-                        "name": "currentLiquidationThreshold",
-                        "type": "uint256",
+                        "internalType": "uint128",
+                        "name": "tokensOwed0",
+                        "type": "uint128",
                     },
-                    {"internalType": "uint256", "name": "ltv", "type": "uint256"},
                     {
-                        "internalType": "uint256",
-                        "name": "healthFactor",
-                        "type": "uint256",
+                        "internalType": "uint128",
+                        "name": "tokensOwed1",
+                        "type": "uint128",
                     },
                 ],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "user", "type": "address"}
-                ],
-                "name": "getUserConfiguration",
+                "inputs": [],
+                "name": "protocolFees",
                 "outputs": [
-                    {
-                        "components": [
-                            {
-                                "internalType": "uint256",
-                                "name": "data",
-                                "type": "uint256",
-                            }
-                        ],
-                        "internalType": "struct DataTypes.UserConfigurationMap",
-                        "name": "",
-                        "type": "tuple",
-                    }
+                    {"internalType": "uint128", "name": "token0", "type": "uint128"},
+                    {"internalType": "uint128", "name": "token1", "type": "uint128"},
                 ],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "reserve", "type": "address"},
+                    {"internalType": "uint8", "name": "feeProtocol0", "type": "uint8"},
+                    {"internalType": "uint8", "name": "feeProtocol1", "type": "uint8"},
+                ],
+                "name": "setFeeProtocol",
+                "outputs": [],
+                "stateMutability": "nonpayable",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "slot0",
+                "outputs": [
                     {
-                        "internalType": "address",
-                        "name": "aTokenAddress",
-                        "type": "address",
+                        "internalType": "uint160",
+                        "name": "sqrtPriceX96",
+                        "type": "uint160",
                     },
+                    {"internalType": "int24", "name": "tick", "type": "int24"},
                     {
-                        "internalType": "address",
-                        "name": "stableDebtAddress",
-                        "type": "address",
+                        "internalType": "uint16",
+                        "name": "observationIndex",
+                        "type": "uint16",
                     },
                     {
-                        "internalType": "address",
-                        "name": "variableDebtAddress",
-                        "type": "address",
+                        "internalType": "uint16",
+                        "name": "observationCardinality",
+                        "type": "uint16",
                     },
                     {
-                        "internalType": "address",
-                        "name": "interestRateStrategyAddress",
-                        "type": "address",
+                        "internalType": "uint16",
+                        "name": "observationCardinalityNext",
+                        "type": "uint16",
                     },
+                    {"internalType": "uint8", "name": "feeProtocol", "type": "uint8"},
+                    {"internalType": "bool", "name": "unlocked", "type": "bool"},
                 ],
-                "name": "initReserve",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
+                    {"internalType": "int24", "name": "tickLower", "type": "int24"},
+                    {"internalType": "int24", "name": "tickUpper", "type": "int24"},
+                ],
+                "name": "snapshotCumulativesInside",
+                "outputs": [
                     {
-                        "internalType": "address",
-                        "name": "collateralAsset",
-                        "type": "address",
+                        "internalType": "int56",
+                        "name": "tickCumulativeInside",
+                        "type": "int56",
                     },
-                    {"internalType": "address", "name": "debtAsset", "type": "address"},
-                    {"internalType": "address", "name": "user", "type": "address"},
                     {
-                        "internalType": "uint256",
-                        "name": "debtToCover",
-                        "type": "uint256",
+                        "internalType": "uint160",
+                        "name": "secondsPerLiquidityInsideX128",
+                        "type": "uint160",
+                    },
+                    {
+                        "internalType": "uint32",
+                        "name": "secondsInside",
+                        "type": "uint32",
                     },
-                    {"internalType": "bool", "name": "receiveAToken", "type": "bool"},
                 ],
-                "name": "liquidationCall",
-                "outputs": [],
-                "stateMutability": "nonpayable",
-                "type": "function",
-            },
-            {
-                "inputs": [],
-                "name": "paused",
-                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "asset", "type": "address"},
-                    {"internalType": "address", "name": "user", "type": "address"},
-                ],
-                "name": "rebalanceStableBorrowRate",
-                "outputs": [],
-                "stateMutability": "nonpayable",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "address", "name": "asset", "type": "address"},
-                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
-                    {"internalType": "uint256", "name": "rateMode", "type": "uint256"},
+                    {"internalType": "address", "name": "recipient", "type": "address"},
+                    {"internalType": "bool", "name": "zeroForOne", "type": "bool"},
                     {
-                        "internalType": "address",
-                        "name": "onBehalfOf",
-                        "type": "address",
+                        "internalType": "int256",
+                        "name": "amountSpecified",
+                        "type": "int256",
+                    },
+                    {
+                        "internalType": "uint160",
+                        "name": "sqrtPriceLimitX96",
+                        "type": "uint160",
                     },
+                    {"internalType": "bytes", "name": "data", "type": "bytes"},
+                ],
+                "name": "swap",
+                "outputs": [
+                    {"internalType": "int256", "name": "amount0", "type": "int256"},
+                    {"internalType": "int256", "name": "amount1", "type": "int256"},
                 ],
-                "name": "repay",
-                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "reserve", "type": "address"},
-                    {
-                        "internalType": "uint256",
-                        "name": "configuration",
-                        "type": "uint256",
-                    },
+                    {"internalType": "int16", "name": "wordPosition", "type": "int16"}
                 ],
-                "name": "setConfiguration",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "name": "tickBitmap",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [{"internalType": "bool", "name": "val", "type": "bool"}],
-                "name": "setPause",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "inputs": [],
+                "name": "tickSpacing",
+                "outputs": [{"internalType": "int24", "name": "", "type": "int24"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "reserve", "type": "address"},
+                "inputs": [{"internalType": "int24", "name": "tick", "type": "int24"}],
+                "name": "ticks",
+                "outputs": [
                     {
-                        "internalType": "address",
-                        "name": "rateStrategyAddress",
-                        "type": "address",
+                        "internalType": "uint128",
+                        "name": "liquidityGross",
+                        "type": "uint128",
                     },
+                    {
+                        "internalType": "int128",
+                        "name": "liquidityNet",
+                        "type": "int128",
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "feeGrowthOutside0X128",
+                        "type": "uint256",
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "feeGrowthOutside1X128",
+                        "type": "uint256",
+                    },
+                    {
+                        "internalType": "int56",
+                        "name": "tickCumulativeOutside",
+                        "type": "int56",
+                    },
+                    {
+                        "internalType": "uint160",
+                        "name": "secondsPerLiquidityOutsideX128",
+                        "type": "uint160",
+                    },
+                    {
+                        "internalType": "uint32",
+                        "name": "secondsOutside",
+                        "type": "uint32",
+                    },
+                    {"internalType": "bool", "name": "initialized", "type": "bool"},
                 ],
-                "name": "setReserveInterestRateStrategyAddress",
-                "outputs": [],
-                "stateMutability": "nonpayable",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "address", "name": "asset", "type": "address"},
-                    {"internalType": "bool", "name": "useAsCollateral", "type": "bool"},
-                ],
-                "name": "setUserUseReserveAsCollateral",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "asset", "type": "address"},
-                    {"internalType": "uint256", "name": "rateMode", "type": "uint256"},
-                ],
-                "name": "swapBorrowRateMode",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "inputs": [],
+                "name": "token0",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "asset", "type": "address"},
-                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
-                    {"internalType": "address", "name": "to", "type": "address"},
-                ],
-                "name": "withdraw",
-                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
-                "stateMutability": "nonpayable",
+                "inputs": [],
+                "name": "token1",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "stateMutability": "view",
                 "type": "function",
             },
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def borrow(
+    def burn(
         self,
-        asset: str,
+        tick_lower: int,
+        tick_upper: int,
         amount: int,
-        interest_rate_mode: int,
-        referral_code: None,
-        on_behalf_of: str,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.borrow(
-            asset, amount, interest_rate_mode, referral_code, on_behalf_of
-        ).build_transaction(override_tx_parameters)
+        return c.functions.burn(tick_lower, tick_upper, amount).build_transaction(
+            override_tx_parameters
+        )
 
-    def deposit(
+    def collect(
         self,
-        asset: str,
-        amount: int,
-        on_behalf_of: str,
-        referral_code: None,
+        recipient: str,
+        tick_lower: int,
+        tick_upper: int,
+        amount0_requested: int,
+        amount1_requested: int,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.deposit(
-            asset, amount, on_behalf_of, referral_code
+        return c.functions.collect(
+            recipient, tick_lower, tick_upper, amount0_requested, amount1_requested
         ).build_transaction(override_tx_parameters)
 
-    def finalize_transfer(
+    def collect_protocol(
         self,
-        asset: str,
-        _from: str,
-        to: str,
-        amount: int,
-        balance_from_after: int,
-        balance_to_before: int,
+        recipient: str,
+        amount0_requested: int,
+        amount1_requested: int,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.finalizeTransfer(
-            asset, _from, to, amount, balance_from_after, balance_to_before
+        return c.functions.collectProtocol(
+            recipient, amount0_requested, amount1_requested
         ).build_transaction(override_tx_parameters)
 
-    def flash_loan(
-        self,
-        receiver_address: str,
-        assets: None,
-        amounts: None,
-        modes: None,
-        on_behalf_of: str,
-        params: bytes,
-        referral_code: None,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def factory(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.flashLoan(
-            receiver_address,
-            assets,
-            amounts,
-            modes,
-            on_behalf_of,
-            params,
-            referral_code,
-        ).build_transaction(override_tx_parameters)
+        return c.functions.factory().call()
 
-    def get_addresses_provider(self) -> str:
+    def fee(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.getAddressesProvider().call()
+        return c.functions.fee().call()
 
-    def get_configuration(self, asset: str) -> tuple:
+    def fee_growth_global0_x128(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.getConfiguration(asset).call()
+        return c.functions.feeGrowthGlobal0X128().call()
 
-    def get_reserve_data(self, asset: str) -> tuple:
+    def fee_growth_global1_x128(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.getReserveData(asset).call()
+        return c.functions.feeGrowthGlobal1X128().call()
 
-    def get_reserve_normalized_income(self, asset: str) -> int:
+    def flash(
+        self,
+        recipient: str,
+        amount0: int,
+        amount1: int,
+        data: bytes,
+        override_tx_parameters: Optional[TxParams] = None,
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.getReserveNormalizedIncome(asset).call()
+        return c.functions.flash(recipient, amount0, amount1, data).build_transaction(
+            override_tx_parameters
+        )
 
-    def get_reserve_normalized_variable_debt(self, asset: str) -> int:
+    def increase_observation_cardinality_next(
+        self,
+        observation_cardinality_next: int,
+        override_tx_parameters: Optional[TxParams] = None,
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.getReserveNormalizedVariableDebt(asset).call()
+        return c.functions.increaseObservationCardinalityNext(
+            observation_cardinality_next
+        ).build_transaction(override_tx_parameters)
 
-    def get_reserves_list(self) -> TxParams:
+    def initialize(
+        self, sqrt_price_x96: int, override_tx_parameters: Optional[TxParams] = None
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.getReservesList().build_transaction()
+        return c.functions.initialize(sqrt_price_x96).build_transaction(
+            override_tx_parameters
+        )
 
-    def get_user_account_data(self, user: str) -> TxParams:
+    def liquidity(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.getUserAccountData(user).build_transaction()
+        return c.functions.liquidity().call()
 
-    def get_user_configuration(self, user: str) -> tuple:
+    def max_liquidity_per_tick(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.getUserConfiguration(user).call()
+        return c.functions.maxLiquidityPerTick().call()
 
-    def init_reserve(
+    def mint(
         self,
-        reserve: str,
-        a_token_address: str,
-        stable_debt_address: str,
-        variable_debt_address: str,
-        interest_rate_strategy_address: str,
+        recipient: str,
+        tick_lower: int,
+        tick_upper: int,
+        amount: int,
+        data: bytes,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.initReserve(
-            reserve,
-            a_token_address,
-            stable_debt_address,
-            variable_debt_address,
-            interest_rate_strategy_address,
+        return c.functions.mint(
+            recipient, tick_lower, tick_upper, amount, data
         ).build_transaction(override_tx_parameters)
 
-    def liquidation_call(
-        self,
-        collateral_asset: str,
-        debt_asset: str,
-        user: str,
-        debt_to_cover: int,
-        receive_a_token: bool,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def observations(self, index: int) -> Tuple[int, int, int, bool]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.liquidationCall(
-            collateral_asset, debt_asset, user, debt_to_cover, receive_a_token
-        ).build_transaction(override_tx_parameters)
+        return c.functions.observations(index).call()
 
-    def paused(self) -> bool:
+    def observe(self, seconds_agos: List[None]) -> Tuple[List[None], List[None]]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.paused().call()
+        return c.functions.observe(seconds_agos).call()
 
-    def rebalance_stable_borrow_rate(
-        self, asset: str, user: str, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
+    def positions(self, key: bytes) -> Tuple[int, int, int, int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.rebalanceStableBorrowRate(asset, user).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.positions(key).call()
+
+    def protocol_fees(self) -> Tuple[int, int]:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-    def repay(
+        return c.functions.protocolFees().call()
+
+    def set_fee_protocol(
         self,
-        asset: str,
-        amount: int,
-        rate_mode: int,
-        on_behalf_of: str,
+        fee_protocol0: int,
+        fee_protocol1: int,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.repay(
-            asset, amount, rate_mode, on_behalf_of
+        return c.functions.setFeeProtocol(
+            fee_protocol0, fee_protocol1
         ).build_transaction(override_tx_parameters)
 
-    def set_configuration(
-        self,
-        reserve: str,
-        configuration: int,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def slot0(self) -> Tuple[int, int, int, int, int, int, bool]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.setConfiguration(reserve, configuration).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.slot0().call()
 
-    def set_pause(
-        self, val: bool, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
+    def snapshot_cumulatives_inside(
+        self, tick_lower: int, tick_upper: int
+    ) -> Tuple[int, int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.setPause(val).build_transaction(override_tx_parameters)
+        return c.functions.snapshotCumulativesInside(tick_lower, tick_upper).call()
 
-    def set_reserve_interest_rate_strategy_address(
+    def swap(
         self,
-        reserve: str,
-        rate_strategy_address: str,
+        recipient: str,
+        zero_for_one: bool,
+        amount_specified: int,
+        sqrt_price_limit_x96: int,
+        data: bytes,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.setReserveInterestRateStrategyAddress(
-            reserve, rate_strategy_address
+        return c.functions.swap(
+            recipient, zero_for_one, amount_specified, sqrt_price_limit_x96, data
         ).build_transaction(override_tx_parameters)
 
-    def set_user_use_reserve_as_collateral(
-        self,
-        asset: str,
-        use_as_collateral: bool,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def tick_bitmap(self, word_position: int) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.setUserUseReserveAsCollateral(
-            asset, use_as_collateral
-        ).build_transaction(override_tx_parameters)
+        return c.functions.tickBitmap(word_position).call()
 
-    def swap_borrow_rate_mode(
-        self,
-        asset: str,
-        rate_mode: int,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def tick_spacing(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.swapBorrowRateMode(asset, rate_mode).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.tickSpacing().call()
 
-    def withdraw(
-        self,
-        asset: str,
-        amount: int,
-        to: str,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def ticks(self, tick: int) -> Tuple[int, int, int, int, int, int, int, bool]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.withdraw(asset, amount, to).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.ticks(tick).call()
+
+    def token0(self) -> str:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.token0().call()
+
+    def token1(self) -> str:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.token1().call()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_nonfungible_position_manager.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_market.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Optional, Union
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class INonfungiblePositionManager:
+class IPMarket:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
@@ -24,143 +24,155 @@
                         "internalType": "address",
                         "name": "owner",
                         "type": "address",
                     },
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "approved",
+                        "name": "spender",
                         "type": "address",
                     },
                     {
-                        "indexed": True,
+                        "indexed": False,
                         "internalType": "uint256",
-                        "name": "tokenId",
+                        "name": "value",
                         "type": "uint256",
                     },
                 ],
                 "name": "Approval",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "owner",
+                        "name": "receiverSy",
                         "type": "address",
                     },
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "operator",
+                        "name": "receiverPt",
                         "type": "address",
                     },
                     {
                         "indexed": False,
-                        "internalType": "bool",
-                        "name": "approved",
-                        "type": "bool",
-                    },
-                ],
-                "name": "ApprovalForAll",
-                "type": "event",
-            },
-            {
-                "anonymous": False,
-                "inputs": [
-                    {
-                        "indexed": True,
                         "internalType": "uint256",
-                        "name": "tokenId",
+                        "name": "netLpBurned",
                         "type": "uint256",
                     },
                     {
                         "indexed": False,
-                        "internalType": "address",
-                        "name": "recipient",
-                        "type": "address",
+                        "internalType": "uint256",
+                        "name": "netSyOut",
+                        "type": "uint256",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "amount0",
+                        "name": "netPtOut",
                         "type": "uint256",
                     },
+                ],
+                "name": "Burn",
+                "type": "event",
+            },
+            {
+                "anonymous": False,
+                "inputs": [
                     {
                         "indexed": False,
-                        "internalType": "uint256",
-                        "name": "amount1",
-                        "type": "uint256",
+                        "internalType": "uint16",
+                        "name": "observationCardinalityNextOld",
+                        "type": "uint16",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint16",
+                        "name": "observationCardinalityNextNew",
+                        "type": "uint16",
                     },
                 ],
-                "name": "Collect",
+                "name": "IncreaseObservationCardinalityNext",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
-                        "internalType": "uint256",
-                        "name": "tokenId",
-                        "type": "uint256",
+                        "internalType": "address",
+                        "name": "receiver",
+                        "type": "address",
                     },
                     {
                         "indexed": False,
-                        "internalType": "uint128",
-                        "name": "liquidity",
-                        "type": "uint128",
+                        "internalType": "uint256",
+                        "name": "netLpMinted",
+                        "type": "uint256",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "amount0",
+                        "name": "netSyUsed",
                         "type": "uint256",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "amount1",
+                        "name": "netPtUsed",
                         "type": "uint256",
                     },
                 ],
-                "name": "DecreaseLiquidity",
+                "name": "Mint",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
-                        "internalType": "uint256",
-                        "name": "tokenId",
-                        "type": "uint256",
+                        "internalType": "address",
+                        "name": "caller",
+                        "type": "address",
+                    },
+                    {
+                        "indexed": True,
+                        "internalType": "address",
+                        "name": "receiver",
+                        "type": "address",
                     },
                     {
                         "indexed": False,
-                        "internalType": "uint128",
-                        "name": "liquidity",
-                        "type": "uint128",
+                        "internalType": "int256",
+                        "name": "netPtOut",
+                        "type": "int256",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "int256",
+                        "name": "netSyOut",
+                        "type": "int256",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "amount0",
+                        "name": "netSyFee",
                         "type": "uint256",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "amount1",
+                        "name": "netSyToReserve",
                         "type": "uint256",
                     },
                 ],
-                "name": "IncreaseLiquidity",
+                "name": "Swap",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
@@ -171,892 +183,634 @@
                     {
                         "indexed": True,
                         "internalType": "address",
                         "name": "to",
                         "type": "address",
                     },
                     {
-                        "indexed": True,
+                        "indexed": False,
                         "internalType": "uint256",
-                        "name": "tokenId",
+                        "name": "value",
                         "type": "uint256",
                     },
                 ],
                 "name": "Transfer",
                 "type": "event",
             },
             {
-                "inputs": [],
-                "name": "DOMAIN_SEPARATOR",
-                "outputs": [{"internalType": "bytes32", "name": "", "type": "bytes32"}],
-                "stateMutability": "view",
-                "type": "function",
+                "anonymous": False,
+                "inputs": [
+                    {
+                        "indexed": True,
+                        "internalType": "uint256",
+                        "name": "timestamp",
+                        "type": "uint256",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "lnLastImpliedRate",
+                        "type": "uint256",
+                    },
+                ],
+                "name": "UpdateImpliedRate",
+                "type": "event",
             },
             {
-                "inputs": [],
-                "name": "PERMIT_TYPEHASH",
-                "outputs": [{"internalType": "bytes32", "name": "", "type": "bytes32"}],
-                "stateMutability": "pure",
+                "inputs": [
+                    {"internalType": "address", "name": "user", "type": "address"}
+                ],
+                "name": "activeBalance",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [],
-                "name": "WETH9",
-                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "inputs": [
+                    {"internalType": "address", "name": "owner", "type": "address"},
+                    {"internalType": "address", "name": "spender", "type": "address"},
+                ],
+                "name": "allowance",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
+                    {"internalType": "address", "name": "spender", "type": "address"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
                 "name": "approve",
-                "outputs": [],
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"}
+                    {"internalType": "address", "name": "account", "type": "address"}
                 ],
                 "name": "balanceOf",
-                "outputs": [
-                    {"internalType": "uint256", "name": "balance", "type": "uint256"}
-                ],
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"}
+                    {
+                        "internalType": "address",
+                        "name": "receiverSy",
+                        "type": "address",
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "receiverPt",
+                        "type": "address",
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "netLpToBurn",
+                        "type": "uint256",
+                    },
                 ],
                 "name": "burn",
-                "outputs": [],
-                "stateMutability": "payable",
+                "outputs": [
+                    {"internalType": "uint256", "name": "netSyOut", "type": "uint256"},
+                    {"internalType": "uint256", "name": "netPtOut", "type": "uint256"},
+                ],
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {
-                        "components": [
-                            {
-                                "internalType": "uint256",
-                                "name": "tokenId",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "address",
-                                "name": "recipient",
-                                "type": "address",
-                            },
-                            {
-                                "internalType": "uint128",
-                                "name": "amount0Max",
-                                "type": "uint128",
-                            },
-                            {
-                                "internalType": "uint128",
-                                "name": "amount1Max",
-                                "type": "uint128",
-                            },
-                        ],
-                        "internalType": "struct INonfungiblePositionManager.CollectParams",
-                        "name": "params",
-                        "type": "tuple",
-                    }
-                ],
-                "name": "collect",
-                "outputs": [
-                    {"internalType": "uint256", "name": "amount0", "type": "uint256"},
-                    {"internalType": "uint256", "name": "amount1", "type": "uint256"},
-                ],
-                "stateMutability": "payable",
+                "inputs": [],
+                "name": "decimals",
+                "outputs": [{"internalType": "uint8", "name": "", "type": "uint8"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "token0", "type": "address"},
-                    {"internalType": "address", "name": "token1", "type": "address"},
-                    {"internalType": "uint24", "name": "fee", "type": "uint24"},
-                    {
-                        "internalType": "uint160",
-                        "name": "sqrtPriceX96",
-                        "type": "uint160",
-                    },
-                ],
-                "name": "createAndInitializePoolIfNecessary",
+                "inputs": [],
+                "name": "expiry",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "getRewardTokens",
                 "outputs": [
-                    {"internalType": "address", "name": "pool", "type": "address"}
+                    {"internalType": "address[]", "name": "", "type": "address[]"}
                 ],
-                "stateMutability": "payable",
+                "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
                     {
-                        "components": [
-                            {
-                                "internalType": "uint256",
-                                "name": "tokenId",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "uint128",
-                                "name": "liquidity",
-                                "type": "uint128",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "amount0Min",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "amount1Min",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "deadline",
-                                "type": "uint256",
-                            },
-                        ],
-                        "internalType": "struct INonfungiblePositionManager.DecreaseLiquidityParams",
-                        "name": "params",
-                        "type": "tuple",
+                        "internalType": "uint16",
+                        "name": "cardinalityNext",
+                        "type": "uint16",
                     }
                 ],
-                "name": "decreaseLiquidity",
-                "outputs": [
-                    {"internalType": "uint256", "name": "amount0", "type": "uint256"},
-                    {"internalType": "uint256", "name": "amount1", "type": "uint256"},
-                ],
-                "stateMutability": "payable",
+                "name": "increaseObservationsCardinalityNext",
+                "outputs": [],
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "factory",
-                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "name": "isExpired",
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"}
+                    {"internalType": "address", "name": "receiver", "type": "address"},
+                    {
+                        "internalType": "uint256",
+                        "name": "netSyDesired",
+                        "type": "uint256",
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "netPtDesired",
+                        "type": "uint256",
+                    },
                 ],
-                "name": "getApproved",
+                "name": "mint",
                 "outputs": [
-                    {"internalType": "address", "name": "operator", "type": "address"}
+                    {"internalType": "uint256", "name": "netLpOut", "type": "uint256"},
+                    {"internalType": "uint256", "name": "netSyUsed", "type": "uint256"},
+                    {"internalType": "uint256", "name": "netPtUsed", "type": "uint256"},
                 ],
+                "stateMutability": "nonpayable",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "name",
+                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
                     {
-                        "components": [
-                            {
-                                "internalType": "uint256",
-                                "name": "tokenId",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "amount0Desired",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "amount1Desired",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "amount0Min",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "amount1Min",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "deadline",
-                                "type": "uint256",
-                            },
-                        ],
-                        "internalType": "struct INonfungiblePositionManager.IncreaseLiquidityParams",
-                        "name": "params",
-                        "type": "tuple",
+                        "internalType": "uint32[]",
+                        "name": "secondsAgos",
+                        "type": "uint32[]",
                     }
                 ],
-                "name": "increaseLiquidity",
+                "name": "observe",
                 "outputs": [
-                    {"internalType": "uint128", "name": "liquidity", "type": "uint128"},
-                    {"internalType": "uint256", "name": "amount0", "type": "uint256"},
-                    {"internalType": "uint256", "name": "amount1", "type": "uint256"},
-                ],
-                "stateMutability": "payable",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"},
-                    {"internalType": "address", "name": "operator", "type": "address"},
+                    {
+                        "internalType": "uint216[]",
+                        "name": "lnImpliedRateCumulative",
+                        "type": "uint216[]",
+                    }
                 ],
-                "name": "isApprovedForAll",
-                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
+                    {"internalType": "address", "name": "router", "type": "address"}
+                ],
+                "name": "readState",
+                "outputs": [
                     {
                         "components": [
                             {
-                                "internalType": "address",
-                                "name": "token0",
-                                "type": "address",
+                                "internalType": "int256",
+                                "name": "totalPt",
+                                "type": "int256",
                             },
                             {
-                                "internalType": "address",
-                                "name": "token1",
-                                "type": "address",
+                                "internalType": "int256",
+                                "name": "totalSy",
+                                "type": "int256",
                             },
-                            {"internalType": "uint24", "name": "fee", "type": "uint24"},
                             {
-                                "internalType": "int24",
-                                "name": "tickLower",
-                                "type": "int24",
+                                "internalType": "int256",
+                                "name": "totalLp",
+                                "type": "int256",
                             },
                             {
-                                "internalType": "int24",
-                                "name": "tickUpper",
-                                "type": "int24",
+                                "internalType": "address",
+                                "name": "treasury",
+                                "type": "address",
                             },
                             {
-                                "internalType": "uint256",
-                                "name": "amount0Desired",
-                                "type": "uint256",
+                                "internalType": "int256",
+                                "name": "scalarRoot",
+                                "type": "int256",
                             },
                             {
                                 "internalType": "uint256",
-                                "name": "amount1Desired",
+                                "name": "expiry",
                                 "type": "uint256",
                             },
                             {
                                 "internalType": "uint256",
-                                "name": "amount0Min",
+                                "name": "lnFeeRateRoot",
                                 "type": "uint256",
                             },
                             {
                                 "internalType": "uint256",
-                                "name": "amount1Min",
+                                "name": "reserveFeePercent",
                                 "type": "uint256",
                             },
                             {
-                                "internalType": "address",
-                                "name": "recipient",
-                                "type": "address",
-                            },
-                            {
                                 "internalType": "uint256",
-                                "name": "deadline",
+                                "name": "lastLnImpliedRate",
                                 "type": "uint256",
                             },
                         ],
-                        "internalType": "struct INonfungiblePositionManager.MintParams",
-                        "name": "params",
+                        "internalType": "struct MarketState",
+                        "name": "market",
                         "type": "tuple",
                     }
                 ],
-                "name": "mint",
-                "outputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
-                    {"internalType": "uint128", "name": "liquidity", "type": "uint128"},
-                    {"internalType": "uint256", "name": "amount0", "type": "uint256"},
-                    {"internalType": "uint256", "name": "amount1", "type": "uint256"},
-                ],
-                "stateMutability": "payable",
-                "type": "function",
-            },
-            {
-                "inputs": [],
-                "name": "name",
-                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"}
-                ],
-                "name": "ownerOf",
-                "outputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"}
-                ],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "address", "name": "spender", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
-                    {"internalType": "uint256", "name": "deadline", "type": "uint256"},
-                    {"internalType": "uint8", "name": "v", "type": "uint8"},
-                    {"internalType": "bytes32", "name": "r", "type": "bytes32"},
-                    {"internalType": "bytes32", "name": "s", "type": "bytes32"},
-                ],
-                "name": "permit",
-                "outputs": [],
-                "stateMutability": "payable",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"}
-                ],
-                "name": "positions",
+                "inputs": [],
+                "name": "readTokens",
                 "outputs": [
-                    {"internalType": "uint96", "name": "nonce", "type": "uint96"},
-                    {"internalType": "address", "name": "operator", "type": "address"},
-                    {"internalType": "address", "name": "token0", "type": "address"},
-                    {"internalType": "address", "name": "token1", "type": "address"},
-                    {"internalType": "uint24", "name": "fee", "type": "uint24"},
-                    {"internalType": "int24", "name": "tickLower", "type": "int24"},
-                    {"internalType": "int24", "name": "tickUpper", "type": "int24"},
-                    {"internalType": "uint128", "name": "liquidity", "type": "uint128"},
                     {
-                        "internalType": "uint256",
-                        "name": "feeGrowthInside0LastX128",
-                        "type": "uint256",
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "feeGrowthInside1LastX128",
-                        "type": "uint256",
+                        "internalType": "contract IStandardizedYield",
+                        "name": "_SY",
+                        "type": "address",
                     },
                     {
-                        "internalType": "uint128",
-                        "name": "tokensOwed0",
-                        "type": "uint128",
+                        "internalType": "contract IPPrincipalToken",
+                        "name": "_PT",
+                        "type": "address",
                     },
                     {
-                        "internalType": "uint128",
-                        "name": "tokensOwed1",
-                        "type": "uint128",
+                        "internalType": "contract IPYieldToken",
+                        "name": "_YT",
+                        "type": "address",
                     },
                 ],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [],
-                "name": "refundETH",
-                "outputs": [],
-                "stateMutability": "payable",
-                "type": "function",
-            },
-            {
                 "inputs": [
-                    {"internalType": "address", "name": "from", "type": "address"},
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
+                    {"internalType": "address", "name": "user", "type": "address"}
+                ],
+                "name": "redeemRewards",
+                "outputs": [
+                    {"internalType": "uint256[]", "name": "", "type": "uint256[]"}
                 ],
-                "name": "safeTransferFrom",
-                "outputs": [],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "from", "type": "address"},
-                    {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
+                    {"internalType": "address", "name": "receiver", "type": "address"},
+                    {"internalType": "uint256", "name": "exactPtIn", "type": "uint256"},
                     {"internalType": "bytes", "name": "data", "type": "bytes"},
                 ],
-                "name": "safeTransferFrom",
-                "outputs": [],
-                "stateMutability": "nonpayable",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "address", "name": "operator", "type": "address"},
-                    {"internalType": "bool", "name": "_approved", "type": "bool"},
+                "name": "swapExactPtForSy",
+                "outputs": [
+                    {"internalType": "uint256", "name": "netSyOut", "type": "uint256"},
+                    {"internalType": "uint256", "name": "netSyFee", "type": "uint256"},
                 ],
-                "name": "setApprovalForAll",
-                "outputs": [],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "bytes4", "name": "interfaceId", "type": "bytes4"}
-                ],
-                "name": "supportsInterface",
-                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "address", "name": "token", "type": "address"},
+                    {"internalType": "address", "name": "receiver", "type": "address"},
                     {
                         "internalType": "uint256",
-                        "name": "amountMinimum",
+                        "name": "exactPtOut",
                         "type": "uint256",
                     },
-                    {"internalType": "address", "name": "recipient", "type": "address"},
+                    {"internalType": "bytes", "name": "data", "type": "bytes"},
                 ],
-                "name": "sweepToken",
-                "outputs": [],
-                "stateMutability": "payable",
+                "name": "swapSyForExactPt",
+                "outputs": [
+                    {"internalType": "uint256", "name": "netSyIn", "type": "uint256"},
+                    {"internalType": "uint256", "name": "netSyFee", "type": "uint256"},
+                ],
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [],
                 "name": "symbol",
                 "outputs": [{"internalType": "string", "name": "", "type": "string"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "uint256", "name": "index", "type": "uint256"}
-                ],
-                "name": "tokenByIndex",
-                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "address", "name": "owner", "type": "address"},
-                    {"internalType": "uint256", "name": "index", "type": "uint256"},
-                ],
-                "name": "tokenOfOwnerByIndex",
+                "inputs": [],
+                "name": "totalActiveSupply",
                 "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"}
-                ],
-                "name": "tokenURI",
-                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
                 "inputs": [],
                 "name": "totalSupply",
                 "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "from", "type": "address"},
                     {"internalType": "address", "name": "to", "type": "address"},
-                    {"internalType": "uint256", "name": "tokenId", "type": "uint256"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
-                "name": "transferFrom",
-                "outputs": [],
+                "name": "transfer",
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {
-                        "internalType": "uint256",
-                        "name": "amountMinimum",
-                        "type": "uint256",
-                    },
-                    {"internalType": "address", "name": "recipient", "type": "address"},
+                    {"internalType": "address", "name": "from", "type": "address"},
+                    {"internalType": "address", "name": "to", "type": "address"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
-                "name": "unwrapWETH9",
-                "outputs": [],
-                "stateMutability": "payable",
+                "name": "transferFrom",
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def d_o_m_a_i_n__s_e_p_a_r_a_t_o_r(self) -> bytes:
+    def active_balance(self, user: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.DOMAIN_SEPARATOR().call()
+        return c.functions.activeBalance(user).call()
 
-    def p_e_r_m_i_t__t_y_p_e_h_a_s_h(
-        self, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
+    def allowance(self, owner: str, spender: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.PERMIT_TYPEHASH().build_transaction(override_tx_parameters)
-
-    def w_e_t_h9(self) -> str:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.WETH9().call()
+        return c.functions.allowance(owner, spender).call()
 
     def approve(
-        self, to: str, token_id: int, override_tx_parameters: Optional[TxParams] = None
+        self,
+        spender: str,
+        amount: int,
+        override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.approve(to, token_id).build_transaction(
+        return c.functions.approve(spender, amount).build_transaction(
             override_tx_parameters
         )
 
-    def balance_of(self, owner: str) -> int:
+    def balance_of(self, account: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.balanceOf(owner).call()
+        return c.functions.balanceOf(account).call()
 
     def burn(
-        self, token_id: int, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.burn(token_id).build_transaction(override_tx_parameters)
-
-    def collect(
-        self, params: tuple, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.collect(params).build_transaction(override_tx_parameters)
-
-    def create_and_initialize_pool_if_necessary(
         self,
-        token0: str,
-        token1: str,
-        fee: None,
-        sqrt_price_x96: None,
+        receiver_sy: str,
+        receiver_pt: str,
+        net_lp_to_burn: int,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.createAndInitializePoolIfNecessary(
-            token0, token1, fee, sqrt_price_x96
+        return c.functions.burn(
+            receiver_sy, receiver_pt, net_lp_to_burn
         ).build_transaction(override_tx_parameters)
 
-    def decrease_liquidity(
-        self, params: tuple, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
+    def decimals(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.decreaseLiquidity(params).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.decimals().call()
 
-    def factory(self) -> str:
+    def expiry(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.factory().call()
+        return c.functions.expiry().call()
 
-    def get_approved(self, token_id: int) -> str:
+    def get_reward_tokens(self) -> List[str]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.getApproved(token_id).call()
+        return c.functions.getRewardTokens().call()
 
-    def increase_liquidity(
-        self, params: tuple, override_tx_parameters: Optional[TxParams] = None
+    def increase_observations_cardinality_next(
+        self, cardinality_next: int, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.increaseLiquidity(params).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.increaseObservationsCardinalityNext(
+            cardinality_next
+        ).build_transaction(override_tx_parameters)
 
-    def is_approved_for_all(self, owner: str, operator: str) -> bool:
+    def is_expired(self) -> bool:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.isApprovedForAll(owner, operator).call()
+        return c.functions.isExpired().call()
 
     def mint(
-        self, params: tuple, override_tx_parameters: Optional[TxParams] = None
+        self,
+        receiver: str,
+        net_sy_desired: int,
+        net_pt_desired: int,
+        override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.mint(params).build_transaction(override_tx_parameters)
-
-    def name(self) -> TxParams:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.name().build_transaction()
+        return c.functions.mint(
+            receiver, net_sy_desired, net_pt_desired
+        ).build_transaction(override_tx_parameters)
 
-    def owner_of(self, token_id: int) -> str:
+    def name(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.ownerOf(token_id).call()
+        return c.functions.name().call()
 
-    def permit(
-        self,
-        spender: str,
-        token_id: int,
-        deadline: int,
-        v: int,
-        r: bytes,
-        s: bytes,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def observe(self, seconds_agos: List[int]) -> List[int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.permit(
-            spender, token_id, deadline, v, r, s
-        ).build_transaction(override_tx_parameters)
+        return c.functions.observe(seconds_agos).call()
 
-    def positions(self, token_id: int) -> TxParams:
+    def read_state(self, router: str) -> tuple:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.positions(token_id).build_transaction()
+        return c.functions.readState(router).call()
 
-    def refund_e_t_h(
-        self, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
+    def read_tokens(self) -> Tuple[str, str, str]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.refundETH().build_transaction(override_tx_parameters)
+        return c.functions.readTokens().call()
 
-    def safe_transfer_from(
-        self,
-        _from: str,
-        to: str,
-        token_id: int,
-        override_tx_parameters: Optional[TxParams] = None,
+    def redeem_rewards(
+        self, user: str, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.safeTransferFrom(_from, to, token_id).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.redeemRewards(user).build_transaction(override_tx_parameters)
 
-    def safe_transfer_from(
+    def swap_exact_pt_for_sy(
         self,
-        _from: str,
-        to: str,
-        token_id: int,
+        receiver: str,
+        exact_pt_in: int,
         data: bytes,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.safeTransferFrom(
-            _from, to, token_id, data
+        return c.functions.swapExactPtForSy(
+            receiver, exact_pt_in, data
         ).build_transaction(override_tx_parameters)
 
-    def set_approval_for_all(
+    def swap_sy_for_exact_pt(
         self,
-        operator: str,
-        _approved: bool,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.setApprovalForAll(operator, _approved).build_transaction(
-            override_tx_parameters
-        )
-
-    def supports_interface(self, interface_id: None) -> bool:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.supportsInterface(interface_id).call()
-
-    def sweep_token(
-        self,
-        token: str,
-        amount_minimum: int,
-        recipient: str,
+        receiver: str,
+        exact_pt_out: int,
+        data: bytes,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.sweepToken(
-            token, amount_minimum, recipient
+        return c.functions.swapSyForExactPt(
+            receiver, exact_pt_out, data
         ).build_transaction(override_tx_parameters)
 
-    def symbol(self) -> TxParams:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.symbol().build_transaction()
-
-    def token_by_index(self, index: int) -> int:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.tokenByIndex(index).call()
-
-    def token_of_owner_by_index(self, owner: str, index: int) -> int:
+    def symbol(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.tokenOfOwnerByIndex(owner, index).call()
+        return c.functions.symbol().call()
 
-    def token_u_r_i(self, token_id: int) -> TxParams:
+    def total_active_supply(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.tokenURI(token_id).build_transaction()
+        return c.functions.totalActiveSupply().call()
 
     def total_supply(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.totalSupply().call()
 
-    def transfer_from(
-        self,
-        _from: str,
-        to: str,
-        token_id: int,
-        override_tx_parameters: Optional[TxParams] = None,
+    def transfer(
+        self, to: str, amount: int, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.transferFrom(_from, to, token_id).build_transaction(
+        return c.functions.transfer(to, amount).build_transaction(
             override_tx_parameters
         )
 
-    def unwrap_w_e_t_h9(
+    def transfer_from(
         self,
-        amount_minimum: int,
-        recipient: str,
+        _from: str,
+        to: str,
+        amount: int,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.unwrapWETH9(amount_minimum, recipient).build_transaction(
+        return c.functions.transferFrom(_from, to, amount).build_transaction(
             override_tx_parameters
         )
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_periphery_immutable_state.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_gauge.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-from typing import Optional, Union
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class IPeripheryImmutableState:
+class IPGauge:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
             {
-                "inputs": [],
-                "name": "WETH9",
-                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "inputs": [
+                    {"internalType": "address", "name": "user", "type": "address"}
+                ],
+                "name": "activeBalance",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "factory",
-                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "name": "totalActiveSupply",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def w_e_t_h9(self) -> str:
+    def active_balance(self, user: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.WETH9().call()
+        return c.functions.activeBalance(user).call()
 
-    def factory(self) -> str:
+    def total_active_supply(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.factory().call()
+        return c.functions.totalActiveSupply().call()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_periphery_payments.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_swap_aggregator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,96 @@
-from typing import Optional, Union
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
+from .multi_approval import MultiApproval
+from .call3 import Call3
+
+
+def serialize_struct(d) -> tuple:
+    if isinstance(d, dict):
+        return tuple(serialize_struct(v) for v in d.values())
+    elif isinstance(d, (list, tuple)):
+        return tuple(serialize_struct(x) for x in d)
+    else:
+        return d
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class IPeripheryPayments:
+class IPSwapAggregator:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
             {
-                "inputs": [],
-                "name": "refundETH",
-                "outputs": [],
-                "stateMutability": "payable",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "address", "name": "token", "type": "address"},
-                    {
-                        "internalType": "uint256",
-                        "name": "amountMinimum",
-                        "type": "uint256",
-                    },
-                    {"internalType": "address", "name": "recipient", "type": "address"},
-                ],
-                "name": "sweepToken",
-                "outputs": [],
-                "stateMutability": "payable",
-                "type": "function",
-            },
-            {
                 "inputs": [
+                    {"internalType": "address", "name": "tokenIn", "type": "address"},
+                    {"internalType": "uint256", "name": "amountIn", "type": "uint256"},
                     {
-                        "internalType": "uint256",
-                        "name": "amountMinimum",
-                        "type": "uint256",
+                        "components": [
+                            {
+                                "internalType": "enum SwapType",
+                                "name": "swapType",
+                                "type": "uint8",
+                            },
+                            {
+                                "internalType": "address",
+                                "name": "extRouter",
+                                "type": "address",
+                            },
+                            {
+                                "internalType": "bytes",
+                                "name": "extCalldata",
+                                "type": "bytes",
+                            },
+                            {
+                                "internalType": "bool",
+                                "name": "needScale",
+                                "type": "bool",
+                            },
+                        ],
+                        "internalType": "struct SwapData",
+                        "name": "swapData",
+                        "type": "tuple",
                     },
-                    {"internalType": "address", "name": "recipient", "type": "address"},
                 ],
-                "name": "unwrapWETH9",
+                "name": "swap",
                 "outputs": [],
                 "stateMutability": "payable",
                 "type": "function",
-            },
+            }
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def refund_e_t_h(
-        self, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.refundETH().build_transaction(override_tx_parameters)
-
-    def sweep_token(
+    def swap(
         self,
-        token: str,
-        amount_minimum: int,
-        recipient: str,
+        token_in: str,
+        amount_in: int,
+        swap_data: SwapData,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.sweepToken(
-            token, amount_minimum, recipient
+        return c.functions.swap(
+            token_in, amount_in, serialize_struct(swap_data)
         ).build_transaction(override_tx_parameters)
-
-    def unwrap_w_e_t_h9(
-        self,
-        amount_minimum: int,
-        recipient: str,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.unwrapWETH9(amount_minimum, recipient).build_transaction(
-            override_tx_parameters
-        )
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_pool_initializer.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_market_swap_callback.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,70 @@
-from typing import Optional, Union
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
+from .multi_approval import MultiApproval
+from .call3 import Call3
+
+
+def serialize_struct(d) -> tuple:
+    if isinstance(d, dict):
+        return tuple(serialize_struct(v) for v in d.values())
+    elif isinstance(d, (list, tuple)):
+        return tuple(serialize_struct(x) for x in d)
+    else:
+        return d
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class IPoolInitializer:
+class IPMarketSwapCallback:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
             {
                 "inputs": [
-                    {"internalType": "address", "name": "token0", "type": "address"},
-                    {"internalType": "address", "name": "token1", "type": "address"},
-                    {"internalType": "uint24", "name": "fee", "type": "uint24"},
-                    {
-                        "internalType": "uint160",
-                        "name": "sqrtPriceX96",
-                        "type": "uint160",
-                    },
-                ],
-                "name": "createAndInitializePoolIfNecessary",
-                "outputs": [
-                    {"internalType": "address", "name": "pool", "type": "address"}
+                    {"internalType": "int256", "name": "ptToAccount", "type": "int256"},
+                    {"internalType": "int256", "name": "syToAccount", "type": "int256"},
+                    {"internalType": "bytes", "name": "data", "type": "bytes"},
                 ],
-                "stateMutability": "payable",
+                "name": "swapCallback",
+                "outputs": [],
+                "stateMutability": "nonpayable",
                 "type": "function",
             }
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def create_and_initialize_pool_if_necessary(
+    def swap_callback(
         self,
-        token0: str,
-        token1: str,
-        fee: None,
-        sqrt_price_x96: None,
+        pt_to_account: int,
+        sy_to_account: int,
+        data: bytes,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.createAndInitializePoolIfNecessary(
-            token0, token1, fee, sqrt_price_x96
+        return c.functions.swapCallback(
+            pt_to_account, sy_to_account, data
         ).build_transaction(override_tx_parameters)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_swap_router.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_action_storage_static.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,293 +1,276 @@
-from typing import Optional, Union
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
+from .multi_approval import MultiApproval
+from .call3 import Call3
+
+
+def serialize_struct(d) -> tuple:
+    if isinstance(d, dict):
+        return tuple(serialize_struct(v) for v in d.values())
+    elif isinstance(d, (list, tuple)):
+        return tuple(serialize_struct(x) for x in d)
+    else:
+        return d
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class ISwapRouter:
+class IPActionStorageStatic:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
             {
+                "anonymous": False,
                 "inputs": [
                     {
-                        "components": [
-                            {"internalType": "bytes", "name": "path", "type": "bytes"},
-                            {
-                                "internalType": "address",
-                                "name": "recipient",
-                                "type": "address",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "deadline",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "amountIn",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "amountOutMinimum",
-                                "type": "uint256",
-                            },
-                        ],
-                        "internalType": "struct ISwapRouter.ExactInputParams",
-                        "name": "params",
-                        "type": "tuple",
-                    }
-                ],
-                "name": "exactInput",
-                "outputs": [
-                    {"internalType": "uint256", "name": "amountOut", "type": "uint256"}
+                        "indexed": True,
+                        "internalType": "address",
+                        "name": "previousOwner",
+                        "type": "address",
+                    },
+                    {
+                        "indexed": True,
+                        "internalType": "address",
+                        "name": "newOwner",
+                        "type": "address",
+                    },
                 ],
-                "stateMutability": "payable",
+                "name": "OwnershipTransferred",
+                "type": "event",
+            },
+            {
+                "inputs": [],
+                "name": "claimOwnership",
+                "outputs": [],
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
-                "inputs": [
+                "inputs": [],
+                "name": "getBulkSellerFactory",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "getDefaultApproxParams",
+                "outputs": [
                     {
                         "components": [
                             {
-                                "internalType": "address",
-                                "name": "tokenIn",
-                                "type": "address",
-                            },
-                            {
-                                "internalType": "address",
-                                "name": "tokenOut",
-                                "type": "address",
-                            },
-                            {"internalType": "uint24", "name": "fee", "type": "uint24"},
-                            {
-                                "internalType": "address",
-                                "name": "recipient",
-                                "type": "address",
+                                "internalType": "uint256",
+                                "name": "guessMin",
+                                "type": "uint256",
                             },
                             {
                                 "internalType": "uint256",
-                                "name": "deadline",
+                                "name": "guessMax",
                                 "type": "uint256",
                             },
                             {
                                 "internalType": "uint256",
-                                "name": "amountIn",
+                                "name": "guessOffchain",
                                 "type": "uint256",
                             },
                             {
                                 "internalType": "uint256",
-                                "name": "amountOutMinimum",
+                                "name": "maxIteration",
                                 "type": "uint256",
                             },
                             {
-                                "internalType": "uint160",
-                                "name": "sqrtPriceLimitX96",
-                                "type": "uint160",
+                                "internalType": "uint256",
+                                "name": "eps",
+                                "type": "uint256",
                             },
                         ],
-                        "internalType": "struct ISwapRouter.ExactInputSingleParams",
-                        "name": "params",
+                        "internalType": "struct ApproxParams",
+                        "name": "",
                         "type": "tuple",
                     }
                 ],
-                "name": "exactInputSingle",
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "getOwnerAndPendingOwner",
                 "outputs": [
-                    {"internalType": "uint256", "name": "amountOut", "type": "uint256"}
+                    {"internalType": "address", "name": "_owner", "type": "address"},
+                    {
+                        "internalType": "address",
+                        "name": "_pendingOwner",
+                        "type": "address",
+                    },
                 ],
-                "stateMutability": "payable",
+                "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
                     {
-                        "components": [
-                            {"internalType": "bytes", "name": "path", "type": "bytes"},
-                            {
-                                "internalType": "address",
-                                "name": "recipient",
-                                "type": "address",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "deadline",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "amountOut",
-                                "type": "uint256",
-                            },
-                            {
-                                "internalType": "uint256",
-                                "name": "amountInMaximum",
-                                "type": "uint256",
-                            },
-                        ],
-                        "internalType": "struct ISwapRouter.ExactOutputParams",
-                        "name": "params",
-                        "type": "tuple",
+                        "internalType": "address",
+                        "name": "_bulkSellerFactory",
+                        "type": "address",
                     }
                 ],
-                "name": "exactOutput",
-                "outputs": [
-                    {"internalType": "uint256", "name": "amountIn", "type": "uint256"}
-                ],
-                "stateMutability": "payable",
+                "name": "setBulkSellerFactory",
+                "outputs": [],
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
                     {
                         "components": [
                             {
-                                "internalType": "address",
-                                "name": "tokenIn",
-                                "type": "address",
-                            },
-                            {
-                                "internalType": "address",
-                                "name": "tokenOut",
-                                "type": "address",
-                            },
-                            {"internalType": "uint24", "name": "fee", "type": "uint24"},
-                            {
-                                "internalType": "address",
-                                "name": "recipient",
-                                "type": "address",
+                                "internalType": "uint256",
+                                "name": "guessMin",
+                                "type": "uint256",
                             },
                             {
                                 "internalType": "uint256",
-                                "name": "deadline",
+                                "name": "guessMax",
                                 "type": "uint256",
                             },
                             {
                                 "internalType": "uint256",
-                                "name": "amountOut",
+                                "name": "guessOffchain",
                                 "type": "uint256",
                             },
                             {
                                 "internalType": "uint256",
-                                "name": "amountInMaximum",
+                                "name": "maxIteration",
                                 "type": "uint256",
                             },
                             {
-                                "internalType": "uint160",
-                                "name": "sqrtPriceLimitX96",
-                                "type": "uint160",
+                                "internalType": "uint256",
+                                "name": "eps",
+                                "type": "uint256",
                             },
                         ],
-                        "internalType": "struct ISwapRouter.ExactOutputSingleParams",
+                        "internalType": "struct ApproxParams",
                         "name": "params",
                         "type": "tuple",
                     }
                 ],
-                "name": "exactOutputSingle",
-                "outputs": [
-                    {"internalType": "uint256", "name": "amountIn", "type": "uint256"}
-                ],
-                "stateMutability": "payable",
+                "name": "setDefaultApproxParams",
+                "outputs": [],
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {
-                        "internalType": "int256",
-                        "name": "amount0Delta",
-                        "type": "int256",
-                    },
-                    {
-                        "internalType": "int256",
-                        "name": "amount1Delta",
-                        "type": "int256",
-                    },
-                    {"internalType": "bytes", "name": "data", "type": "bytes"},
+                    {"internalType": "address", "name": "newOwner", "type": "address"},
+                    {"internalType": "bool", "name": "direct", "type": "bool"},
+                    {"internalType": "bool", "name": "renounce", "type": "bool"},
                 ],
-                "name": "uniswapV3SwapCallback",
+                "name": "transferOwnership",
                 "outputs": [],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def exact_input(
-        self, params: tuple, override_tx_parameters: Optional[TxParams] = None
+    def claim_ownership(
+        self, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.exactInput(params).build_transaction(override_tx_parameters)
+        return c.functions.claimOwnership().build_transaction(override_tx_parameters)
 
-    def exact_input_single(
-        self, params: tuple, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
+    def get_bulk_seller_factory(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.exactInputSingle(params).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.getBulkSellerFactory().call()
 
-    def exact_output(
-        self, params: tuple, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
+    def get_default_approx_params(self) -> tuple:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.exactOutput(params).build_transaction(override_tx_parameters)
+        return c.functions.getDefaultApproxParams().call()
 
-    def exact_output_single(
-        self, params: tuple, override_tx_parameters: Optional[TxParams] = None
+    def get_owner_and_pending_owner(self) -> Tuple[str, str]:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.getOwnerAndPendingOwner().call()
+
+    def set_bulk_seller_factory(
+        self,
+        _bulk_seller_factory: str,
+        override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.exactOutputSingle(params).build_transaction(
+        return c.functions.setBulkSellerFactory(_bulk_seller_factory).build_transaction(
             override_tx_parameters
         )
 
-    def uniswap_v3_swap_callback(
+    def set_default_approx_params(
+        self, params: ApproxParams, override_tx_parameters: Optional[TxParams] = None
+    ) -> TxParams:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.setDefaultApproxParams(
+            serialize_struct(params)
+        ).build_transaction(override_tx_parameters)
+
+    def transfer_ownership(
         self,
-        amount0_delta: None,
-        amount1_delta: None,
-        data: bytes,
+        new_owner: str,
+        direct: bool,
+        renounce: bool,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.uniswapV3SwapCallback(
-            amount0_delta, amount1_delta, data
+        return c.functions.transferOwnership(
+            new_owner, direct, renounce
         ).build_transaction(override_tx_parameters)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/i_uniswap_v3_pool.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_yield_token.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Optional, Union
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class IUniswapV3Pool:
+class IPYieldToken:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
@@ -23,1054 +23,737 @@
                         "indexed": True,
                         "internalType": "address",
                         "name": "owner",
                         "type": "address",
                     },
                     {
                         "indexed": True,
-                        "internalType": "int24",
-                        "name": "tickLower",
-                        "type": "int24",
-                    },
-                    {
-                        "indexed": True,
-                        "internalType": "int24",
-                        "name": "tickUpper",
-                        "type": "int24",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "uint128",
-                        "name": "amount",
-                        "type": "uint128",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "uint256",
-                        "name": "amount0",
-                        "type": "uint256",
+                        "internalType": "address",
+                        "name": "spender",
+                        "type": "address",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "amount1",
+                        "name": "value",
                         "type": "uint256",
                     },
                 ],
-                "name": "Burn",
+                "name": "Approval",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "owner",
+                        "name": "caller",
                         "type": "address",
                     },
                     {
-                        "indexed": False,
+                        "indexed": True,
                         "internalType": "address",
-                        "name": "recipient",
+                        "name": "receiver",
                         "type": "address",
                     },
                     {
-                        "indexed": True,
-                        "internalType": "int24",
-                        "name": "tickLower",
-                        "type": "int24",
-                    },
-                    {
-                        "indexed": True,
-                        "internalType": "int24",
-                        "name": "tickUpper",
-                        "type": "int24",
-                    },
-                    {
                         "indexed": False,
-                        "internalType": "uint128",
-                        "name": "amount0",
-                        "type": "uint128",
+                        "internalType": "uint256",
+                        "name": "amountPYToRedeem",
+                        "type": "uint256",
                     },
                     {
                         "indexed": False,
-                        "internalType": "uint128",
-                        "name": "amount1",
-                        "type": "uint128",
+                        "internalType": "uint256",
+                        "name": "amountSyOut",
+                        "type": "uint256",
                     },
                 ],
-                "name": "Collect",
+                "name": "Burn",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "sender",
+                        "name": "caller",
                         "type": "address",
                     },
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "recipient",
+                        "name": "receiverPT",
                         "type": "address",
                     },
                     {
-                        "indexed": False,
-                        "internalType": "uint128",
-                        "name": "amount0",
-                        "type": "uint128",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "uint128",
-                        "name": "amount1",
-                        "type": "uint128",
-                    },
-                ],
-                "name": "CollectProtocol",
-                "type": "event",
-            },
-            {
-                "anonymous": False,
-                "inputs": [
-                    {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "sender",
-                        "type": "address",
-                    },
-                    {
-                        "indexed": True,
-                        "internalType": "address",
-                        "name": "recipient",
+                        "name": "receiverYT",
                         "type": "address",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "amount0",
+                        "name": "amountSyToMint",
                         "type": "uint256",
                     },
                     {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "amount1",
-                        "type": "uint256",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "uint256",
-                        "name": "paid0",
-                        "type": "uint256",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "uint256",
-                        "name": "paid1",
+                        "name": "amountPYOut",
                         "type": "uint256",
                     },
                 ],
-                "name": "Flash",
-                "type": "event",
-            },
-            {
-                "anonymous": False,
-                "inputs": [
-                    {
-                        "indexed": False,
-                        "internalType": "uint16",
-                        "name": "observationCardinalityNextOld",
-                        "type": "uint16",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "uint16",
-                        "name": "observationCardinalityNextNew",
-                        "type": "uint16",
-                    },
-                ],
-                "name": "IncreaseObservationCardinalityNext",
+                "name": "Mint",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
-                        "indexed": False,
-                        "internalType": "uint160",
-                        "name": "sqrtPriceX96",
-                        "type": "uint160",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "int24",
-                        "name": "tick",
-                        "type": "int24",
-                    },
+                        "indexed": True,
+                        "internalType": "uint256",
+                        "name": "newIndex",
+                        "type": "uint256",
+                    }
                 ],
-                "name": "Initialize",
+                "name": "NewInterestIndex",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
-                        "indexed": False,
-                        "internalType": "address",
-                        "name": "sender",
-                        "type": "address",
-                    },
-                    {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "owner",
+                        "name": "user",
                         "type": "address",
                     },
                     {
-                        "indexed": True,
-                        "internalType": "int24",
-                        "name": "tickLower",
-                        "type": "int24",
-                    },
-                    {
-                        "indexed": True,
-                        "internalType": "int24",
-                        "name": "tickUpper",
-                        "type": "int24",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "uint128",
-                        "name": "amount",
-                        "type": "uint128",
-                    },
-                    {
                         "indexed": False,
                         "internalType": "uint256",
-                        "name": "amount0",
-                        "type": "uint256",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "uint256",
-                        "name": "amount1",
+                        "name": "interestOut",
                         "type": "uint256",
                     },
                 ],
-                "name": "Mint",
+                "name": "RedeemInterest",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
-                        "indexed": False,
-                        "internalType": "uint8",
-                        "name": "feeProtocol0Old",
-                        "type": "uint8",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "uint8",
-                        "name": "feeProtocol1Old",
-                        "type": "uint8",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "uint8",
-                        "name": "feeProtocol0New",
-                        "type": "uint8",
+                        "indexed": True,
+                        "internalType": "address",
+                        "name": "user",
+                        "type": "address",
                     },
                     {
                         "indexed": False,
-                        "internalType": "uint8",
-                        "name": "feeProtocol1New",
-                        "type": "uint8",
+                        "internalType": "uint256[]",
+                        "name": "amountRewardsOut",
+                        "type": "uint256[]",
                     },
                 ],
-                "name": "SetFeeProtocol",
+                "name": "RedeemRewards",
                 "type": "event",
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "sender",
+                        "name": "from",
                         "type": "address",
                     },
                     {
                         "indexed": True,
                         "internalType": "address",
-                        "name": "recipient",
+                        "name": "to",
                         "type": "address",
                     },
                     {
                         "indexed": False,
-                        "internalType": "int256",
-                        "name": "amount0",
-                        "type": "int256",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "int256",
-                        "name": "amount1",
-                        "type": "int256",
-                    },
-                    {
-                        "indexed": False,
-                        "internalType": "uint160",
-                        "name": "sqrtPriceX96",
-                        "type": "uint160",
+                        "internalType": "uint256",
+                        "name": "value",
+                        "type": "uint256",
                     },
+                ],
+                "name": "Transfer",
+                "type": "event",
+            },
+            {
+                "anonymous": False,
+                "inputs": [
                     {
                         "indexed": False,
-                        "internalType": "uint128",
-                        "name": "liquidity",
-                        "type": "uint128",
+                        "internalType": "uint256[]",
+                        "name": "amountRewardsOut",
+                        "type": "uint256[]",
                     },
                     {
                         "indexed": False,
-                        "internalType": "int24",
-                        "name": "tick",
-                        "type": "int24",
+                        "internalType": "uint256",
+                        "name": "syOut",
+                        "type": "uint256",
                     },
                 ],
-                "name": "Swap",
+                "name": "WithdrawFeeToTreasury",
                 "type": "event",
             },
             {
+                "inputs": [],
+                "name": "PT",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "SY",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
                 "inputs": [
-                    {"internalType": "int24", "name": "tickLower", "type": "int24"},
-                    {"internalType": "int24", "name": "tickUpper", "type": "int24"},
-                    {"internalType": "uint128", "name": "amount", "type": "uint128"},
-                ],
-                "name": "burn",
-                "outputs": [
-                    {"internalType": "uint256", "name": "amount0", "type": "uint256"},
-                    {"internalType": "uint256", "name": "amount1", "type": "uint256"},
+                    {"internalType": "address", "name": "owner", "type": "address"},
+                    {"internalType": "address", "name": "spender", "type": "address"},
                 ],
-                "stateMutability": "nonpayable",
+                "name": "allowance",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "recipient", "type": "address"},
-                    {"internalType": "int24", "name": "tickLower", "type": "int24"},
-                    {"internalType": "int24", "name": "tickUpper", "type": "int24"},
-                    {
-                        "internalType": "uint128",
-                        "name": "amount0Requested",
-                        "type": "uint128",
-                    },
-                    {
-                        "internalType": "uint128",
-                        "name": "amount1Requested",
-                        "type": "uint128",
-                    },
-                ],
-                "name": "collect",
-                "outputs": [
-                    {"internalType": "uint128", "name": "amount0", "type": "uint128"},
-                    {"internalType": "uint128", "name": "amount1", "type": "uint128"},
+                    {"internalType": "address", "name": "spender", "type": "address"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
+                "name": "approve",
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "recipient", "type": "address"},
-                    {
-                        "internalType": "uint128",
-                        "name": "amount0Requested",
-                        "type": "uint128",
-                    },
-                    {
-                        "internalType": "uint128",
-                        "name": "amount1Requested",
-                        "type": "uint128",
-                    },
+                    {"internalType": "address", "name": "account", "type": "address"}
                 ],
-                "name": "collectProtocol",
-                "outputs": [
-                    {"internalType": "uint128", "name": "amount0", "type": "uint128"},
-                    {"internalType": "uint128", "name": "amount1", "type": "uint128"},
-                ],
-                "stateMutability": "nonpayable",
+                "name": "balanceOf",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "factory",
-                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "name": "decimals",
+                "outputs": [{"internalType": "uint8", "name": "", "type": "uint8"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "fee",
-                "outputs": [{"internalType": "uint24", "name": "", "type": "uint24"}],
+                "name": "doCacheIndexSameBlock",
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "feeGrowthGlobal0X128",
+                "name": "expiry",
                 "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "feeGrowthGlobal1X128",
-                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "name": "factory",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "recipient", "type": "address"},
-                    {"internalType": "uint256", "name": "amount0", "type": "uint256"},
-                    {"internalType": "uint256", "name": "amount1", "type": "uint256"},
-                    {"internalType": "bytes", "name": "data", "type": "bytes"},
+                "inputs": [],
+                "name": "getRewardTokens",
+                "outputs": [
+                    {"internalType": "address[]", "name": "", "type": "address[]"}
                 ],
-                "name": "flash",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {
-                        "internalType": "uint16",
-                        "name": "observationCardinalityNext",
-                        "type": "uint16",
-                    }
-                ],
-                "name": "increaseObservationCardinalityNext",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "inputs": [],
+                "name": "isExpired",
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
                     {
-                        "internalType": "uint160",
-                        "name": "sqrtPriceX96",
-                        "type": "uint160",
+                        "internalType": "address",
+                        "name": "receiverPT",
+                        "type": "address",
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "receiverYT",
+                        "type": "address",
+                    },
+                ],
+                "name": "mintPY",
+                "outputs": [
+                    {
+                        "internalType": "uint256",
+                        "name": "amountPYOut",
+                        "type": "uint256",
                     }
                 ],
-                "name": "initialize",
-                "outputs": [],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "liquidity",
-                "outputs": [{"internalType": "uint128", "name": "", "type": "uint128"}],
+                "name": "name",
+                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "maxLiquidityPerTick",
-                "outputs": [{"internalType": "uint128", "name": "", "type": "uint128"}],
-                "stateMutability": "view",
+                "name": "pyIndexCurrent",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "recipient", "type": "address"},
-                    {"internalType": "int24", "name": "tickLower", "type": "int24"},
-                    {"internalType": "int24", "name": "tickUpper", "type": "int24"},
-                    {"internalType": "uint128", "name": "amount", "type": "uint128"},
-                    {"internalType": "bytes", "name": "data", "type": "bytes"},
-                ],
-                "name": "mint",
-                "outputs": [
-                    {"internalType": "uint256", "name": "amount0", "type": "uint256"},
-                    {"internalType": "uint256", "name": "amount1", "type": "uint256"},
-                ],
-                "stateMutability": "nonpayable",
+                "inputs": [],
+                "name": "pyIndexStored",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "uint256", "name": "index", "type": "uint256"}
+                    {"internalType": "address", "name": "user", "type": "address"},
+                    {"internalType": "bool", "name": "redeemInterest", "type": "bool"},
+                    {"internalType": "bool", "name": "redeemRewards", "type": "bool"},
                 ],
-                "name": "observations",
+                "name": "redeemDueInterestAndRewards",
                 "outputs": [
                     {
-                        "internalType": "uint32",
-                        "name": "blockTimestamp",
-                        "type": "uint32",
-                    },
-                    {
-                        "internalType": "int56",
-                        "name": "tickCumulative",
-                        "type": "int56",
+                        "internalType": "uint256",
+                        "name": "interestOut",
+                        "type": "uint256",
                     },
                     {
-                        "internalType": "uint160",
-                        "name": "secondsPerLiquidityCumulativeX128",
-                        "type": "uint160",
+                        "internalType": "uint256[]",
+                        "name": "rewardsOut",
+                        "type": "uint256[]",
                     },
-                    {"internalType": "bool", "name": "initialized", "type": "bool"},
                 ],
-                "stateMutability": "view",
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {
-                        "internalType": "uint32[]",
-                        "name": "secondsAgos",
-                        "type": "uint32[]",
-                    }
+                    {"internalType": "address", "name": "receiver", "type": "address"}
                 ],
-                "name": "observe",
+                "name": "redeemPY",
                 "outputs": [
                     {
-                        "internalType": "int56[]",
-                        "name": "tickCumulatives",
-                        "type": "int56[]",
-                    },
-                    {
-                        "internalType": "uint160[]",
-                        "name": "secondsPerLiquidityCumulativeX128s",
-                        "type": "uint160[]",
-                    },
+                        "internalType": "uint256",
+                        "name": "amountSyOut",
+                        "type": "uint256",
+                    }
                 ],
-                "stateMutability": "view",
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "bytes32", "name": "key", "type": "bytes32"}
-                ],
-                "name": "positions",
-                "outputs": [
-                    {"internalType": "uint128", "name": "liquidity", "type": "uint128"},
-                    {
-                        "internalType": "uint256",
-                        "name": "feeGrowthInside0LastX128",
-                        "type": "uint256",
-                    },
                     {
-                        "internalType": "uint256",
-                        "name": "feeGrowthInside1LastX128",
-                        "type": "uint256",
+                        "internalType": "address[]",
+                        "name": "receivers",
+                        "type": "address[]",
                     },
                     {
-                        "internalType": "uint128",
-                        "name": "tokensOwed0",
-                        "type": "uint128",
+                        "internalType": "uint256[]",
+                        "name": "amountPYToRedeems",
+                        "type": "uint256[]",
                     },
+                ],
+                "name": "redeemPYMulti",
+                "outputs": [
                     {
-                        "internalType": "uint128",
-                        "name": "tokensOwed1",
-                        "type": "uint128",
-                    },
+                        "internalType": "uint256[]",
+                        "name": "amountSyOuts",
+                        "type": "uint256[]",
+                    }
                 ],
-                "stateMutability": "view",
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "protocolFees",
+                "name": "rewardIndexesCurrent",
                 "outputs": [
-                    {"internalType": "uint128", "name": "token0", "type": "uint128"},
-                    {"internalType": "uint128", "name": "token1", "type": "uint128"},
+                    {"internalType": "uint256[]", "name": "", "type": "uint256[]"}
                 ],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
-                "inputs": [
-                    {"internalType": "uint8", "name": "feeProtocol0", "type": "uint8"},
-                    {"internalType": "uint8", "name": "feeProtocol1", "type": "uint8"},
-                ],
-                "name": "setFeeProtocol",
-                "outputs": [],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "slot0",
-                "outputs": [
-                    {
-                        "internalType": "uint160",
-                        "name": "sqrtPriceX96",
-                        "type": "uint160",
-                    },
-                    {"internalType": "int24", "name": "tick", "type": "int24"},
-                    {
-                        "internalType": "uint16",
-                        "name": "observationIndex",
-                        "type": "uint16",
-                    },
-                    {
-                        "internalType": "uint16",
-                        "name": "observationCardinality",
-                        "type": "uint16",
-                    },
-                    {
-                        "internalType": "uint16",
-                        "name": "observationCardinalityNext",
-                        "type": "uint16",
-                    },
-                    {"internalType": "uint8", "name": "feeProtocol", "type": "uint8"},
-                    {"internalType": "bool", "name": "unlocked", "type": "bool"},
-                ],
+                "name": "symbol",
+                "outputs": [{"internalType": "string", "name": "", "type": "string"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "int24", "name": "tickLower", "type": "int24"},
-                    {"internalType": "int24", "name": "tickUpper", "type": "int24"},
-                ],
-                "name": "snapshotCumulativesInside",
-                "outputs": [
-                    {
-                        "internalType": "int56",
-                        "name": "tickCumulativeInside",
-                        "type": "int56",
-                    },
-                    {
-                        "internalType": "uint160",
-                        "name": "secondsPerLiquidityInsideX128",
-                        "type": "uint160",
-                    },
-                    {
-                        "internalType": "uint32",
-                        "name": "secondsInside",
-                        "type": "uint32",
-                    },
-                ],
+                "inputs": [],
+                "name": "totalSupply",
+                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "recipient", "type": "address"},
-                    {"internalType": "bool", "name": "zeroForOne", "type": "bool"},
-                    {
-                        "internalType": "int256",
-                        "name": "amountSpecified",
-                        "type": "int256",
-                    },
-                    {
-                        "internalType": "uint160",
-                        "name": "sqrtPriceLimitX96",
-                        "type": "uint160",
-                    },
-                    {"internalType": "bytes", "name": "data", "type": "bytes"},
-                ],
-                "name": "swap",
-                "outputs": [
-                    {"internalType": "int256", "name": "amount0", "type": "int256"},
-                    {"internalType": "int256", "name": "amount1", "type": "int256"},
+                    {"internalType": "address", "name": "to", "type": "address"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
+                "name": "transfer",
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "int16", "name": "wordPosition", "type": "int16"}
+                    {"internalType": "address", "name": "from", "type": "address"},
+                    {"internalType": "address", "name": "to", "type": "address"},
+                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
-                "name": "tickBitmap",
-                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
-                "inputs": [],
-                "name": "tickSpacing",
-                "outputs": [{"internalType": "int24", "name": "", "type": "int24"}],
-                "stateMutability": "view",
+                "name": "transferFrom",
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
+                "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
-                "inputs": [{"internalType": "int24", "name": "tick", "type": "int24"}],
-                "name": "ticks",
+                "inputs": [
+                    {"internalType": "address", "name": "user", "type": "address"}
+                ],
+                "name": "userInterest",
                 "outputs": [
                     {
                         "internalType": "uint128",
-                        "name": "liquidityGross",
+                        "name": "lastPYIndex",
                         "type": "uint128",
                     },
                     {
-                        "internalType": "int128",
-                        "name": "liquidityNet",
-                        "type": "int128",
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "feeGrowthOutside0X128",
-                        "type": "uint256",
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "feeGrowthOutside1X128",
-                        "type": "uint256",
-                    },
-                    {
-                        "internalType": "int56",
-                        "name": "tickCumulativeOutside",
-                        "type": "int56",
-                    },
-                    {
-                        "internalType": "uint160",
-                        "name": "secondsPerLiquidityOutsideX128",
-                        "type": "uint160",
-                    },
-                    {
-                        "internalType": "uint32",
-                        "name": "secondsOutside",
-                        "type": "uint32",
+                        "internalType": "uint128",
+                        "name": "accruedInterest",
+                        "type": "uint128",
                     },
-                    {"internalType": "bool", "name": "initialized", "type": "bool"},
                 ],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [],
-                "name": "token0",
-                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
-                "inputs": [],
-                "name": "token1",
-                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "inputs": [
+                    {"internalType": "address", "name": "token", "type": "address"},
+                    {"internalType": "address", "name": "user", "type": "address"},
+                ],
+                "name": "userReward",
+                "outputs": [
+                    {"internalType": "uint128", "name": "index", "type": "uint128"},
+                    {"internalType": "uint128", "name": "accrued", "type": "uint128"},
+                ],
                 "stateMutability": "view",
                 "type": "function",
             },
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def burn(
-        self,
-        tick_lower: None,
-        tick_upper: None,
-        amount: None,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.burn(tick_lower, tick_upper, amount).build_transaction(
-            override_tx_parameters
-        )
-
-    def collect(
-        self,
-        recipient: str,
-        tick_lower: None,
-        tick_upper: None,
-        amount0_requested: None,
-        amount1_requested: None,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def p_t(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.collect(
-            recipient, tick_lower, tick_upper, amount0_requested, amount1_requested
-        ).build_transaction(override_tx_parameters)
+        return c.functions.PT().call()
 
-    def collect_protocol(
-        self,
-        recipient: str,
-        amount0_requested: None,
-        amount1_requested: None,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def s_y(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.collectProtocol(
-            recipient, amount0_requested, amount1_requested
-        ).build_transaction(override_tx_parameters)
+        return c.functions.SY().call()
 
-    def factory(self) -> str:
+    def allowance(self, owner: str, spender: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.factory().call()
+        return c.functions.allowance(owner, spender).call()
 
-    def fee(self) -> TxParams:
+    def approve(
+        self,
+        spender: str,
+        amount: int,
+        override_tx_parameters: Optional[TxParams] = None,
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.fee().build_transaction()
+        return c.functions.approve(spender, amount).build_transaction(
+            override_tx_parameters
+        )
 
-    def fee_growth_global0_x128(self) -> int:
+    def balance_of(self, account: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.feeGrowthGlobal0X128().call()
+        return c.functions.balanceOf(account).call()
 
-    def fee_growth_global1_x128(self) -> int:
+    def decimals(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.feeGrowthGlobal1X128().call()
+        return c.functions.decimals().call()
 
-    def flash(
-        self,
-        recipient: str,
-        amount0: int,
-        amount1: int,
-        data: bytes,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def do_cache_index_same_block(self) -> bool:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.flash(recipient, amount0, amount1, data).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.doCacheIndexSameBlock().call()
 
-    def increase_observation_cardinality_next(
-        self,
-        observation_cardinality_next: None,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def expiry(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.increaseObservationCardinalityNext(
-            observation_cardinality_next
-        ).build_transaction(override_tx_parameters)
+        return c.functions.expiry().call()
 
-    def initialize(
-        self, sqrt_price_x96: None, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
+    def factory(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.initialize(sqrt_price_x96).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.factory().call()
 
-    def liquidity(self) -> TxParams:
+    def get_reward_tokens(self) -> List[str]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.liquidity().build_transaction()
+        return c.functions.getRewardTokens().call()
 
-    def max_liquidity_per_tick(self) -> TxParams:
+    def is_expired(self) -> bool:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.maxLiquidityPerTick().build_transaction()
+        return c.functions.isExpired().call()
 
-    def mint(
+    def mint_p_y(
         self,
-        recipient: str,
-        tick_lower: None,
-        tick_upper: None,
-        amount: None,
-        data: bytes,
+        receiver_p_t: str,
+        receiver_y_t: str,
         override_tx_parameters: Optional[TxParams] = None,
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.mint(
-            recipient, tick_lower, tick_upper, amount, data
-        ).build_transaction(override_tx_parameters)
+        return c.functions.mintPY(receiver_p_t, receiver_y_t).build_transaction(
+            override_tx_parameters
+        )
 
-    def observations(self, index: int) -> TxParams:
+    def name(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.observations(index).build_transaction()
+        return c.functions.name().call()
 
-    def observe(self, seconds_agos: None) -> TxParams:
+    def py_index_current(
+        self, override_tx_parameters: Optional[TxParams] = None
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.observe(seconds_agos).build_transaction()
+        return c.functions.pyIndexCurrent().build_transaction(override_tx_parameters)
 
-    def positions(self, key: bytes) -> TxParams:
+    def py_index_stored(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.positions(key).build_transaction()
+        return c.functions.pyIndexStored().call()
 
-    def protocol_fees(self) -> TxParams:
+    def redeem_due_interest_and_rewards(
+        self,
+        user: str,
+        redeem_interest: bool,
+        redeem_rewards: bool,
+        override_tx_parameters: Optional[TxParams] = None,
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.protocolFees().build_transaction()
+        return c.functions.redeemDueInterestAndRewards(
+            user, redeem_interest, redeem_rewards
+        ).build_transaction(override_tx_parameters)
 
-    def set_fee_protocol(
-        self,
-        fee_protocol0: int,
-        fee_protocol1: int,
-        override_tx_parameters: Optional[TxParams] = None,
+    def redeem_p_y(
+        self, receiver: str, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.setFeeProtocol(
-            fee_protocol0, fee_protocol1
-        ).build_transaction(override_tx_parameters)
+        return c.functions.redeemPY(receiver).build_transaction(override_tx_parameters)
 
-    def slot0(self) -> TxParams:
+    def redeem_p_y_multi(
+        self,
+        receivers: List[str],
+        amount_p_y_to_redeems: List[int],
+        override_tx_parameters: Optional[TxParams] = None,
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.slot0().build_transaction()
+        return c.functions.redeemPYMulti(
+            receivers, amount_p_y_to_redeems
+        ).build_transaction(override_tx_parameters)
 
-    def snapshot_cumulatives_inside(
-        self, tick_lower: None, tick_upper: None
+    def reward_indexes_current(
+        self, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.snapshotCumulativesInside(
-            tick_lower, tick_upper
-        ).build_transaction()
+        return c.functions.rewardIndexesCurrent().build_transaction(
+            override_tx_parameters
+        )
 
-    def swap(
-        self,
-        recipient: str,
-        zero_for_one: bool,
-        amount_specified: None,
-        sqrt_price_limit_x96: None,
-        data: bytes,
-        override_tx_parameters: Optional[TxParams] = None,
-    ) -> TxParams:
+    def symbol(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.swap(
-            recipient, zero_for_one, amount_specified, sqrt_price_limit_x96, data
-        ).build_transaction(override_tx_parameters)
+        return c.functions.symbol().call()
 
-    def tick_bitmap(self, word_position: None) -> int:
+    def total_supply(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.tickBitmap(word_position).call()
+        return c.functions.totalSupply().call()
 
-    def tick_spacing(self) -> TxParams:
+    def transfer(
+        self, to: str, amount: int, override_tx_parameters: Optional[TxParams] = None
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.tickSpacing().build_transaction()
+        return c.functions.transfer(to, amount).build_transaction(
+            override_tx_parameters
+        )
 
-    def ticks(self, tick: None) -> TxParams:
+    def transfer_from(
+        self,
+        _from: str,
+        to: str,
+        amount: int,
+        override_tx_parameters: Optional[TxParams] = None,
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.ticks(tick).build_transaction()
+        return c.functions.transferFrom(_from, to, amount).build_transaction(
+            override_tx_parameters
+        )
 
-    def token0(self) -> str:
+    def user_interest(self, user: str) -> Tuple[int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.token0().call()
+        return c.functions.userInterest(user).call()
 
-    def token1(self) -> str:
+    def user_reward(self, token: str, user: str) -> Tuple[int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.token1().call()
+        return c.functions.userReward(token, user).call()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_diamond_loupe.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_diamond_loupe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
@@ -94,15 +94,15 @@
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def facet_address(self, _function_selector: None) -> str:
+    def facet_address(self, _function_selector: bytes) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.facetAddress(_function_selector).call()
@@ -112,15 +112,15 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.facetAddresses().call()
 
-    def facet_function_selectors(self, _facet: str) -> List[None]:
+    def facet_function_selectors(self, _facet: str) -> List[bytes]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.facetFunctionSelectors(_facet).call()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_e_r_c20_permit.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_e_r_c20_permit.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,26 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
+from .multi_approval import MultiApproval
+from .call3 import Call3
+
+
+def serialize_struct(d) -> tuple:
+    if isinstance(d, dict):
+        return tuple(serialize_struct(v) for v in d.values())
+    elif isinstance(d, (list, tuple)):
+        return tuple(serialize_struct(x) for x in d)
+    else:
+        return d
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
 class IERC20Permit:
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_action_add_remove_liq.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_action_add_remove_liq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
-from eulith_web3.contract_bindings.pendle.swap_data import SwapData
-from eulith_web3.contract_bindings.pendle.token_input import TokenInput
-from eulith_web3.contract_bindings.pendle.approx_params import ApproxParams
-from eulith_web3.contract_bindings.pendle.token_output import TokenOutput
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
 
 
 def serialize_struct(d) -> tuple:
     if isinstance(d, dict):
         return tuple(serialize_struct(v) for v in d.values())
     elif isinstance(d, (list, tuple)):
         return tuple(serialize_struct(x) for x in d)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_action_mint_redeem.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_action_mint_redeem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
-from eulith_web3.contract_bindings.pendle.swap_data import SwapData
-from eulith_web3.contract_bindings.pendle.token_input import TokenInput
-from eulith_web3.contract_bindings.pendle.approx_params import ApproxParams
-from eulith_web3.contract_bindings.pendle.token_output import TokenOutput
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
 
 
 def serialize_struct(d) -> tuple:
     if isinstance(d, dict):
         return tuple(serialize_struct(v) for v in d.values())
     elif isinstance(d, (list, tuple)):
         return tuple(serialize_struct(x) for x in d)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_action_misc.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_action_misc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
-from eulith_web3.contract_bindings.pendle.swap_data import SwapData
-from eulith_web3.contract_bindings.pendle.token_input import TokenInput
-from eulith_web3.contract_bindings.pendle.approx_params import ApproxParams
-from eulith_web3.contract_bindings.pendle.token_output import TokenOutput
-from eulith_web3.contract_bindings.pendle.multi_approval import MultiApproval
-from eulith_web3.contract_bindings.pendle.call3 import Call3
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
+from .multi_approval import MultiApproval
+from .call3 import Call3
 
 
 def serialize_struct(d) -> tuple:
     if isinstance(d, dict):
         return tuple(serialize_struct(v) for v in d.values())
     elif isinstance(d, (list, tuple)):
         return tuple(serialize_struct(x) for x in d)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_p_t.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_p_t.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
-from eulith_web3.contract_bindings.pendle.swap_data import SwapData
-from eulith_web3.contract_bindings.pendle.token_input import TokenInput
-from eulith_web3.contract_bindings.pendle.approx_params import ApproxParams
-from eulith_web3.contract_bindings.pendle.token_output import TokenOutput
-from eulith_web3.contract_bindings.pendle.multi_approval import MultiApproval
-from eulith_web3.contract_bindings.pendle.call3 import Call3
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
+from .multi_approval import MultiApproval
+from .call3 import Call3
 
 
 def serialize_struct(d) -> tuple:
     if isinstance(d, dict):
         return tuple(serialize_struct(v) for v in d.values())
     elif isinstance(d, (list, tuple)):
         return tuple(serialize_struct(x) for x in d)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_y_t.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_y_t.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
-from eulith_web3.contract_bindings.pendle.swap_data import SwapData
-from eulith_web3.contract_bindings.pendle.token_input import TokenInput
-from eulith_web3.contract_bindings.pendle.approx_params import ApproxParams
-from eulith_web3.contract_bindings.pendle.token_output import TokenOutput
-from eulith_web3.contract_bindings.pendle.multi_approval import MultiApproval
-from eulith_web3.contract_bindings.pendle.call3 import Call3
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
+from .multi_approval import MultiApproval
+from .call3 import Call3
 
 
 def serialize_struct(d) -> tuple:
     if isinstance(d, dict):
         return tuple(serialize_struct(v) for v in d.values())
     elif isinstance(d, (list, tuple)):
         return tuple(serialize_struct(x) for x in d)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_all_action.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_all_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
-from eulith_web3.contract_bindings.pendle.swap_data import SwapData
-from eulith_web3.contract_bindings.pendle.token_input import TokenInput
-from eulith_web3.contract_bindings.pendle.approx_params import ApproxParams
-from eulith_web3.contract_bindings.pendle.token_output import TokenOutput
-from eulith_web3.contract_bindings.pendle.multi_approval import MultiApproval
-from eulith_web3.contract_bindings.pendle.call3 import Call3
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
+from .multi_approval import MultiApproval
+from .call3 import Call3
 
 
 def serialize_struct(d) -> tuple:
     if isinstance(d, dict):
         return tuple(serialize_struct(v) for v in d.values())
     elif isinstance(d, (list, tuple)):
         return tuple(serialize_struct(x) for x in d)
@@ -3020,15 +3020,15 @@
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.batchExec(serialize_struct(calls)).build_transaction(
             override_tx_parameters
         )
 
-    def facet_address(self, _function_selector: None) -> str:
+    def facet_address(self, _function_selector: bytes) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.facetAddress(_function_selector).call()
@@ -3038,15 +3038,15 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.facetAddresses().call()
 
-    def facet_function_selectors(self, _facet: str) -> List[None]:
+    def facet_function_selectors(self, _facet: str) -> List[bytes]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.facetFunctionSelectors(_facet).call()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_gauge.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_reward_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,49 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class IPGauge:
+class IRewardManager:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
             {
                 "inputs": [
-                    {"internalType": "address", "name": "user", "type": "address"}
+                    {"internalType": "address", "name": "token", "type": "address"},
+                    {"internalType": "address", "name": "user", "type": "address"},
+                ],
+                "name": "userReward",
+                "outputs": [
+                    {"internalType": "uint128", "name": "index", "type": "uint128"},
+                    {"internalType": "uint128", "name": "accrued", "type": "uint128"},
                 ],
-                "name": "activeBalance",
-                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
-                "inputs": [],
-                "name": "totalActiveSupply",
-                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
-            },
+            }
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def active_balance(self, user: str) -> int:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.activeBalance(user).call()
-
-    def total_active_supply(self) -> int:
+    def user_reward(self, token: str, user: str) -> Tuple[int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.totalActiveSupply().call()
+        return c.functions.userReward(token, user).call()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_interest_manager_y_t.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_p_interest_manager_y_t.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,11 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
-from eulith_web3.contract_bindings.pendle.swap_data import SwapData
-from eulith_web3.contract_bindings.pendle.token_input import TokenInput
-from eulith_web3.contract_bindings.pendle.approx_params import ApproxParams
-from eulith_web3.contract_bindings.pendle.token_output import TokenOutput
-from eulith_web3.contract_bindings.pendle.multi_approval import MultiApproval
-from eulith_web3.contract_bindings.pendle.call3 import Call3
-
-
-def serialize_struct(d) -> tuple:
-    if isinstance(d, dict):
-        return tuple(serialize_struct(v) for v in d.values())
-    elif isinstance(d, (list, tuple)):
-        return tuple(serialize_struct(x) for x in d)
-    else:
-        return d
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
 class IPInterestManagerYT:
@@ -57,15 +42,15 @@
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def user_interest(self, user: str) -> (int, int):
+    def user_interest(self, user: str) -> Tuple[int, int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.userInterest(user).call()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/pendle/i_p_principal_token.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/pendle/i_standardized_yield.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Any, Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
-from eulith_web3.contract_bindings.pendle.swap_data import SwapData
-from eulith_web3.contract_bindings.pendle.token_input import TokenInput
-from eulith_web3.contract_bindings.pendle.approx_params import ApproxParams
-from eulith_web3.contract_bindings.pendle.token_output import TokenOutput
-from eulith_web3.contract_bindings.pendle.multi_approval import MultiApproval
-from eulith_web3.contract_bindings.pendle.call3 import Call3
+from .swap_data import SwapData
+from .token_input import TokenInput
+from .approx_params import ApproxParams
+from .token_output import TokenOutput
+from .multi_approval import MultiApproval
+from .call3 import Call3
 
 
 def serialize_struct(d) -> tuple:
     if isinstance(d, dict):
         return tuple(serialize_struct(v) for v in d.values())
     elif isinstance(d, (list, tuple)):
         return tuple(serialize_struct(x) for x in d)
@@ -19,15 +19,15 @@
         return d
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class IPPrincipalToken:
+class IStandardizedYield:
     def __init__(
         self,
         web3: Web3,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
     ):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
         self.abi = [
@@ -58,14 +58,113 @@
             },
             {
                 "anonymous": False,
                 "inputs": [
                     {
                         "indexed": True,
                         "internalType": "address",
+                        "name": "user",
+                        "type": "address",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "address[]",
+                        "name": "rewardTokens",
+                        "type": "address[]",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256[]",
+                        "name": "rewardAmounts",
+                        "type": "uint256[]",
+                    },
+                ],
+                "name": "ClaimRewards",
+                "type": "event",
+            },
+            {
+                "anonymous": False,
+                "inputs": [
+                    {
+                        "indexed": True,
+                        "internalType": "address",
+                        "name": "caller",
+                        "type": "address",
+                    },
+                    {
+                        "indexed": True,
+                        "internalType": "address",
+                        "name": "receiver",
+                        "type": "address",
+                    },
+                    {
+                        "indexed": True,
+                        "internalType": "address",
+                        "name": "tokenIn",
+                        "type": "address",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "amountDeposited",
+                        "type": "uint256",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "amountSyOut",
+                        "type": "uint256",
+                    },
+                ],
+                "name": "Deposit",
+                "type": "event",
+            },
+            {
+                "anonymous": False,
+                "inputs": [
+                    {
+                        "indexed": True,
+                        "internalType": "address",
+                        "name": "caller",
+                        "type": "address",
+                    },
+                    {
+                        "indexed": True,
+                        "internalType": "address",
+                        "name": "receiver",
+                        "type": "address",
+                    },
+                    {
+                        "indexed": True,
+                        "internalType": "address",
+                        "name": "tokenOut",
+                        "type": "address",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "amountSyToRedeem",
+                        "type": "uint256",
+                    },
+                    {
+                        "indexed": False,
+                        "internalType": "uint256",
+                        "name": "amountTokenOut",
+                        "type": "uint256",
+                    },
+                ],
+                "name": "Redeem",
+                "type": "event",
+            },
+            {
+                "anonymous": False,
+                "inputs": [
+                    {
+                        "indexed": True,
+                        "internalType": "address",
                         "name": "from",
                         "type": "address",
                     },
                     {
                         "indexed": True,
                         "internalType": "address",
                         "name": "to",
@@ -78,24 +177,25 @@
                         "type": "uint256",
                     },
                 ],
                 "name": "Transfer",
                 "type": "event",
             },
             {
-                "inputs": [],
-                "name": "SY",
-                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
-                "stateMutability": "view",
-                "type": "function",
-            },
-            {
-                "inputs": [],
-                "name": "YT",
-                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "inputs": [
+                    {"internalType": "address", "name": "user", "type": "address"}
+                ],
+                "name": "accruedRewards",
+                "outputs": [
+                    {
+                        "internalType": "uint256[]",
+                        "name": "rewardAmounts",
+                        "type": "uint256[]",
+                    }
+                ],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
                     {"internalType": "address", "name": "owner", "type": "address"},
                     {"internalType": "address", "name": "spender", "type": "address"},
@@ -112,87 +212,248 @@
                 ],
                 "name": "approve",
                 "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
+                "inputs": [],
+                "name": "assetInfo",
+                "outputs": [
+                    {
+                        "internalType": "enum IStandardizedYield.AssetType",
+                        "name": "assetType",
+                        "type": "uint8",
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "assetAddress",
+                        "type": "address",
+                    },
+                    {"internalType": "uint8", "name": "assetDecimals", "type": "uint8"},
+                ],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
                 "inputs": [
                     {"internalType": "address", "name": "account", "type": "address"}
                 ],
                 "name": "balanceOf",
                 "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "user", "type": "address"},
-                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
+                    {"internalType": "address", "name": "user", "type": "address"}
+                ],
+                "name": "claimRewards",
+                "outputs": [
+                    {
+                        "internalType": "uint256[]",
+                        "name": "rewardAmounts",
+                        "type": "uint256[]",
+                    }
                 ],
-                "name": "burnByYT",
-                "outputs": [],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
             {
                 "inputs": [],
                 "name": "decimals",
                 "outputs": [{"internalType": "uint8", "name": "", "type": "uint8"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
+                "inputs": [
+                    {"internalType": "address", "name": "receiver", "type": "address"},
+                    {"internalType": "address", "name": "tokenIn", "type": "address"},
+                    {
+                        "internalType": "uint256",
+                        "name": "amountTokenToDeposit",
+                        "type": "uint256",
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "minSharesOut",
+                        "type": "uint256",
+                    },
+                ],
+                "name": "deposit",
+                "outputs": [
+                    {
+                        "internalType": "uint256",
+                        "name": "amountSharesOut",
+                        "type": "uint256",
+                    }
+                ],
+                "stateMutability": "payable",
+                "type": "function",
+            },
+            {
                 "inputs": [],
-                "name": "expiry",
-                "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}],
+                "name": "exchangeRate",
+                "outputs": [
+                    {"internalType": "uint256", "name": "res", "type": "uint256"}
+                ],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "factory",
-                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "name": "getRewardTokens",
+                "outputs": [
+                    {"internalType": "address[]", "name": "", "type": "address[]"}
+                ],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
-                "inputs": [
-                    {"internalType": "address", "name": "_YT", "type": "address"}
+                "inputs": [],
+                "name": "getTokensIn",
+                "outputs": [
+                    {"internalType": "address[]", "name": "res", "type": "address[]"}
                 ],
-                "name": "initialize",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [],
-                "name": "isExpired",
+                "name": "getTokensOut",
+                "outputs": [
+                    {"internalType": "address[]", "name": "res", "type": "address[]"}
+                ],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [
+                    {"internalType": "address", "name": "token", "type": "address"}
+                ],
+                "name": "isValidTokenIn",
                 "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [
-                    {"internalType": "address", "name": "user", "type": "address"},
-                    {"internalType": "uint256", "name": "amount", "type": "uint256"},
+                    {"internalType": "address", "name": "token", "type": "address"}
                 ],
-                "name": "mintByYT",
-                "outputs": [],
-                "stateMutability": "nonpayable",
+                "name": "isValidTokenOut",
+                "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
+                "stateMutability": "view",
                 "type": "function",
             },
             {
                 "inputs": [],
                 "name": "name",
                 "outputs": [{"internalType": "string", "name": "", "type": "string"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
+                "inputs": [
+                    {"internalType": "address", "name": "tokenIn", "type": "address"},
+                    {
+                        "internalType": "uint256",
+                        "name": "amountTokenToDeposit",
+                        "type": "uint256",
+                    },
+                ],
+                "name": "previewDeposit",
+                "outputs": [
+                    {
+                        "internalType": "uint256",
+                        "name": "amountSharesOut",
+                        "type": "uint256",
+                    }
+                ],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [
+                    {"internalType": "address", "name": "tokenOut", "type": "address"},
+                    {
+                        "internalType": "uint256",
+                        "name": "amountSharesToRedeem",
+                        "type": "uint256",
+                    },
+                ],
+                "name": "previewRedeem",
+                "outputs": [
+                    {
+                        "internalType": "uint256",
+                        "name": "amountTokenOut",
+                        "type": "uint256",
+                    }
+                ],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
+                "inputs": [
+                    {"internalType": "address", "name": "receiver", "type": "address"},
+                    {
+                        "internalType": "uint256",
+                        "name": "amountSharesToRedeem",
+                        "type": "uint256",
+                    },
+                    {"internalType": "address", "name": "tokenOut", "type": "address"},
+                    {
+                        "internalType": "uint256",
+                        "name": "minTokenOut",
+                        "type": "uint256",
+                    },
+                    {
+                        "internalType": "bool",
+                        "name": "burnFromInternalBalance",
+                        "type": "bool",
+                    },
+                ],
+                "name": "redeem",
+                "outputs": [
+                    {
+                        "internalType": "uint256",
+                        "name": "amountTokenOut",
+                        "type": "uint256",
+                    }
+                ],
+                "stateMutability": "nonpayable",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "rewardIndexesCurrent",
+                "outputs": [
+                    {
+                        "internalType": "uint256[]",
+                        "name": "indexes",
+                        "type": "uint256[]",
+                    }
+                ],
+                "stateMutability": "nonpayable",
+                "type": "function",
+            },
+            {
+                "inputs": [],
+                "name": "rewardIndexesStored",
+                "outputs": [
+                    {
+                        "internalType": "uint256[]",
+                        "name": "indexes",
+                        "type": "uint256[]",
+                    }
+                ],
+                "stateMutability": "view",
+                "type": "function",
+            },
+            {
                 "inputs": [],
                 "name": "symbol",
                 "outputs": [{"internalType": "string", "name": "", "type": "string"}],
                 "stateMutability": "view",
                 "type": "function",
             },
             {
@@ -219,41 +480,39 @@
                     {"internalType": "uint256", "name": "amount", "type": "uint256"},
                 ],
                 "name": "transferFrom",
                 "outputs": [{"internalType": "bool", "name": "", "type": "bool"}],
                 "stateMutability": "nonpayable",
                 "type": "function",
             },
+            {
+                "inputs": [],
+                "name": "yieldToken",
+                "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+                "stateMutability": "view",
+                "type": "function",
+            },
         ]
         self.bytecode = ""
         self.w3 = web3
 
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
         self.address = tx_receipt.contractAddress
 
-    def s_y(self) -> str:
-        if not self.address:
-            raise ContractAddressNotSet(
-                "you must either deploy or initialize the contract with an address"
-            )
-        c = self.w3.eth.contract(address=self.address, abi=self.abi)
-
-        return c.functions.SY().call()
-
-    def y_t(self) -> str:
+    def accrued_rewards(self, user: str) -> List[int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.YT().call()
+        return c.functions.accruedRewards(user).call()
 
     def allowance(self, owner: str, spender: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
@@ -272,104 +531,195 @@
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.approve(spender, amount).build_transaction(
             override_tx_parameters
         )
 
+    def asset_info(self) -> Tuple[int, str, int]:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.assetInfo().call()
+
     def balance_of(self, account: str) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.balanceOf(account).call()
 
-    def burn_by_y_t(
-        self, user: str, amount: int, override_tx_parameters: Optional[TxParams] = None
+    def claim_rewards(
+        self, user: str, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.burnByYT(user, amount).build_transaction(
-            override_tx_parameters
-        )
+        return c.functions.claimRewards(user).build_transaction(override_tx_parameters)
 
     def decimals(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.decimals().call()
 
-    def expiry(self) -> int:
+    def deposit(
+        self,
+        receiver: str,
+        token_in: str,
+        amount_token_to_deposit: int,
+        min_shares_out: int,
+        override_tx_parameters: Optional[TxParams] = None,
+    ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.expiry().call()
+        return c.functions.deposit(
+            receiver, token_in, amount_token_to_deposit, min_shares_out
+        ).build_transaction(override_tx_parameters)
 
-    def factory(self) -> str:
+    def exchange_rate(self) -> int:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.factory().call()
+        return c.functions.exchangeRate().call()
 
-    def initialize(
-        self, __y_t: str, override_tx_parameters: Optional[TxParams] = None
-    ) -> TxParams:
+    def get_reward_tokens(self) -> List[str]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.initialize(__y_t).build_transaction(override_tx_parameters)
+        return c.functions.getRewardTokens().call()
 
-    def is_expired(self) -> bool:
+    def get_tokens_in(self) -> List[str]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.isExpired().call()
+        return c.functions.getTokensIn().call()
 
-    def mint_by_y_t(
-        self, user: str, amount: int, override_tx_parameters: Optional[TxParams] = None
+    def get_tokens_out(self) -> List[str]:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.getTokensOut().call()
+
+    def is_valid_token_in(self, token: str) -> bool:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.isValidTokenIn(token).call()
+
+    def is_valid_token_out(self, token: str) -> bool:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.isValidTokenOut(token).call()
+
+    def name(self) -> str:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.name().call()
+
+    def preview_deposit(self, token_in: str, amount_token_to_deposit: int) -> int:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.previewDeposit(token_in, amount_token_to_deposit).call()
+
+    def preview_redeem(self, token_out: str, amount_shares_to_redeem: int) -> int:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.previewRedeem(token_out, amount_shares_to_redeem).call()
+
+    def redeem(
+        self,
+        receiver: str,
+        amount_shares_to_redeem: int,
+        token_out: str,
+        min_token_out: int,
+        burn_from_internal_balance: bool,
+        override_tx_parameters: Optional[TxParams] = None,
+    ) -> TxParams:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.redeem(
+            receiver,
+            amount_shares_to_redeem,
+            token_out,
+            min_token_out,
+            burn_from_internal_balance,
+        ).build_transaction(override_tx_parameters)
+
+    def reward_indexes_current(
+        self, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.mintByYT(user, amount).build_transaction(
+        return c.functions.rewardIndexesCurrent().build_transaction(
             override_tx_parameters
         )
 
-    def name(self) -> str:
+    def reward_indexes_stored(self) -> List[int]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
-        return c.functions.name().call()
+        return c.functions.rewardIndexesStored().call()
 
     def symbol(self) -> str:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
@@ -410,7 +760,16 @@
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.transferFrom(_from, to, amount).build_transaction(
             override_tx_parameters
         )
+
+    def yield_token(self) -> str:
+        if not self.address:
+            raise ContractAddressNotSet(
+                "you must either deploy or initialize the contract with an address"
+            )
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+
+        return c.functions.yieldToken().call()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/contract_bindings/safe/i_safe.py` & `eulith_web3-0.27.0/src/eulith_web3/contract_bindings/safe/i_safe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union, List, TypedDict
+from typing import Optional, Union, List, Tuple, TypedDict
 from eth_typing import Address, ChecksumAddress
 from web3 import Web3
 from web3.types import TxParams
 
 
 class ContractAddressNotSet(Exception):
     pass
@@ -905,15 +905,17 @@
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getChainId().call()
 
-    def get_modules_paginated(self, start: str, page_size: int) -> (List[str], str):
+    def get_modules_paginated(
+        self, start: str, page_size: int
+    ) -> Tuple[List[str], str]:
         if not self.address:
             raise ContractAddressNotSet(
                 "you must either deploy or initialize the contract with an address"
             )
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
 
         return c.functions.getModulesPaginated(start, page_size).call()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/curve.py` & `eulith_web3-0.27.0/src/eulith_web3/curve.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import List
+from typing import Any, List
 
 import web3.exceptions
 
 from eulith_web3.erc20 import EulithERC20, TokenSymbol
+from eulith_web3.eulith_web3 import EulithWeb3
 from eulith_web3.swap import EulithSwapRequest
 
 
 class CurveUtils:
-    def __init__(self, eulith_web3, curve_pool):
+    def __init__(self, eulith_web3: EulithWeb3, curve_pool: Any) -> None:
         self.w3 = eulith_web3
         self.curve_pool = curve_pool
         self.tokens = self.get_pool_tokens()
 
     def get_pool_tokens(self) -> List[EulithERC20]:
         tokens = []
         for i in range(0, 3):
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/dydx/v3/_core.py` & `eulith_web3-0.27.0/src/eulith_web3/dydx/v3/_core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,80 @@
+from typing import List
+
 from eth_account.messages import encode_typed_data
 from eth_utils import keccak
 
 from eulith_web3.dydx.v3._eip712 import DydxV3CreateOrderHashInput
+from eulith_web3.eip712_types import Eip712Data, Eip712Domain, Eip712Field
 
 
-def eip712_domain() -> dict:
-    return {"name": "EulithAceDydxV3", "version": "1"}
+def eip712_domain() -> Eip712Domain:
+    return Eip712Domain(name="EulithAceDydxV3", version="1")
 
 
-def eip712_domain_type() -> list:
+def eip712_domain_type() -> List[Eip712Field]:
     return [
-        {"name": "name", "type": "string"},
-        {"name": "version", "type": "string"},
+        Eip712Field(name="name", type="string"),
+        Eip712Field(name="version", type="string"),
     ]
 
 
 class CreateOrderHashInputEip712:
     x: DydxV3CreateOrderHashInput
 
     def __init__(self, x: DydxV3CreateOrderHashInput) -> None:
         self.x = x
 
     @classmethod
-    def eip712_type(cls) -> list:
+    def eip712_type(cls) -> List[Eip712Field]:
         return [
-            {"name": "market", "type": "string"},
-            {"name": "side", "type": "string"},
-            {"name": "orderType", "type": "string"},
-            {"name": "postOnly", "type": "bool"},
-            {"name": "reduceOnly", "type": "bool"},
-            {"name": "size", "type": "string"},
-            {"name": "price", "type": "string"},
-            {"name": "limitFee", "type": "string"},
-            {"name": "expiration", "type": "string"},
-            {"name": "timeInForce", "type": "string"},
-            {"name": "triggerPrice", "type": "string"},
-            {"name": "trailingPercent", "type": "string"},
-            {"name": "accountName", "type": "string"},
+            Eip712Field(name="market", type="string"),
+            Eip712Field(name="side", type="string"),
+            Eip712Field(name="orderType", type="string"),
+            Eip712Field(name="postOnly", type="bool"),
+            Eip712Field(name="reduceOnly", type="bool"),
+            Eip712Field(name="size", type="string"),
+            Eip712Field(name="price", type="string"),
+            Eip712Field(name="limitFee", type="string"),
+            Eip712Field(name="expiration", type="string"),
+            Eip712Field(name="timeInForce", type="string"),
+            Eip712Field(name="triggerPrice", type="string"),
+            Eip712Field(name="trailingPercent", type="string"),
+            Eip712Field(name="accountName", type="string"),
         ]
 
     @classmethod
     def eip712_type_name(cls) -> str:
         return "DydxV3CreateOrderHashInput"
 
-    def typed_data(self) -> dict:
+    def typed_data(self) -> Eip712Data:
         types = {
             "EIP712Domain": eip712_domain_type(),
             self.eip712_type_name(): self.eip712_type(),
         }
 
-        payload = {
-            "types": types,
-            "primaryType": self.eip712_type_name(),
-            "domain": eip712_domain(),
-            "message": {
+        payload = Eip712Data(
+            types=types,
+            primaryType=self.eip712_type_name(),
+            domain=eip712_domain(),
+            message={
                 "market": self.x["market"],
                 "side": self.x["side"],
                 "orderType": self.x["order_type"],
                 "postOnly": self.x["post_only"],
                 "reduceOnly": self.x["reduce_only"],
                 "size": self.x["size"],
                 "price": self.x["price"],
                 "limitFee": self.x["limit_fee"],
                 "expiration": self.x["expiration"],
                 "timeInForce": self.x["time_in_force"],
                 "triggerPrice": self.x["trigger_price"],
                 "trailingPercent": self.x["trailing_percent"],
                 "accountName": self.x["account_name"],
             },
-        }
+        )
 
         return payload
 
     def compute_hash(self) -> bytes:
-        signable_message = encode_typed_data(full_message=self.typed_data())
+        signable_message = encode_typed_data(full_message=dict(self.typed_data()))
         return keccak(b"\x19\x01" + signable_message.header + signable_message.body)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/dydx/v3/_eip712.py` & `eulith_web3-0.27.0/src/eulith_web3/dydx/v3/_eip712.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/dydx/v3/rpc.py` & `eulith_web3-0.27.0/src/eulith_web3/dydx/v3/rpc.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/dydx/v3/v3.py` & `eulith_web3-0.27.0/src/eulith_web3/dydx/v3/v3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from typing import List
-
-from eth_account._utils.signing import to_eth_v
+from typing import Any, List, cast
 
 from eulith_web3.dydx.v3._core import CreateOrderHashInputEip712
 from eulith_web3.dydx.v3._eip712 import parse_request_to_hash_input
 from eulith_web3.dydx.v3.rpc import (
     DydxV3AceManagedAccount,
     DyDxV3CreateOrderParams,
     DydxV3CreateOrderResponse,
@@ -18,69 +16,57 @@
 class DyDxV3:
     def __init__(self, eulith_service: EulithService):
         self.eulith_service = eulith_service
 
     def get_ace_managed_accounts(
         self, ace_address: str
     ) -> List[DydxV3AceManagedAccount]:
-        response, error = self.eulith_service.dydx_v3_get_ace_managed_accounts(
-            ace_address
-        )
-        if error:
-            raise EulithRpcException(error)
-        return response
+        return self.eulith_service.dydx_v3_get_ace_managed_accounts(ace_address)
 
-    def get_positions(self, ace_address: str, dydx_account_name: str) -> List:
+    def get_positions(self, ace_address: str, dydx_account_name: str) -> List[Any]:
         """
         :param ace_address: the ETH signing address associated with your ACE
         :param dydx_account_name: the DyDx account name you configured on your ACE
         :return: List of current positions held by the requested DyDx account
         """
-        response, error = self.eulith_service.dydx_v3_get_for_account(
+        response = self.eulith_service.dydx_v3_get_for_account(
             ace_address, dydx_account_name, "positions"
         )
-        if error:
-            raise EulithRpcException(error)
-        return response.get("positions")
+        return response["positions"]
 
-    def get_orders(self, ace_address: str, dydx_account_name: str) -> List:
+    def get_orders(self, ace_address: str, dydx_account_name: str) -> List[Any]:
         """
         :param ace_address: the ETH signing address associated with your ACE
         :param dydx_account_name: the DyDx account name you configured on your ACE
         :return: List of current orders held by the requested DyDx account
         """
-        response, error = self.eulith_service.dydx_v3_get_for_account(
+        response = self.eulith_service.dydx_v3_get_for_account(
             ace_address, dydx_account_name, "orders"
         )
-        if error:
-            raise EulithRpcException(error)
-        return response.get("orders")
+        return response["orders"]
 
-    def get_transfers(self, ace_address: str, dydx_account_name: str) -> List:
+    def get_transfers(self, ace_address: str, dydx_account_name: str) -> List[Any]:
         """
         :param ace_address: the ETH signing address associated with your ACE
         :param dydx_account_name: the DyDx account name you configured on your ACE
         :return: List of current transfers pending in the requested DyDx account
         """
-        response, error = self.eulith_service.dydx_v3_get_for_account(
+        response = self.eulith_service.dydx_v3_get_for_account(
             ace_address, dydx_account_name, "transfers"
         )
-        if error:
-            raise EulithRpcException(error)
-        return response.get("transfers")
+        return response["transfers"]
 
     def create_order(
         self, order: DyDxV3CreateOrderParams, ace_address: str, ace_signer: Signer
     ) -> DydxV3CreateOrderResponse:
         hash_input = parse_request_to_hash_input(order)
         hash_me = CreateOrderHashInputEip712(hash_input)
         hash_to_sign = hash_me.compute_hash()
         signature = ace_signer.sign_msg_hash(hash_to_sign)
         signature_string = normalize_signature(signature)
 
-        response, error = self.eulith_service.dydx_v3_create_order(
-            order, signature_string, ace_address
+        return cast(
+            DydxV3CreateOrderResponse,
+            self.eulith_service.dydx_v3_create_order(
+                order, signature_string, ace_address
+            ),
         )
-        if error:
-            raise EulithRpcException(error)
-
-        return response
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/erc20.py` & `eulith_web3-0.27.0/src/eulith_web3/erc20.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Union, Optional
+from typing import Any, Union, Optional
 
 from eth_typing import ChecksumAddress, Address
 from web3.types import TxParams, Wei
 
 from eulith_web3.contract_bindings.i_e_r_c_detailed import IERCDetailed
 from eulith_web3.contract_bindings.w_e_t_h_interface import WETHInterface
 
@@ -49,15 +49,15 @@
     WOO = "WOO"
     COMP = "COMP"
 
 
 class EulithERC20(IERCDetailed):
     def __init__(
         self,
-        eulith_web3,
+        eulith_web3: Any,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
         decimals: Optional[int] = None,
         symbol: Optional[str] = None,
     ):
         super().__init__(eulith_web3, contract_address)
         self._decimals = decimals
         self._symbol = symbol
@@ -120,26 +120,26 @@
         return self._symbol if self._symbol is not None else super().symbol()
 
 
 # WETH is special because you can deposit native ETH to the contract to get WETH back
 class EulithWETH(WETHInterface, EulithERC20):
     def __init__(
         self,
-        eulith_web3,
+        eulith_web3: Any,
         contract_address: Optional[Union[Address, ChecksumAddress]] = None,
-    ):
+    ) -> None:
         super().__init__(eulith_web3, contract_address)
         self._decimals = 18
         self._symbol = "WETH"
 
     def deposit_eth(
         self,
         whole_eth_as_float: float,
         override_tx_parameters: Optional[TxParams] = None,
-    ):
+    ) -> TxParams:
         wei = int(whole_eth_as_float * 1e18)  # convert to wei
         return self.deposit_wei(wei, override_tx_parameters)
 
     def deposit_wei(
         self, wei: int, override_tx_parameters: Optional[TxParams] = None
     ) -> TxParams:
         tx = self.deposit(override_tx_parameters)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/eulith_service.py` & `eulith_web3-0.27.0/src/eulith_web3/eulith_web3.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1378 +1,1268 @@
-import urllib.parse
-import uuid
-from typing import cast, Optional, List, Dict, Union
+import time
+from typing import Union, Any, cast, Callable, Dict, Optional, List, Tuple
+from warnings import warn
 
-import requests
-from eth_keys.datatypes import Signature
+import web3.middleware
+from eth_account.messages import encode_typed_data
 from eth_typing import URI, ChecksumAddress, HexStr
-from web3.types import RPCResponse, RPCEndpoint, TxParams
-
-from eulith_web3.gmx.v2.rpc import (
-    GmxV2CreateOrderRequest,
-    GmxV2CreateOrderResponse,
-    GmxV2GetPositionsRequest,
-    GmxV2GetPositionsResponse,
+from eth_utils import is_hex_address, keccak
+from hexbytes import HexBytes
+from web3 import Web3
+from web3.types import Nonce, RPCEndpoint, RPCResponse, TxParams, TxReceipt
+
+from eulith_web3.hyperliquid.hyperliquid import HyperliquidClient
+from eulith_web3 import atomic, whitelists_v2
+from eulith_web3.ace import (
+    get_ace_immediate_tx_typed_data,
+    get_ace_immediate_tx_hash,
+    AcePingResponse,
 )
-
-from eulith_web3.gmx.v2.rpc import (
-    GmxV2GetMarketPoolDataRequest,
-    GmxV2GetMarketPoolDataResponse,
-    GmxV2CreateDepositRequest,
-    GmxV2CreateDepositResponse,
+from eulith_web3.common import INT_FEE_TO_FLOAT_DIVISOR, ETHEREUM_STATUS_SUCCESS
+from eulith_web3.contract_bindings.safe.i_safe import ISafe
+from eulith_web3.dydx.dydx import DyDx
+from eulith_web3.erc20 import TokenSymbol, EulithWETH, EulithERC20
+from eulith_web3.eulith_service import EulithService
+from eulith_web3.exceptions import EulithDeprecationException, EulithRpcException
+from eulith_web3.gmx.gmx import GMXClient
+from eulith_web3.lightsim import (
+    LightSimulationProposal,
+    LightSimulationHashInput,
+    LightSimulationSubmitResponse,
 )
-
-from eulith_web3.hyperliquid.rpc import HyperliquidGetDataRequest
-
-from eulith_web3.hyperliquid._eip712 import HyperliquidCreateOrderHashInput
-from eulith_web3 import whitelists_v2
-from eulith_web3.ace import AceImmediateTx, AcePingResponse
-from eulith_web3.atomic import BundleRequest
-from eulith_web3.dydx.v3.rpc import DydxV3AceManagedAccount, DyDxV3CreateOrderParams
-from eulith_web3.erc20 import EulithERC20, TokenSymbol
-from eulith_web3.exceptions import EulithRpcException
-from eulith_web3.pendle import PendleMarketSymbol
 from eulith_web3.requests import (
     EulithShortOnRequest,
     EulithShortOffRequest,
     EulithAaveV2StartLoanRequest,
+    FlashRequest,
 )
-from eulith_web3.response import raise_if_error
-from eulith_web3.swap import (
-    EulithSwapRequest,
-    EulithSwapProvider,
-    EulithLiquiditySource,
-)
+from eulith_web3.response import raise_if_error, check_tx_receipt
+from eulith_web3.safe_utils.transaction_data import get_enable_module_typed_data
+from eulith_web3.signer import Signer
+from eulith_web3.signing import EulithSigningMiddleware, normalize_signature
+from eulith_web3.swap import EulithSwapRequest
 from eulith_web3.uniswap import (
+    EulithUniswapV3Pool,
     EulithUniV3StartLoanRequest,
     EulithUniV3StartSwapRequest,
     EulithUniV3SwapQuoteRequest,
     EulithUniswapPoolLookupRequest,
+    UniswapPoolFee,
 )
-from eulith_web3.websocket import (
-    EulithWebsocketProvider,
-    SubscribeRequest,
-    EulithWebsocketRequestHandler,
-    SubscriptionHandle,
-)
-from eulith_web3.whitelists import AcceptedEnableArmorSignature
+from eulith_web3.websocket import EulithWebsocketRequestHandler, SubscribeRequest
+from eulith_web3.whitelists import CurrentWhitelists, AcceptedEnableArmorSignature
+from eulith_web3.whitelists_v2 import ActivateHashInputEip712
 
 
-def ensure_formatted_ws_url(eulith_url: str) -> str:
-    if eulith_url.startswith("http://"):
-        return "ws" + eulith_url[4:]
-    elif eulith_url.startswith("https://"):
-        return "wss" + eulith_url[5:]
-    return eulith_url
-
+class EulithWeb3(Web3):
+    """
+    The main drop-in replacement for Web3.py for users of Eulith
 
-def get_headers(token: str) -> Dict:
+    :ivar eulith_service: internal methods to help with Eulith functionality
+    :ivar middleware_onion: web3py middleware
+    :ivar v0: versioned namespace for Eulith interactions
     """
-    Function returns a dictionary of headers to be used in an HTTP request.
 
-    :param token: The bearer token to be included in the Authorization header.
-    :type token: str
+    def __init__(
+        self,
+        eulith_url: Union[URI, str],
+        eulith_token: str,
+        signing_middle_ware: Optional[EulithSigningMiddleware] = None,
+        private: bool = False,
+        **kwargs: Any,
+    ) -> None:
+        """
+        :param eulith_url: The Eulith endpoint; different endpoints will point this library to different chains.
+        :param eulith_token: The refresh token used to authenticate the Eulith API
+        :param signing_middle_ware: The signing middleware used to sign transactions.
+        :param private: Flag that indicates whether transactions are routed through a private mempool
+        :param kwargs: Varying number of keyword or named arguments that should be passed to the `Web3` class.
+        """
 
-    :return: A dictionary of headers to be used in an HTTP request.
-    :rtype: Dict
+        auth_address = signing_middle_ware.address if signing_middle_ware else None
 
-    Example:
-        get_headers("https://www.exampletokenwebsite.com", "token123")
-    Returns: {
-        'Authorization': 'Bearer token123',
-        'Content-Type': 'application/json'
-    }
-    """
+        self.eulith_service = EulithService(
+            eulith_url, eulith_token, private, auth_address
+        )
+        kwargs.update({"provider": self.eulith_service.eulith_provider})
+        super().__init__(**kwargs)
 
-    headers = {"Authorization": "Bearer " + token, "Content-Type": "application/json"}
+        self.wallet_address = None
+        try:
+            self.chain_id = self.eth.chain_id
+        except Exception:
+            self.chain_id = 0
 
-    return headers
+        if signing_middle_ware:
+            self.wallet_address = signing_middle_ware.address
+            self.signer = signing_middle_ware.signer
+            self.middleware_onion.add(signing_middle_ware.middleware)
 
+        self.middleware_onion.add(eulith_atomic_middleware)
+        self.middleware_onion.add(web3.middleware.request_parameter_normalizer)
+        self.middleware_onion.add(
+            web3.middleware.pythonic_middleware, "eulith_pythonic"
+        )
+        self.v0 = v0(self)
+        self.dydx = DyDx(self.eulith_service)
+        self.gmx = GMXClient(self)
+        self.hyperliquid = HyperliquidClient(self)
 
-def add_params_to_url(url: str, params) -> str:
-    """
-    This function takes in a URL and a dictionary of parameters and adds the parameters to the URL as query parameters.
-    Eulith relies on query params to specify your atomic tx id or gnosis safe address, for example.
+        # Config for `wait_for_transaction_receipt_with_confirmations`
+        self.default_confirmations = 3
+        self._cached_confirmations_timeout_secs: Optional[float] = None
 
-    :param url: The URL to which the parameters will be added.
-    :type url: str
-    :param params: The dictionary of parameters that will be added to the URL.
-    :type params: Dict
-
-    :return: The URL with the added parameters as query parameters.
-    :rtype: str
-
-    Example:
-        add_params_to_url("https://www.example.com", {"param1": "value1", "param2": "value2"})
-        Returns: "https://www.example.com?param1=value1&param2=value2"
-    """
+    def terminate(self) -> None:
+        self.eulith_service.terminate()
 
-    url_parts = urllib.parse.urlparse(url)
-    query = dict(urllib.parse.parse_qsl(url_parts.query))
-    query.update(params)
-
-    return url_parts._replace(query=urllib.parse.urlencode(query)).geturl()
-
-
-class AtomicTxParams:
-    def __init__(self, tx_id: str, safe_address: str, trading_key: str):
-        self.tx_id = tx_id
-        self.safe_address = safe_address
-        self.trading_key = trading_key
-
-    def inject_in_body(self, post_body: Dict):
-        post_body.update({"auth_address": self.trading_key})
-
-        if self.tx_id:
-            post_body.update(
-                {
-                    "atomic_tx_id": self.tx_id,
-                }
-            )
+    def __enter__(self) -> "EulithWeb3":
+        return self
 
-        if self.safe_address:
-            post_body.update({"gnosis_address": self.safe_address})
+    def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
+        self.terminate()
 
+    def is_atomic(self) -> bool:
+        return self.eulith_service.is_atomic()
 
-class EulithService:
-    """
-    Embedded class to represent data of the Eulith API and provides methods to interact with the API.
+    def _eulith_send_atomic(self, params: Any) -> RPCResponse:
+        """
+        This function is used to send an atomic transaction.
 
-    :ivar eulith_url: URL of the Eulith API
-    :type eulith_url: URI
-    :ivar eulith_token: Refresh token for the Eulith API
-    :type eulith_token: str
-    :ivar private: bool switches on whether transactions are routed through a private mempool or not
-    :type private: bool
-    :ivar atomic: Boolean indicating if the current transaction is atomic
-    :type atomic: bool
-    :ivar tx_id: ID of the current transaction
-    :type tx_id: str
-    :ivar eulith_provider: HTTP provider instance to make requests to the Eulith API
-    :type eulith_provider: WebsocketProviderV2
-    """
+        :param params: A dictionary that contains the parameters required for the transaction.
+        """
+        return self.eulith_service.send_transaction(params)
 
-    def __init__(
-        self,
-        eulith_url: str,
-        eulith_token: str,
-        private: bool = False,
-        auth_address: Optional[str] = None,
-    ) -> None:
+    def eulith_start_transaction(self, account: str, gnosis: str = "") -> None:
         """
-        :param eulith_url: URL of the Eulith API
-        :type eulith_url: Union[URI, str]
-        :param eulith_token: Refresh token for the Eulith API
-        :type eulith_token: str
+        Begins an atomic transaction with your wallet as the authorized address,
+        or optionally with your gnosis safe as msg.sender
+
+        :param account: Your ETH wallet address
+        :param gnosis: Optional. Gnosis Safe address.
         """
 
-        self.token = eulith_token
+        if not is_hex_address(account):
+            raise TypeError("account must be a hex-formatted address")
+        if len(gnosis) > 0 and not is_hex_address(gnosis):
+            raise TypeError("gnosis must either be blank or a hex-formatted address")
+        self.eulith_service.start_transaction(account, gnosis)
 
-        url_params = {}
+    def eulith_commit_transaction(self) -> TxParams:
+        """
+        Serializes your pending atomic unit into a single transaction and returns the params to be signed
 
-        if private:
-            url_params["private"] = "true"
+        :returns: The parameters of the committed transaction.
+        """
 
-        if auth_address:
-            url_params["auth_address"] = auth_address
+        return self.eulith_service.commit()
 
-        self.eulith_url = URI(
-            add_params_to_url(ensure_formatted_ws_url(eulith_url), url_params)
-        )
+    def eulith_rollback_transaction(self) -> None:
+        """
+        Rollback a transaction, discard the current atomic transaction
+        """
 
-        self.atomic_params: Optional[AtomicTxParams] = None
-        self.headers = get_headers(self.token)
+        self.eulith_service.rollback()
 
-        self.eulith_provider = EulithWebsocketProvider(
-            uri=self.eulith_url, bearer_token=self.token
-        )
+    def eulith_contract_address(self, account: str) -> str:
+        """
+        Retrieve the toolkit contract address bearing a one-to-one relationship to the `account` address.
+        One toolkit contract is generated per wallet address.
 
-    def is_atomic(self):
-        if not self.atomic_params:
-            return False
+        :param account: The hex formatted address of the account.
 
-        return self.atomic_params.tx_id
+        :returns: The hex formatted address of the contract. If no contract is found, an empty string is returned.
+        """
 
-    def server_version(self) -> RPCResponse:
-        response = self.eulith_provider.make_request(RPCEndpoint("eulith_version"), [])
-        raise_if_error(response)
-        return response
+        if not is_hex_address(account):
+            raise TypeError("`account` must be a hex formatted address")
 
-    def send_transaction(self, params) -> RPCResponse:
-        """
-        Sends a transaction to the blockchain via the Eulith RPC provider, handling exceptions that may occur
-        when making a request with the make_request method from the HTTPProvider class.
+        contracts = self.eulith_service.get_deployed_execution_contracts()
 
-        :param params: Dictionary containing the parameters for the transaction
-        :type params: dict
+        for c in contracts:
+            if (
+                c["authorized_address"].lower() == account.lower()
+                and c["chain_id"] == self.chain_id
+            ):
+                return c["contract_address"]
 
-        :returns: The response from the Eulith API
-        :rtype: RPCResponse
+        return ""
 
-        :raises EulithRpcException: If there was an error with the RPC request
+    def eulith_create_contract_if_not_exist(self, account: str) -> str:
         """
+        Check if a toolkit contract exists for an account, and creates a new unique contract for the account
+        if it doesn't already exist.
 
-        params = list(params)
+        :param account: The hex formatted address of the account.
 
-        if self.atomic_params and len(params) > 0:
-            self.atomic_params.inject_in_body(params[0])
+        :return: The hex formatted address of the contract.
+        """
 
-        resp = self.eulith_provider.make_request(
-            RPCEndpoint("eth_sendTransaction"), params
-        )
-        raise_if_error(resp)
-        return resp
+        c = self.eulith_contract_address(account)
+        if c == "":
+            c = cast(str, self.eulith_create_contract(account))
+
+        return c
 
-    def create_new_contract(
+    def eulith_create_contract(
         self,
-        trading_key: str,
+        account: str,
         contract_type: Optional[str] = None,
         deploy_new_safe: bool = True,
-    ):
-        params = {"authorized_address": trading_key}
+        seed: Optional[int] = None,
+    ) -> Union[str, TxParams]:
+        """
+        Creates a new toolkit or armor contract for the specified authorized wallet address (account).
+        Toolkit contracts are deployed by us, we require the client to deploy their own armor contract.
+        Hence, you might either get a contract address back as a string or a ready-to-sign TxParams
+        object that you will need to sign and send yourself.
 
-        if contract_type:
-            params["contract_type"] = contract_type
+        :param deploy_new_safe: (bool) If true, deploy Armor and Safe at the same time. Otherwise, deploy armor only
+        and specify the existing Safe at a later step. Only relevant if contract_type == 'armor'.
+        :param account: The hex formatted address of the account.
+        :param contract_type: Optional contract type, defaults to toolkit contract.
+                              Can also pass `armor` to generate new DeFi armor deployment transaction
+        :param seed: The seed used to create the same safe address on a different network
 
-        if not deploy_new_safe:
-            params["safe_already_exists"] = True
+        :return: The hex formatted address of the newly created contract.
+        """
 
-        response = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_new_contract"), [params]
-        )
-        raise_if_error(response)
-        return response
+        if not is_hex_address(account):
+            raise TypeError("account must be a hex formatted address")
 
-    def start_transaction(self, trading_key: str, safe_address: str):
-        """
-        Starts a Eulith atomic transaction. Anything transaction you send within an atomic transaction
-        will get confirmed as a single unit. Everything operation in the unit will succeeds,
-        or the whole transactions fails. The state of the blockchain is frozen while your atomic transaction
-        is processing; there can't be any sandwiches, state changes, etc, in between your atomic operations.
-        """
+        if contract_type and contract_type != "armor":
+            raise TypeError(
+                f"we currently only support toolkit and armor contracts. "
+                f"If you're trying to deploy a toolkit contract, leave contract_type blank. "
+                f"Unrecognized type: {contract_type}"
+            )
 
-        self.atomic_params = AtomicTxParams(
-            str(uuid.uuid4()), safe_address, trading_key
+        result = self.eulith_service.create_new_contract(
+            account, contract_type, deploy_new_safe, seed
         )
 
-    def commit(self) -> TxParams:
+        if not contract_type:
+            tx_receipt = self.wait_for_transaction_receipt_with_confirmations(
+                result["new_contract_tx_hash"]
+            )
+            check_tx_receipt(tx_receipt)
+            return result["contract_address"]
+        elif contract_type == "armor":
+            return cast(TxParams, result)
+        else:
+            raise TypeError(f"unknown contract type: {contract_type!r}")
+
+    def eulith_swap_quote(
+        self, params: EulithSwapRequest
+    ) -> Tuple[float, List[TxParams]]:
         """
-        Serializes the current pending atomic tx into a single transactional unit, and returns
-        the unsigned params. To get the atomic transaction on-chain, you need to sign these params
-        and submit the transaction as a signed payload. The Eulith API handles this automatically for you.
+        Gets a swap quote which contains information about the price and liquidity of assets. Returns the price of the
+        quote and the transactions needed to execute the trade
 
-        :returns: A dictionary containing the transaction parameters.
-        :rtype: TxParams
+        :param params: The parameters for the swap.
 
-        :raises EulithRpcException: If the request fails or the response from the server contains an error.
+        :returns: A tuple containing the price of the swap and a list of `TxParams` objects that represent
+                  the transactions required for the swap.
         """
 
         if not self.is_atomic():
-            raise EulithRpcException("cannot commit outside atomic context")
+            warn(
+                "Performing swaps outside an atomic context is deprecated",
+                DeprecationWarning,
+                stacklevel=2,
+            )
 
-        params = {}
-        self.atomic_params.inject_in_body(params)
-        self.atomic_params = None
+        result = self.eulith_service.swap_quote(params)
+        price = result.get("price", 0.0)
+        txs = result.get("txs", [])
+        return price, txs
 
-        response = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_commit"), [params]
-        )
-        raise_if_error(response)
-        return cast(TxParams, response["result"])
+    # If the eulith_data.atomic flag is not set, the function will wait for each transaction receipt using the
+    # wait_for_transaction_receipt_with_confirmations method
+    def eulith_send_multi_transaction(self, txs: List[TxParams]) -> Optional[TxReceipt]:
+        """
+        Sends multiple transactions to the blockchain (or appends to the current atomic context) in a single batch,
+        with each transaction executed one after the other (order is preserved).
 
-    def commit_for_ace(self) -> AceImmediateTx:
+        :param txs: List of `TxParams` objects, each representing a single transaction to be executed.
         """
-        Variant of `commit` which returns a typed data payload rather than an unsigned transaction. The client should
-        then sign the payload and send it back to the server via the `send_ace_transaction` method.
 
-        Use this method when you are using an ACE server for signing rather than signing transactions directly from the
-        Python client.
+        r = None
+
+        for tx in txs:
+            tx_hash = self.eth.send_transaction(tx)
+            if not self.is_atomic():
+                r = self.wait_for_transaction_receipt_with_confirmations(tx_hash)
+                check_tx_receipt(r)
+
+        return r
 
-        :returns: The typed data to be signed by the client.
-        :rtype: AceImmediateTx
+    def eulith_get_erc_token(
+        self, symbol: TokenSymbol
+    ) -> Union[EulithERC20, EulithWETH]:
+        """
+        Obtains an instance of either the `EulithERC20` or `EulithWETH` class based on the provided token symbol.
         """
 
-        params = {}
-        self.atomic_params.inject_in_body(params)
-        self.atomic_params = None
+        contract_address, decimals = self.eulith_service.lookup_token_symbol(symbol)
+        if symbol == TokenSymbol.WETH:
+            return EulithWETH(self, self.to_checksum_address(contract_address))
+        else:
+            return EulithERC20(
+                self, self.to_checksum_address(contract_address), decimals
+            )
 
-        response = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_commit_for_ace"), [params]
-        )
-        raise_if_error(response)
-        return AceImmediateTx.from_json(response["result"])
+    def parse_uni_quote_to_swap_request(
+        self,
+        result: Dict[Any, Any],
+        fill_or_kill: bool,
+        recipient: Optional[ChecksumAddress],
+        pay_transfer_from: Optional[ChecksumAddress],
+    ) -> Tuple[float, UniswapPoolFee, EulithUniV3StartSwapRequest]:
+        """
+        This function takes in the result of Uniswap swap quote and converts it into a swap request that can be passed
+        to the `start_swap` function. Rather than manually extracting and formatting the necessary data,
+        this function does the work for you. The parse_uni_quote_to_swap_request function returns an instance of the
+        EulithUniV3StartSwapRequest class, which is the expected input type for the start_uniswap_v3_swap function.
+        This makes it easy to pass the swap request directly to the start_uniswap_v3_swap function after it has been
+        generated by the parse_uni_quote_to_swap_request function.
+
+        :param res: The result of a Uniswap swap quote, which is a dictionary containing information about the swap.
+        :param fill_or_kill: Default True doesn't allow any partial fills. If the order can't be filled
+                             fully at the specified price, we revert.
+        :param recipient: The Ethereum address of the recipient of the swap. This is an optional parameter.
+        :param pay_transfer_from: The Ethereum address of the account that will pay the sell_token to cover the swap.
+
+        :returns: A tuple containing the price of the swap, the pool fee, and the swap request.
+        """
+
+        price = result["price"]
+        sell_token_address = result["sell_token"]
+        sell_token = EulithERC20(self, sell_token_address)
+        amount = result["amount"]
+        pool_address = result["pool_address"]
+        limit_price = result["sqrt_limit_price"]
+        fee = result["fee"]
+        true_for_amount_in = result.get("true_for_amount_in")
+
+        if not true_for_amount_in:
+            amount *= -1.0  # make negative if we want exact amount out
+
+        swap_request = EulithUniV3StartSwapRequest(
+            sell_token=sell_token,
+            amount=amount,
+            pool_address=self.to_checksum_address(pool_address),
+            fill_or_kill=fill_or_kill,
+            sqrt_limit_price=limit_price,
+            recipient=recipient,
+            pay_transfer_from=pay_transfer_from,
+        )
+
+        return price, UniswapPoolFee(fee), swap_request
+
+    def wait_for_transaction_receipt_with_confirmations(
+        self, tx_hash: HexBytes, *, confirmations: int = 0
+    ) -> TxReceipt:
+        """
+        Wait for a receipt for the transaction hash, optionally waiting for a number of confirmed blocks before
+        returning.
+
+        If calling this function from within `EulithWeb3` with `confirmations` greater than zero, prefer setting it to
+        `confirmations=self.default_confirmations`. This is so that test code running against Anvil can set
+        `self.default_confirmations` to 0 and avoid timing out waiting for blocks that will never come.
+
+        :param tx_hash: The hash of the transaction to wait for.
+        :param confirmations: If greater than zero, this function will wait until
+                              current_block_number == tx_block_number + confirmations
+        """
+        tx_receipt = self.eth.wait_for_transaction_receipt(tx_hash)
+
+        if confirmations == 0:
+            return tx_receipt
+
+        attempts = 0
+        max_attempts = 3
+        timeout_secs = self._get_confirmation_timeout_secs()
+        last_block_number_seen = None
+
+        while True:
+            attempts += 1
+
+            current_block_number = self.eth.get_block_number()
+            if current_block_number >= tx_receipt["blockNumber"] + confirmations:
+                return tx_receipt
+
+            if (
+                last_block_number_seen is not None
+                and current_block_number > last_block_number_seen
+            ):
+                # We have made progress, so we can reset the number of attempts.
+                attempts = 0
+
+            last_block_number_seen = current_block_number
+
+            if attempts == max_attempts:
+                raise EulithRpcException(
+                    f"failed to confirm transaction {tx_receipt['transactionHash']!r}"
+                )
+
+            # We do not do exponential backoff here as we expect blocks to be created at a regular rate.
+            time.sleep(timeout_secs)
+
+    def _get_confirmation_timeout_secs(self) -> float:
+        if self._cached_confirmations_timeout_secs is not None:
+            return self._cached_confirmations_timeout_secs
+
+        # The duration of time to wait for confirmation is strongly dependent on how quickly the chain creates new
+        # blocks, which varies from chain to chain (e.g., Arbitrum is much faster than Ethereum mainnet). We take the
+        # average time of the last 3 blocks, add half a second as a hedge, and cap the timeout at 30 seconds.
+        current_block = self.eth.get_block("latest")
+        current_block_minus_3 = self.eth.get_block(current_block["number"] - 3)
+        timeout_secs = (
+            current_block["timestamp"] - current_block_minus_3["timestamp"]
+        ) / 3.0
+        timeout_secs += 0.5
+        timeout_secs = min(timeout_secs, 30.0)
+
+        r = timeout_secs
+        self._cached_confirmations_timeout_secs = r
+        return r
+
+
+# Namespace
+class v0:
+    """
+    Simplified and versioned access to the methods and functionality of `EulithWeb3`.
+    """
 
-    def rollback(self):
+    def __init__(self, ew3: EulithWeb3):
         """
-        Rollback here refers to discarding txs added to the atomic tx bundle during the call.
+        Initialize the `v0` class by taking an instance of `EulithWeb3` as an argument.
         """
 
-        if not self.is_atomic():
-            return
+        self.ew3 = ew3
 
-        params = {}
-        self.atomic_params.inject_in_body(params)
-        self.atomic_params = None
-
-        response = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_discard_atomic_transactions"), [params]
-        )
-        raise_if_error(response)
-        return
+    def get_server_version(self) -> str:
+        """
+        Returns the currently deployed version of the remote server.
+        """
+        return self.ew3.eulith_service.server_version()
 
-    def swap_quote(self, params: EulithSwapRequest) -> (bool, RPCResponse):
+    def send_multi_transaction(self, txs: List[TxParams]) -> Optional[TxReceipt]:
         """
-        Makes a request to the Eulith API to obtain a quote for a token swap. The returned quote is by default
-        the best price across multiple DEX aggregators.
+        Sends multiple transactions to the blockchain (or appends to the current atomic context) in a single batch,
+        with each transaction executed one after the other (order is preserved).
 
-        :param params: Request parameters
-        :type params: EulithSwapRequest
+        :param txs: List of `TxParams` objects, each representing a single transaction to be executed.
+        """
 
-        :returns: A tuple of a boolean indicating success and a `RPCResponse` object.
-        :rtype: (bool, RPCResponse)
+        return self.ew3.eulith_send_multi_transaction(txs)
 
-        :raises: requests.exceptions.HTTPError if there was an error making the request.
+    def start_atomic_transaction(
+        self, account: str, gnosis: str = ""
+    ) -> "AtomicContextManager":
         """
+        Begins an atomic transaction with your wallet as the authorized address,
+        or optionally with your gnosis safe as msg.sender
 
-        try:
-            sell_token: EulithERC20
-            buy_token: EulithERC20
-            sell_amount: float
-            recipient: Optional[ChecksumAddress]
-            route_through: Optional[EulithSwapProvider]
-            slippage_tolerance: Optional[float]
-            liquidity_source: Optional[EulithLiquiditySource]
-            from_address: Optional[ChecksumAddress]
-
-            sell_address = params.get("sell_token").address
-            buy_address = params.get("buy_token").address
-            parsed_params = {
-                "sell_token": sell_address,
-                "buy_token": buy_address,
-                "sell_amount": params.get("sell_amount"),
-            }
-            recipient = params.get("recipient", None)
-            route_through = params.get("route_through", None)
-            liquidity_source = params.get("liquidity_source", None)
-            slippage_tolerance = params.get("slippage_tolerance", None)
-            from_address = params.get("from_address", None)
-
-            if recipient:
-                parsed_params["recipient"] = recipient
-            if route_through:
-                parsed_params["route_through"] = route_through
-            if liquidity_source:
-                parsed_params["liquidity_source"] = liquidity_source
-            if slippage_tolerance:
-                parsed_params["slippage_tolerance"] = slippage_tolerance
-            if from_address:
-                parsed_params["from_address"] = from_address
-
-            if self.is_atomic():
-                rpc_method = "eulith_swap_atomic"
-                self.atomic_params.inject_in_body(parsed_params)
-            else:
-                rpc_method = "eulith_swap"
+        Use the return value as a context manager to automatically discard the atomic transaction on error. You still need to explicitly commit.
 
-            response = self.eulith_provider.make_request(
-                RPCEndpoint(rpc_method), [parsed_params]
-            )
-            raise_if_error(response)
+            with ew3.v0.start_atomic_transaction(account):
+               ...
+               tx_params = ew3.v0.commit_atomic_transaction()
+
+        :param account: Your ETH wallet address
+        :param gnosis: Optional. Gnosis Safe address.
+        """
 
-            return True, response
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
+        self.ew3.eulith_start_transaction(account, gnosis)
+        return AtomicContextManager(self.ew3)
 
-    def short_on(self, params: EulithShortOnRequest) -> (bool, RPCResponse):
+    def bundle_and_commit(
+        self,
+        auth_address: str,
+        txs: List[Any],
+        commit_options: Optional[atomic.CommitRequest] = None,
+    ) -> TxParams:
         """
-        Request the Eulith API to open a levered short position on a token.
+        Equivalent to calling `ew3.eth.send_transaction` for each transaction, followed by `commit_atomic_transaction()`
+        """
+        request = atomic.BundleRequest(
+            auth_address=auth_address, transactions=txs, commit_options=commit_options
+        )
+        return self.ew3.eulith_service.tx_bundle(request)
 
-        :param params: Request params
-        :type params: EulithShortOnRequest
-            collateral_token (EulithERC20) -- ERC20 token to be used as collateral.
-            short_token (EulithERC20) -- ERC20 token to be shorted.
-            collateral_amount (float) -- A float representing the amount of the `collateral_token` to be used.
+    def commit_atomic_transaction(self) -> TxParams:
+        """
+        Serializes your pending atomic unit into a single transaction and returns the params to be signed
+
+        :returns: The parameters of the committed transaction.
+        """
 
-        :returns: A tuple of a boolean indicating success and a `RPCResponse` object.
-        :rtype: (bool, RPCResponse)
+        r = self.ew3.eulith_commit_transaction()
+        if "message" in r:
+            # TODO: armor-policy specific exception
+            raise EulithRpcException(r)
+        return r
 
-        :raises: requests.exceptions.HTTPError if there was an error making the request.
+    def commit_atomic_transaction_for_ace(self, signer: Signer) -> HexStr:
         """
+        Serializes your pending atomic unit into an immediate transaction request for your ACE server, sends the
+        unsigned transaction to the ACE server for signing, submits the signed transaction to the network, and returns
+        the transaction hash.
 
-        try:
-            # Extract the addresses of the collateral and short tokens from the `params` argument.
-            collateral_address = params.get("collateral_token").address
-            short_address = params.get("short_token").address
-
-            # Create a dictionary of parameters for the request with the token addresses and collateral amount.
-            parsed_params = {
-                "collateral_token": collateral_address,
-                "short_token": short_address,
-                "collateral_amount": params.get("collateral_amount"),
-            }
-
-            if self.atomic_params:
-                self.atomic_params.inject_in_body(parsed_params)
-            else:
-                return False, RPCResponse(
-                    error="cannot call short on outside of an atomic context"
-                )
+        :param signer: The signer to sign the transaction request for ACE. Note that this signer is for authentication
+                       of the transaction request with ACE, *not* for signing the transaction itself, which is done by
+                       the private key on ACE.
 
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_short_on"), [parsed_params]
-            )
-            raise_if_error(response)
-            return True, response
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
+        :returns: The hash of the atomic transaction.
+        """
+        ace_immediate_tx = self.ew3.eulith_service.commit_for_ace()
+        typed_data = get_ace_immediate_tx_typed_data(ace_immediate_tx)
+        message_hash = get_ace_immediate_tx_hash(ace_immediate_tx)
+        signed_typed_data = signer.sign_typed_data(typed_data, message_hash)
+        serialized_signed_typed_data = normalize_signature(signed_typed_data)
+        return self.ew3.eulith_service.send_ace_transaction(
+            serialized_signed_typed_data, ace_immediate_tx
+        )
 
-    def short_off(self, params: EulithShortOffRequest) -> (bool, RPCResponse):
+    def rollback_atomic_transaction(self) -> None:
         """
-        Makes a request to the Eulith API to unwind an existing short.
+        Rollback a transaction, discard the current atomic transaction
+        """
+        self.ew3.eulith_rollback_transaction()
 
-        :param params: Request params
-        :type params: EulithShortOffRequest
+    def get_toolkit_contract_address(self, account: str) -> str:
+        """
+        Retrieve the toolkit contract address bearing a one-to-one relationship to the `account` address.
+        One toolkit contract is generated per wallet address.
 
-        :returns: A tuple of a boolean indicating success and a `RPCResponse` object.
-        :rtype: (bool, RPCResponse)
+        :param account: The hex formatted address of the account.
 
-        :raises: requests.exceptions.HTTPError if there was an error making the request.
+        :returns: The hex formatted address of the contract. If no contract is found, an empty string is returned.
         """
 
-        try:
-            collateral_address = params.get("collateral_token").address
-            short_address = params.get("short_token").address
+        return self.ew3.eulith_contract_address(account)
 
-            parsed_params = {
-                "collateral_token": collateral_address,
-                "short_token": short_address,
-                "repay_short_amount": params.get("repay_short_amount"),
-                "true_for_unwind_a": params.get("true_for_unwind_a", True),
-            }
-
-            if self.atomic_params:
-                self.atomic_params.inject_in_body(parsed_params)
-            else:
-                return False, RPCResponse(
-                    error="cannot call short on outside of an atomic context"
-                )
+    def get_armor_and_safe_addresses(
+        self, authorized_trading_address: str
+    ) -> Tuple[str, str]:
+        """
+        Get the armor and safe addresses for a specific authorized_trading_address.
 
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_short_off"), [parsed_params]
-            )
-            raise_if_error(response)
-            return True, response
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
+        This method retrieves the armor and safe addresses associated with the provided authorized_trading_address.
+
+        :param authorized_trading_address: The Ethereum address (str) to search for.
+        :return: A tuple (str, str) containing the contract address and safe address, respectively.
+                 If no match is found, an empty tuple ('', '') is returned.
 
-    def start_uniswap_v3_loan(
-        self, params: EulithUniV3StartLoanRequest
-    ) -> (bool, RPCResponse):
+        :raises EulithRpcException: If there is an issue fetching the deployed execution contracts.
         """
-        Makes a request to start a loan in Uniswap V3. This loan is its own atomic structure, meaning
-        after you start a loan you have immediate access to the borrow tokens. Transactions you send
-        after starting the loan are included in the loan until you call finish_inner to close the loan and
-        return one layer up in the nested atomic structure.
+        contracts = self.ew3.eulith_service.get_deployed_execution_contracts()
 
-        Note that loans have to execute in an atomic transaction. You can't execute a loan on its own.
+        for c in contracts:
+            if (
+                c["authorized_address"].lower() == authorized_trading_address.lower()
+                and c["chain_id"] == self.ew3.chain_id
+            ):
+                return c["contract_address"], c["safe_address"]
 
-        :param params: Request params
-        :type params: EulithUniV3StartLoanRequest
+        return "", ""
+
+    def ensure_toolkit_contract(self, account: str) -> str:
+        """
+        Check if a toolkit contract exists for an account, and creates a new unique contract for the account
+        if it doesn't already exist.
 
-        :returns: A tuple of a boolean indicating success and an `RPCResponse` object.
-        :rtype: (bool, RPCResponse)
+        :param account: The hex formatted address of the account.
 
-        :raises: requests.exceptions.HTTPError if there was an error making the request.
+        :return: The hex formatted address of the contract.
         """
 
-        try:
-            borrow_token_a = params.get("borrow_token_a").address
-            borrow_amount_a = params.get("borrow_amount_a")
-            borrow_token_b = params.get("borrow_token_b", None)
-            borrow_amount_b = params.get("borrow_amount_b", None)
-            pay_transfer_from = params.get("pay_transfer_from", None)
-            recipient = params.get("recipient", None)
-
-            parsed_params = {
-                "borrow_token_a": borrow_token_a,
-                "borrow_amount_a": borrow_amount_a,
-            }
-
-            if borrow_token_b:
-                parsed_params["borrow_token_b"] = borrow_token_b.address
-            if borrow_amount_b:
-                parsed_params["borrow_amount_b"] = borrow_amount_b
-            if pay_transfer_from:
-                parsed_params["pay_transfer_from"] = pay_transfer_from
-            if recipient:
-                parsed_params["recipient"] = recipient
-
-            if self.atomic_params:
-                self.atomic_params.inject_in_body(parsed_params)
-            else:
-                return False, RPCResponse(
-                    error="cannot call short on outside of an atomic context"
-                )
+        return self.ew3.eulith_create_contract_if_not_exist(account)
 
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_start_uniswapv3_loan"), [parsed_params]
-            )
-            raise_if_error(response)
-            return True, response
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
-
-    def start_uniswap_v3_swap(
-        self, params: EulithUniV3StartSwapRequest
-    ) -> (bool, RPCResponse):
+    def create_toolkit_contract(self, account: str) -> str:
         """
-        Starting a uniswap V3 swap, a trade of one token for another on the Uniswap v3 protocol.
+        Creates a new toolkit contract for the specified authorized wallet address (account).
 
-        This swap is its own atomic structure, meaning after you start a swap you have immediate access to the
-        buy_tokens tokens. Transactions you send after starting the swap are included in the loan until you call
-        finish_inner to close the swap and return one layer up in the nested atomic structure.
+        :param account: The hex formatted address of the account.
 
-        :param params: Request params
-        :type params: EulithUniV3StartSwapRequest
+        :return: The hex formatted address of the newly created contract.
+        """
 
-        :returns: A tuple of a boolean indicating success and a `RPCResponse` object.
-        :rtype: (bool, RPCResponse)
+        return cast(str, self.ew3.eulith_create_contract(account))
 
-        :raises: requests.exceptions.HTTPError if there was an error making the request.
+    def get_armor_deploy_tx(
+        self, account: str, deploy_new_safe: bool = True, seed: Optional[int] = None,
+    ) -> TxParams:
         """
+        Generates transaction to create a new armor and safe contract for the specified authorized wallet address (account).
 
-        try:
-            sell_token = params.get("sell_token").address
-            amount = params.get("amount")
-            pool_address = params.get("pool_address")
-            fill_or_kill = params.get("fill_or_kill")
-            sqrt_limit_price = params.get("sqrt_limit_price")
-            recipient = params.get("recipient", None)
-            pay_transfer_from = params.get("pay_transfer_from", None)
-
-            parsed_params = {
-                "sell_token": sell_token,
-                "amount": amount,
-                "pool_address": pool_address,
-                "fill_or_kill": fill_or_kill,
-                "sqrt_limit_price": sqrt_limit_price,
-            }
-
-            if recipient:
-                parsed_params["recipient"] = recipient
-
-            if pay_transfer_from:
-                parsed_params["pay_transfer_from"] = pay_transfer_from
-
-            if self.atomic_params:
-                self.atomic_params.inject_in_body(parsed_params)
-            else:
-                return False, RPCResponse(error="must call in atomic context")
+        :param deploy_new_safe: (bool) If true, deploy Armor and Safe at the same time. Otherwise, deploy armor only
+        and specify the existing Safe at a later step
+        :param account: The hex formatted address of the account.
+        :param seed: The seed used to reproduce the same address on a different network
 
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_start_uniswapv3_swap"), [parsed_params]
-            )
-            raise_if_error(response)
-            return True, response
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
+        :return: The TxParams to sign and send in order to deploy your new armor and safe contracts.
+        """
+        return cast(
+            TxParams, self.ew3.eulith_create_contract(account, "armor", deploy_new_safe, seed)
+        )
+
+    def ensure_valid_api_token(self) -> None:
+        pass
+
+    def get_erc_token(self, symbol: TokenSymbol) -> Union[EulithERC20, EulithWETH]:
+        """
+        Obtains an instance of either the `EulithERC20` or `EulithWETH` class based on the provided token symbol.
+
+        :param symbol: Symbol of the token to look up.
 
-    def start_aave_v2_loan(
-        self, params: EulithAaveV2StartLoanRequest
-    ) -> (bool, RPCResponse):
+        :returns: An instance of either the `EulithERC20` or `EulithWETH` class.
         """
-        Start a loan using the Aave V2 protocol
 
-        :param params: Request params
-        :type params: EulithAaveV2StartLoanRequest
+        return self.ew3.eulith_get_erc_token(symbol)
 
-        :returns: A tuple of a boolean indicating success and a `RPCResponse` object.
-        :rtype: (bool, RPCResponse)
+    def get_swap_quote(self, params: EulithSwapRequest) -> Tuple[float, List[TxParams]]:
+        """
+        Gets a swap quote which contains information about the price and liquidity of assets. Returns the price of the
+        quote and the transactions needed to execute the trade
 
-        :raises: requests.exceptions.HTTPError if there was an error making the request.
+        :param params: The parameters for the swap.
+
+        :returns: A tuple containing the price of the swap and a list of `TxParams` objects that represent
+                  the transactions required for the swap.
         """
 
-        try:
-            tokens = params.get("tokens")
-            token_params = []
-            for t in tokens:
-                token_params.append(
+        if not self.ew3.is_atomic():
+            warn(
+                "Performing swaps outside an atomic context is not recommended; its dangerous. "
+                "Use DeFi Armor.",
+                DeprecationWarning,
+            )
+
+            if self.ew3.wallet_address and not params.get("from_address", None):
+                params.update(
                     {
-                        "token_address": t.get("token_address").address,
-                        "amount": t.get("amount"),
+                        "from_address": self.ew3.to_checksum_address(
+                            self.ew3.wallet_address
+                        )
                     }
                 )
 
-            parsed_params = {
-                "tokens": token_params,
-            }
-
-            if self.atomic_params:
-                self.atomic_params.inject_in_body(parsed_params)
-            else:
-                return False, RPCResponse(error="must call in atomic context")
+        return self.ew3.eulith_swap_quote(params)
 
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_start_aavev2_loan"), [parsed_params]
-            )
-            raise_if_error(response)
-            return True, response
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
+    def short_on(self, params: EulithShortOnRequest) -> float:
+        """
+        Request the Eulith API to open a levered short position on a token.
 
-    def finish_inner(self) -> (bool, RPCResponse):
+        :return: the leverage of the short position
         """
-        Uniswap & Aave flash loans and swaps are their own "sub atomic" structures. So when you start
-        one of those actions, you have to finish it by calling this method. "Finishing" here means you close the
-        transaction and append it to the outer atomic structure.
 
-        :return: A tuple that contains a boolean indicating if the request was successful, and a `RPCResponse`
-        :rtype: (bool, RPCResponse)
+        result = self.ew3.eulith_service.short_on(params)
+        return result.get("leverage", 0.0)
 
-        :raises HTTPError: In case of an error in the HTTP request.
+    def short_off(self, params: EulithShortOffRequest) -> float:
         """
-        params = {}
+        Makes a request to the Eulith API to unwind an existing short.
 
-        if self.atomic_params:
-            self.atomic_params.inject_in_body(params)
-        else:
-            return False, RPCResponse(error="must call in atomic context")
+        :return: The amount of released collateral.
+        """
 
-        try:
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_finish_inner"), [params]
-            )
-            raise_if_error(response)
-            return True, response
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
+        result = self.ew3.eulith_service.short_off(params)
+        return result.get("released_collateral", 0.0)
 
-    def uniswap_v3_quote(
-        self, params: EulithUniV3SwapQuoteRequest
-    ) -> (bool, RPCResponse):
+    def get_univ3_pool(
+        self, params: EulithUniswapPoolLookupRequest
+    ) -> EulithUniswapV3Pool:
+        """
+        Looking up information about UniSwap V3 pools.
+
+        :param params: Request parameters
+
+        :return: An instance of `EulithUniswapV3Pool` class representing the Uniswap pool information.
         """
-        Request a quote from Uniswap V3 for a swap between two tokens.
 
-        :param params: Request params
-        :type params: EulithUniV3SwapQuoteRequest
+        result = self.ew3.eulith_service.lookup_univ3_pool(params)
+        if len(result) != 1:
+            raise EulithRpcException(
+                f"uniswap v3 pool lookup came back with an unexpected response: {result}"
+            )
+        inner_result = result[0]
 
-        :returns: A tuple of a boolean indicating success and a `RPCResponse` object.
-        :rtype: (bool, RPCResponse)
+        token_zero = inner_result["token_zero"]
+        token_one = inner_result["token_one"]
+        fee = inner_result["fee"]
+        pool_address = inner_result["pool_address"]
+        return EulithUniswapV3Pool(
+            self.ew3,
+            self.ew3.to_checksum_address(pool_address),
+            UniswapPoolFee(fee),
+            self.ew3.to_checksum_address(token_zero),
+            self.ew3.to_checksum_address(token_one),
+        )
 
-        :raises: requests.exceptions.HTTPError if there was an error making the request.
+    # returns fee (float) as percent: i.e. 0.001 = 0.1%
+    def start_flash_loan(
+        self, params: Union[EulithUniV3StartLoanRequest, EulithAaveV2StartLoanRequest]
+    ) -> float:
         """
+        Initiates a flash loan. A flash loan is a type of loan that can be taken and repaid within a single transaction.
+        This is a generic wrapper around Uniswap flash loans and Aave flash loans. You can pass either as the params
+        and it will handle the request appropriately.
 
-        try:
-            parsed_params = {
-                "sell_token": params.get("sell_token").address,
-                "buy_token": params.get("buy_token").address,
-                "amount": params.get("amount"),
-                "true_for_amount_in": params.get("true_for_amount_in", True),
-            }
-
-            fee = params.get("fee", None)
-            if fee:
-                parsed_params["fee"] = fee.value
+        :param params: The parameters required to initiate the flash loan.
+
+        :return: The fee of the flash loan.
+        """
 
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_uniswapv3_quote"), [parsed_params]
+        param_keys = params.keys()
+        if "borrow_token_a" in param_keys:
+            result = self.ew3.eulith_service.start_uniswap_v3_loan(
+                cast(EulithUniV3StartLoanRequest, params)
+            )
+        else:
+            result = self.ew3.eulith_service.start_aave_v2_loan(
+                cast(EulithAaveV2StartLoanRequest, params)
             )
-            raise_if_error(response)
-            return True, response
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
 
-    def lookup_univ3_pool(
-        self, params: EulithUniswapPoolLookupRequest
-    ) -> (bool, RPCResponse):
+        fee = int(result, 16)
+        return fee / INT_FEE_TO_FLOAT_DIVISOR
+
+    def start_uni_swap(self, params: EulithUniV3StartSwapRequest) -> float:
         """
-        Looking up information about UniSwap V3 pools.
+        Starting a uniswap V3 swap, a trade of one token for another on the Uniswap v3 protocol.
+
+        This swap is its own atomic structure, meaning after you start a swap you have immediate access to the
+        buy_tokens tokens. Transactions you send after starting the swap are included in the loan until you call
+        finish_inner to close the swap and return one layer up in the nested atomic structure.
 
-        :param params: Request params
-        :type params: EulithUniswapPoolLookupRequest
+        :return: The fee of the Uniswap V3 swap, represented as a percentage.
+        """
 
-        :returns: A tuple of a boolean indicating success and a `RPCResponse` object.
-        :rtype: (bool, RPCResponse)
+        result = self.ew3.eulith_service.start_uniswap_v3_swap(params)
+        fee = int(result, 16)
+        return fee / INT_FEE_TO_FLOAT_DIVISOR
 
-        :raises: requests.exceptions.HTTPError if there was an error making the request.
+    def get_univ3_best_price_quote(
+        self,
+        sell_token: EulithERC20,
+        buy_token: EulithERC20,
+        amount: float,
+        true_for_amount_in: bool = True,
+        fill_or_kill: bool = True,
+        recipient: Optional[ChecksumAddress] = None,
+        pay_transfer_from: Optional[ChecksumAddress] = None,
+    ) -> Tuple[float, float, EulithUniV3StartSwapRequest]:
         """
+        Get the best price quote for a given token exchange on Uniswap V3.
 
-        try:
-            parsed_params = {
-                "token_a": params.get("token_a").address,
-                "token_b": params.get("token_b").address,
-                "fee": params.get("fee").value,
-            }
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_uniswapv3_pool_lookup"), [parsed_params]
-            )
-            raise_if_error(response)
-            return True, response
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
+        :param sell_token: The token that is to be sold.
+        :param buy_token: The token that is to be bought.
+        :param amount: The amount of the trade. If true_for_amount_in, this is the exact sell_amount in. Otherwise, the exact buy_amount out.
+        :param true_for_amount_in: Whether the `amount` is in `sell_token` IN or `buy_token` OUT. Defaults to True.
+        :param fill_or_kill: Default True doesn't allow any partial fills. If the order can't be filled fully at the specified price, revert.
+        :param recipient: The address of the recipient of the `buy_token`. Defaults to msg.sender
+        :param pay_transfer_from: The address to pay the sell side of the transaction. Defaults to msg.sender
 
-    def lookup_token_symbol(self, symbol: TokenSymbol) -> (bool, ChecksumAddress, int):
+        :return: A tuple containing three values:
+            - price (float): The price of the `buy_token` in terms of `sell_token`.
+            - fee (float): The fee for the transaction.
+            - swap_request (EulithUniV3StartSwapRequest): The swap request details. These can be immediately used to execute the swap
         """
-        Look up token information by ERC20 symbol.
 
-        :param symbol: Token symbol to look up.
-        :type symbol: TokenSymbol
+        parsed_params = EulithUniV3SwapQuoteRequest(
+            sell_token=sell_token,
+            buy_token=buy_token,
+            amount=amount,
+            true_for_amount_in=true_for_amount_in,
+            fee=None,
+        )
+        result = self.ew3.eulith_service.uniswap_v3_quote(parsed_params)
+        price, fee, swap_request = self.ew3.parse_uni_quote_to_swap_request(
+            result, fill_or_kill, recipient, pay_transfer_from
+        )
+        return price, fee / INT_FEE_TO_FLOAT_DIVISOR, swap_request
 
-        :return: A tuple containing a boolean indicating the success of the request,
-                 the contract address of the token, and the number of decimals of the token.
-        :rtype: tuple(bool, ChecksumAddress, int)
+    def finish_inner(self) -> int:
         """
+        Finishes the actual exchange of tokens in the swap or loan and returns the scope back to the outer atomic
+        context. Remember, uniswap swaps and loans are SUB ATOMIC, meaning they have their own atomic structure that you
+        can add to. When you're done with those transactions you need to close them with this method
 
-        try:
-            res = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_erc_lookup"), [{"symbol": symbol}]
-            )
-            raise_if_error(res)
-            parsed_res = res.get("result", [])
-            if len(parsed_res) != 1:
-                return (
-                    False,
-                    RPCResponse(
-                        error=f"unexpected response for {symbol} lookup, token isn't recognized"
-                    ),
-                    -1,
+        :returns: The number of transactions appended to the root atomic transaction
+        """
+
+        result = self.ew3.eulith_service.finish_inner()
+        return int(result, 16)
+
+    def start_flash(self, params: FlashRequest) -> Tuple[float, float]:
+        """
+        A generic wrapper for any kind of flash transaction between any two tokens.
+
+        :returns: A tuple of two floats representing (price, fee) of the flash. If take and pay are the same token, the
+                  price is 1.0. Fee is returned as a percent, e.g. 0.001 = 0.1%
+        """
+
+        amount = params["take_amount"]
+        pay_transfer_from = params.get("pay_transfer_from", None)
+        recipient = params.get("recipient", None)
+
+        take_address = params["take"].address
+        pay_address = params["pay"].address
+
+        if not take_address:
+            raise ValueError("missing take address")
+
+        if not pay_address:
+            raise ValueError("missing pay address")
+
+        if take_address.lower() == pay_address.lower():
+            fee = self.start_flash_loan(
+                EulithUniV3StartLoanRequest(
+                    borrow_token_a=params["take"],
+                    borrow_amount_a=amount,
+                    borrow_token_b=None,
+                    borrow_amount_b=None,
+                    pay_transfer_from=pay_transfer_from,
+                    recipient=recipient,
                 )
-            return (
+            )
+
+            return 1.0, fee
+        else:
+            price, fee, swap_request = self.get_univ3_best_price_quote(
+                params["pay"],
+                params["take"],
+                amount,
+                False,
                 True,
-                parsed_res[0].get("contract_address"),
-                parsed_res[0].get("decimals"),
+                recipient,
+                pay_transfer_from,
             )
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e)), -1
+            fee = self.start_uni_swap(swap_request)
+            return price, fee
 
-    def get_gmx_addresses(self) -> (bool, dict):
+    def pay_flash(self) -> int:
         """
-        Returns a dictionary of GMX contract addresses.
+        Pays and closes an open flash transaction.
 
-        :return: A tuple containing a boolean indicating success or failure, and a dictionary of GMX contract addresses.
-        :rtype: tuple
+        :returns: The number of transactions in the current atomic unit.
         """
-        try:
-            res = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_gmx_address_lookup"), None
-            )
-            raise_if_error(res)
-            result = res.get("result", {})
-            return True, result
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
 
-    def get_gmx_positions(
-        self,
-        wallet_address: ChecksumAddress,
-        collateral_tokens: List[EulithERC20],
-        index_tokens: List[EulithERC20],
-        is_long: List[bool],
-    ) -> (bool, dict):
-        """
-        Get positions of the given wallet for a given set of collateral and index tokens and directions
-
-        :param wallet_address: The address to get the positions of
-        :type wallet_address: ChecksumAddress
-        :param collateral_tokens: List of the collateral tokens the positions belong to
-        :type collateral_tokens: List[EulithERC20]
-        :param index_tokens: List of the index tokens the positions belong to
-        :type index_tokens: List[EulithERC20]
-        :param is_long: List of the direction of each position True is long False is short
-        :type is_long: List[bool]
-        :return: A tuple with the status and result
-        :rtype: (bool, dict)
+        return self.finish_inner()
+
+    def get_gmx_addresses(self) -> Dict[Any, Any]:
         """
-        try:
-            collateral_addresses = []
-            index_addresses = []
+        Returns the addresses of various contracts used by GMX protocol.
 
-            for t in collateral_tokens:
-                collateral_addresses.append(t.address)
+        :return: A dictionary with the contract addresses as values and their names as keys.
+        """
+        return self.ew3.eulith_service.get_gmx_addresses()
 
-            for t in index_tokens:
-                index_addresses.append(t.address)
+    def deploy_new_armor(
+        self,
+        authorized_trading_address: ChecksumAddress,
+        existing_safe_address: Optional[ChecksumAddress] = None,
+        override_tx_params: Optional[TxParams] = None,
+        seed: Optional[int] = None,
+    ) -> Tuple[str, str]:
+        """
+        Deploys new armor contract using the current wallet configured in EulithWeb3. Note that the
+        deploying wallet is NOT the same thing as the authorized_address on the armor contract. The user
+        must choose the authorized trading address and pass it into this method.
 
-            params = {
-                "wallet_address": wallet_address,
-                "collateral_addresses": collateral_addresses,
-                "index_addresses": index_addresses,
-                "is_long": is_long,
-            }
+        :param existing_safe_address: Deploy Armor into an existing safe instead of setting up a new one.
+        :param authorized_trading_address: (str) The address authorized to execute trades through the new armor contract
+        :param override_tx_params: (TxParams, optional) The optional transaction parameters
+                                   to override default values (like gas, gas_price, etc). Defaults to None.
+        :param seed: the seed used to create the same safe address on a different network
 
-            res = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_gmx_position_lookup"), [params]
-            )
-            raise_if_error(res)
-            result = res.get("result", {})
-            return True, result
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
-
-    def request_gmx_mint_glp(
-        self, pay_token: EulithERC20, pay_amount: float, slippage: Optional[float]
-    ) -> (bool, dict):
-        """
-        Requests to mint GLP tokens by providing pay_token and pay_amount.
-        Returns minimum GLP tokens to be minted, minimum USD value and transactions to be executed to take the position.
-        We handle some of this logic server-side to keep the client light and simple.
-
-        :param pay_token: The token to pay with
-        :type pay_token: EulithERC20
-        :param pay_amount: The amount of pay_token to use
-        :type pay_amount: float
-        :param slippage: The slippage tolerance as a percentage, defaults to None, in percentage units i.e. 0.01
-        :type slippage: Optional[float]
-        :return: A tuple containing whether the request was successful and the resulting dictionary
-        :rtype: Tuple[bool, dict]
+        :return: A tuple of armor and safe addresses.
         """
-        try:
-            params = {
-                "pay_token_address": pay_token.address,
-                "pay_amount": pay_amount,
-            }
 
-            if slippage:
-                params["slippage"] = slippage
+        deploy_new_safe = existing_safe_address is None
 
-            res = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_mint_and_stake_glp"), [params]
-            )
-            raise_if_error(res)
-            result = res.get("result", {})
-            return True, result
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
-
-    def get_pt_quote(
-        self, buy_pt_amount: float, market_address: ChecksumAddress
-    ) -> (bool, dict):
-        try:
-            params = {
-                "market_address": market_address,
-                "exact_pt_out": buy_pt_amount,
-            }
+        deploy_armor_tx = self.get_armor_deploy_tx(
+            authorized_trading_address, deploy_new_safe, seed
+        )
 
-            res = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_pendle_pt_quote"), [params]
-            )
-            raise_if_error(res)
-            result = res.get("result", {})
-            return True, result
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
+        if override_tx_params:
+            deploy_armor_tx.update(override_tx_params)
+
+        h = self.ew3.eth.send_transaction(deploy_armor_tx)
+        tx_receipt = self.ew3.wait_for_transaction_receipt_with_confirmations(
+            h, confirmations=self.ew3.default_confirmations
+        )
+        check_tx_receipt(tx_receipt)
+
+        accepted = self.ew3.eulith_service.submit_new_armor_hash(
+            h.hex(), existing_safe_address
+        )
+
+        if not accepted:
+            raise EulithRpcException("failed to submit new armor tx hash to the server")
 
-    def submit_new_armor_hash(
-        self, tx_hash: str, existing_safe_address: Optional[ChecksumAddress] = None
+        return self.get_armor_and_safe_addresses(authorized_trading_address)
+
+    def submit_enable_module_signature(
+        self, authorized_trading_address: str, signer: Signer
     ) -> bool:
-        try:
-            params = {"tx_hash": tx_hash}
+        """
+        Submits a signature to enable a module for a safe. Note that the signature must come from a safe owner,
+        but submitting a signature here DOES NOT add the signing address as an owner of the safe. The owners are
+        specified in a later initialization step.
 
-            if existing_safe_address:
-                params["safe_address"] = existing_safe_address
+        :param authorized_trading_address: (str) The address authorized to execute trades through the new armor contract
+        :param signer: The signer to apply the signature to enable the armor module
 
-            res = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_submit_armor_hash"), [params]
-            )
-            raise_if_error(res)
-            result = res.get("result", False)
-            return result
-        except EulithRpcException:
-            return False
+        :return: true if ok, false if failed
+        """
+        aa, sa = self.get_armor_and_safe_addresses(authorized_trading_address)
+        safe = ISafe(self.ew3, self.ew3.to_checksum_address(sa))
 
-    def get_deployed_execution_contracts(self) -> (bool, dict):
-        try:
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_get_contracts"), {}
-            )
-            raise_if_error(response)
-            contracts = response["result"]["contracts"]
-            return True, contracts
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
+        enable_module_tx = safe.enable_module(
+            self.ew3.to_checksum_address(aa),
+            override_tx_parameters={
+                "gas": 0,
+                "nonce": Nonce(0),
+            },
+        )
 
-    def submit_safe_signature(
-        self,
-        module_address: str,
-        owner_address: str,
-        signature: str,
-        signed_hash: str,
-        signature_type: str,
-    ) -> (bool, dict):
-        try:
-            params = {
-                "module_address": module_address,
-                "owner_address": owner_address,
-                "signature": str(signature),
-                "signed_hash": signed_hash,
-                "signature_type": signature_type,
-            }
+        checksum_sa = self.ew3.to_checksum_address(sa)
 
-            res = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_submit_enable_safe_signature"), [params]
-            )
-            raise_if_error(res)
-            result = res.get("result", False)
-            return True, result
-        except requests.exceptions.HTTPError as e:
-            return False, RPCResponse(error=str(e))
-
-    def get_enable_safe_tx(
-        self, auth_address: str, owner_threshold: int, owners: List[str]
-    ) -> (bool, TxParams):  # For new Safes
-        try:
-            params = {
-                "auth_address": auth_address,
-                "owner_threshold": owner_threshold,
-                "owners": owners,
-            }
+        enable_data = enable_module_tx["data"]
 
-            res = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_get_setup_safe_tx"), [params]
-            )
-            raise_if_error(res)
-            result = res.get("result", {})
-            return True, result
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
+        typed_data_payload = get_enable_module_typed_data(
+            checksum_sa, self.ew3.eth.chain_id, str(enable_data), safe.nonce()
+        )
+
+        signable_message = encode_typed_data(full_message=dict(typed_data_payload))
+        typed_data_hash = keccak(
+            b"\x19\x01" + signable_message.header + signable_message.body
+        )
 
-    def get_enable_module_tx(
+        signature = signer.sign_typed_data(typed_data_payload, typed_data_hash)
+
+        serialized_signature = normalize_signature(signature)
+
+        return self.ew3.eulith_service.submit_safe_signature(
+            aa,
+            str(signer.address),
+            serialized_signature,
+            f"0x{typed_data_hash.hex()}",
+            "enable_module",
+        )
+
+    def enable_armor_for_new_safe(
         self,
         auth_address: str,
-    ) -> (bool, TxParams):  # For existing Safes
-        try:
-            params = {
-                "auth_address": auth_address,
-            }
+        owner_threshold: int,
+        owners: List[str],
+        override_tx_params: Optional[TxParams] = None,
+        has_ace: bool = False,
+    ) -> bool:
+        """
+        Enable the armor for the contract by creating and submitting an initialization transaction. Note that
+        the owners passed here MUST include the addresses of the signatures you submitted in the enable
+        module step AND you must have submitted at least `owner_threshold` signatures in that step.
 
-            res = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_get_enable_module_tx"), [params]
-            )
-            raise_if_error(res)
-            result = res.get("result", {})
-            return True, result
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
-
-    def submit_enable_safe_tx_hash(
-        self, tx_hash: str, *, has_ace: bool
-    ) -> (bool, dict):
-        try:
-            params = {
-                "tx_hash": tx_hash,
-                "has_ace": has_ace,
-            }
+        :param auth_address: The authorized address of the Armor contract.
+        :param owner_threshold: The minimum number of owner signatures required to authorize a transaction on the safe
+        :param owners: A list of owner addresses that are allowed to manage the contract.
+        :param override_tx_params: Optional dictionary to override transaction parameters.
+        :param has_ace: Whether ACE is enabled for the armor contract to be created
 
-            res = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_submit_setup_safe_hash"), [params]
-            )
-            raise_if_error(res)
-            result = res.get("result", False)
-            return result, {}
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
-
-    def submit_enable_module_tx_hash(
-        self, tx_hash: str, trading_key_address: str
-    ) -> (bool, dict):
-        try:
-            params = {
-                "tx_hash": tx_hash,
-                "auth_address": trading_key_address,
-            }
+        :return: True if the transaction is successfully submitted, False otherwise.
+        """
+        result = self.ew3.eulith_service.get_enable_safe_tx(
+            auth_address, owner_threshold, owners
+        )
 
-            res = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_submit_enable_module_hash"), [params]
-            )
-            raise_if_error(res)
-            result = res.get("result", False)
-            return result, {}
-        except EulithRpcException as e:
-            return False, RPCResponse(error=str(e))
+        if override_tx_params:
+            result.update(override_tx_params)
+        else:
+            result.update({"from": self.ew3.wallet_address})
+
+        h = self.ew3.eth.send_transaction(cast(TxParams, result))
+        tx_receipt = self.ew3.wait_for_transaction_receipt_with_confirmations(
+            h, confirmations=self.ew3.default_confirmations
+        )
+        check_tx_receipt(tx_receipt)
+
+        return self.ew3.eulith_service.submit_enable_safe_tx_hash(
+            h.hex(), has_ace=has_ace
+        )
+
+    def enable_armor_for_existing_safe(
+        self,
+        trading_key_address: str,
+        override_tx_params: Optional[TxParams] = None,
+    ) -> bool:
+        result = self.ew3.eulith_service.get_enable_module_tx(trading_key_address)
+
+        if override_tx_params:
+            result.update(override_tx_params)
+        else:
+            result.update({"from": self.ew3.wallet_address})
+
+        h = self.ew3.eth.send_transaction(cast(TxParams, result))
+        tx_receipt = self.ew3.wait_for_transaction_receipt_with_confirmations(
+            h, confirmations=self.ew3.default_confirmations
+        )
+        check_tx_receipt(tx_receipt)
+
+        return self.ew3.eulith_service.submit_enable_module_tx_hash(
+            h.hex(), trading_key_address
+        )
+
+    def create_draft_client_whitelist(
+        self, auth_address: str, addresses: List[str]
+    ) -> int:
+        raise EulithDeprecationException(
+            "This method has been removed. Use create_draft_client_whitelist_v2 instead."
+        )
 
     def create_draft_client_whitelist_v2(
-        self, request: whitelists_v2.rpc.CreateRequest
-    ) -> whitelists_v2.rpc.CreateResponse:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_create_draft_client_whitelist_v2"), [request]
+        self, display_name: str, addresses: List[whitelists_v2.AddressOnChain]
+    ) -> int:
+        """
+        Create a draft of the client whitelist for an Armor contract.
+
+        :param display_name:
+        :param addresses: The list of addresses to include on the whitelist.
+
+        :return: An opaque identifier for the whitelist, to be passed to `submit_draft_client_whitelist_signature_v2`.
+        """
+        request = whitelists_v2.rpc.CreateRequest(
+            display_name=display_name, addresses=addresses
+        )
+        response = self.ew3.eulith_service.create_draft_client_whitelist_v2(request)
+        return response["list_id"]
+
+    def append_to_draft_client_whitelist(
+        self, auth_address: str, addresses: List[str], chain_id: Optional[int] = None
+    ) -> int:
+        """
+        DEPRECATED: Use append_to_draft_client_whitelist_v2 instead.
+        """
+        raise EulithDeprecationException(
+            "This method has been removed. Use append_to_draft_client_whitelist_v2 instead."
         )
-        raise_if_error(json_rpc)
-        return cast(whitelists_v2.rpc.CreateResponse, json_rpc["result"])
 
     def append_to_draft_client_whitelist_v2(
-        self, request: whitelists_v2.rpc.AppendRequest
-    ) -> whitelists_v2.rpc.AppendResponse:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_append_to_draft_client_whitelist_v2"), [request]
-        )
-        raise_if_error(json_rpc)
-        return cast(whitelists_v2.rpc.AppendResponse, json_rpc["result"])
-
-    def publish_client_whitelist(
-        self, request: whitelists_v2.rpc.PublishRequest
-    ) -> whitelists_v2.rpc.PublishResponse:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_publish_whitelist"), [request]
+        self, list_id: int, addresses: List[whitelists_v2.AddressOnChain]
+    ) -> whitelists_v2.Whitelist:
+        """
+        Appends to an existing draft, or otherwise creates a new draft whitelist if no draft currently exists
+
+        :param list_id: The ID of the list to append to.
+        :param addresses: The list of addresses to include on the whitelist.
+        """
+        request = whitelists_v2.rpc.AppendRequest(list_id=list_id, addresses=addresses)
+        response = self.ew3.eulith_service.append_to_draft_client_whitelist_v2(request)
+        return response["draft"]
+
+    def submit_draft_client_whitelist_signature(
+        self, list_id: int, signer: Signer
+    ) -> bool:
+        raise EulithDeprecationException(
+            "This method has been removed. Use submit_activate_whitelist_signature instead."
         )
-        raise_if_error(json_rpc)
-        return cast(whitelists_v2.rpc.PublishResponse, json_rpc["result"])
+
+    def get_current_client_whitelist(
+        self, auth_address: str, chain_id: Optional[int] = None
+    ) -> CurrentWhitelists:
+        raise EulithDeprecationException(
+            "This method has been removed. Use get_whitelist_by_id instead."
+        )
+
+    def publish_client_whitelist(self, list_id: int) -> whitelists_v2.Whitelist:
+        request = whitelists_v2.rpc.PublishRequest(list_id=list_id)
+        response = self.ew3.eulith_service.publish_client_whitelist(request)
+        return response["published"]
 
     def start_activate_whitelist(
-        self, request: whitelists_v2.rpc.StartActivateRequest
+        self, list_id: int, auth_address: str, safe_address: str, chain_id: int
     ) -> whitelists_v2.rpc.StartActivateResponse:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_start_activate_whitelist"), [request]
+        request = whitelists_v2.rpc.StartActivateRequest(
+            list_id=list_id,
+            auth_address=auth_address,
+            safe_address=safe_address,
+            chain_id=chain_id,
         )
-        raise_if_error(json_rpc)
-        return cast(whitelists_v2.rpc.StartActivateResponse, json_rpc["result"])
+        return self.ew3.eulith_service.start_activate_whitelist(request)
 
     def submit_activate_whitelist_signature(
-        self, request: whitelists_v2.rpc.SubmitActivateSignatureRequest
+        self, signer: Signer, activate_request: whitelists_v2.rpc.StartActivateResponse
     ) -> whitelists_v2.rpc.SubmitActivateSignatureResponse:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_submit_activate_whitelist_signature"), [request]
-        )
-        raise_if_error(json_rpc)
-        return cast(
-            whitelists_v2.rpc.SubmitActivateSignatureResponse, json_rpc["result"]
+        typed_data_payload = ActivateHashInputEip712(
+            activate_request["hash_input"]
+        ).typed_data()
+        signature = signer.sign_typed_data(
+            typed_data_payload, HexBytes(activate_request["hash"])
         )
+        serialized_signature = normalize_signature(signature)
 
-    def get_whitelist_by_id(
-        self, request: whitelists_v2.rpc.GetByIdRequest
-    ) -> whitelists_v2.rpc.GetByIdResponse:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_get_whitelist_by_id"), [request]
-        )
-        raise_if_error(json_rpc)
-        return cast(whitelists_v2.rpc.GetByIdResponse, json_rpc["result"])
-
-    def delete_draft_client_whitelist_v2(
-        self, request: whitelists_v2.rpc.DeleteRequest
-    ) -> whitelists_v2.rpc.DeleteResponse:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_delete_draft_client_whitelist_v2"), [request]
+        request = whitelists_v2.rpc.SubmitActivateSignatureRequest(
+            activation_id=activate_request["activation_id"],
+            signer_address=signer.address,
+            signature=serialized_signature,
+            hash=activate_request["hash"],
         )
-        raise_if_error(json_rpc)
-        return cast(whitelists_v2.rpc.DeleteResponse, json_rpc["result"])
+        return self.ew3.eulith_service.submit_activate_whitelist_signature(request)
+
+    def get_whitelist_by_id(self, list_id: int) -> whitelists_v2.Whitelist:
+        """
+        Retrieve a whitelist by its ID.
+        """
+        request = whitelists_v2.rpc.GetByIdRequest(list_id=list_id)
+        response = self.ew3.eulith_service.get_whitelist_by_id(request)
+        return response["whitelist"]
+
+    def delete_draft_client_whitelist_v2(self, list_id: int) -> whitelists_v2.Whitelist:
+        """
+        Delete a draft client whitelist.
+
+        :param list_id: The ID of the whitelist, as returned by `create_draft_client_whitelist_v2`.
+
+        :return: the whitelist that was deleted
+        """
+        request = whitelists_v2.rpc.DeleteRequest(list_id=list_id)
+        response = self.ew3.eulith_service.delete_draft_client_whitelist_v2(request)
+        return response["deleted"]
 
     def propose_light_simulation(
         self, safe_address: str, chain_id: int, to_enable: bool
-    ) -> (dict, dict):
-        try:
-            params = dict(
-                safe_address=safe_address, chain_id=chain_id, to_enable=to_enable
-            )
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_propose_light_simulation"), [params]
-            )
-            raise_if_error(response)
-            return response["result"], {}
-        except EulithRpcException as e:
-            return None, RPCResponse(error=str(e))
+    ) -> LightSimulationProposal:
+        """
+        Propose that light simulation be enabled/disabled for transactions on the Safe.
 
-    def get_light_simulation_proposal_hash(self, proposal_id: int) -> (dict, dict):
-        try:
-            params = dict(proposal_id=proposal_id)
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_get_light_simulation_proposal_hash"), [params]
-            )
-            raise_if_error(response)
-            return response["result"], {}
-        except EulithRpcException as e:
-            return None, RPCResponse(error=str(e))
+        The proposal must be approved by a threshold of Safe owners, using `submit_light_simulation_signature`.
+
+        :param safe_address: the Safe
+        :param chain_id: the chain the Safe is deployed on
+        :param to_enable: True to enable, False to disable
+        :return: the proposal
+        """
+        response = self.ew3.eulith_service.propose_light_simulation(
+            safe_address, chain_id, to_enable
+        )
+        return LightSimulationProposal.from_json(response["proposal"])
 
     def submit_light_simulation_signature(
-        self, proposal_id: int, owner_address: str, signature: str, signed_hash: str
-    ) -> (dict, dict):
-        try:
-            params = dict(
-                proposal_id=proposal_id,
-                owner_address=owner_address,
-                signature=signature,
-                signed_hash=signed_hash,
-            )
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_submit_light_simulation_proposal_signature"),
-                [params],
-            )
-            raise_if_error(response)
-            return response["result"], {}
-        except EulithRpcException as e:
-            return None, RPCResponse(error=str(e))
+        self, signer: Signer, proposal_id: int
+    ) -> LightSimulationSubmitResponse:
+        """
+        Submit a Safe owner's approval for a light simulation proposal.
 
-    def get_active_light_simulation_proposals(self) -> (dict, dict):
-        try:
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_get_active_light_simulation_proposals"), []
-            )
-            raise_if_error(response)
-            return response["result"], {}
-        except EulithRpcException as e:
-            return None, RPCResponse(error=str(e))
+        A threshold of Safe owners must approve the proposal for it to go into effect.
 
-    def delete_light_simulation_proposal(self, proposal_id: int) -> (dict, dict):
-        try:
-            params = dict(proposal_id=proposal_id)
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_delete_light_simulation_proposal"), [params]
-            )
-            raise_if_error(response)
-            return response["result"], {}
-        except EulithRpcException as e:
-            return None, RPCResponse(error=str(e))
+        :param signer: a Safe owner
+        :param proposal_id: the ID of the proposal, as returned by `propose_light_simulation`
+        :return: the proposal and whether it was approved
+        """
+        hash_response = self.ew3.eulith_service.get_light_simulation_proposal_hash(
+            proposal_id
+        )
 
-    def get_accepted_enable_armor_signatures(
-        self, auth_address: str
-    ) -> (List[AcceptedEnableArmorSignature], dict):
-        try:
-            params = {
-                "auth_address": auth_address,
-            }
+        hash_input = LightSimulationHashInput.from_json(hash_response["hash_input"])
+        typed_data_payload = hash_input.typed_data()
+        signature = signer.sign_typed_data(
+            typed_data_payload, HexBytes(hash_response["hash"])
+        )
+        serialized_signature = normalize_signature(signature)
 
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_get_enable_module_sigs"), [params]
-            )
-            raise_if_error(response)
-            return response["result"], {}
-        except EulithRpcException as e:
-            return None, RPCResponse(error=str(e))
-
-    def dydx_v3_get_ace_managed_accounts(
-        self, ace_address: str
-    ) -> (List[DydxV3AceManagedAccount], dict):
-        try:
-            params = {
-                "ace_address": ace_address,
-            }
+        response = self.ew3.eulith_service.submit_light_simulation_signature(
+            proposal_id, signer.address, serialized_signature, hash_response["hash"]
+        )
+        return LightSimulationSubmitResponse.from_json(response)
 
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_dydx_v3_get_ace_managed_accounts"), [params]
-            )
-            raise_if_error(response)
-            return response["result"], {}
-        except EulithRpcException as e:
-            return None, RPCResponse(error=str(e))
+    def get_active_light_simulation_proposals(self) -> List[LightSimulationProposal]:
+        """
+        Get all active light simulation proposals for the user.
 
-    def dydx_v3_create_order(
-        self,
-        order: DyDxV3CreateOrderParams,
-        signature: Union[Signature, str],
-        ace_address: str,
-    ):
-        try:
-            params = {
-                "ace_address": ace_address,
-                "signature": str(signature),
-                "order": order,
-            }
+        Active proposals are those that are neither deleted nor approved. Proposals start in the 'active' state.
 
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_dydx_v3_create_order"), [params]
-            )
+        :return: the list of proposals
+        """
+        response = self.ew3.eulith_service.get_active_light_simulation_proposals()
+        return [LightSimulationProposal.from_json(p) for p in response["proposals"]]
 
-            raise_if_error(response)
-            return response["result"], {}
-        except EulithRpcException as e:
-            return None, RPCResponse(error=str(e))
-
-    def dydx_v3_get_for_account(
-        self, ace_address: str, dydx_account_name: str, data: str
-    ):
-        try:
-            params = {
-                "ace_address": ace_address,
-                "account_name": dydx_account_name,
-                "data": data,
-            }
+    def delete_light_simulation_proposal(
+        self, proposal_id: int
+    ) -> LightSimulationProposal:
+        """
+        Delete a light simulation proposal.
 
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_dydx_v3_get_for_account"), [params]
-            )
+        :param proposal_id: the ID of the proposal to delete
+        :return: the deleted proposal
+        """
+        response = self.ew3.eulith_service.delete_light_simulation_proposal(proposal_id)
+        return LightSimulationProposal.from_json(response["proposal"])
 
-            raise_if_error(response)
-            return response["result"], {}
-        except EulithRpcException as e:
-            return None, RPCResponse(error=str(e))
+    def get_accepted_enable_armor_signatures(
+        self, auth_address: str
+    ) -> List[AcceptedEnableArmorSignature]:
+        """
+        Retrieve the current draft and published versions of the user's client whitelist.
 
-    def get_gmx_v2_tickers(self):
-        try:
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_gmx_v2_ticker_lookup"), []
-            )
-            raise_if_error(response)
-            return response["result"], {}
-        except EulithRpcException as e:
-            return None, RPCResponse(error=str(e))
+        :param auth_address: The authorized trading address of the armor to query
 
-    def get_gmx_v2_funding_rates(self):
-        try:
-            response = self.eulith_provider.make_request(
-                RPCEndpoint("eulith_gmx_v2_funding_rate_lookup"), []
-            )
-            raise_if_error(response)
-            return response["result"], {}
-        except EulithRpcException as e:
-            return None, RPCResponse(error=str(e))
-
-    def gmx_v2_get_positions(
-        self, request: GmxV2GetPositionsRequest
-    ) -> GmxV2GetPositionsResponse:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_gmx_v2_get_positions"), [request]
-        )
-        raise_if_error(json_rpc)
-        return cast(GmxV2GetPositionsResponse, json_rpc["result"])
-
-    def gmx_v2_create_order(
-        self, request: GmxV2CreateOrderRequest
-    ) -> GmxV2CreateOrderResponse:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_gmx_v2_create_order"), [request]
-        )
-        raise_if_error(json_rpc)
-        return cast(GmxV2CreateOrderResponse, json_rpc["result"])
-
-    def gmx_v2_get_market_pool_data(
-        self, request: GmxV2GetMarketPoolDataRequest
-    ) -> GmxV2GetMarketPoolDataResponse:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_gmx_v2_get_market_pool_data"), [request]
-        )
-        raise_if_error(json_rpc)
-        return cast(GmxV2GetMarketPoolDataResponse, json_rpc["result"])
-
-    def gmx_v2_create_deposit(
-        self, request: GmxV2CreateDepositRequest
-    ) -> GmxV2CreateDepositResponse:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_gmx_v2_create_deposit"), [request]
-        )
-        raise_if_error(json_rpc)
-        return cast(GmxV2CreateDepositResponse, json_rpc["result"])
-
-    def hyperliquid_get_data(self, request: HyperliquidGetDataRequest) -> Dict:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_hyperliquid_get_data"), [request]
+        :return: A list of all the currently accepted enable armor signatures
+        """
+        return self.ew3.eulith_service.get_accepted_enable_armor_signatures(
+            auth_address
         )
-        raise_if_error(json_rpc)
-        return cast(Dict, json_rpc["result"])
 
-    def hyperliquid_create_order(
-        self,
-        order_params: HyperliquidCreateOrderHashInput,
-        signature: str,
-        ace_address: str,
-    ):
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_hyperliquid_create_order"),
-            [
-                {
-                    "create_order_instruction": order_params.to_json(),
-                    "signature": signature,
-                    "ace_address": ace_address,
-                }
-            ],
-        )
-        raise_if_error(json_rpc)
-        return cast(Dict, json_rpc["result"])
+    def ping_ace(self, auth_address: str) -> AcePingResponse:
+        """
+        Ping the ACE server associated with the current auth address.
+        """
+        return self.ew3.eulith_service.ping_ace(auth_address)
 
-    def hyperliquid_cancel_order(
-        self,
-        order_params: HyperliquidCreateOrderHashInput,
-        signature: str,
-        ace_address: str,
-    ):
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_hyperliquid_cancel_order"),
-            [
-                {
-                    "cancel_order_instruction": order_params.to_json(),
-                    "signature": signature,
-                    "ace_address": ace_address,
-                }
-            ],
-        )
-        raise_if_error(json_rpc)
-        return cast(Dict, json_rpc["result"])
-
-    def ping_ace(self, auth_address: str) -> (AcePingResponse, dict):
-        params = {
-            "auth_address": auth_address,
-        }
-        response = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_ping_ace"), [params]
-        )
-        raise_if_error(response)
-        return response["result"], {}
-
-    def send_ace_transaction(
-        self, signature: str, ace_immediate_tx: AceImmediateTx
-    ) -> (HexStr, dict):
-        params = {
-            "signature": signature,
-            "immediate_tx": ace_immediate_tx.to_json(),
-        }
+    def subscribe_pending_transactions(
+        self, handler: EulithWebsocketRequestHandler
+    ) -> None:
+        """
+        Subscribe to pending transactions in the mempool.
 
-        response = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_send_ace_transaction"), [params]
-        )
-        raise_if_error(response)
-        return response["result"], {}
+        Note: only supported for ETH Mainnet and Polygon Mainnet.
+        """
+        subscription_request = SubscribeRequest(args=["newPendingTransactions"])
 
-    def pendle_swap(
-        self,
-        sell_token: Union[EulithERC20, PendleMarketSymbol],
-        buy_token: Union[EulithERC20, PendleMarketSymbol],
-        sell_amount: float,
-        slippage: float,
-        pendle_market: ChecksumAddress,
-        recipient: Optional[ChecksumAddress] = None,
-    ):
-        sell_token = (
-            sell_token.address
-            if isinstance(sell_token, EulithERC20)
-            else sell_token.value
-        )
-        buy_token = (
-            buy_token.address if isinstance(buy_token, EulithERC20) else buy_token.value
-        )
+        self.ew3.eulith_service.subscribe(subscription_request, handler)
 
-        params = {
-            "sell_token": sell_token,
-            "buy_token": buy_token,
-            "sell_amount": sell_amount,
-            "slippage_tolerance": slippage,
-            "market": pendle_market,
-        }
+    def check_tx_receipt_diag(self, tx_receipt: TxReceipt) -> None:
+        if tx_receipt["status"] != ETHEREUM_STATUS_SUCCESS:
+            self.ew3.eulith_service.eulith_provider.make_request(
+                RPCEndpoint("trace_transaction"), [tx_receipt["transactionHash"].hex()]
+            )
+            hash = tx_receipt["transactionHash"].hex()
+            raise EulithRpcException(f"transaction reverted ({hash})")
 
-        if recipient:
-            params["recipient"] = recipient
 
-        if self.atomic_params:
-            self.atomic_params.inject_in_body(params)
+def eulith_atomic_middleware(
+    make_request: Callable[[RPCEndpoint, Any], Any], web3: "Web3"
+) -> Callable[[RPCEndpoint, Any], RPCResponse]:
+    def middleware(method: RPCEndpoint, params: Any) -> RPCResponse:
+        if method != "eth_sendTransaction" or (
+            isinstance(web3, EulithWeb3) and not web3.is_atomic()
+        ):
+            resp = make_request(method, params)
+            raise_if_error(resp)
+            return resp
 
-        res = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_pendle_swap"), [params]
-        )
-        raise_if_error(res)
+        return cast(EulithWeb3, web3)._eulith_send_atomic(params)
 
-        return res
+    return middleware
 
-    def tx_bundle(self, request: BundleRequest) -> TxParams:
-        json_rpc = self.eulith_provider.make_request(
-            RPCEndpoint("eulith_tx_bundle"), [request]
-        )
-        raise_if_error(json_rpc)
-        return cast(TxParams, json_rpc["result"])
 
-    def get_subscriptions(self):
-        return self.eulith_provider.active_subscriptions
+class AtomicContextManager:
+    def __init__(self, ew3: EulithWeb3) -> None:
+        self.ew3 = ew3
 
-    def subscribe(
-        self,
-        subscription_request: SubscribeRequest,
-        handler: EulithWebsocketRequestHandler,
-    ) -> SubscriptionHandle:
-        return self.eulith_provider.subscribe(subscription_request, handler)
+    def __enter__(self) -> None:
+        pass
 
-    def terminate(self):
-        self.eulith_provider.terminate()
+    def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
+        # ok to unconditionally rollback because it's a no-op if already committed
+        self.ew3.v0.rollback_atomic_transaction()
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/exceptions.py` & `eulith_web3-0.27.0/src/eulith_web3/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Any
+
+
 class EulithAuthException(Exception):
     pass
 
 
 class EulithRpcException(Exception):
     pass
 
@@ -14,14 +17,14 @@
     pass
 
 
 class EulithNoSignerException(Exception):
     pass
 
 
-def guard_non_safe_atomic(ew3):
+def guard_non_safe_atomic(ew3: Any) -> None:
     if ew3.is_atomic() and "gnosis_address" not in str(ew3.eulith_service.eulith_url):
         raise EulithUnsafeRequestException(
             "calling this method in an atomic "
             "transaction without a Safe exposes you to "
             "leaving funds in your toolkit contract accidentally"
         )
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/fireblocks.py` & `eulith_web3-0.27.0/src/eulith_web3/fireblocks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
+from typing import Optional
 
 from eth_keys.backends import NativeECCBackend, BaseECCBackend
 from eth_keys.datatypes import PublicKey, Signature
 from eth_utils import big_endian_to_int
-from fireblocks_sdk import FireblocksSDK, RawMessage, UnsignedMessage
+from fireblocks_sdk import FireblocksSDK, RawMessage, UnsignedMessage  # type: ignore
 
 from hexbytes import HexBytes
 
 from eulith_web3.signing import SigningException
 from eulith_web3.signer import Signer
 
 logger = logging.getLogger(__name__)
@@ -18,35 +19,38 @@
 
 class FireblocksSigner(Signer):
     def __init__(
         self,
         api_private_key: str,
         api_key: str,
         vault_acct_id: int,
-        api_base_url="https://api.fireblocks.io",
-        backend: BaseECCBackend = NativeECCBackend,
-    ):
+        api_base_url: str = "https://api.fireblocks.io",
+        backend: Optional[BaseECCBackend] = None,
+    ) -> None:
+        if backend is None:
+            backend = NativeECCBackend()
+
         self.fireblocks = FireblocksSDK(
             api_private_key, api_key, api_base_url=api_base_url
         )
         self.vault_acct_id = vault_acct_id
         self.derivation_path = "[44,60," + str(vault_acct_id) + ",0,0]"
         pub_key = self.fireblocks.get_public_key_info(
             ALGO, self.derivation_path, COMPRESSED
         )
         actual_pk = PublicKey(HexBytes(pub_key["publicKey"][2:]), backend)
         self.public_address = actual_pk.to_checksum_address()
         logger.info("Fireblocks signer for ethereum address %s", self.public_address)
         self.backend = backend
 
     @property
-    def address(self):
+    def address(self) -> str:
         return self.public_address
 
-    def sign_msg_hash(self, message_hash: bytes) -> "Signature":
+    def sign_msg_hash(self, message_hash: bytes) -> Signature:
         raw = RawMessage(
             [
                 UnsignedMessage(
                     message_hash.hex(),
                     derivationPath=[44, 60, self.vault_acct_id, 0, 0],
                 )
             ],
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/gmx/v1/v1.py` & `eulith_web3-0.27.0/src/eulith_web3/gmx/v1/v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import List, Optional
+from typing import Any, Dict, List, Optional, Tuple, Union
 
-from eth_typing import ChecksumAddress
-from web3.types import TxParams, TxReceipt
+from eth_typing import Address, ChecksumAddress
+from web3 import Web3
+from web3.types import TxParams, TxReceipt, Wei
 
 from eulith_web3.contract_bindings.gmx.i_glp_manager import IGlpManager
 from eulith_web3.contract_bindings.gmx.i_order_book import IOrderBook
 from eulith_web3.contract_bindings.gmx.i_position_router import IPositionRouter
 from eulith_web3.contract_bindings.gmx.i_reader import IReader
 from eulith_web3.contract_bindings.gmx.i_reward_router import IRewardRouter
 from eulith_web3.contract_bindings.gmx.i_reward_tracker import IRewardTracker
@@ -16,48 +17,31 @@
 
 
 class GMXV1Position:
     """
     A class that represents a GMX position.
 
     :param from_dict: A dictionary that contains position data from the Eulith server.
-    :type from_dict: dict
 
     :ivar collateral_token_address: The address of the collateral token.
-    :vartype collateral_token_address: Optional[str]
-
     :ivar index_token_address: The address of the index token.
-    :vartype index_token_address: Optional[str]
-
     :ivar is_long: True if the position is long, False if it is short.
-    :vartype is_long: Optional[bool]
-
     :ivar position_size_denom_usd: The size of the position in USD.
-    :vartype position_size_denom_usd: Optional[float]
-
     :ivar collateral_size_denom_usd: The size of the collateral in USD.
-    :vartype collateral_size_denom_usd: Optional[float]
-
     :ivar entry_price_denom_usd: The entry price of the position in USD.
-    :vartype entry_price_denom_usd: Optional[float]
-
     :ivar realized_pnl: The realized profit and loss of the position in USD.
-    :vartype realized_pnl: Optional[float]
-
     :ivar has_profit: True if the position has profit, False otherwise.
-    :vartype has_profit: Optional[bool]
-
     :ivar liquidation_price_denom_usd: The liquidation price of the position in USD.
-    :vartype liquidation_price_denom_usd: Optional[float]
-
     :ivar current_delta_denom_usd: The current delta of the position in USD.
-    :vartype current_delta_denom_usd: Optional[float]
     """
 
-    def __init__(self, from_dict: dict):
+    def __init__(self, from_dict: Dict[Any, Any]) -> None:
+        """
+        :param from_dict: A dictionary that contains position data from the Eulith server.
+        """
         self.collateral_token_address: Optional[str] = None
         self.index_token_address: Optional[str] = None
         self.is_long: Optional[bool] = None
         self.position_size_denom_usd: Optional[float] = None
         self.collateral_size_denom_usd: Optional[float] = None
         self.entry_price_denom_usd: Optional[float] = None
         self.realized_pnl: Optional[float] = None
@@ -66,202 +50,170 @@
         self.current_delta_denom_usd: Optional[float] = None
 
         for key, val in from_dict.items():
             setattr(self, key, val)
 
 
 class GmxV1Client:
-    def __init__(self, ew3):
+    def __init__(self, ew3: Any) -> None:
+        """
+        :type ew3: EulithWeb3
+        """
         self.addresses = None
         self.price_precision_decimals = 30
         self.ew3 = ew3
 
     def get_address(self, address_key: str) -> str:
         if self.addresses is None:
             self.addresses = self.ew3.v0.get_gmx_addresses()
 
-        return self.addresses.get(address_key, "")
+        return self.addresses.get(address_key, "")  # type: ignore
 
     def get_router(self) -> IRouter:
         """
         Gets an instance of `IRouter` that provides access to the GMX Router Contract.
-
-        :return: An instance of `IRouter`.
-        :rtype: IRouter
         """
         router_address = self.ew3.to_checksum_address(self.get_address("router"))
         gmx_router = IRouter(self.ew3, router_address)
         return gmx_router
 
     def get_vault(self) -> IVault:
         """
         Gets an instance of `IVault` that provides access to the GMX Vault Contract.
-
-        :return: An instance of `IVault`.
-        :rtype: IVault
         """
         vault_address = self.ew3.to_checksum_address(self.get_address("vault"))
         vault = IVault(self.ew3, vault_address)
         return vault
 
     def get_reader(self) -> IReader:
         """
         Gets an instance of `IReader` that provides access to the GMX Reader Contract.
-
-        :return: An instance of `IReader`.
-        :rtype: IReader
         """
         reader_address = self.ew3.to_checksum_address(self.get_address("reader"))
         reader = IReader(self.ew3, reader_address)
         return reader
 
     def get_reward_tracker(self) -> IRewardTracker:
         """
         Gets an instance of `IRewardTracker` that provides access to the GMX RewardTracker contract.
-
-        :return: An instance of IRewardTracker.
-        :rtype: IRewardTracker
         """
         reward_tracker_address = self.ew3.to_checksum_address(
             self.get_address("reward_tracker")
         )
         reward_tracker = IRewardTracker(self.ew3, reward_tracker_address)
         return reward_tracker
 
     def get_position_router(self) -> IPositionRouter:
         """
         Returns an instance of the `IPositionRouter` that provides access to the GMX PositionRouter contract.
-
-        :return: An instance of `IPositionRouter`.
-        :rtype: IPositionRouter
         """
         position_router_address = self.ew3.to_checksum_address(
             self.get_address("position_router")
         )
         pr = IPositionRouter(self.ew3, position_router_address)
         return pr
 
     def get_reward_router(self) -> IRewardRouter:
         """
         Returns an instance of the `IRewardRouter` that provides access to the GMX RewardRouter contract.
-
-        :return: An instance of `IRewardRouter`.
-        :rtype: IRewardRouter
         """
         rra = self.ew3.to_checksum_address(self.get_address("reward_router"))
         rr = IRewardRouter(self.ew3, rra)
         return rr
 
     def get_glp_manager(self) -> IGlpManager:
         """
         Returns an instance of the `IGlpManager` that provides access to the GMX GLPManager contract.
-
-        :return: An instance of `GlpManager`
-        :rtype: IGlpManager
         """
         glp_manager_address = self.ew3.to_checksum_address(
             self.get_address("glp_manager")
         )
         gm = IGlpManager(self.ew3, glp_manager_address)
         return gm
 
     def get_orderbook(self) -> IOrderBook:
         """
         Returns an instance of the `IOrderBook` that provides access to the GMX OrderBook contract.
-
-        :return: An instance of `IOrderBook`
-        :rtype: IOrderBook
         """
         ob_address = self.ew3.to_checksum_address(self.get_address("orderbook"))
         ob = IOrderBook(self.ew3, ob_address)
         return ob
 
-    def get_dollar_denominated_token_amt(
-        self, token: EulithERC20, amount: float
-    ) -> float:
+    def get_dollar_denominated_token_amt(self, token: EulithERC20, amount: float) -> float:
         """
         Get the dollar-denominated amount of a given token amount on GMX.
 
         :param token: The token to convert.
-        :type token: EulithERC20
         :param amount: The amount of the token to convert.
-        :type amount: float
         :return: The dollar-denominated value of the token, returned in whole float units.
-        :rtype: float
         """
         vault = self.get_vault()
         full_int_amount = int(amount * 10 ** token.decimals())
-        token_usd_min = vault.token_to_usd_min(token.address, full_int_amount)
+        token_usd_min = vault.token_to_usd_min(_ensure_address(token.address), full_int_amount)
         return token_usd_min / 10**self.price_precision_decimals
 
-    def ensure_approved_plugin(self, plugin_address: ChecksumAddress) -> str:
+    def ensure_approved_plugin(self, plugin_address: ChecksumAddress) -> Optional[str]:
         """
         Ensures the specified plugin is approved by the GMX router. If not, it sends a transaction to approve it.
 
         :param plugin_address: The address of the plugin to be approved.
-        :type plugin_address: ChecksumAddress
         :return: The hexadecimal representation of the transaction hash if approval was necessary.
-        :rtype: str
         """
         gmx_router = self.get_router()
 
         if not gmx_router.approved_plugins(self.ew3.wallet_address, plugin_address):
             approve_plugin_tx = gmx_router.approve_plugin(
                 plugin_address, {"from": self.ew3.wallet_address, "gas": 5000000}
             )
             h = self.ew3.eth.send_transaction(approve_plugin_tx)
             if not self.ew3.is_atomic():
                 self.ew3.eth.wait_for_transaction_receipt(h)
 
             return h.hex()
+        else:
+            return None
 
-    def ensure_approved_position_router_plugin(self) -> str:
+    def ensure_approved_position_router_plugin(self) -> Optional[str]:
         """
         Ensures that the PositionRouter contract is an approved plugin on the router for the current wallet address.
 
         :return: A string representing the transaction hash of the approval transaction, if a new approval was required.
-        :rtype: str
         """
         pr = self.get_position_router()
-        return self.ensure_approved_plugin(pr.address)
+        return self.ensure_approved_plugin(_ensure_address_checksum(pr.address))
 
-    def ensure_approved_orderbook_plugin(self) -> str:
+    def ensure_approved_orderbook_plugin(self) -> Optional[str]:
         """
         Ensures the orderbook plugin is approved by the GMX router. If not, it sends a transaction to approve it.
 
         :return: The hexadecimal representation of the transaction hash if approval was necessary.
-        :rtype: str
         """
         ob = self.get_orderbook()
-        return self.ensure_approved_plugin(ob.address)
+        return self.ensure_approved_plugin(_ensure_address_checksum(ob.address))
 
     def get_max_ask_price(self, token: EulithERC20) -> float:
         """
         Get the maximum ask price for the given token in USD.
 
         :param token: An instance of the EulithERC20 class representing the token.
-        :type token: EulithERC20
         :return: The maximum ask price in USD.
-        :rtype: float
         """
         vault = self.get_vault()
-        max_price = vault.get_max_price(token.address)
+        max_price = vault.get_max_price(_ensure_address(token.address))
         return max_price / 10**self.price_precision_decimals
 
     def get_min_bid_price(self, token: EulithERC20) -> float:
         """
         Returns the minimum bid price for a given token.
 
         :param token: An instance of the EulithERC20 class representing the token.
-        :type token: EulithERC20
         :return: The minimum bid price for the given token in USD
-        :rtype: float
         """
         vault = self.get_vault()
-        min_price = vault.get_min_price(token.address)
+        min_price = vault.get_min_price(_ensure_address(token.address))
         return min_price / 10**self.price_precision_decimals
 
     def get_positions(
         self,
         wallet: ChecksumAddress,
         collateral_tokens: List[EulithERC20],
         index_tokens: List[EulithERC20],
@@ -269,194 +221,160 @@
     ) -> List[GMXV1Position]:
         """
         Returns a list of GMXPosition objects representing the positions for the specified wallet.
         The returned list matches the order of the collateral_token, index_token, and is_long tuples
         passed in their respective lists.
 
         :param wallet: The Ethereum wallet address to get the positions for.
-        :type wallet: ChecksumAddress
         :param collateral_tokens: A list of EulithERC20 tokens that the positions are collateralized with.
-        :type collateral_tokens: List[EulithERC20]
         :param index_tokens: A list of EulithERC20 tokens that the positions track.
-        :type index_tokens: List[EulithERC20]
         :param is_long: A list of boolean values indicating whether the positions are long or short.
-        :type is_long: List[bool]
         :return: A list of GMXPosition objects representing the positions for the specified wallet.
-        :rtype: List[GMXV1Position]
-        :raises EulithRpcException: If there was an error fetching the positions.
         """
-        status, res = self.ew3.eulith_service.get_gmx_positions(
+        result = self.ew3.eulith_service.get_gmx_positions(
             wallet, collateral_tokens, index_tokens, is_long
         )
-        if status:
-            positions = res.get("positions", [])
-            return_positions = []
-            for p in positions:
-                return_positions.append(GMXV1Position(p))
+        positions = result.get("positions", [])
+        return_positions = []
+        for p in positions:
+            return_positions.append(GMXV1Position(p))
 
-            return return_positions
-        else:
-            raise EulithRpcException(res)
+        return return_positions
 
     def mint_glp(
         self, pay_in: EulithERC20, pay_amount: float, slippage: Optional[float] = None
-    ) -> (float, float, List[TxParams]):
+    ) -> Tuple[float, float, List[TxParams]]:
         """
         Mint and stake GLP tokens for a given token and amount.
 
         :param pay_in: The token to pay with.
-        :type pay_in: EulithERC20
         :param pay_amount: The amount of the token to pay with.
-        :type pay_amount: float
         :param slippage: Optional slippage in percentage units i.e. slippage = 0.01 == 1%.
-        :type slippage: Optional[float]
         :return: A tuple of minimum GLP, minimum USD value, and a list of transactions to be executed.
-        :rtype: Tuple[float, float, List[TxParams]]
-        :raises EulithRpcException: If there is an error in the RPC response.
         """
-        status, res = self.ew3.eulith_service.request_gmx_mint_glp(
+        result = self.ew3.eulith_service.request_gmx_mint_glp(
             pay_in, pay_amount, slippage
         )
-        if status:
-            if len(res) > 0:
-                r = res[0]
-                txs = r.get("txs")
-                for t in txs:
-                    t["from"] = self.ew3.wallet_address
-                min_usd_value = r.get("min_usd_value")
-                min_glp = r.get("min_glp")
-                return min_glp, min_usd_value, txs
-            else:
-                raise EulithRpcException(
-                    "mint and stake glp returned empty list response"
-                )
+        if len(result) > 0:
+            r = result[0]
+            txs = r.get("txs")
+            for t in txs:
+                t["from"] = self.ew3.wallet_address
+            min_usd_value = r.get("min_usd_value")
+            min_glp = r.get("min_glp")
+            return min_glp, min_usd_value, txs
         else:
-            raise EulithRpcException(res)
+            raise EulithRpcException("mint and stake glp returned empty list response")
 
     def redeem_glp(
         self,
         receive_token: EulithERC20,
         glp_amount: float,
         min_receive_token: Optional[float] = None,
         receiving_address: Optional[ChecksumAddress] = None,
     ) -> TxParams:
         """
         Redeems GLP tokens for an equivalent value of `receive_token`.
 
         :param receive_token: The token to receive in exchange for GLP.
-        :type receive_token: EulithERC20
         :param glp_amount: The amount of GLP tokens to redeem.
-        :type glp_amount: float
         :param min_receive_token: The minimum amount of `receive_token` to receive.
-        :type min_receive_token: Optional[float]
         :param receiving_address: The address to receive the `receive_token`. Defaults to the current wallet address.
-        :type receiving_address: Optional[ChecksumAddress]
         :return: A dictionary containing transaction parameters.
-        :rtype: TxParams
         """
         rr = self.get_reward_router()
         glp_amount_int = int(glp_amount * 10**18)
         min_receive_int = int(min_receive_token * 10 ** receive_token.decimals())
 
         if not receiving_address:
             receiving_address = self.ew3.wallet_address
 
         tx = rr.unstake_and_redeem_glp(
-            receive_token.address,
+            _ensure_address(receive_token.address),
             glp_amount_int,
             min_receive_int,
-            receiving_address,
+            _ensure_address(receiving_address),
             {"from": self.ew3.wallet_address, "gas": 1500000},
         )
 
         return tx
 
     def get_dollar_denom_glp_value(self) -> float:
         """
         Get the dollar-denominated value of one GLP.
 
         :return: The dollar-denominated value of one GLP.
-        :rtype: float
         """
         glp_manager = self.get_glp_manager()
         price = glp_manager.get_price(False)
         return price / 10**self.price_precision_decimals
 
     def get_staked_glp_balance(self, wallet_address: ChecksumAddress) -> float:
         """
         Get the amount of staked GLP for the given wallet address.
 
         :param wallet_address: The wallet address to check the staked GLP balance for.
-        :type wallet_address: ChecksumAddress
         :return: The amount of staked GLP for the given wallet address.
-        :rtype: float
         """
         reward_tracker = self.get_reward_tracker()
         balance = reward_tracker.balance_of(wallet_address)
         return balance / 10**18  # 18 magic number here is the token decimal value
 
     # The fee is whole units denominated in the buy_token. For example on a swap from WETH to USDC, fee = 0.04
     # means 0.04 USDC is being taken as a fee
     # Swap fees are 0.2% - 0.8% https://gmxio.gitbook.io/gmx/trading
     def swap(
         self,
         sell_token: EulithERC20,
         buy_token: EulithERC20,
         amount_in: float,
         slippage: float = 0.01,
-        recipient: ChecksumAddress = None,
+        recipient: Optional[ChecksumAddress] = None,
         approve_erc: bool = False,
-    ) -> (float, float, TxParams):
+    ) -> Tuple[float, float, TxParams]:
         """
         Executes a swap between two tokens using the current router.
 
         :param sell_token: The token to sell.
-        :type sell_token: EulithERC20
         :param buy_token: The token to buy.
-        :type buy_token: EulithERC20
         :param amount_in: The amount of sell_token to sell in whole float units.
-        :type amount_in: float
         :param slippage: The acceptable slippage for the trade, expressed as decimal percentage defaults to 0.01 == 1%
-        :type slippage: float
         :param recipient: The address to send the purchased tokens to. Defaults to the calling wallet address.
-        :type recipient: ChecksumAddress
         :param approve_erc: If True, do the necessary pre-requisite ERC20 approvals automatically
-        :type approve_erc: bool
         :return: A tuple of the swap price, fee amount and transaction parameters.
                  The fee is whole units denominated in the buy_token
-        :rtype: tuple
         """
         router = self.get_router()
         reader = self.get_reader()
         vault = self.get_vault()
 
         amount_in_int = int(amount_in * 10 ** sell_token.decimals())
 
         router_allowance = sell_token.allowance_float(
-            self.ew3.wallet_address, router.address
+            self.ew3.wallet_address, _ensure_address(router.address)
         )
 
         if approve_erc and router_allowance < amount_in:
             self._approve_erc(amount_in - router_allowance, sell_token)
 
         out_amount, fee = reader.get_amount_out(
-            vault.address, sell_token.address, buy_token.address, amount_in_int
+            vault.address, _ensure_address(sell_token.address), _ensure_address(buy_token.address), amount_in_int
         )
         out_amount_float = out_amount / 10 ** buy_token.decimals()
 
         min_amount_out = int((1 - slippage) * out_amount)
 
         if not recipient:
             recipient = self.ew3.wallet_address
 
         tx_params = router.swap(
-            [sell_token.address, buy_token.address],
+            [_ensure_address(sell_token.address), _ensure_address(buy_token.address)],
             amount_in_int,
             min_amount_out,
-            recipient,
+            _ensure_address(recipient),
             {"from": self.ew3.wallet_address, "gas": 2000000},
         )
 
         price = amount_in / out_amount_float
 
         float_fee = fee / 10 ** buy_token.decimals()
 
@@ -472,29 +390,21 @@
         limit_price_usd: float,
         approve_erc: bool = True,
     ) -> Optional[TxReceipt]:
         """
         Creates an increase order (buy limit order) for a given position token, paid with a specified pay token.
 
         :param position_token: The token for which the position will be increased.
-        :type position_token: EulithERC20
         :param pay_token: The token to be used for payment.
-        :type pay_token: EulithERC20
         :param true_for_long: True for a long position, false for a short one.
-        :type true_for_long: bool
         :param amount_in: The amount of pay token to be used.
-        :type amount_in: float
         :param size_delta_usd: The change in position size in USD (whole float values i.e. 1.0 = 1 USD).
-        :type size_delta_usd: float
         :param limit_price_usd: The limit price in USD for the order. The order will execute at or below this price (for long positions).
-        :type limit_price_usd: float
         :param approve_erc: If True, approves the ERC20 token for the transaction.
-        :type approve_erc: bool, optional
         :return: The transaction receipt if the order was created successfully.
-        :rtype: Optional[TxReceipt]
         """
 
         guard_non_safe_atomic(self.ew3)
 
         self.ensure_approved_orderbook_plugin()
 
         ob = self.get_orderbook()
@@ -506,31 +416,31 @@
 
         pr = self.get_position_router()
         fee = pr.min_execution_fee()
 
         if approve_erc:
             self._approve_erc(amount_in_int, pay_token)
 
-        path = [pay_token.address]
+        path = [_ensure_address(pay_token.address)]
 
         trigger_above_threshold = not true_for_long
 
         order_tx = ob.create_increase_order(
             path,
             amount_in_int,
-            position_token.address,
+            _ensure_address(position_token.address),
             0,
             size_delta_int,
-            position_token.address,
+            _ensure_address(position_token.address),
             true_for_long,
             limit_price_int,
             trigger_above_threshold,
             fee,
             False,
-            {"from": self.ew3.wallet_address, "gas": 20000000, "value": fee},
+            {"from": self.ew3.wallet_address, "gas": 20000000, "value": Wei(fee)},
         )
 
         return self._send_and_wait_if_not_atomic(order_tx)
 
     def create_decrease_order(
         self,
         position_token: EulithERC20,
@@ -541,27 +451,20 @@
         limit_price_usd: float,
     ) -> Optional[TxReceipt]:
         """
         Creates a decrease order (sell limit order) for a given position/collateral pair. In most cases, the collateral
         token will be the same as the permission token unless you specifically have an otherwise collateralized position.
 
         :param position_token: The token for which the position will be decreased.
-        :type position_token: EulithERC20
         :param collateral_token: The collateral token to be decreased by `collateral_delta_usd`
-        :type collateral_token: EulithERC20
         :param size_delta_usd: The size delta in USD for the position.
-        :type size_delta_usd: float
         :param collateral_delta_usd: The collateral delta in USD for the position.
-        :type collateral_delta_usd: float
         :param true_for_long: True for a long position, false for a short one.
-        :type true_for_long: bool
         :param limit_price_usd: The limit price in USD for the order. The order will be executed at or above this price (for long positions).
-        :type limit_price_usd: float
         :return: The transaction receipt if the order was created successfully.
-        :rtype: Optional[TxReceipt]
         """
 
         guard_non_safe_atomic(self.ew3)
 
         size_delta_int = int(size_delta_usd * 10**self.price_precision_decimals)
         collateral_delta_int = int(
             collateral_delta_usd * 10**self.price_precision_decimals
@@ -575,22 +478,22 @@
 
         ob = self.get_orderbook()
 
         pr = self.get_position_router()
         fee = pr.min_execution_fee()
 
         order_tx = ob.create_decrease_order(
-            position_token.address,
+            _ensure_address(position_token.address),
             size_delta_int,
-            collateral_token.address,
+            _ensure_address(collateral_token.address),
             collateral_delta_int,
             true_for_long,
             limit_price_int,
             trigger_above_threshold,
-            {"from": self.ew3.wallet_address, "gas": 5000000, "value": fee},
+            {"from": self.ew3.wallet_address, "gas": 5000000, "value": Wei(fee)},
         )
 
         return self._send_and_wait_if_not_atomic(order_tx)
 
     def increase_position(
         self,
         position_token: EulithERC20,
@@ -600,27 +503,20 @@
         leverage: float = 1.0,
         approve_erc: bool = True,
     ) -> Optional[TxReceipt]:
         """
         Increases a GMX position.
 
         :param position_token: The position token to be manipulated.
-        :type position_token: EulithERC20
         :param collateral_token: The token to use for collateral.
-        :type collateral_token: EulithERC20
         :param true_for_long: If True, the position is a long position. Otherwise, it is a short position.
-        :type true_for_long: bool
         :param collateral_amount_in: The amount of collateral to add to the position.
-        :type collateral_amount_in: float
         :param leverage: The leverage to use. Default is 1.0.
-        :type leverage: float
         :param approve_erc: If True, do the necessary pre-requisite ERC20 approvals automatically
-        :type approve_erc: bool
         :return: If successful, returns a transaction receipt. Otherwise, returns None.
-        :rtype: Optional[TxReceipt]
         """
         self.ensure_approved_position_router_plugin()
 
         token_usd_min = int(
             self.get_dollar_denominated_token_amt(
                 collateral_token, collateral_amount_in
             )
@@ -629,15 +525,15 @@
         )
 
         full_int_amount = int(collateral_amount_in * 10 ** collateral_token.decimals())
 
         pr = self.get_position_router()
         fee = pr.min_execution_fee()
 
-        increase_position_path = [collateral_token.address]
+        increase_position_path = [_ensure_address(collateral_token.address)]
         zero_address = "0x0000000000000000000000000000000000000000"
 
         if true_for_long:
             acceptable_price = int(
                 self.get_max_ask_price(position_token)
                 * 10**self.price_precision_decimals
             )
@@ -648,54 +544,47 @@
             )
 
         if approve_erc:
             self._approve_erc(collateral_amount_in, collateral_token)
 
         increase_position_tx = pr.create_increase_position(
             increase_position_path,
-            position_token.address,
+            _ensure_address(position_token.address),
             full_int_amount,
             0,
             token_usd_min,
             true_for_long,
             acceptable_price,
             fee,
             b"00000000000000000000000000000000",
             zero_address,
-            {"from": self.ew3.wallet_address, "gas": 5000000, "value": fee},
+            {"from": self.ew3.wallet_address, "gas": 5000000, "value": Wei(fee)},
         )
 
         return self._send_and_wait_if_not_atomic(increase_position_tx)
 
     def decrease_position(
         self,
         position_token: EulithERC20,
         collateral_token: EulithERC20,
         true_for_long: bool,
         decrease_collateral: float,
         decrease_exposure: float,
-        recipient: str = None,
+        recipient: Optional[str] = None,
     ) -> Optional[TxReceipt]:
         """
         Decreases an existing position.
 
         :param position_token: The position token to decrease.
-        :type position_token: EulithERC20
         :param collateral_token: The collateral token.
-        :type collateral_token: EulithERC20
         :param true_for_long: True if the position is long, False if short.
-        :type true_for_long: bool
         :param decrease_collateral: The amount of collateral to decrease.
-        :type decrease_collateral: float
         :param decrease_exposure: The amount of position token to decrease.
-        :type decrease_exposure: float
         :param recipient: The address to receive the returned tokens. Defaults to the wallet address.
-        :type recipient: str, optional
         :return: The transaction receipt if the transaction was successful, otherwise None.
-        :rtype: Optional[TxReceipt]
         """
         self.ensure_approved_position_router_plugin()
 
         collateral_change = int(
             self.get_dollar_denominated_token_amt(collateral_token, decrease_collateral)
             * 10**self.price_precision_decimals
         )
@@ -704,15 +593,15 @@
             self.get_dollar_denominated_token_amt(position_token, decrease_exposure)
             * 10**self.price_precision_decimals
         )
 
         pr = self.get_position_router()
         fee = pr.min_execution_fee()
 
-        decrease_path = [collateral_token.address]
+        decrease_path = [_ensure_address(collateral_token.address)]
         zero_address = "0x0000000000000000000000000000000000000000"
 
         if true_for_long:
             acceptable_price = int(
                 self.get_max_ask_price(position_token)
                 * 10**self.price_precision_decimals
             )
@@ -723,38 +612,54 @@
             )
 
         if not recipient:
             recipient = self.ew3.wallet_address
 
         decrease_position_tx = pr.create_decrease_position(
             decrease_path,
-            position_token.address,
+            _ensure_address(position_token.address),
             collateral_change,
             size_change,
             true_for_long,
-            recipient,
+            recipient,  # type: ignore
             acceptable_price,
             0,
             fee,
             False,
             zero_address,
-            {"from": self.ew3.wallet_address, "gas": 5000000, "value": fee},
+            {"from": self.ew3.wallet_address, "gas": 5000000, "value": Wei(fee)},
         )
 
         return self._send_and_wait_if_not_atomic(decrease_position_tx)
 
     def _approve_erc(self, amount_in: float, input_token: EulithERC20) -> None:
         router_address = self.ew3.to_checksum_address(self.get_address("router"))
         at = input_token.approve_float(
             router_address, amount_in, {"from": self.ew3.wallet_address, "gas": 2000000}
         )
         h = self.ew3.eth.send_transaction(at)
         if not self.ew3.is_atomic():
             self.ew3.eth.wait_for_transaction_receipt(h)
 
-    def _send_and_wait_if_not_atomic(self, order_tx) -> Optional[TxReceipt]:
+    def _send_and_wait_if_not_atomic(self, order_tx: Any) -> Optional[TxReceipt]:
         h = self.ew3.eth.send_transaction(order_tx)
         if not self.ew3.is_atomic():
             r = self.ew3.eth.wait_for_transaction_receipt(h)
             return r
         else:
             return None
+
+
+def _ensure_address_checksum(address: Union[Address, ChecksumAddress, None]) -> ChecksumAddress:
+    if address is None:
+        raise ValueError("address is None")
+
+    if isinstance(address, bytes):
+        # address is Address
+        return Web3.to_checksum_address(address)
+    else:
+        # address is ChecksumAddress
+        return address
+
+
+def _ensure_address(address: Union[Address, ChecksumAddress, None]) -> str:
+    return str(_ensure_address_checksum(address))
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/gmx/v2/rpc.py` & `eulith_web3-0.27.0/src/eulith_web3/gmx/v2/rpc.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/gmx/v2/v2.py` & `eulith_web3-0.27.0/src/eulith_web3/gmx/v2/v2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from typing import List
-
-from eulith_web3.eulith_service import EulithService
+from eulith_web3.eulith_service import EulithService, JsonDict
 from eulith_web3.exceptions import EulithRpcException
 from eulith_web3.gmx.v2.rpc import (
     GmxV2CreateOrderRequest,
     GmxV2CreateOrderResponse,
     GmxV2GetPositionsRequest,
     GmxV2GetPositionsResponse,
 )
@@ -14,37 +12,29 @@
     GmxV2GetMarketPoolDataRequest,
     GmxV2CreateDepositRequest,
     GmxV2CreateDepositResponse,
 )
 
 
 class GmxV2Client:
-    def __init__(self, eulith_service: EulithService):
+    def __init__(self, eulith_service: EulithService) -> None:
         self.eulith_service = eulith_service
 
-    def get_tickers(self):
-        response, error = self.eulith_service.get_gmx_v2_tickers()
-        if error:
-            raise EulithRpcException(error)
-        return response
-
-    def get_funding_rates(self):
-        response, error = self.eulith_service.get_gmx_v2_funding_rates()
-        if error:
-            raise EulithRpcException(error)
-        return response
+    def get_tickers(self) -> JsonDict:
+        return self.eulith_service.get_gmx_v2_tickers()
+
+    def get_funding_rates(self) -> JsonDict:
+        return self.eulith_service.get_gmx_v2_funding_rates()
 
     def get_positions(self, account: str) -> GmxV2GetPositionsResponse:
         request = GmxV2GetPositionsRequest(account=account)
-        response = self.eulith_service.gmx_v2_get_positions(request)
-        return response
+        return self.eulith_service.gmx_v2_get_positions(request)
 
     def create_order(self, order: GmxV2CreateOrderRequest) -> GmxV2CreateOrderResponse:
-        response = self.eulith_service.gmx_v2_create_order(order)
-        return response
+        return self.eulith_service.gmx_v2_create_order(order)
 
     def get_market_pool_data(
         self, req: GmxV2GetMarketPoolDataRequest
     ) -> GmxV2GetMarketPoolDataResponse:
         return self.eulith_service.gmx_v2_get_market_pool_data(req)
 
     def create_deposit(
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/hyperliquid/_eip712.py` & `eulith_web3-0.27.0/src/eulith_web3/hyperliquid/_eip712.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,141 @@
 from dataclasses import dataclass
+from typing import Any, Dict
 
 from eth_account.messages import encode_typed_data
 from eth_utils import keccak
 
+from eulith_web3.eip712_types import Eip712Data, Eip712Domain, Eip712Field
+
 
 @dataclass
 class HyperliquidCreateOrderHashInput:
     coin: str
     is_buy: bool
     size: str
     limit_price: str
     time_in_force: str
     reduce_only: bool
     vault_address: str
 
     @classmethod
-    def from_json(cls, data: dict) -> "HyperliquidCreateOrderHashInput":
+    def from_json(cls, data: Dict[str, Any]) -> "HyperliquidCreateOrderHashInput":
         return cls(
             coin=data["coin"],
             is_buy=data["is_buy"],
             size=data["size"],
             limit_price=data["limit_price"],
             time_in_force=data["time_in_force"],
             reduce_only=data["reduce_only"],
             vault_address=data["vault_address"],
         )
 
-    def to_json(self) -> dict:
+    def to_json(self) -> Dict[str, Any]:
         return dict(
             coin=self.coin,
             is_buy=self.is_buy,
             size=self.size,
             limit_price=self.limit_price,
             time_in_force=self.time_in_force,
             reduce_only=self.reduce_only,
             vault_address=self.vault_address,
         )
 
 
 def get_hyper_liquid_create_order_typed_data(
     message: HyperliquidCreateOrderHashInput,
-) -> dict:
+) -> Eip712Data:
     types = {
         "EIP712Domain": [
-            {"name": "name", "type": "string"},
-            {"name": "version", "type": "string"},
+            Eip712Field(name="name", type="string"),
+            Eip712Field(name="version", type="string"),
         ],
         "HyperliquidCreateOrderHashInput": [
-            {"name": "coin", "type": "string"},
-            {"name": "isBuy", "type": "bool"},
-            {"name": "size", "type": "string"},
-            {"name": "limitPrice", "type": "string"},
-            {"name": "timeInForce", "type": "string"},
-            {"name": "reduceOnly", "type": "bool"},
-            {"name": "vaultAddress", "type": "string"},
+            Eip712Field(name="coin", type="string"),
+            Eip712Field(name="isBuy", type="bool"),
+            Eip712Field(name="size", type="string"),
+            Eip712Field(name="limitPrice", type="string"),
+            Eip712Field(name="timeInForce", type="string"),
+            Eip712Field(name="reduceOnly", type="bool"),
+            Eip712Field(name="vaultAddress", type="string"),
         ],
     }
 
-    payload = {
-        "types": types,
-        "primaryType": "HyperliquidCreateOrderHashInput",
-        "domain": {"name": "EulithAceHyperliquid", "version": "1"},
-        "message": {
+    payload = Eip712Data(
+        types=types,
+        primaryType="HyperliquidCreateOrderHashInput",
+        domain={"name": "EulithAceHyperliquid", "version": "1"},
+        message={
             "coin": message.coin,
             "isBuy": message.is_buy,
             "size": message.size,
             "limitPrice": message.limit_price,
             "timeInForce": message.time_in_force,
             "reduceOnly": message.reduce_only,
             "vaultAddress": message.vault_address,
         },
-    }
+    )
 
     return payload
 
 
 def get_hyper_liquid_create_order_hash(
     message: HyperliquidCreateOrderHashInput,
 ) -> bytes:
     signable_message = encode_typed_data(
-        full_message=get_hyper_liquid_create_order_typed_data(message)
+        full_message=dict(get_hyper_liquid_create_order_typed_data(message))
     )
     return keccak(b"\x19\x01" + signable_message.header + signable_message.body)
 
 
 @dataclass
 class HyperliquidCancelOrderHashInput:
     coin: str
     oid: str
     vault_address: str
 
     @classmethod
-    def from_json(cls, data: dict) -> "HyperliquidCancelOrderHashInput":
+    def from_json(cls, data: Dict[str, Any]) -> "HyperliquidCancelOrderHashInput":
         return cls(
             coin=data["coin"], oid=data["oid"], vault_address=data["vault_address"]
         )
 
-    def to_json(self) -> dict:
+    def to_json(self) -> Dict[str, Any]:
         return dict(coin=self.coin, oid=self.oid, vault_address=self.vault_address)
 
 
 def get_hyper_liquid_cancel_order_typed_data(
     message: HyperliquidCancelOrderHashInput,
-) -> dict:
+) -> Eip712Data:
     types = {
         "EIP712Domain": [
-            {"name": "name", "type": "string"},
-            {"name": "version", "type": "string"},
+            Eip712Field(name="name", type="string"),
+            Eip712Field(name="version", type="string"),
         ],
         "HyperliquidCancelOrderHashInput": [
-            {"name": "coin", "type": "string"},
-            {"name": "oid", "type": "string"},
-            {"name": "vaultAddress", "type": "string"},
+            Eip712Field(name="coin", type="string"),
+            Eip712Field(name="oid", type="string"),
+            Eip712Field(name="vaultAddress", type="string"),
         ],
     }
 
-    payload = {
-        "types": types,
-        "primaryType": "HyperliquidCancelOrderHashInput",
-        "domain": {"name": "EulithAceHyperliquid", "version": "1"},
-        "message": {
+    payload = Eip712Data(
+        types=types,
+        primaryType="HyperliquidCancelOrderHashInput",
+        domain=Eip712Domain(name="EulithAceHyperliquid", version="1"),
+        message={
             "coin": message.coin,
             "oid": message.oid,
             "vaultAddress": message.vault_address,
         },
-    }
+    )
 
     return payload
 
 
 def get_hyper_liquid_cancel_order_hash(
     message: HyperliquidCancelOrderHashInput,
 ) -> bytes:
     signable_message = encode_typed_data(
-        full_message=get_hyper_liquid_cancel_order_typed_data(message)
+        full_message=dict(get_hyper_liquid_cancel_order_typed_data(message))
     )
     return keccak(b"\x19\x01" + signable_message.header + signable_message.body)
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/hyperliquid/hyperliquid.py` & `eulith_web3-0.27.0/src/eulith_web3/hyperliquid/hyperliquid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Union, Optional
+from typing import Any, Dict, Union, Optional
 
 from eulith_web3.hyperliquid.rpc import (
     HyperliquidGetDataRequest,
     HyperliquidTimeInForce,
 )
 from eulith_web3.exceptions import EulithNoSignerException
 from eulith_web3.hyperliquid._eip712 import (
@@ -12,45 +12,52 @@
     get_hyper_liquid_create_order_typed_data,
     get_hyper_liquid_cancel_order_typed_data,
     get_hyper_liquid_cancel_order_hash,
 )
 
 from eulith_web3.signing import normalize_signature
 
+from eulith_web3.hyperliquid.rpc import HyperliquidGetHistoricalFundingRequest
+
 
 class HyperliquidClient:
     """
     A class that provides access to the GMX protocol.
 
     :param ew3: An instance of `EulithWeb3`.
     :type ew3: EulithWeb3
     """
 
-    def __init__(self, ew3):
+    def __init__(self, ew3: Any) -> None:
         self.ew3 = ew3
 
-    def get_data(self, request: HyperliquidGetDataRequest) -> Dict:
+    def get_data(self, request: HyperliquidGetDataRequest) -> Dict[str, Any]:
         parsed_request = {
             "account_address": request.get("account_address"),
-            "data_type": request.get("data_type").value,
+            "data_type": request["data_type"].value,
             "ace_address": request.get("ace_address"),
         }
         return self.ew3.eulith_service.hyperliquid_get_data(parsed_request)
 
+    def get_funding_rates(
+        self, request: HyperliquidGetHistoricalFundingRequest
+    ) -> Dict[str, Any]:
+        return self.ew3.eulith_service.hyperliquid_get_funding_rates(request)
+
     def create_order(
         self,
         coin: str,
         is_buy: bool,
         size: Union[float, str],
         limit_price: Union[float, str],
         time_in_force: HyperliquidTimeInForce,
         reduce_only: bool,
         ace_address: str,
         vault_address: Optional[str] = None,
-    ) -> Dict:
+    ) -> Dict[str, Any]:
         try:
             self.ew3.signer.sign_msg_hash(b"")
         except AttributeError:
             raise EulithNoSignerException(
                 "you must have a valid signer attached to your ew3 instance to create a hyperliquid order"
             )
 
@@ -68,26 +75,24 @@
         }
 
         hash_input = HyperliquidCreateOrderHashInput.from_json(hash_input_json)
 
         typed_data = get_hyper_liquid_create_order_typed_data(hash_input)
         message_hash = get_hyper_liquid_create_order_hash(hash_input)
 
-        print(f"message hash {message_hash.hex()}")
-
         signature = self.ew3.signer.sign_typed_data(typed_data, message_hash)
         signature_string = normalize_signature(signature)
 
         return self.ew3.eulith_service.hyperliquid_create_order(
             hash_input, signature_string, ace_address
         )
 
     def cancel_order(
         self, coin: str, oid: int, ace_address: str, vault_address: Optional[str] = None
-    ) -> Dict:
+    ) -> Dict[str, Any]:
         try:
             self.ew3.signer.sign_msg_hash(b"")
         except AttributeError:
             raise EulithNoSignerException(
                 "you must have a valid signer attached to your ew3 instance to create a hyperliquid order"
             )
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/hyperliquid/rpc.py` & `eulith_web3-0.27.0/src/eulith_web3/hyperliquid/rpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import TypedDict
+from typing import TypedDict, List
 
 from eulith_web3.hyperliquid._eip712 import (
     HyperliquidCreateOrderHashInput,
     HyperliquidCancelOrderHashInput,
 )
 
 
@@ -32,7 +32,25 @@
     order: HyperliquidCreateOrderHashInput
 
 
 class HyperliquidCancelOrderRequest(TypedDict):
     ace_address: str
     signature: str
     order: HyperliquidCancelOrderHashInput
+
+
+class HyperliquidGetHistoricalFundingRequest(TypedDict):
+    start_time: int
+    end_time: int
+    coin: str
+    ace_address: str
+
+
+class HyperliquidGetHistoricalFundingResponseInner(TypedDict):
+    coin: str
+    premium: str
+    time: int
+    funding_rate: str
+
+
+class HyperliquidGetHistoricalFundingResponse(TypedDict):
+    funding_rates: List[HyperliquidGetHistoricalFundingResponseInner]
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/kms.py` & `eulith_web3-0.27.0/src/eulith_web3/kms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import logging
 from pprint import pprint
-from typing import Any
+from typing import Any, Optional
 
-import asn1
-from botocore.exceptions import ClientError
+import asn1  # type: ignore
+from botocore.exceptions import ClientError  # type: ignore
 from eth_keys.backends import BaseECCBackend, NativeECCBackend
 from eth_keys.datatypes import PublicKey
 
 from eulith_web3.signing import recover_v
 from eulith_web3.signer import Signer
 from eth_keys.datatypes import Signature
 
 
 class KmsSigner(Signer):
     def __init__(
-        self, kms_client: Any, key_id: str, backend: BaseECCBackend = NativeECCBackend
+        self, kms_client: Any, key_id: str, backend: Optional[BaseECCBackend] = None
     ):
         self.key_id = key_id
         self.client = kms_client
-        self.backend = backend
+        self.backend = backend or NativeECCBackend()
         try:
             key = self.client.get_public_key(KeyId=key_id)
         except ClientError as err:
             logging.error(
                 "Couldn't get key '%s'. Here's why: %s",
                 key_id,
                 err.response["Error"]["Message"],
             )
             raise err
         pk_bytes = self.decode_pk(key["PublicKey"])
         self.public_address = PublicKey(pk_bytes, backend).to_checksum_address()
 
     @property
-    def address(self):
+    def address(self) -> str:
         return self.public_address
 
     def sign_msg_hash(self, message_hash: bytes) -> Signature:
         der_sig = self.client.sign(
             KeyId=self.key_id,
             Message=message_hash,
             MessageType="DIGEST",
@@ -45,29 +45,29 @@
         decoder = asn1.Decoder()
         decoder.start(der_sig["Signature"])
         decoder.enter()
         _, r = decoder.read()
         _, s = decoder.read()
         return recover_v(r, s, message_hash, self.address, self.backend)
 
-    def print_pk(self, key_id: str):
+    def print_pk(self, key_id: str) -> None:
         try:
             key = self.client.get_public_key(KeyId=key_id)
         except ClientError as err:
             logging.error(
                 "Couldn't get key '%s'. Here's why: %s",
                 key_id,
                 err.response["Error"]["Message"],
             )
         else:
             print(f"Got key {key_id}:")
             pprint(key)
 
     @staticmethod
-    def decode_pk(pk_bytes) -> bytes:
+    def decode_pk(pk_bytes: bytes) -> bytes:
         decoder = asn1.Decoder()
         decoder.start(pk_bytes)
         decoder.enter()
         decoder.enter()
         decoder.leave()
         tag, value = decoder.read()
         return value[1:]
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/ledger.py` & `eulith_web3-0.27.0/src/eulith_web3/ledger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 import re
+from typing import Any, Dict, Optional, Union
 
 from eth_account._utils.signing import to_standard_v
+from eth_account._utils.typed_transactions import TypedTransaction
 from eth_keys.backends import BaseECCBackend, NativeECCBackend
 from eth_keys.datatypes import Signature
 from web3.types import TxParams
 
+from eulith_web3.eip712_types import Eip712Data
 from eulith_web3.ledger_interface.account import get_ledger_accounts, get_signer_path
 from eulith_web3.ledger_interface.comms import init_dongle
 from eulith_web3.ledger_interface.exceptions import LedgerError
 from eulith_web3.ledger_interface.messages import ledger_sign_typed_data
 from eulith_web3.ledger_interface.objects import Type2Transaction, Type1Transaction
 from eulith_web3.ledger_interface.transactions import ledger_sign_transaction
 from eulith_web3.signer import Signer
 
 
-def camel_to_snake(name):
+def camel_to_snake(name: str) -> str:
     name = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", name)
     return re.sub("([a-z0-9])([A-Z])", r"\1_\2", name).lower()
 
 
 class LedgerSigner(Signer):
     def __init__(
-        self, account_index: int = 0, backend: BaseECCBackend = NativeECCBackend
+        self, account_index: int = 0, backend: Optional[BaseECCBackend] = None
     ):
-        self.backend = backend
+        self.backend = backend or NativeECCBackend()
         try:
             self.account = get_ledger_accounts()[account_index]
             self.dongle = init_dongle()
             self.signer_path = get_signer_path(account_index)
         except LedgerError:
             print("Could not communicate with your Ledger. Is it asleep?")
             exit(1)
 
     @property
     def address(self) -> str:
         return self.account.address
 
-    def sign_transaction(self, tx: TxParams, message_hash: bytes) -> Signature:
+    def sign_transaction(
+        self, tx: Union[TxParams, TypedTransaction], message_hash: bytes
+    ) -> Signature:
         formatted_tx = {}
-        tx_dict = tx.as_dict()
+        if isinstance(tx, TypedTransaction):
+            tx_dict = tx.as_dict()
+        else:
+            tx_dict = dict(tx)
+
         tx_type = tx_dict.get("type", 2)  # default to EIP 1559
 
         tx_dict.pop("type")
 
         for k, v in tx_dict.items():
             formatted_tx[camel_to_snake(k)] = v
 
@@ -59,12 +68,14 @@
 
         v = signature.v
         r = signature.r
         s = signature.s
 
         return Signature(vrs=(v, r, s))
 
-    def sign_typed_data(self, eip712_data: dict, message_hash: bytes) -> Signature:
+    def sign_typed_data(
+        self, eip712_data: Union[Eip712Data, Dict[str, Any]], message_hash: bytes
+    ) -> Signature:
         signature = ledger_sign_typed_data(
             eip712_data, dongle=self.dongle, sender_path=self.signer_path
         )
         return Signature(vrs=(to_standard_v(signature.v), signature.r, signature.s))
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/ledger_interface/account.py` & `eulith_web3-0.27.0/src/eulith_web3/ledger_interface/account.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/ledger_interface/comms.py` & `eulith_web3-0.27.0/src/eulith_web3/ledger_interface/comms.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/ledger_interface/constants.py` & `eulith_web3-0.27.0/src/eulith_web3/ledger_interface/constants.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/ledger_interface/exceptions.py` & `eulith_web3-0.27.0/src/eulith_web3/ledger_interface/exceptions.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/ledger_interface/messages.py` & `eulith_web3-0.27.0/src/eulith_web3/ledger_interface/messages.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/ledger_interface/objects.py` & `eulith_web3-0.27.0/src/eulith_web3/ledger_interface/objects.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/ledger_interface/transactions.py` & `eulith_web3-0.27.0/src/eulith_web3/ledger_interface/transactions.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/ledger_interface/utils.py` & `eulith_web3-0.27.0/src/eulith_web3/ledger_interface/utils.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/lightsim.py` & `eulith_web3-0.27.0/src/eulith_web3/lightsim.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from dataclasses import dataclass
+from typing import Any, Dict
+
+from eulith_web3.eip712_types import Eip712Data, Eip712Domain, Eip712Field
 
 
 @dataclass
 class LightSimulationProposal:
     proposal_id: int
     to_enable: bool
     safe_address: str
     network_id: int
     proposer_sub: str
     safe_owner_sub: str
     status: str
 
     @classmethod
-    def from_json(cls, j: dict) -> "LightSimulationProposal":
+    def from_json(cls, j: Dict[str, Any]) -> "LightSimulationProposal":
         return cls(**j)
 
 
 @dataclass
 class LightSimulationSubmitResponse:
     proposal: LightSimulationProposal
     approved: bool
 
     @classmethod
-    def from_json(cls, j: dict) -> "LightSimulationSubmitResponse":
+    def from_json(cls, j: Dict[str, Any]) -> "LightSimulationSubmitResponse":
         proposal = LightSimulationProposal.from_json(j["proposal"])
         approved = j["approved"]
         return cls(proposal=proposal, approved=approved)
 
 
 @dataclass
 class LightSimulationHashInput:
@@ -34,41 +37,41 @@
     chain_id: int
     proposer_id: int
     safe_owner_id: int
     to_enable: bool
     proposal_id: int
 
     @classmethod
-    def from_json(cls, j: dict) -> "LightSimulationHashInput":
+    def from_json(cls, j: Dict[str, Any]) -> "LightSimulationHashInput":
         return cls(**j)
 
-    def typed_data(self) -> dict:
+    def typed_data(self) -> Eip712Data:
         types = {
             "EIP712Domain": [
-                {"name": "name", "type": "string"},
-                {"name": "version", "type": "string"},
+                Eip712Field(name="name", type="string"),
+                Eip712Field(name="version", type="string"),
             ],
             "LightSimulationProposalHashInput": [
-                {"name": "safeAddress", "type": "string"},
-                {"name": "chainId", "type": "int32"},
-                {"name": "proposerId", "type": "int32"},
-                {"name": "safeOwnerId", "type": "int32"},
-                {"name": "toEnable", "type": "bool"},
-                {"name": "proposalId", "type": "int32"},
+                Eip712Field(name="safeAddress", type="string"),
+                Eip712Field(name="chainId", type="int32"),
+                Eip712Field(name="proposerId", type="int32"),
+                Eip712Field(name="safeOwnerId", type="int32"),
+                Eip712Field(name="toEnable", type="bool"),
+                Eip712Field(name="proposalId", type="int32"),
             ],
         }
 
-        payload = {
-            "types": types,
-            "primaryType": "LightSimulationProposalHashInput",
-            "domain": {"name": "EulithLightSimulationProposal", "version": "1"},
-            "message": {
+        payload = Eip712Data(
+            types=types,
+            primaryType="LightSimulationProposalHashInput",
+            domain=Eip712Domain(name="EulithLightSimulationProposal", version="1"),
+            message={
                 "safeAddress": self.safe_address,
                 "chainId": self.chain_id,
                 "proposerId": self.proposer_id,
                 "safeOwnerId": self.safe_owner_id,
                 "toEnable": self.to_enable,
                 "proposalId": self.proposal_id,
             },
-        }
+        )
 
         return payload
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/pendle.py` & `eulith_web3-0.27.0/src/eulith_web3/pendle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from enum import Enum
-from typing import Optional, Union
+from typing import Any, Dict, Optional, Union, cast
 
-import requests
 from eth_typing import ChecksumAddress
-from web3.types import TxParams, RPCEndpoint
+from web3.types import TxParams
 
 from eulith_web3.erc20 import EulithERC20
 from eulith_web3.exceptions import EulithRpcException
 
 
 class PendleClientException(Exception):
     pass
@@ -23,47 +22,46 @@
     :ivar implied_yield: The current implied yield (as of the last trade).
     :vartype implied_yield: Optional[float]
 
     :ivar sy_underlying_exchange_rate: The exchange rate of the underlying asset to the SY asset.
     :vartype sy_underlying_exchange_rate: Optional[float]
     """
 
-    def __init__(self, from_dict: dict):
+    def __init__(self, from_dict: Dict[Any, Any]) -> None:
         self.price_denom_underlying: Optional[float] = None
         self.implied_yield: Optional[float] = None
         self.sy_underlying_exchange_rate: Optional[float] = None
 
         for key, val in from_dict.items():
             setattr(self, key, val)
 
 
 class PendleSwap:
     """
     The PendleSwap class encapsulates response data from the Eulith server in convenient typed fields
 
-    :param ew3: The Eulith web3 instance.
-    :type ew3: EulithWeb3
-    :param from_dict: Response body from the Eulith Pendle Swap request
-    :type from_dict: dict
-
     :ivar sell_token: The token to be sold.
     :vartype sell_token: Optional[EulithERC20]
     :ivar buy_token: The token to be bought.
     :vartype buy_token: Optional[EulithERC20]
     :ivar sell_amount: The amount of sell token to be sold.
     :vartype sell_amount: Optional[float]
     :ivar buy_amount: The amount of buy token to be bought.
     :vartype buy_amount: Optional[float]
     :ivar approve_address: The ERC20 address you need to approve(sell_amount) for the swap to work
     :vartype approve_address: Optional[ChecksumAddress]
     :ivar tx: The transaction parameters.
     :vartype tx: Optional[TxParams]
     """
 
-    def __init__(self, ew3, from_dict: dict):
+    def __init__(self, ew3: Any, from_dict: Dict[Any, Any]):
+        """
+        :param ew3: The Eulith web3 instance.
+        :param from_dict: Response body from the Eulith Pendle Swap request
+        """
         self.sell_token: Optional[EulithERC20] = None
         self.buy_token: Optional[EulithERC20] = None
         self.sell_amount: Optional[float] = None
         self.buy_amount: Optional[float] = None
         self.approve_address: Optional[ChecksumAddress] = None
         self.tx: Optional[TxParams] = None
 
@@ -78,15 +76,17 @@
 
 class PendleMarketSymbol(str, Enum):
     PT = "pt"
     YT = "yt"
 
 
 class PendleClient:
-    def __init__(self, ew3, router_override: Optional[ChecksumAddress] = None):
+    def __init__(
+        self, ew3: Any, router_override: Optional[ChecksumAddress] = None
+    ) -> None:
         self.ew3 = ew3
 
         # Default address from https://docs.pendle.finance/Developers/DeployedContracts/Ethereum
         # Default address is true for both Ethereum and Arbitrum
         self.router = (
             router_override
             if router_override
@@ -98,71 +98,51 @@
     def quote_pt(
         self, buy_pt_amount: float, market_address: ChecksumAddress
     ) -> PendlePtQuote:
         """
         Get a quote for buying a certain amount of Pendle Token (PT) in exchange for underlying assets.
 
         :param buy_pt_amount: The amount of PT to buy.
-        :type buy_pt_amount: float
-
         :param market_address: The address of the Pendle market to buy PT from.
-        :type market_address: ChecksumAddress
 
         :return: A PendlePtQuote object containing the PT purchase quote.
-        :rtype: PendlePtQuote
-
-        :raises EulithRpcException: If there is an error while getting the PT quote.
         """
-        status, result = self.ew3.eulith_service.get_pt_quote(
-            buy_pt_amount, market_address
-        )
-        if status:
-            return PendlePtQuote(result)
-        else:
-            raise EulithRpcException(result)
+        result = self.ew3.eulith_service.get_pt_quote(buy_pt_amount, market_address)
+        return PendlePtQuote(result)
 
     def swap(
         self,
         sell_token: Union[EulithERC20, PendleMarketSymbol],
         buy_token: Union[EulithERC20, PendleMarketSymbol],
         sell_amount: float,
         slippage: float,
         pendle_market: ChecksumAddress,
         recipient: Optional[ChecksumAddress] = None,
     ) -> PendleSwap:
         """
         Retrieves pricing and transaction data needed to swap between two tokens in a given Pendle market.
 
         :param sell_token: The token to be sold.
-        :type sell_token: Union[EulithERC20, PendleMarketSymbol]
         :param buy_token: The token to be bought.
-        :type buy_token: Union[EulithERC20, PendleMarketSymbol]
         :param sell_amount: The amount of sell token to be sold.
-        :type sell_amount: float
         :param slippage: The acceptable slippage percentage for the swap, represented in float terms like 0.01 == 1%
-        :type slippage: float
         :param pendle_market: The Pendle market address where the swap will occur.
-        :type pendle_market: ChecksumAddress
         :param recipient: The address that will receive the bought tokens. If not provided, the wallet attached to EulithWeb3 will be used.
-        :type recipient: Optional[ChecksumAddress]
 
         :return: A PendleSwap object representing the executed swap.
-        :rtype: PendleSwap
-
-        :raises EulithRpcException: If no recipient is provided and no wallet is attached to EulithWeb3, or if the request fails.
         """
 
         try:
-            res = self.ew3.eulith_service.pendle_swap(
+            result = self.ew3.eulith_service.pendle_swap(
                 sell_token, buy_token, sell_amount, slippage, pendle_market, recipient
             )
-            result = res.get("result", {})
 
-            if self.ew3.wallet_address:
-                result["tx"]["from"] = self.ew3.wallet_address
+            wallet_address = cast(str, self.ew3.wallet_address)
+            if wallet_address:
+                result["tx"]["from"] = wallet_address
             else:
                 # The server returns None in the 'from' field.
                 # If we can't set it, we pop it out to avoid serialization issues with a None value
                 result["tx"].pop("from")
 
             return PendleSwap(self.ew3, result)
         except KeyError as e:
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/requests.py` & `eulith_web3-0.27.0/src/eulith_web3/requests.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3/response.py` & `eulith_web3-0.27.0/src/eulith_web3/response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from web3.types import RPCResponse, TxReceipt
 
 from eulith_web3.common import ETHEREUM_STATUS_SUCCESS
 from eulith_web3.exceptions import EulithRpcException
 
 
-def raise_if_error(resp: RPCResponse):
+def raise_if_error(resp: RPCResponse) -> None:
     """
     Checks if the resp object passed as an argument to the handle_rpc_response function contains a key 'error'.
     If the key 'error' exists in the dictionary 'resp' and if its value is not an empty string, we handle RPC response
     from the API and raise EulithRpcException
 
     :param resp: RPC response from the API
     :type resp: RPCResponse
@@ -16,11 +16,11 @@
     :raises EulithRpcException: If the 'error' field in the RPC response is not empty
     """
 
     if "error" in resp:
         raise EulithRpcException("RPC Error: " + str(resp.get("error")))
 
 
-def check_tx_receipt(tx_receipt: TxReceipt):
+def check_tx_receipt(tx_receipt: TxReceipt) -> None:
     if tx_receipt["status"] != ETHEREUM_STATUS_SUCCESS:
         hash = tx_receipt["transactionHash"].hex()
         raise EulithRpcException(f"transaction reverted ({hash})")
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/signing.py` & `eulith_web3-0.27.0/src/eulith_web3/signing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import logging
+from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Mapping,
+    Optional,
+    Tuple,
 )
 
-from cytoolz import dissoc
+from cytoolz import dissoc  # type: ignore
 from eth_account._utils.legacy_transactions import (
     serializable_unsigned_transaction_from_dict,
     UnsignedTransaction,
     Transaction,
     encode_transaction,
 )
-from eth_account._utils.signing import sign_transaction_dict, to_eth_v
+from eth_account._utils.signing import to_eth_v
 from eth_account._utils.typed_transactions import TypedTransaction
 from eth_account.datastructures import SignedTransaction
 from eth_keys.backends import NativeECCBackend, BaseECCBackend
 from eth_keys.datatypes import PrivateKey, Signature
 from eth_utils.toolz import (
     compose,
 )
@@ -93,15 +96,15 @@
     ):
         return sig1
     raise SigningException("Could not determine v")
 
 
 # signer has two functions: address, sign_msg_hash
 #    def sign_msg_hash(self, message_hash: bytes) -> 'Signature':
-def sign_transaction(transaction_dict, signer: Signer) -> SignedTransaction:
+def sign_transaction(transaction_dict: Any, signer: Signer) -> SignedTransaction:
     if not isinstance(transaction_dict, Mapping):
         raise TypeError("transaction_dict must be dict-like, got %r" % transaction_dict)
 
     # allow from field, *only* if it matches the private key
     if "from" in transaction_dict:
         if transaction_dict["from"] == signer.address:
             sanitized_transaction = dissoc(transaction_dict, "from")
@@ -125,15 +128,17 @@
         hash=HexBytes(transaction_hash),
         r=r,
         s=s,
         v=v,
     )
 
 
-def sign_transaction_dict(eth_key: Signer, transaction_dict):
+def sign_transaction_dict(
+    eth_key: Signer, transaction_dict: Any
+) -> Tuple[int, int, int, Any, bytes]:
     # generate RLP-serializable transaction, with defaults filled
     unsigned_transaction = serializable_unsigned_transaction_from_dict(transaction_dict)
     transaction_hash = unsigned_transaction.hash()
 
     # detect chain
     if isinstance(unsigned_transaction, UnsignedTransaction):
         signature = eth_key.sign_transaction(unsigned_transaction, transaction_hash)
@@ -158,26 +163,38 @@
     # serialize transaction with rlp
     encoded_transaction = encode_transaction(unsigned_transaction, vrs=(v, r, s))
 
     return v, r, s, encoded_transaction, transaction_hash
 
 
 class LocalSigner(Signer):
-    def __init__(self, private_key, backend: BaseECCBackend = NativeECCBackend):
-        self.private_key = PrivateKey(HexBytes(private_key), backend)
-        self.address = self.private_key.public_key.to_checksum_address()
+    def __init__(
+        self, private_key: Any, backend: Optional[BaseECCBackend] = None
+    ) -> None:
+        self.private_key = PrivateKey(
+            HexBytes(private_key), backend or NativeECCBackend()
+        )
+        self._address = self.private_key.public_key.to_checksum_address()
 
+    @property
     def address(self) -> str:
-        return self.address
+        return self._address
 
     def sign_msg_hash(self, message_hash: bytes) -> Signature:
         return self.private_key.sign_msg_hash(message_hash)
 
 
-def construct_signing_middleware(account: Signer) -> Middleware:
+@dataclass
+class EulithSigningMiddleware:
+    middleware: Middleware
+    address: str
+    signer: Signer
+
+
+def construct_signing_middleware(account: Signer) -> EulithSigningMiddleware:
     """
     Wrap signature source in middleware to allow for automatic signing when necessary for transactions
     being signed and sent directly to the network (as opposed to an atomic transaction, which gets sent
     unsigned to the Eulith server).
 
     :param account: The LocalSigner, KMSSigner, or FireblocksSigner for your wallet
     :type account: Signer
@@ -204,19 +221,17 @@
 
             raw_tx = sign_transaction(transaction, acct).rawTransaction
 
             return make_request(RPCEndpoint("eth_sendRawTransaction"), [raw_tx])
 
         return middleware
 
-    smw = sign_and_send_raw_middleware
-    smw.address = account.address
-    smw.signer = acct
-
-    return smw
+    return EulithSigningMiddleware(
+        middleware=sign_and_send_raw_middleware, address=account.address, signer=acct
+    )
 
 
 def normalize_signature(signature: Signature) -> str:
     """
     Normalize the signature to a string, for instance for serialization for an RPC method.
     """
     compatible_v = signature.v + 27
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/swap.py` & `eulith_web3-0.27.0/src/eulith_web3/swap.py`

 * *Files 25% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     SADDLE = "saddle"
     SHELL = "shell"
     SHIBA = "shiba"
     SYNAPSE = "synapse"
     SYNTHETIX = "synthetix"
 
 
-class EulithSwapRequest(TypedDict):
+class EulithSwapRequest(TypedDict, total=False):
     sell_token: EulithERC20
     buy_token: EulithERC20
     sell_amount: float
     recipient: Optional[ChecksumAddress]
     route_through: Optional[EulithSwapProvider]
     slippage_tolerance: Optional[float]
     liquidity_source: Optional[EulithLiquiditySource]
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/trezor.py` & `eulith_web3-0.27.0/src/eulith_web3/trezor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from typing import Optional
+from typing import Any, Dict, Union
 
+from eth_account._utils.typed_transactions import TypedTransaction
 from eth_keys.datatypes import Signature
 from trezorlib import ethereum
 from trezorlib.client import get_default_client
 from trezorlib.exceptions import TrezorException
 from trezorlib.tools import parse_path
 from web3.types import TxParams
 
+from eulith_web3.eip712_types import Eip712Data
 from eulith_web3.signer import Signer
 
 
-def bytes_to_str_in_eip712(data):
+def bytes_to_str_in_eip712(data: Any) -> Any:
     """
     Recursively converts all bytes fields to hex strings in a dictionary.
     """
     if isinstance(data, dict):
         # If the data is a dictionary, iterate over it
         return {k: bytes_to_str_in_eip712(v) for k, v in data.items()}
     elif isinstance(data, bytes):
@@ -30,45 +32,53 @@
 
 class TrezorSigner(Signer):
     """
     Signs EIP712 and transaction data with a Trezor.
     Note this requires a manual interaction with the connected device. This is NOT an automated signer
     """
 
-    def __init__(self, derivation_path: Optional[str] = "44'/60'/0'/0/0"):
+    def __init__(self, derivation_path: str = "44'/60'/0'/0/0"):
         self.client = get_default_client()
         self.derivation_path = parse_path(derivation_path)
         self.cached_address = str(
             ethereum.get_address(self.client, self.derivation_path, False, None)
         )
 
     @property
     def address(self) -> str:
         return self.cached_address
 
-    def sign_typed_data(self, eip712_data: dict, message_hash: bytes) -> Signature:
+    def sign_typed_data(
+        self, eip712_data: Union[Eip712Data, Dict[str, Any]], message_hash: bytes
+    ) -> Signature:
         formatted_d = bytes_to_str_in_eip712(eip712_data)
 
         signature = ethereum.sign_typed_data(
             self.client, self.derivation_path, formatted_d
         )
 
         signature_bytes = signature.signature.hex()
 
         returned_v = signature_bytes[-2:]
         formatted_v = "0" + hex(int(returned_v, 16) - 27)[2:]
 
         formatted_bytes = signature_bytes[:-2] + formatted_v
         return Signature(bytes.fromhex(formatted_bytes))
 
-    def sign_transaction(self, tx: TxParams, message_hash: bytes) -> Signature:
-        tx_dict = tx.as_dict()
-        value = tx_dict.get("value")
-        data = tx_dict.get("data")
-        to = tx_dict.get("to")
+    def sign_transaction(
+        self, tx: Union[TxParams, TypedTransaction], message_hash: bytes
+    ) -> Signature:
+        if isinstance(tx, TypedTransaction):
+            tx_dict = tx.as_dict()
+        else:
+            tx_dict = dict(tx)
+
+        value = tx_dict["value"]
+        data = tx_dict["data"]
+        to = tx_dict["to"]
 
         if isinstance(value, int):
             parsed_value = value
         else:
             parsed_value = int(value, 16)
 
         if isinstance(data, bytes):
@@ -86,33 +96,33 @@
         max_priority_per_gas = tx_dict.get("maxPriorityFeePerGas")
 
         if gas_price:
             signature = ethereum.sign_tx(
                 self.client,
                 self.derivation_path,
                 nonce=tx_dict.get("nonce", 0),
-                gas_price=tx_dict.get("gasPrice"),
-                gas_limit=tx_dict.get("gas"),
+                gas_price=gas_price,
+                gas_limit=tx_dict["gas"],
                 to=parsed_to,
                 value=parsed_value,
                 data=parsed_data,
-                chain_id=tx_dict.get("chainId"),
+                chain_id=tx_dict["chainId"],
             )
         elif max_per_gas and max_priority_per_gas:
             signature = ethereum.sign_tx_eip1559(
                 self.client,
                 self.derivation_path,
                 nonce=tx_dict.get("nonce", 0),
                 max_gas_fee=max_per_gas,
                 max_priority_fee=max_priority_per_gas,
-                gas_limit=tx_dict.get("gas"),
+                gas_limit=tx_dict["gas"],
                 to=parsed_to,
                 value=parsed_value,
                 data=parsed_data,
-                chain_id=tx_dict.get("chainId"),
+                chain_id=tx_dict["chainId"],
             )
         else:
             raise TrezorException(
                 "you must pass either gasPrice "
                 "OR maxFeePerGas AND maxPriorityFeePerGas "
                 "in your txParams to sign the tx with Trezor"
             )
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/uniswap.py` & `eulith_web3-0.27.0/src/eulith_web3/uniswap.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from enum import Enum
-from typing import Optional, TypedDict, Callable
+from typing import Any, Optional, Tuple, TypedDict
 
 from eth_account.messages import encode_structured_data
 from eth_typing import Address, ChecksumAddress
 from eth_utils import keccak
 
 from eulith_web3.common import INT_FEE_TO_FLOAT_DIVISOR
 from eulith_web3.contract_bindings.i_uniswap_v3_pool import IUniswapV3Pool
@@ -12,14 +12,16 @@
 from eulith_web3.exceptions import EulithRpcException
 from eulith_web3.websocket import (
     SubscribeRequest,
     SubscriptionHandle,
     EulithWebsocketRequestHandler,
 )
 
+from eulith_web3.eip712_types import Eip712Data, Eip712Domain, Eip712Field
+
 
 class UniswapPoolFee(int, Enum):
     FiveBips = 500
     ThirtyBips = 3000
     OneHundredBips = 10000
 
 
@@ -55,20 +57,20 @@
     token_b: EulithERC20
     fee: UniswapPoolFee
 
 
 class EulithUniswapV3Pool(IUniswapV3Pool):
     def __init__(
         self,
-        eulith_web3,
+        eulith_web3: Any,
         pool_address: ChecksumAddress,
         fee: Optional[UniswapPoolFee] = None,
         token0: Optional[ChecksumAddress] = None,
         token1: Optional[ChecksumAddress] = None,
-    ):
+    ) -> None:
         super().__init__(eulith_web3, pool_address)
         self.pool_fee = fee
         self.t0 = token0
         self.t1 = token1
         self.ew3 = eulith_web3
 
     def get_token_zero(self) -> EulithERC20:
@@ -83,29 +85,30 @@
             self.t1 = self.ew3.to_checksum_address(self.token1())
             return EulithERC20(self.ew3, self.t1)
         else:
             return EulithERC20(self.ew3, self.t1)
 
     def get_fee(self) -> UniswapPoolFee:
         if not self.pool_fee:
-            self.pool_fee = UniswapPoolFee(self.fee())
-            return self.pool_fee
+            r = UniswapPoolFee(self.fee())
+            self.pool_fee = r
+            return r
         else:
             return self.pool_fee
 
     # returns price (float), fee (float as percent: i.e. 0.001 = 0.1%), swap_request (EulithUniV3StartSwapRequest)
     def get_quote(
         self,
         sell_token: EulithERC20,
         amount: float,
         true_for_amount_in: Optional[bool] = True,
         fill_or_kill: Optional[bool] = True,
         recipient: Optional[ChecksumAddress] = None,
         pay_transfer_from: Optional[ChecksumAddress] = None,
-    ) -> (float, float, EulithUniV3StartSwapRequest):
+    ) -> Tuple[float, float, EulithUniV3StartSwapRequest]:
 
         if (
             sell_token.address != self.get_token_one().address
             and sell_token.address != self.get_token_zero().address
         ):
             raise EulithRpcException(
                 "cannot start swap on pool with no matching sell token, "
@@ -123,23 +126,19 @@
             sell_token=sell_token,
             buy_token=buy_token,
             amount=amount,
             fee=fee,
             true_for_amount_in=true_for_amount_in,
         )
 
-        status, res = self.ew3.eulith_service.uniswap_v3_quote(params)
-
-        if status:
-            price, fee, swap_request = self.ew3.parse_uni_quote_to_swap_request(
-                res, fill_or_kill, recipient, pay_transfer_from
-            )
-            return price, fee / INT_FEE_TO_FLOAT_DIVISOR, swap_request
-        else:
-            raise EulithRpcException(res)
+        result = self.ew3.eulith_service.uniswap_v3_quote(params)
+        price, fee, swap_request = self.ew3.parse_uni_quote_to_swap_request(
+            result, fill_or_kill, recipient, pay_transfer_from
+        )
+        return price, fee / INT_FEE_TO_FLOAT_DIVISOR, swap_request
 
     def subscribe_prices(
         self, handler: EulithWebsocketRequestHandler
     ) -> SubscriptionHandle:
         subscribe_request = SubscribeRequest(
             subscription_type="uni_prices", args={"pool_address": self.address}
         )
@@ -155,36 +154,36 @@
     tick_upper: int
     pool: Address
 
     def tx_hash(self) -> bytes:
         signable_message = encode_structured_data(self.typed_data())
         return keccak(b"\x19\x01" + signable_message.header + signable_message.body)
 
-    def typed_data(self) -> dict:
+    def typed_data(self) -> Eip712Data:
         types = {
             "EIP712Domain": [
-                {"name": "name", "type": "string"},
-                {"name": "version", "type": "string"},
+                Eip712Field(name="name", type="string"),
+                Eip712Field(name="version", type="string"),
             ],
             "AceUniBurnCollect": [
-                {"name": "chainId", "type": "int64"},
-                {"name": "liquidity", "type": "uint128"},
-                {"name": "tickLower", "type": "int32"},
-                {"name": "tickUpper", "type": "int32"},
-                {"name": "pool", "type": "address"},
+                Eip712Field(name="chainId", type="int64"),
+                Eip712Field(name="liquidity", type="uint128"),
+                Eip712Field(name="tickLower", type="int32"),
+                Eip712Field(name="tickUpper", type="int32"),
+                Eip712Field(name="pool", type="address"),
             ],
         }
 
-        payload = {
-            "types": types,
-            "primaryType": "AceUniBurnCollect",
-            "domain": {"name": "EulithAceUniBurnCollect", "version": "1"},
-            "message": {
+        payload = Eip712Data(
+            types=types,
+            primaryType="AceUniBurnCollect",
+            domain=Eip712Domain(name="EulithAceUniBurnCollect", version="1"),
+            message={
                 "chainId": self.chain_id,
                 "liquidity": self.liquidity,
                 "tickLower": self.tick_lower,
                 "tickUpper": self.tick_upper,
                 "pool": self.pool,
             },
-        }
+        )
 
         return payload
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/websocket.py` & `eulith_web3-0.27.0/src/eulith_web3/websocket.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,141 +2,150 @@
 import queue
 import random
 import threading
 import time
 from abc import ABC, abstractmethod
 from concurrent.futures import ThreadPoolExecutor
 from json import JSONDecodeError
-from typing import TypedDict, Any, Dict, Optional, Union
+from typing import TypedDict, Any, Dict, List, Optional, Tuple, Union, cast
 import logging
 
 import websocket
 from web3.providers import JSONBaseProvider
 from web3.types import RPCEndpoint, RPCResponse
 
 EULITH_SUBSCRIPTION_TYPES = ["uni_prices"]
 
 logger = logging.getLogger("eulith")
 
 
 class EulithWebsocketRequestHandler(ABC):
     @abstractmethod
-    def handle_result(self, message: Dict):
+    def handle_result(self, message: Dict[Any, Any]) -> Any:
         pass
 
     @abstractmethod
-    def handle_error(self, message: Dict):
+    def handle_error(self, message: Dict[Any, Any]) -> Any:
         pass
 
 
-class SubscribeRequest(TypedDict):
+class SubscribeRequest(TypedDict, total=False):
     # if you're using a eulith subscription, you should specify the type here, otherwise leave empty
     # note eth_subscribe requests do not have a subscription_type. These are non-eulith subscriptions
     subscription_type: Optional[str]
     # whatever arguments should be passed in the `params` field of the request
-    args: Union[dict, list]
+    args: Union[Dict[Any, Any], List[Any]]
 
 
 class EulithSyncResponse:
-    def __init__(self):
+    error: Optional[Exception]
+
+    def __init__(self) -> None:
         self.event = threading.Event()
         self.value = None
         self.error = None
 
-    def set_value(self, value):
+    def set_value(self, value: Any) -> None:
         self.value = value
         self.event.set()
 
-    def set_error(self, e: Exception):
+    def set_error(self, e: Exception) -> None:
         self.error = e
         self.event.set()
 
-    def get_value(self):
+    def get_value(self) -> Any:
         self.event.wait()
         if self.error is not None:
             raise self.error
 
         return self.value
 
 
 class SubscriptionDetails:
+    subscription_id: Optional[str]
+
     def __init__(
-        self, handler: EulithWebsocketRequestHandler, resubscribe_payload: Dict
-    ):
+        self,
+        handler: EulithWebsocketRequestHandler,
+        resubscribe_payload: Dict[Any, Any],
+    ) -> None:
         self.handler = handler
         self.subscription_id = None
         self.resubscribe_payload = resubscribe_payload
 
-    def handle_message(self, data):
+    def handle_message(self, data: Dict[Any, Any]) -> Any:
         return self.handler.handle_result(data)
 
-    def handle_error(self, data):
+    def handle_error(self, data: Dict[Any, Any]) -> Any:
         return self.handler.handle_error(data)
 
-    def set_subscription_id(self, sub_id: str):
+    def set_subscription_id(self, sub_id: str) -> None:
         self.subscription_id = sub_id
 
-    def get_resubscribe_payload(self):
+    def get_resubscribe_payload(self) -> Dict[Any, Any]:
         return self.resubscribe_payload
 
 
 class SubscriptionHandle:
-    def __init__(self, sub_details: SubscriptionDetails, eulith_service):
+    def __init__(self, sub_details: SubscriptionDetails, eulith_service: Any) -> None:
         self.sub_details = sub_details
         self.eulith_service = eulith_service
 
     def unsubscribe(self) -> bool:
         return self.eulith_service.unsubscribe(self.sub_details)
 
 
 class CouldNotConnectException(Exception):
     pass
 
 
 class ThreadSafeDict:
-    def __init__(self, initial_dict=None):
+    def __init__(self, initial_dict: Optional[Dict[Any, Any]] = None) -> None:
         self.lock = threading.Lock()
         self.internal = initial_dict or {}
 
-    def set(self, key, value):
+    def set(self, key: Any, value: Any) -> None:
         with self.lock:
             self.internal[key] = value
 
-    def get(self, key, default=None):
+    def get(self, key: Any, default: Any = None) -> Any:
         with self.lock:
             return self.internal.get(key, default)
 
-    def pop(self, key):
+    def pop(self, key: Any) -> Any:
         with self.lock:
             return self.internal.pop(key, None)
 
-    def get_and_clear(self):
+    def get_and_clear(self) -> Dict[Any, Any]:
         with self.lock:
             contents = self.internal.copy()
             self.internal.clear()
             return contents
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.internal)
 
-    def drain(self):
+    def drain(self) -> Dict[Any, Any]:
         with self.lock:
             copy = self.internal.copy()
             self.internal.clear()
             return copy
 
 
 class EulithWebsocketProvider(JSONBaseProvider):
+    send_queue: queue.Queue[Tuple[Dict[Any, Any], Any]]
+    termination_exception: Optional[Exception]
+
     def __init__(
         self,
-        uri,
+        uri: str,
         bearer_token: str,
         thread_pool_workers: int = 10,
         max_reconnect_attempts: int = 10,
-    ):
+    ) -> None:
         super().__init__()
 
         self.uri = uri
         self.connection = None
         self.thread_pool = ThreadPoolExecutor(
             max_workers=thread_pool_workers, thread_name_prefix="eulith_ws_worker"
         )
@@ -154,15 +163,15 @@
         self.awaiting_unsubscribe = ThreadSafeDict()
 
         self.max_reconnect_attempts = max_reconnect_attempts
 
         self.main_thread = threading.Thread(target=self.run)
         self.main_thread.start()
 
-    def run(self):
+    def run(self) -> None:
         while not self.shutdown_event.is_set():
             try:
                 to_reestablish = self.active_subscriptions.get_and_clear()
 
                 connection = self.connect()
 
                 send_thread = threading.Thread(
@@ -187,15 +196,15 @@
                 logger.error(f"Could not connect after retrying {ce}")
                 self.terminate()
             except Exception as e:
                 logger.error(f"Something unexpected happened: {e}")
                 self.termination_exception = e
                 self.terminate()
 
-    def connect(self):
+    def connect(self) -> Any:
         bearer_header = {"Authorization": f"Bearer {self.bearer}"}
 
         sleep = 1
         attempts = 0
 
         while attempts < self.max_reconnect_attempts:
             try:
@@ -205,24 +214,24 @@
             except ConnectionRefusedError:
                 time.sleep(random.uniform(0, sleep))
                 sleep *= 2
                 attempts += 1
 
         raise CouldNotConnectException()
 
-    def reestablish_subscriptions(self, to_reestablish: Dict):
+    def reestablish_subscriptions(self, to_reestablish: Dict[Any, Any]) -> None:
         for key, val in to_reestablish.items():
             resubscribe_payload = val.get_resubscribe_payload()
             if resubscribe_payload:
                 request_id = self.next_request_id()
                 resubscribe_payload["id"] = request_id
                 self.send_queue.put((resubscribe_payload, None))
                 self.awaiting_subscription_id.set(request_id, val)
 
-    def send_loop(self, connection):
+    def send_loop(self, connection: Any) -> None:
         """
         Runs on its own thread
         """
         while not self.shutdown_event.is_set():
             try:
                 request, response_handler = self.send_queue.get(timeout=1)
                 request_id = request.get("id")
@@ -235,15 +244,15 @@
                 continue  # timeout after 1 second to check the shutdown event
             except Exception as e:
                 logger.error(f"caught exception in eulith websocket send loop: {e}")
                 return
 
         connection.close()
 
-    def receive_loop(self, connection):
+    def receive_loop(self, connection: Any) -> None:
         """
         Runs on its own thread
         """
         while not self.shutdown_event.is_set():
             try:
                 message = connection.recv()
 
@@ -300,71 +309,70 @@
             raise CouldNotConnectException()
 
         response_handler = EulithSyncResponse()
         request_payload = self.get_request_payload(method, params)
         self.send_queue.put((request_payload, response_handler))
         return response_handler.get_value()
 
-    def next_request_id(self):
+    def next_request_id(self) -> int:
         with self.lock:
             self.request_id += 1
             return self.request_id
 
-    def terminate(self):
+    def terminate(self) -> None:
         self.shutdown_event.set()
         self.thread_pool.shutdown(False)
         self.drain_queue()
         self.drain_handlers()
 
-    def drain_queue(self):
+    def drain_queue(self) -> None:
         done = 0
         while done == 0:
             try:
                 request, response_handler = self.send_queue.get(timeout=1)
                 if response_handler:
                     if self.termination_exception is not None:
                         response_handler.set_error(self.termination_exception)
                     else:
                         response_handler.set_error(CouldNotConnectException())
             except queue.Empty:
                 done = 1
 
-    def drain_handlers(self):
+    def drain_handlers(self) -> None:
         for (
             request_id,
             response_handler,
         ) in self.awaiting_one_time_response.drain().items():
             if self.termination_exception is not None:
                 response_handler.set_error(self.termination_exception)
             else:
                 response_handler.set_error(CouldNotConnectException())
 
-    def restart(
-        self,
-    ):  # This method is only used in CI to test connection going up and down
+    def restart(self) -> None:
+        # This method is only used in CI to test connection going up and down
         self.shutdown_event.clear()
         self.main_thread = threading.Thread(target=self.run)
         self.main_thread.start()
         self.thread_pool = ThreadPoolExecutor(
             max_workers=2, thread_name_prefix="eulith_ws_worker"
         )
 
-    def get_unsubscribe_message(self, subscription_id: str) -> Dict:
+    def get_unsubscribe_message(self, subscription_id: str) -> Dict[str, Any]:
         rid = self.next_request_id()
         unsub_payload = {
             "jsonrpc": "2.0",
             "method": "eth_unsubscribe",
             "params": [subscription_id],
             "id": rid,
         }
         return unsub_payload
 
     def get_request_payload(
         self, method: RPCEndpoint, params: Any, rid: Optional[int] = None
-    ) -> Dict:
+    ) -> Dict[str, Any]:
         if not rid:
             rid = self.next_request_id()
 
         return {"id": rid, "method": str(method), "params": params, "jsonrpc": "2.0"}
 
     def subscribe(
         self,
@@ -374,39 +382,45 @@
         subscription_type = subscription_request.get("subscription_type", None)
         method = (
             "eulith_subscribe"
             if subscription_type in EULITH_SUBSCRIPTION_TYPES
             else "eth_subscribe"
         )
 
+        params: List[Any]
         if method == "eulith_subscribe":
             args = subscription_request.get("args", None)
+
+            sub_type_body: Any
             if args:
                 sub_type_body = {subscription_type: args}
             else:
                 sub_type_body = subscription_type
 
             params = [
                 {
                     "subscription_type": sub_type_body,
                 }
             ]
         else:
-            params = subscription_request.get("args", [])
+            params = cast(List[Any], subscription_request.get("args", []))
 
         request_message = self.get_request_payload(RPCEndpoint(method), params)
         rid = request_message.get("id")
 
         sub_details = SubscriptionDetails(handler, request_message)
         self.awaiting_subscription_id.set(rid, sub_details)
         self.send_queue.put((request_message, None))
 
         return SubscriptionHandle(sub_details, self)
 
     def unsubscribe(self, sub_details: SubscriptionDetails) -> bool:
+        if not sub_details.subscription_id:
+            raise ValueError("subscription_id is missing")
+
         unsub_payload = self.get_unsubscribe_message(sub_details.subscription_id)
         unsub_response = EulithSyncResponse()
 
         request_id = unsub_payload.get("id", None)
         if not request_id:
             return False
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/whitelists.py` & `eulith_web3-0.27.0/src/eulith_web3/whitelists.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import List, Optional, TypedDict
 
+from eulith_web3.eip712_types import Eip712Data, Eip712Domain, Eip712Field
+
 
 class ClientWhitelist(TypedDict):
     list_id: int
     sorted_addresses: List[str]
     is_draft: bool
 
 
@@ -27,36 +29,36 @@
 
 
 class AcceptedEnableArmorSignature(TypedDict):
     signature: str
     owner_address: str
 
 
-def get_client_whitelist_typed_data(message: ClientWhitelistHashInput) -> dict:
+def get_client_whitelist_typed_data(message: ClientWhitelistHashInput) -> Eip712Data:
     types = {
         "EIP712Domain": [
-            {"name": "name", "type": "string"},
-            {"name": "version", "type": "string"},
+            Eip712Field(name="name", type="string"),
+            Eip712Field(name="version", type="string"),
         ],
         "ClientWhitelistHashInput": [
-            {"name": "ownerAddress", "type": "string"},
-            {"name": "safeAddress", "type": "string"},
-            {"name": "listContents", "type": "string[]"},
-            {"name": "sub", "type": "string"},
-            {"name": "networkId", "type": "int32"},
+            Eip712Field(name="ownerAddress", type="string"),
+            Eip712Field(name="safeAddress", type="string"),
+            Eip712Field(name="listContents", type="string[]"),
+            Eip712Field(name="sub", type="string"),
+            Eip712Field(name="networkId", type="int32"),
         ],
     }
 
-    payload = {
-        "types": types,
-        "primaryType": "ClientWhitelistHashInput",
-        "domain": {"name": "Eulith", "version": "1"},
-        "message": {
+    payload = Eip712Data(
+        types=types,
+        primaryType="ClientWhitelistHashInput",
+        domain=Eip712Domain(name="Eulith", version="1"),
+        message={
             "ownerAddress": message["owner_address"],
             "safeAddress": message["safe_address"],
             "listContents": message["list_contents"],
             "sub": message["sub"],
             "networkId": message["network_id"],
         },
-    }
+    )
 
     return payload
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3/whitelists_v2/rpc.py` & `eulith_web3-0.27.0/src/eulith_web3/whitelists_v2/rpc.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.22.9/src/eulith_web3.egg-info/PKG-INFO` & `eulith_web3-0.27.0/src/eulith_web3.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulith_web3
-Version: 0.22.9
+Version: 0.27.0
 Summary: A Web3.py compatible wrapper library for Eulith clients
 Author-email: Eulith Team <kristian@eulith.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `eulith_web3-0.22.9/src/eulith_web3.egg-info/SOURCES.txt` & `eulith_web3-0.27.0/src/eulith_web3.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
 src/eulith_web3/__init__.py
 src/eulith_web3/ace.py
-src/eulith_web3/asn_dump.py
 src/eulith_web3/atomic.py
-src/eulith_web3/binding_generator.py
 src/eulith_web3/common.py
 src/eulith_web3/curve.py
+src/eulith_web3/eip712_types.py
 src/eulith_web3/erc20.py
 src/eulith_web3/eulith_service.py
 src/eulith_web3/eulith_web3.py
 src/eulith_web3/exceptions.py
 src/eulith_web3/fireblocks.py
 src/eulith_web3/kms.py
 src/eulith_web3/ledger.py
@@ -29,25 +28,15 @@
 src/eulith_web3.egg-info/PKG-INFO
 src/eulith_web3.egg-info/SOURCES.txt
 src/eulith_web3.egg-info/dependency_links.txt
 src/eulith_web3.egg-info/requires.txt
 src/eulith_web3.egg-info/top_level.txt
 src/eulith_web3/contract_bindings/__init__.py
 src/eulith_web3/contract_bindings/i_e_r_c20.py
-src/eulith_web3/contract_bindings/i_e_r_c721.py
-src/eulith_web3/contract_bindings/i_e_r_c721_enumerable.py
-src/eulith_web3/contract_bindings/i_e_r_c721_metadata.py
-src/eulith_web3/contract_bindings/i_e_r_c721_permit.py
 src/eulith_web3/contract_bindings/i_e_r_c_detailed.py
-src/eulith_web3/contract_bindings/i_lending_pool.py
-src/eulith_web3/contract_bindings/i_nonfungible_position_manager.py
-src/eulith_web3/contract_bindings/i_periphery_immutable_state.py
-src/eulith_web3/contract_bindings/i_periphery_payments.py
-src/eulith_web3/contract_bindings/i_pool_initializer.py
-src/eulith_web3/contract_bindings/i_swap_router.py
 src/eulith_web3/contract_bindings/i_uniswap_v3_pool.py
 src/eulith_web3/contract_bindings/w_e_t_h_interface.py
 src/eulith_web3/contract_bindings/convex/__init__.py
 src/eulith_web3/contract_bindings/convex/i_booster.py
 src/eulith_web3/contract_bindings/convex/i_convex_deposits.py
 src/eulith_web3/contract_bindings/convex/i_reward_staking.py
 src/eulith_web3/contract_bindings/convex/i_rewards.py
```

### Comparing `eulith_web3-0.22.9/tests/test_guard.py` & `eulith_web3-0.27.0/tests/test_guard.py`

 * *Files identical despite different names*

