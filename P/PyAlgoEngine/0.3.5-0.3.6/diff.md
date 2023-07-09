# Comparing `tmp/PyAlgoEngine-0.3.5.tar.gz` & `tmp/PyAlgoEngine-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAlgoEngine-0.3.5.tar", last modified: Thu Jun 22 05:29:59 2023, max compression
+gzip compressed data, was "PyAlgoEngine-0.3.6.tar", last modified: Sun Jul  9 05:29:43 2023, max compression
```

## Comparing `PyAlgoEngine-0.3.5.tar` & `PyAlgoEngine-0.3.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-22 05:29:59.047923 PyAlgoEngine-0.3.5/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-22 05:29:57.915037 PyAlgoEngine-0.3.5/AlgoEngine/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-22 05:29:58.375515 PyAlgoEngine-0.3.5/AlgoEngine/Engine/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    31968 2023-06-18 06:25:52.000000 PyAlgoEngine-0.3.5/AlgoEngine/Engine/AlgoEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1517 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.5/AlgoEngine/Engine/EventEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    32583 2023-06-21 12:41:22.000000 PyAlgoEngine-0.3.5/AlgoEngine/Engine/MarketEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    81457 2023-06-21 11:54:46.000000 PyAlgoEngine-0.3.5/AlgoEngine/Engine/TradeEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3754 2023-06-17 05:15:57.000000 PyAlgoEngine-0.3.5/AlgoEngine/Engine/__init__.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-22 05:29:58.645474 PyAlgoEngine-0.3.5/AlgoEngine/Strategies/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1866 2023-06-18 06:25:52.000000 PyAlgoEngine-0.3.5/AlgoEngine/Strategies/BackTest.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    12684 2023-06-21 11:52:19.000000 PyAlgoEngine-0.3.5/AlgoEngine/Strategies/_StrategyEngine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1778 2023-06-18 06:25:52.000000 PyAlgoEngine-0.3.5/AlgoEngine/Strategies/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      444 2023-06-21 12:41:36.000000 PyAlgoEngine-0.3.5/AlgoEngine/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1087 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.5/LICENSE
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      515 2023-06-22 05:29:59.040926 PyAlgoEngine-0.3.5/PKG-INFO
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-22 05:29:58.972763 PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      515 2023-06-22 05:29:51.000000 PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/PKG-INFO
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      499 2023-06-22 05:29:53.000000 PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/SOURCES.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2023-06-22 05:29:51.000000 PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/dependency_links.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       56 2023-06-22 05:29:51.000000 PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/requires.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       11 2023-06-22 05:29:51.000000 PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/top_level.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       44 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.5/README.md
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2023-06-22 05:29:59.051238 PyAlgoEngine-0.3.5/setup.cfg
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1579 2023-06-12 04:21:56.000000 PyAlgoEngine-0.3.5/setup.py
+drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2023-07-09 05:29:43.305027 PyAlgoEngine-0.3.6/
+drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2023-07-09 05:29:43.301026 PyAlgoEngine-0.3.6/AlgoEngine/
+drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2023-07-09 05:29:43.301026 PyAlgoEngine-0.3.6/AlgoEngine/Engine/
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)    31104 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Engine/AlgoEngine.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)     1465 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Engine/EventEngine.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)    31699 2023-07-09 05:24:08.000000 PyAlgoEngine-0.3.6/AlgoEngine/Engine/MarketEngine.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)    79235 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Engine/TradeEngine.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)     3653 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Engine/__init__.py
+drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2023-07-09 05:29:43.301026 PyAlgoEngine-0.3.6/AlgoEngine/Strategies/
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)     1814 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Strategies/BackTest.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)    12359 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Strategies/_StrategyEngine.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)     1738 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/AlgoEngine/Strategies/__init__.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)      426 2023-07-09 05:27:54.000000 PyAlgoEngine-0.3.6/AlgoEngine/__init__.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)     1066 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/LICENSE
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)      515 2023-07-09 05:29:43.305027 PyAlgoEngine-0.3.6/PKG-INFO
+drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2023-07-09 05:29:43.305027 PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)      515 2023-07-09 05:29:43.000000 PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/PKG-INFO
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)      499 2023-07-09 05:29:43.000000 PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/SOURCES.txt
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)        1 2023-07-09 05:29:43.000000 PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/dependency_links.txt
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)       57 2023-07-09 05:29:43.000000 PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/requires.txt
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)       11 2023-07-09 05:29:43.000000 PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/top_level.txt
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)       42 2023-07-09 04:44:22.000000 PyAlgoEngine-0.3.6/README.md
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)       38 2023-07-09 05:29:43.305027 PyAlgoEngine-0.3.6/setup.cfg
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)     1528 2023-07-09 05:26:34.000000 PyAlgoEngine-0.3.6/setup.py
```

### Comparing `PyAlgoEngine-0.3.5/AlgoEngine/Engine/AlgoEngine.py` & `PyAlgoEngine-0.3.6/AlgoEngine/Engine/AlgoEngine.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,864 +1,864 @@
-from __future__ import annotations
-
-import abc
-import datetime
-import enum
-import functools
-import json
-import threading
-import uuid
-from typing import Type
-
-import numpy as np
-from PyQuantKit import TransactionSide, TradeInstruction, MarketData, TradeReport, OrderState, OrderType
-
-from . import LOGGER
-from .MarketEngine import MDS
-
-LOGGER = LOGGER.getChild('AlgoEngine')
-__all__ = ['AlgoTemplate', 'AlgoRegistry', 'AlgoEngine', 'ALGO_ENGINE', 'ALGO_REGISTRY']
-
-
-class AlgoStatus(enum.Enum):
-    idle = 'idle'  # init state 
-    preparing = 'preparing'  # preparing
-    ready = 'ready'  # ready to launch order
-    working = 'working'  # order launched
-    done = 'done'  # transaction complete!
-    closed = 'closed'  # transaction failed and close
-    stopping = 'stopping'  # trying to stop transaction
-    rejected = 'rejected'  # internal / external rejected
-    error = 'error'  # internal / external error
-
-
-class AlgoTemplate(object, metaclass=abc.ABCMeta):
-    Status = AlgoStatus
-
-    def __init__(self, dma, ticker: str, target_volume: float, side: TransactionSide, **kwargs):
-        """ Template for trading algorithm
-        an abstract class to create a trading algorithm
-
-        :param dma: direct market access
-        :param ticker: the given symbol of the underlying to trade
-        :param target_volume: the given volume to trade
-        :param side: the given TransactionSide
-        :keyword algo_engine: the algo_engine instance, default is ALGO_ENGINE
-        :keyword logger: the logger instance, default is LOGGER
-        :keyword algo_id: the id of the algo, default is uuid4()
-        """
-        self.dma = dma
-        self.ticker = ticker
-        self.side = side
-        self.target_volume = target_volume
-        self.algo_engine = kwargs.pop('algo_engine', ALGO_ENGINE)
-        self.algo_type = kwargs.get('algo_type', self.algo_engine.registry.reversed_registry[self.__class__.__name__])
-        self.logger = kwargs.pop('logger', LOGGER)
-        self.algo_id = kwargs.pop('algo_id', uuid.uuid4().hex)
-
-        self.status: AlgoStatus = self.Status.idle
-        self._target_progress = 0
-        self._lock = threading.Lock()
-        self._thread = threading.Thread(target=self.work)
-
-        self.working_order: dict[str, TradeInstruction] = {}
-        self.order: dict[str, TradeInstruction] = {}
-
-        self.is_active = False
-        self.start_time = None
-        self.finish_time = None
-
-    def __repr__(self):
-        return f'<TradeAlgo>(ticker={self.ticker}, target={self.side.sign * self.target_volume}, done={self.side.sign * self.exposure_volume}, algo={self.__class__.__name__}, status={self.status.value}, id={id(self)})'
-
-    def on_sync_progress(self, progress: float, **kwargs):
-        self._target_progress = max(min(progress, 1), 0)
-        self._sync(progress=progress, **kwargs)
-
-    def on_market_data(self, market_data: MarketData, **kwargs):
-        pass
-
-    def on_filled(self, report: TradeReport, **kwargs):
-        if report.order_id in self.working_order:
-            self._filled(order=self.working_order[report.order_id], report=report, **kwargs)
-            return 1
-        else:
-            self.logger.warning(f'[Failed to fill] {self} has no matching for working order {report.order_id}')
-            return 0
-
-    def on_canceled(self, order_id: str = None, **kwargs):
-        if order_id in self.working_order:
-            self._canceled(order=self.working_order[order_id], **kwargs)
-            return 1
-        else:
-            self.logger.warning(f'[Failed to cancel] {self} has no matching for working order {order_id}')
-            return 0
-
-    def on_rejected(self, order: TradeInstruction, **kwargs):
-        if order.order_id in self.working_order:
-            self._rejected(order=order, **kwargs)
-            return 1
-        else:
-            self.logger.warning(f'[Failed to reject] {self} has no matching for working order {order.order_id}')
-            return 0
-
-    def recover(self):
-        self._update_working_order()
-
-        if not self.working_volume:
-            if self.exposure_volume:
-                self._update_status(status=self.Status.done)
-            else:
-                self._update_status(status=self.Status.closed)
-            LOGGER.info(f'{self} recovery successful! status {self.status}')
-        else:
-            LOGGER.warning(f'Caution! Recovering WORKING trade handler {self} may cause unexpected error!')
-            self._update_status(status=self.Status.working)
-
-    def _update_working_order(self):
-        """
-        refresh working order, to remove the finished orders
-        :return: a dict of working orders
-        """
-        for order_id in list(self.working_order):
-            order = self.working_order.get(order_id)
-
-            if order is None:
-                continue
-
-            if order.is_done:
-                self.working_order.pop(order_id, None)
-
-        return self.working_order
-
-    def _update_status(self, status=None, sync_pos=True, **kwargs):
-        """
-        ._update_status provides a method to clear working orders and auto assign status
-        ._update_status DOES NOT call .on_filled, .on_rejected nor .on_canceled, these method is triggered by position management service
-        ._update_status should be called in .on_filled .on_rejected and .on_canceled
-
-        as the result of concurrency, assigning status while sync_pos may cause unexpected result, use with caution
-
-        :param status: the given status
-        :param sync_pos: whether to auto-clear working orders
-        :param kwargs: market_time to assign the exact time when status is changed, used in backtesting
-        """
-        if sync_pos:
-            self._update_working_order()
-
-        if 'market_time' in kwargs:
-            self.start_time = kwargs['market_time']
-
-        # update status with given status and datetime
-        if status is not None:
-            if isinstance(status, self.Status):
-                self.status = status
-            else:
-                raise TypeError(f'Invalid status {status}')
-        # update status with self info
-        else:
-            # with working order
-            if self.working_order:
-                if self.status == self.Status.idle:
-                    self.status = self.Status.working
-            # without any working order
-            else:
-                if self.filled_volume == self.target_volume:
-                    self.status = self.Status.done
-
-        return self.status
-
-    def _launch(self, order, **kwargs):
-        self.dma.launch_order(order=order, **kwargs)
-        # order launched, order state can be pending, placed, or rejected (by internal on_order risk control)
-        # DO NOT assume order state is_working, it may be rejected!
-        # DO NOT assume order is in .working_order, it may be rejected!
-        # DO NOT assume algo state is working, it may be rejected!
-        # therefor calling _update_status is recommended but still optional.
-        # self._update_status(sync_pos=False)
-
-    def _cancel_order(self, order, **kwargs):
-        self.dma.cancel_order(order=order, **kwargs)
-        # self._update_status(sync_pos=False)
-
-    def _filled(self, order: TradeInstruction, report: TradeReport, **kwargs):
-        """
-        callback on order filled / part-filled
-
-        this callback will REMOVE filled order from working order dict and update algo status
-        :param order: the given filled order
-        :param kwargs: keyword args for updating status. e.g. timestamp
-        """
-        if report.trade_id not in order.trades:
-            order.fill(trade_report=report)
-
-        kwargs['sync_pos'] = True
-        self._update_status(**kwargs)
-
-    def _canceled(self, order: TradeInstruction, **kwargs):
-        """
-        callback on order canceled
-
-        this callback will REMOVE cancelled order from working order dict and update algo status
-        :param order: the given canceled order
-        :param kwargs: keyword args for updating status. e.g. timestamp
-        """
-        self._update_working_order()
-        kwargs['sync_pos'] = False
-
-        if self.working_order:
-            self._update_status(status=self.Status.working, **kwargs)
-        elif self.exposure_volume:
-            self._update_status(status=self.Status.done, **kwargs)
-        else:
-            self._update_status(status=self.Status.closed, **kwargs)
-
-    def _rejected(self, order: TradeInstruction, **kwargs):
-        self._update_status(status=self.Status.rejected, **kwargs)
-
-    def _sync(self, progress, **kwargs):
-        ...
-
-    def to_json(self, fmt='str') -> str | dict:
-        json_dict = {
-            'algo_type': self.algo_type,
-            'ticker': self.ticker,
-            'side': self.side.name,
-            'target_volume': self.target_volume,
-            'algo_id': self.algo_id,
-            'status': self.status.name,
-            'target_progress': self._target_progress,
-            'start_time': datetime.datetime.timestamp(self.start_time) if self.start_time else None,
-            'finish_time': datetime.datetime.timestamp(self.finish_time) if self.finish_time else None,
-            'order': {_: self.order[_].to_json(fmt='dict') for _ in self.order},
-        }
-
-        if fmt == 'dict':
-            return json_dict
-        else:
-            return json.dumps(json_dict)
-
-    def from_json(self, json_str: str | dict):
-        if isinstance(json_str, (str, bytes)):
-            json_dict = json.loads(json_str)
-        elif isinstance(json_str, dict):
-            json_dict = json_str
-        else:
-            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
-
-        self.ticker = json_dict['ticker']
-        self.side = TransactionSide(json_dict['side'])
-        self.target_volume = json_dict['target_volume']
-        self.algo_id = json_dict['algo_id']
-        self.status = self.Status[json_dict['status']]
-        self._target_progress = json_dict['target_progress']
-        self.start_time = None if json_dict['start_time'] is None else datetime.datetime.fromtimestamp(json_dict['start_time'])
-        self.finish_time = None if json_dict['finish_time'] is None else datetime.datetime.fromtimestamp(json_dict['finish_time'])
-        self.order = {_: TradeInstruction.from_json(json_dict['order'][_]) for _ in json_dict['order']}
-        self.working_order = {order_id: order for order_id, order in self.order.items() if not order.is_done}
-
-        return self
-
-    @abc.abstractmethod
-    def work(self):
-        ...
-
-    @abc.abstractmethod
-    def launch(self, **kwargs) -> list[TradeInstruction]:
-        """
-        launch is a method to initiate the algo and launching orders.
-        this method will set the algo is_active = true
-        this method will set a new algo state, usually idle -> working
-        launch method is designed to be called by strategy / position management service.
-
-        :param kwargs: other keywords needed to launch an algo
-        :return: a list of working orders. Noted, that not all working order is returned by this method, for example, TWAP algo will init a sequence of order and return later.
-        """
-        ...
-
-    @abc.abstractmethod
-    def cancel(self, **kwargs):
-        """
-        cancel is a method to cancel / stop ALL working orders
-        this method will set the algo is_active = false
-        this method may set a new algo state, usually working -> stopping
-        launch method is designed to be called by strategy / position management service.
-
-        :param kwargs: other keywords needed to cancel an algo
-        :return: None
-        """
-        ...
-
-    @property
-    def trades(self) -> dict[str, TradeReport]:
-        trades = {}
-
-        for order in list(self.order.values()):
-            for trade_id in list(order.trades):
-                trade_report = order.trades.get(trade_id)
-
-                if trade_report is None:
-                    continue
-
-                trades[trade_report.trade_id] = trade_report
-
-        return trades
-
-    @property
-    def average_price(self) -> float:
-        adjust_volume = 0.
-        notional = 0.
-
-        for report in list(self.trades.values()):
-            if report.price == 0:
-                adjust_volume += report.volume
-            else:
-                adjust_volume += report.notional / report.price
-            notional += report.notional
-
-        if adjust_volume == 0:
-            return np.nan
-        else:
-            return notional / adjust_volume
-
-    @property
-    def exposure_volume(self) -> float:
-        """
-        <WITH SIGN> net exposed VOLUME indicating the exposure of the pos
-        :return: float
-        """
-        exposure = 0.
-
-        for report in list(self.trades.values()):
-            exposure += report.volume * report.side.sign
-
-        return exposure
-
-    @property
-    def working_volume(self) -> float:
-        """
-        <WITHOUT SIGN> net working VOLUME indicating the working status of the pos
-        :return: float
-        """
-        working = 0.
-
-        for order_id in self.working_order:
-            working_order = self.working_order.get(order_id)
-
-            if working_order is None:
-                continue
-
-            working += working_order.working_volume  # should be all positive
-
-        return working
-
-    @property
-    def filled_volume(self) -> float:
-        """
-        <WITHOUT SIGN> filled VOLUME
-        :return: float
-        """
-        volume = 0.
-
-        for report in list(self.trades.values()):
-            volume += report.volume
-
-        return volume
-
-    @property
-    def filled_notional(self) -> float:
-        """
-        <POSSIBLY WITH SIGN> total filled Notional
-        :return: float
-        """
-        notional = 0.
-
-        for report in list(self.trades.values()):
-            notional += report.notional  # which should be a POSITIVE number in normal cases.
-
-        return notional
-
-    @property
-    def fee(self) -> float:
-        """
-        <POSSIBLY WITH SIGN> total transaction fee
-        :return: float
-        """
-        total_fee = 0.
-
-        for report in list(self.trades.values()):
-            total_fee += report.fee
-
-        return total_fee
-
-    @property
-    def cash_flow(self) -> float:
-        """
-        <WITH SIGN> total cash flow
-        :return: float
-        """
-        cash_flow = -self.filled_notional * self.side.sign
-        return cash_flow
-
-    @property
-    def multiplier(self) -> float:
-        if self.order:
-            return self.order[list(self.order)[0]].multiplier
-        else:
-            return 1.0
-
-    @property
-    def filled_progress(self):
-        return self.filled_volume / self.target_volume
-
-    @property
-    def placed_progress(self):
-        return abs(self.working_volume / self.target_volume) + self.filled_progress
-
-    @property
-    def target_progress(self):
-        return self._target_progress
-
-    @property
-    def market_price(self):
-        return self.algo_engine.mds.market_price.get(self.ticker)
-
-    @property
-    def market_time(self):
-        return self.algo_engine.mds.market_time
-
-
-class Passive(AlgoTemplate):
-    """ Passive trading algorithm
-    Passive is a basic trading algo which trades all target volume into one single LIMIT order.
-    Algo will stop after order get filled or canceled.
-    no additional order will be launched except the initial one
-
-    a limit price can be set by keyword arguments, see also in doc: AlgoEngine.calculate_limit
-
-    """
-
-    def __init__(self, **kwargs):
-        """
-        init a Passive trade algo
-
-        requires all params from AlgoTemplate and additional following 4
-        :keyword limit_price: the absolute limit price of the order
-        :keyword limit_adjust_factor: limit price = market_price * (1 + factor) for long order else limit price = market_price * (1 - factor) for short order
-        :keyword limit_adjust_level:  for long order, limit price = bid[lvl] if lvl > 0 else ask[lvl] for lvl < 0.
-        :keyword limit_mode: if multiple limit price standard is provided, use "strict" to select strictest limit price or "loose" to select loosest one. Default is None, which is "strict".
-        """
-        self.limit_price = kwargs.pop('limit_price', None)
-        self.limit_adjust_factor = kwargs.pop('limit_adjust_factor', None)
-        self.limit_adjust_level = kwargs.pop('limit_adjust_level', None)
-        self.limit_mode = kwargs.pop('limit_mode', None)
-
-        super().__init__(**kwargs)
-
-    def work(self):
-        pass
-
-    def launch(self, **kwargs):
-        if self.is_active:
-            raise RuntimeError(f'{self} is working already')
-
-        self.is_active = True
-
-        limit_price = kwargs.pop('limit_price', self.limit_price)
-        limit_adjust_factor = kwargs.pop('limit_adjust_factor', self.limit_adjust_factor)
-        limit_adjust_level = kwargs.pop('limit_adjust_level', self.limit_adjust_level)
-        limit_mode = kwargs.pop('limit_mode', self.limit_mode)
-
-        limit = self.algo_engine.calculate_limit(
-            algo=self,
-            limit_price=limit_price,
-            limit_adjust_factor=limit_adjust_factor,
-            limit_adjust_level=limit_adjust_level,
-            mode=limit_mode
-        )
-        order_type = OrderType.LimitOrder
-        volume = self.target_volume - self.filled_volume - self.working_volume
-
-        LOGGER.info(f'{self} launching {order_type} {self.ticker} {self.side.name} {volume}')
-
-        if volume:
-            order = TradeInstruction(
-                ticker=self.ticker,
-                side=self.side,
-                order_type=order_type,
-                volume=volume,
-                limit_price=limit,
-                order_id=f'{self.__class__.__name__}.{self.ticker}.{self.side.side_name}.{uuid.uuid4().hex}'
-            )
-
-            self.working_order[order.order_id] = order
-            self.order[order.order_id] = order
-            self.start_time = self.market_time
-            self._launch(order=order, **kwargs)
-
-    def cancel(self, **kwargs):
-        self.status = self.Status.stopping
-        self.is_active = False
-        self._cancel_all_order(**kwargs)
-
-    def _cancel_all_order(self, **kwargs):
-        for order_id in list(self.working_order):
-            order = self.working_order.get(order_id)
-
-            if order is None:
-                continue
-
-            if order.order_state in [OrderState.Pending, OrderState.Placed, OrderState.PartFilled]:
-                LOGGER.info(f'{self} canceling {order}')
-                self.dma.cancel_order(order=order, **kwargs)
-
-    def _rejected(self, order: TradeInstruction, **kwargs):
-        super()._rejected(order=order)
-
-        if not self.exposure_volume:
-            self._update_status(status=self.Status.closed)
-        else:
-            self._update_status(status=self.Status.done)
-
-    def _filled(self, order: TradeInstruction, report: TradeReport, **kwargs):
-        super()._filled(order=order, report=report, **kwargs)
-
-        if order.order_id not in self.working_order:
-            if self.status == self.Status.working:
-                if self.filled_volume:
-                    self._update_status(status=self.Status.done)
-                else:
-                    self._update_status(status=self.Status.closed)
-
-    def _canceled(self, order: TradeInstruction, **kwargs):
-        super()._canceled(order=order, **kwargs)
-
-        if order.order_id not in self.working_order:
-            if self.status == self.Status.working:
-                if self.filled_volume:
-                    self._update_status(status=self.Status.done)
-                else:
-                    self._update_status(status=self.Status.closed)
-
-        if not self.is_active:
-            self._update_status(status=self.Status.done)
-
-    def to_json(self, fmt='str') -> str | dict:
-        json_dict = super().to_json(fmt='dict')
-
-        additional_dict = dict(
-            limit_price=self.limit_price,
-            limit_adjust_factor=self.limit_adjust_factor,
-            limit_adjust_level=self.limit_adjust_level,
-            limit_mode=self.limit_mode
-        )
-
-        json_dict.update(additional_dict)
-
-        if fmt == 'dict':
-            return json_dict
-        else:
-            return json.dumps(json_dict)
-
-    def from_json(self, json_str: str | dict):
-        if isinstance(json_str, (str, bytes)):
-            json_dict = json.loads(json_str)
-        elif isinstance(json_str, dict):
-            json_dict = json_str
-        else:
-            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
-
-        super().from_json(json_dict)
-
-        self.limit_price = json_dict['limit_price']
-        self.limit_adjust_factor = json_dict['limit_adjust_factor']
-        self.limit_adjust_level = json_dict['limit_adjust_level']
-        self.limit_mode = json_dict['limit_mode']
-
-        return self
-
-
-class PassiveTimeout(Passive):
-    """ Passive handler with timeout function
-    PassiveTimeout is similar to Passive, with a timeout value (in seconds) and cancel working order after that
-
-    Default timeout is 0, which is no timeout (same as passive).
-    """
-
-    def __init__(self, **kwargs):
-        self.timeout = kwargs.pop('timeout', 0)
-
-        super().__init__(**kwargs)
-
-    def on_market_data(self, market_data: MarketData, **kwargs):
-        if self.is_active:
-            self.work()
-
-    def work(self):
-        ts = self.algo_engine.mds.trade_time_between(start_time=self.start_time, end_time=self.market_time).total_seconds()
-        if self.status == self.Status.working and self.timeout and ts > self.timeout:
-            self.cancel()
-            self.logger.debug(f'{self} canceling. status={self.status}, ts={ts:.3f}s')
-        else:
-            self.logger.debug(f'{self} working. status={self.status}, ts={ts:.3f}s, timeout={self.timeout:.3f}s')
-
-    def to_json(self, fmt='str') -> str | dict:
-        json_dict = super().to_json(fmt='dict')
-
-        additional_dict = dict(
-            timeout=self.timeout
-        )
-
-        json_dict.update(additional_dict)
-
-        if fmt == 'dict':
-            return json_dict
-        else:
-            return json.dumps(json_dict)
-
-    def from_json(self, json_str: str | dict):
-        if isinstance(json_str, (str, bytes)):
-            json_dict = json.loads(json_str)
-        elif isinstance(json_str, dict):
-            json_dict = json_str
-        else:
-            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
-
-        super().from_json(json_dict)
-
-        self.timeout = json_dict['timeout']
-
-        return self
-
-
-class Aggressive(Passive):
-    """ Aggressive trading algorithm
-    Aggressive is similar as Passive.
-    Aggressive will re-launch a "fixing" order immediately
-    after working order got canceled or filled, if there is any un-filled volume.
-
-    USE WITH CAUTION
-    """
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    def _filled(self, order: TradeInstruction, report: TradeReport, **kwargs):
-        super()._filled(order=order, report=report, **kwargs)
-
-        if not self.is_active:
-            self._update_status(status=self.Status.done)
-        elif order.order_id not in self.working_order:
-            if self.status == self.Status.working:
-                self.launch()
-
-    def _canceled(self, order: TradeInstruction, **kwargs):
-        super()._canceled(order=order, **kwargs)
-
-        if not self.is_active:
-            self._update_status(status=self.Status.done)
-        elif order.order_id not in self.working_order:
-            if self.status == self.Status.working:
-                self.launch()
-
-
-class AggressiveTimeout(PassiveTimeout, Aggressive):
-    """ Similar to PassiveTimeout, AggressiveTimeout cancel working order after timeout and re-launch "fixing" order after canceled or filled.
-    """
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    def _filled(self, order: TradeInstruction, report: TradeReport, **kwargs):
-        return Aggressive._filled(self=self, order=order, report=report, **kwargs)
-
-    def _canceled(self, order: TradeInstruction, **kwargs):
-        return Aggressive._canceled(self=self, order=order, **kwargs)
-
-
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
-class AlgoEngine(object):
-    def __init__(self, mds=None, registry=None):
-        self.mds = mds if mds is not None else MDS
-        self.registry = registry if registry is not None else ALGO_REGISTRY
-
-    @classmethod
-    def _compare_price(cls, side: TransactionSide, limit_price: float = None, original_limit: float = None, mode='strict') -> float:
-        calculated_limit = original_limit
-
-        if limit_price is None:
-            return calculated_limit
-        elif calculated_limit is None:
-            return limit_price
-        if mode is None or mode == 'strict':
-            if side.sign > 0:
-                calculated_limit = min(calculated_limit, limit_price)
-            else:
-                calculated_limit = max(calculated_limit, limit_price)
-        elif mode == 'loose':
-            if side.sign > 0:
-                calculated_limit = max(calculated_limit, limit_price)
-            else:
-                calculated_limit = min(calculated_limit, limit_price)
-        else:
-            LOGGER.error(f'Invalid compare mode {mode}!')
-            return limit_price
-
-        return calculated_limit
-
-    def get_algo(self, name: str):
-        algo = self.registry.to_algo(name=name.lower(), algo_engine=self)
-        return algo
-
-    def calculate_limit(
-            self,
-            algo: AlgoTemplate,
-            limit_price: float = None,
-            limit_adjust_factor: float = None,
-            limit_adjust_level: float = None,
-            mode: str = 'loose'
-    ) -> float | None:
-        """Calculate limit price
-
-        :param algo: given algo
-        :param limit_price: absolute limit_price
-        :param limit_adjust_factor: limit_price = market_price * (1 + factor) for long order else limit price = market_price * (1 - factor) for short order
-        :param limit_adjust_level:  for long order, limit price = bid[lvl] if lvl > 0 else ask[lvl] for lvl < 0.
-        :param mode: "strict" to select strictest limit price or "loose" to select loosest one. Default is None, which is "strict".
-        :return: the calculated limit price, if there is any
-        """
-        ticker = algo.ticker
-        side = algo.side
-        market_price = self.mds.market_price.get(ticker)
-
-        # validate side
-        if side.sign == 0:
-            LOGGER.error(f'Invalid side {side}')
-            return None
-
-        # market data not available
-        if market_price is None:
-            LOGGER.error(f'{ticker} market data not available')
-            return None
-
-        calculated_limit: float | None = None
-        limit_abs = None
-        limit_adj = None
-        limit_lvl = None
-
-        # compare with absolute limit_price
-        if limit_price is not None:
-            limit_abs = limit_price
-
-        if limit_adjust_factor is not None:
-            limit_adj = market_price * (1 + limit_adjust_factor * side.sign)
-
-        if limit_adjust_level is not None:
-            order_book = self.mds.get_order_book(ticker=ticker)
-
-            if order_book is not None:
-                lvl = abs(limit_adjust_level)
-
-                if limit_adjust_level > 0:
-                    if side.sign > 0:
-                        book = order_book.bid.price
-                    else:
-                        book = order_book.ask.price
-
-                    limit_lvl = book[min(lvl, len(book) - 1)]
-                elif limit_adjust_level < 0:
-                    if side.sign > 0:
-                        book = order_book.ask.price
-                    else:
-                        book = order_book.bid.price
-
-                    limit_lvl = book[min(lvl, len(book) - 1)]
-
-        calculated_limit = self._compare_price(limit_price=limit_abs, original_limit=calculated_limit, side=side, mode=mode)
-        calculated_limit = self._compare_price(limit_price=limit_adj, original_limit=calculated_limit, side=side, mode=mode)
-        calculated_limit = self._compare_price(limit_price=limit_lvl, original_limit=calculated_limit, side=side, mode=mode)
-        calculated_limit = self._compare_price(limit_price=market_price, original_limit=calculated_limit, side=side, mode=mode)
-
-        LOGGER.info(f'BBA limits {ticker} market_price={market_price}, lmt_abs={limit_price}, lmt_adj={limit_adj}, lmt_lvl={limit_lvl}, mode={mode}, cal_lmt={calculated_limit}')
-        return calculated_limit
-
-    def from_json(self, json_str, dma) -> AlgoTemplate:
-        if isinstance(json_str, (str, bytes)):
-            json_dict = json.loads(json_str)
-        elif isinstance(json_str, dict):
-            json_dict = json_str
-        else:
-            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
-
-        algo: AlgoTemplate = self.get_algo(json_dict['algo_type'])(
-            ticker=json_dict['ticker'],
-            side=TransactionSide(json_dict['side']),
-            target_volume=json_dict['target_volume'],
-            dma=dma,
-            algo_id=json_dict['algo_id']
-        )
-        algo.from_json(json_dict)
-
-        return algo
-
-
-ALGO_REGISTRY = AlgoRegistry()
-
-ALGO_REGISTRY.add_algo('aggressive', 'aggr', handler=Aggressive)
-ALGO_REGISTRY.add_algo('passive', 'pass', handler=Passive)
-ALGO_REGISTRY.add_algo('aggressive_timeout', 'aggr_timeout', handler=AggressiveTimeout)
-ALGO_REGISTRY.add_algo('passive_timeout', 'pass_timeout', handler=PassiveTimeout)
-
-ALGO_ENGINE = AlgoEngine(mds=MDS, registry=ALGO_REGISTRY)
+from __future__ import annotations
+
+import abc
+import datetime
+import enum
+import functools
+import json
+import threading
+import uuid
+from typing import Type
+
+import numpy as np
+from PyQuantKit import TransactionSide, TradeInstruction, MarketData, TradeReport, OrderState, OrderType
+
+from . import LOGGER
+from .MarketEngine import MDS
+
+LOGGER = LOGGER.getChild('AlgoEngine')
+__all__ = ['AlgoTemplate', 'AlgoRegistry', 'AlgoEngine', 'ALGO_ENGINE', 'ALGO_REGISTRY']
+
+
+class AlgoStatus(enum.Enum):
+    idle = 'idle'  # init state 
+    preparing = 'preparing'  # preparing
+    ready = 'ready'  # ready to launch order
+    working = 'working'  # order launched
+    done = 'done'  # transaction complete!
+    closed = 'closed'  # transaction failed and close
+    stopping = 'stopping'  # trying to stop transaction
+    rejected = 'rejected'  # internal / external rejected
+    error = 'error'  # internal / external error
+
+
+class AlgoTemplate(object, metaclass=abc.ABCMeta):
+    Status = AlgoStatus
+
+    def __init__(self, dma, ticker: str, target_volume: float, side: TransactionSide, **kwargs):
+        """ Template for trading algorithm
+        an abstract class to create a trading algorithm
+
+        :param dma: direct market access
+        :param ticker: the given symbol of the underlying to trade
+        :param target_volume: the given volume to trade
+        :param side: the given TransactionSide
+        :keyword algo_engine: the algo_engine instance, default is ALGO_ENGINE
+        :keyword logger: the logger instance, default is LOGGER
+        :keyword algo_id: the id of the algo, default is uuid4()
+        """
+        self.dma = dma
+        self.ticker = ticker
+        self.side = side
+        self.target_volume = target_volume
+        self.algo_engine = kwargs.pop('algo_engine', ALGO_ENGINE)
+        self.algo_type = kwargs.get('algo_type', self.algo_engine.registry.reversed_registry[self.__class__.__name__])
+        self.logger = kwargs.pop('logger', LOGGER)
+        self.algo_id = kwargs.pop('algo_id', uuid.uuid4().hex)
+
+        self.status: AlgoStatus = self.Status.idle
+        self._target_progress = 0
+        self._lock = threading.Lock()
+        self._thread = threading.Thread(target=self.work)
+
+        self.working_order: dict[str, TradeInstruction] = {}
+        self.order: dict[str, TradeInstruction] = {}
+
+        self.is_active = False
+        self.start_time = None
+        self.finish_time = None
+
+    def __repr__(self):
+        return f'<TradeAlgo>(ticker={self.ticker}, target={self.side.sign * self.target_volume}, done={self.side.sign * self.exposure_volume}, algo={self.__class__.__name__}, status={self.status.value}, id={id(self)})'
+
+    def on_sync_progress(self, progress: float, **kwargs):
+        self._target_progress = max(min(progress, 1), 0)
+        self._sync(progress=progress, **kwargs)
+
+    def on_market_data(self, market_data: MarketData, **kwargs):
+        pass
+
+    def on_filled(self, report: TradeReport, **kwargs):
+        if report.order_id in self.working_order:
+            self._filled(order=self.working_order[report.order_id], report=report, **kwargs)
+            return 1
+        else:
+            self.logger.warning(f'[Failed to fill] {self} has no matching for working order {report.order_id}')
+            return 0
+
+    def on_canceled(self, order_id: str = None, **kwargs):
+        if order_id in self.working_order:
+            self._canceled(order=self.working_order[order_id], **kwargs)
+            return 1
+        else:
+            self.logger.warning(f'[Failed to cancel] {self} has no matching for working order {order_id}')
+            return 0
+
+    def on_rejected(self, order: TradeInstruction, **kwargs):
+        if order.order_id in self.working_order:
+            self._rejected(order=order, **kwargs)
+            return 1
+        else:
+            self.logger.warning(f'[Failed to reject] {self} has no matching for working order {order.order_id}')
+            return 0
+
+    def recover(self):
+        self._update_working_order()
+
+        if not self.working_volume:
+            if self.exposure_volume:
+                self._update_status(status=self.Status.done)
+            else:
+                self._update_status(status=self.Status.closed)
+            LOGGER.info(f'{self} recovery successful! status {self.status}')
+        else:
+            LOGGER.warning(f'Caution! Recovering WORKING trade handler {self} may cause unexpected error!')
+            self._update_status(status=self.Status.working)
+
+    def _update_working_order(self):
+        """
+        refresh working order, to remove the finished orders
+        :return: a dict of working orders
+        """
+        for order_id in list(self.working_order):
+            order = self.working_order.get(order_id)
+
+            if order is None:
+                continue
+
+            if order.is_done:
+                self.working_order.pop(order_id, None)
+
+        return self.working_order
+
+    def _update_status(self, status=None, sync_pos=True, **kwargs):
+        """
+        ._update_status provides a method to clear working orders and auto assign status
+        ._update_status DOES NOT call .on_filled, .on_rejected nor .on_canceled, these method is triggered by position management service
+        ._update_status should be called in .on_filled .on_rejected and .on_canceled
+
+        as the result of concurrency, assigning status while sync_pos may cause unexpected result, use with caution
+
+        :param status: the given status
+        :param sync_pos: whether to auto-clear working orders
+        :param kwargs: market_time to assign the exact time when status is changed, used in backtesting
+        """
+        if sync_pos:
+            self._update_working_order()
+
+        if 'market_time' in kwargs:
+            self.start_time = kwargs['market_time']
+
+        # update status with given status and datetime
+        if status is not None:
+            if isinstance(status, self.Status):
+                self.status = status
+            else:
+                raise TypeError(f'Invalid status {status}')
+        # update status with self info
+        else:
+            # with working order
+            if self.working_order:
+                if self.status == self.Status.idle:
+                    self.status = self.Status.working
+            # without any working order
+            else:
+                if self.filled_volume == self.target_volume:
+                    self.status = self.Status.done
+
+        return self.status
+
+    def _launch(self, order, **kwargs):
+        self.dma.launch_order(order=order, **kwargs)
+        # order launched, order state can be pending, placed, or rejected (by internal on_order risk control)
+        # DO NOT assume order state is_working, it may be rejected!
+        # DO NOT assume order is in .working_order, it may be rejected!
+        # DO NOT assume algo state is working, it may be rejected!
+        # therefor calling _update_status is recommended but still optional.
+        # self._update_status(sync_pos=False)
+
+    def _cancel_order(self, order, **kwargs):
+        self.dma.cancel_order(order=order, **kwargs)
+        # self._update_status(sync_pos=False)
+
+    def _filled(self, order: TradeInstruction, report: TradeReport, **kwargs):
+        """
+        callback on order filled / part-filled
+
+        this callback will REMOVE filled order from working order dict and update algo status
+        :param order: the given filled order
+        :param kwargs: keyword args for updating status. e.g. timestamp
+        """
+        if report.trade_id not in order.trades:
+            order.fill(trade_report=report)
+
+        kwargs['sync_pos'] = True
+        self._update_status(**kwargs)
+
+    def _canceled(self, order: TradeInstruction, **kwargs):
+        """
+        callback on order canceled
+
+        this callback will REMOVE cancelled order from working order dict and update algo status
+        :param order: the given canceled order
+        :param kwargs: keyword args for updating status. e.g. timestamp
+        """
+        self._update_working_order()
+        kwargs['sync_pos'] = False
+
+        if self.working_order:
+            self._update_status(status=self.Status.working, **kwargs)
+        elif self.exposure_volume:
+            self._update_status(status=self.Status.done, **kwargs)
+        else:
+            self._update_status(status=self.Status.closed, **kwargs)
+
+    def _rejected(self, order: TradeInstruction, **kwargs):
+        self._update_status(status=self.Status.rejected, **kwargs)
+
+    def _sync(self, progress, **kwargs):
+        ...
+
+    def to_json(self, fmt='str') -> str | dict:
+        json_dict = {
+            'algo_type': self.algo_type,
+            'ticker': self.ticker,
+            'side': self.side.name,
+            'target_volume': self.target_volume,
+            'algo_id': self.algo_id,
+            'status': self.status.name,
+            'target_progress': self._target_progress,
+            'start_time': datetime.datetime.timestamp(self.start_time) if self.start_time else None,
+            'finish_time': datetime.datetime.timestamp(self.finish_time) if self.finish_time else None,
+            'order': {_: self.order[_].to_json(fmt='dict') for _ in self.order},
+        }
+
+        if fmt == 'dict':
+            return json_dict
+        else:
+            return json.dumps(json_dict)
+
+    def from_json(self, json_str: str | dict):
+        if isinstance(json_str, (str, bytes)):
+            json_dict = json.loads(json_str)
+        elif isinstance(json_str, dict):
+            json_dict = json_str
+        else:
+            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
+
+        self.ticker = json_dict['ticker']
+        self.side = TransactionSide(json_dict['side'])
+        self.target_volume = json_dict['target_volume']
+        self.algo_id = json_dict['algo_id']
+        self.status = self.Status[json_dict['status']]
+        self._target_progress = json_dict['target_progress']
+        self.start_time = None if json_dict['start_time'] is None else datetime.datetime.fromtimestamp(json_dict['start_time'])
+        self.finish_time = None if json_dict['finish_time'] is None else datetime.datetime.fromtimestamp(json_dict['finish_time'])
+        self.order = {_: TradeInstruction.from_json(json_dict['order'][_]) for _ in json_dict['order']}
+        self.working_order = {order_id: order for order_id, order in self.order.items() if not order.is_done}
+
+        return self
+
+    @abc.abstractmethod
+    def work(self):
+        ...
+
+    @abc.abstractmethod
+    def launch(self, **kwargs) -> list[TradeInstruction]:
+        """
+        launch is a method to initiate the algo and launching orders.
+        this method will set the algo is_active = true
+        this method will set a new algo state, usually idle -> working
+        launch method is designed to be called by strategy / position management service.
+
+        :param kwargs: other keywords needed to launch an algo
+        :return: a list of working orders. Noted, that not all working order is returned by this method, for example, TWAP algo will init a sequence of order and return later.
+        """
+        ...
+
+    @abc.abstractmethod
+    def cancel(self, **kwargs):
+        """
+        cancel is a method to cancel / stop ALL working orders
+        this method will set the algo is_active = false
+        this method may set a new algo state, usually working -> stopping
+        launch method is designed to be called by strategy / position management service.
+
+        :param kwargs: other keywords needed to cancel an algo
+        :return: None
+        """
+        ...
+
+    @property
+    def trades(self) -> dict[str, TradeReport]:
+        trades = {}
+
+        for order in list(self.order.values()):
+            for trade_id in list(order.trades):
+                trade_report = order.trades.get(trade_id)
+
+                if trade_report is None:
+                    continue
+
+                trades[trade_report.trade_id] = trade_report
+
+        return trades
+
+    @property
+    def average_price(self) -> float:
+        adjust_volume = 0.
+        notional = 0.
+
+        for report in list(self.trades.values()):
+            if report.price == 0:
+                adjust_volume += report.volume
+            else:
+                adjust_volume += report.notional / report.price
+            notional += report.notional
+
+        if adjust_volume == 0:
+            return np.nan
+        else:
+            return notional / adjust_volume
+
+    @property
+    def exposure_volume(self) -> float:
+        """
+        <WITH SIGN> net exposed VOLUME indicating the exposure of the pos
+        :return: float
+        """
+        exposure = 0.
+
+        for report in list(self.trades.values()):
+            exposure += report.volume * report.side.sign
+
+        return exposure
+
+    @property
+    def working_volume(self) -> float:
+        """
+        <WITHOUT SIGN> net working VOLUME indicating the working status of the pos
+        :return: float
+        """
+        working = 0.
+
+        for order_id in self.working_order:
+            working_order = self.working_order.get(order_id)
+
+            if working_order is None:
+                continue
+
+            working += working_order.working_volume  # should be all positive
+
+        return working
+
+    @property
+    def filled_volume(self) -> float:
+        """
+        <WITHOUT SIGN> filled VOLUME
+        :return: float
+        """
+        volume = 0.
+
+        for report in list(self.trades.values()):
+            volume += report.volume
+
+        return volume
+
+    @property
+    def filled_notional(self) -> float:
+        """
+        <POSSIBLY WITH SIGN> total filled Notional
+        :return: float
+        """
+        notional = 0.
+
+        for report in list(self.trades.values()):
+            notional += report.notional  # which should be a POSITIVE number in normal cases.
+
+        return notional
+
+    @property
+    def fee(self) -> float:
+        """
+        <POSSIBLY WITH SIGN> total transaction fee
+        :return: float
+        """
+        total_fee = 0.
+
+        for report in list(self.trades.values()):
+            total_fee += report.fee
+
+        return total_fee
+
+    @property
+    def cash_flow(self) -> float:
+        """
+        <WITH SIGN> total cash flow
+        :return: float
+        """
+        cash_flow = -self.filled_notional * self.side.sign
+        return cash_flow
+
+    @property
+    def multiplier(self) -> float:
+        if self.order:
+            return self.order[list(self.order)[0]].multiplier
+        else:
+            return 1.0
+
+    @property
+    def filled_progress(self):
+        return self.filled_volume / self.target_volume
+
+    @property
+    def placed_progress(self):
+        return abs(self.working_volume / self.target_volume) + self.filled_progress
+
+    @property
+    def target_progress(self):
+        return self._target_progress
+
+    @property
+    def market_price(self):
+        return self.algo_engine.mds.market_price.get(self.ticker)
+
+    @property
+    def market_time(self):
+        return self.algo_engine.mds.market_time
+
+
+class Passive(AlgoTemplate):
+    """ Passive trading algorithm
+    Passive is a basic trading algo which trades all target volume into one single LIMIT order.
+    Algo will stop after order get filled or canceled.
+    no additional order will be launched except the initial one
+
+    a limit price can be set by keyword arguments, see also in doc: AlgoEngine.calculate_limit
+
+    """
+
+    def __init__(self, **kwargs):
+        """
+        init a Passive trade algo
+
+        requires all params from AlgoTemplate and additional following 4
+        :keyword limit_price: the absolute limit price of the order
+        :keyword limit_adjust_factor: limit price = market_price * (1 + factor) for long order else limit price = market_price * (1 - factor) for short order
+        :keyword limit_adjust_level:  for long order, limit price = bid[lvl] if lvl > 0 else ask[lvl] for lvl < 0.
+        :keyword limit_mode: if multiple limit price standard is provided, use "strict" to select strictest limit price or "loose" to select loosest one. Default is None, which is "strict".
+        """
+        self.limit_price = kwargs.pop('limit_price', None)
+        self.limit_adjust_factor = kwargs.pop('limit_adjust_factor', None)
+        self.limit_adjust_level = kwargs.pop('limit_adjust_level', None)
+        self.limit_mode = kwargs.pop('limit_mode', None)
+
+        super().__init__(**kwargs)
+
+    def work(self):
+        pass
+
+    def launch(self, **kwargs):
+        if self.is_active:
+            raise RuntimeError(f'{self} is working already')
+
+        self.is_active = True
+
+        limit_price = kwargs.pop('limit_price', self.limit_price)
+        limit_adjust_factor = kwargs.pop('limit_adjust_factor', self.limit_adjust_factor)
+        limit_adjust_level = kwargs.pop('limit_adjust_level', self.limit_adjust_level)
+        limit_mode = kwargs.pop('limit_mode', self.limit_mode)
+
+        limit = self.algo_engine.calculate_limit(
+            algo=self,
+            limit_price=limit_price,
+            limit_adjust_factor=limit_adjust_factor,
+            limit_adjust_level=limit_adjust_level,
+            mode=limit_mode
+        )
+        order_type = OrderType.LimitOrder
+        volume = self.target_volume - self.filled_volume - self.working_volume
+
+        LOGGER.info(f'{self} launching {order_type} {self.ticker} {self.side.name} {volume}')
+
+        if volume:
+            order = TradeInstruction(
+                ticker=self.ticker,
+                side=self.side,
+                order_type=order_type,
+                volume=volume,
+                limit_price=limit,
+                order_id=f'{self.__class__.__name__}.{self.ticker}.{self.side.side_name}.{uuid.uuid4().hex}'
+            )
+
+            self.working_order[order.order_id] = order
+            self.order[order.order_id] = order
+            self.start_time = self.market_time
+            self._launch(order=order, **kwargs)
+
+    def cancel(self, **kwargs):
+        self.status = self.Status.stopping
+        self.is_active = False
+        self._cancel_all_order(**kwargs)
+
+    def _cancel_all_order(self, **kwargs):
+        for order_id in list(self.working_order):
+            order = self.working_order.get(order_id)
+
+            if order is None:
+                continue
+
+            if order.order_state in [OrderState.Pending, OrderState.Placed, OrderState.PartFilled]:
+                LOGGER.info(f'{self} canceling {order}')
+                self.dma.cancel_order(order=order, **kwargs)
+
+    def _rejected(self, order: TradeInstruction, **kwargs):
+        super()._rejected(order=order)
+
+        if not self.exposure_volume:
+            self._update_status(status=self.Status.closed)
+        else:
+            self._update_status(status=self.Status.done)
+
+    def _filled(self, order: TradeInstruction, report: TradeReport, **kwargs):
+        super()._filled(order=order, report=report, **kwargs)
+
+        if order.order_id not in self.working_order:
+            if self.status == self.Status.working:
+                if self.filled_volume:
+                    self._update_status(status=self.Status.done)
+                else:
+                    self._update_status(status=self.Status.closed)
+
+    def _canceled(self, order: TradeInstruction, **kwargs):
+        super()._canceled(order=order, **kwargs)
+
+        if order.order_id not in self.working_order:
+            if self.status == self.Status.working:
+                if self.filled_volume:
+                    self._update_status(status=self.Status.done)
+                else:
+                    self._update_status(status=self.Status.closed)
+
+        if not self.is_active:
+            self._update_status(status=self.Status.done)
+
+    def to_json(self, fmt='str') -> str | dict:
+        json_dict = super().to_json(fmt='dict')
+
+        additional_dict = dict(
+            limit_price=self.limit_price,
+            limit_adjust_factor=self.limit_adjust_factor,
+            limit_adjust_level=self.limit_adjust_level,
+            limit_mode=self.limit_mode
+        )
+
+        json_dict.update(additional_dict)
+
+        if fmt == 'dict':
+            return json_dict
+        else:
+            return json.dumps(json_dict)
+
+    def from_json(self, json_str: str | dict):
+        if isinstance(json_str, (str, bytes)):
+            json_dict = json.loads(json_str)
+        elif isinstance(json_str, dict):
+            json_dict = json_str
+        else:
+            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
+
+        super().from_json(json_dict)
+
+        self.limit_price = json_dict['limit_price']
+        self.limit_adjust_factor = json_dict['limit_adjust_factor']
+        self.limit_adjust_level = json_dict['limit_adjust_level']
+        self.limit_mode = json_dict['limit_mode']
+
+        return self
+
+
+class PassiveTimeout(Passive):
+    """ Passive handler with timeout function
+    PassiveTimeout is similar to Passive, with a timeout value (in seconds) and cancel working order after that
+
+    Default timeout is 0, which is no timeout (same as passive).
+    """
+
+    def __init__(self, **kwargs):
+        self.timeout = kwargs.pop('timeout', 0)
+
+        super().__init__(**kwargs)
+
+    def on_market_data(self, market_data: MarketData, **kwargs):
+        if self.is_active:
+            self.work()
+
+    def work(self):
+        ts = self.algo_engine.mds.trade_time_between(start_time=self.start_time, end_time=self.market_time).total_seconds()
+        if self.status == self.Status.working and self.timeout and ts > self.timeout:
+            self.cancel()
+            self.logger.debug(f'{self} canceling. status={self.status}, ts={ts:.3f}s')
+        else:
+            self.logger.debug(f'{self} working. status={self.status}, ts={ts:.3f}s, timeout={self.timeout:.3f}s')
+
+    def to_json(self, fmt='str') -> str | dict:
+        json_dict = super().to_json(fmt='dict')
+
+        additional_dict = dict(
+            timeout=self.timeout
+        )
+
+        json_dict.update(additional_dict)
+
+        if fmt == 'dict':
+            return json_dict
+        else:
+            return json.dumps(json_dict)
+
+    def from_json(self, json_str: str | dict):
+        if isinstance(json_str, (str, bytes)):
+            json_dict = json.loads(json_str)
+        elif isinstance(json_str, dict):
+            json_dict = json_str
+        else:
+            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
+
+        super().from_json(json_dict)
+
+        self.timeout = json_dict['timeout']
+
+        return self
+
+
+class Aggressive(Passive):
+    """ Aggressive trading algorithm
+    Aggressive is similar as Passive.
+    Aggressive will re-launch a "fixing" order immediately
+    after working order got canceled or filled, if there is any un-filled volume.
+
+    USE WITH CAUTION
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+    def _filled(self, order: TradeInstruction, report: TradeReport, **kwargs):
+        super()._filled(order=order, report=report, **kwargs)
+
+        if not self.is_active:
+            self._update_status(status=self.Status.done)
+        elif order.order_id not in self.working_order:
+            if self.status == self.Status.working:
+                self.launch()
+
+    def _canceled(self, order: TradeInstruction, **kwargs):
+        super()._canceled(order=order, **kwargs)
+
+        if not self.is_active:
+            self._update_status(status=self.Status.done)
+        elif order.order_id not in self.working_order:
+            if self.status == self.Status.working:
+                self.launch()
+
+
+class AggressiveTimeout(PassiveTimeout, Aggressive):
+    """ Similar to PassiveTimeout, AggressiveTimeout cancel working order after timeout and re-launch "fixing" order after canceled or filled.
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+    def _filled(self, order: TradeInstruction, report: TradeReport, **kwargs):
+        return Aggressive._filled(self=self, order=order, report=report, **kwargs)
+
+    def _canceled(self, order: TradeInstruction, **kwargs):
+        return Aggressive._canceled(self=self, order=order, **kwargs)
+
+
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
+class AlgoEngine(object):
+    def __init__(self, mds=None, registry=None):
+        self.mds = mds if mds is not None else MDS
+        self.registry = registry if registry is not None else ALGO_REGISTRY
+
+    @classmethod
+    def _compare_price(cls, side: TransactionSide, limit_price: float = None, original_limit: float = None, mode='strict') -> float:
+        calculated_limit = original_limit
+
+        if limit_price is None:
+            return calculated_limit
+        elif calculated_limit is None:
+            return limit_price
+        if mode is None or mode == 'strict':
+            if side.sign > 0:
+                calculated_limit = min(calculated_limit, limit_price)
+            else:
+                calculated_limit = max(calculated_limit, limit_price)
+        elif mode == 'loose':
+            if side.sign > 0:
+                calculated_limit = max(calculated_limit, limit_price)
+            else:
+                calculated_limit = min(calculated_limit, limit_price)
+        else:
+            LOGGER.error(f'Invalid compare mode {mode}!')
+            return limit_price
+
+        return calculated_limit
+
+    def get_algo(self, name: str):
+        algo = self.registry.to_algo(name=name.lower(), algo_engine=self)
+        return algo
+
+    def calculate_limit(
+            self,
+            algo: AlgoTemplate,
+            limit_price: float = None,
+            limit_adjust_factor: float = None,
+            limit_adjust_level: float = None,
+            mode: str = 'loose'
+    ) -> float | None:
+        """Calculate limit price
+
+        :param algo: given algo
+        :param limit_price: absolute limit_price
+        :param limit_adjust_factor: limit_price = market_price * (1 + factor) for long order else limit price = market_price * (1 - factor) for short order
+        :param limit_adjust_level:  for long order, limit price = bid[lvl] if lvl > 0 else ask[lvl] for lvl < 0.
+        :param mode: "strict" to select strictest limit price or "loose" to select loosest one. Default is None, which is "strict".
+        :return: the calculated limit price, if there is any
+        """
+        ticker = algo.ticker
+        side = algo.side
+        market_price = self.mds.market_price.get(ticker)
+
+        # validate side
+        if side.sign == 0:
+            LOGGER.error(f'Invalid side {side}')
+            return None
+
+        # market data not available
+        if market_price is None:
+            LOGGER.error(f'{ticker} market data not available')
+            return None
+
+        calculated_limit: float | None = None
+        limit_abs = None
+        limit_adj = None
+        limit_lvl = None
+
+        # compare with absolute limit_price
+        if limit_price is not None:
+            limit_abs = limit_price
+
+        if limit_adjust_factor is not None:
+            limit_adj = market_price * (1 + limit_adjust_factor * side.sign)
+
+        if limit_adjust_level is not None:
+            order_book = self.mds.get_order_book(ticker=ticker)
+
+            if order_book is not None:
+                lvl = abs(limit_adjust_level)
+
+                if limit_adjust_level > 0:
+                    if side.sign > 0:
+                        book = order_book.bid.price
+                    else:
+                        book = order_book.ask.price
+
+                    limit_lvl = book[min(lvl, len(book) - 1)]
+                elif limit_adjust_level < 0:
+                    if side.sign > 0:
+                        book = order_book.ask.price
+                    else:
+                        book = order_book.bid.price
+
+                    limit_lvl = book[min(lvl, len(book) - 1)]
+
+        calculated_limit = self._compare_price(limit_price=limit_abs, original_limit=calculated_limit, side=side, mode=mode)
+        calculated_limit = self._compare_price(limit_price=limit_adj, original_limit=calculated_limit, side=side, mode=mode)
+        calculated_limit = self._compare_price(limit_price=limit_lvl, original_limit=calculated_limit, side=side, mode=mode)
+        calculated_limit = self._compare_price(limit_price=market_price, original_limit=calculated_limit, side=side, mode=mode)
+
+        LOGGER.info(f'BBA limits {ticker} market_price={market_price}, lmt_abs={limit_price}, lmt_adj={limit_adj}, lmt_lvl={limit_lvl}, mode={mode}, cal_lmt={calculated_limit}')
+        return calculated_limit
+
+    def from_json(self, json_str, dma) -> AlgoTemplate:
+        if isinstance(json_str, (str, bytes)):
+            json_dict = json.loads(json_str)
+        elif isinstance(json_str, dict):
+            json_dict = json_str
+        else:
+            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
+
+        algo: AlgoTemplate = self.get_algo(json_dict['algo_type'])(
+            ticker=json_dict['ticker'],
+            side=TransactionSide(json_dict['side']),
+            target_volume=json_dict['target_volume'],
+            dma=dma,
+            algo_id=json_dict['algo_id']
+        )
+        algo.from_json(json_dict)
+
+        return algo
+
+
+ALGO_REGISTRY = AlgoRegistry()
+
+ALGO_REGISTRY.add_algo('aggressive', 'aggr', handler=Aggressive)
+ALGO_REGISTRY.add_algo('passive', 'pass', handler=Passive)
+ALGO_REGISTRY.add_algo('aggressive_timeout', 'aggr_timeout', handler=AggressiveTimeout)
+ALGO_REGISTRY.add_algo('passive_timeout', 'pass_timeout', handler=PassiveTimeout)
+
+ALGO_ENGINE = AlgoEngine(mds=MDS, registry=ALGO_REGISTRY)
```

### Comparing `PyAlgoEngine-0.3.5/AlgoEngine/Engine/EventEngine.py` & `PyAlgoEngine-0.3.6/AlgoEngine/Engine/EventEngine.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from types import SimpleNamespace
-
-import EventEngine
-
-from . import LOGGER
-
-__all__ = ['EVENT_ENGINE', 'TOPIC']
-LOGGER = LOGGER.getChild('EventEngine')
-EventEngine.set_logger(LOGGER)
-
-
-class TopicSet(object):
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
-
-    @classmethod
-    def push(cls, market_data):
-        return cls.realtime(ticker=market_data.ticker, dtype=market_data.__class__.__name__)
-
-    @classmethod
-    def parse(cls, topic: EventEngine.Topic) -> SimpleNamespace:
-        try:
-            _ = topic.value.split('.')
-
-            action = _.pop(0)
-            if action in ['open', 'close']:
-                dtype = None
-            else:
-                dtype = _.pop(-1)
-            ticker = '.'.join(_)
-
-            p = SimpleNamespace(
-                action=action,
-                dtype=dtype,
-                ticker=ticker
-            )
-            return p
-        except Exception as _:
-            raise ValueError(f'Invalid topic {topic}')
-
-
-EVENT_ENGINE = EventEngine.EventEngine()
-TOPIC = TopicSet
-# EVENT_ENGINE.start()
+from types import SimpleNamespace
+
+import EventEngine
+
+from . import LOGGER
+
+__all__ = ['EVENT_ENGINE', 'TOPIC']
+LOGGER = LOGGER.getChild('EventEngine')
+EventEngine.set_logger(LOGGER)
+
+
+class TopicSet(object):
+    on_order = EventEngine.Topic('on_order')
+    on_report = EventEngine.Topic('on_report')
+    eod = EventEngine.Topic('eod')
+    eod_done = EventEngine.Topic('eod_done')
+    bod = EventEngine.Topic('bod')
+    bod_done = EventEngine.Topic('bod_done')
+
+    launch_order = EventEngine.PatternTopic('launch_order.{ticker}')
+    cancel_order = EventEngine.PatternTopic('cancel_order.{ticker}')
+    realtime = EventEngine.PatternTopic('realtime.{ticker}.{dtype}')
+
+    @classmethod
+    def push(cls, market_data):
+        return cls.realtime(ticker=market_data.ticker, dtype=market_data.__class__.__name__)
+
+    @classmethod
+    def parse(cls, topic: EventEngine.Topic) -> SimpleNamespace:
+        try:
+            _ = topic.value.split('.')
+
+            action = _.pop(0)
+            if action in ['open', 'close']:
+                dtype = None
+            else:
+                dtype = _.pop(-1)
+            ticker = '.'.join(_)
+
+            p = SimpleNamespace(
+                action=action,
+                dtype=dtype,
+                ticker=ticker
+            )
+            return p
+        except Exception as _:
+            raise ValueError(f'Invalid topic {topic}')
+
+
+EVENT_ENGINE = EventEngine.EventEngine()
+TOPIC = TopicSet
+# EVENT_ENGINE.start()
```

### Comparing `PyAlgoEngine-0.3.5/AlgoEngine/Engine/MarketEngine.py` & `PyAlgoEngine-0.3.6/AlgoEngine/Engine/MarketEngine.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,888 +1,888 @@
-from __future__ import annotations
-
-import abc
-import datetime
-import functools
-import threading
-import uuid
-from collections import defaultdict
-
-from PyQuantKit import TickData, TradeData, OrderBook, MarketData, Progress, TransactionSide, BarData, TransactionData
-
-from . import LOGGER
-
-__all__ = ['MDS', 'MarketDataService', 'MarketDataMonitor', 'SyntheticOrderBookMonitor', 'MinuteBarMonitor', 'Profile', 'ProgressiveReplay', 'SimpleReplay', 'Replay']
-LOGGER = LOGGER.getChild('MarketEngine')
-
-
-class MarketDataMonitor(object, metaclass=abc.ABCMeta):
-    """
-    this is a template for market data monitor
-
-    A data monitor is a module that process market data and generate custom index
-
-    When MDS receive an update of market data, the __call__ function of this monitor is triggered.
-
-    Note: all the market_data, of all subscribed ticker will be fed into monitor. It should be assumed that a storage for multiple ticker is required.
-    To access the monitor, use `monitor = MDS[monitor_id]`
-    To access the index generated by the monitor, use `monitor.value`
-    To indicate that the monitor is ready to use set `monitor.is_ready = True`
-
-    The implemented monitor should be initialized and use `MDS.add_monitor(monitor)` to attach onto the engine
-    """
-
-    def __init__(self, name: str, monitor_id: str = None, mds: MarketDataService = None):
-        self.name = name
-        self.monitor_id = uuid.uuid4().hex if monitor_id is None else monitor_id
-        self.mds = MDS if mds is None else mds
-
-    @abc.abstractmethod
-    def __call__(self, market_data: MarketData, **kwargs): ...
-
-    @property
-    @abc.abstractmethod
-    def value(self): ...
-
-    @property
-    @abc.abstractmethod
-    def is_ready(self) -> bool: ...
-
-
-class SyntheticOrderBookMonitor(MarketDataMonitor):
-    def __init__(self, keep_order_log: bool = False, **kwargs):
-        self.keep_order_log = keep_order_log
-
-        super().__init__(
-            name=kwargs.pop('name', 'Monitor.SyntheticOrderBook'),
-            monitor_id=kwargs.pop('monitor_id', None),
-            mds=kwargs.pop('mds', None),
-        )
-
-        self._is_ready = True
-        self._value = {}
-        self.order_book = {}
-        self.order_log = {}
-
-    def __call__(self, market_data: MarketData, **kwargs):
-        if isinstance(market_data, TradeData):
-            self.on_trade_data(trade_data=market_data)
-
-    def on_trade_data(self, trade_data: TradeData):
-        ticker = trade_data.ticker
-
-        if order_book := self.order_book.get(ticker):
-            if order_book.market_time <= trade_data.market_time:
-                side: TransactionSide = trade_data.side
-                price = trade_data.price
-                book = order_book.ask if side.sign > 0 else order_book.bid
-                listed_volume = book.at_price(price).volume if price in book else 0.
-                traded_volume = trade_data.volume
-                book.update_entry(price=price, volume=max(0, listed_volume - traded_volume))
-
-        if self.keep_order_log:
-            self._update_order_log(trade_data=trade_data)
-
-    def on_transaction_data(self, transaction_data: TransactionData):
-        pass
-
-    def _update_order_log(self, trade_data: TradeData):
-        side: TransactionSide = trade_data.side
-        price = trade_data.price
-        traded_volume = trade_data.volume
-
-        for order_id in list(self.order_log):
-            order_log = self.order_log.get(order_id)
-
-            if order_log is None:
-                continue
-
-            if side.sign > 0:
-                if order_log.side.sign < 0:
-                    if price == order_log.price:
-                        order_log.volume -= traded_volume
-                    elif price > order_log.price:
-                        order_log.volume = 0.
-                else:
-                    if price <= order_log.price:
-                        order_log.volume = 0.
-            elif side.sign < 0:
-                if order_log.side.sign > 0:
-                    if price == order_log.price:
-                        order_log.volume -= traded_volume
-                    elif price < order_log.price:
-                        order_log.volume = 0.
-                else:
-                    if price >= order_log.price:
-                        order_log.volume = 0.
-
-            if order_log.volume <= 0:
-                self.order_log.pop(order_id)
-
-    @property
-    def is_ready(self) -> bool:
-        return self._is_ready
-
-    @property
-    def value(self) -> dict[str, OrderBook]:
-        return self.order_book
-
-
-class MinuteBarMonitor(MarketDataMonitor):
-    def __init__(self, interval: float = 60., **kwargs):
-        self.interval = interval
-
-        super().__init__(
-            name=kwargs.pop('name', 'Monitor.MinuteBarMonitor'),
-            monitor_id=kwargs.pop('monitor_id', None),
-            mds=kwargs.pop('mds', None),
-        )
-
-        self._minute_bar_data: dict[str, BarData] = {}
-        self._last_bar_data: dict[str, BarData] = {}
-
-        self._is_ready = True
-        self._value = {}
-
-    def __call__(self, market_data: MarketData, **kwargs):
-        self._update_last_bar(market_data=market_data, interval=self.interval)
-        # self._update_active_bar(market_data=market_data, interval=self.interval)
-
-    def _update_last_bar(self, market_data: MarketData, interval: float):
-        ticker = market_data.ticker
-        market_price = market_data.market_price
-        market_time = market_data.market_time
-
-        if ticker not in self._minute_bar_data or market_time >= self._minute_bar_data[ticker].bar_end_time:
-            # update bar_data
-            if ticker in self._minute_bar_data:
-                self._last_bar_data[ticker] = self._minute_bar_data[ticker]
-
-            bar_data = self._minute_bar_data[ticker] = BarData(
-                ticker=ticker,
-                bar_start_time=datetime.datetime.fromtimestamp(self.mds.timestamp // interval * interval),
-                bar_span=datetime.timedelta(seconds=interval),
-                high_price=market_price,
-                low_price=market_price,
-                open_price=market_price,
-                close_price=market_price,
-                volume=0.,
-                notional=0.,
-                trade_count=0
-            )
-        else:
-            bar_data = self._minute_bar_data[ticker]
-
-        if isinstance(market_data, TradeData):
-            bar_data.volume += market_data.volume
-            bar_data.notional += market_data.notional
-            bar_data.trade_count += 1
-
-        bar_data.close_price = market_price
-        bar_data.high_price = max(bar_data.high_price, market_price)
-        bar_data.low_price = min(bar_data.low_price, market_price)
-
-    def _update_active_bar(self, market_data: MarketData, interval: float):
-        ticker = market_data.ticker
-        market_price = market_data.market_price
-        market_time = MarketData.market_time
-
-        if ticker not in self._minute_bar_data or market_time >= self._minute_bar_data[ticker].bar_end_time:
-            bar_data = self._minute_bar_data[ticker] = BarData(
-                ticker=ticker,
-                bar_start_time=datetime.datetime.fromtimestamp(self.mds.timestamp - interval),
-                bar_span=datetime.timedelta(seconds=interval),
-                high_price=market_price,
-                low_price=market_price,
-                open_price=market_price,
-                close_price=market_price,
-                volume=0.,
-                notional=0.,
-                trade_count=0
-            )
-            bar_data.history = []
-
-        else:
-            bar_data = self._minute_bar_data[ticker]
-
-        history: list[TradeData] = getattr(bar_data, 'history')
-        bar_data.bar_start_time = datetime.datetime.fromtimestamp(self.mds.timestamp - interval)
-
-        if isinstance(market_data, TradeData):
-            history.append(market_data)
-
-        while True:
-            if history[0].market_time >= bar_data.bar_start_time:
-                break
-            else:
-                history.pop(0)
-
-        bar_data.volume = sum([_.volume for _ in history])
-        bar_data.notional = sum([_.notional for _ in history])
-        bar_data.trade_count = len([_.notional for _ in history])
-        bar_data.close_price = market_price
-        bar_data.open_price = history[0].market_price
-        bar_data.high_price = max([_.market_price for _ in history])
-        bar_data.low_price = min([_.market_price for _ in history])
-
-    @property
-    def is_ready(self) -> bool:
-        return self._is_ready
-
-    @property
-    def value(self) -> dict[str, BarData]:
-        return self._last_bar_data
-
-
-class Profile(object, metaclass=abc.ABCMeta):
-    def __init__(
-            self,
-            session_start: datetime.time | None = None,
-            session_end: datetime.time | None = None,
-            session_break: tuple[datetime.time, datetime.time] | None = None
-    ):
-        self.session_start: datetime.time | None = session_start
-        self.session_end: datetime.time | None = session_end
-        self.session_break: tuple[datetime.time, datetime.time] | None = session_break
-
-    @abc.abstractmethod
-    def trade_time_between(self, start_time: datetime.datetime | float, end_time: datetime.datetime | float, **kwargs) -> datetime.timedelta:
-        ...
-
-    @abc.abstractmethod
-    def in_trade_session(self, market_time: datetime.datetime | float) -> bool:
-        ...
-
-
-class DefaultProfile(Profile):
-    def __init__(self):
-        super().__init__(
-            session_start=datetime.time(0),
-            session_end=None,
-            session_break=None
-        )
-
-    def trade_time_between(self, start_time: datetime.datetime | float, end_time: datetime.datetime | float, **kwargs) -> datetime.timedelta:
-        if start_time is not None and isinstance(start_time, (float, int)):
-            start_time = datetime.datetime.fromtimestamp(start_time)
-
-        if end_time is not None and isinstance(end_time, (float, int)):
-            end_time = datetime.datetime.fromtimestamp(end_time)
-
-        if start_time is None or end_time is None:
-            return datetime.timedelta(seconds=0)
-
-        if start_time > end_time:
-            return datetime.timedelta(seconds=0)
-
-        return end_time - start_time
-
-    def in_trade_session(self, market_time: datetime.datetime | float) -> bool:
-        return True
-
-
-class CN_Profile(Profile):
-    def __init__(self):
-        super().__init__(
-            session_start=datetime.time(9, 30),
-            session_end=datetime.time(15, 0),
-            session_break=(datetime.time(11, 30), datetime.time(13, 0))
-        )
-
-        self._trade_calendar = {}
-
-    @functools.lru_cache
-    def trade_calendar(self, start_date: datetime.date, end_date: datetime.date, market='XSHG', tz='UTC') -> list[datetime.date]:
-        import pandas as pd
-
-        if market in self.trade_calendar:
-            trade_calendar = self._trade_calendar[market]
-        else:
-            import trading_calendars
-            trade_calendar = self._trade_calendar[market] = trading_calendars.get_calendar(market)
-
-        calendar = trade_calendar.sessions_in_range(
-            pd.Timestamp(start_date, tz=tz),
-            pd.Timestamp(end_date, tz=tz)
-        )
-
-        # noinspection PyTypeChecker
-        result = list(pd.to_datetime(calendar).date)
-
-        return result
-
-    @functools.lru_cache
-    def is_trade_day(self, market_date: datetime.date, market='XSHG', tz='UTC') -> bool:
-        import pandas as pd
-
-        if market in self.trade_calendar:
-            trade_calendar = self._trade_calendar[market]
-        else:
-            import trading_calendars
-            trade_calendar = self._trade_calendar[market] = trading_calendars.get_calendar(market)
-
-        return trade_calendar.is_session(pd.Timestamp(market_date, tz=tz))
-
-    def trade_days_between(self, start_date: datetime.date, end_date: datetime.date = datetime.date.today(), **kwargs) -> int:
-        """
-        Returns the number of trade days between the given date, which is the pre-open of the start_date to the pre-open of the end_date.
-        :param start_date: the given trade date
-        :param end_date: the given trade date
-        :return: integer number of days
-        """
-        assert start_date <= end_date, "The end date must not before the start date"
-
-        if start_date == end_date:
-            offset = 0
-        else:
-            market_date_list = self.trade_calendar(start_date=start_date, end_date=end_date, **kwargs)
-            if not market_date_list:
-                offset = 0
-            else:
-                last_trade_date = market_date_list[-1]
-                offset = len(market_date_list)
-
-                if last_trade_date == end_date:
-                    offset -= 1
-
-        return offset
-
-    @classmethod
-    def time_to_seconds(cls, t: datetime.time):
-        return (t.hour * 60 + t.minute) * 60 + t.second + t.microsecond / 1000
-
-    def trade_time_between(self, start_time: datetime.datetime | datetime.time | float | int, end_time: datetime.datetime | datetime.time | float | int, fmt='timedelta', **kwargs):
-        if start_time is None or end_time is None:
-            if fmt == 'timestamp':
-                return 0.
-            elif fmt == 'timedelta':
-                return datetime.timedelta(0)
-            else:
-                raise NotImplementedError(f'Invalid fmt {fmt}, should be "timestamp" or "timedelta"')
-
-        session_start = kwargs.pop('session_start', self.session_start)
-        session_break = kwargs.pop('session_break', self.session_break)
-        session_end = kwargs.pop('session_end', self.session_end)
-        session_length_0 = datetime.timedelta(seconds=self.time_to_seconds(session_break[0]) - self.time_to_seconds(session_start))
-        session_length_1 = datetime.timedelta(seconds=self.time_to_seconds(session_end) - self.time_to_seconds(session_break[1]))
-        session_length = session_length_0 + session_length_1
-        implied_date = datetime.date.today()
-
-        if isinstance(start_time, (float, int)):
-            start_time = datetime.datetime.fromtimestamp(start_time)
-            implied_date = start_time.date()
-
-        if isinstance(end_time, (float, int)):
-            end_time = datetime.datetime.fromtimestamp(end_time)
-            implied_date = end_time.date()
-
-        if isinstance(start_time, datetime.time):
-            start_time = datetime.datetime.combine(implied_date, start_time)
-
-        if isinstance(end_time, datetime.time):
-            end_time = datetime.datetime.combine(implied_date, end_time)
-
-        offset = datetime.timedelta()
-
-        market_time = start_time.time()
-
-        # calculate the timespan from start_time to session_end
-        if market_time <= session_start:
-            offset += session_length
-        elif session_start < market_time <= session_break[0]:
-            offset += datetime.datetime.combine(start_time.date(), session_break[0]) - start_time
-            offset += session_length_1
-        elif session_break[0] < market_time <= session_break[1]:
-            offset += session_length_1
-        elif session_break[1] < market_time <= session_end:
-            offset += datetime.datetime.combine(start_time.date(), session_end) - start_time
-        else:
-            offset += datetime.timedelta(0)
-
-        offset -= session_length
-
-        market_time = end_time.time()
-
-        # calculate the timespan from session_start to end_time
-        if market_time <= session_start:
-            offset += datetime.timedelta(0)
-        elif session_start < market_time <= session_break[0]:
-            offset += end_time - datetime.datetime.combine(end_time.date(), session_start)
-        elif session_break[0] < market_time <= session_break[1]:
-            offset += session_length_0
-        elif session_break[1] < market_time <= session_end:
-            offset += end_time - datetime.datetime.combine(end_time.date(), session_break[1])
-            offset += session_length_0
-        else:
-            offset += session_length
-
-        # calculate market_date difference
-        if start_time.date() != end_time.date():
-            offset += session_length * self.trade_days_between(start_date=start_time.date(), end_date=end_time.date(), **kwargs)
-
-        if fmt == 'timestamp':
-            return offset.total_seconds()
-        elif fmt == 'timedelta':
-            return offset
-        else:
-            raise NotImplementedError(f'Invalid fmt {fmt}, should be "timestamp" or "timedelta"')
-
-    def in_trade_session(self, market_time: datetime.datetime | float | int = None) -> bool:
-        if market_time is None:
-            market_time = datetime.datetime.now()
-
-        if isinstance(market_time, (float, int)):
-            market_time = datetime.datetime.fromtimestamp(market_time)
-
-        market_date = market_time.date()
-        market_time = market_time.time()
-
-        if not self.is_trade_day(market_date=market_date):
-            return False
-
-        if market_time < datetime.time(9, 30):
-            return False
-
-        if datetime.time(11, 30) < market_time < datetime.time(13, 00):
-            return False
-
-        if market_time > datetime.time(15, 00):
-            return False
-
-        return True
-
-
-class MarketDataService(object):
-    def __init__(self, profile: Profile = None, **kwargs):
-        self.profile = DefaultProfile() if profile is None else profile
-        self.synthetic_orderbook = kwargs.pop('synthetic_orderbook', False)
-        self.cache_history = kwargs.pop('cache_history', False)
-
-        self._market_price = {}
-        self._market_history = defaultdict(dict)
-        self._market_time: datetime.datetime | None = None
-        self._timestamp: float | None = None
-
-        self._order_book: dict[str, OrderBook] = {}
-        self._tick_data: dict[str, TickData] = {}
-        self._trade_data: dict[str, TradeData] = {}
-        self._monitor: dict[str, MarketDataMonitor] = {}
-
-        self.lock = threading.Lock()
-
-        if self.synthetic_orderbook:
-            # init synthetic orderbook monitor
-            _ = SyntheticOrderBookMonitor(mds=self)
-            self.add_monitor(monitor=_)
-            # override current orderbook
-            self._order_book = _.order_book
-
-    def __call__(self, **kwargs):
-        if 'market_data' in kwargs:
-            self.on_market_data(market_data=kwargs['market_data'])
-
-    def __getitem__(self, monitor_id: str) -> MarketDataMonitor:
-        return self._monitor[monitor_id]
-
-    def add_monitor(self, monitor: MarketDataMonitor):
-        self._monitor[monitor.monitor_id] = monitor
-
-    def init_cn_override(self):
-        self.profile = CN_Profile()
-
-    def _on_trade_data(self, trade_data: TradeData):
-        ticker = trade_data.ticker
-
-        if ticker not in self._trade_data:
-            LOGGER.info(f'MDS confirmed {ticker} TradeData subscribed!')
-
-        self._trade_data[ticker] = trade_data
-
-    def _on_tick_data(self, tick_data: TickData):
-        ticker = tick_data.ticker
-
-        if ticker not in self._tick_data:
-            LOGGER.info(f'MDS confirmed {ticker} TickData subscribed!')
-
-        self._tick_data[ticker] = tick_data
-        self._order_book[ticker] = tick_data.order_book
-
-    def _on_order_book(self, order_book):
-        ticker = order_book.ticker
-
-        if ticker not in self._order_book:
-            LOGGER.info(f'MDS confirmed {ticker} OrderBook subscribed!')
-
-        self._order_book[ticker] = order_book
-
-    def on_market_data(self, market_data: MarketData):
-        self.lock.acquire()
-        ticker = market_data.ticker
-        market_time = market_data.market_time
-        timestamp = market_data.timestamp
-        market_price = market_data.market_price
-
-        self._market_price[ticker] = market_price
-        self._market_time = market_time
-        self._timestamp = timestamp
-
-        if self.cache_history:
-            self._market_history[ticker][market_time] = market_price
-
-        if isinstance(market_data, TradeData):
-            self._on_trade_data(trade_data=market_data)
-        elif isinstance(market_data, TickData):
-            self._on_tick_data(tick_data=market_data)
-        elif isinstance(market_data, OrderBook):
-            self._on_order_book(order_book=market_data)
-
-        for monitor_id in self._monitor:
-            monitor = self._monitor.get(monitor_id)
-
-            if monitor is None:
-                continue
-
-            monitor.__call__(market_data)
-
-        self.lock.release()
-
-    def get_order_book(self, ticker: str) -> OrderBook:
-        return self._order_book.get(ticker, None)
-
-    def get_queued_volume(self, ticker: str, side: TransactionSide | str | int, prior: float, posterior: float = None) -> float:
-        """
-        get queued volume prior / posterior to given price, NOT COUNTING GIVEN PRICE!
-        :param ticker: the given ticker
-        :param side: the given trade side
-        :param prior: the given price
-        :param posterior: optional the given posterior price
-        :return: the summed queued volume, in float.
-        """
-        order_book = self.get_order_book(ticker=ticker)
-
-        if order_book is None:
-            queued_volume = float('nan')
-        else:
-            trade_side = TransactionSide(side)
-
-            if trade_side.sign > 0:
-                book = order_book.bid
-            elif trade_side < 0:
-                book = order_book.ask
-            else:
-                raise ValueError(f'Invalid side {side}')
-
-            queued_volume = book.loc(prior=prior, posterior=posterior)
-        return queued_volume
-
-    def trade_time_between(self, start_time: datetime.datetime | float, end_time: datetime.datetime | float, **kwargs) -> datetime.timedelta:
-        return self.profile.trade_time_between(start_time=start_time, end_time=end_time, **kwargs)
-
-    def in_trade_session(self, market_time: datetime.datetime | float) -> bool:
-        return self.profile.in_trade_session(market_time=market_time)
-
-    def clear(self):
-        self.lock.acquire()
-        # self._market_price.clear()
-        # self._market_time = None
-        # self._timestamp = None
-
-        self._market_history.clear()
-        self._order_book.clear()
-        self._monitor.clear()
-        self.lock.release()
-
-    @property
-    def market_price(self) -> dict[str, float]:
-        self.lock.acquire()
-        result = self._market_price
-        self.lock.release()
-        return result
-
-    @property
-    def market_history(self) -> dict[str, dict[datetime.datetime, float]]:
-        self.lock.acquire()
-        result = self._market_history
-        self.lock.release()
-        return result
-
-    @property
-    def market_time(self) -> datetime.datetime | None:
-        if self._market_time is None:
-            if self._timestamp is None:
-                return None
-            else:
-                return datetime.datetime.fromtimestamp(self._timestamp)
-        else:
-            return self._market_time
-
-    @property
-    def market_date(self) -> datetime.date | None:
-        if self.market_time is None:
-            return None
-
-        return self._market_time.date()
-
-    @property
-    def timestamp(self) -> float | None:
-        if self._timestamp is None:
-            if self._market_time is None:
-                return None
-            else:
-                return self._market_time.timestamp()
-        else:
-            return self._timestamp
-
-    @property
-    def session_start(self) -> datetime.time | None:
-        return self.profile.session_start
-
-    @property
-    def session_end(self) -> datetime.time | None:
-        return self.profile.session_end
-
-    @property
-    def session_break(self) -> tuple[datetime.time, datetime.time] | None:
-        return self.profile.session_break
-
-
-class Replay(object, metaclass=abc.ABCMeta):
-    @abc.abstractmethod
-    def __next__(self): ...
-
-    @abc.abstractmethod
-    def __iter__(self): ...
-
-
-class SimpleReplay(Replay):
-    def __init__(self, **kwargs):
-        self.eod = kwargs.pop('eod', None)
-        self.bod = kwargs.pop('bod', None)
-
-        self.replay_task = []
-        self.task_progress = 0
-        self.task_date = None
-        self.progress = Progress(tasks=1, **kwargs)
-
-    def load(self, data):
-        if isinstance(data, dict):
-            self.replay_task.extend(list(data.values()))
-        else:
-            self.replay_task.extend(data)
-
-    def reset(self):
-        self.replay_task.clear()
-        self.task_progress = 0
-        self.task_date = None
-        self.progress.reset()
-
-    def next_task(self):
-        if self.task_progress < len(self.replay_task):
-            market_data = self.replay_task[self.task_progress]
-            market_time = market_data.market_time
-
-            if isinstance(market_time, datetime.datetime):
-                market_date = market_time.date()
-            else:
-                market_date = market_time
-
-            if market_date != self.task_date:
-                if callable(self.eod) and self.task_date:
-                    self.eod(self.task_date)
-
-                self.task_date = market_date
-                self.progress.prompt = f'Replay {market_date:%Y-%m-%d}:'
-
-                if callable(self.bod):
-                    self.bod(market_date)
-
-            self.progress.done_tasks = self.task_progress / len(self.replay_task)
-
-            if (not self.progress.tick_size) or self.progress.progress >= self.progress.tick_size + self.progress.last_output:
-                self.progress.output()
-
-            self.task_progress += 1
-        else:
-            raise StopIteration()
-
-        return market_data
-
-    def __next__(self):
-        try:
-            return self.next_task()
-        except StopIteration:
-            if not self.progress.is_done:
-                self.progress.done_tasks = 1
-                self.progress.output()
-
-            self.reset()
-            raise StopIteration()
-
-    def __iter__(self):
-        return self
-
-
-class ProgressiveReplay(Replay):
-    """
-    progressively loading and replaying market data
-
-    requires arguments
-    loader: a data loading function. Expect loader = Callable(market_date: datetime.date, ticker: str, dtype: str| type) -> dict[any, MarketData]
-    start_date & end_date: the given replay period
-    or calendar: the given replay calendar.
-
-    accepts kwargs:
-    ticker / tickers: the given symbols to replay, expect a str| list[str]
-    dtype / dtypes: the given dtype(s) of symbol to replay, expect a str | type, list[str | type]. default = all, which is (TradeData, TickData, OrderBook)
-    subscription / subscribe: the given ticker-dtype pair to replay, expect a list[dict[str, str | type]]
-    """
-
-    def __init__(
-            self,
-            loader,
-            **kwargs
-    ):
-        self.loader = loader
-        self.start_date: datetime.date = kwargs.pop('start_date', None)
-        self.end_date: datetime.date = kwargs.pop('end_date', None)
-        self.calendar: list[datetime.date] = kwargs.pop('calendar', None)
-
-        self.eod = kwargs.pop('eod', None)
-        self.bod = kwargs.pop('bod', None)
-
-        self.replay_subscription = {}
-        self.replay_calendar = []
-        self.replay_task = []
-
-        self.date_progress = 0
-        self.task_progress = 0
-        self.progress = Progress(tasks=1, **kwargs)
-
-        tickers = kwargs.pop('ticker', kwargs.pop('tickers', []))
-        dtypes = kwargs.pop('dtype', kwargs.pop('dtypes', [TradeData, OrderBook, TickData]))
-
-        if not isinstance(tickers, list):
-            tickers = [tickers]
-
-        if not isinstance(dtypes, list):
-            dtypes = [dtypes]
-
-        for ticker in tickers:
-            for dtype in dtypes:
-                self.add_subscription(ticker=ticker, dtype=dtype)
-
-        subscription = kwargs.pop('subscription', kwargs.pop('subscribe', []))
-
-        if not isinstance(subscription, list):
-            subscription = [subscription]
-
-        for sub in subscription:
-            self.add_subscription(**sub)
-
-        self.reset()
-
-    def add_subscription(self, ticker: str, dtype: type | str):
-        if isinstance(dtype, str):
-            pass
-        else:
-            dtype = dtype.__name__
-
-        topic = f'{ticker}.{dtype}'
-        self.replay_subscription[topic] = (ticker, dtype)
-
-    def remove_subscription(self, ticker: str, dtype: type | str):
-        if isinstance(dtype, str):
-            pass
-        else:
-            dtype = dtype.__name__
-
-        topic = f'{ticker}.{dtype}'
-        self.replay_subscription.pop(topic, None)
-
-    def reset(self):
-        if self.calendar is None:
-            md = self.start_date
-            self.replay_calendar.clear()
-
-            while md <= self.end_date:
-                self.replay_calendar.append(md)
-                md += datetime.timedelta(days=1)
-
-        elif callable(self.calendar):
-            self.replay_calendar = self.calendar(start_date=self.start_date, end_date=self.end_date)
-        else:
-            self.replay_calendar = self.calendar
-
-        self.date_progress = 0
-        self.progress.reset()
-
-    def next_trade_day(self):
-        self.replay_task.clear()
-        self.task_progress = 0
-
-        if self.date_progress < len(self.replay_calendar):
-            market_date = self.replay_calendar[self.date_progress]
-            self.progress.prompt = f'Replay {market_date:%Y-%m-%d} ({self.date_progress + 1} / {len(self.replay_calendar)}):'
-            for topic in self.replay_subscription:
-                ticker, dtype = self.replay_subscription[topic]
-                LOGGER.info(f'{self} loading {market_date} {ticker} {dtype}')
-                data = self.loader(market_date=market_date, ticker=ticker, dtype=dtype)
-
-                if isinstance(data, dict):
-                    self.replay_task.extend(list(data.values()))
-                elif isinstance(data, (list, tuple)):
-                    self.replay_task.extend(data)
-
-            self.date_progress += 1
-        else:
-            raise StopIteration()
-
-        self.replay_task.sort(key=lambda x: x.market_time)
-
-    def next_task(self):
-        if self.task_progress < len(self.replay_task):
-            data = self.replay_task[self.task_progress]
-            self.task_progress += 1
-        else:
-            if self.eod is not None and self.date_progress:
-                self.eod(market_date=self.replay_calendar[self.date_progress - 1], replay=self)
-
-            if self.bod is not None and self.date_progress < len(self.replay_calendar):
-                self.bod(market_date=self.replay_calendar[self.date_progress], replay=self)
-
-            self.next_trade_day()
-
-            data = self.next_task()
-
-        if self.replay_task and self.replay_calendar:
-            current_progress = (self.date_progress - 1 + (self.task_progress / len(self.replay_task))) / len(self.replay_calendar)
-            self.progress.done_tasks = current_progress
-        else:
-            self.progress.done_tasks = 1
-
-        if (not self.progress.tick_size) \
-                or self.progress.progress >= self.progress.tick_size + self.progress.last_output \
-                or self.progress.is_done:
-            self.progress.output()
-
-        return data
-
-    def __next__(self):
-        try:
-            return self.next_task()
-        except StopIteration:
-            if not self.progress.is_done:
-                self.progress.done_tasks = 1
-                self.progress.output()
-
-            self.reset()
-            raise StopIteration()
-
-    def __iter__(self):
-        self.reset()
-        return self
-
-    def __repr__(self):
-        return f'{self.__class__.__name__}{{id={id(self)}, from={self.start_date}, to={self.end_date}}}'
-
-
-MDS = MarketDataService()
+from __future__ import annotations
+
+import abc
+import datetime
+import functools
+import threading
+import uuid
+from collections import defaultdict
+
+from PyQuantKit import TickData, TradeData, OrderBook, MarketData, Progress, TransactionSide, BarData, TransactionData
+
+from . import LOGGER
+
+__all__ = ['MDS', 'MarketDataService', 'MarketDataMonitor', 'SyntheticOrderBookMonitor', 'MinuteBarMonitor', 'Profile', 'ProgressiveReplay', 'SimpleReplay', 'Replay']
+LOGGER = LOGGER.getChild('MarketEngine')
+
+
+class MarketDataMonitor(object, metaclass=abc.ABCMeta):
+    """
+    this is a template for market data monitor
+
+    A data monitor is a module that process market data and generate custom index
+
+    When MDS receive an update of market data, the __call__ function of this monitor is triggered.
+
+    Note: all the market_data, of all subscribed ticker will be fed into monitor. It should be assumed that a storage for multiple ticker is required.
+    To access the monitor, use `monitor = MDS[monitor_id]`
+    To access the index generated by the monitor, use `monitor.value`
+    To indicate that the monitor is ready to use set `monitor.is_ready = True`
+
+    The implemented monitor should be initialized and use `MDS.add_monitor(monitor)` to attach onto the engine
+    """
+
+    def __init__(self, name: str, monitor_id: str = None, mds: MarketDataService = None):
+        self.name = name
+        self.monitor_id = uuid.uuid4().hex if monitor_id is None else monitor_id
+        self.mds = MDS if mds is None else mds
+
+    @abc.abstractmethod
+    def __call__(self, market_data: MarketData, **kwargs): ...
+
+    @property
+    @abc.abstractmethod
+    def value(self): ...
+
+    @property
+    @abc.abstractmethod
+    def is_ready(self) -> bool: ...
+
+
+class SyntheticOrderBookMonitor(MarketDataMonitor):
+    def __init__(self, keep_order_log: bool = False, **kwargs):
+        self.keep_order_log = keep_order_log
+
+        super().__init__(
+            name=kwargs.pop('name', 'Monitor.SyntheticOrderBook'),
+            monitor_id=kwargs.pop('monitor_id', None),
+            mds=kwargs.pop('mds', None),
+        )
+
+        self._is_ready = True
+        self._value = {}
+        self.order_book = {}
+        self.order_log = {}
+
+    def __call__(self, market_data: MarketData, **kwargs):
+        if isinstance(market_data, TradeData):
+            self.on_trade_data(trade_data=market_data)
+
+    def on_trade_data(self, trade_data: TradeData):
+        ticker = trade_data.ticker
+
+        if order_book := self.order_book.get(ticker):
+            if order_book.market_time <= trade_data.market_time:
+                side: TransactionSide = trade_data.side
+                price = trade_data.price
+                book = order_book.ask if side.sign > 0 else order_book.bid
+                listed_volume = book.at_price(price).volume if price in book else 0.
+                traded_volume = trade_data.volume
+                book.update_entry(price=price, volume=max(0, listed_volume - traded_volume))
+
+        if self.keep_order_log:
+            self._update_order_log(trade_data=trade_data)
+
+    def on_transaction_data(self, transaction_data: TransactionData):
+        pass
+
+    def _update_order_log(self, trade_data: TradeData):
+        side: TransactionSide = trade_data.side
+        price = trade_data.price
+        traded_volume = trade_data.volume
+
+        for order_id in list(self.order_log):
+            order_log = self.order_log.get(order_id)
+
+            if order_log is None:
+                continue
+
+            if side.sign > 0:
+                if order_log.side.sign < 0:
+                    if price == order_log.price:
+                        order_log.volume -= traded_volume
+                    elif price > order_log.price:
+                        order_log.volume = 0.
+                else:
+                    if price <= order_log.price:
+                        order_log.volume = 0.
+            elif side.sign < 0:
+                if order_log.side.sign > 0:
+                    if price == order_log.price:
+                        order_log.volume -= traded_volume
+                    elif price < order_log.price:
+                        order_log.volume = 0.
+                else:
+                    if price >= order_log.price:
+                        order_log.volume = 0.
+
+            if order_log.volume <= 0:
+                self.order_log.pop(order_id)
+
+    @property
+    def is_ready(self) -> bool:
+        return self._is_ready
+
+    @property
+    def value(self) -> dict[str, OrderBook]:
+        return self.order_book
+
+
+class MinuteBarMonitor(MarketDataMonitor):
+    def __init__(self, interval: float = 60., **kwargs):
+        self.interval = interval
+
+        super().__init__(
+            name=kwargs.pop('name', 'Monitor.MinuteBarMonitor'),
+            monitor_id=kwargs.pop('monitor_id', None),
+            mds=kwargs.pop('mds', None),
+        )
+
+        self._minute_bar_data: dict[str, BarData] = {}
+        self._last_bar_data: dict[str, BarData] = {}
+
+        self._is_ready = True
+        self._value = {}
+
+    def __call__(self, market_data: MarketData, **kwargs):
+        self._update_last_bar(market_data=market_data, interval=self.interval)
+        # self._update_active_bar(market_data=market_data, interval=self.interval)
+
+    def _update_last_bar(self, market_data: MarketData, interval: float):
+        ticker = market_data.ticker
+        market_price = market_data.market_price
+        market_time = market_data.market_time
+
+        if ticker not in self._minute_bar_data or market_time >= self._minute_bar_data[ticker].bar_end_time:
+            # update bar_data
+            if ticker in self._minute_bar_data:
+                self._last_bar_data[ticker] = self._minute_bar_data[ticker]
+
+            bar_data = self._minute_bar_data[ticker] = BarData(
+                ticker=ticker,
+                bar_start_time=datetime.datetime.fromtimestamp(self.mds.timestamp // interval * interval),
+                bar_span=datetime.timedelta(seconds=interval),
+                high_price=market_price,
+                low_price=market_price,
+                open_price=market_price,
+                close_price=market_price,
+                volume=0.,
+                notional=0.,
+                trade_count=0
+            )
+        else:
+            bar_data = self._minute_bar_data[ticker]
+
+        if isinstance(market_data, TradeData):
+            bar_data.volume += market_data.volume
+            bar_data.notional += market_data.notional
+            bar_data.trade_count += 1
+
+        bar_data.close_price = market_price
+        bar_data.high_price = max(bar_data.high_price, market_price)
+        bar_data.low_price = min(bar_data.low_price, market_price)
+
+    def _update_active_bar(self, market_data: MarketData, interval: float):
+        ticker = market_data.ticker
+        market_price = market_data.market_price
+        market_time = MarketData.market_time
+
+        if ticker not in self._minute_bar_data or market_time >= self._minute_bar_data[ticker].bar_end_time:
+            bar_data = self._minute_bar_data[ticker] = BarData(
+                ticker=ticker,
+                bar_start_time=datetime.datetime.fromtimestamp(self.mds.timestamp - interval),
+                bar_span=datetime.timedelta(seconds=interval),
+                high_price=market_price,
+                low_price=market_price,
+                open_price=market_price,
+                close_price=market_price,
+                volume=0.,
+                notional=0.,
+                trade_count=0
+            )
+            bar_data.history = []
+
+        else:
+            bar_data = self._minute_bar_data[ticker]
+
+        history: list[TradeData] = getattr(bar_data, 'history')
+        bar_data.bar_start_time = datetime.datetime.fromtimestamp(self.mds.timestamp - interval)
+
+        if isinstance(market_data, TradeData):
+            history.append(market_data)
+
+        while True:
+            if history[0].market_time >= bar_data.bar_start_time:
+                break
+            else:
+                history.pop(0)
+
+        bar_data.volume = sum([_.volume for _ in history])
+        bar_data.notional = sum([_.notional for _ in history])
+        bar_data.trade_count = len([_.notional for _ in history])
+        bar_data.close_price = market_price
+        bar_data.open_price = history[0].market_price
+        bar_data.high_price = max([_.market_price for _ in history])
+        bar_data.low_price = min([_.market_price for _ in history])
+
+    @property
+    def is_ready(self) -> bool:
+        return self._is_ready
+
+    @property
+    def value(self) -> dict[str, BarData]:
+        return self._last_bar_data
+
+
+class Profile(object, metaclass=abc.ABCMeta):
+    def __init__(
+            self,
+            session_start: datetime.time | None = None,
+            session_end: datetime.time | None = None,
+            session_break: tuple[datetime.time, datetime.time] | None = None
+    ):
+        self.session_start: datetime.time | None = session_start
+        self.session_end: datetime.time | None = session_end
+        self.session_break: tuple[datetime.time, datetime.time] | None = session_break
+
+    @abc.abstractmethod
+    def trade_time_between(self, start_time: datetime.datetime | float, end_time: datetime.datetime | float, **kwargs) -> datetime.timedelta:
+        ...
+
+    @abc.abstractmethod
+    def in_trade_session(self, market_time: datetime.datetime | float) -> bool:
+        ...
+
+
+class DefaultProfile(Profile):
+    def __init__(self):
+        super().__init__(
+            session_start=datetime.time(0),
+            session_end=None,
+            session_break=None
+        )
+
+    def trade_time_between(self, start_time: datetime.datetime | float, end_time: datetime.datetime | float, **kwargs) -> datetime.timedelta:
+        if start_time is not None and isinstance(start_time, (float, int)):
+            start_time = datetime.datetime.fromtimestamp(start_time)
+
+        if end_time is not None and isinstance(end_time, (float, int)):
+            end_time = datetime.datetime.fromtimestamp(end_time)
+
+        if start_time is None or end_time is None:
+            return datetime.timedelta(seconds=0)
+
+        if start_time > end_time:
+            return datetime.timedelta(seconds=0)
+
+        return end_time - start_time
+
+    def in_trade_session(self, market_time: datetime.datetime | float) -> bool:
+        return True
+
+
+class CN_Profile(Profile):
+    def __init__(self):
+        super().__init__(
+            session_start=datetime.time(9, 30),
+            session_end=datetime.time(15, 0),
+            session_break=(datetime.time(11, 30), datetime.time(13, 0))
+        )
+
+        self._trade_calendar = {}
+
+    @functools.lru_cache
+    def trade_calendar(self, start_date: datetime.date, end_date: datetime.date, market='XSHG', tz='UTC') -> list[datetime.date]:
+        import pandas as pd
+
+        if market in self.trade_calendar:
+            trade_calendar = self._trade_calendar[market]
+        else:
+            import exchange_calendars
+            trade_calendar = self._trade_calendar[market] = exchange_calendars.get_calendar(market)
+
+        calendar = trade_calendar.sessions_in_range(
+            pd.Timestamp(start_date, tz=tz),
+            pd.Timestamp(end_date, tz=tz)
+        )
+
+        # noinspection PyTypeChecker
+        result = list(pd.to_datetime(calendar).date)
+
+        return result
+
+    @functools.lru_cache
+    def is_trade_day(self, market_date: datetime.date, market='XSHG', tz='UTC') -> bool:
+        import pandas as pd
+
+        if market in self.trade_calendar:
+            trade_calendar = self._trade_calendar[market]
+        else:
+            import exchange_calendars
+            trade_calendar = self._trade_calendar[market] = exchange_calendars.get_calendar(market)
+
+        return trade_calendar.is_session(pd.Timestamp(market_date, tz=tz))
+
+    def trade_days_between(self, start_date: datetime.date, end_date: datetime.date = datetime.date.today(), **kwargs) -> int:
+        """
+        Returns the number of trade days between the given date, which is the pre-open of the start_date to the pre-open of the end_date.
+        :param start_date: the given trade date
+        :param end_date: the given trade date
+        :return: integer number of days
+        """
+        assert start_date <= end_date, "The end date must not before the start date"
+
+        if start_date == end_date:
+            offset = 0
+        else:
+            market_date_list = self.trade_calendar(start_date=start_date, end_date=end_date, **kwargs)
+            if not market_date_list:
+                offset = 0
+            else:
+                last_trade_date = market_date_list[-1]
+                offset = len(market_date_list)
+
+                if last_trade_date == end_date:
+                    offset -= 1
+
+        return offset
+
+    @classmethod
+    def time_to_seconds(cls, t: datetime.time):
+        return (t.hour * 60 + t.minute) * 60 + t.second + t.microsecond / 1000
+
+    def trade_time_between(self, start_time: datetime.datetime | datetime.time | float | int, end_time: datetime.datetime | datetime.time | float | int, fmt='timedelta', **kwargs):
+        if start_time is None or end_time is None:
+            if fmt == 'timestamp':
+                return 0.
+            elif fmt == 'timedelta':
+                return datetime.timedelta(0)
+            else:
+                raise NotImplementedError(f'Invalid fmt {fmt}, should be "timestamp" or "timedelta"')
+
+        session_start = kwargs.pop('session_start', self.session_start)
+        session_break = kwargs.pop('session_break', self.session_break)
+        session_end = kwargs.pop('session_end', self.session_end)
+        session_length_0 = datetime.timedelta(seconds=self.time_to_seconds(session_break[0]) - self.time_to_seconds(session_start))
+        session_length_1 = datetime.timedelta(seconds=self.time_to_seconds(session_end) - self.time_to_seconds(session_break[1]))
+        session_length = session_length_0 + session_length_1
+        implied_date = datetime.date.today()
+
+        if isinstance(start_time, (float, int)):
+            start_time = datetime.datetime.fromtimestamp(start_time)
+            implied_date = start_time.date()
+
+        if isinstance(end_time, (float, int)):
+            end_time = datetime.datetime.fromtimestamp(end_time)
+            implied_date = end_time.date()
+
+        if isinstance(start_time, datetime.time):
+            start_time = datetime.datetime.combine(implied_date, start_time)
+
+        if isinstance(end_time, datetime.time):
+            end_time = datetime.datetime.combine(implied_date, end_time)
+
+        offset = datetime.timedelta()
+
+        market_time = start_time.time()
+
+        # calculate the timespan from start_time to session_end
+        if market_time <= session_start:
+            offset += session_length
+        elif session_start < market_time <= session_break[0]:
+            offset += datetime.datetime.combine(start_time.date(), session_break[0]) - start_time
+            offset += session_length_1
+        elif session_break[0] < market_time <= session_break[1]:
+            offset += session_length_1
+        elif session_break[1] < market_time <= session_end:
+            offset += datetime.datetime.combine(start_time.date(), session_end) - start_time
+        else:
+            offset += datetime.timedelta(0)
+
+        offset -= session_length
+
+        market_time = end_time.time()
+
+        # calculate the timespan from session_start to end_time
+        if market_time <= session_start:
+            offset += datetime.timedelta(0)
+        elif session_start < market_time <= session_break[0]:
+            offset += end_time - datetime.datetime.combine(end_time.date(), session_start)
+        elif session_break[0] < market_time <= session_break[1]:
+            offset += session_length_0
+        elif session_break[1] < market_time <= session_end:
+            offset += end_time - datetime.datetime.combine(end_time.date(), session_break[1])
+            offset += session_length_0
+        else:
+            offset += session_length
+
+        # calculate market_date difference
+        if start_time.date() != end_time.date():
+            offset += session_length * self.trade_days_between(start_date=start_time.date(), end_date=end_time.date(), **kwargs)
+
+        if fmt == 'timestamp':
+            return offset.total_seconds()
+        elif fmt == 'timedelta':
+            return offset
+        else:
+            raise NotImplementedError(f'Invalid fmt {fmt}, should be "timestamp" or "timedelta"')
+
+    def in_trade_session(self, market_time: datetime.datetime | float | int = None) -> bool:
+        if market_time is None:
+            market_time = datetime.datetime.now()
+
+        if isinstance(market_time, (float, int)):
+            market_time = datetime.datetime.fromtimestamp(market_time)
+
+        market_date = market_time.date()
+        market_time = market_time.time()
+
+        if not self.is_trade_day(market_date=market_date):
+            return False
+
+        if market_time < datetime.time(9, 30):
+            return False
+
+        if datetime.time(11, 30) < market_time < datetime.time(13, 00):
+            return False
+
+        if market_time > datetime.time(15, 00):
+            return False
+
+        return True
+
+
+class MarketDataService(object):
+    def __init__(self, profile: Profile = None, **kwargs):
+        self.profile = DefaultProfile() if profile is None else profile
+        self.synthetic_orderbook = kwargs.pop('synthetic_orderbook', False)
+        self.cache_history = kwargs.pop('cache_history', False)
+
+        self._market_price = {}
+        self._market_history = defaultdict(dict)
+        self._market_time: datetime.datetime | None = None
+        self._timestamp: float | None = None
+
+        self._order_book: dict[str, OrderBook] = {}
+        self._tick_data: dict[str, TickData] = {}
+        self._trade_data: dict[str, TradeData] = {}
+        self._monitor: dict[str, MarketDataMonitor] = {}
+
+        self.lock = threading.Lock()
+
+        if self.synthetic_orderbook:
+            # init synthetic orderbook monitor
+            _ = SyntheticOrderBookMonitor(mds=self)
+            self.add_monitor(monitor=_)
+            # override current orderbook
+            self._order_book = _.order_book
+
+    def __call__(self, **kwargs):
+        if 'market_data' in kwargs:
+            self.on_market_data(market_data=kwargs['market_data'])
+
+    def __getitem__(self, monitor_id: str) -> MarketDataMonitor:
+        return self._monitor[monitor_id]
+
+    def add_monitor(self, monitor: MarketDataMonitor):
+        self._monitor[monitor.monitor_id] = monitor
+
+    def init_cn_override(self):
+        self.profile = CN_Profile()
+
+    def _on_trade_data(self, trade_data: TradeData):
+        ticker = trade_data.ticker
+
+        if ticker not in self._trade_data:
+            LOGGER.info(f'MDS confirmed {ticker} TradeData subscribed!')
+
+        self._trade_data[ticker] = trade_data
+
+    def _on_tick_data(self, tick_data: TickData):
+        ticker = tick_data.ticker
+
+        if ticker not in self._tick_data:
+            LOGGER.info(f'MDS confirmed {ticker} TickData subscribed!')
+
+        self._tick_data[ticker] = tick_data
+        self._order_book[ticker] = tick_data.order_book
+
+    def _on_order_book(self, order_book):
+        ticker = order_book.ticker
+
+        if ticker not in self._order_book:
+            LOGGER.info(f'MDS confirmed {ticker} OrderBook subscribed!')
+
+        self._order_book[ticker] = order_book
+
+    def on_market_data(self, market_data: MarketData):
+        self.lock.acquire()
+        ticker = market_data.ticker
+        market_time = market_data.market_time
+        timestamp = market_data.timestamp
+        market_price = market_data.market_price
+
+        self._market_price[ticker] = market_price
+        self._market_time = market_time
+        self._timestamp = timestamp
+
+        if self.cache_history:
+            self._market_history[ticker][market_time] = market_price
+
+        if isinstance(market_data, TradeData):
+            self._on_trade_data(trade_data=market_data)
+        elif isinstance(market_data, TickData):
+            self._on_tick_data(tick_data=market_data)
+        elif isinstance(market_data, OrderBook):
+            self._on_order_book(order_book=market_data)
+
+        for monitor_id in self._monitor:
+            monitor = self._monitor.get(monitor_id)
+
+            if monitor is None:
+                continue
+
+            monitor.__call__(market_data)
+
+        self.lock.release()
+
+    def get_order_book(self, ticker: str) -> OrderBook:
+        return self._order_book.get(ticker, None)
+
+    def get_queued_volume(self, ticker: str, side: TransactionSide | str | int, prior: float, posterior: float = None) -> float:
+        """
+        get queued volume prior / posterior to given price, NOT COUNTING GIVEN PRICE!
+        :param ticker: the given ticker
+        :param side: the given trade side
+        :param prior: the given price
+        :param posterior: optional the given posterior price
+        :return: the summed queued volume, in float.
+        """
+        order_book = self.get_order_book(ticker=ticker)
+
+        if order_book is None:
+            queued_volume = float('nan')
+        else:
+            trade_side = TransactionSide(side)
+
+            if trade_side.sign > 0:
+                book = order_book.bid
+            elif trade_side < 0:
+                book = order_book.ask
+            else:
+                raise ValueError(f'Invalid side {side}')
+
+            queued_volume = book.loc(prior=prior, posterior=posterior)
+        return queued_volume
+
+    def trade_time_between(self, start_time: datetime.datetime | float, end_time: datetime.datetime | float, **kwargs) -> datetime.timedelta:
+        return self.profile.trade_time_between(start_time=start_time, end_time=end_time, **kwargs)
+
+    def in_trade_session(self, market_time: datetime.datetime | float) -> bool:
+        return self.profile.in_trade_session(market_time=market_time)
+
+    def clear(self):
+        self.lock.acquire()
+        # self._market_price.clear()
+        # self._market_time = None
+        # self._timestamp = None
+
+        self._market_history.clear()
+        self._order_book.clear()
+        self._monitor.clear()
+        self.lock.release()
+
+    @property
+    def market_price(self) -> dict[str, float]:
+        self.lock.acquire()
+        result = self._market_price
+        self.lock.release()
+        return result
+
+    @property
+    def market_history(self) -> dict[str, dict[datetime.datetime, float]]:
+        self.lock.acquire()
+        result = self._market_history
+        self.lock.release()
+        return result
+
+    @property
+    def market_time(self) -> datetime.datetime | None:
+        if self._market_time is None:
+            if self._timestamp is None:
+                return None
+            else:
+                return datetime.datetime.fromtimestamp(self._timestamp)
+        else:
+            return self._market_time
+
+    @property
+    def market_date(self) -> datetime.date | None:
+        if self.market_time is None:
+            return None
+
+        return self._market_time.date()
+
+    @property
+    def timestamp(self) -> float | None:
+        if self._timestamp is None:
+            if self._market_time is None:
+                return None
+            else:
+                return self._market_time.timestamp()
+        else:
+            return self._timestamp
+
+    @property
+    def session_start(self) -> datetime.time | None:
+        return self.profile.session_start
+
+    @property
+    def session_end(self) -> datetime.time | None:
+        return self.profile.session_end
+
+    @property
+    def session_break(self) -> tuple[datetime.time, datetime.time] | None:
+        return self.profile.session_break
+
+
+class Replay(object, metaclass=abc.ABCMeta):
+    @abc.abstractmethod
+    def __next__(self): ...
+
+    @abc.abstractmethod
+    def __iter__(self): ...
+
+
+class SimpleReplay(Replay):
+    def __init__(self, **kwargs):
+        self.eod = kwargs.pop('eod', None)
+        self.bod = kwargs.pop('bod', None)
+
+        self.replay_task = []
+        self.task_progress = 0
+        self.task_date = None
+        self.progress = Progress(tasks=1, **kwargs)
+
+    def load(self, data):
+        if isinstance(data, dict):
+            self.replay_task.extend(list(data.values()))
+        else:
+            self.replay_task.extend(data)
+
+    def reset(self):
+        self.replay_task.clear()
+        self.task_progress = 0
+        self.task_date = None
+        self.progress.reset()
+
+    def next_task(self):
+        if self.task_progress < len(self.replay_task):
+            market_data = self.replay_task[self.task_progress]
+            market_time = market_data.market_time
+
+            if isinstance(market_time, datetime.datetime):
+                market_date = market_time.date()
+            else:
+                market_date = market_time
+
+            if market_date != self.task_date:
+                if callable(self.eod) and self.task_date:
+                    self.eod(self.task_date)
+
+                self.task_date = market_date
+                self.progress.prompt = f'Replay {market_date:%Y-%m-%d}:'
+
+                if callable(self.bod):
+                    self.bod(market_date)
+
+            self.progress.done_tasks = self.task_progress / len(self.replay_task)
+
+            if (not self.progress.tick_size) or self.progress.progress >= self.progress.tick_size + self.progress.last_output:
+                self.progress.output()
+
+            self.task_progress += 1
+        else:
+            raise StopIteration()
+
+        return market_data
+
+    def __next__(self):
+        try:
+            return self.next_task()
+        except StopIteration:
+            if not self.progress.is_done:
+                self.progress.done_tasks = 1
+                self.progress.output()
+
+            self.reset()
+            raise StopIteration()
+
+    def __iter__(self):
+        return self
+
+
+class ProgressiveReplay(Replay):
+    """
+    progressively loading and replaying market data
+
+    requires arguments
+    loader: a data loading function. Expect loader = Callable(market_date: datetime.date, ticker: str, dtype: str| type) -> dict[any, MarketData]
+    start_date & end_date: the given replay period
+    or calendar: the given replay calendar.
+
+    accepts kwargs:
+    ticker / tickers: the given symbols to replay, expect a str| list[str]
+    dtype / dtypes: the given dtype(s) of symbol to replay, expect a str | type, list[str | type]. default = all, which is (TradeData, TickData, OrderBook)
+    subscription / subscribe: the given ticker-dtype pair to replay, expect a list[dict[str, str | type]]
+    """
+
+    def __init__(
+            self,
+            loader,
+            **kwargs
+    ):
+        self.loader = loader
+        self.start_date: datetime.date = kwargs.pop('start_date', None)
+        self.end_date: datetime.date = kwargs.pop('end_date', None)
+        self.calendar: list[datetime.date] = kwargs.pop('calendar', None)
+
+        self.eod = kwargs.pop('eod', None)
+        self.bod = kwargs.pop('bod', None)
+
+        self.replay_subscription = {}
+        self.replay_calendar = []
+        self.replay_task = []
+
+        self.date_progress = 0
+        self.task_progress = 0
+        self.progress = Progress(tasks=1, **kwargs)
+
+        tickers = kwargs.pop('ticker', kwargs.pop('tickers', []))
+        dtypes = kwargs.pop('dtype', kwargs.pop('dtypes', [TradeData, OrderBook, TickData]))
+
+        if not isinstance(tickers, list):
+            tickers = [tickers]
+
+        if not isinstance(dtypes, list):
+            dtypes = [dtypes]
+
+        for ticker in tickers:
+            for dtype in dtypes:
+                self.add_subscription(ticker=ticker, dtype=dtype)
+
+        subscription = kwargs.pop('subscription', kwargs.pop('subscribe', []))
+
+        if not isinstance(subscription, list):
+            subscription = [subscription]
+
+        for sub in subscription:
+            self.add_subscription(**sub)
+
+        self.reset()
+
+    def add_subscription(self, ticker: str, dtype: type | str):
+        if isinstance(dtype, str):
+            pass
+        else:
+            dtype = dtype.__name__
+
+        topic = f'{ticker}.{dtype}'
+        self.replay_subscription[topic] = (ticker, dtype)
+
+    def remove_subscription(self, ticker: str, dtype: type | str):
+        if isinstance(dtype, str):
+            pass
+        else:
+            dtype = dtype.__name__
+
+        topic = f'{ticker}.{dtype}'
+        self.replay_subscription.pop(topic, None)
+
+    def reset(self):
+        if self.calendar is None:
+            md = self.start_date
+            self.replay_calendar.clear()
+
+            while md <= self.end_date:
+                self.replay_calendar.append(md)
+                md += datetime.timedelta(days=1)
+
+        elif callable(self.calendar):
+            self.replay_calendar = self.calendar(start_date=self.start_date, end_date=self.end_date)
+        else:
+            self.replay_calendar = self.calendar
+
+        self.date_progress = 0
+        self.progress.reset()
+
+    def next_trade_day(self):
+        self.replay_task.clear()
+        self.task_progress = 0
+
+        if self.date_progress < len(self.replay_calendar):
+            market_date = self.replay_calendar[self.date_progress]
+            self.progress.prompt = f'Replay {market_date:%Y-%m-%d} ({self.date_progress + 1} / {len(self.replay_calendar)}):'
+            for topic in self.replay_subscription:
+                ticker, dtype = self.replay_subscription[topic]
+                LOGGER.info(f'{self} loading {market_date} {ticker} {dtype}')
+                data = self.loader(market_date=market_date, ticker=ticker, dtype=dtype)
+
+                if isinstance(data, dict):
+                    self.replay_task.extend(list(data.values()))
+                elif isinstance(data, (list, tuple)):
+                    self.replay_task.extend(data)
+
+            self.date_progress += 1
+        else:
+            raise StopIteration()
+
+        self.replay_task.sort(key=lambda x: x.market_time)
+
+    def next_task(self):
+        if self.task_progress < len(self.replay_task):
+            data = self.replay_task[self.task_progress]
+            self.task_progress += 1
+        else:
+            if self.eod is not None and self.date_progress:
+                self.eod(market_date=self.replay_calendar[self.date_progress - 1], replay=self)
+
+            if self.bod is not None and self.date_progress < len(self.replay_calendar):
+                self.bod(market_date=self.replay_calendar[self.date_progress], replay=self)
+
+            self.next_trade_day()
+
+            data = self.next_task()
+
+        if self.replay_task and self.replay_calendar:
+            current_progress = (self.date_progress - 1 + (self.task_progress / len(self.replay_task))) / len(self.replay_calendar)
+            self.progress.done_tasks = current_progress
+        else:
+            self.progress.done_tasks = 1
+
+        if (not self.progress.tick_size) \
+                or self.progress.progress >= self.progress.tick_size + self.progress.last_output \
+                or self.progress.is_done:
+            self.progress.output()
+
+        return data
+
+    def __next__(self):
+        try:
+            return self.next_task()
+        except StopIteration:
+            if not self.progress.is_done:
+                self.progress.done_tasks = 1
+                self.progress.output()
+
+            self.reset()
+            raise StopIteration()
+
+    def __iter__(self):
+        self.reset()
+        return self
+
+    def __repr__(self):
+        return f'{self.__class__.__name__}{{id={id(self)}, from={self.start_date}, to={self.end_date}}}'
+
+
+MDS = MarketDataService()
```

### Comparing `PyAlgoEngine-0.3.5/AlgoEngine/Engine/TradeEngine.py` & `PyAlgoEngine-0.3.6/AlgoEngine/Engine/TradeEngine.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,2222 +1,2222 @@
-from __future__ import annotations
-
-import abc
-import datetime
-import json
-import os
-import pathlib
-import queue
-import threading
-import time
-import uuid
-from collections import defaultdict
-from enum import Enum
-
-import numpy as np
-import pandas as pd
-from PyQuantKit import TransactionSide, TradeInstruction, OrderType, MarketData, BarData, TradeData, TickData, OrderState, OrderBook, TradeReport
-
-from . import LOGGER
-from .AlgoEngine import ALGO_ENGINE, AlgoTemplate
-from .EventEngine import TOPIC, EVENT_ENGINE
-from .MarketEngine import MarketDataService
-
-LOGGER = LOGGER.getChild('TradeEngine')
-__all__ = ['DirectMarketAccess', 'PositionManagementService', 'Balance', 'Inventory', 'RiskProfile', 'SimMatch']
-
-
-class NameSpace(dict):
-    def __init__(self, name: str = None, **kwargs):
-        self.name = name
-        super().__init__(**kwargs)
-
-    def __getattr__(self, entry):
-        if entry in self:
-            return self[entry]
-
-        raise KeyError(f'Entry {entry} not exist!')
-
-    def __repr__(self):
-        if self.name:
-            repr_str = f'<{self.name}>'
-        else:
-            repr_str = f'<NameSpace>'
-
-        repr_str += f'({super().__repr__()})'
-        return repr_str
-
-    def unpack(self):
-        return list(self.values())
-
-
-class DirectMarketAccess(object, metaclass=abc.ABCMeta):
-    """
-    Direct Market Access
-
-    send launch/cancel order direct to market(exchange)
-
-    also contains an order buff designed to process order and control risk
-
-    2 ways to implement this api
-    - override the abstractmethod _launch_order_handler, _cancel_order_handler, _reject_order_handler to api directly
-    - or use event engine
-    """
-
-    def __init__(self, mds: MarketDataService, risk_profile: RiskProfile, cool_down: float = None):
-        self.mds = mds
-        self.risk_profile = risk_profile
-        self.cool_down = cool_down
-
-        self.order_queue = queue.Queue()
-        self.worker = threading.Thread(target=self._run)
-        self._is_done = False
-
-    def __repr__(self):
-        return f'<OrderHandler>(cd={self.cool_down}, id={id(self)})'
-
-    @abc.abstractmethod
-    def _launch_order_handler(self, order: TradeInstruction, **kwargs):
-        ...
-
-    @abc.abstractmethod
-    def _cancel_order_handler(self, order: TradeInstruction, **kwargs):
-        ...
-
-    @abc.abstractmethod
-    def _reject_order_handler(self, order: TradeInstruction, **kwargs):
-        ...
-
-    def trade_time_between(self, start_time: datetime.datetime | float, end_time: datetime.datetime | float, **kwargs) -> datetime.timedelta:
-        return self.mds.trade_time_between(start_time, end_time, **kwargs)
-
-    def _launch_order_buffed(self, order: TradeInstruction, **kwargs):
-        self.order_queue.put(('launch', order, kwargs))
-
-    def _cancel_order_buffed(self, order: TradeInstruction, **kwargs):
-        self.order_queue.put(('cancel', order, kwargs))
-
-    def _launch_order_no_wait(self, order: TradeInstruction, **kwargs):
-        LOGGER.info(f'{self} sent a LAUNCH signal of {order}')
-        is_pass = self.risk_profile.check(order=order)
-
-        if not is_pass:
-            LOGGER.warning(f'{order} Rejected by risk control! Invalid action {order.ticker} {order.side.name} {order.volume}!')
-            order.set_order_state(order_state=OrderState.Rejected)
-            self._reject_order_handler(order=order, **kwargs)
-            return
-
-        order.set_order_state(order_state=OrderState.Sent)
-        self._launch_order_handler(order=order, **kwargs)
-
-    def _cancel_order_no_wait(self, order: TradeInstruction, **kwargs):
-        LOGGER.info(f'{self} sent a CANCEL signal of {order}')
-
-        order.set_order_state(order_state=OrderState.Canceling)
-        self._cancel_order_handler(order=order, **kwargs)
-
-    def launch_order(self, order: TradeInstruction, **kwargs):
-        LOGGER.info(f'{self} launching order {order}')
-        if self.cool_down:
-            self._launch_order_buffed(order=order, **kwargs)
-        else:
-            self._launch_order_no_wait(order=order, **kwargs)
-
-    def cancel_order(self, order: TradeInstruction, **kwargs):
-        LOGGER.info(f'{self} canceling order {order}')
-        if self.cool_down:
-            self._cancel_order_buffed(order=order, **kwargs)
-        else:
-            self._cancel_order_no_wait(order=order, **kwargs)
-
-    def _process_order(self):
-        try:
-            flag, order, kwargs = self.order_queue.get(block=False)
-
-            if flag == 'launch':
-                self._launch_order_no_wait(order=order, **kwargs)
-            elif flag == 'cancel':
-                self._cancel_order_no_wait(order=order, **kwargs)
-            else:
-                LOGGER.info(f'Invalid order type {flag}')
-        except queue.Empty:
-            pass
-
-    def _run(self):
-        while True:
-            self._process_order()
-
-            time.sleep(self.cool_down)
-
-            if self._is_done:
-                break
-        LOGGER.info('DMA successfully shutdown!')
-
-    def run(self):
-        self.worker.run()
-
-    @property
-    def is_done(self):
-        return self._is_done
-
-    def shut_down(self):
-        self._is_done = True
-        LOGGER.info(f'Order buff shutting down!')
-
-    @property
-    def market_price(self):
-        return self.mds.market_price
-
-    @property
-    def market_time(self):
-        return self.mds.market_time
-
-
-class PositionManagementService(object):
-    """
-    Position Module controls the position of a single strategy,
-
-    The tracker provides basic tracing of PnL, exposure, holding time and interface with risk monitor module
-    The Strategy should interface with Position module, not the algo
-
-    a range of easy method is provided to facilitate development
-    """
-
-    def __init__(
-            self,
-            dma: DirectMarketAccess,
-            algo_engine=None,
-            default_algo: str = None,
-            **kwargs
-    ):
-        self.dma = dma
-        self.algo_engine = algo_engine if algo_engine is not None else ALGO_ENGINE
-        self.algo_registry = self.algo_engine.registry
-        self.default_algo = self.algo_registry.passive if default_algo is None else default_algo
-        self.position_id = kwargs.pop('position_id', uuid.uuid4().hex)
-        self.logger = kwargs.pop('logger', LOGGER)
-
-        self.algos: dict[str, AlgoTemplate] = {}
-        self.working_algos: dict[str, AlgoTemplate] = {}
-
-    def __call__(self, market_data: MarketData):
-        self.on_market_data(market_data=market_data)
-
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
-
-            self.logger.debug(f'{algo} opening {ticker} {trade_side.side_name} {target_volume} position!')
-            self.algos[algo.algo_id] = self.working_algos[algo.algo_id] = algo
-
-            algo.launch(**kwargs)
-            self._update_status()
-            return algo
-
-    def on_filled(self, report: TradeReport, **kwargs):
-        order_id = report.order_id
-        algo = self.reversed_order_mapping.get(order_id)
-
-        if algo is None:
-            return 0
-
-        result = algo.on_filled(report=report, **kwargs)
-        self._update_status()
-        return result
-
-    def on_canceled(self, order_id: str, **kwargs):
-        algo = self.reversed_order_mapping.get(order_id)
-
-        if algo is None:
-            return 0
-
-        result = algo.on_canceled(order_id=order_id, **kwargs)
-        self._update_status()
-        return result
-
-    def on_rejected(self, order: TradeInstruction, **kwargs):
-        order_id = order.order_id
-        algo = self.reversed_order_mapping.get(order_id)
-
-        if algo is None:
-            return 0
-
-        result = algo.on_rejected(order=order, **kwargs)
-        self._update_status()
-        return result
-
-    def unwind_all(self, **kwargs):
-        exposure = self.exposure_volume
-        additional_kwargs = kwargs.copy()
-
-        for ticker in exposure:
-            self.unwind_ticker(ticker, **additional_kwargs)
-
-        return 0.
-
-    def unwind_ticker(self, ticker: str, **kwargs):
-        LOGGER.info(f'fully cancel and unwind {ticker} position!')
-
-        # cancel all
-        for algo_id in list(self.algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is not None and ticker == algo.ticker and algo.working_order:
-                algo.is_active = False
-                algo.cancel(**kwargs)
-
-        # calculate exposure
-        exposure = self.exposure_volume.get(ticker)
-        working = self.working_volume.get(ticker, {})
-        working_long = working.get('Long', 0)
-        working_short = working.get('Short', 0)
-
-        if not exposure:
-            self.logger.info(f'No exposure for {ticker}, no unwind actions!')
-            # no exposure, good!
-            return
-        elif working_long and working_short:
-            # with exposure, and working orders on both side, no action
-            self.logger.info(f'Multiple trade actions for {ticker}, skip unwind actions! Try again later!')
-            return
-        elif (exposure > 0 and working_short) or (exposure < 0 and working_long):
-            # with exposure, and working unwinding orders, no action
-            self.logger.info(f'Unwinding actions exists for {ticker}, skip unwind actions! Try again later!')
-            return
-
-        to_unwind = abs(exposure)
-        side = TransactionSide.Sell_to_Unwind if exposure > 0 else TransactionSide.Buy_to_Cover
-        self.open(ticker=ticker, target_volume=to_unwind, trade_side=side)
-
-    def cancel_all(self, **kwargs):
-        # EMERGENCY ONLY
-        for algo_id in list(self.working_algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is not None:
-                algo.cancel(**kwargs)
-
-        return 0
-
-    def on_market_data(self, market_data: MarketData):
-        for algo_id in list(self.working_algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is None:
-                continue
-
-            algo.on_market_data(market_data=market_data)
-
-    def to_json(self, fmt='str') -> str | dict:
-        json_dict = {}
-        map_id = self.position_id
-
-        json_dict[map_id] = {}
-
-        # dump algos
-        for algo_id in list(self.algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is not None:
-                json_dict[map_id][algo_id] = algo.to_json(fmt='dict')
-
-        if fmt == 'dict':
-            return json_dict
-        else:
-            return json.dumps(json_dict)
-
-    def _update_status(self):
-        for algo_id in list(self.working_algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is None:
-                continue
-
-            if algo.status == algo.Status.closed or algo.status == algo.Status.done:
-                self.algo_done(algo=algo)
-            elif algo.status == algo.Status.rejected or algo.status == algo.Status.error:
-                self.algo_error(algo=algo)
-
-    def _algo_pnl(self, algo: AlgoTemplate):
-        if algo.exposure_volume:
-            if (market_price := self.market_price.get(algo.ticker)) is not None:
-                pnl = market_price * algo.exposure_volume * algo.multiplier + algo.cash_flow
-            else:
-                pnl = np.nan
-        else:
-            pnl = algo.cash_flow
-        return pnl
-
-    def algo_done(self, algo: AlgoTemplate):
-        self.working_algos.pop(algo.algo_id, None)
-
-    def algo_error(self, algo: AlgoTemplate):
-        self.working_algos.pop(algo.algo_id, None)
-        self.logger.warning(f'{algo} encounter error, manual intervention')
-
-    def clear(self):
-        self.algos.clear()
-        self.working_algos.clear()
-
-    def pnl(self) -> dict[str, float]:
-        pnl = {}
-        for algo_id in list(self.algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is None:
-                continue
-
-            ticker = algo.ticker
-            pnl[ticker] = self._algo_pnl(algo=algo) + pnl.get(ticker, 0)
-
-        return pnl
-
-    @property
-    def notional(self) -> dict[str, float]:
-        notional = {}
-        for algo_id in list(self.algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is None:
-                continue
-
-            ticker = algo.ticker
-            notional[ticker] = algo.filled_notional + notional.get(ticker, 0)
-
-        return notional
-
-    @property
-    def working_volume(self) -> dict[str, dict[str, float]]:
-        """
-        a dictionary indicating current working volume of all orders
-
-        {'Long': +float, 'Short': +float}
-
-        :return: a dict with non-negative numbers
-        """
-        working_long = {}
-        working_short = {}
-        working = {'Long': working_long, 'Short': working_short}
-
-        for algo_id in list(self.working_algos):
-            algo = self.algos.get(algo_id)
-            ticker = algo.ticker
-
-            if algo is not None:
-                if algo.side.sign > 0:
-                    working_long[ticker] = working_long.get(ticker, 0.) + algo.working_volume
-                elif algo.side.sign < 0:
-                    working_short[ticker] = working_short.get(ticker, 0.) + algo.working_volume
-
-        for side in working:
-            _ = working[side]
-
-            for ticker in list(_):
-                if not _[ticker]:
-                    _.pop(ticker)
-
-        return working
-
-    @property
-    def exposure_volume(self) -> dict[str, float]:
-        """
-        a dictionary indicating current net exposed volume of all orders
-
-        :return: a dict with float numbers (positive and negatives)
-        """
-        exposure = {}
-
-        for algo_id in list(self.algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is not None:
-                ticker = algo.ticker
-                exposure[ticker] = exposure.get(ticker, 0.) + algo.exposure_volume
-
-        for ticker in list(exposure):
-            if not exposure[ticker]:
-                exposure.pop(ticker)
-
-        return exposure
-
-    @property
-    def working_volume_net(self) -> dict[str, float]:
-        """
-        a dictionary indicating current working volume of all orders
-
-        :return: a dict with summed working volume for each ticker numbers, with positive value as net-long and negative value as net-short
-        """
-        working = {}
-
-        for algo_id in list(self.algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is not None:
-                ticker = algo.ticker
-                working[ticker] = working.get(ticker, 0.) + algo.working_volume * algo.side.sign
-
-        for ticker in list(working):
-            if not working[ticker]:
-                working.pop(ticker)
-
-        return working
-
-    @property
-    def market_price(self):
-        return self.dma.market_price
-
-    @property
-    def market_time(self):
-        return self.dma.market_time
-
-    @property
-    def orders(self) -> dict[str, TradeInstruction]:
-        orders = {}
-
-        for algo_id in list(self.algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is None:
-                continue
-
-            orders.update(algo.order)
-
-        return orders
-
-    @property
-    def working_order(self) -> dict[str, TradeInstruction]:
-        working_order = {}
-
-        for algo_id in list(self.algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is None:
-                continue
-
-            working_order.update(algo.working_order)
-
-        return working_order
-
-    @property
-    def trades(self) -> dict[str, TradeReport]:
-        trades = {}
-
-        for algo_id in list(self.algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is None:
-                continue
-
-            trades.update(algo.trades)
-
-        return trades
-
-    @property
-    def order_mapping(self) -> dict[str, dict[str, TradeInstruction]]:
-        order_mapping = {}
-
-        for algo_id in list(self.algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is None:
-                continue
-
-            order_mapping[algo.algo_id] = algo.order
-
-        return order_mapping
-
-    @property
-    def reversed_order_mapping(self) -> dict[str, AlgoTemplate]:
-        reversed_order_mapping = {}
-
-        for algo_id in list(self.algos):
-            algo = self.algos.get(algo_id)
-
-            if algo is None:
-                continue
-
-            for order_id in algo.order:
-                reversed_order_mapping[order_id] = algo
-
-        return reversed_order_mapping
-
-
-class Balance(object):
-    """
-    Balance handles mapping of PositionTracker <-> Strategy
-    """
-
-    def __init__(self, inventory: Inventory = None):
-        self.inventory = inventory if inventory is not None else Inventory()
-
-        self.strategy = {}
-        self.trade_logs: list[TradeReport] = []
-        self.position_tracker: dict[str, PositionManagementService] = {}
-
-        self.last_update_timestamp = None
-
-    def __repr__(self):
-        return f'<Balance>{{id={id(self)}}}'
-
-    def add(self, map_id: str = None, strategy=None, position_tracker: PositionManagementService = None):
-        if map_id is None:
-            map_id = uuid.uuid4().hex
-
-        if strategy is not None:
-            self.strategy[map_id] = strategy
-        elif position_tracker is not None:
-            self.position_tracker[map_id] = position_tracker
-        else:
-            raise ValueError('Must assign ether strategy or position_tracker')
-
-    def pop(self, map_id: str):
-        self.strategy.pop(map_id, None)
-        self.position_tracker.pop(map_id, None)
-
-    def get(self, **kwargs) -> PositionManagementService | None:
-        map_id = kwargs.pop('map_id', None)
-        strategy = kwargs.pop('strategy', None)
-
-        if map_id is not None:
-            return self.position_tracker.get(map_id)
-        elif strategy is not None:
-            map_id = self.reversed_strategy_mapping.get(id(strategy))
-
-            if map_id is None:
-                raise KeyError(f'Can not found strategy {strategy}')
-            return self.position_tracker.get(map_id)
-        else:
-            raise TypeError('Must assign one value of map_id, strategy or position_tracker')
-
-    def get_strategy(self, strategy_name: str = None, strategy_id=None):
-        match = None
-
-        if strategy_name is not None:
-            for _ in self.strategy.values():
-                if _.name == strategy_name:
-                    match = _
-                    break
-        elif strategy_id is not None:
-            for _ in self.strategy.values():
-                if _.strategy_id == strategy_id:
-                    match = _
-                    break
-        else:
-            LOGGER.error(ValueError('Must assign ether a strategy_name or a strategy_id'))
-
-        return match
-
-    def get_tracker(self, strategy_name: str = None, strategy_id=None) -> PositionManagementService | None:
-        strategy = self.get_strategy(strategy_name=strategy_name, strategy_id=strategy_id)
-
-        if strategy is None:
-            return None
-
-        map_id = self.reversed_strategy_mapping.get(id(strategy))
-        tracker = self.position_tracker.get(map_id)
-        return tracker
-
-    def on_update(self, market_time=None):
-        pass
-        # step 0: update market time
-        # self.last_update_timestamp = time.time() if market_time is None else market_time
-
-        # step 1: write balance file
-        # self.dump(file_path=pathlib.Path(WORKING_DIRECTORY).joinpath('Dumps', 'balance.updated.json'))
-
-        # step 2: write trade file
-        # self.dump_trades(file_path=pathlib.Path(WORKING_DIRECTORY).joinpath('Dumps', 'trades.updated.csv'))
-
-    def on_order(self, order: TradeInstruction, **kwargs):
-        order_id = order.order_id
-        order_state = order.order_state
-        status_code = 0
-
-        for position_id in list(self.position_tracker):
-            position_tracker = self.position_tracker.get(position_id)
-
-            if position_tracker is None:
-                continue
-
-            if order_id in position_tracker.working_order:
-                if position_tracker.working_order[order_id] is not order:
-                    LOGGER.error(f'Order object not static! stored id {id(position_tracker.working_order[order_id])}, updated id {id(order)}')
-
-                if order_state == OrderState.Canceled:
-                    position_tracker.on_canceled(order_id=order_id, **kwargs)
-                elif order_state == OrderState.Rejected:
-                    position_tracker.on_rejected(order=order, **kwargs)
-
-                status_code = 1
-                break
-
-        if not status_code:
-            if order_state == OrderState.Filled:
-                LOGGER.debug(f'No match for filled order {order}, perhaps the Algo.on_filled called before Balance.on_order. This is not an error.')
-            else:
-                LOGGER.error(f'No match for {order.side} order {order}')
-
-        self.on_update()
-        return status_code
-
-    def on_report(self, report: TradeReport, **kwargs):
-        order_id = report.order_id
-        status_code = 0
-
-        for position_id in list(self.position_tracker):
-            position_tracker = self.position_tracker.get(position_id)
-
-            if position_tracker is None:
-                continue
-
-            if order_id in position_tracker.working_order:
-                position_tracker.on_filled(report=report, **kwargs)
-
-                status_code = 1
-                break
-
-        if not status_code:
-            LOGGER.warning(f'No match for report {report}')
-
-        self.on_update()
-        self.trade_logs.append(report)
-        return status_code
-
-    def reset(self):
-        self.position_tracker.clear()
-        self.strategy.clear()
-        self.trade_logs.clear()
-
-    def to_json(self, fmt='str') -> str | dict:
-        json_dict = {}
-
-        for map_id in self.position_tracker:
-            tracker = self.position_tracker.get(map_id)
-
-            if tracker is not None:
-                json_dict.update(tracker.to_json(fmt='dict'))
-
-        if fmt == 'dict':
-            return json_dict
-        else:
-            return json.dumps(json_dict)
-
-    def from_json(self, json_str: str | dict):
-        if isinstance(json_str, (str, bytes)):
-            json_dict = json.loads(json_str)
-        elif isinstance(json_str, dict):
-            json_dict = json_str
-        else:
-            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
-
-        for map_id in json_dict:
-            if map_id not in self.strategy:
-                LOGGER.error(f'No strategy with key {map_id} found! Must register strategy before loading balance!')
-                continue
-
-            pos_tracker = self.position_tracker[map_id]
-            algo_json = json_dict[map_id]
-
-            for algo_id in algo_json:
-                algo_dict = algo_json[algo_id]
-                algo = ALGO_ENGINE.from_json(algo_dict)
-                pos_tracker.algos[algo.algo_id] = pos_tracker.working_algos[algo.algo_id] = algo
-
-                if algo.status == algo.Status.closed or algo.status == algo.Status.done:
-                    pos_tracker.algo_done(algo=algo)
-                elif algo.status == algo.Status.rejected or algo.status == algo.Status.error:
-                    pos_tracker.algo_error(algo=algo)
-
-        return self
-
-    def dump(self, file_path: str | pathlib.Path):
-        file_path = pathlib.Path(file_path)
-        dump_dir = file_path.parent
-
-        os.makedirs(dump_dir, exist_ok=True)
-
-        with open(file_path, 'w') as f:
-            f.write(json.dumps(self.to_json(fmt='dict'), indent=4, sort_keys=True))
-
-    def dump_trades(self, file_path: pathlib.Path | str = None, ts_from: float = None, ts_to: float = None) -> dict:
-        """
-        export all trade monitored by position manager
-
-        :param file_path: Optional, the exported path, without it, the dict will not be dumped
-        :param ts_from: timestamp from
-        :param ts_to: timestamp to
-        :return: a dict containing all the trades
-        """
-        trades_dict = {}
-
-        for mapping_id in self.position_tracker:
-            tracker = self.position_tracker[mapping_id]
-            trades = tracker.trades
-
-            for trade_id in trades:
-                report = trades[trade_id]
-                trade_time = report.trade_time
-                ts = trade_time.timestamp()
-
-                if ts_from is not None and ts < ts_from:
-                    continue
-                elif ts_to is not None and ts > ts_to:
-                    continue
-
-                trades_dict[trade_id] = dict(
-                    strategy=mapping_id,
-                    ticker=report.ticker,
-                    side=report.side.side_name,
-                    volume=report.volume,
-                    price=report.price,
-                    notional=report.notional,
-                    time=report.trade_time,
-                    ts=report.timestamp,
-                )
-
-        if file_path and trades_dict:
-            trades_df = pd.DataFrame(trades_dict).T
-            trades_df.sort_values('ts')
-            trades_df.to_csv(file_path)
-
-        return trades_dict
-
-    def dump_trades_all(self, file_path: pathlib.Path | str = None, ts_from: float = None, ts_to: float = None) -> list:
-        """
-        export all the trades received by Balance module, even if there is no strategy corresponding to it.
-
-        :param file_path: Optional, the exported path, without it, the dict will not be dumped
-        :param ts_from: timestamp from
-        :param ts_to: timestamp to
-        :return: a list containing all the trades info
-        """
-        trade_logs = []
-
-        for report in self.trade_logs:  # type: TradeReport
-            trade_time = report.trade_time
-            ts = trade_time.timestamp()
-
-            if ts_from is not None and ts < ts_from:
-                continue
-            elif ts_to is not None and ts > ts_to:
-                continue
-
-            trade_logs.append(dict(
-                trade_id=report.trade_id,
-                ticker=report.ticker,
-                side=report.side.side_name,
-                volume=report.volume,
-                price=report.price,
-                notional=report.notional,
-                time=report.trade_time,
-                ts=report.timestamp,
-            ))
-
-        if file_path and trade_logs:
-            trades_df = pd.DataFrame(trade_logs)
-            trades_df.sort_values('ts')
-            trades_df.to_csv(file_path)
-
-        return trade_logs
-
-    def load(self, file_path: str | pathlib.Path):
-        if not os.path.isfile(file_path):
-            LOGGER.error(f'No such file {file_path}')
-            return
-
-        with open(file_path, 'r') as f:
-            json_str = f.read()
-
-        self.from_json(json_str)
-
-    @property
-    def tracker_mapping(self) -> dict[str, str]:
-        mapping = {}
-
-        for map_id in self.position_tracker:
-            tracker = self.position_tracker.get(map_id)
-
-            if tracker is None:
-                continue
-
-            mapping[map_id] = tracker.position_id
-
-        return mapping
-
-    @property
-    def reversed_tracker_mapping(self) -> dict[str, str]:
-        mapping = {}
-
-        for id_0, id_1 in self.tracker_mapping.items():
-            mapping[id_1] = id_0
-
-        return mapping
-
-    @property
-    def strategy_mapping(self) -> dict[str, int]:
-        mapping = {}
-
-        for map_id in self.strategy:
-            strategy = self.strategy.get(map_id)
-
-            if strategy is None:
-                continue
-
-            mapping[map_id] = id(strategy)
-
-        return mapping
-
-    @property
-    def reversed_strategy_mapping(self) -> dict[int, str]:
-        mapping = {}
-
-        for id_0, id_1 in self.strategy_mapping.items():
-            mapping[id_1] = id_0
-
-        return mapping
-
-    @property
-    def working_volume_summed(self) -> dict[str, float]:
-        working_summed = {}
-
-        for tracker_id in list(self.position_tracker):
-            tracker = self.position_tracker.get(tracker_id)
-
-            if tracker is not None:
-                for side in tracker.working_volume:
-                    working = tracker.working_volume[side]
-
-                    for ticker in working:
-                        working_summed[ticker] = working_summed.get(ticker, 0.) + abs(working.get(ticker, 0.))
-
-        for ticker in list(working_summed):
-            if not working_summed[ticker]:
-                working_summed.pop(ticker)
-
-        return working_summed
-
-    @property
-    def exposure_volume(self) -> dict[str, float]:
-        exposure = {}
-
-        for tracker_id in list(self.position_tracker):
-            tracker = self.position_tracker.get(tracker_id)
-
-            if tracker is not None:
-                for ticker in tracker.exposure_volume:
-                    exposure[ticker] = exposure.get(ticker, 0.) + tracker.exposure_volume[ticker]
-
-                    if exposure[ticker] == 0:
-                        exposure.pop(ticker)
-
-        return exposure
-
-    @property
-    def working_volume(self) -> dict[str, dict[str, float]]:
-
-        working_long = {}
-        working_short = {}
-        working = {'Long': working_long, 'Short': working_short}
-
-        for tracker_id in list(self.position_tracker):
-            tracker = self.position_tracker.get(tracker_id)
-
-            if tracker is not None:
-                tracker_working = tracker.working_volume
-
-                for ticker in (_ := tracker_working['Long']):
-                    working_long[ticker] = working_long.get(ticker, 0.) + _.get(ticker, 0.)
-
-                for ticker in (_ := tracker_working['Short']):
-                    working_short[ticker] = working_short.get(ticker, 0.) + _.get(ticker, 0.)
-
-        for side in working:
-            _ = working[side]
-
-            for ticker in list(_):
-                if not _[ticker]:
-                    _.pop(ticker)
-
-        return working
-
-    def exposure_notional(self, mds) -> dict[str, float]:
-        notional = {}
-
-        for ticker in self.exposure_volume:
-            notional[ticker] = self.exposure_volume.get(ticker, 0.) * mds.market_price.get(ticker, 0)
-
-        return notional
-
-    def working_notional(self, mds) -> dict[str, float]:
-        notional = {}
-
-        for ticker in (tracker_working := self.working_volume_summed):
-            notional[ticker] = tracker_working[ticker] * mds.market_price.get(ticker, 0)
-
-        return notional
-
-    @property
-    def orders(self) -> dict[str, TradeInstruction]:
-        orders = {}
-
-        for tracker_id in list(self.position_tracker):
-            tracker = self.position_tracker.get(tracker_id)
-
-            if tracker is None:
-                continue
-
-            orders.update(tracker.orders)
-
-        return orders
-
-    @property
-    def working_order(self) -> dict[str, TradeInstruction]:
-        working_order = {}
-
-        for tracker_id in list(self.position_tracker):
-            tracker = self.position_tracker.get(tracker_id)
-
-            if tracker is None:
-                continue
-
-            working_order.update(tracker.working_order)
-
-        return working_order
-
-    @property
-    def trades_today(self):
-        trades = {}
-        from .MarketEngine import MDS
-
-        market_date = MDS.market_date
-        if market_date is None:
-            return {}
-
-        for tracker_id in list(self.position_tracker):
-            tracker = self.position_tracker.get(tracker_id)
-
-            if tracker is None:
-                continue
-
-            for trade in tracker.trades.values():
-                if trade.trade_time.date() == market_date:
-                    trades[trade.trade_id] = trade
-
-            # trades.update(tracker.trades)
-
-        return trades
-
-    @property
-    def trades_session(self) -> dict[str, TradeReport]:
-        trades = {_.trade_id: _ for _ in self.trade_logs}
-
-        return trades
-
-    @property
-    def trades(self) -> dict[str, TradeReport]:
-        return self.trades_today
-
-    @property
-    def info(self) -> pd.DataFrame:
-        info_dict = {
-            'exposure': self.exposure_volume,
-            'working_lone': self.working_volume['Long'],
-            'working_short': self.working_volume['Short'],
-        }
-
-        return pd.DataFrame(info_dict).fillna(0)
-
-
-class Inventory(object):
-    """
-    Inventory stores the info of security lending
-    """
-
-    class SecurityType(Enum):
-        Commodity = 'Commodity'
-        CurrencySwap = 'CurrencySwap'
-        Crypto = 'Crypto'
-        IndexFuture = 'IndexFuture'
-        Stock = 'Stock'
-
-    class CashDividend(object):
-        def __init__(self, market_date: datetime.date, dividend_per_share: float):
-            self.market_date = market_date
-            self.dividend_per_share = dividend_per_share
-
-    class StockDividend(object):
-        def __init__(self, market_date: datetime.date, dividend_per_share: float):
-            self.market_date = market_date
-            self.dividend_per_share = dividend_per_share
-
-    class StockSplit(object):
-        def __init__(self, market_date: datetime.date, multiplier: float):
-            self.market_date = market_date
-            self.multiplier = multiplier
-
-    class StockConversion(object):
-        def __init__(self, market_date: datetime.date, convert_to: str, multiplier: float):
-            self.convert_to = convert_to
-            self.market_date = market_date
-            self.multiplier = multiplier
-
-    class Entry(object):
-        def __init__(self, ticker: str, volume: float, price: float, security_type: Inventory.SecurityType, direction: TransactionSide, **kwargs):
-            if volume < 0:
-                LOGGER.warning('volume of Inventory.Entry normally should be positive!')
-
-            self.ticker = ticker
-            self.volume = volume
-            self.price = price
-            self.security_type = security_type
-            self.direction = direction
-
-            self.notional = kwargs.pop('notional', volume * price)
-            self.fee = kwargs.pop('fee', 0.)
-            self.recalled = kwargs.pop('recalled', 0.)
-
-        def __repr__(self):
-            return f'<Inventory.Entry>(ticker={self.ticker}, side={self.direction.side_name}, volume={self.volume:,}, fee={self.fee:.2f})'
-
-        def __add__(self, other):
-            if isinstance(other, self.__class__):
-                return self.merge(other)
-
-            raise TypeError(f'Can only merge type {self.__class__.__name__}')
-
-        def __bool__(self):
-            return self.volume.__bool__()
-
-        def apply_cash_dividend(self, dividend: Inventory.CashDividend):
-            raise NotImplementedError()
-
-        def apply_stock_dividend(self, dividend: Inventory.StockDividend):
-            raise NotImplementedError()
-
-        def apply_conversion(self, stock_conversion: Inventory.StockConversion):
-            raise NotImplementedError()
-
-        def apply_split(self, stock_split: Inventory.StockSplit):
-            raise NotImplementedError()
-
-        def merge(self, entry: Inventory.Entry, inplace=False, **kwargs):
-            if entry.ticker != self.ticker:
-                raise ValueError(f'<ticker> not match! Expect {self.ticker}, got {entry.ticker}')
-
-            if entry.direction.sign != self.direction.sign:
-                raise ValueError(f'<direction> not match! Expect {self.direction}, got {entry.direction}')
-
-            if entry.security_type != self.security_type:
-                raise ValueError(f'<security_type> not match! Expect {self.security_type}, got {entry.security_type}')
-
-            volume = kwargs.pop('volume', self.volume + entry.volume)
-            notional = kwargs.pop('notional', self.notional + entry.notional)
-            price = kwargs.pop('price', (self.price * self.volume + entry.price * entry.volume) / (self.volume + entry.volume))
-            fee = kwargs.pop('fee', self.fee + entry.fee)
-            recalled = kwargs.pop('recalled', self.recalled + entry.recalled)
-
-            if inplace:
-                self.volume = volume
-                self.notional = notional
-                self.price = price
-                self.fee = fee
-                self.recalled = recalled
-
-                return self
-            else:
-                new_entry = self.__class__(
-                    ticker=self.ticker,
-                    volume=volume,
-                    price=price,
-                    security_type=self.security_type,
-                    direction=self.direction,
-                    notional=notional,
-                    fee=fee,
-                    recalled=recalled
-                )
-
-                return new_entry
-
-        def to_json(self, fmt='str') -> str | dict:
-            json_dict = dict(
-                ticker=self.ticker,
-                volume=self.volume,
-                price=self.price,
-                security_type=self.security_type.name,
-                direction=self.direction.side_name,
-                notional=self.notional,
-                fee=self.fee,
-                recalled=self.recalled
-            )
-
-            if fmt == 'dict':
-                return json_dict
-            else:
-                return json.dumps(json_dict)
-
-        @classmethod
-        def from_json(cls, json_str: str | dict):
-            if isinstance(json_str, (str, bytes)):
-                json_dict = json.loads(json_str)
-            elif isinstance(json_str, dict):
-                json_dict = json_str
-            else:
-                raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
-
-            entry = cls(
-                ticker=json_dict['ticker'],
-                volume=json_dict['volume'],
-                price=json_dict['price'],
-                security_type=Inventory.SecurityType[json_dict['security_type']],
-                direction=TransactionSide(json_dict['direction']),
-                notional=json_dict['notional'],
-                fee=json_dict.get('fee', 0.),
-                recalled=json_dict.get('recalled', 0.),
-            )
-
-            return entry
-
-        @property
-        def available(self):
-            return max(self.volume - self.recalled, 0.)
-
-    def __init__(self):
-        self._inv: dict[str, list[Inventory.Entry]] = {}
-        self._traded: dict[str, float] = {}
-        self._tickers = set()
-
-    def __repr__(self):
-        return f'<Inventory>{{id={id(self)}}}'
-
-    def __call__(self, ticker: str):
-        return dict(
-            Long=self.available_volume(ticker=ticker, direction=TransactionSide.LongOpen),
-            Short=self.available_volume(ticker=ticker, direction=TransactionSide.ShortOpen)
-        )
-
-    def recall(self, ticker: str, volume: float, direction: TransactionSide = TransactionSide.LongOpen):
-        key = f'{ticker}.{direction.side_name}'
-        _ = self._inv.get(key, [])
-        to_recall = volume
-
-        for entry in _[:]:
-            recalled = max(entry.volume, to_recall)
-            entry.recalled += recalled
-
-            if not entry.available:
-                _.remove(entry)
-                LOGGER.info(f'{entry} fully recalled!')
-            else:
-                LOGGER.info(f'{entry} recalled {recalled}, {entry.available} remains!')
-
-            if not to_recall:
-                break
-
-        if not _:
-            self._inv.pop(key)
-
-    def add_inv(self, entry: Entry):
-        self._tickers.add(entry.ticker)
-        key = f'{entry.ticker}.{entry.direction.side_name}'
-        _ = self._inv.get(key, [])
-
-        _.append(entry)
-
-        self._inv[key] = _
-
-    def get_inv(self, ticker: str, direction: TransactionSide = TransactionSide.LongOpen) -> Entry | None:
-        key = f'{ticker}.{direction.side_name}'
-        _ = self._inv.get(key, [])
-
-        merged_entry = None
-        for entry in _:
-            if merged_entry is None:
-                merged_entry = entry
-            else:
-                merged_entry = merged_entry + entry
-
-        return merged_entry
-
-    def use_inv(self, ticker: str, volume: float, direction: TransactionSide = TransactionSide.LongOpen):
-        key = f'{ticker}.{direction.side_name}'
-
-        self._traded[key] = self._traded.get(key, 0.) + volume
-
-    def available_volume(self, ticker: str, direction: TransactionSide = TransactionSide.LongOpen) -> float:
-        inv = self.get_inv(ticker=ticker, direction=direction)
-
-        if inv is None:
-            return 0.
-
-        used = self._traded.get(ticker, 0.)
-        return inv.available - used
-
-    def clear(self):
-        self._inv.clear()
-        self._traded.clear()
-        self._tickers.clear()
-
-    def to_json(self, fmt='str') -> str | dict:
-        json_dict = {}
-
-        for name in self._inv:
-            json_dict[name] = {
-                'used': 0.,
-                'inv': []
-            }
-            _ = self._inv[name]
-
-            for entry in _:
-                json_dict[name]['inv'].append(entry.to_json(fmt=fmt))
-
-            json_dict[name]['used'] = self._traded.get(name, 0.)
-
-        if fmt == 'dict':
-            return json_dict
-        else:
-            return json.dumps(json_dict)
-
-    def from_json(self, json_str: str | dict, with_used=False):
-        if isinstance(json_str, (str, bytes)):
-            json_dict = json.loads(json_str)
-        elif isinstance(json_str, dict):
-            json_dict = json_str
-        else:
-            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
-
-        for name in json_dict:
-            inv = json_dict[name]['inv']
-            used = json_dict[name]['used']
-
-            for entry_json in inv:
-                entry = self.Entry.from_json(entry_json)
-                self.add_inv(entry=entry)
-
-            if with_used:
-                self._traded[name] = used
-
-        return self
-
-    def dump(self, file_path: str | pathlib.Path):
-        file_path = pathlib.Path(file_path)
-        dump_dir = file_path.parent
-
-        os.makedirs(dump_dir, exist_ok=True)
-
-        with open(file_path, 'w') as f:
-            f.write(json.dumps(self.to_json(fmt='dict'), indent=4, sort_keys=True))
-
-    def to_csv(self, file_path: str | pathlib.Path):
-        inv_dict = {'inv_l': {}, 'inv_s': {}}
-
-        for ticker in self._inv:
-            if (long_inv := self.get_inv(ticker=ticker, direction=TransactionSide.LongOpen)) is not None:
-                inv_dict['inv_l'][ticker] = long_inv.volume
-
-            if (short_inv := self.get_inv(ticker=ticker, direction=TransactionSide.ShortOpen)) is not None:
-                inv_dict['inv_s'][ticker] = short_inv.volume
-
-        inv_df = pd.DataFrame(inv_dict)
-        inv_df.to_csv(file_path)
-
-    def load(self, file_path: str | pathlib.Path, with_used=False):
-        if not os.path.isfile(file_path):
-            LOGGER.error(f'No such file {file_path}')
-            return
-
-        with open(file_path, 'r') as f:
-            json_str = f.read()
-
-        self.clear()
-        self.from_json(json_str, with_used=with_used)
-
-    @property
-    def tickers(self):
-        return self._tickers
-
-    @property
-    def info(self) -> pd.DataFrame:
-        info_dict = {'inv_l': {}, 'inv_s': {}}
-
-        for ticker in self.tickers:
-            inv_l = self.get_inv(ticker, TransactionSide.LongOpen)
-            inv_s = self.get_inv(ticker, TransactionSide.ShortOpen)
-
-            if inv_l is not None:
-                info_dict['inv_l'][ticker] = inv_l.volume
-
-            if inv_s is not None:
-                info_dict['inv_s'][ticker] = inv_s.volume
-
-        return pd.DataFrame(info_dict)
-
-
-class RiskProfile(object):
-    class Risk(Exception):
-        def __init__(self, risk_type: str, code: int, msg: str, *args, **kwargs):
-            self.code = code
-            self.type = risk_type
-            self.msg = msg
-
-            super().__init__(msg, *args)
-
-            for kwarg in kwargs:
-                setattr(self, kwarg, kwargs[kwarg])
-
-    def __init__(self, mds: MarketDataService, balance: Balance, **kwargs):
-        self.mds = mds
-        self.balance = balance
-
-        self.rules = NameSpace(
-            entry=set(),
-            # --- individual constrains ---
-            max_percentile={},
-            max_trade_long={},
-            max_trade_short={},
-            max_exposure_long={},
-            max_exposure_short={},
-            max_notional_long={},
-            max_notional_short={},
-            # --- global constrains ---
-            max_ttl_notional_long=None,
-            max_ttl_notional_short=None,
-            max_net_notional_long=None,
-            max_net_notional_short=None,
-        )
-
-        self.rules.update(kwargs)
-
-    def __repr__(self):
-        return f'<RiskProfile>{{id={id(self)}}}'
-
-    def __call__(self, *order: TradeInstruction):
-        if len(order) == 1:
-            return self.check(order=order[0])
-        else:
-            return self.check_basket(*order)
-
-    def set_rule(self, key: str, value: float, ticker: str = None):
-        if key in self.rules:
-            limit_set = self.rules[key]
-            new_limit = value
-
-            # update global constrains
-            if ticker is None:
-                if not isinstance(limit_set, dict):
-                    old_limit = limit_set
-                    self.rules[key] = new_limit
-                    LOGGER.info(f'{self} limit updated: <{key}>: {old_limit} -> {new_limit}')
-                else:
-                    LOGGER.error(f'Invalid action: limit <{key}> requires a valid ticker')
-            # update individual constrains
-            else:
-                if isinstance(limit_set, dict):
-                    self.rules.entry.add(ticker)
-                    old_limit = limit_set.get(ticker, 'null')
-                    self.rules[key][ticker] = new_limit
-                    LOGGER.info(f'{self} limit updated: <{key}>({ticker}): {old_limit} -> {new_limit}')
-                else:
-                    LOGGER.error(f'Invalid action: can not set any ticker for limit <{key}>')
-        else:
-            LOGGER.error(f'Invalid action: limit <{key}> not found!')
-
-    def get(self, ticker: str) -> dict[str, float | dict[str, float]]:
-        limit = NameSpace(name=f'RiskLimit.{ticker}', market_price=self.mds.market_price.get(ticker))
-
-        limit['working'] = self._get_volume(ticker=ticker, flag='working')
-        limit['traded'] = self._get_volume(ticker=ticker, flag='traded')
-        limit['exposure'] = self._get_volume(ticker=ticker, flag='exposure')
-
-        # --- global constrains ---
-        if self.rules.max_ttl_notional_long is not None:
-            limit['max_ttl_notional_long'] = self.rules.max_ttl_notional_long
-
-        if self.rules.max_ttl_notional_short is not None:
-            limit['max_ttl_notional_short'] = self.rules.max_ttl_notional_short
-
-        if self.rules.max_net_notional_long is not None:
-            limit['max_net_notional_long'] = self.rules.max_net_notional_long
-
-        if self.rules.max_net_notional_short is not None:
-            limit['max_net_notional_short'] = self.rules.max_net_notional_short
-
-        # --- individual constrains ---
-        if ticker in self.rules.max_percentile:
-            limit['max_percentile'] = self.rules.max_percentile.get(ticker, 1.)
-
-        if ticker in self.rules.max_trade_long:
-            limit['max_trade_long'] = self.rules.max_trade_long.get(ticker, np.inf)
-
-        if ticker in self.rules.max_trade_short:
-            limit['max_trade_short'] = self.rules.max_trade_short.get(ticker, np.inf)
-
-        if ticker in self.rules.max_exposure_long:
-            limit['max_exposure_long'] = self.rules.max_exposure_long.get(ticker, np.inf)
-
-        if ticker in self.rules.max_exposure_short:
-            limit['max_exposure_short'] = self.rules.max_exposure_short.get(ticker, np.inf)
-
-        if ticker in self.rules.max_notional_long:
-            limit['max_notional_long'] = self.rules.max_notional_long.get(ticker, np.inf)
-
-        if ticker in self.rules.max_notional_short:
-            limit['max_notional_short'] = self.rules.max_notional_short.get(ticker, np.inf)
-
-        return limit
-
-    def check(self, order: TradeInstruction):
-        ticker = order.ticker
-
-        # step 0: get limits
-        limit = self.get(ticker=ticker)
-        LOGGER.info(f'{self} defines {limit}')
-
-        try:
-            # step 0: check validity
-            self._check_validity(order=order, limit=limit)
-
-            # step 1: check inventory limit
-            self._check_max_trade(order=order, limit=limit)
-
-            # step 2: check position limit
-            self._check_max_exposure(order=order, limit=limit)
-
-            # step 3: check percentile limit
-            self._check_max_percentile(order=order, limit=limit)
-
-            # step 4: check notional limit
-            self._check_max_notional(order=order, limit=limit)
-
-            # step 5: check portfolio net limit
-            self._check_net_portfolio(order=order, limit=limit)
-
-            # step 6: check portfolio total limit
-            self._check_ttl_portfolio(order=order, limit=limit)
-        except self.Risk as e:
-            LOGGER.error(f'<{e.type}.{e.code}>: {e.msg}')
-            return False
-
-        return True
-
-    def check_order(self, ticker: str, volume: float, side: TransactionSide):
-        fake_order = TradeInstruction(
-            ticker=ticker,
-            side=side,
-            volume=volume
-        )
-
-        return self.check(order=fake_order)
-
-    def check_basket(self, *order: TradeInstruction):
-        LOGGER.warning('risk control for basket order not implemented, check order individually')
-
-        for _ in order:
-            self.check(_)
-
-    def clear(self):
-        self.rules.entry.clear()
-
-        self.rules.max_percentile.clear()
-        self.rules.max_trade_long.clear()
-        self.rules.max_trade_short.clear()
-        self.rules.max_exposure_long.clear()
-        self.rules.max_exposure_short.clear()
-        self.rules.max_notional_long.clear()
-        self.rules.max_notional_short.clear()
-
-        self.rules.max_ttl_notional_long = np.inf
-        self.rules.max_ttl_notional_short = np.inf
-        self.rules.max_net_notional_long = np.inf
-        self.rules.max_net_notional_short = np.inf
-
-    def to_json(self, fmt='str') -> str | dict:
-        json_dict = dict(self.rules)
-        json_dict['entry'] = list(json_dict['entry'])
-
-        if fmt == 'dict':
-            return json_dict
-        else:
-            return json.dumps(json_dict)
-
-    def from_json(self, json_str: str | dict):
-        if isinstance(json_str, (str, bytes)):
-            json_dict = json.loads(json_str)
-        elif isinstance(json_str, dict):
-            json_dict = json_str
-        else:
-            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
-
-        self.rules.update(json_dict)
-        self.rules['entry'] = set(self.rules['entry'])
-
-        return self
-
-    def dump(self, file_path: str | pathlib.Path):
-        file_path = pathlib.Path(file_path)
-        dump_dir = file_path.parent
-
-        os.makedirs(dump_dir, exist_ok=True)
-
-        with open(file_path, 'w') as f:
-            f.write(json.dumps(self.to_json(fmt='dict'), indent=4, sort_keys=True))
-
-    def load(self, file_path: str | pathlib.Path):
-        if not os.path.isfile(file_path):
-            LOGGER.error(f'No such file {file_path}')
-            return
-
-        with open(file_path, 'r') as f:
-            json_str = f.read()
-
-        self.from_json(json_str)
-
-    def _check_validity(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
-        ticker = order.ticker
-        market_price = limit['market_price']
-
-        if market_price is None:
-            raise self.Risk(
-                risk_type='RiskProfile.Internal.Price',
-                code=100,
-                msg=f'no valid market price for ticker {ticker}'
-            )
-
-        return True
-
-    def _check_max_trade(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
-        ticker = order.ticker
-        action = abs(order.volume)
-        side = order.side
-
-        if side.sign > 0:
-            flag = 'long'
-        elif side.sign < 0:
-            flag = 'short'
-        else:
-            return
-
-        if f'max_trade_{flag}' not in limit:
-            raise self.Risk(
-                risk_type='RiskProfile.TradeLimit.Invalid',
-                code=1003,
-                msg=f'{ticker} {side.sign * action} rejected! {ticker} not trade-able!'
-            )
-
-        trade_limit = limit[f'max_trade_{flag}']
-        working = limit['working']
-        traded = limit['traded']
-        trade_count = working[flag] + traded[flag]
-
-        # for long order
-        if side.sign > 0:
-            if trade_count + action > trade_limit:
-                raise self.Risk(
-                    risk_type='RiskProfile.TradeLimit.Long',
-                    code=1001,
-                    msg=f'{ticker} {side.sign * action} rejected! lmt={trade_limit}, ttl={trade_count}, inv={trade_limit - trade_count}, action={action}'
-                )
-        elif side.sign < 0:
-            if trade_count + action > trade_limit:
-                raise self.Risk(
-                    risk_type='RiskProfile.TradeLimit.Short',
-                    code=1002,
-                    msg=f'{ticker} {side.sign * action} rejected! lmt={trade_limit}, ttl={trade_count}, inv={trade_limit - trade_count}, action={-action}'
-                )
-
-        return True
-
-    def _check_max_exposure(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
-        ticker = order.ticker
-        action = abs(order.volume)
-        side = order.side
-
-        if side.sign > 0:
-            flag = 'long'
-        elif side.sign < 0:
-            flag = 'short'
-        else:
-            return
-
-        if f'max_exposure_{flag}' not in limit:
-            return
-
-        working = limit['working']
-        exposure = limit['exposure']
-        max_exposure = limit[f'max_exposure_{flag}']
-        working = working[flag]
-
-        ttl_exposure = exposure['long'] - exposure['short']
-
-        expectation_volume_0 = ttl_exposure + working
-        expectation_volume_1 = ttl_exposure + action * side.sign
-        expectation_volume_2 = ttl_exposure + action * side.sign + working
-
-        if side.sign > 0:
-            if expectation_volume_0 <= max_exposure \
-                    and expectation_volume_1 <= max_exposure \
-                    and expectation_volume_2 <= max_exposure:
-                return True
-            else:
-                raise self.Risk(
-                    risk_type='RiskProfile.ExposureLimit.Long',
-                    code=2001,
-                    msg=f'{ticker} {side.sign * action} rejected! lmt_exp={max_exposure}, exp={ttl_exposure}, working={working}, action={action}'
-                )
-        elif side.sign < 0:
-            if expectation_volume_0 >= -max_exposure \
-                    and expectation_volume_1 >= -max_exposure \
-                    and expectation_volume_2 >= -max_exposure:
-                return True
-            else:
-                raise self.Risk(
-                    risk_type='RiskProfile.ExposureLimit.Short',
-                    code=2002,
-                    msg=f'{ticker} {side.sign * action} rejected! lmt_exp={max_exposure}, exp={ttl_exposure}, working={working}, action={-action}'
-                )
-
-    def _check_max_percentile(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
-        ticker = order.ticker
-        action = abs(order.volume)
-        side = order.side
-
-        if 'max_percentile' not in limit:
-            return
-
-        max_percentile = limit['max_percentile']
-        market_price = limit['market_price']
-        total_notional = sum([abs(_) for _ in self.balance.exposure_notional(mds=self.mds).values()])
-
-        if np.isfinite(max_percentile) and max_percentile < 1 and np.isfinite(total_notional):
-            max_notional = np.divide(total_notional, 1 - max_percentile) * max_percentile
-        else:
-            return True
-
-        max_position = np.divide(max_notional, market_price)
-
-        working = limit['working']
-        exposure = limit['exposure']
-
-        ttl_exposure = exposure['long'] - exposure['short']
-
-        if side.sign > 0:
-            working = working['long']
-        elif side.sign < 0:
-            working = working['short']
-        else:
-            return True
-
-        expectation_volume_0 = ttl_exposure + working
-        expectation_volume_1 = ttl_exposure + action * side.sign
-        expectation_volume_2 = ttl_exposure + action * side.sign + working
-
-        if abs(expectation_volume_0) <= max_position \
-                and abs(expectation_volume_1) <= max_position \
-                and abs(expectation_volume_2) <= max_position:
-            return True
-
-        if side.sign > 0:
-            raise self.Risk(
-                risk_type='RiskProfile.PercentileLimit.Long',
-                code=3001,
-                msg=f'{ticker} {side.sign * action} rejected! lmt_pct={max_percentile}, lmt_exp={max_position}, exp={ttl_exposure}, working={working}, action={action}'
-            )
-        elif side.sign < 0:
-            raise self.Risk(
-                risk_type='RiskProfile.PercentileLimit.Short',
-                code=3002,
-                msg=f'{ticker} {side.sign * action} rejected! lmt_pct={max_percentile}, lmt_exp={max_position}, exp={ttl_exposure}, working={working}, action={-action}'
-            )
-
-    def _check_max_notional(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
-        ticker = order.ticker
-        action = abs(order.volume)
-        side = order.side
-
-        if side.sign > 0:
-            flag = 'long'
-        elif side.sign < 0:
-            flag = 'short'
-        else:
-            return
-
-        if f'max_notional_{flag}' not in limit:
-            return
-
-        market_price = limit['market_price']
-        working = limit['working']
-        exposure = limit['exposure']
-        max_notional = limit[f'max_notional_{flag}']
-        working = working[flag]
-        ttl_exposure = exposure['long'] - exposure['short']
-        max_position = np.divide(max_notional, market_price)
-
-        expectation_volume_0 = ttl_exposure + working
-        expectation_volume_1 = ttl_exposure + action * side.sign
-        expectation_volume_2 = ttl_exposure + action * side.sign + working
-
-        if side.sign > 0:
-            if expectation_volume_0 <= max_position \
-                    and expectation_volume_1 <= max_position \
-                    and expectation_volume_2 <= max_position:
-                return True
-            else:
-                raise self.Risk(
-                    risk_type='RiskProfile.NotionalLimit.Long',
-                    code=4001,
-                    msg=f'{ticker} {side.sign * action} rejected! lmt_ntl={max_notional}, lmt_exp={max_position}, exp={ttl_exposure}, working={working}, action={action}'
-                )
-        elif side.sign < 0:
-            if expectation_volume_0 >= -max_position \
-                    and expectation_volume_1 >= -max_position \
-                    and expectation_volume_2 >= -max_position:
-                return True
-            else:
-                raise self.Risk(
-                    risk_type='RiskProfile.NotionalLimit.Short',
-                    code=4002,
-                    msg=f'{ticker} {side.sign * action} rejected! lmt_ntl={max_notional}, lmt_exp={max_position}, exp={ttl_exposure}, working={working}, action={-action}'
-                )
-
-    def _check_net_portfolio(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
-        ticker = order.ticker
-        action = abs(order.volume)
-        side = order.side
-
-        if side.sign > 0:
-            flag = 'long'
-        elif side.sign < 0:
-            flag = 'short'
-        else:
-            return
-
-        if f'max_net_notional_{flag}' not in limit:
-            return
-
-        max_net_notional = limit[f'max_net_notional_{flag}']
-        market_price = limit['market_price']
-        portfolio_working_notional = self.balance.working_notional(mds=self.mds)
-        portfolio_exposure_notional = self.balance.exposure_notional(mds=self.mds)
-
-        net_exposure = sum(portfolio_exposure_notional.values())
-        net_working = sum(portfolio_working_notional.values())
-
-        expectation_var_0 = net_exposure + net_working
-        expectation_var_1 = net_exposure + action * side.sign * market_price
-        expectation_var_2 = net_exposure + action * side.sign * market_price + net_working
-
-        if side.sign > 0:
-            if expectation_var_0 <= max_net_notional \
-                    and expectation_var_1 <= max_net_notional \
-                    and expectation_var_2 <= max_net_notional:
-                return True
-
-            raise self.Risk(
-                risk_type='RiskProfile.NotionalLimit.PortfolioNet.Long',
-                code=5001,
-                msg=f'{ticker} {side.sign * action} rejected! lmt_ntl={max_net_notional}, net_exp={net_exposure}, net_working={net_working}, action={action}'
-            )
-        elif side.sign < 0:
-            if -max_net_notional <= expectation_var_0 \
-                    and -max_net_notional <= expectation_var_1 \
-                    and -max_net_notional <= expectation_var_2:
-                return True
-
-            raise self.Risk(
-                risk_type='RiskProfile.NotionalLimit.PortfolioNet.Short',
-                code=5002,
-                msg=f'{ticker} {side.sign * action} rejected! lmt_ntl={max_net_notional}, net_exp={net_exposure}, net_working={net_working}, action={action}'
-            )
-
-    def _check_ttl_portfolio(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
-        ticker = order.ticker
-        action = abs(order.volume)
-        side = order.side
-
-        if side.sign > 0:
-            flag = 'long'
-        elif side.sign < 0:
-            flag = 'short'
-        else:
-            return
-
-        if f'max_ttl_notional_{flag}' not in limit:
-            return
-
-        market_price = limit['market_price']
-        max_notional = limit[f'max_ttl_notional_{flag}']
-        working_notional = {'long': 0., 'short': 0.}
-        exposure_notional = {'long': 0., 'short': 0.}
-
-        for order_id in list(self.balance.working_order):
-            order = self.balance.working_order.get(order_id, None)
-
-            if order is None:
-                continue
-
-            if order.side.sign > 0:
-                working_notional['long'] += abs(order.working_volume) * market_price
-            elif order.side.sign < 0:
-                working_notional['short'] += abs(order.working_volume) * market_price
-
-        for ticker, notional in self.balance.exposure_notional(mds=self.mds).items():
-            if notional > 0:
-                exposure_notional['long'] += abs(notional)
-            else:
-                exposure_notional['short'] += abs(notional)
-
-        ttl_exposure = exposure_notional[flag]
-        ttl_working = working_notional[flag]
-
-        expectation_var_0 = ttl_exposure + ttl_working
-        expectation_var_1 = ttl_exposure + action * market_price
-        expectation_var_2 = ttl_exposure + action * market_price + ttl_working
-
-        if expectation_var_0 <= max_notional \
-                and expectation_var_1 <= max_notional \
-                and expectation_var_2 <= max_notional:
-            return True
-
-        if side.sign > 0:
-            raise self.Risk(
-                risk_type='RiskProfile.NotionalLimit.PortfolioTotal.Long',
-                code=5003,
-                msg=f'{ticker} {side.sign * action} rejected! lmt_ntl={max_notional}, ttl_exp={ttl_exposure}, ttl_working={ttl_working}, action={action}'
-            )
-        elif side.sign < 0:
-            raise self.Risk(
-                risk_type='RiskProfile.NotionalLimit.PortfolioTotal.Short',
-                code=5004,
-                msg=f'{ticker} {side.sign * action} rejected! lmt_ntl={max_notional}, ttl_exp={ttl_exposure}, ttl_working={ttl_working}, action={action}'
-            )
-
-    def _get_volume(self, ticker: str, flag: str = 'working') -> dict[str, float]:
-        volume = {'long': 0., 'short': 0.}
-        if flag == 'working':
-            for order_id in list(self.balance.working_order):
-                order = self.balance.working_order.get(order_id, None)
-
-                if order is None or order.ticker != ticker or not order.is_working:
-                    continue
-
-                if order.side.sign > 0:
-                    volume['long'] += abs(order.working_volume)
-                elif order.side.sign < 0:
-                    volume['short'] += abs(order.working_volume)
-        elif flag == 'exposure':
-            for trade_id in list(self.balance.trades):
-                trade = self.balance.trades.get(trade_id, None)
-
-                if trade is None or trade.ticker != ticker:
-                    continue
-
-                if trade.side.sign > 0:
-                    volume['long'] += abs(trade.volume)
-                elif trade.side.sign < 0:
-                    volume['short'] += abs(trade.volume)
-        elif flag == 'traded':
-            for trade_id in list(self.balance.trades):
-                trade = self.balance.trades.get(trade_id, None)
-
-                if trade is None \
-                        or trade.ticker != ticker \
-                        or trade.trade_time.date() != self.market_time.date():  # apply to A-Stock when daily inventory is limited
-                    continue
-
-                if trade.side.sign > 0:
-                    volume['long'] += abs(trade.volume)
-                elif trade.side.sign < 0:
-                    volume['short'] += abs(trade.volume)
-        else:
-            raise ValueError(f'Invalid flag {flag}')
-
-        return volume
-
-    @property
-    def market_time(self):
-        return self.mds.market_time
-
-    @property
-    def info(self) -> pd.DataFrame:
-        info_dict = defaultdict(dict)
-
-        rules = self.rules.copy()
-
-        for ticker in rules['entry']:
-            for key in ['max_percentile', 'max_trade_long', 'max_trade_short', 'max_exposure_long', 'max_exposure_short', 'max_notional_long', 'max_notional_short']:
-                if ticker in rules[key]:
-                    info_dict[ticker][key] = rules[key][ticker]
-
-        for key in ['max_ttl_notional_long', 'max_ttl_notional_short', 'max_net_notional_long', 'max_net_notional_short']:
-            if rules[key] is not None:
-                info_dict['global'][key] = rules[key]
-
-        return pd.DataFrame(info_dict).T
-
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
+from __future__ import annotations
+
+import abc
+import datetime
+import json
+import os
+import pathlib
+import queue
+import threading
+import time
+import uuid
+from collections import defaultdict
+from enum import Enum
+
+import numpy as np
+import pandas as pd
+from PyQuantKit import TransactionSide, TradeInstruction, OrderType, MarketData, BarData, TradeData, TickData, OrderState, OrderBook, TradeReport
+
+from . import LOGGER
+from .AlgoEngine import ALGO_ENGINE, AlgoTemplate
+from .EventEngine import TOPIC, EVENT_ENGINE
+from .MarketEngine import MarketDataService
+
+LOGGER = LOGGER.getChild('TradeEngine')
+__all__ = ['DirectMarketAccess', 'PositionManagementService', 'Balance', 'Inventory', 'RiskProfile', 'SimMatch']
+
+
+class NameSpace(dict):
+    def __init__(self, name: str = None, **kwargs):
+        self.name = name
+        super().__init__(**kwargs)
+
+    def __getattr__(self, entry):
+        if entry in self:
+            return self[entry]
+
+        raise KeyError(f'Entry {entry} not exist!')
+
+    def __repr__(self):
+        if self.name:
+            repr_str = f'<{self.name}>'
+        else:
+            repr_str = f'<NameSpace>'
+
+        repr_str += f'({super().__repr__()})'
+        return repr_str
+
+    def unpack(self):
+        return list(self.values())
+
+
+class DirectMarketAccess(object, metaclass=abc.ABCMeta):
+    """
+    Direct Market Access
+
+    send launch/cancel order direct to market(exchange)
+
+    also contains an order buff designed to process order and control risk
+
+    2 ways to implement this api
+    - override the abstractmethod _launch_order_handler, _cancel_order_handler, _reject_order_handler to api directly
+    - or use event engine
+    """
+
+    def __init__(self, mds: MarketDataService, risk_profile: RiskProfile, cool_down: float = None):
+        self.mds = mds
+        self.risk_profile = risk_profile
+        self.cool_down = cool_down
+
+        self.order_queue = queue.Queue()
+        self.worker = threading.Thread(target=self._run)
+        self._is_done = False
+
+    def __repr__(self):
+        return f'<OrderHandler>(cd={self.cool_down}, id={id(self)})'
+
+    @abc.abstractmethod
+    def _launch_order_handler(self, order: TradeInstruction, **kwargs):
+        ...
+
+    @abc.abstractmethod
+    def _cancel_order_handler(self, order: TradeInstruction, **kwargs):
+        ...
+
+    @abc.abstractmethod
+    def _reject_order_handler(self, order: TradeInstruction, **kwargs):
+        ...
+
+    def trade_time_between(self, start_time: datetime.datetime | float, end_time: datetime.datetime | float, **kwargs) -> datetime.timedelta:
+        return self.mds.trade_time_between(start_time, end_time, **kwargs)
+
+    def _launch_order_buffed(self, order: TradeInstruction, **kwargs):
+        self.order_queue.put(('launch', order, kwargs))
+
+    def _cancel_order_buffed(self, order: TradeInstruction, **kwargs):
+        self.order_queue.put(('cancel', order, kwargs))
+
+    def _launch_order_no_wait(self, order: TradeInstruction, **kwargs):
+        LOGGER.info(f'{self} sent a LAUNCH signal of {order}')
+        is_pass = self.risk_profile.check(order=order)
+
+        if not is_pass:
+            LOGGER.warning(f'{order} Rejected by risk control! Invalid action {order.ticker} {order.side.name} {order.volume}!')
+            order.set_order_state(order_state=OrderState.Rejected)
+            self._reject_order_handler(order=order, **kwargs)
+            return
+
+        order.set_order_state(order_state=OrderState.Sent)
+        self._launch_order_handler(order=order, **kwargs)
+
+    def _cancel_order_no_wait(self, order: TradeInstruction, **kwargs):
+        LOGGER.info(f'{self} sent a CANCEL signal of {order}')
+
+        order.set_order_state(order_state=OrderState.Canceling)
+        self._cancel_order_handler(order=order, **kwargs)
+
+    def launch_order(self, order: TradeInstruction, **kwargs):
+        LOGGER.info(f'{self} launching order {order}')
+        if self.cool_down:
+            self._launch_order_buffed(order=order, **kwargs)
+        else:
+            self._launch_order_no_wait(order=order, **kwargs)
+
+    def cancel_order(self, order: TradeInstruction, **kwargs):
+        LOGGER.info(f'{self} canceling order {order}')
+        if self.cool_down:
+            self._cancel_order_buffed(order=order, **kwargs)
+        else:
+            self._cancel_order_no_wait(order=order, **kwargs)
+
+    def _process_order(self):
+        try:
+            flag, order, kwargs = self.order_queue.get(block=False)
+
+            if flag == 'launch':
+                self._launch_order_no_wait(order=order, **kwargs)
+            elif flag == 'cancel':
+                self._cancel_order_no_wait(order=order, **kwargs)
+            else:
+                LOGGER.info(f'Invalid order type {flag}')
+        except queue.Empty:
+            pass
+
+    def _run(self):
+        while True:
+            self._process_order()
+
+            time.sleep(self.cool_down)
+
+            if self._is_done:
+                break
+        LOGGER.info('DMA successfully shutdown!')
+
+    def run(self):
+        self.worker.run()
+
+    @property
+    def is_done(self):
+        return self._is_done
+
+    def shut_down(self):
+        self._is_done = True
+        LOGGER.info(f'Order buff shutting down!')
+
+    @property
+    def market_price(self):
+        return self.mds.market_price
+
+    @property
+    def market_time(self):
+        return self.mds.market_time
+
+
+class PositionManagementService(object):
+    """
+    Position Module controls the position of a single strategy,
+
+    The tracker provides basic tracing of PnL, exposure, holding time and interface with risk monitor module
+    The Strategy should interface with Position module, not the algo
+
+    a range of easy method is provided to facilitate development
+    """
+
+    def __init__(
+            self,
+            dma: DirectMarketAccess,
+            algo_engine=None,
+            default_algo: str = None,
+            **kwargs
+    ):
+        self.dma = dma
+        self.algo_engine = algo_engine if algo_engine is not None else ALGO_ENGINE
+        self.algo_registry = self.algo_engine.registry
+        self.default_algo = self.algo_registry.passive if default_algo is None else default_algo
+        self.position_id = kwargs.pop('position_id', uuid.uuid4().hex)
+        self.logger = kwargs.pop('logger', LOGGER)
+
+        self.algos: dict[str, AlgoTemplate] = {}
+        self.working_algos: dict[str, AlgoTemplate] = {}
+
+    def __call__(self, market_data: MarketData):
+        self.on_market_data(market_data=market_data)
+
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
+            self.logger.debug(f'{algo} opening {ticker} {trade_side.side_name} {target_volume} position!')
+            self.algos[algo.algo_id] = self.working_algos[algo.algo_id] = algo
+
+            algo.launch(**kwargs)
+            self._update_status()
+            return algo
+
+    def on_filled(self, report: TradeReport, **kwargs):
+        order_id = report.order_id
+        algo = self.reversed_order_mapping.get(order_id)
+
+        if algo is None:
+            return 0
+
+        result = algo.on_filled(report=report, **kwargs)
+        self._update_status()
+        return result
+
+    def on_canceled(self, order_id: str, **kwargs):
+        algo = self.reversed_order_mapping.get(order_id)
+
+        if algo is None:
+            return 0
+
+        result = algo.on_canceled(order_id=order_id, **kwargs)
+        self._update_status()
+        return result
+
+    def on_rejected(self, order: TradeInstruction, **kwargs):
+        order_id = order.order_id
+        algo = self.reversed_order_mapping.get(order_id)
+
+        if algo is None:
+            return 0
+
+        result = algo.on_rejected(order=order, **kwargs)
+        self._update_status()
+        return result
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
+    def unwind_ticker(self, ticker: str, **kwargs):
+        LOGGER.info(f'fully cancel and unwind {ticker} position!')
+
+        # cancel all
+        for algo_id in list(self.algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is not None and ticker == algo.ticker and algo.working_order:
+                algo.is_active = False
+                algo.cancel(**kwargs)
+
+        # calculate exposure
+        exposure = self.exposure_volume.get(ticker)
+        working = self.working_volume.get(ticker, {})
+        working_long = working.get('Long', 0)
+        working_short = working.get('Short', 0)
+
+        if not exposure:
+            self.logger.info(f'No exposure for {ticker}, no unwind actions!')
+            # no exposure, good!
+            return
+        elif working_long and working_short:
+            # with exposure, and working orders on both side, no action
+            self.logger.info(f'Multiple trade actions for {ticker}, skip unwind actions! Try again later!')
+            return
+        elif (exposure > 0 and working_short) or (exposure < 0 and working_long):
+            # with exposure, and working unwinding orders, no action
+            self.logger.info(f'Unwinding actions exists for {ticker}, skip unwind actions! Try again later!')
+            return
+
+        to_unwind = abs(exposure)
+        side = TransactionSide.Sell_to_Unwind if exposure > 0 else TransactionSide.Buy_to_Cover
+        self.open(ticker=ticker, target_volume=to_unwind, trade_side=side)
+
+    def cancel_all(self, **kwargs):
+        # EMERGENCY ONLY
+        for algo_id in list(self.working_algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is not None:
+                algo.cancel(**kwargs)
+
+        return 0
+
+    def on_market_data(self, market_data: MarketData):
+        for algo_id in list(self.working_algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is None:
+                continue
+
+            algo.on_market_data(market_data=market_data)
+
+    def to_json(self, fmt='str') -> str | dict:
+        json_dict = {}
+        map_id = self.position_id
+
+        json_dict[map_id] = {}
+
+        # dump algos
+        for algo_id in list(self.algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is not None:
+                json_dict[map_id][algo_id] = algo.to_json(fmt='dict')
+
+        if fmt == 'dict':
+            return json_dict
+        else:
+            return json.dumps(json_dict)
+
+    def _update_status(self):
+        for algo_id in list(self.working_algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is None:
+                continue
+
+            if algo.status == algo.Status.closed or algo.status == algo.Status.done:
+                self.algo_done(algo=algo)
+            elif algo.status == algo.Status.rejected or algo.status == algo.Status.error:
+                self.algo_error(algo=algo)
+
+    def _algo_pnl(self, algo: AlgoTemplate):
+        if algo.exposure_volume:
+            if (market_price := self.market_price.get(algo.ticker)) is not None:
+                pnl = market_price * algo.exposure_volume * algo.multiplier + algo.cash_flow
+            else:
+                pnl = np.nan
+        else:
+            pnl = algo.cash_flow
+        return pnl
+
+    def algo_done(self, algo: AlgoTemplate):
+        self.working_algos.pop(algo.algo_id, None)
+
+    def algo_error(self, algo: AlgoTemplate):
+        self.working_algos.pop(algo.algo_id, None)
+        self.logger.warning(f'{algo} encounter error, manual intervention')
+
+    def clear(self):
+        self.algos.clear()
+        self.working_algos.clear()
+
+    def pnl(self) -> dict[str, float]:
+        pnl = {}
+        for algo_id in list(self.algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is None:
+                continue
+
+            ticker = algo.ticker
+            pnl[ticker] = self._algo_pnl(algo=algo) + pnl.get(ticker, 0)
+
+        return pnl
+
+    @property
+    def notional(self) -> dict[str, float]:
+        notional = {}
+        for algo_id in list(self.algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is None:
+                continue
+
+            ticker = algo.ticker
+            notional[ticker] = algo.filled_notional + notional.get(ticker, 0)
+
+        return notional
+
+    @property
+    def working_volume(self) -> dict[str, dict[str, float]]:
+        """
+        a dictionary indicating current working volume of all orders
+
+        {'Long': +float, 'Short': +float}
+
+        :return: a dict with non-negative numbers
+        """
+        working_long = {}
+        working_short = {}
+        working = {'Long': working_long, 'Short': working_short}
+
+        for algo_id in list(self.working_algos):
+            algo = self.algos.get(algo_id)
+            ticker = algo.ticker
+
+            if algo is not None:
+                if algo.side.sign > 0:
+                    working_long[ticker] = working_long.get(ticker, 0.) + algo.working_volume
+                elif algo.side.sign < 0:
+                    working_short[ticker] = working_short.get(ticker, 0.) + algo.working_volume
+
+        for side in working:
+            _ = working[side]
+
+            for ticker in list(_):
+                if not _[ticker]:
+                    _.pop(ticker)
+
+        return working
+
+    @property
+    def exposure_volume(self) -> dict[str, float]:
+        """
+        a dictionary indicating current net exposed volume of all orders
+
+        :return: a dict with float numbers (positive and negatives)
+        """
+        exposure = {}
+
+        for algo_id in list(self.algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is not None:
+                ticker = algo.ticker
+                exposure[ticker] = exposure.get(ticker, 0.) + algo.exposure_volume
+
+        for ticker in list(exposure):
+            if not exposure[ticker]:
+                exposure.pop(ticker)
+
+        return exposure
+
+    @property
+    def working_volume_net(self) -> dict[str, float]:
+        """
+        a dictionary indicating current working volume of all orders
+
+        :return: a dict with summed working volume for each ticker numbers, with positive value as net-long and negative value as net-short
+        """
+        working = {}
+
+        for algo_id in list(self.algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is not None:
+                ticker = algo.ticker
+                working[ticker] = working.get(ticker, 0.) + algo.working_volume * algo.side.sign
+
+        for ticker in list(working):
+            if not working[ticker]:
+                working.pop(ticker)
+
+        return working
+
+    @property
+    def market_price(self):
+        return self.dma.market_price
+
+    @property
+    def market_time(self):
+        return self.dma.market_time
+
+    @property
+    def orders(self) -> dict[str, TradeInstruction]:
+        orders = {}
+
+        for algo_id in list(self.algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is None:
+                continue
+
+            orders.update(algo.order)
+
+        return orders
+
+    @property
+    def working_order(self) -> dict[str, TradeInstruction]:
+        working_order = {}
+
+        for algo_id in list(self.algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is None:
+                continue
+
+            working_order.update(algo.working_order)
+
+        return working_order
+
+    @property
+    def trades(self) -> dict[str, TradeReport]:
+        trades = {}
+
+        for algo_id in list(self.algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is None:
+                continue
+
+            trades.update(algo.trades)
+
+        return trades
+
+    @property
+    def order_mapping(self) -> dict[str, dict[str, TradeInstruction]]:
+        order_mapping = {}
+
+        for algo_id in list(self.algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is None:
+                continue
+
+            order_mapping[algo.algo_id] = algo.order
+
+        return order_mapping
+
+    @property
+    def reversed_order_mapping(self) -> dict[str, AlgoTemplate]:
+        reversed_order_mapping = {}
+
+        for algo_id in list(self.algos):
+            algo = self.algos.get(algo_id)
+
+            if algo is None:
+                continue
+
+            for order_id in algo.order:
+                reversed_order_mapping[order_id] = algo
+
+        return reversed_order_mapping
+
+
+class Balance(object):
+    """
+    Balance handles mapping of PositionTracker <-> Strategy
+    """
+
+    def __init__(self, inventory: Inventory = None):
+        self.inventory = inventory if inventory is not None else Inventory()
+
+        self.strategy = {}
+        self.trade_logs: list[TradeReport] = []
+        self.position_tracker: dict[str, PositionManagementService] = {}
+
+        self.last_update_timestamp = None
+
+    def __repr__(self):
+        return f'<Balance>{{id={id(self)}}}'
+
+    def add(self, map_id: str = None, strategy=None, position_tracker: PositionManagementService = None):
+        if map_id is None:
+            map_id = uuid.uuid4().hex
+
+        if strategy is not None:
+            self.strategy[map_id] = strategy
+        elif position_tracker is not None:
+            self.position_tracker[map_id] = position_tracker
+        else:
+            raise ValueError('Must assign ether strategy or position_tracker')
+
+    def pop(self, map_id: str):
+        self.strategy.pop(map_id, None)
+        self.position_tracker.pop(map_id, None)
+
+    def get(self, **kwargs) -> PositionManagementService | None:
+        map_id = kwargs.pop('map_id', None)
+        strategy = kwargs.pop('strategy', None)
+
+        if map_id is not None:
+            return self.position_tracker.get(map_id)
+        elif strategy is not None:
+            map_id = self.reversed_strategy_mapping.get(id(strategy))
+
+            if map_id is None:
+                raise KeyError(f'Can not found strategy {strategy}')
+            return self.position_tracker.get(map_id)
+        else:
+            raise TypeError('Must assign one value of map_id, strategy or position_tracker')
+
+    def get_strategy(self, strategy_name: str = None, strategy_id=None):
+        match = None
+
+        if strategy_name is not None:
+            for _ in self.strategy.values():
+                if _.name == strategy_name:
+                    match = _
+                    break
+        elif strategy_id is not None:
+            for _ in self.strategy.values():
+                if _.strategy_id == strategy_id:
+                    match = _
+                    break
+        else:
+            LOGGER.error(ValueError('Must assign ether a strategy_name or a strategy_id'))
+
+        return match
+
+    def get_tracker(self, strategy_name: str = None, strategy_id=None) -> PositionManagementService | None:
+        strategy = self.get_strategy(strategy_name=strategy_name, strategy_id=strategy_id)
+
+        if strategy is None:
+            return None
+
+        map_id = self.reversed_strategy_mapping.get(id(strategy))
+        tracker = self.position_tracker.get(map_id)
+        return tracker
+
+    def on_update(self, market_time=None):
+        pass
+        # step 0: update market time
+        # self.last_update_timestamp = time.time() if market_time is None else market_time
+
+        # step 1: write balance file
+        # self.dump(file_path=pathlib.Path(WORKING_DIRECTORY).joinpath('Dumps', 'balance.updated.json'))
+
+        # step 2: write trade file
+        # self.dump_trades(file_path=pathlib.Path(WORKING_DIRECTORY).joinpath('Dumps', 'trades.updated.csv'))
+
+    def on_order(self, order: TradeInstruction, **kwargs):
+        order_id = order.order_id
+        order_state = order.order_state
+        status_code = 0
+
+        for position_id in list(self.position_tracker):
+            position_tracker = self.position_tracker.get(position_id)
+
+            if position_tracker is None:
+                continue
+
+            if order_id in position_tracker.working_order:
+                if position_tracker.working_order[order_id] is not order:
+                    LOGGER.error(f'Order object not static! stored id {id(position_tracker.working_order[order_id])}, updated id {id(order)}')
+
+                if order_state == OrderState.Canceled:
+                    position_tracker.on_canceled(order_id=order_id, **kwargs)
+                elif order_state == OrderState.Rejected:
+                    position_tracker.on_rejected(order=order, **kwargs)
+
+                status_code = 1
+                break
+
+        if not status_code:
+            if order_state == OrderState.Filled:
+                LOGGER.debug(f'No match for filled order {order}, perhaps the Algo.on_filled called before Balance.on_order. This is not an error.')
+            else:
+                LOGGER.error(f'No match for {order.side} order {order}')
+
+        self.on_update()
+        return status_code
+
+    def on_report(self, report: TradeReport, **kwargs):
+        order_id = report.order_id
+        status_code = 0
+
+        for position_id in list(self.position_tracker):
+            position_tracker = self.position_tracker.get(position_id)
+
+            if position_tracker is None:
+                continue
+
+            if order_id in position_tracker.working_order:
+                position_tracker.on_filled(report=report, **kwargs)
+
+                status_code = 1
+                break
+
+        if not status_code:
+            LOGGER.warning(f'No match for report {report}')
+
+        self.on_update()
+        self.trade_logs.append(report)
+        return status_code
+
+    def reset(self):
+        self.position_tracker.clear()
+        self.strategy.clear()
+        self.trade_logs.clear()
+
+    def to_json(self, fmt='str') -> str | dict:
+        json_dict = {}
+
+        for map_id in self.position_tracker:
+            tracker = self.position_tracker.get(map_id)
+
+            if tracker is not None:
+                json_dict.update(tracker.to_json(fmt='dict'))
+
+        if fmt == 'dict':
+            return json_dict
+        else:
+            return json.dumps(json_dict)
+
+    def from_json(self, json_str: str | dict):
+        if isinstance(json_str, (str, bytes)):
+            json_dict = json.loads(json_str)
+        elif isinstance(json_str, dict):
+            json_dict = json_str
+        else:
+            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
+
+        for map_id in json_dict:
+            if map_id not in self.strategy:
+                LOGGER.error(f'No strategy with key {map_id} found! Must register strategy before loading balance!')
+                continue
+
+            pos_tracker = self.position_tracker[map_id]
+            algo_json = json_dict[map_id]
+
+            for algo_id in algo_json:
+                algo_dict = algo_json[algo_id]
+                algo = ALGO_ENGINE.from_json(algo_dict)
+                pos_tracker.algos[algo.algo_id] = pos_tracker.working_algos[algo.algo_id] = algo
+
+                if algo.status == algo.Status.closed or algo.status == algo.Status.done:
+                    pos_tracker.algo_done(algo=algo)
+                elif algo.status == algo.Status.rejected or algo.status == algo.Status.error:
+                    pos_tracker.algo_error(algo=algo)
+
+        return self
+
+    def dump(self, file_path: str | pathlib.Path):
+        file_path = pathlib.Path(file_path)
+        dump_dir = file_path.parent
+
+        os.makedirs(dump_dir, exist_ok=True)
+
+        with open(file_path, 'w') as f:
+            f.write(json.dumps(self.to_json(fmt='dict'), indent=4, sort_keys=True))
+
+    def dump_trades(self, file_path: pathlib.Path | str = None, ts_from: float = None, ts_to: float = None) -> dict:
+        """
+        export all trade monitored by position manager
+
+        :param file_path: Optional, the exported path, without it, the dict will not be dumped
+        :param ts_from: timestamp from
+        :param ts_to: timestamp to
+        :return: a dict containing all the trades
+        """
+        trades_dict = {}
+
+        for mapping_id in self.position_tracker:
+            tracker = self.position_tracker[mapping_id]
+            trades = tracker.trades
+
+            for trade_id in trades:
+                report = trades[trade_id]
+                trade_time = report.trade_time
+                ts = trade_time.timestamp()
+
+                if ts_from is not None and ts < ts_from:
+                    continue
+                elif ts_to is not None and ts > ts_to:
+                    continue
+
+                trades_dict[trade_id] = dict(
+                    strategy=mapping_id,
+                    ticker=report.ticker,
+                    side=report.side.side_name,
+                    volume=report.volume,
+                    price=report.price,
+                    notional=report.notional,
+                    time=report.trade_time,
+                    ts=report.timestamp,
+                )
+
+        if file_path and trades_dict:
+            trades_df = pd.DataFrame(trades_dict).T
+            trades_df.sort_values('ts')
+            trades_df.to_csv(file_path)
+
+        return trades_dict
+
+    def dump_trades_all(self, file_path: pathlib.Path | str = None, ts_from: float = None, ts_to: float = None) -> list:
+        """
+        export all the trades received by Balance module, even if there is no strategy corresponding to it.
+
+        :param file_path: Optional, the exported path, without it, the dict will not be dumped
+        :param ts_from: timestamp from
+        :param ts_to: timestamp to
+        :return: a list containing all the trades info
+        """
+        trade_logs = []
+
+        for report in self.trade_logs:  # type: TradeReport
+            trade_time = report.trade_time
+            ts = trade_time.timestamp()
+
+            if ts_from is not None and ts < ts_from:
+                continue
+            elif ts_to is not None and ts > ts_to:
+                continue
+
+            trade_logs.append(dict(
+                trade_id=report.trade_id,
+                ticker=report.ticker,
+                side=report.side.side_name,
+                volume=report.volume,
+                price=report.price,
+                notional=report.notional,
+                time=report.trade_time,
+                ts=report.timestamp,
+            ))
+
+        if file_path and trade_logs:
+            trades_df = pd.DataFrame(trade_logs)
+            trades_df.sort_values('ts')
+            trades_df.to_csv(file_path)
+
+        return trade_logs
+
+    def load(self, file_path: str | pathlib.Path):
+        if not os.path.isfile(file_path):
+            LOGGER.error(f'No such file {file_path}')
+            return
+
+        with open(file_path, 'r') as f:
+            json_str = f.read()
+
+        self.from_json(json_str)
+
+    @property
+    def tracker_mapping(self) -> dict[str, str]:
+        mapping = {}
+
+        for map_id in self.position_tracker:
+            tracker = self.position_tracker.get(map_id)
+
+            if tracker is None:
+                continue
+
+            mapping[map_id] = tracker.position_id
+
+        return mapping
+
+    @property
+    def reversed_tracker_mapping(self) -> dict[str, str]:
+        mapping = {}
+
+        for id_0, id_1 in self.tracker_mapping.items():
+            mapping[id_1] = id_0
+
+        return mapping
+
+    @property
+    def strategy_mapping(self) -> dict[str, int]:
+        mapping = {}
+
+        for map_id in self.strategy:
+            strategy = self.strategy.get(map_id)
+
+            if strategy is None:
+                continue
+
+            mapping[map_id] = id(strategy)
+
+        return mapping
+
+    @property
+    def reversed_strategy_mapping(self) -> dict[int, str]:
+        mapping = {}
+
+        for id_0, id_1 in self.strategy_mapping.items():
+            mapping[id_1] = id_0
+
+        return mapping
+
+    @property
+    def working_volume_summed(self) -> dict[str, float]:
+        working_summed = {}
+
+        for tracker_id in list(self.position_tracker):
+            tracker = self.position_tracker.get(tracker_id)
+
+            if tracker is not None:
+                for side in tracker.working_volume:
+                    working = tracker.working_volume[side]
+
+                    for ticker in working:
+                        working_summed[ticker] = working_summed.get(ticker, 0.) + abs(working.get(ticker, 0.))
+
+        for ticker in list(working_summed):
+            if not working_summed[ticker]:
+                working_summed.pop(ticker)
+
+        return working_summed
+
+    @property
+    def exposure_volume(self) -> dict[str, float]:
+        exposure = {}
+
+        for tracker_id in list(self.position_tracker):
+            tracker = self.position_tracker.get(tracker_id)
+
+            if tracker is not None:
+                for ticker in tracker.exposure_volume:
+                    exposure[ticker] = exposure.get(ticker, 0.) + tracker.exposure_volume[ticker]
+
+                    if exposure[ticker] == 0:
+                        exposure.pop(ticker)
+
+        return exposure
+
+    @property
+    def working_volume(self) -> dict[str, dict[str, float]]:
+
+        working_long = {}
+        working_short = {}
+        working = {'Long': working_long, 'Short': working_short}
+
+        for tracker_id in list(self.position_tracker):
+            tracker = self.position_tracker.get(tracker_id)
+
+            if tracker is not None:
+                tracker_working = tracker.working_volume
+
+                for ticker in (_ := tracker_working['Long']):
+                    working_long[ticker] = working_long.get(ticker, 0.) + _.get(ticker, 0.)
+
+                for ticker in (_ := tracker_working['Short']):
+                    working_short[ticker] = working_short.get(ticker, 0.) + _.get(ticker, 0.)
+
+        for side in working:
+            _ = working[side]
+
+            for ticker in list(_):
+                if not _[ticker]:
+                    _.pop(ticker)
+
+        return working
+
+    def exposure_notional(self, mds) -> dict[str, float]:
+        notional = {}
+
+        for ticker in self.exposure_volume:
+            notional[ticker] = self.exposure_volume.get(ticker, 0.) * mds.market_price.get(ticker, 0)
+
+        return notional
+
+    def working_notional(self, mds) -> dict[str, float]:
+        notional = {}
+
+        for ticker in (tracker_working := self.working_volume_summed):
+            notional[ticker] = tracker_working[ticker] * mds.market_price.get(ticker, 0)
+
+        return notional
+
+    @property
+    def orders(self) -> dict[str, TradeInstruction]:
+        orders = {}
+
+        for tracker_id in list(self.position_tracker):
+            tracker = self.position_tracker.get(tracker_id)
+
+            if tracker is None:
+                continue
+
+            orders.update(tracker.orders)
+
+        return orders
+
+    @property
+    def working_order(self) -> dict[str, TradeInstruction]:
+        working_order = {}
+
+        for tracker_id in list(self.position_tracker):
+            tracker = self.position_tracker.get(tracker_id)
+
+            if tracker is None:
+                continue
+
+            working_order.update(tracker.working_order)
+
+        return working_order
+
+    @property
+    def trades_today(self):
+        trades = {}
+        from .MarketEngine import MDS
+
+        market_date = MDS.market_date
+        if market_date is None:
+            return {}
+
+        for tracker_id in list(self.position_tracker):
+            tracker = self.position_tracker.get(tracker_id)
+
+            if tracker is None:
+                continue
+
+            for trade in tracker.trades.values():
+                if trade.trade_time.date() == market_date:
+                    trades[trade.trade_id] = trade
+
+            # trades.update(tracker.trades)
+
+        return trades
+
+    @property
+    def trades_session(self) -> dict[str, TradeReport]:
+        trades = {_.trade_id: _ for _ in self.trade_logs}
+
+        return trades
+
+    @property
+    def trades(self) -> dict[str, TradeReport]:
+        return self.trades_today
+
+    @property
+    def info(self) -> pd.DataFrame:
+        info_dict = {
+            'exposure': self.exposure_volume,
+            'working_lone': self.working_volume['Long'],
+            'working_short': self.working_volume['Short'],
+        }
+
+        return pd.DataFrame(info_dict).fillna(0)
+
+
+class Inventory(object):
+    """
+    Inventory stores the info of security lending
+    """
+
+    class SecurityType(Enum):
+        Commodity = 'Commodity'
+        CurrencySwap = 'CurrencySwap'
+        Crypto = 'Crypto'
+        IndexFuture = 'IndexFuture'
+        Stock = 'Stock'
+
+    class CashDividend(object):
+        def __init__(self, market_date: datetime.date, dividend_per_share: float):
+            self.market_date = market_date
+            self.dividend_per_share = dividend_per_share
+
+    class StockDividend(object):
+        def __init__(self, market_date: datetime.date, dividend_per_share: float):
+            self.market_date = market_date
+            self.dividend_per_share = dividend_per_share
+
+    class StockSplit(object):
+        def __init__(self, market_date: datetime.date, multiplier: float):
+            self.market_date = market_date
+            self.multiplier = multiplier
+
+    class StockConversion(object):
+        def __init__(self, market_date: datetime.date, convert_to: str, multiplier: float):
+            self.convert_to = convert_to
+            self.market_date = market_date
+            self.multiplier = multiplier
+
+    class Entry(object):
+        def __init__(self, ticker: str, volume: float, price: float, security_type: Inventory.SecurityType, direction: TransactionSide, **kwargs):
+            if volume < 0:
+                LOGGER.warning('volume of Inventory.Entry normally should be positive!')
+
+            self.ticker = ticker
+            self.volume = volume
+            self.price = price
+            self.security_type = security_type
+            self.direction = direction
+
+            self.notional = kwargs.pop('notional', volume * price)
+            self.fee = kwargs.pop('fee', 0.)
+            self.recalled = kwargs.pop('recalled', 0.)
+
+        def __repr__(self):
+            return f'<Inventory.Entry>(ticker={self.ticker}, side={self.direction.side_name}, volume={self.volume:,}, fee={self.fee:.2f})'
+
+        def __add__(self, other):
+            if isinstance(other, self.__class__):
+                return self.merge(other)
+
+            raise TypeError(f'Can only merge type {self.__class__.__name__}')
+
+        def __bool__(self):
+            return self.volume.__bool__()
+
+        def apply_cash_dividend(self, dividend: Inventory.CashDividend):
+            raise NotImplementedError()
+
+        def apply_stock_dividend(self, dividend: Inventory.StockDividend):
+            raise NotImplementedError()
+
+        def apply_conversion(self, stock_conversion: Inventory.StockConversion):
+            raise NotImplementedError()
+
+        def apply_split(self, stock_split: Inventory.StockSplit):
+            raise NotImplementedError()
+
+        def merge(self, entry: Inventory.Entry, inplace=False, **kwargs):
+            if entry.ticker != self.ticker:
+                raise ValueError(f'<ticker> not match! Expect {self.ticker}, got {entry.ticker}')
+
+            if entry.direction.sign != self.direction.sign:
+                raise ValueError(f'<direction> not match! Expect {self.direction}, got {entry.direction}')
+
+            if entry.security_type != self.security_type:
+                raise ValueError(f'<security_type> not match! Expect {self.security_type}, got {entry.security_type}')
+
+            volume = kwargs.pop('volume', self.volume + entry.volume)
+            notional = kwargs.pop('notional', self.notional + entry.notional)
+            price = kwargs.pop('price', (self.price * self.volume + entry.price * entry.volume) / (self.volume + entry.volume))
+            fee = kwargs.pop('fee', self.fee + entry.fee)
+            recalled = kwargs.pop('recalled', self.recalled + entry.recalled)
+
+            if inplace:
+                self.volume = volume
+                self.notional = notional
+                self.price = price
+                self.fee = fee
+                self.recalled = recalled
+
+                return self
+            else:
+                new_entry = self.__class__(
+                    ticker=self.ticker,
+                    volume=volume,
+                    price=price,
+                    security_type=self.security_type,
+                    direction=self.direction,
+                    notional=notional,
+                    fee=fee,
+                    recalled=recalled
+                )
+
+                return new_entry
+
+        def to_json(self, fmt='str') -> str | dict:
+            json_dict = dict(
+                ticker=self.ticker,
+                volume=self.volume,
+                price=self.price,
+                security_type=self.security_type.name,
+                direction=self.direction.side_name,
+                notional=self.notional,
+                fee=self.fee,
+                recalled=self.recalled
+            )
+
+            if fmt == 'dict':
+                return json_dict
+            else:
+                return json.dumps(json_dict)
+
+        @classmethod
+        def from_json(cls, json_str: str | dict):
+            if isinstance(json_str, (str, bytes)):
+                json_dict = json.loads(json_str)
+            elif isinstance(json_str, dict):
+                json_dict = json_str
+            else:
+                raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
+
+            entry = cls(
+                ticker=json_dict['ticker'],
+                volume=json_dict['volume'],
+                price=json_dict['price'],
+                security_type=Inventory.SecurityType[json_dict['security_type']],
+                direction=TransactionSide(json_dict['direction']),
+                notional=json_dict['notional'],
+                fee=json_dict.get('fee', 0.),
+                recalled=json_dict.get('recalled', 0.),
+            )
+
+            return entry
+
+        @property
+        def available(self):
+            return max(self.volume - self.recalled, 0.)
+
+    def __init__(self):
+        self._inv: dict[str, list[Inventory.Entry]] = {}
+        self._traded: dict[str, float] = {}
+        self._tickers = set()
+
+    def __repr__(self):
+        return f'<Inventory>{{id={id(self)}}}'
+
+    def __call__(self, ticker: str):
+        return dict(
+            Long=self.available_volume(ticker=ticker, direction=TransactionSide.LongOpen),
+            Short=self.available_volume(ticker=ticker, direction=TransactionSide.ShortOpen)
+        )
+
+    def recall(self, ticker: str, volume: float, direction: TransactionSide = TransactionSide.LongOpen):
+        key = f'{ticker}.{direction.side_name}'
+        _ = self._inv.get(key, [])
+        to_recall = volume
+
+        for entry in _[:]:
+            recalled = max(entry.volume, to_recall)
+            entry.recalled += recalled
+
+            if not entry.available:
+                _.remove(entry)
+                LOGGER.info(f'{entry} fully recalled!')
+            else:
+                LOGGER.info(f'{entry} recalled {recalled}, {entry.available} remains!')
+
+            if not to_recall:
+                break
+
+        if not _:
+            self._inv.pop(key)
+
+    def add_inv(self, entry: Entry):
+        self._tickers.add(entry.ticker)
+        key = f'{entry.ticker}.{entry.direction.side_name}'
+        _ = self._inv.get(key, [])
+
+        _.append(entry)
+
+        self._inv[key] = _
+
+    def get_inv(self, ticker: str, direction: TransactionSide = TransactionSide.LongOpen) -> Entry | None:
+        key = f'{ticker}.{direction.side_name}'
+        _ = self._inv.get(key, [])
+
+        merged_entry = None
+        for entry in _:
+            if merged_entry is None:
+                merged_entry = entry
+            else:
+                merged_entry = merged_entry + entry
+
+        return merged_entry
+
+    def use_inv(self, ticker: str, volume: float, direction: TransactionSide = TransactionSide.LongOpen):
+        key = f'{ticker}.{direction.side_name}'
+
+        self._traded[key] = self._traded.get(key, 0.) + volume
+
+    def available_volume(self, ticker: str, direction: TransactionSide = TransactionSide.LongOpen) -> float:
+        inv = self.get_inv(ticker=ticker, direction=direction)
+
+        if inv is None:
+            return 0.
+
+        used = self._traded.get(ticker, 0.)
+        return inv.available - used
+
+    def clear(self):
+        self._inv.clear()
+        self._traded.clear()
+        self._tickers.clear()
+
+    def to_json(self, fmt='str') -> str | dict:
+        json_dict = {}
+
+        for name in self._inv:
+            json_dict[name] = {
+                'used': 0.,
+                'inv': []
+            }
+            _ = self._inv[name]
+
+            for entry in _:
+                json_dict[name]['inv'].append(entry.to_json(fmt=fmt))
+
+            json_dict[name]['used'] = self._traded.get(name, 0.)
+
+        if fmt == 'dict':
+            return json_dict
+        else:
+            return json.dumps(json_dict)
+
+    def from_json(self, json_str: str | dict, with_used=False):
+        if isinstance(json_str, (str, bytes)):
+            json_dict = json.loads(json_str)
+        elif isinstance(json_str, dict):
+            json_dict = json_str
+        else:
+            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
+
+        for name in json_dict:
+            inv = json_dict[name]['inv']
+            used = json_dict[name]['used']
+
+            for entry_json in inv:
+                entry = self.Entry.from_json(entry_json)
+                self.add_inv(entry=entry)
+
+            if with_used:
+                self._traded[name] = used
+
+        return self
+
+    def dump(self, file_path: str | pathlib.Path):
+        file_path = pathlib.Path(file_path)
+        dump_dir = file_path.parent
+
+        os.makedirs(dump_dir, exist_ok=True)
+
+        with open(file_path, 'w') as f:
+            f.write(json.dumps(self.to_json(fmt='dict'), indent=4, sort_keys=True))
+
+    def to_csv(self, file_path: str | pathlib.Path):
+        inv_dict = {'inv_l': {}, 'inv_s': {}}
+
+        for ticker in self._inv:
+            if (long_inv := self.get_inv(ticker=ticker, direction=TransactionSide.LongOpen)) is not None:
+                inv_dict['inv_l'][ticker] = long_inv.volume
+
+            if (short_inv := self.get_inv(ticker=ticker, direction=TransactionSide.ShortOpen)) is not None:
+                inv_dict['inv_s'][ticker] = short_inv.volume
+
+        inv_df = pd.DataFrame(inv_dict)
+        inv_df.to_csv(file_path)
+
+    def load(self, file_path: str | pathlib.Path, with_used=False):
+        if not os.path.isfile(file_path):
+            LOGGER.error(f'No such file {file_path}')
+            return
+
+        with open(file_path, 'r') as f:
+            json_str = f.read()
+
+        self.clear()
+        self.from_json(json_str, with_used=with_used)
+
+    @property
+    def tickers(self):
+        return self._tickers
+
+    @property
+    def info(self) -> pd.DataFrame:
+        info_dict = {'inv_l': {}, 'inv_s': {}}
+
+        for ticker in self.tickers:
+            inv_l = self.get_inv(ticker, TransactionSide.LongOpen)
+            inv_s = self.get_inv(ticker, TransactionSide.ShortOpen)
+
+            if inv_l is not None:
+                info_dict['inv_l'][ticker] = inv_l.volume
+
+            if inv_s is not None:
+                info_dict['inv_s'][ticker] = inv_s.volume
+
+        return pd.DataFrame(info_dict)
+
+
+class RiskProfile(object):
+    class Risk(Exception):
+        def __init__(self, risk_type: str, code: int, msg: str, *args, **kwargs):
+            self.code = code
+            self.type = risk_type
+            self.msg = msg
+
+            super().__init__(msg, *args)
+
+            for kwarg in kwargs:
+                setattr(self, kwarg, kwargs[kwarg])
+
+    def __init__(self, mds: MarketDataService, balance: Balance, **kwargs):
+        self.mds = mds
+        self.balance = balance
+
+        self.rules = NameSpace(
+            entry=set(),
+            # --- individual constrains ---
+            max_percentile={},
+            max_trade_long={},
+            max_trade_short={},
+            max_exposure_long={},
+            max_exposure_short={},
+            max_notional_long={},
+            max_notional_short={},
+            # --- global constrains ---
+            max_ttl_notional_long=None,
+            max_ttl_notional_short=None,
+            max_net_notional_long=None,
+            max_net_notional_short=None,
+        )
+
+        self.rules.update(kwargs)
+
+    def __repr__(self):
+        return f'<RiskProfile>{{id={id(self)}}}'
+
+    def __call__(self, *order: TradeInstruction):
+        if len(order) == 1:
+            return self.check(order=order[0])
+        else:
+            return self.check_basket(*order)
+
+    def set_rule(self, key: str, value: float, ticker: str = None):
+        if key in self.rules:
+            limit_set = self.rules[key]
+            new_limit = value
+
+            # update global constrains
+            if ticker is None:
+                if not isinstance(limit_set, dict):
+                    old_limit = limit_set
+                    self.rules[key] = new_limit
+                    LOGGER.info(f'{self} limit updated: <{key}>: {old_limit} -> {new_limit}')
+                else:
+                    LOGGER.error(f'Invalid action: limit <{key}> requires a valid ticker')
+            # update individual constrains
+            else:
+                if isinstance(limit_set, dict):
+                    self.rules.entry.add(ticker)
+                    old_limit = limit_set.get(ticker, 'null')
+                    self.rules[key][ticker] = new_limit
+                    LOGGER.info(f'{self} limit updated: <{key}>({ticker}): {old_limit} -> {new_limit}')
+                else:
+                    LOGGER.error(f'Invalid action: can not set any ticker for limit <{key}>')
+        else:
+            LOGGER.error(f'Invalid action: limit <{key}> not found!')
+
+    def get(self, ticker: str) -> dict[str, float | dict[str, float]]:
+        limit = NameSpace(name=f'RiskLimit.{ticker}', market_price=self.mds.market_price.get(ticker))
+
+        limit['working'] = self._get_volume(ticker=ticker, flag='working')
+        limit['traded'] = self._get_volume(ticker=ticker, flag='traded')
+        limit['exposure'] = self._get_volume(ticker=ticker, flag='exposure')
+
+        # --- global constrains ---
+        if self.rules.max_ttl_notional_long is not None:
+            limit['max_ttl_notional_long'] = self.rules.max_ttl_notional_long
+
+        if self.rules.max_ttl_notional_short is not None:
+            limit['max_ttl_notional_short'] = self.rules.max_ttl_notional_short
+
+        if self.rules.max_net_notional_long is not None:
+            limit['max_net_notional_long'] = self.rules.max_net_notional_long
+
+        if self.rules.max_net_notional_short is not None:
+            limit['max_net_notional_short'] = self.rules.max_net_notional_short
+
+        # --- individual constrains ---
+        if ticker in self.rules.max_percentile:
+            limit['max_percentile'] = self.rules.max_percentile.get(ticker, 1.)
+
+        if ticker in self.rules.max_trade_long:
+            limit['max_trade_long'] = self.rules.max_trade_long.get(ticker, np.inf)
+
+        if ticker in self.rules.max_trade_short:
+            limit['max_trade_short'] = self.rules.max_trade_short.get(ticker, np.inf)
+
+        if ticker in self.rules.max_exposure_long:
+            limit['max_exposure_long'] = self.rules.max_exposure_long.get(ticker, np.inf)
+
+        if ticker in self.rules.max_exposure_short:
+            limit['max_exposure_short'] = self.rules.max_exposure_short.get(ticker, np.inf)
+
+        if ticker in self.rules.max_notional_long:
+            limit['max_notional_long'] = self.rules.max_notional_long.get(ticker, np.inf)
+
+        if ticker in self.rules.max_notional_short:
+            limit['max_notional_short'] = self.rules.max_notional_short.get(ticker, np.inf)
+
+        return limit
+
+    def check(self, order: TradeInstruction):
+        ticker = order.ticker
+
+        # step 0: get limits
+        limit = self.get(ticker=ticker)
+        LOGGER.info(f'{self} defines {limit}')
+
+        try:
+            # step 0: check validity
+            self._check_validity(order=order, limit=limit)
+
+            # step 1: check inventory limit
+            self._check_max_trade(order=order, limit=limit)
+
+            # step 2: check position limit
+            self._check_max_exposure(order=order, limit=limit)
+
+            # step 3: check percentile limit
+            self._check_max_percentile(order=order, limit=limit)
+
+            # step 4: check notional limit
+            self._check_max_notional(order=order, limit=limit)
+
+            # step 5: check portfolio net limit
+            self._check_net_portfolio(order=order, limit=limit)
+
+            # step 6: check portfolio total limit
+            self._check_ttl_portfolio(order=order, limit=limit)
+        except self.Risk as e:
+            LOGGER.error(f'<{e.type}.{e.code}>: {e.msg}')
+            return False
+
+        return True
+
+    def check_order(self, ticker: str, volume: float, side: TransactionSide):
+        fake_order = TradeInstruction(
+            ticker=ticker,
+            side=side,
+            volume=volume
+        )
+
+        return self.check(order=fake_order)
+
+    def check_basket(self, *order: TradeInstruction):
+        LOGGER.warning('risk control for basket order not implemented, check order individually')
+
+        for _ in order:
+            self.check(_)
+
+    def clear(self):
+        self.rules.entry.clear()
+
+        self.rules.max_percentile.clear()
+        self.rules.max_trade_long.clear()
+        self.rules.max_trade_short.clear()
+        self.rules.max_exposure_long.clear()
+        self.rules.max_exposure_short.clear()
+        self.rules.max_notional_long.clear()
+        self.rules.max_notional_short.clear()
+
+        self.rules.max_ttl_notional_long = np.inf
+        self.rules.max_ttl_notional_short = np.inf
+        self.rules.max_net_notional_long = np.inf
+        self.rules.max_net_notional_short = np.inf
+
+    def to_json(self, fmt='str') -> str | dict:
+        json_dict = dict(self.rules)
+        json_dict['entry'] = list(json_dict['entry'])
+
+        if fmt == 'dict':
+            return json_dict
+        else:
+            return json.dumps(json_dict)
+
+    def from_json(self, json_str: str | dict):
+        if isinstance(json_str, (str, bytes)):
+            json_dict = json.loads(json_str)
+        elif isinstance(json_str, dict):
+            json_dict = json_str
+        else:
+            raise TypeError(f'Invalid type {type(json_str)}, expect [str, bytes, dict]')
+
+        self.rules.update(json_dict)
+        self.rules['entry'] = set(self.rules['entry'])
+
+        return self
+
+    def dump(self, file_path: str | pathlib.Path):
+        file_path = pathlib.Path(file_path)
+        dump_dir = file_path.parent
+
+        os.makedirs(dump_dir, exist_ok=True)
+
+        with open(file_path, 'w') as f:
+            f.write(json.dumps(self.to_json(fmt='dict'), indent=4, sort_keys=True))
+
+    def load(self, file_path: str | pathlib.Path):
+        if not os.path.isfile(file_path):
+            LOGGER.error(f'No such file {file_path}')
+            return
+
+        with open(file_path, 'r') as f:
+            json_str = f.read()
+
+        self.from_json(json_str)
+
+    def _check_validity(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
+        ticker = order.ticker
+        market_price = limit['market_price']
+
+        if market_price is None:
+            raise self.Risk(
+                risk_type='RiskProfile.Internal.Price',
+                code=100,
+                msg=f'no valid market price for ticker {ticker}'
+            )
+
+        return True
+
+    def _check_max_trade(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
+        ticker = order.ticker
+        action = abs(order.volume)
+        side = order.side
+
+        if side.sign > 0:
+            flag = 'long'
+        elif side.sign < 0:
+            flag = 'short'
+        else:
+            return
+
+        if f'max_trade_{flag}' not in limit:
+            raise self.Risk(
+                risk_type='RiskProfile.TradeLimit.Invalid',
+                code=1003,
+                msg=f'{ticker} {side.sign * action} rejected! {ticker} not trade-able!'
+            )
+
+        trade_limit = limit[f'max_trade_{flag}']
+        working = limit['working']
+        traded = limit['traded']
+        trade_count = working[flag] + traded[flag]
+
+        # for long order
+        if side.sign > 0:
+            if trade_count + action > trade_limit:
+                raise self.Risk(
+                    risk_type='RiskProfile.TradeLimit.Long',
+                    code=1001,
+                    msg=f'{ticker} {side.sign * action} rejected! lmt={trade_limit}, ttl={trade_count}, inv={trade_limit - trade_count}, action={action}'
+                )
+        elif side.sign < 0:
+            if trade_count + action > trade_limit:
+                raise self.Risk(
+                    risk_type='RiskProfile.TradeLimit.Short',
+                    code=1002,
+                    msg=f'{ticker} {side.sign * action} rejected! lmt={trade_limit}, ttl={trade_count}, inv={trade_limit - trade_count}, action={-action}'
+                )
+
+        return True
+
+    def _check_max_exposure(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
+        ticker = order.ticker
+        action = abs(order.volume)
+        side = order.side
+
+        if side.sign > 0:
+            flag = 'long'
+        elif side.sign < 0:
+            flag = 'short'
+        else:
+            return
+
+        if f'max_exposure_{flag}' not in limit:
+            return
+
+        working = limit['working']
+        exposure = limit['exposure']
+        max_exposure = limit[f'max_exposure_{flag}']
+        working = working[flag]
+
+        ttl_exposure = exposure['long'] - exposure['short']
+
+        expectation_volume_0 = ttl_exposure + working
+        expectation_volume_1 = ttl_exposure + action * side.sign
+        expectation_volume_2 = ttl_exposure + action * side.sign + working
+
+        if side.sign > 0:
+            if expectation_volume_0 <= max_exposure \
+                    and expectation_volume_1 <= max_exposure \
+                    and expectation_volume_2 <= max_exposure:
+                return True
+            else:
+                raise self.Risk(
+                    risk_type='RiskProfile.ExposureLimit.Long',
+                    code=2001,
+                    msg=f'{ticker} {side.sign * action} rejected! lmt_exp={max_exposure}, exp={ttl_exposure}, working={working}, action={action}'
+                )
+        elif side.sign < 0:
+            if expectation_volume_0 >= -max_exposure \
+                    and expectation_volume_1 >= -max_exposure \
+                    and expectation_volume_2 >= -max_exposure:
+                return True
+            else:
+                raise self.Risk(
+                    risk_type='RiskProfile.ExposureLimit.Short',
+                    code=2002,
+                    msg=f'{ticker} {side.sign * action} rejected! lmt_exp={max_exposure}, exp={ttl_exposure}, working={working}, action={-action}'
+                )
+
+    def _check_max_percentile(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
+        ticker = order.ticker
+        action = abs(order.volume)
+        side = order.side
+
+        if 'max_percentile' not in limit:
+            return
+
+        max_percentile = limit['max_percentile']
+        market_price = limit['market_price']
+        total_notional = sum([abs(_) for _ in self.balance.exposure_notional(mds=self.mds).values()])
+
+        if np.isfinite(max_percentile) and max_percentile < 1 and np.isfinite(total_notional):
+            max_notional = np.divide(total_notional, 1 - max_percentile) * max_percentile
+        else:
+            return True
+
+        max_position = np.divide(max_notional, market_price)
+
+        working = limit['working']
+        exposure = limit['exposure']
+
+        ttl_exposure = exposure['long'] - exposure['short']
+
+        if side.sign > 0:
+            working = working['long']
+        elif side.sign < 0:
+            working = working['short']
+        else:
+            return True
+
+        expectation_volume_0 = ttl_exposure + working
+        expectation_volume_1 = ttl_exposure + action * side.sign
+        expectation_volume_2 = ttl_exposure + action * side.sign + working
+
+        if abs(expectation_volume_0) <= max_position \
+                and abs(expectation_volume_1) <= max_position \
+                and abs(expectation_volume_2) <= max_position:
+            return True
+
+        if side.sign > 0:
+            raise self.Risk(
+                risk_type='RiskProfile.PercentileLimit.Long',
+                code=3001,
+                msg=f'{ticker} {side.sign * action} rejected! lmt_pct={max_percentile}, lmt_exp={max_position}, exp={ttl_exposure}, working={working}, action={action}'
+            )
+        elif side.sign < 0:
+            raise self.Risk(
+                risk_type='RiskProfile.PercentileLimit.Short',
+                code=3002,
+                msg=f'{ticker} {side.sign * action} rejected! lmt_pct={max_percentile}, lmt_exp={max_position}, exp={ttl_exposure}, working={working}, action={-action}'
+            )
+
+    def _check_max_notional(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
+        ticker = order.ticker
+        action = abs(order.volume)
+        side = order.side
+
+        if side.sign > 0:
+            flag = 'long'
+        elif side.sign < 0:
+            flag = 'short'
+        else:
+            return
+
+        if f'max_notional_{flag}' not in limit:
+            return
+
+        market_price = limit['market_price']
+        working = limit['working']
+        exposure = limit['exposure']
+        max_notional = limit[f'max_notional_{flag}']
+        working = working[flag]
+        ttl_exposure = exposure['long'] - exposure['short']
+        max_position = np.divide(max_notional, market_price)
+
+        expectation_volume_0 = ttl_exposure + working
+        expectation_volume_1 = ttl_exposure + action * side.sign
+        expectation_volume_2 = ttl_exposure + action * side.sign + working
+
+        if side.sign > 0:
+            if expectation_volume_0 <= max_position \
+                    and expectation_volume_1 <= max_position \
+                    and expectation_volume_2 <= max_position:
+                return True
+            else:
+                raise self.Risk(
+                    risk_type='RiskProfile.NotionalLimit.Long',
+                    code=4001,
+                    msg=f'{ticker} {side.sign * action} rejected! lmt_ntl={max_notional}, lmt_exp={max_position}, exp={ttl_exposure}, working={working}, action={action}'
+                )
+        elif side.sign < 0:
+            if expectation_volume_0 >= -max_position \
+                    and expectation_volume_1 >= -max_position \
+                    and expectation_volume_2 >= -max_position:
+                return True
+            else:
+                raise self.Risk(
+                    risk_type='RiskProfile.NotionalLimit.Short',
+                    code=4002,
+                    msg=f'{ticker} {side.sign * action} rejected! lmt_ntl={max_notional}, lmt_exp={max_position}, exp={ttl_exposure}, working={working}, action={-action}'
+                )
+
+    def _check_net_portfolio(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
+        ticker = order.ticker
+        action = abs(order.volume)
+        side = order.side
+
+        if side.sign > 0:
+            flag = 'long'
+        elif side.sign < 0:
+            flag = 'short'
+        else:
+            return
+
+        if f'max_net_notional_{flag}' not in limit:
+            return
+
+        max_net_notional = limit[f'max_net_notional_{flag}']
+        market_price = limit['market_price']
+        portfolio_working_notional = self.balance.working_notional(mds=self.mds)
+        portfolio_exposure_notional = self.balance.exposure_notional(mds=self.mds)
+
+        net_exposure = sum(portfolio_exposure_notional.values())
+        net_working = sum(portfolio_working_notional.values())
+
+        expectation_var_0 = net_exposure + net_working
+        expectation_var_1 = net_exposure + action * side.sign * market_price
+        expectation_var_2 = net_exposure + action * side.sign * market_price + net_working
+
+        if side.sign > 0:
+            if expectation_var_0 <= max_net_notional \
+                    and expectation_var_1 <= max_net_notional \
+                    and expectation_var_2 <= max_net_notional:
+                return True
+
+            raise self.Risk(
+                risk_type='RiskProfile.NotionalLimit.PortfolioNet.Long',
+                code=5001,
+                msg=f'{ticker} {side.sign * action} rejected! lmt_ntl={max_net_notional}, net_exp={net_exposure}, net_working={net_working}, action={action}'
+            )
+        elif side.sign < 0:
+            if -max_net_notional <= expectation_var_0 \
+                    and -max_net_notional <= expectation_var_1 \
+                    and -max_net_notional <= expectation_var_2:
+                return True
+
+            raise self.Risk(
+                risk_type='RiskProfile.NotionalLimit.PortfolioNet.Short',
+                code=5002,
+                msg=f'{ticker} {side.sign * action} rejected! lmt_ntl={max_net_notional}, net_exp={net_exposure}, net_working={net_working}, action={action}'
+            )
+
+    def _check_ttl_portfolio(self, order: TradeInstruction, limit: dict[str, float | dict[str, float]]):
+        ticker = order.ticker
+        action = abs(order.volume)
+        side = order.side
+
+        if side.sign > 0:
+            flag = 'long'
+        elif side.sign < 0:
+            flag = 'short'
+        else:
+            return
+
+        if f'max_ttl_notional_{flag}' not in limit:
+            return
+
+        market_price = limit['market_price']
+        max_notional = limit[f'max_ttl_notional_{flag}']
+        working_notional = {'long': 0., 'short': 0.}
+        exposure_notional = {'long': 0., 'short': 0.}
+
+        for order_id in list(self.balance.working_order):
+            order = self.balance.working_order.get(order_id, None)
+
+            if order is None:
+                continue
+
+            if order.side.sign > 0:
+                working_notional['long'] += abs(order.working_volume) * market_price
+            elif order.side.sign < 0:
+                working_notional['short'] += abs(order.working_volume) * market_price
+
+        for ticker, notional in self.balance.exposure_notional(mds=self.mds).items():
+            if notional > 0:
+                exposure_notional['long'] += abs(notional)
+            else:
+                exposure_notional['short'] += abs(notional)
+
+        ttl_exposure = exposure_notional[flag]
+        ttl_working = working_notional[flag]
+
+        expectation_var_0 = ttl_exposure + ttl_working
+        expectation_var_1 = ttl_exposure + action * market_price
+        expectation_var_2 = ttl_exposure + action * market_price + ttl_working
+
+        if expectation_var_0 <= max_notional \
+                and expectation_var_1 <= max_notional \
+                and expectation_var_2 <= max_notional:
+            return True
+
+        if side.sign > 0:
+            raise self.Risk(
+                risk_type='RiskProfile.NotionalLimit.PortfolioTotal.Long',
+                code=5003,
+                msg=f'{ticker} {side.sign * action} rejected! lmt_ntl={max_notional}, ttl_exp={ttl_exposure}, ttl_working={ttl_working}, action={action}'
+            )
+        elif side.sign < 0:
+            raise self.Risk(
+                risk_type='RiskProfile.NotionalLimit.PortfolioTotal.Short',
+                code=5004,
+                msg=f'{ticker} {side.sign * action} rejected! lmt_ntl={max_notional}, ttl_exp={ttl_exposure}, ttl_working={ttl_working}, action={action}'
+            )
+
+    def _get_volume(self, ticker: str, flag: str = 'working') -> dict[str, float]:
+        volume = {'long': 0., 'short': 0.}
+        if flag == 'working':
+            for order_id in list(self.balance.working_order):
+                order = self.balance.working_order.get(order_id, None)
+
+                if order is None or order.ticker != ticker or not order.is_working:
+                    continue
+
+                if order.side.sign > 0:
+                    volume['long'] += abs(order.working_volume)
+                elif order.side.sign < 0:
+                    volume['short'] += abs(order.working_volume)
+        elif flag == 'exposure':
+            for trade_id in list(self.balance.trades):
+                trade = self.balance.trades.get(trade_id, None)
+
+                if trade is None or trade.ticker != ticker:
+                    continue
+
+                if trade.side.sign > 0:
+                    volume['long'] += abs(trade.volume)
+                elif trade.side.sign < 0:
+                    volume['short'] += abs(trade.volume)
+        elif flag == 'traded':
+            for trade_id in list(self.balance.trades):
+                trade = self.balance.trades.get(trade_id, None)
+
+                if trade is None \
+                        or trade.ticker != ticker \
+                        or trade.trade_time.date() != self.market_time.date():  # apply to A-Stock when daily inventory is limited
+                    continue
+
+                if trade.side.sign > 0:
+                    volume['long'] += abs(trade.volume)
+                elif trade.side.sign < 0:
+                    volume['short'] += abs(trade.volume)
+        else:
+            raise ValueError(f'Invalid flag {flag}')
+
+        return volume
+
+    @property
+    def market_time(self):
+        return self.mds.market_time
+
+    @property
+    def info(self) -> pd.DataFrame:
+        info_dict = defaultdict(dict)
+
+        rules = self.rules.copy()
+
+        for ticker in rules['entry']:
+            for key in ['max_percentile', 'max_trade_long', 'max_trade_short', 'max_exposure_long', 'max_exposure_short', 'max_notional_long', 'max_notional_short']:
+                if ticker in rules[key]:
+                    info_dict[ticker][key] = rules[key][ticker]
+
+        for key in ['max_ttl_notional_long', 'max_ttl_notional_short', 'max_net_notional_long', 'max_net_notional_short']:
+            if rules[key] is not None:
+                info_dict['global'][key] = rules[key]
+
+        return pd.DataFrame(info_dict).T
+
+
+class SimMatch(object):
+    def __init__(self, ticker, event_engine=None, **kwargs):
+        self.ticker = ticker
+        self.event_engine = event_engine if event_engine is not None else EVENT_ENGINE
+        self.topic_set = kwargs.pop('topic_set', TOPIC)
+
+        self.fee = kwargs.pop('fee', 0.)
+        self.working: dict[str, TradeInstruction] = {}
+        self.history: dict[str, TradeInstruction] = {}
+
+        self.market_time = datetime.datetime.min
+
+    def __call__(self, **kwargs):
+        order = kwargs.pop('order', None)
+        market_data = kwargs.pop('market_data', None)
+
+        if order is not None:
+            if order.order_type == OrderType.LimitOrder:
+                self.launch_order(order=order)
+            elif order.order_type == OrderType.CancelOrder:
+                self.cancel_order(order=order)
+            else:
+                raise ValueError(f'Invalid order {order}')
+
+        if market_data is not None:
+            self.market_time = max(self.market_time, market_data.market_time)
+
+            if isinstance(market_data, BarData):
+                self._check_bar_data(market_data=market_data)
+            elif isinstance(market_data, TickData):
+                self._check_tick_data(market_data=market_data)
+            elif isinstance(market_data, TradeData):
+                self._check_trade_data(market_data=market_data)
+            elif isinstance(market_data, OrderBook):
+                self._check_order_book(market_data=market_data)
+
+    def register(self, topic_set=None, event_engine=None):
+        if topic_set is not None:
+            self.topic_set = topic_set
+
+        if event_engine is not None:
+            self.event_engine = event_engine
+
+        self.event_engine.register_handler(topic=self.topic_set.launch_order(ticker=self.ticker), handler=self.launch_order)
+        self.event_engine.register_handler(topic=self.topic_set.cancel_order(ticker=self.ticker), handler=self.cancel_order)
+        self.event_engine.register_handler(topic=self.topic_set.realtime(ticker=self.ticker), handler=self)
+
+    def unregister(self):
+        self.event_engine.unregister_handler(topic=self.topic_set.launch_order(ticker=self.ticker), handler=self.launch_order)
+        self.event_engine.unregister_handler(topic=self.topic_set.cancel_order(ticker=self.ticker), handler=self.cancel_order)
+        self.event_engine.unregister_handler(topic=self.topic_set.realtime(ticker=self.ticker), handler=self)
+
+    def launch_order(self, order: TradeInstruction, **kwargs):
+        if (order.order_id in self.working) or (order.order_id in self.history):
+            raise ValueError(f'Invalid instruction {order}, OrderId already in working or history')
+        elif order.limit_price is None:
+            LOGGER.warning(f'order {order} does not have a valid limit price!')
+            # raise ValueError(f'Invalid instruction {order}, instruction must have a LimitPrice')
+
+        order.set_order_state(order_state=OrderState.Placed, market_datetime=self.market_time)
+        self.working[order.order_id] = order
+        if 'market_time' not in kwargs:
+            kwargs['market_time'] = self.market_time
+        self.on_order(order=order, **kwargs)
+
+    def cancel_order(self, order: TradeInstruction = None, order_id: str = None, **kwargs):
+        if order is None and order_id is None:
+            raise ValueError('Must assign a order or order_id to cancel order')
+        elif order_id is None:
+            order_id = order.order_id
+
+        # if order_id not in self.working:
+        #     raise ValueError(f'Invalid cancel order {order}, OrderId not found')
+
+        order: TradeInstruction = self.working.pop(order_id, None)
+        if order is None:
+            LOGGER.info(f'[{self.market_time:%Y-%m-%d %H:%M:%S}] failed to cancel {order_id} order!')
+            return
+
+        if order.order_state == OrderState.Filled:
+            pass
+        else:
+            order.set_order_state(order_state=OrderState.Canceled, market_datetime=self.market_time)
+            LOGGER.info(f'[{self.market_time:%Y-%m-%d %H:%M:%S}] Sim-canceled {order.side.name} {order.ticker} order!')
+
+        self.history[order_id] = order
+        self.on_order(order=order, **kwargs)
+
+    def _check_bar_data(self, market_data: BarData):
+        for order_id in list(self.working):
+            order = self.working.get(order_id)
+            if order is None:
+                pass
+            elif order.order_state in [OrderState.Placed, OrderState.PartFilled]:
+                if order.side.sign > 0:
+                    # match order based on worst offer
+                    if order.limit_price is None:
+                        self._match(order=order, match_price=market_data.VWAP)
+                    elif market_data.high_price < order.limit_price:
+                        self._match(order=order, match_price=market_data.high_price)
+                    # match order based on limit price
+                    elif market_data.low_price < order.limit_price:
+                        self._match(order=order, match_price=order.limit_price)
+                    # no match
+                    else:
+                        pass
+                elif order.side.sign < 0:
+                    # match order based on worst offer
+                    if order.limit_price is None:
+                        self._match(order=order, match_price=market_data.VWAP)
+                    elif market_data.low_price > order.limit_price:
+                        self._match(order=order, match_price=market_data.low_price)
+                    # match order based on limit price
+                    elif market_data.high_price > order.limit_price:
+                        self._match(order=order, match_price=order.limit_price)
+                    # no match
+                    else:
+                        pass
+            else:
+                continue
+                # raise ValueError(f'Invalid working order state {order}')
+
+    def _check_trade_data(self, market_data: TradeData):
+        for order_id in list(self.working):
+            order = self.working.get(order_id)
+            if order is None:
+                pass
+            elif order.is_working:
+                if order.start_time > market_data.market_time:
+                    pass
+                elif order.limit_price is None:
+                    if order.side.sign * market_data.side.sign > 0:
+                        self._match(order=order, match_volume=market_data.volume, match_price=market_data.market_price)
+                elif order.side.sign > 0 and market_data.market_price < order.limit_price:
+                    self._match(order=order, match_volume=market_data.volume, match_price=market_data.market_price)
+                elif order.side.sign < 0 and market_data.market_price > order.limit_price:
+                    self._match(order=order, match_volume=market_data.volume, match_price=market_data.market_price)
+            else:
+                continue
+                # raise ValueError(f'Invalid working order state {order}')
+
+    def _check_order_book(self, market_data: OrderBook):
+        for order_id in list(self.working):
+            order = self.working.get(order_id)
+
+            match_volume = 0.
+            match_notional = 0.
+
+            if order is None:
+                pass
+            elif order.order_state in [OrderState.Placed, OrderState.PartFilled]:
+                if order.limit_price is None:
+                    if order.side.sign > 0:
+                        for entry in market_data.ask:
+                            if match_volume < order.working_volume:
+                                addition_volume = min(entry.volume, order.working_volume - match_volume)
+                                match_volume += addition_volume
+                                match_notional += addition_volume * entry.price
+                            else:
+                                break
+                    else:
+                        for entry in market_data.bid:
+                            if match_volume < order.working_volume:
+                                addition_volume = min(entry.volume, order.working_volume - match_volume)
+                                match_volume += addition_volume
+                                match_notional += addition_volume * entry.price
+                            else:
+                                break
+                elif order.side.sign > 0 and market_data.best_ask_price <= order.limit_price:
+                    for entry in market_data.ask:
+                        if entry.price <= order.limit_price:
+                            if match_volume < order.working_volume:
+                                addition_volume = min(entry.volume, order.working_volume - match_volume)
+                                match_volume += addition_volume
+                                match_notional += addition_volume * entry.price
+                            else:
+                                break
+                        else:
+                            break
+                elif order.side.sign < 0 and market_data.best_bid_price >= order.limit_price:
+                    for entry in market_data.bid:
+                        if entry.price >= order.limit_price:
+                            if match_volume < order.working_volume:
+                                addition_volume = min(entry.volume, order.working_volume - match_volume)
+                                match_volume += addition_volume
+                                match_notional += addition_volume * entry.price
+                            else:
+                                break
+                        else:
+                            break
+
+                if match_volume:
+                    self._match(order=order, match_volume=match_volume, match_price=match_notional / match_volume)
+            else:
+                continue
+                # raise ValueError(f'Invalid working order state {order}')
+
+    def _check_tick_data(self, market_data: TickData):
+        return self._check_order_book(market_data=market_data.order_book)
+
+    def _match(self, order: TradeInstruction, match_volume: float = None, match_price: float = None):
+        if match_volume is None:
+            match_volume = order.working_volume
+        elif match_volume > order.working_volume:
+            match_volume = order.working_volume
+
+        if order.limit_price is None:
+            pass
+        elif match_price is None:
+            match_price = order.limit_price
+        elif order.side.sign > 0 and match_price > order.limit_price:
+            LOGGER.warning(f'match price greater than limit price for bid order {order}')
+            match_price = order.limit_price
+        elif order.side.sign < 0 and match_price < order.limit_price:
+            match_price = order.limit_price
+            LOGGER.warning(f'match price less than limit price for ask order {order}')
+
+        if match_volume:
+            report = TradeReport(
+                ticker=order.ticker,
+                side=order.side,
+                volume=match_volume,
+                notional=match_volume * match_price * order.multiplier,
+                trade_time=self.market_time,
+                order_id=order.order_id,
+                price=match_price,
+                multiplier=order.multiplier,
+                fee=self.fee * match_volume * match_price * order.multiplier
+            )
+
+            LOGGER.info(f'[{self.market_time:%Y-%m-%d %H:%M:%S}] Sim-filled {order.ticker} {order.side.name} {report.volume:,.2f} @ {report.price:.2f}')
+            order.fill(trade_report=report)
+
+            if order.order_state == OrderState.Filled:
+                self.working.pop(order.order_id, None)
+                self.history[order.order_id] = order
+
+            self.on_report(report=report)
+            self.on_order(order=order)
+            return report
+        else:
+            return None
+
+    def on_order(self, order, **kwargs):
+        self.event_engine.put(topic=self.topic_set.on_order, order=order)
+
+    def on_report(self, report, **kwargs):
+        self.event_engine.put(topic=self.topic_set.on_report, report=report, **kwargs)
+
+    def eod(self):
+        for order_id in list(self.working):
+            self.cancel_order(order_id=order_id)
+
+    def clear(self):
+        self.fee = 0.
+        self.working.clear()
+        self.history.clear()
+        self.market_time = datetime.datetime.min
```

### Comparing `PyAlgoEngine-0.3.5/AlgoEngine/Strategies/BackTest.py` & `PyAlgoEngine-0.3.6/AlgoEngine/Strategies/BackTest.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from __future__ import annotations
-
-import datetime
-
-import EventEngine
-
-from . import EventDMA
-from ._StrategyEngine import StrategyEngine
-from ..Engine import LOGGER, TOPIC, MarketDataService, Balance, RiskProfile, PositionManagementService
-from ..Engine.AlgoEngine import AlgoRegistry, AlgoEngine
-
-LOGGER = LOGGER.getChild('BackTest')
-
-
-def test_stop(code=0):
-    EVENT_ENGINE.stop()
-    # noinspection PyUnresolvedReferences, PyProtectedMember
-    # `import os`
-    # `os._exit(code)`
-
-
-def test_start(start_date: datetime.date, end_date: datetime.date, data_loader: callable, **kwargs):
-    EVENT_ENGINE.start()
-    STRATEGY_ENGINE.back_test(
-        start_date=start_date,
-        end_date=end_date,
-        data_loader=data_loader,
-        **kwargs
-    )
-
-
-# in backtest, the global objects is newly inited to separate from production
-EVENT_ENGINE = EventEngine.EventEngine()
-MDS = MarketDataService()
-ALGO_REGISTRY = AlgoRegistry()
-ALGO_ENGINE = AlgoEngine(mds=MDS, registry=ALGO_REGISTRY)
-
-BALANCE = Balance()
-RISK_PROFILE = RiskProfile(mds=MDS, balance=BALANCE)
-DMA = EventDMA(event_engine=EVENT_ENGINE, mds=MDS, risk_profile=RISK_PROFILE)
-POSITION_TRACKER = PositionManagementService(dma=DMA, algo_engine=ALGO_ENGINE)
-STRATEGY_ENGINE = StrategyEngine(event_engine=EVENT_ENGINE, position_tracker=POSITION_TRACKER)
-BALANCE.add(strategy=STRATEGY_ENGINE, position_tracker=POSITION_TRACKER)
-
-EVENT_ENGINE.register_handler(topic=TOPIC.realtime, handler=MDS.on_market_data)
-EVENT_ENGINE.register_handler(topic=TOPIC.on_report, handler=BALANCE.on_report)
-EVENT_ENGINE.register_handler(topic=TOPIC.on_order, handler=BALANCE.on_order)
-STRATEGY_ENGINE.register()
-
-MDS.synthetic_orderbook = True
-
-__all__ = ['BALANCE', 'RISK_PROFILE', 'DMA', 'POSITION_TRACKER', 'STRATEGY_ENGINE', 'BALANCE', 'EVENT_ENGINE', 'MDS']
+from __future__ import annotations
+
+import datetime
+
+import EventEngine
+
+from . import EventDMA
+from ._StrategyEngine import StrategyEngine
+from ..Engine import LOGGER, TOPIC, MarketDataService, Balance, RiskProfile, PositionManagementService
+from ..Engine.AlgoEngine import AlgoRegistry, AlgoEngine
+
+LOGGER = LOGGER.getChild('BackTest')
+
+
+def test_stop(code=0):
+    EVENT_ENGINE.stop()
+    # noinspection PyUnresolvedReferences, PyProtectedMember
+    # `import os`
+    # `os._exit(code)`
+
+
+def test_start(start_date: datetime.date, end_date: datetime.date, data_loader: callable, **kwargs):
+    EVENT_ENGINE.start()
+    STRATEGY_ENGINE.back_test(
+        start_date=start_date,
+        end_date=end_date,
+        data_loader=data_loader,
+        **kwargs
+    )
+
+
+# in backtest, the global objects is newly inited to separate from production
+EVENT_ENGINE = EventEngine.EventEngine()
+MDS = MarketDataService()
+ALGO_REGISTRY = AlgoRegistry()
+ALGO_ENGINE = AlgoEngine(mds=MDS, registry=ALGO_REGISTRY)
+
+BALANCE = Balance()
+RISK_PROFILE = RiskProfile(mds=MDS, balance=BALANCE)
+DMA = EventDMA(event_engine=EVENT_ENGINE, mds=MDS, risk_profile=RISK_PROFILE)
+POSITION_TRACKER = PositionManagementService(dma=DMA, algo_engine=ALGO_ENGINE)
+STRATEGY_ENGINE = StrategyEngine(event_engine=EVENT_ENGINE, position_tracker=POSITION_TRACKER)
+BALANCE.add(strategy=STRATEGY_ENGINE, position_tracker=POSITION_TRACKER)
+
+EVENT_ENGINE.register_handler(topic=TOPIC.realtime, handler=MDS.on_market_data)
+EVENT_ENGINE.register_handler(topic=TOPIC.on_report, handler=BALANCE.on_report)
+EVENT_ENGINE.register_handler(topic=TOPIC.on_order, handler=BALANCE.on_order)
+STRATEGY_ENGINE.register()
+
+MDS.synthetic_orderbook = True
+
+__all__ = ['BALANCE', 'RISK_PROFILE', 'DMA', 'POSITION_TRACKER', 'STRATEGY_ENGINE', 'BALANCE', 'EVENT_ENGINE', 'MDS']
```

### Comparing `PyAlgoEngine-0.3.5/AlgoEngine/Strategies/__init__.py` & `PyAlgoEngine-0.3.6/AlgoEngine/Strategies/__init__.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from __future__ import annotations
-
-import threading
-
-from PyQuantKit import TradeInstruction
-
-from ._StrategyEngine import StrategyEngine
-from ..Engine import LOGGER
-from ..Engine.EventEngine import EVENT_ENGINE, TOPIC
-from ..Engine.MarketEngine import MDS, MarketDataService
-from ..Engine.TradeEngine import Balance, Inventory, DirectMarketAccess, RiskProfile, PositionManagementService
-
-LOGGER = LOGGER.getChild('Strategies')
-
-
-class EventDMA(DirectMarketAccess):
-    def __init__(self, mds: MarketDataService, risk_profile: RiskProfile, event_engine=None, cool_down: float = None):
-        self.event_engine = EVENT_ENGINE if event_engine is None else event_engine
-        super().__init__(mds=mds, risk_profile=risk_profile, cool_down=cool_down)
-
-    def _launch_order_handler(self, order: TradeInstruction, **kwargs):
-        self.event_engine.put(topic=TOPIC.launch_order(ticker=order.ticker), order=order, **kwargs)
-
-    def _cancel_order_handler(self, order: TradeInstruction, **kwargs):
-        self.event_engine.put(topic=TOPIC.cancel_order(ticker=order.ticker), order_id=order.order_id, **kwargs)
-
-    def _reject_order_handler(self, order: TradeInstruction, **kwargs):
-        raise NotImplementedError()
-
-
-REPLAY_LOCK = threading.Lock()
-INVENTORY = Inventory()
-BALANCE = Balance(inventory=INVENTORY)
-RISK_PROFILE = RiskProfile(mds=MDS, balance=BALANCE)
-DMA = EventDMA(mds=MDS, risk_profile=RISK_PROFILE)
-POSITION_TRACKER = PositionManagementService(dma=DMA)
-STRATEGY_ENGINE = StrategyEngine(event_engine=EVENT_ENGINE, position_tracker=POSITION_TRACKER)
-BALANCE.add(strategy=STRATEGY_ENGINE, position_tracker=POSITION_TRACKER)
-
-__all__ = ['INVENTORY', 'BALANCE', 'RISK_PROFILE', 'DMA', 'POSITION_TRACKER', 'STRATEGY_ENGINE']
+from __future__ import annotations
+
+import threading
+
+from PyQuantKit import TradeInstruction
+
+from ._StrategyEngine import StrategyEngine
+from ..Engine import LOGGER
+from ..Engine.EventEngine import EVENT_ENGINE, TOPIC
+from ..Engine.MarketEngine import MDS, MarketDataService
+from ..Engine.TradeEngine import Balance, Inventory, DirectMarketAccess, RiskProfile, PositionManagementService
+
+LOGGER = LOGGER.getChild('Strategies')
+
+
+class EventDMA(DirectMarketAccess):
+    def __init__(self, mds: MarketDataService, risk_profile: RiskProfile, event_engine=None, cool_down: float = None):
+        self.event_engine = EVENT_ENGINE if event_engine is None else event_engine
+        super().__init__(mds=mds, risk_profile=risk_profile, cool_down=cool_down)
+
+    def _launch_order_handler(self, order: TradeInstruction, **kwargs):
+        self.event_engine.put(topic=TOPIC.launch_order(ticker=order.ticker), order=order, **kwargs)
+
+    def _cancel_order_handler(self, order: TradeInstruction, **kwargs):
+        self.event_engine.put(topic=TOPIC.cancel_order(ticker=order.ticker), order_id=order.order_id, **kwargs)
+
+    def _reject_order_handler(self, order: TradeInstruction, **kwargs):
+        raise NotImplementedError()
+
+
+REPLAY_LOCK = threading.Lock()
+INVENTORY = Inventory()
+BALANCE = Balance(inventory=INVENTORY)
+RISK_PROFILE = RiskProfile(mds=MDS, balance=BALANCE)
+DMA = EventDMA(mds=MDS, risk_profile=RISK_PROFILE)
+POSITION_TRACKER = PositionManagementService(dma=DMA)
+STRATEGY_ENGINE = StrategyEngine(event_engine=EVENT_ENGINE, position_tracker=POSITION_TRACKER)
+BALANCE.add(strategy=STRATEGY_ENGINE, position_tracker=POSITION_TRACKER)
+
+__all__ = ['INVENTORY', 'BALANCE', 'RISK_PROFILE', 'DMA', 'POSITION_TRACKER', 'STRATEGY_ENGINE']
```

### Comparing `PyAlgoEngine-0.3.5/PKG-INFO` & `PyAlgoEngine-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.3.5
+Version: 0.3.6
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `PyAlgoEngine-0.3.5/PyAlgoEngine.egg-info/PKG-INFO` & `PyAlgoEngine-0.3.6/PyAlgoEngine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.3.5
+Version: 0.3.6
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

