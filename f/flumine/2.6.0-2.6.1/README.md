# Comparing `tmp/flumine-2.6.0.tar.gz` & `tmp/flumine-2.6.1.tar.gz`

## Comparing `flumine-2.6.0.tar` & `flumine-2.6.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0    38867 2020-02-02 00:00:00.000000 flumine-2.6.0/HISTORY.rst
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/__version__.py
--rw-r--r--   0        0        0    18129 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/baseflumine.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/config.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/exceptions.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/flumine.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/patching.py
--rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/utils.py
--rw-r--r--   0        0        0     9223 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/worker.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/clients/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/clients/baseclient.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/clients/betconnectclient.py
--rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/clients/betfairclient.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/clients/clients.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/clients/simulatedclient.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/controls/__init__.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/controls/clientcontrols.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/controls/loggingcontrols.py
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/controls/tradingcontrols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/events/__init__.py
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/events/events.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/execution/__init__.py
--rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/execution/baseexecution.py
--rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/execution/betfairexecution.py
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/execution/simulatedexecution.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/execution/transaction.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/markets/__init__.py
--rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/markets/blotter.py
--rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/markets/market.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/markets/markets.py
--rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/markets/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/order/__init__.py
--rw-r--r--   0        0        0    16842 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/order/order.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/order/orderpackage.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/order/ordertype.py
--rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/order/process.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/order/responses.py
--rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/order/trade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/simulation/__init__.py
--rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/simulation/simulatedorder.py
--rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/simulation/simulation.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/simulation/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/strategy/__init__.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/strategy/runnercontext.py
--rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/strategy/strategy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/streams/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/streams/basestream.py
--rw-r--r--   0        0        0     9705 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/streams/datastream.py
--rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/streams/historicalstream.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/streams/marketstream.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/streams/orderstream.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/streams/simulatedorderstream.py
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/streams/sportsdatastream.py
--rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 flumine-2.6.0/flumine/streams/streams.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/__init__.py
--rw-r--r--   0        0        0    31232 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_baseflumine.py
--rw-r--r--   0        0        0    31747 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_blotter.py
--rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_clientcontrols.py
--rw-r--r--   0        0        0    19619 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_clients.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_config.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_events.py
--rw-r--r--   0        0        0    65530 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_execution.py
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_flumine.py
--rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_fluminesimulation.py
--rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_integration.py
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_loggingcontrols.py
--rw-r--r--   0        0        0    18354 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_markets.py
--rw-r--r--   0        0        0    21607 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_middleware.py
--rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_order.py
--rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_orderpackage.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_ordertype.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_process.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_release.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_responses.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_runnercontext.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_simulated_utils.py
--rw-r--r--   0        0        0    64569 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_simulatedorder.py
--rw-r--r--   0        0        0    14383 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_strategy.py
--rw-r--r--   0        0        0    41232 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_streams.py
--rw-r--r--   0        0        0     8862 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_trade.py
--rw-r--r--   0        0        0    39115 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_tradingcontrols.py
--rw-r--r--   0        0        0    18014 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_transaction.py
--rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_utils.py
--rw-r--r--   0        0        0    15964 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/test_worker.py
--rw-r--r--   0        0        0   395421 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/resources/1.197931750
--rw-r--r--   0        0        0   299851 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/resources/1.197931751
--rw-r--r--   0        0        0  3071885 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/resources/1.200806927
--rwxr-xr-x   0        0        0   101027 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/resources/BASIC-1.132153978
--rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/resources/BASIC-1.132153978.gz
--rwxr-xr-x   0        0        0  5995014 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/resources/PRO-1.170258213
--rw-r--r--   0        0        0  9510086 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/resources/SELF-1.181223994
--rw-r--r--   0        0        0  4022415 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/resources/SELF-1.181223995
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/resources/catalogues/1.197931750.json
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/resources/catalogues/1.197931751.json
--rw-r--r--   0        0        0  2773842 2020-02-02 00:00:00.000000 flumine-2.6.0/tests/resources/sportsdata/1.200806927
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 flumine-2.6.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flumine-2.6.0/LICENSE
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 flumine-2.6.0/README.md
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 flumine-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 flumine-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0    39105 2020-02-02 00:00:00.000000 flumine-2.6.1/HISTORY.rst
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/__version__.py
+-rw-r--r--   0        0        0    18129 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/baseflumine.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/config.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/exceptions.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/flumine.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/patching.py
+-rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/utils.py
+-rw-r--r--   0        0        0     9223 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/worker.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/clients/__init__.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/clients/baseclient.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/clients/betconnectclient.py
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/clients/betfairclient.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/clients/clients.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/clients/simulatedclient.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/controls/__init__.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/controls/clientcontrols.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/controls/loggingcontrols.py
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/controls/tradingcontrols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/events/__init__.py
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/events/events.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/execution/__init__.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/execution/baseexecution.py
+-rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/execution/betfairexecution.py
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/execution/simulatedexecution.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/execution/transaction.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/markets/__init__.py
+-rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/markets/blotter.py
+-rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/markets/market.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/markets/markets.py
+-rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/markets/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/order/__init__.py
+-rw-r--r--   0        0        0    16842 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/order/order.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/order/orderpackage.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/order/ordertype.py
+-rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/order/process.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/order/responses.py
+-rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/order/trade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/simulation/__init__.py
+-rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/simulation/simulatedorder.py
+-rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/simulation/simulation.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/simulation/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/strategy/__init__.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/strategy/runnercontext.py
+-rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/strategy/strategy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/streams/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/streams/basestream.py
+-rw-r--r--   0        0        0     9705 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/streams/datastream.py
+-rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/streams/historicalstream.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/streams/marketstream.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/streams/orderstream.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/streams/simulatedorderstream.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/streams/sportsdatastream.py
+-rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 flumine-2.6.1/flumine/streams/streams.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/__init__.py
+-rw-r--r--   0        0        0    31232 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_baseflumine.py
+-rw-r--r--   0        0        0    31747 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_blotter.py
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_clientcontrols.py
+-rw-r--r--   0        0        0    19619 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_clients.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_config.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_events.py
+-rw-r--r--   0        0        0    65530 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_execution.py
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_flumine.py
+-rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_fluminesimulation.py
+-rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_integration.py
+-rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_loggingcontrols.py
+-rw-r--r--   0        0        0    21201 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_markets.py
+-rw-r--r--   0        0        0    21607 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_middleware.py
+-rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_order.py
+-rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_orderpackage.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_ordertype.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_process.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_release.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_responses.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_runnercontext.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_simulated_utils.py
+-rw-r--r--   0        0        0    64569 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_simulatedorder.py
+-rw-r--r--   0        0        0    14383 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_strategy.py
+-rw-r--r--   0        0        0    41232 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_streams.py
+-rw-r--r--   0        0        0     8862 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_trade.py
+-rw-r--r--   0        0        0    39115 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_tradingcontrols.py
+-rw-r--r--   0        0        0    18014 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_transaction.py
+-rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_utils.py
+-rw-r--r--   0        0        0    15964 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/test_worker.py
+-rw-r--r--   0        0        0   395421 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/resources/1.197931750
+-rw-r--r--   0        0        0   299851 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/resources/1.197931751
+-rw-r--r--   0        0        0  3071885 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/resources/1.200806927
+-rwxr-xr-x   0        0        0   101027 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/resources/BASIC-1.132153978
+-rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/resources/BASIC-1.132153978.gz
+-rwxr-xr-x   0        0        0  5995014 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/resources/PRO-1.170258213
+-rw-r--r--   0        0        0  9510086 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/resources/SELF-1.181223994
+-rw-r--r--   0        0        0  4022415 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/resources/SELF-1.181223995
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/resources/catalogues/1.197931750.json
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/resources/catalogues/1.197931751.json
+-rw-r--r--   0        0        0  2773842 2020-02-02 00:00:00.000000 flumine-2.6.1/tests/resources/sportsdata/1.200806927
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 flumine-2.6.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flumine-2.6.1/LICENSE
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 flumine-2.6.1/README.md
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 flumine-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 flumine-2.6.1/PKG-INFO
```

### Comparing `flumine-2.6.0/HISTORY.rst` & `flumine-2.6.1/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 .. :changelog:
 
 Release History
 ---------------
 
