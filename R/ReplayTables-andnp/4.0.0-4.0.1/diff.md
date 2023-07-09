# Comparing `tmp/ReplayTables-andnp-4.0.0.tar.gz` & `tmp/ReplayTables-andnp-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReplayTables-andnp-4.0.0.tar", last modified: Fri Jul  7 20:37:16 2023, max compression
+gzip compressed data, was "ReplayTables-andnp-4.0.1.tar", last modified: Sun Jul  9 02:21:39 2023, max compression
```

## Comparing `ReplayTables-andnp-4.0.0.tar` & `ReplayTables-andnp-4.0.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     2350 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/README.md
--rw-r--r--   0        0        0     5287 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/Distributions.py
--rw-r--r--   0        0        0     2140 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/LagBuffer.py
--rw-r--r--   0        0        0     1972 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/PER.py
--rw-r--r--   0        0        0     2787 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/ReplayBuffer.py
--rw-r--r--   0        0        0     8237 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/Table.py
--rw-r--r--   0        0        0        0 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/__init__.py
--rw-r--r--   0        0        0      398 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/_utils/LagBuffer.py
--rw-r--r--   0        0        0     3418 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/_utils/MemoryWriter.py
--rw-r--r--   0        0        0     5811 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/_utils/MinMaxHeap.py
--rw-r--r--   0        0        0     1772 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/_utils/RandDict.py
--rw-r--r--   0        0        0     3822 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/_utils/SumTree.py
--rw-r--r--   0        0        0        0 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/_utils/__init__.py
--rw-r--r--   0        0        0     1356 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/_utils/jit.py
--rw-r--r--   0        0        0       58 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/_utils/logger.py
--rw-r--r--   0        0        0      622 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/ingress/CircularMapper.py
--rw-r--r--   0        0        0      452 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/ingress/IndexMapper.py
--rw-r--r--   0        0        0     1080 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/interface.py
--rw-r--r--   0        0        0      668 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/sampling/IndexSampler.py
--rw-r--r--   0        0        0     1772 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/sampling/PrioritySampler.py
--rw-r--r--   0        0        0      886 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/sampling/UniformSampler.py
--rw-r--r--   0        0        0     2878 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/storage/BasicStorage.py
--rw-r--r--   0        0        0      828 2023-07-07 20:36:35.796446 ReplayTables-andnp-4.0.0/ReplayTables/storage/Storage.py
--rw-r--r--   0        0        0      938 2023-07-07 20:37:13.012448 ReplayTables-andnp-4.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 20:36:35.800446 ReplayTables-andnp-4.0.0/tests/__init__.py
--rw-r--r--   0        0        0      653 2023-07-07 20:36:35.800446 ReplayTables-andnp-4.0.0/tests/_utils/fake_data.py
--rw-r--r--   0        0        0     2932 2023-07-07 20:36:35.800446 ReplayTables-andnp-4.0.0/tests/test_LagBuffer.py
--rw-r--r--   0        0        0     3839 2023-07-07 20:36:35.800446 ReplayTables-andnp-4.0.0/tests/test_PER.py
--rw-r--r--   0        0        0     3052 2023-07-07 20:36:35.800446 ReplayTables-andnp-4.0.0/tests/test_ReplayBuffer.py
--rw-r--r--   0        0        0     1422 2023-07-07 20:36:35.800446 ReplayTables-andnp-4.0.0/tests/test_Table.py
--rw-r--r--   0        0        0     5453 2023-07-07 20:36:35.800446 ReplayTables-andnp-4.0.0/tests/test_View.py
--rw-r--r--   0        0        0     1198 2023-07-07 20:36:35.800446 ReplayTables-andnp-4.0.0/tests/test_integration.py
--rw-r--r--   0        0        0        0 2023-07-07 20:36:35.800446 ReplayTables-andnp-4.0.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1002 2023-07-07 20:36:35.800446 ReplayTables-andnp-4.0.0/tests/utils/test_MinMaxHeap.py
--rw-r--r--   0        0        0     3635 2023-07-07 20:36:35.800446 ReplayTables-andnp-4.0.0/tests/utils/test_SumTree.py
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 ReplayTables-andnp-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2350 2023-07-09 02:20:54.011301 ReplayTables-andnp-4.0.1/README.md
+-rw-r--r--   0        0        0     5287 2023-07-09 02:20:54.011301 ReplayTables-andnp-4.0.1/ReplayTables/Distributions.py
+-rw-r--r--   0        0        0     2140 2023-07-09 02:20:54.011301 ReplayTables-andnp-4.0.1/ReplayTables/LagBuffer.py
+-rw-r--r--   0        0        0     1999 2023-07-09 02:20:54.011301 ReplayTables-andnp-4.0.1/ReplayTables/PER.py
+-rw-r--r--   0        0        0     2799 2023-07-09 02:20:54.011301 ReplayTables-andnp-4.0.1/ReplayTables/ReplayBuffer.py
+-rw-r--r--   0        0        0     8237 2023-07-09 02:20:54.011301 ReplayTables-andnp-4.0.1/ReplayTables/Table.py
+-rw-r--r--   0        0        0        0 2023-07-09 02:20:54.011301 ReplayTables-andnp-4.0.1/ReplayTables/__init__.py
+-rw-r--r--   0        0        0      398 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/_utils/LagBuffer.py
+-rw-r--r--   0        0        0     3418 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/_utils/MemoryWriter.py
+-rw-r--r--   0        0        0     5811 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/_utils/MinMaxHeap.py
+-rw-r--r--   0        0        0     1772 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/_utils/RandDict.py
+-rw-r--r--   0        0        0     2694 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/_utils/SamplableSet.py
+-rw-r--r--   0        0        0     3822 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/_utils/SumTree.py
+-rw-r--r--   0        0        0        0 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/_utils/__init__.py
+-rw-r--r--   0        0        0     1356 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/_utils/jit.py
+-rw-r--r--   0        0        0       58 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/_utils/logger.py
+-rw-r--r--   0        0        0      622 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/ingress/CircularMapper.py
+-rw-r--r--   0        0        0      452 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/ingress/IndexMapper.py
+-rw-r--r--   0        0        0     1081 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/interface.py
+-rw-r--r--   0        0        0      721 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/sampling/IndexSampler.py
+-rw-r--r--   0        0        0     1978 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/sampling/PrioritySampler.py
+-rw-r--r--   0        0        0      809 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/sampling/UniformSampler.py
+-rw-r--r--   0        0        0     3567 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/storage/BasicStorage.py
+-rw-r--r--   0        0        0      838 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/ReplayTables/storage/Storage.py
+-rw-r--r--   0        0        0      938 2023-07-09 02:21:36.305425 ReplayTables-andnp-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      653 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/tests/_utils/fake_data.py
+-rw-r--r--   0        0        0     2932 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/tests/test_LagBuffer.py
+-rw-r--r--   0        0        0     3737 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/tests/test_PER.py
+-rw-r--r--   0        0        0     3527 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/tests/test_ReplayBuffer.py
+-rw-r--r--   0        0        0     1422 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/tests/test_Table.py
+-rw-r--r--   0        0        0     5453 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/tests/test_View.py
+-rw-r--r--   0        0        0     1198 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/tests/test_integration.py
+-rw-r--r--   0        0        0        0 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1002 2023-07-09 02:20:54.015301 ReplayTables-andnp-4.0.1/tests/utils/test_MinMaxHeap.py
+-rw-r--r--   0        0        0     3635 2023-07-09 02:20:54.019301 ReplayTables-andnp-4.0.1/tests/utils/test_SumTree.py
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 ReplayTables-andnp-4.0.1/PKG-INFO
```

### Comparing `ReplayTables-andnp-4.0.0/README.md` & `ReplayTables-andnp-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/Distributions.py` & `ReplayTables-andnp-4.0.1/ReplayTables/Distributions.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/LagBuffer.py` & `ReplayTables-andnp-4.0.1/ReplayTables/LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/PER.py` & `ReplayTables-andnp-4.0.1/ReplayTables/PER.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from dataclasses import dataclass
 from typing import Any, Optional
