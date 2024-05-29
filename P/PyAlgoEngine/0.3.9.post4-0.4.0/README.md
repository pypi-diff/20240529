# Comparing `tmp/PyAlgoEngine-0.3.9.post4.tar.gz` & `tmp/pyalgoengine-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAlgoEngine-0.3.9.post4.tar", last modified: Tue Dec 26 15:01:34 2023, max compression
+gzip compressed data, was "pyalgoengine-0.4.0.tar", last modified: Wed May 29 07:24:17 2024, max compression
```

## Comparing `PyAlgoEngine-0.3.9.post4.tar` & `pyalgoengine-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,34 @@
-drwxr-xr-x   0 bolun     (1000) bolun     (1000)        0 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/
-drwxr-xr-x   0 bolun     (1000) bolun     (1000)        0 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/AlgoEngine/
-drwxr-xr-x   0 bolun     (1000) bolun     (1000)        0 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/
--rw-r--r--   0 bolun     (1000) bolun     (1000)    31104 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/AlgoEngine.py
--rw-r--r--   0 bolun     (1000) bolun     (1000)     1465 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/EventEngine.py
--rw-r--r--   0 bolun     (1000) bolun     (1000)    32576 2023-12-26 14:54:56.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/MarketEngine.py
--rw-r--r--   0 bolun     (1000) bolun     (1000)    80159 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/TradeEngine.py
--rw-r--r--   0 bolun     (1000) bolun     (1000)     3653 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/__init__.py
-drwxr-xr-x   0 bolun     (1000) bolun     (1000)        0 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/
--rw-r--r--   0 bolun     (1000) bolun     (1000)     1814 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/BackTest.py
--rw-r--r--   0 bolun     (1000) bolun     (1000)    14977 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/_StrategyEngine.py
--rw-r--r--   0 bolun     (1000) bolun     (1000)     1738 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/__init__.py
--rw-r--r--   0 bolun     (1000) bolun     (1000)      432 2023-12-26 14:55:20.000000 PyAlgoEngine-0.3.9.post4/AlgoEngine/__init__.py
--rw-r--r--   0 bolun     (1000) bolun     (1000)     1066 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/LICENSE
--rw-r--r--   0 bolun     (1000) bolun     (1000)      653 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/PKG-INFO
-drwxr-xr-x   0 bolun     (1000) bolun     (1000)        0 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/
--rw-r--r--   0 bolun     (1000) bolun     (1000)      653 2023-12-26 15:01:34.000000 PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/PKG-INFO
--rw-r--r--   0 bolun     (1000) bolun     (1000)      499 2023-12-26 15:01:34.000000 PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/SOURCES.txt
--rw-r--r--   0 bolun     (1000) bolun     (1000)        1 2023-12-26 15:01:34.000000 PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/dependency_links.txt
--rw-r--r--   0 bolun     (1000) bolun     (1000)       57 2023-12-26 15:01:34.000000 PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/requires.txt
--rw-r--r--   0 bolun     (1000) bolun     (1000)       11 2023-12-26 15:01:34.000000 PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/top_level.txt
--rw-r--r--   0 bolun     (1000) bolun     (1000)       42 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/README.md
--rw-r--r--   0 bolun     (1000) bolun     (1000)       38 2023-12-26 15:01:34.331208 PyAlgoEngine-0.3.9.post4/setup.cfg
--rw-r--r--   0 bolun     (1000) bolun     (1000)     1528 2023-12-13 07:18:50.000000 PyAlgoEngine-0.3.9.post4/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.697980 pyalgoengine-0.4.0/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-15 04:37:41.000000 pyalgoengine-0.4.0/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      769 2024-05-29 07:24:17.683160 pyalgoengine-0.4.0/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.679160 pyalgoengine-0.4.0/PyAlgoEngine.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      769 2024-05-29 07:24:17.000000 pyalgoengine-0.4.0/PyAlgoEngine.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      747 2024-05-29 07:24:17.000000 pyalgoengine-0.4.0/PyAlgoEngine.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-29 07:24:17.000000 pyalgoengine-0.4.0/PyAlgoEngine.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       77 2024-05-29 07:24:17.000000 pyalgoengine-0.4.0/PyAlgoEngine.egg-info/requires.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       12 2024-05-29 07:24:17.000000 pyalgoengine-0.4.0/PyAlgoEngine.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       42 2024-05-15 04:37:41.000000 pyalgoengine-0.4.0/README.md
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.373379 pyalgoengine-0.4.0/algo_engine/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1936 2024-05-29 07:16:50.000000 pyalgoengine-0.4.0/algo_engine/__init__.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.418403 pyalgoengine-0.4.0/algo_engine/back_test/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      232 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0/algo_engine/back_test/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1821 2024-05-29 07:23:17.000000 pyalgoengine-0.4.0/algo_engine/back_test/__main__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     9216 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0/algo_engine/back_test/replay.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    14126 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0/algo_engine/back_test/sim_match.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.535651 pyalgoengine-0.4.0/algo_engine/engine/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      672 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0/algo_engine/engine/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    31180 2024-05-29 07:23:17.000000 pyalgoengine-0.4.0/algo_engine/engine/algo_engine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1354 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0/algo_engine/engine/event_engine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    11697 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0/algo_engine/engine/market_engine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    69005 2024-05-29 06:58:50.000000 pyalgoengine-0.4.0/algo_engine/engine/trade_engine.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.579651 pyalgoengine-0.4.0/algo_engine/monitor/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      449 2024-05-28 11:24:54.000000 pyalgoengine-0.4.0/algo_engine/monitor/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     8940 2024-05-28 10:54:06.000000 pyalgoengine-0.4.0/algo_engine/monitor/advanced_data_interface.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.624159 pyalgoengine-0.4.0/algo_engine/profile/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1900 2024-05-29 07:03:58.000000 pyalgoengine-0.4.0/algo_engine/profile/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     7052 2024-05-28 11:28:56.000000 pyalgoengine-0.4.0/algo_engine/profile/cn.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.668160 pyalgoengine-0.4.0/algo_engine/strategie/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1619 2024-05-29 07:16:50.000000 pyalgoengine-0.4.0/algo_engine/strategie/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    15413 2024-05-29 07:23:17.000000 pyalgoengine-0.4.0/algo_engine/strategie/strategy_engine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2024-05-29 07:24:17.702980 pyalgoengine-0.4.0/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1649 2024-05-29 07:23:17.000000 pyalgoengine-0.4.0/setup.py
```

### Comparing `PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/AlgoEngine.py` & `pyalgoengine-0.4.0/algo_engine/engine/algo_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from __future__ import annotations
-
 import abc
 import datetime
 import enum
 import functools
 import json
 import threading
 import uuid
-from typing import Type
+from typing import Type, TYPE_CHECKING
 
 import numpy as np
 from PyQuantKit import TransactionSide, TradeInstruction, MarketData, TradeReport, OrderState, OrderType
 
 from . import LOGGER
-from .MarketEngine import MDS
+from .market_engine import MDS
+
+if TYPE_CHECKING:
+    from .trade_engine import DirectMarketAccess
 