+2.6.1 (2024-03-26)
++++++++++++++++++++
+
+**Improvements**
+
+- docs
+
+**Libraries**
+
+- betfairlightweight upgraded to 2.20.2
+- betconnect upgraded to 0.2.1
+- black upgraded to 24.4.2
+- smart-open upgraded to <8
+- tenacity upgraded to <8.3.1
+
 2.6.0 (2024-03-11)
 +++++++++++++++++++
 
 **Improvements**
 
 - toml file added / repo cleanup
```

### Comparing `flumine-2.6.0/flumine/__init__.py` & `flumine-2.6.1/flumine/__init__.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/baseflumine.py` & `flumine-2.6.1/flumine/baseflumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/config.py` & `flumine-2.6.1/flumine/config.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/exceptions.py` & `flumine-2.6.1/flumine/exceptions.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/flumine.py` & `flumine-2.6.1/flumine/flumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/patching.py` & `flumine-2.6.1/flumine/patching.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/utils.py` & `flumine-2.6.1/flumine/utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/worker.py` & `flumine-2.6.1/flumine/worker.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/clients/baseclient.py` & `flumine-2.6.1/flumine/clients/baseclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/clients/betconnectclient.py` & `flumine-2.6.1/flumine/clients/betconnectclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/clients/betfairclient.py` & `flumine-2.6.1/flumine/clients/betfairclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/clients/clients.py` & `flumine-2.6.1/flumine/clients/clients.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/clients/simulatedclient.py` & `flumine-2.6.1/flumine/clients/simulatedclient.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/controls/__init__.py` & `flumine-2.6.1/flumine/controls/__init__.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/controls/clientcontrols.py` & `flumine-2.6.1/flumine/controls/clientcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/controls/loggingcontrols.py` & `flumine-2.6.1/flumine/controls/loggingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/controls/tradingcontrols.py` & `flumine-2.6.1/flumine/controls/tradingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/events/events.py` & `flumine-2.6.1/flumine/events/events.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/execution/baseexecution.py` & `flumine-2.6.1/flumine/execution/baseexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/execution/betfairexecution.py` & `flumine-2.6.1/flumine/execution/betfairexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/execution/simulatedexecution.py` & `flumine-2.6.1/flumine/execution/simulatedexecution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/execution/transaction.py` & `flumine-2.6.1/flumine/execution/transaction.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/markets/blotter.py` & `flumine-2.6.1/flumine/markets/blotter.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/markets/market.py` & `flumine-2.6.1/flumine/markets/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     def event(self) -> dict:
         event = defaultdict(list)
         market_start_datetime = self.market_start_datetime
         event_type_id = self.event_type_id
         for market in self.flumine.markets.events[self.event_id]:
             if (
                 market_start_datetime == market.market_start_datetime
-                or event_type_id == "1"
+                or event_type_id in ["1", "3"]  # soccer, golf
             ):
                 event[market.market_type].append(market)
         return event
 
     @property
     def event_type_id(self) -> str:
         if self.market_catalogue:
@@ -133,15 +133,15 @@
         if self.market_catalogue:
             return self.market_catalogue.event.id
         elif self.market_book:
             return self.market_book.market_definition.event_id
 
     @property
     def market_type(self) -> str:
-        if self.market_catalogue:
+        if self.market_catalogue and self.market_catalogue.description:
             return self.market_catalogue.description.market_type
         elif self.market_book:
             return self.market_book.market_definition.market_type
 
     @property
     def seconds_to_start(self) -> float:
         return (self.market_start_datetime - datetime.datetime.utcnow()).total_seconds()
@@ -185,15 +185,15 @@
         if self.market_catalogue:
             return self.market_catalogue.event.venue
         elif self.market_book:
             return self.market_book.market_definition.venue
 
     @property
     def race_type(self) -> Optional[str]:
-        if self.market_catalogue:
+        if self.market_catalogue and self.market_catalogue.description:
             return self.market_catalogue.description.race_type
         elif self.market_book:
             return self.market_book.market_definition.race_type
 
     @property
     def status(self) -> Optional[str]:
         if self.market_book:
```

### Comparing `flumine-2.6.0/flumine/markets/markets.py` & `flumine-2.6.1/flumine/markets/markets.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/markets/middleware.py` & `flumine-2.6.1/flumine/markets/middleware.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/order/order.py` & `flumine-2.6.1/flumine/order/order.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/order/orderpackage.py` & `flumine-2.6.1/flumine/order/orderpackage.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/order/ordertype.py` & `flumine-2.6.1/flumine/order/ordertype.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/order/process.py` & `flumine-2.6.1/flumine/order/process.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/order/responses.py` & `flumine-2.6.1/flumine/order/responses.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/order/trade.py` & `flumine-2.6.1/flumine/order/trade.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/simulation/simulatedorder.py` & `flumine-2.6.1/flumine/simulation/simulatedorder.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/simulation/simulation.py` & `flumine-2.6.1/flumine/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/simulation/utils.py` & `flumine-2.6.1/flumine/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/strategy/runnercontext.py` & `flumine-2.6.1/flumine/strategy/runnercontext.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/strategy/strategy.py` & `flumine-2.6.1/flumine/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/streams/basestream.py` & `flumine-2.6.1/flumine/streams/basestream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/streams/datastream.py` & `flumine-2.6.1/flumine/streams/datastream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/streams/historicalstream.py` & `flumine-2.6.1/flumine/streams/historicalstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/streams/marketstream.py` & `flumine-2.6.1/flumine/streams/marketstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/streams/orderstream.py` & `flumine-2.6.1/flumine/streams/orderstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/streams/simulatedorderstream.py` & `flumine-2.6.1/flumine/streams/simulatedorderstream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/streams/sportsdatastream.py` & `flumine-2.6.1/flumine/streams/sportsdatastream.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/flumine/streams/streams.py` & `flumine-2.6.1/flumine/streams/streams.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_baseflumine.py` & `flumine-2.6.1/tests/test_baseflumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_blotter.py` & `flumine-2.6.1/tests/test_blotter.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_clientcontrols.py` & `flumine-2.6.1/tests/test_clientcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_clients.py` & `flumine-2.6.1/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_config.py` & `flumine-2.6.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_events.py` & `flumine-2.6.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_execution.py` & `flumine-2.6.1/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_flumine.py` & `flumine-2.6.1/tests/test_flumine.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_fluminesimulation.py` & `flumine-2.6.1/tests/test_fluminesimulation.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_integration.py` & `flumine-2.6.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_loggingcontrols.py` & `flumine-2.6.1/tests/test_loggingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_markets.py` & `flumine-2.6.1/tests/test_markets.py`

 * *Files 11% similar despite different names*

```diff
@@ -217,30 +217,78 @@
         mock_order = mock.Mock()
         self.assertTrue(self.market.replace_order(mock_order, 2, False, force=True))
         mock_transaction.assert_called_with(client=mock_order.client)
         mock_transaction.replace_order.assert_called_with(mock_order, 2, False, True)
 
     def test_event(self):
         self.market.market_catalogue.event.id = 12