-from ReplayTables.interface import EID, EIDs, Timestep
+from ReplayTables.interface import EID, Timestep, Batch
 from ReplayTables.ReplayBuffer import ReplayBufferInterface
 from ReplayTables.sampling.PrioritySampler import PrioritySampler
 
 @dataclass
 class PERConfig:
     new_priority_mode: str = 'max'
     uniform_probability: float = 1e-3
@@ -35,21 +35,21 @@
             priority = total_priority / self.size()
             if priority == 0:
                 priority = 1e-16
         else:
             raise NotImplementedError()
 
         idx = self._idx_mapper.eid2idx(eid)
-        self._sampler.replace(idx, priority=priority)
+        self._sampler.replace(idx, transition, priority=priority)
 
-    def update_priorities(self, eids: EIDs, priorities: np.ndarray):
-        idxs = self._idx_mapper.eids2idxs(eids)
+    def update_priorities(self, batch: Batch, priorities: np.ndarray):
+        idxs = self._idx_mapper.eids2idxs(batch.eid)
 
         priorities = priorities ** self._c.priority_exponent
-        self._sampler.update(idxs, priorities=priorities)
+        self._sampler.update(idxs, batch, priorities=priorities)
 
         self._max_priority = max(
             self._c.max_decay * self._max_priority,
             priorities.max(),
         )
 
     def delete_sample(self, eid: EID):