-LOGGER = LOGGER.getChild('AlgoEngine')
 __all__ = ['AlgoTemplate', 'AlgoRegistry', 'AlgoEngine', 'ALGO_ENGINE', 'ALGO_REGISTRY']
 
 
 class AlgoStatus(enum.Enum):
     idle = 'idle'  # init state 
     preparing = 'preparing'  # preparing
     ready = 'ready'  # ready to launch order
@@ -30,15 +30,15 @@
     rejected = 'rejected'  # internal / external rejected
     error = 'error'  # internal / external error
 
 
 class AlgoTemplate(object, metaclass=abc.ABCMeta):
     Status = AlgoStatus
 
-    def __init__(self, dma, ticker: str, target_volume: float, side: TransactionSide, **kwargs):
+    def __init__(self, dma: DirectMarketAccess, ticker: str, target_volume: float, side: TransactionSide, **kwargs):
         """ Template for trading algorithm
         an abstract class to create a trading algorithm
 
         :param dma: direct market access
         :param ticker: the given symbol of the underlying to trade
         :param target_volume: the given volume to trade
         :param side: the given TransactionSide
@@ -429,15 +429,15 @@
 
 class Passive(AlgoTemplate):
     """ Passive trading algorithm
     Passive is a basic trading algo which trades all target volume into one single LIMIT order.
     Algo will stop after order get filled or canceled.
     no additional order will be launched except the initial one
 
-    a limit price can be set by keyword arguments, see also in doc: AlgoEngine.calculate_limit
+    a limit price can be set by keyword arguments, see also in doc: algo_engine.calculate_limit
 
     """
 
     def __init__(self, **kwargs):
         """
         init a Passive trade algo
 
@@ -483,15 +483,16 @@
         if volume:
             order = TradeInstruction(
                 ticker=self.ticker,
                 side=self.side,
                 order_type=order_type,
                 volume=volume,
                 limit_price=limit,
-                order_id=f'{self.__class__.__name__}.{self.ticker}.{self.side.side_name}.{uuid.uuid4().hex}'
+                order_id=f'{self.__class__.__name__}.{self.ticker}.{self.side.side_name}.{uuid.uuid4().hex}',
+                timestamp=self.dma.timestamp
             )
 
             self.working_order[order.order_id] = order
             self.order[order.order_id] = order
             self.start_time = self.market_time
             self._launch(order=order, **kwargs)
 
@@ -671,68 +672,14 @@
     def _filled(self, order: TradeInstruction, report: TradeReport, **kwargs):
         return Aggressive._filled(self=self, order=order, report=report, **kwargs)
 
     def _canceled(self, order: TradeInstruction, **kwargs):
         return Aggressive._canceled(self=self, order=order, **kwargs)
 
 
-class AlgoRegistry(object):
-    """
-    registry for trade algos
-
-    to add a new algo, add name to __init__ method, add handler to .cast() method
-
-    DO NOT add any other value to __init__.
-    """
-
-    def __init__(self):
-        super().__init__()
-
-        self.alias = {}
-        self.registry = {}
-
-        # pre-defined algo name for easy access
-        self.aggressive = 'aggressive'
-        self.passive = 'passive'
-        self.aggressive_timeout = 'aggressive_timeout'
-        self.passive_timeout = 'passive_timeout'
-        self.limit_range = 'limit_range'
-
-    def add_algo(self, name: str, *alias, handler: Type[AlgoTemplate]):
-        self.registry[name] = handler
-
-        for _alias in alias:
-            self.alias[_alias] = name
-
-    def cast(self, value: str):
-        name = value.lower()
-
-        # check alias
-        if name in self.alias:
-            name = self.alias[name]
-
-        # init from storage
-        if name in self.registry:
-            return self.registry[name]
-        else:
-            raise ValueError(f'Invalid name {value}')
-
-    @property
-    def reversed_registry(self) -> dict[str, str]:
-        reversed_registry = {algo.__name__: name for name, algo in self.registry.items()}
-        return reversed_registry
-
-    def to_algo(self, name: str, algo_engine: AlgoEngine = None):
-        if algo_engine is None:
-            algo_engine = ALGO_ENGINE
-
-        algo = self.registry.get(name.lower())
-        return functools.partial(algo, algo_engine=algo_engine)
-
-
 class AlgoEngine(object):
     def __init__(self, mds=None, registry=None):
         self.mds = mds if mds is not None else MDS
         self.registry = registry if registry is not None else ALGO_REGISTRY
 
     @classmethod
     def _compare_price(cls, side: TransactionSide, limit_price: float = None, original_limit: float = None, mode='strict') -> float:
@@ -850,14 +797,68 @@
             algo_id=json_dict['algo_id']
         )
         algo.from_json(json_dict)
 
         return algo
 
 
+class AlgoRegistry(object):
+    """
+    registry for trade algos
+
+    to add a new algo, add name to __init__ method, add handler to .cast() method
+
+    DO NOT add any other value to __init__.
+    """
+
+    def __init__(self):
+        super().__init__()
+
+        self.alias = {}
+        self.registry = {}
+
+        # pre-defined algo name for easy access
+        self.aggressive = 'aggressive'
+        self.passive = 'passive'
+        self.aggressive_timeout = 'aggressive_timeout'
+        self.passive_timeout = 'passive_timeout'
+        self.limit_range = 'limit_range'
+
+    def add_algo(self, name: str, *alias, handler: Type[AlgoTemplate]):
+        self.registry[name] = handler
+
+        for _alias in alias:
+            self.alias[_alias] = name
+
+    def cast(self, value: str):
+        name = value.lower()
+
+        # check alias
+        if name in self.alias:
+            name = self.alias[name]
+
+        # init from storage
+        if name in self.registry:
+            return self.registry[name]
+        else:
+            raise ValueError(f'Invalid name {value}')
+
+    @property
+    def reversed_registry(self) -> dict[str, str]:
+        reversed_registry = {algo.__name__: name for name, algo in self.registry.items()}
+        return reversed_registry
+
+    def to_algo(self, name: str, algo_engine: AlgoEngine = None):
+        if algo_engine is None:
+            algo_engine = ALGO_ENGINE
+
+        algo = self.registry.get(name.lower())
+        return functools.partial(algo, algo_engine=algo_engine)
+
+
 ALGO_REGISTRY = AlgoRegistry()
 
 ALGO_REGISTRY.add_algo('aggressive', 'aggr', handler=Aggressive)
 ALGO_REGISTRY.add_algo('passive', 'pass', handler=Passive)
 ALGO_REGISTRY.add_algo('aggressive_timeout', 'aggr_timeout', handler=AggressiveTimeout)
 ALGO_REGISTRY.add_algo('passive_timeout', 'pass_timeout', handler=PassiveTimeout)
```

### Comparing `PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/EventEngine.py` & `pyalgoengine-0.4.0/algo_engine/engine/event_engine.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from types import SimpleNamespace
 
-import EventEngine
+import event_engine
+from event_engine import Topic, PatternTopic, EventEngine
 
 from . import LOGGER
 
 __all__ = ['EVENT_ENGINE', 'TOPIC']
-LOGGER = LOGGER.getChild('EventEngine')
-EventEngine.set_logger(LOGGER)
+
+event_engine.set_logger(LOGGER)
 
 
 class TopicSet(object):