+        self.market.market_catalogue.event_type.id = "7"
         self.market.market_book.market_definition.market_time = 12
         self.market.flumine.markets.events = defaultdict(list)
         self.assertEqual(self.market.event, {})
 
         m_one = mock.Mock(market_type=1, event_id=12, market_start_datetime=12)
         m_two = mock.Mock(market_type=2, event_id=12, market_start_datetime=12)
         m_three = mock.Mock(market_type=3, event_id=123, market_start_datetime=12)
         m_four = mock.Mock(market_type=1, event_id=12, market_start_datetime=12)
         m_five = mock.Mock(market_type=2, event_id=12, market_start_datetime=13)
+        m_six = mock.Mock(
+            market_type=2, event_id=13, market_start_datetime=13
+        )  # different event
         self.market.flumine.markets.events[m_one.event_id].append(m_one)
         self.market.flumine.markets.events[m_two.event_id].append(m_two)
         self.market.flumine.markets.events[m_three.event_id].append(m_three)
         self.market.flumine.markets.events[m_four.event_id].append(m_four)
         self.market.flumine.markets.events[m_five.event_id].append(m_five)
+        self.market.flumine.markets.events[m_six.event_id].append(m_six)
         self.assertEqual(self.market.event, {1: [m_one, m_four], 2: [m_two]})
 