```

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/ReplayBuffer.py` & `ReplayTables-andnp-4.0.1/ReplayTables/ReplayBuffer.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,8 +72,8 @@
 
 class ReplayBuffer(ReplayBufferInterface):
     def __init__(self, max_size: int, lag: int, rng: np.random.Generator):
         super().__init__(max_size, lag, rng)
 
     def _on_add(self, eid: EID, transition: Timestep, /, **kwargs: Any):
         idx = self._idx_mapper.add_eid(eid)
-        self._sampler.replace(idx, **kwargs)
+        self._sampler.replace(idx, transition, **kwargs)
```

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/Table.py` & `ReplayTables-andnp-4.0.1/ReplayTables/Table.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/_utils/MemoryWriter.py` & `ReplayTables-andnp-4.0.1/ReplayTables/_utils/MemoryWriter.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/_utils/MinMaxHeap.py` & `ReplayTables-andnp-4.0.1/ReplayTables/_utils/MinMaxHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/_utils/RandDict.py` & `ReplayTables-andnp-4.0.1/ReplayTables/_utils/RandDict.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/_utils/SumTree.py` & `ReplayTables-andnp-4.0.1/ReplayTables/_utils/SumTree.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/_utils/jit.py` & `ReplayTables-andnp-4.0.1/ReplayTables/_utils/jit.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/ingress/CircularMapper.py` & `ReplayTables-andnp-4.0.1/ReplayTables/ingress/CircularMapper.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/interface.py` & `ReplayTables-andnp-4.0.1/ReplayTables/interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def __rmul__(self, other: Any, /) -> Any:
         ...
 
     def __pow__(self, other: Any, /) -> Any:
         ...
 
 class Timestep(NamedTuple):
-    x: Any
+    x: Any | None
     a: Any
     r: Ring | None
     gamma: Ring
     terminal: Any
 
 class TaggedTimestep(NamedTuple):
     x: Any
@@ -40,15 +40,15 @@
 
 class Batch(NamedTuple):
     x: np.ndarray
     a: np.ndarray
     r: np.ndarray
     gamma: np.ndarray
     terminal: np.ndarray