-    on_order = EventEngine.Topic('on_order')
-    on_report = EventEngine.Topic('on_report')
-    eod = EventEngine.Topic('eod')
-    eod_done = EventEngine.Topic('eod_done')
-    bod = EventEngine.Topic('bod')
-    bod_done = EventEngine.Topic('bod_done')
-
-    launch_order = EventEngine.PatternTopic('launch_order.{ticker}')
-    cancel_order = EventEngine.PatternTopic('cancel_order.{ticker}')
-    realtime = EventEngine.PatternTopic('realtime.{ticker}.{dtype}')
+    on_order = Topic('on_order')
+    on_report = Topic('on_report')
+    eod = Topic('eod')
+    eod_done = Topic('eod_done')
+    bod = Topic('bod')
+    bod_done = Topic('bod_done')
+
+    launch_order = PatternTopic('launch_order.{ticker}')
+    cancel_order = PatternTopic('cancel_order.{ticker}')
+    realtime = PatternTopic('realtime.{ticker}.{dtype}')
 
     @classmethod
     def push(cls, market_data):
         return cls.realtime(ticker=market_data.ticker, dtype=market_data.__class__.__name__)
 
     @classmethod
-    def parse(cls, topic: EventEngine.Topic) -> SimpleNamespace:
+    def parse(cls, topic: Topic) -> SimpleNamespace:
         try:
             _ = topic.value.split('.')
 
             action = _.pop(0)
             if action in ['open', 'close']:
                 dtype = None
             else:
@@ -43,10 +44,10 @@
                 ticker=ticker
             )
             return p
         except Exception as _:
             raise ValueError(f'Invalid topic {topic}')
 
 
-EVENT_ENGINE = EventEngine.EventEngine()
+EVENT_ENGINE = EventEngine()
 TOPIC = TopicSet
 # EVENT_ENGINE.start()
```

### Comparing `PyAlgoEngine-0.3.9.post4/AlgoEngine/Engine/TradeEngine.py` & `pyalgoengine-0.4.0/algo_engine/engine/trade_engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from __future__ import annotations
 
 import abc
 import datetime
 import json
 import os
 import pathlib
-import queue
-import threading
 import time
 import uuid
-from collections import defaultdict
+from collections import defaultdict, deque
 from enum import Enum
+from threading import Thread, Semaphore
 
 import numpy as np
 import pandas as pd
-from PyQuantKit import TransactionSide, TradeInstruction, OrderType, MarketData, BarData, TradeData, TickData, OrderState, OrderBook, TradeReport
+from PyQuantKit import TransactionSide, TradeInstruction, MarketData, OrderState, TradeReport
 
 from . import LOGGER
-from .AlgoEngine import ALGO_ENGINE, AlgoTemplate
-from .EventEngine import TOPIC, EVENT_ENGINE
-from .MarketEngine import MarketDataService
+from .algo_engine import ALGO_ENGINE, AlgoTemplate
+from .market_engine import MarketDataService
 
-LOGGER = LOGGER.getChild('TradeEngine')
-__all__ = ['DirectMarketAccess', 'PositionManagementService', 'Balance', 'Inventory', 'RiskProfile', 'SimMatch']
+
+__all__ = ['DirectMarketAccess', 'PositionManagementService', 'Balance', 'Inventory', 'RiskProfile']
 
 
 class NameSpace(dict):
     def __init__(self, name: str = None, **kwargs):
         self.name = name
         super().__init__(**kwargs)
 
@@ -59,21 +57,24 @@
 
     2 ways to implement this api
     - override the abstractmethod _launch_order_handler, _cancel_order_handler, _reject_order_handler to api directly
     - or use event engine
     """
 
     def __init__(self, mds: MarketDataService, risk_profile: RiskProfile, cool_down: float = None):
+        assert cool_down is None or cool_down > 0, 'Order buff cool down must greater than 0.'
+
         self.mds = mds
         self.risk_profile = risk_profile
         self.cool_down = cool_down
 
-        self.order_queue = queue.Queue()
-        self.worker = threading.Thread(target=self._run)
-        self._is_done = False
+        self.order_queue = deque()
+        self.worker = Thread(target=self._order_buffer)
+        self.lock = Semaphore(0)
+        self.enabled = False
 
     def __repr__(self):
         return f'<OrderHandler>(cd={self.cool_down}, id={id(self)})'
 
     @abc.abstractmethod
     def _launch_order_handler(self, order: TradeInstruction, **kwargs):
         ...
@@ -82,40 +83,41 @@
     def _cancel_order_handler(self, order: TradeInstruction, **kwargs):
         ...
 
     @abc.abstractmethod
     def _reject_order_handler(self, order: TradeInstruction, **kwargs):
         ...
 
-    def trade_time_between(self, start_time: datetime.datetime | float, end_time: datetime.datetime | float, **kwargs) -> datetime.timedelta:
-        return self.mds.trade_time_between(start_time, end_time, **kwargs)
-
     def _launch_order_buffed(self, order: TradeInstruction, **kwargs):
-        self.order_queue.put(('launch', order, kwargs))
+        self.lock.release()
+        self.order_queue.append(('launch', order, kwargs))
 
     def _cancel_order_buffed(self, order: TradeInstruction, **kwargs):
-        self.order_queue.put(('cancel', order, kwargs))
+        self.lock.release()
+        self.order_queue.append(('cancel', order, kwargs))
 
     def _launch_order_no_wait(self, order: TradeInstruction, **kwargs):
         LOGGER.info(f'{self} sent a LAUNCH signal of {order}')
-        is_pass = self.risk_profile.check(order=order)
 
-        if not is_pass:
+        if not self.enabled:
+            LOGGER.warning(f'{order} Rejected by {self}! {self} not enabled!')
+            order.set_order_state(order_state=OrderState.Rejected, timestamp=self.mds.timestamp)
+            self._reject_order_handler(order=order, **kwargs)
+        elif not (is_pass := self.risk_profile.check(order=order)):
             LOGGER.warning(f'{order} Rejected by risk control! Invalid action {order.ticker} {order.side.name} {order.volume}!')
-            order.set_order_state(order_state=OrderState.Rejected)
+            order.set_order_state(order_state=OrderState.Rejected, timestamp=self.mds.timestamp)
             self._reject_order_handler(order=order, **kwargs)
-            return
-
-        order.set_order_state(order_state=OrderState.Sent)
-        self._launch_order_handler(order=order, **kwargs)
+        else:
+            order.set_order_state(order_state=OrderState.Sent, timestamp=self.mds.timestamp)
+            self._launch_order_handler(order=order, **kwargs)
 
     def _cancel_order_no_wait(self, order: TradeInstruction, **kwargs):
         LOGGER.info(f'{self} sent a CANCEL signal of {order}')
 
-        order.set_order_state(order_state=OrderState.Canceling)
+        order.set_order_state(order_state=OrderState.Canceling, timestamp=self.mds.timestamp)
         self._cancel_order_handler(order=order, **kwargs)
 
     def launch_order(self, order: TradeInstruction, **kwargs):
         LOGGER.info(f'{self} launching order {order}')
         if self.cool_down:
             self._launch_order_buffed(order=order, **kwargs)
         else:
@@ -124,49 +126,60 @@
     def cancel_order(self, order: TradeInstruction, **kwargs):
         LOGGER.info(f'{self} canceling order {order}')
         if self.cool_down:
             self._cancel_order_buffed(order=order, **kwargs)
         else:
             self._cancel_order_no_wait(order=order, **kwargs)
 
-    def _process_order(self):
-        try:
-            flag, order, kwargs = self.order_queue.get(block=False)
+    def _order_buffer(self):
+        while True:
+            ts = time.time()
+            self.lock.acquire(blocking=True)
+
+            try:
+                action, order, kwargs = self.order_queue.popleft()
+            except IndexError as e:
+                if not self.enabled:
+                    break
+                else:
+                    raise e
 
-            if flag == 'launch':
+            if action == 'launch':
                 self._launch_order_no_wait(order=order, **kwargs)
-            elif flag == 'cancel':
+            elif action == 'cancel':
                 self._cancel_order_no_wait(order=order, **kwargs)
             else:
-                LOGGER.info(f'Invalid order type {flag}')
-        except queue.Empty:
-            pass
+                LOGGER.info(f'Invalid order action {action}!')
 
-    def _run(self):
-        while True:
-            self._process_order()
-
-            time.sleep(self.cool_down)
+            if self.cool_down and (cool_down := (ts + self.cool_down - time.time())) > 0:
+                time.sleep(cool_down)
 
-            if self._is_done:
+            if not self.enabled:
                 break
-        LOGGER.info('DMA successfully shutdown!')
 
     def run(self):
-        self.worker.run()
+        if self.enabled:
+            LOGGER.error(f'{self} already started!')
 
-    @property
-    def is_done(self):
-        return self._is_done
+        self.enabled = True
+        self.worker.run()
 
     def shut_down(self):
-        self._is_done = True
+        if not self.enabled:
+            LOGGER.error(f'{self} already stopped!')
+
+        self.enabled = False
+        self.lock.release()
         LOGGER.info(f'Order buff shutting down!')
 
     @property
+    def timestamp(self):
+        return self.mds.timestamp
+
+    @property
     def market_price(self):
         return self.mds.market_price
 
     @property
     def market_time(self):
         return self.mds.market_time
 
@@ -182,115 +195,105 @@
     """
 
     def __init__(
             self,
             dma: DirectMarketAccess,
             algo_engine=None,
             default_algo: str = None,
+            no_cache: bool = False,
             **kwargs
     ):
         self.dma = dma
         self.algo_engine = algo_engine if algo_engine is not None else ALGO_ENGINE
         self.algo_registry = self.algo_engine.registry
         self.default_algo = self.algo_registry.passive if default_algo is None else default_algo
         self.position_id = kwargs.pop('position_id', uuid.uuid4().hex)