+    def test_event_filters(self):
+        self.market.market_catalogue.event.id = 12
+        self.market.market_catalogue.event_type.id = "1"
+        self.market.market_book.market_definition.market_time = 12
+        self.market.flumine.markets.events = defaultdict(list)
+        self.assertEqual(self.market.event, {})
+
+        m_one = mock.Mock(
+            market_type=1, event_id=12, event_type_id="1", market_start_datetime=12
+        )
+        m_two = mock.Mock(
+            market_type=2, event_id=12, event_type_id="1", market_start_datetime=12
+        )
+        m_three = mock.Mock(
+            market_type=3, event_id=123, event_type_id="1", market_start_datetime=12
+        )
+        m_four = mock.Mock(
+            market_type=2, event_id=12, event_type_id="1", market_start_datetime=13
+        )
+        m_five = mock.Mock(
+            market_type=1, event_id=13, event_type_id="1", market_start_datetime=13
+        )
+        m_six = mock.Mock(
+            market_type=2, event_id=13, event_type_id="3", market_start_datetime=13
+        )
+        self.market.flumine.markets.events[m_one.event_id].append(m_one)
+        self.market.flumine.markets.events[m_two.event_id].append(m_two)
+        self.market.flumine.markets.events[m_three.event_id].append(m_three)
+        self.market.flumine.markets.events[m_four.event_id].append(m_four)
+        self.market.flumine.markets.events[m_five.event_id].append(m_five)
+        self.market.flumine.markets.events[m_six.event_id].append(m_six)
+        self.assertEqual(self.market.event, {1: [m_one], 2: [m_two, m_four]})
+
+        self.market.market_catalogue.event.id = 13
+        self.market.market_catalogue.event_type.id = "3"
+        self.market.market_book.market_definition.market_time = 12
+        self.market.flumine.markets.events = defaultdict(list)
+        m_six = mock.Mock(
+            market_type=2, event_id=13, event_type_id="3", market_start_datetime=13
+        )
+        self.market.flumine.markets.events[m_six.event_id].append(m_six)
+        self.assertEqual(self.market.event, {2: [m_six]})
+
     def test_event_type_id_mc(self):
         mock_market_catalogue = mock.Mock()
         self.market.market_catalogue = mock_market_catalogue
         self.assertEqual(self.market.event_type_id, mock_market_catalogue.event_type.id)
 
     def test_event_type_id_mb(self):
         self.market.market_catalogue = None
@@ -265,14 +313,20 @@
 
     def test_market_type_mc(self):
         mock_market_catalogue = mock.Mock()
         self.market.market_catalogue = mock_market_catalogue
         self.assertEqual(
             self.market.market_type, mock_market_catalogue.description.market_type
         )