-    eid: np.ndarray
+    eid: EIDs
     xp: np.ndarray
 
 T = TypeVar('T', bound=Timestep)
 
 def expect_tagged(t: Timestep) -> TaggedTimestep:
     assert hasattr(t, 'eid')
     return cast(Any, t)
```

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/sampling/IndexSampler.py` & `ReplayTables-andnp-4.0.1/ReplayTables/storage/Storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,35 @@
-import numpy as np
 from abc import abstractmethod
 from typing import Any
-from ReplayTables.interface import IDX, IDXs
-from ReplayTables.Distributions import UniformDistribution
+from ReplayTables.interface import Batch, Timestep, TaggedTimestep, EID, EIDs, IDX, IDXs
 
-class IndexSampler:
-    def __init__(self, rng: np.random.Generator) -> None:
-        self._rng = rng
-        self._target = UniformDistribution(0)
+class Storage:
+    def __init__(self, max_size: int):
+        self._max_size = max_size
 
     @abstractmethod
-    def replace(self, idx: IDX, /, **kwargs: Any) -> None:
+    def __len__(self) -> int:
         ...
 
     @abstractmethod
-    def update(self, idxs: IDXs, /, **kwargs: Any) -> None:
+    def __delitem__(self, idx: IDX):
         ...
 
     @abstractmethod
-    def isr_weights(self, idxs: IDXs) -> np.ndarray:
+    def get(self, idxs: IDXs, n_idxs: IDXs, lag: int) -> Batch:
         ...
 
     @abstractmethod
-    def sample(self, n: int) -> IDXs:
+    def get_item(self, idx: IDX) -> TaggedTimestep:
+        ...
+
+    @abstractmethod
+    def set(self, idx: IDX, eid: EID, transition: Timestep):
+        ...
+
+    @abstractmethod
+    def add(self, idx: IDX, eid: EID, transition: Timestep, /, **kwargs: Any) -> None:
+        ...
+
+    @abstractmethod
+    def get_eids(self, idxs: IDXs) -> EIDs:
         ...
```

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/sampling/PrioritySampler.py` & `ReplayTables-andnp-4.0.1/ReplayTables/sampling/PrioritySampler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from typing import Any
 from ReplayTables.sampling.IndexSampler import IndexSampler
 from ReplayTables.Distributions import MixinUniformDistribution, SubDistribution, PrioritizedDistribution, MixtureDistribution