-        self.logger = kwargs.pop('logger', LOGGER)
+        self.no_cache = no_cache
 
         self.algos: dict[str, AlgoTemplate] = {}
         self.working_algos: dict[str, AlgoTemplate] = {}
 
+        # cache
+        self._exposure: dict[str, float] | None = None
+        self._working: dict[str, dict[str, float]] | None = None
+
     def __call__(self, market_data: MarketData):
         self.on_market_data(market_data=market_data)
 
-    def open(self, ticker: str, target_volume: float, trade_side: TransactionSide, algo: str = None, **kwargs):
-        if algo is None:
-            algo = self.default_algo
-
-        if target_volume:
-            algo = self.algo_registry.to_algo(name=algo)(
-                handler=self,
-                ticker=ticker,
-                side=trade_side,
-                target_volume=target_volume,
-                dma=self.dma,
-                **kwargs
-            )
+    def on_market_data(self, market_data: MarketData):
+        for algo_id in list(self.working_algos):
+            algo = self.algos.get(algo_id)
 
-            self.logger.debug(f'{algo} opening {ticker} {trade_side.side_name} {target_volume} position!')
-            self.algos[algo.algo_id] = self.working_algos[algo.algo_id] = algo
+            if algo is None:
+                continue
 
-            algo.launch(**kwargs)
-            self._update_status()
-            return algo
+            algo.on_market_data(market_data=market_data)
 
     def on_filled(self, report: TradeReport, **kwargs):
         order_id = report.order_id
         algo = self.reversed_order_mapping.get(order_id)
 
         if algo is None:
             return 0
 
         result = algo.on_filled(report=report, **kwargs)
         self._update_status()
+        self.clear_cache()
         return result
 
-    def add_exposure(self, ticker: str, volume: float, notional: float, side: TransactionSide, timestamp: float):
-        """
-        this is a method to add dummy algo and fills it.
-
-        the method provides an easy way to amend exposure
-        """
-
-        algo = self.algo_registry.to_algo(name=self.algo_registry.passive)(
-            handler=self,
-            ticker=ticker,
-            side=side,
-            target_volume=volume,
-            dma=None,
-        )
-        self.algos[algo.algo_id] = algo
-
-        order = TradeInstruction(ticker=ticker, order_id=f'Dummy.{uuid.uuid4().hex}', volume=volume, side=side)
-        report = TradeReport(ticker=ticker, volume=volume, notional=notional, side=side, timestamp=timestamp, order_id=order.order_id)
-        order.fill(report)
-        algo.status = algo.Status.done
-        algo.order[order.order_id] = order
-        self._update_status()
-
-        return report
-
     def on_canceled(self, order_id: str, **kwargs):
         algo = self.reversed_order_mapping.get(order_id)
 
         if algo is None:
             return 0
 
         result = algo.on_canceled(order_id=order_id, **kwargs)
         self._update_status()
+        self.clear_cache()
         return result
 
     def on_rejected(self, order: TradeInstruction, **kwargs):
         order_id = order.order_id
         algo = self.reversed_order_mapping.get(order_id)
 
         if algo is None:
             return 0
 
         result = algo.on_rejected(order=order, **kwargs)
         self._update_status()
+        self.clear_cache()
         return result
 
-    def unwind_all(self, **kwargs):
-        exposure = self.exposure_volume
-        additional_kwargs = kwargs.copy()
+    def on_algo_done(self, algo: AlgoTemplate):
+        self.working_algos.pop(algo.algo_id, None)
 
-        for ticker in exposure:
-            self.unwind_ticker(ticker, **additional_kwargs)
+    def on_algo_error(self, algo: AlgoTemplate):
+        self.working_algos.pop(algo.algo_id, None)
+        LOGGER.warning(f'{algo} encounter error, manual intervention')
 
-        return 0.
+    def open(self, ticker: str, target_volume: float, trade_side: TransactionSide, algo: str = None, **kwargs):
+        if algo is None:
+            algo = self.default_algo
+
+        if target_volume:
+            algo = self.algo_registry.to_algo(name=algo)(
+                handler=self,
+                ticker=ticker,
+                side=trade_side,
+                target_volume=target_volume,
+                dma=self.dma,
+                **kwargs
+            )
+
+            LOGGER.debug(f'{algo} opening {ticker} {trade_side.side_name} {target_volume} position!')
+            self.algos[algo.algo_id] = self.working_algos[algo.algo_id] = algo
+
+            algo.launch(**kwargs)
+            self._update_status()
+            return algo
 
     def unwind_ticker(self, ticker: str, **kwargs):
         LOGGER.info(f'fully cancel and unwind {ticker} position!')
 
         # cancel all
         for algo_id in list(self.algos):
             algo = self.algos.get(algo_id)