+        self.market.market_catalogue.description = None
+        mock_market_book = mock.Mock()
+        self.market.market_book = mock_market_book
+        self.assertEqual(
+            self.market.market_type, mock_market_book.market_definition.market_type
+        )
 
     def test_market_type_mb(self):
         self.market.market_catalogue = None
         mock_market_book = mock.Mock()
         self.market.market_book = mock_market_book
         self.assertEqual(
             self.market.market_type, mock_market_book.market_definition.market_type
@@ -379,14 +433,20 @@
 
     def test_race_type_mc(self):
         mock_market_catalogue = mock.Mock()
         self.market.market_catalogue = mock_market_catalogue
         self.assertEqual(
             self.market.race_type, mock_market_catalogue.description.race_type
         )
+        self.market.market_catalogue.description = None
+        mock_market_book = mock.Mock()
+        self.market.market_book = mock_market_book
+        self.assertEqual(
+            self.market.race_type, mock_market_book.market_definition.race_type
+        )
 
     def test_race_type_mb(self):
         self.market.market_catalogue = None
         mock_market_book = mock.Mock()
         self.market.market_book = mock_market_book
         self.assertEqual(
             self.market.race_type, mock_market_book.market_definition.race_type
```

### Comparing `flumine-2.6.0/tests/test_middleware.py` & `flumine-2.6.1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_order.py` & `flumine-2.6.1/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_orderpackage.py` & `flumine-2.6.1/tests/test_orderpackage.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_ordertype.py` & `flumine-2.6.1/tests/test_ordertype.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_process.py` & `flumine-2.6.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_responses.py` & `flumine-2.6.1/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_runnercontext.py` & `flumine-2.6.1/tests/test_runnercontext.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_simulated_utils.py` & `flumine-2.6.1/tests/test_simulated_utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_simulatedorder.py` & `flumine-2.6.1/tests/test_simulatedorder.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_strategy.py` & `flumine-2.6.1/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_streams.py` & `flumine-2.6.1/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_trade.py` & `flumine-2.6.1/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_tradingcontrols.py` & `flumine-2.6.1/tests/test_tradingcontrols.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_transaction.py` & `flumine-2.6.1/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_utils.py` & `flumine-2.6.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/test_worker.py` & `flumine-2.6.1/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/resources/1.197931750` & `flumine-2.6.1/tests/resources/1.197931750`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/resources/1.197931751` & `flumine-2.6.1/tests/resources/1.197931751`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/resources/1.200806927` & `flumine-2.6.1/tests/resources/1.200806927`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/resources/BASIC-1.132153978` & `flumine-2.6.1/tests/resources/BASIC-1.132153978`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/resources/BASIC-1.132153978.gz` & `flumine-2.6.1/tests/resources/BASIC-1.132153978.gz`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/resources/PRO-1.170258213` & `flumine-2.6.1/tests/resources/PRO-1.170258213`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/resources/SELF-1.181223994` & `flumine-2.6.1/tests/resources/SELF-1.181223994`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/resources/SELF-1.181223995` & `flumine-2.6.1/tests/resources/SELF-1.181223995`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/resources/catalogues/1.197931750.json` & `flumine-2.6.1/tests/resources/catalogues/1.197931750.json`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/resources/catalogues/1.197931751.json` & `flumine-2.6.1/tests/resources/catalogues/1.197931751.json`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/tests/resources/sportsdata/1.200806927` & `flumine-2.6.1/tests/resources/sportsdata/1.200806927`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/LICENSE` & `flumine-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/README.md` & `flumine-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `flumine-2.6.0/pyproject.toml` & `flumine-2.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -17,29 +17,29 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "betfairlightweight==2.20.1",
-    "tenacity>=7.0.0,<8.2.4",
+    "betfairlightweight==2.20.2",
+    "tenacity>=7.0.0,<8.3.1",
     "python-json-logger==2.0.7",
     "requests",
-    "betconnect==0.1.7",
-    "smart-open>=6,<7",
+    "betconnect==0.2.1",
+    "smart-open>=6,<8",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 speed = [
-    "betfairlightweight[speed]==2.20.1"
+    "betfairlightweight[speed]==2.20.2"
 ]
 test = [
-    "black==24.2.0",
+    "black==24.4.2",
     "coverage",
     "pre-commit",
     "mkdocs",
     "mkdocs-material",
     "build",
     "twine",
 ]
```

### Comparing `flumine-2.6.0/PKG-INFO` & `flumine-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: flumine
-Version: 2.6.0
+Version: 2.6.1
 Summary: Betting trading framework
 Project-URL: Homepage, https://github.com/betcode-org
 Project-URL: Documentation, https://betcode-org.github.io/flumine/
 Project-URL: Repository, https://github.com/betcode-org/flumine.git
 Project-URL: Bug Tracker, https://github.com/betcode-org/flumine/issues
 Project-URL: Changelog, https://github.com/betcode-org/flumine/blob/master/HISTORY.rst
 Author-email: Liam Pauling <a@unknown.com>
@@ -34,24 +34,24 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: betconnect==0.1.7
-Requires-Dist: betfairlightweight==2.20.1
+Requires-Dist: betconnect==0.2.1
+Requires-Dist: betfairlightweight==2.20.2
 Requires-Dist: python-json-logger==2.0.7
 Requires-Dist: requests
-Requires-Dist: smart-open<7,>=6
-Requires-Dist: tenacity<8.2.4,>=7.0.0
+Requires-Dist: smart-open<8,>=6
+Requires-Dist: tenacity<8.3.1,>=7.0.0
 Provides-Extra: speed
-Requires-Dist: betfairlightweight[speed]==2.20.1; extra == 'speed'
+Requires-Dist: betfairlightweight[speed]==2.20.2; extra == 'speed'
 Provides-Extra: test
-Requires-Dist: black==24.2.0; extra == 'test'
+Requires-Dist: black==24.4.2; extra == 'test'
 Requires-Dist: build; extra == 'test'
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: mkdocs; extra == 'test'
 Requires-Dist: mkdocs-material; extra == 'test'
 Requires-Dist: pre-commit; extra == 'test'
 Requires-Dist: twine; extra == 'test'
 Description-Content-Type: text/markdown
```