-from ReplayTables.interface import IDX, IDXs
+from ReplayTables.interface import IDX, IDXs, Timestep, Batch
 
 class PrioritySampler(IndexSampler):
     def __init__(
         self,
         uniform_probability: float,
         max_size: int,
         rng: np.random.Generator,
@@ -19,22 +19,28 @@
         self._p_dist = PrioritizedDistribution()
         self._dist = MixtureDistribution(max_size, dists=[
             SubDistribution(d=self._p_dist, p=1 - uniform_probability),
             SubDistribution(d=self._uniform, p=uniform_probability)
         ])
         self._max = max_size
 
-    def replace(self, idx: IDX, /, **kwargs: Any) -> None:
-        priority: float = kwargs['priority']
+    def replace(self, idx: IDX, transition: Timestep, /, **kwargs: Any) -> None:
         idxs = np.array([idx])
+
+        if transition.terminal:
+            self._uniform.set(idxs, np.zeros(1))
+            self._p_dist.update(idxs, np.zeros(1))
+            return
+
+        priority: float = kwargs['priority']
         priorities = np.array([priority])
         self._uniform.update(idxs)
         self._p_dist.update(idxs, priorities)
 
-    def update(self, idxs: IDXs, /, **kwargs: Any) -> None:
+    def update(self, idxs: IDXs, batch: Batch, /, **kwargs: Any) -> None:
         priorities = kwargs['priorities']
         self._uniform.update(idxs)
         self._p_dist.update(idxs, priorities)
 
     def isr_weights(self, idxs: IDXs):
         return self._dist.isr(self._target, idxs)
```

### Comparing `ReplayTables-andnp-4.0.0/ReplayTables/storage/BasicStorage.py` & `ReplayTables-andnp-4.0.1/ReplayTables/storage/BasicStorage.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,52 +2,67 @@
 from typing import Any, Dict
 from ReplayTables.interface import Batch, EIDs, Timestep, TaggedTimestep, EID, IDX, IDXs
 from ReplayTables.storage.Storage import Storage
 
 from ReplayTables._utils.jit import try2jit
 
 class BasicStorage(Storage):
-    def __init__(self, max_size: int):
+    def __init__(self, max_size: int, sample_obs: np.ndarray | None = None, action_dtype: Any = np.int_):
         super().__init__(max_size)
 
         self._state_store: Dict[IDX, np.ndarray] = {}
         self._eids = np.zeros(max_size, dtype=np.uint64)
-        # TODO: we should take dtype params to optionally store this as an integer
-        self._a = np.zeros(max_size)
+        self._a = np.zeros(max_size, dtype=action_dtype)
         self._r = np.zeros(max_size)
         self._term = np.zeros(max_size, dtype=np.bool_)
         self._gamma = np.zeros(max_size)
 
+        self._zero_obs: np.ndarray | None = None
+        if sample_obs is not None:
+            self._zero_obs = np.zeros_like(sample_obs)
+
     def add(self, idx: IDX, eid: EID, transition: Timestep, /, **kwargs: Any):
-        self._state_store[idx] = transition.x
+        if transition.x is not None:
+            self._state_store[idx] = transition.x
+        else:
+            assert self._zero_obs is not None, 'Need to specify a default sample observation is terminal states are marked as None'
+            self._state_store[idx] = self._zero_obs
+
         self._r[idx] = transition.r
         self._a[idx] = transition.a
         self._term[idx] = transition.terminal
         self._gamma[idx] = transition.gamma
         self._eids[idx] = eid
 
-    def set(self, idx: IDX, transition: Timestep):
-        self._state_store[idx] = transition.x
+    def set(self, idx: IDX, eid: EID, transition: Timestep):
+        if transition.x is not None:
+            self._state_store[idx] = transition.x
+        else:
+            assert self._zero_obs is not None, 'Need to specify a default sample observation is terminal states are marked as None'
+            self._state_store[idx] = self._zero_obs
+
         self._r[idx] = transition.r
         self._a[idx] = transition.a
         self._term[idx] = transition.terminal
         self._gamma[idx] = transition.gamma
+        self._eids[idx] = eid
 
     def get(self, idxs: IDXs, n_idxs: IDXs, lag: int) -> Batch:
         x = np.stack([self._state_store[idx] for idx in idxs], axis=0)
         xp = np.stack([self._state_store[idx] for idx in n_idxs], axis=0)
 
+        eids: Any = self._eids[idxs]
         r, gamma, term = _return(self._max_size - lag, idxs, lag, self._r, self._term, self._gamma)
         return Batch(
             x=x,
             a=self._a[idxs],
             r=r,
             gamma=gamma,
             terminal=term,
-            eid=self._eids[idxs],
+            eid=eids,
             xp=xp,
         )
 
     def get_item(self, idx: IDX) -> TaggedTimestep:
         eid: Any = self._eids[idx]
         return TaggedTimestep(
             x=self._state_store[idx],
```

### Comparing `ReplayTables-andnp-4.0.0/pyproject.toml` & `ReplayTables-andnp-4.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "4.0.0"
+version = "4.0.1"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
 ]
 
 [tool.pdm]
 source = [
@@ -16,23 +16,23 @@
     "mypy",
     "flake8",
     "commitizen",
     "pre-commit",
     "matplotlib",
     "twine",
     "pytest>=7.3.2",
-    "pytest-benchmark>=4.0.0",
+    "pytest-benchmark>=4.0.1",
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "ReplayTables-andnp"
-version = "4.0.0"
+version = "4.0.1"
 description = "A simple replay buffer implementation in python for sampling n-step trajectories"
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numba>=0.57",
     "numpy>=1.23.5",
```

### Comparing `ReplayTables-andnp-4.0.0/tests/_utils/fake_data.py` & `ReplayTables-andnp-4.0.1/tests/_utils/fake_data.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/tests/test_LagBuffer.py` & `ReplayTables-andnp-4.0.1/tests/test_LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/tests/test_PER.py` & `ReplayTables-andnp-4.0.1/tests/test_PER.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pickle
 import numpy as np
 from typing import cast
 
-from ReplayTables.interface import EID, EIDs, Timestep
+from ReplayTables.interface import EID, Timestep
 from ReplayTables.PER import PrioritizedReplay
 
 from tests._utils.fake_data import fake_timestep
 
 class TestPER:
     def test_simple_buffer(self):
         rng = np.random.default_rng(0)
@@ -77,17 +77,14 @@
         for i in range(5):
             buffer.add(fake_timestep(
                 x=np.ones(8) * i,
                 a=2 * i,
             ))
 
         buffer.add(fake_timestep())
-        ids = cast(EIDs, np.arange(5))
-        buffer.update_priorities(ids, np.arange(5) + 1)
-
         byt = pickle.dumps(buffer)
         buffer2 = pickle.loads(byt)
 
         s, _ = buffer.sample(20)
         s2, _ = buffer2.sample(20)
 
         assert np.all(s.x == s2.x) and np.all(s.a == s2.a)
```

### Comparing `ReplayTables-andnp-4.0.0/tests/test_ReplayBuffer.py` & `ReplayTables-andnp-4.0.1/tests/test_ReplayBuffer.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,32 @@
         assert buffer.size() == 5
 
         samples, _ = buffer.sample(1000)
         unique = np.unique(samples.a)
         unique.sort()
         assert np.all(unique == np.array([2, 3, 4, 5, 6]))
 
+    def test_terminal_states(self):
+        rng = np.random.default_rng(0)
+        buffer = ReplayBuffer(5, 1, rng)
+
+        for i in range(3):
+            d = fake_timestep(r=i)
+            buffer.add(d)
+
+        d = fake_timestep(x=np.ones(8), r=3, terminal=True)
+        buffer.add(d)
+
+        d = fake_timestep()
+        buffer.add(d)
+
+        samples, _ = buffer.sample(25)
+        assert np.all(samples.x == 0)
+        assert np.all(samples.xp[samples.terminal] == 0)
+
     def test_n_step(self):
         rng = np.random.default_rng(0)
         buffer = ReplayBuffer(5, 2, rng)
 
         d = fake_timestep(r=1, gamma=0.99)
         for _ in range(3):
             buffer.add(d)
```

### Comparing `ReplayTables-andnp-4.0.0/tests/test_Table.py` & `ReplayTables-andnp-4.0.1/tests/test_Table.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/tests/test_View.py` & `ReplayTables-andnp-4.0.1/tests/test_View.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/tests/test_integration.py` & `ReplayTables-andnp-4.0.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/tests/utils/test_MinMaxHeap.py` & `ReplayTables-andnp-4.0.1/tests/utils/test_MinMaxHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/tests/utils/test_SumTree.py` & `ReplayTables-andnp-4.0.1/tests/utils/test_SumTree.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-4.0.0/PKG-INFO` & `ReplayTables-andnp-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReplayTables-andnp
-Version: 4.0.0
+Version: 4.0.1
 Summary: A simple replay buffer implementation in python for sampling n-step trajectories
 License: MIT
 Author-email: Andy Patterson <andnpatterson@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # ReplayTables
```