@@ -302,49 +305,74 @@
         # calculate exposure
         exposure = self.exposure_volume.get(ticker)
         working = self.working_volume.get(ticker, {})
         working_long = working.get('Long', 0)
         working_short = working.get('Short', 0)
 
         if not exposure:
-            self.logger.info(f'No exposure for {ticker}, no unwind actions!')
+            LOGGER.info(f'No exposure for {ticker}, no unwind actions!')
             # no exposure, good!
             return
         elif working_long and working_short:
             # with exposure, and working orders on both side, no action
-            self.logger.info(f'Multiple trade actions for {ticker}, skip unwind actions! Try again later!')
+            LOGGER.info(f'Multiple trade actions for {ticker}, skip unwind actions! Try again later!')
             return
         elif (exposure > 0 and working_short) or (exposure < 0 and working_long):
             # with exposure, and working unwinding orders, no action
-            self.logger.info(f'Unwinding actions exists for {ticker}, skip unwind actions! Try again later!')
+            LOGGER.info(f'Unwinding actions exists for {ticker}, skip unwind actions! Try again later!')
             return
 
         to_unwind = abs(exposure)
         side = TransactionSide.Sell_to_Unwind if exposure > 0 else TransactionSide.Buy_to_Cover
         self.open(ticker=ticker, target_volume=to_unwind, trade_side=side)
 
+    def add_exposure(self, ticker: str, volume: float, notional: float, side: TransactionSide, timestamp: float):
+        """
+        this is a method to add dummy algo and fills it.
+
+        the method provides an easy way to amend exposure
+        """
+
+        algo = self.algo_registry.to_algo(name=self.algo_registry.passive)(
+            handler=self,
+            ticker=ticker,
+            side=side,
+            target_volume=volume,
+            dma=None,
+        )
+        self.algos[algo.algo_id] = algo
+
+        order = TradeInstruction(ticker=ticker, order_id=f'Dummy.{uuid.uuid4().int}', volume=volume, side=side, timestamp=timestamp)
+        report = TradeReport(ticker=ticker, volume=volume, price=notional / volume if volume else np.nan, notional=notional, side=side, timestamp=timestamp, order_id=order.order_id)
+        order.fill(report)
+        algo.status = algo.Status.done
+        algo.order[order.order_id] = order
+        self._update_status()
+
+        return report
+
+    def unwind_all(self, **kwargs):
+        exposure = self.exposure_volume
+        additional_kwargs = kwargs.copy()
+
+        for ticker in exposure:
+            self.unwind_ticker(ticker, **additional_kwargs)
+
+        return 0.
+
     def cancel_all(self, **kwargs):
         # EMERGENCY ONLY
         for algo_id in list(self.working_algos):
             algo = self.algos.get(algo_id)
 
             if algo is not None:
                 algo.cancel(**kwargs)
 
         return 0
 
-    def on_market_data(self, market_data: MarketData):
-        for algo_id in list(self.working_algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is None:
-                continue
-
-            algo.on_market_data(market_data=market_data)
-
     def to_json(self, fmt='str') -> str | dict:
         json_dict = {}
         map_id = self.position_id
 
         json_dict[map_id] = {}
 
         # dump algos
@@ -363,38 +391,36 @@
         for algo_id in list(self.working_algos):
             algo = self.algos.get(algo_id)
 
             if algo is None:
                 continue
 
             if algo.status == algo.Status.closed or algo.status == algo.Status.done:
-                self.algo_done(algo=algo)
+                self.on_algo_done(algo=algo)
             elif algo.status == algo.Status.rejected or algo.status == algo.Status.error:
-                self.algo_error(algo=algo)
+                self.on_algo_error(algo=algo)
 
     def _algo_pnl(self, algo: AlgoTemplate):
         if algo.exposure_volume:
             if (market_price := self.market_price.get(algo.ticker)) is not None:
                 pnl = market_price * algo.exposure_volume * algo.multiplier + algo.cash_flow
             else:
                 pnl = np.nan
         else:
             pnl = algo.cash_flow
         return pnl
 
-    def algo_done(self, algo: AlgoTemplate):
-        self.working_algos.pop(algo.algo_id, None)
-
-    def algo_error(self, algo: AlgoTemplate):
-        self.working_algos.pop(algo.algo_id, None)
-        self.logger.warning(f'{algo} encounter error, manual intervention')
+    def clear_cache(self):
+        self._exposure = None
+        self._working = None
 
     def clear(self):
         self.algos.clear()
         self.working_algos.clear()
+        self.clear_cache()
 
     def pnl(self) -> dict[str, float]:
         pnl = {}
         for algo_id in list(self.algos):
             algo = self.algos.get(algo_id)
 
             if algo is None:
@@ -424,14 +450,18 @@
         """
         a dictionary indicating current working volume of all orders
 
         {'Long': +float, 'Short': +float}
 
         :return: a dict with non-negative numbers
         """
+
+        if not self.no_cache and self._working is not None:
+            return self._working
+
         working_long = {}
         working_short = {}
         working = {'Long': working_long, 'Short': working_short}
 
         for algo_id in list(self.working_algos):
             algo = self.algos.get(algo_id)
             ticker = algo.ticker
@@ -454,14 +484,18 @@
     @property
     def exposure_volume(self) -> dict[str, float]:
         """
         a dictionary indicating current net exposed volume of all orders
 
         :return: a dict with float numbers (positive and negatives)
         """
+
+        if not self.no_cache and self._exposure is not None:
+            return self._exposure
+
         exposure = {}
 
         for algo_id in list(self.algos):
             algo = self.algos.get(algo_id)
 
             if algo is not None:
                 ticker = algo.ticker
@@ -604,18 +638,19 @@
             raise ValueError('Must assign ether strategy or position_tracker')
 
     def pop(self, map_id: str):
         self.strategy.pop(map_id, None)
         self.position_tracker.pop(map_id, None)
 
     def get(self, **kwargs) -> PositionManagementService | None:
-        map_id = kwargs.pop('map_id', None)
+        map_id: str | None = kwargs.pop('map_id', None)
         strategy = kwargs.pop('strategy', None)
 
         if map_id is not None:
+            map_id: str
             return self.position_tracker.get(map_id)
         elif strategy is not None:
             map_id = self.reversed_strategy_mapping.get(id(strategy))
 
             if map_id is None:
                 raise KeyError(f'Can not found strategy {strategy}')
             return self.position_tracker.get(map_id)
@@ -749,21 +784,21 @@
                 continue
 
             pos_tracker = self.position_tracker[map_id]
             algo_json = json_dict[map_id]
 
             for algo_id in algo_json:
                 algo_dict = algo_json[algo_id]
-                algo = ALGO_ENGINE.from_json(algo_dict)
+                algo = pos_tracker.algo_engine.from_json(algo_dict)
                 pos_tracker.algos[algo.algo_id] = pos_tracker.working_algos[algo.algo_id] = algo
 
                 if algo.status == algo.Status.closed or algo.status == algo.Status.done:
-                    pos_tracker.algo_done(algo=algo)
+                    pos_tracker.on_algo_done(algo=algo)
                 elif algo.status == algo.Status.rejected or algo.status == algo.Status.error:
-                    pos_tracker.algo_error(algo=algo)
+                    pos_tracker.on_algo_error(algo=algo)
 
         return self
 
     def dump(self, file_path: str | pathlib.Path):
         file_path = pathlib.Path(file_path)
         dump_dir = file_path.parent
 
@@ -1016,15 +1051,15 @@
             working_order.update(tracker.working_order)
 
         return working_order
 
     @property
     def trades_today(self):
         trades = {}
-        from .MarketEngine import MDS
+        from .market_engine import MDS
 
         market_date = MDS.market_date
         if market_date is None:
             return {}
 
         for tracker_id in list(self.position_tracker):
             tracker = self.position_tracker.get(tracker_id)
@@ -1532,15 +1567,16 @@
 
         return True
 
     def check_order(self, ticker: str, volume: float, side: TransactionSide):
         fake_order = TradeInstruction(
             ticker=ticker,
             side=side,
-            volume=volume
+            volume=volume,
+            timestamp=self.mds.timestamp
         )
 
         return self.check(order=fake_order)
 
     def check_basket(self, *order: TradeInstruction):
         LOGGER.warning('risk control for basket order not implemented, check order individually')
 
@@ -1982,266 +2018,7 @@
 
         for key in ['max_ttl_notional_long', 'max_ttl_notional_short', 'max_net_notional_long', 'max_net_notional_short']:
             if rules[key] is not None:
                 info_dict['global'][key] = rules[key]
 
         return pd.DataFrame(info_dict).T
 
-
-class SimMatch(object):
-    def __init__(self, ticker, event_engine=None, **kwargs):
-        self.ticker = ticker
-        self.event_engine = event_engine if event_engine is not None else EVENT_ENGINE
-        self.topic_set = kwargs.pop('topic_set', TOPIC)
-
-        self.fee = kwargs.pop('fee', 0.)
-        self.working: dict[str, TradeInstruction] = {}
-        self.history: dict[str, TradeInstruction] = {}
-
-        self.market_time = datetime.datetime.min
-
-    def __call__(self, **kwargs):
-        order = kwargs.pop('order', None)
-        market_data = kwargs.pop('market_data', None)
-
-        if order is not None:
-            if order.order_type == OrderType.LimitOrder:
-                self.launch_order(order=order)
-            elif order.order_type == OrderType.CancelOrder:
-                self.cancel_order(order=order)
-            else:
-                raise ValueError(f'Invalid order {order}')
-
-        if market_data is not None:
-            self.market_time = max(self.market_time, market_data.market_time)
-
-            if isinstance(market_data, BarData):
-                self._check_bar_data(market_data=market_data)
-            elif isinstance(market_data, TickData):
-                self._check_tick_data(market_data=market_data)
-            elif isinstance(market_data, TradeData):
-                self._check_trade_data(market_data=market_data)
-            elif isinstance(market_data, OrderBook):
-                self._check_order_book(market_data=market_data)
-
-    def register(self, topic_set=None, event_engine=None):
-        if topic_set is not None:
-            self.topic_set = topic_set
-
-        if event_engine is not None:
-            self.event_engine = event_engine
-
-        self.event_engine.register_handler(topic=self.topic_set.launch_order(ticker=self.ticker), handler=self.launch_order)
-        self.event_engine.register_handler(topic=self.topic_set.cancel_order(ticker=self.ticker), handler=self.cancel_order)
-        self.event_engine.register_handler(topic=self.topic_set.realtime(ticker=self.ticker), handler=self)
-
-    def unregister(self):
-        self.event_engine.unregister_handler(topic=self.topic_set.launch_order(ticker=self.ticker), handler=self.launch_order)
-        self.event_engine.unregister_handler(topic=self.topic_set.cancel_order(ticker=self.ticker), handler=self.cancel_order)
-        self.event_engine.unregister_handler(topic=self.topic_set.realtime(ticker=self.ticker), handler=self)
-
-    def launch_order(self, order: TradeInstruction, **kwargs):
-        if (order.order_id in self.working) or (order.order_id in self.history):
-            raise ValueError(f'Invalid instruction {order}, OrderId already in working or history')
-        elif order.limit_price is None:
-            LOGGER.warning(f'order {order} does not have a valid limit price!')
-            # raise ValueError(f'Invalid instruction {order}, instruction must have a LimitPrice')
-
-        order.set_order_state(order_state=OrderState.Placed, market_datetime=self.market_time)
-        self.working[order.order_id] = order
-        if 'market_time' not in kwargs:
-            kwargs['market_time'] = self.market_time
-        self.on_order(order=order, **kwargs)
-
-    def cancel_order(self, order: TradeInstruction = None, order_id: str = None, **kwargs):
-        if order is None and order_id is None:
-            raise ValueError('Must assign a order or order_id to cancel order')
-        elif order_id is None:
-            order_id = order.order_id
-
-        # if order_id not in self.working:
-        #     raise ValueError(f'Invalid cancel order {order}, OrderId not found')
-
-        order: TradeInstruction = self.working.pop(order_id, None)
-        if order is None:
-            LOGGER.info(f'[{self.market_time:%Y-%m-%d %H:%M:%S}] failed to cancel {order_id} order!')
-            return
-
-        if order.order_state == OrderState.Filled:
-            pass
-        else:
-            order.set_order_state(order_state=OrderState.Canceled, market_datetime=self.market_time)
-            LOGGER.info(f'[{self.market_time:%Y-%m-%d %H:%M:%S}] Sim-canceled {order.side.name} {order.ticker} order!')
-
-        self.history[order_id] = order
-        self.on_order(order=order, **kwargs)
-
-    def _check_bar_data(self, market_data: BarData):
-        for order_id in list(self.working):
-            order = self.working.get(order_id)
-            if order is None:
-                pass
-            elif order.order_state in [OrderState.Placed, OrderState.PartFilled]:
-                if order.side.sign > 0:
-                    # match order based on worst offer
-                    if order.limit_price is None:
-                        self._match(order=order, match_price=market_data.VWAP)
-                    elif market_data.high_price < order.limit_price:
-                        self._match(order=order, match_price=market_data.high_price)
-                    # match order based on limit price
-                    elif market_data.low_price < order.limit_price:
-                        self._match(order=order, match_price=order.limit_price)
-                    # no match
-                    else:
-                        pass
-                elif order.side.sign < 0:
-                    # match order based on worst offer
-                    if order.limit_price is None:
-                        self._match(order=order, match_price=market_data.VWAP)
-                    elif market_data.low_price > order.limit_price:
-                        self._match(order=order, match_price=market_data.low_price)
-                    # match order based on limit price
-                    elif market_data.high_price > order.limit_price:
-                        self._match(order=order, match_price=order.limit_price)
-                    # no match
-                    else:
-                        pass
-            else:
-                continue
-                # raise ValueError(f'Invalid working order state {order}')
-
-    def _check_trade_data(self, market_data: TradeData):
-        for order_id in list(self.working):
-            order = self.working.get(order_id)
-            if order is None:
-                pass
-            elif order.is_working:
-                if order.start_time > market_data.market_time:
-                    pass
-                elif order.limit_price is None:
-                    if order.side.sign * market_data.side.sign > 0:
-                        self._match(order=order, match_volume=market_data.volume, match_price=market_data.market_price)
-                elif order.side.sign > 0 and market_data.market_price < order.limit_price:
-                    self._match(order=order, match_volume=market_data.volume, match_price=market_data.market_price)
-                elif order.side.sign < 0 and market_data.market_price > order.limit_price:
-                    self._match(order=order, match_volume=market_data.volume, match_price=market_data.market_price)
-            else:
-                continue
-                # raise ValueError(f'Invalid working order state {order}')
-
-    def _check_order_book(self, market_data: OrderBook):
-        for order_id in list(self.working):
-            order = self.working.get(order_id)
-
-            match_volume = 0.
-            match_notional = 0.
-
-            if order is None:
-                pass
-            elif order.order_state in [OrderState.Placed, OrderState.PartFilled]:
-                if order.limit_price is None:
-                    if order.side.sign > 0:
-                        for entry in market_data.ask:
-                            if match_volume < order.working_volume:
-                                addition_volume = min(entry.volume, order.working_volume - match_volume)
-                                match_volume += addition_volume
-                                match_notional += addition_volume * entry.price
-                            else:
-                                break
-                    else:
-                        for entry in market_data.bid:
-                            if match_volume < order.working_volume:
-                                addition_volume = min(entry.volume, order.working_volume - match_volume)
-                                match_volume += addition_volume
-                                match_notional += addition_volume * entry.price
-                            else:
-                                break
-                elif order.side.sign > 0 and market_data.best_ask_price <= order.limit_price:
-                    for entry in market_data.ask:
-                        if entry.price <= order.limit_price:
-                            if match_volume < order.working_volume:
-                                addition_volume = min(entry.volume, order.working_volume - match_volume)
-                                match_volume += addition_volume
-                                match_notional += addition_volume * entry.price
-                            else:
-                                break
-                        else:
-                            break
-                elif order.side.sign < 0 and market_data.best_bid_price >= order.limit_price:
-                    for entry in market_data.bid:
-                        if entry.price >= order.limit_price:
-                            if match_volume < order.working_volume:
-                                addition_volume = min(entry.volume, order.working_volume - match_volume)
-                                match_volume += addition_volume
-                                match_notional += addition_volume * entry.price
-                            else:
-                                break
-                        else:
-                            break
-
-                if match_volume:
-                    self._match(order=order, match_volume=match_volume, match_price=match_notional / match_volume)
-            else:
-                continue
-                # raise ValueError(f'Invalid working order state {order}')
-
-    def _check_tick_data(self, market_data: TickData):
-        return self._check_order_book(market_data=market_data.order_book)
-
-    def _match(self, order: TradeInstruction, match_volume: float = None, match_price: float = None):
-        if match_volume is None:
-            match_volume = order.working_volume
-        elif match_volume > order.working_volume:
-            match_volume = order.working_volume
-
-        if order.limit_price is None:
-            pass
-        elif match_price is None:
-            match_price = order.limit_price
-        elif order.side.sign > 0 and match_price > order.limit_price:
-            LOGGER.warning(f'match price greater than limit price for bid order {order}')
-            match_price = order.limit_price
-        elif order.side.sign < 0 and match_price < order.limit_price:
-            match_price = order.limit_price
-            LOGGER.warning(f'match price less than limit price for ask order {order}')
-
-        if match_volume:
-            report = TradeReport(
-                ticker=order.ticker,
-                side=order.side,
-                volume=match_volume,
-                notional=match_volume * match_price * order.multiplier,
-                trade_time=self.market_time,
-                order_id=order.order_id,
-                price=match_price,
-                multiplier=order.multiplier,
-                fee=self.fee * match_volume * match_price * order.multiplier
-            )
-
-            LOGGER.info(f'[{self.market_time:%Y-%m-%d %H:%M:%S}] Sim-filled {order.ticker} {order.side.name} {report.volume:,.2f} @ {report.price:.2f}')
-            order.fill(trade_report=report)
-
-            if order.order_state == OrderState.Filled:
-                self.working.pop(order.order_id, None)
-                self.history[order.order_id] = order
-
-            self.on_report(report=report)
-            self.on_order(order=order)
-            return report
-        else:
-            return None
-
-    def on_order(self, order, **kwargs):
-        self.event_engine.put(topic=self.topic_set.on_order, order=order)
-
-    def on_report(self, report, **kwargs):
-        self.event_engine.put(topic=self.topic_set.on_report, report=report, **kwargs)
-
-    def eod(self):
-        for order_id in list(self.working):
-            self.cancel_order(order_id=order_id)
-
-    def clear(self):
-        self.fee = 0.
-        self.working.clear()
-        self.history.clear()
-        self.market_time = datetime.datetime.min
```

### Comparing `PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/BackTest.py` & `pyalgoengine-0.4.0/algo_engine/back_test/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from __future__ import annotations
+__package__ = 'algo_engine.back_test'
 
 import datetime
+from typing import Callable
 
 import EventEngine
 
-from . import EventDMA
-from ._StrategyEngine import StrategyEngine
-from ..Engine import LOGGER, TOPIC, MarketDataService, Balance, RiskProfile, PositionManagementService
-from ..Engine.AlgoEngine import AlgoRegistry, AlgoEngine
-
-LOGGER = LOGGER.getChild('BackTest')
+from ..engine import TOPIC, MarketDataService, Balance, RiskProfile, PositionManagementService
+from ..engine.algo_engine import AlgoRegistry, AlgoEngine
+from ..strategie import EventDMA
+from ..strategie.strategy_engine import StrategyEngine
 
 
 def test_stop(code=0):
     EVENT_ENGINE.stop()
     # noinspection PyUnresolvedReferences, PyProtectedMember
     # `import os`
     # `os._exit(code)`
 
 
-def test_start(start_date: datetime.date, end_date: datetime.date, data_loader: callable, **kwargs):
+def test_start(start_date: datetime.date, end_date: datetime.date, data_loader: Callable, **kwargs):
     EVENT_ENGINE.start()
     STRATEGY_ENGINE.back_test(
         start_date=start_date,
         end_date=end_date,
         data_loader=data_loader,
         **kwargs
     )
```

### Comparing `PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/_StrategyEngine.py` & `pyalgoengine-0.4.0/algo_engine/strategie/strategy_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from __future__ import annotations
-
 import abc
 import datetime
 import threading
 import time
+from typing import Callable
 
 from PyQuantKit import MarketData, TradeReport, TradeInstruction, TransactionSide
 
-from ..Engine import PositionManagementService, TOPIC, EVENT_ENGINE, SimMatch, LOGGER, MDS
-
-LOGGER = LOGGER.getChild('StrategyEngine')
+from . import LOGGER
+from ..back_test import SimMatch, ProgressiveReplay
+from ..engine import PositionManagementService, TOPIC, EVENT_ENGINE, MDS
 
 
 class StrategyEngineTemplate(object, metaclass=abc.ABCMeta):
     def __init__(self, position_tracker: PositionManagementService):
         self.position_tracker = position_tracker
 
     def __call__(self, **kwargs):
@@ -185,22 +184,33 @@
         if topic_set is None:
             topic_set = self.topic_set
 
         event_engine.register_handler(topic=topic_set.realtime, handler=self.__call__)
         event_engine.register_handler(topic=topic_set.on_order, handler=self.on_order)
         event_engine.register_handler(topic=topic_set.on_report, handler=self.on_report)
 
+    def unregister(self, event_engine=None, topic_set=None):
+        if event_engine is None:
+            event_engine = self.event_engine
+
+        if topic_set is None:
+            topic_set = self.topic_set
+
+        event_engine.unregister_handler(topic=topic_set.realtime, handler=self.__call__)
+        event_engine.unregister_handler(topic=topic_set.on_order, handler=self.on_order)
+        event_engine.unregister_handler(topic=topic_set.on_report, handler=self.on_report)
+
     def cancel(self, ticker: str, side: TransactionSide = None, algo_id: str = None, order_id: str = None, **kwargs):
         position_tracker = self.position_tracker
 
         if algo_id is not None:
             algo_id = position_tracker.reversed_order_mapping.get(order_id).algo_id
             if algo_id:
                 LOGGER.info(f'No algo_id specified, found algo {algo_id} associated with order_id {order_id}! Canceling all trade action associated with algo')
-                LOGGER.warning('Strategy should not cancel single trade order, this will break the AlgoEngine Consistency!')
+                LOGGER.warning('Strategy should not cancel single trade order, this will break the algo_engine Consistency!')
 
         if not algo_id:
             LOGGER.warning(f'No algo_id given! Canceling all {ticker} {side.side_name} algos!')
 
             for _algo_id in list(self.algos):
                 algo = self.algos.get(_algo_id)
 
@@ -334,17 +344,15 @@
             handler(market_date=market_date, **kwargs)
 
     def bod(self, market_date: datetime.date, **kwargs):
 
         for handler in self._on_bod:
             handler(market_date=market_date, **kwargs)
 
-    def back_test(self, start_date: datetime.date, end_date: datetime.date, data_loader: callable, **kwargs):
-        from ..Engine import ProgressiveReplay
-
+    def back_test(self, start_date: datetime.date, end_date: datetime.date, data_loader: Callable, **kwargs):
         replay = ProgressiveReplay(
             loader=data_loader,
             tickers=list(self.subscription),
             dtype=['TickData', 'TradeData'],
             start_date=start_date,
             end_date=end_date,
             bod=self.bod,
```

### Comparing `PyAlgoEngine-0.3.9.post4/AlgoEngine/Strategies/__init__.py` & `pyalgoengine-0.4.0/algo_engine/strategie/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-from __future__ import annotations
-
-import threading
+from threading import Lock
 
 from PyQuantKit import TradeInstruction
 
-from ._StrategyEngine import StrategyEngine
-from ..Engine import LOGGER
-from ..Engine.EventEngine import EVENT_ENGINE, TOPIC
-from ..Engine.MarketEngine import MDS, MarketDataService
-from ..Engine.TradeEngine import Balance, Inventory, DirectMarketAccess, RiskProfile, PositionManagementService
+from .strategy_engine import StrategyEngine
+from .. import LOGGER
+from ..engine import EVENT_ENGINE, TOPIC, MDS, MarketDataService, Balance, Inventory, DirectMarketAccess, RiskProfile, PositionManagementService
 
 LOGGER = LOGGER.getChild('Strategies')
 
 
 class EventDMA(DirectMarketAccess):
     def __init__(self, mds: MarketDataService, risk_profile: RiskProfile, event_engine=None, cool_down: float = None):
         self.event_engine = EVENT_ENGINE if event_engine is None else event_engine
@@ -24,15 +20,15 @@
     def _cancel_order_handler(self, order: TradeInstruction, **kwargs):
         self.event_engine.put(topic=TOPIC.cancel_order(ticker=order.ticker), order_id=order.order_id, **kwargs)
 
     def _reject_order_handler(self, order: TradeInstruction, **kwargs):
         raise NotImplementedError()
 
 
-REPLAY_LOCK = threading.Lock()
+REPLAY_LOCK = Lock()
 INVENTORY = Inventory()
 BALANCE = Balance(inventory=INVENTORY)
 RISK_PROFILE = RiskProfile(mds=MDS, balance=BALANCE)
 DMA = EventDMA(mds=MDS, risk_profile=RISK_PROFILE)
 POSITION_TRACKER = PositionManagementService(dma=DMA)
 STRATEGY_ENGINE = StrategyEngine(event_engine=EVENT_ENGINE, position_tracker=POSITION_TRACKER)
 BALANCE.add(strategy=STRATEGY_ENGINE, position_tracker=POSITION_TRACKER)
```

### Comparing `PyAlgoEngine-0.3.9.post4/LICENSE` & `pyalgoengine-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAlgoEngine-0.3.9.post4/PKG-INFO` & `pyalgoengine-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.3.9.post4
+Version: 0.4.0
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: exchange_calendars
-Requires-Dist: PyQuantKit
-Requires-Dist: PyEventEngine
+Requires-Dist: PyQuantKit>=0.3.0
+Requires-Dist: PyEventEngine>=0.3.0.post3
 
 # PyAlgoEngine
 python algo trading engine
```

### Comparing `PyAlgoEngine-0.3.9.post4/PyAlgoEngine.egg-info/PKG-INFO` & `pyalgoengine-0.4.0/PyAlgoEngine.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.3.9.post4
+Version: 0.4.0
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: exchange_calendars
-Requires-Dist: PyQuantKit
-Requires-Dist: PyEventEngine
+Requires-Dist: PyQuantKit>=0.3.0
+Requires-Dist: PyEventEngine>=0.3.0.post3
 
 # PyAlgoEngine
 python algo trading engine
```

### Comparing `PyAlgoEngine-0.3.9.post4/setup.py` & `pyalgoengine-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,33 +20,35 @@
     raise RuntimeError("Unable to find version string.")
 
 
 long_description = read("README.md")
 
 setuptools.setup(
     name="PyAlgoEngine",
-    version=get_version(os.path.join('AlgoEngine', '__init__.py')),
+    version=get_version(os.path.join('algo_engine', '__init__.py')),
     author="Bolun.Han",
     author_email="Bolun.Han@outlook.com",
     description="Basic algo engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BolunHan/PyAlgoEngine",
     packages=setuptools.find_packages(),
     include_package_data=True,
     package_data={
     },
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.8',
+    python_requires='>=3.1',
     install_requires=[
         'numpy',
         'pandas',
         'exchange_calendars',
-        'PyQuantKit',
-        'PyEventEngine',
+        'PyQuantKit>=0.3.0',
+        'PyEventEngine>=0.3.0.post3',
     ]
 )
```

