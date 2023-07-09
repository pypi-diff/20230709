# Comparing `tmp/kfst-1.1.1.tar.gz` & `tmp/kfst-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfst-1.1.1.tar", last modified: Fri Jul  7 10:32:48 2023, max compression
+gzip compressed data, was "kfst-1.2.0.tar", last modified: Sun Jul  9 20:11:19 2023, max compression
```

## Comparing `kfst-1.1.1.tar` & `kfst-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:32:48.381470 kfst-1.1.1/
--rw-r--r--   0 iikka      (501) staff       (20)     7653 2023-07-05 12:46:55.000000 kfst-1.1.1/LICENSE
--rw-r--r--   0 iikka      (501) staff       (20)     2040 2023-07-07 10:32:48.381527 kfst-1.1.1/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)     1456 2023-07-06 13:42:57.000000 kfst-1.1.1/README.md
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:32:48.380401 kfst-1.1.1/kfst/
--rw-r--r--   0 iikka      (501) staff       (20)      742 2023-07-05 14:15:18.000000 kfst-1.1.1/kfst/__init__.py
--rw-r--r--   0 iikka      (501) staff       (20)     1211 2023-07-07 10:30:22.000000 kfst-1.1.1/kfst/convert.py
--rw-r--r--   0 iikka      (501) staff       (20)    17216 2023-07-07 10:26:55.000000 kfst-1.1.1/kfst/transducer.py
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 10:32:48.381333 kfst-1.1.1/kfst.egg-info/
--rw-r--r--   0 iikka      (501) staff       (20)     2040 2023-07-07 10:32:48.000000 kfst-1.1.1/kfst.egg-info/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)      233 2023-07-07 10:32:48.000000 kfst-1.1.1/kfst.egg-info/SOURCES.txt
--rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-07 10:32:48.000000 kfst-1.1.1/kfst.egg-info/dependency_links.txt
--rw-r--r--   0 iikka      (501) staff       (20)       11 2023-07-07 10:32:48.000000 kfst-1.1.1/kfst.egg-info/requires.txt
--rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-07 10:32:48.000000 kfst-1.1.1/kfst.egg-info/top_level.txt
--rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:15.000000 kfst-1.1.1/pyproject.toml
--rw-r--r--   0 iikka      (501) staff       (20)      708 2023-07-07 10:32:48.381769 kfst-1.1.1/setup.cfg
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-09 20:11:19.436770 kfst-1.2.0/
+-rw-r--r--   0 iikka      (501) staff       (20)     7653 2023-07-05 12:46:55.000000 kfst-1.2.0/LICENSE
+-rw-r--r--   0 iikka      (501) staff       (20)     2040 2023-07-09 20:11:19.436819 kfst-1.2.0/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)     1456 2023-07-06 13:42:57.000000 kfst-1.2.0/README.md
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-09 20:11:19.435833 kfst-1.2.0/kfst/
+-rw-r--r--   0 iikka      (501) staff       (20)      742 2023-07-05 14:15:18.000000 kfst-1.2.0/kfst/__init__.py
+-rw-r--r--   0 iikka      (501) staff       (20)     1211 2023-07-07 10:30:22.000000 kfst-1.2.0/kfst/convert.py
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-09 20:11:19.436648 kfst-1.2.0/kfst/format/
+-rw-r--r--   0 iikka      (501) staff       (20)     1139 2023-07-09 19:39:38.000000 kfst-1.2.0/kfst/format/att.py
+-rw-r--r--   0 iikka      (501) staff       (20)     4223 2023-07-09 19:37:41.000000 kfst-1.2.0/kfst/format/kfst.py
+-rw-r--r--   0 iikka      (501) staff       (20)    12749 2023-07-09 20:09:03.000000 kfst-1.2.0/kfst/transducer.py
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-09 20:11:19.436394 kfst-1.2.0/kfst.egg-info/
+-rw-r--r--   0 iikka      (501) staff       (20)     2040 2023-07-09 20:11:19.000000 kfst-1.2.0/kfst.egg-info/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)      272 2023-07-09 20:11:19.000000 kfst-1.2.0/kfst.egg-info/SOURCES.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-09 20:11:19.000000 kfst-1.2.0/kfst.egg-info/dependency_links.txt
+-rw-r--r--   0 iikka      (501) staff       (20)       11 2023-07-09 20:11:19.000000 kfst-1.2.0/kfst.egg-info/requires.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-09 20:11:19.000000 kfst-1.2.0/kfst.egg-info/top_level.txt
+-rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:15.000000 kfst-1.2.0/pyproject.toml
+-rw-r--r--   0 iikka      (501) staff       (20)      723 2023-07-09 20:11:19.437029 kfst-1.2.0/setup.cfg
```

### Comparing `kfst-1.1.1/LICENSE` & `kfst-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kfst-1.1.1/PKG-INFO` & `kfst-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfst
-Version: 1.1.1
+Version: 1.2.0
 Summary: A pure-python finite state transducer library
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU LGPLv3 or later
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `kfst-1.1.1/README.md` & `kfst-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kfst-1.1.1/kfst/__init__.py` & `kfst-1.2.0/kfst/__init__.py`

 * *Files identical despite different names*

### Comparing `kfst-1.1.1/kfst/convert.py` & `kfst-1.2.0/kfst/convert.py`

 * *Files identical despite different names*

### Comparing `kfst-1.1.1/kfst/transducer.py` & `kfst-1.2.0/kfst/transducer.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,20 +14,16 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with KFST. If not, see <https://www.gnu.org/licenses/>. 
 
 from __future__ import annotations
 
 import argparse
-import lzma
-import re
-import struct
-from collections import defaultdict
 from pathlib import Path
-from typing import NamedTuple
+from typing import Mapping, NamedTuple
 
 from frozendict import frozendict
 
 
 class FSTState(NamedTuple):
     state_num: int
     path_weight: float = 0
@@ -39,20 +35,32 @@
         return f"FSTState({self.state_num}, {self.path_weight}, {self.input_flags}, {self.output_flags}, {self.output_symbols})"
 
 
 class FST(NamedTuple):
     """
     Represents a finite state transducer
     """
-    final_states: dict[int, float]
-    rules: defaultdict[int, defaultdict[str, list[tuple[int, str, float]]]]
-    symbols: set[str]
+    final_states: Mapping[int, float]
+    rules: Mapping[int, Mapping[str, list[tuple[int, str, float]]]]
+    symbols: list[str] # Must be sorted in reverse order by length
     debug: bool = False
 
     @staticmethod
+    def from_rules(
+        final_states: Mapping[int, float],
+        rules: Mapping[int, Mapping[str, list[tuple[int, str, float]]]],
+        symbols: set[str],
+        debug: bool = False,
+    ):
+        """
+        Creates an FST from a dictionary of final states, a dictionary of rules and a set of symbols.
+        """
+        return FST(final_states, rules, sorted(symbols, key=lambda s: -len(s)), debug=debug)
+
+    @staticmethod
     def from_att_file(att_file: str | Path, debug: bool = False) -> "FST":
         """
         Parses a transducer in A&AT format and returns an FST object.
         The input must be the path to the .att file.
 
         If you already have the content of the .att file, use FST.from_att_code() instead.
 
@@ -72,42 +80,15 @@
         """
         Parses a transducer in A&AT format and returns an FST object.
         
         Note that the input must be the content of the .att file, not the path to the file.
         For that, use FST.from_att_file() instead.
         """
 
-        fst = FST(
-            final_states={},
-            rules=defaultdict(lambda: defaultdict(list)),
-            symbols=set(),
-            debug=debug,
-        )
-        for line in att_code.splitlines():
-            fields = line.split("\t")
-            if len(fields) == 1:
-                fst.final_states[int(fields[0])] = 0
-            
-            elif len(fields) == 2:
-                fst.final_states[int(fields[0])] = float(fields[1])
-
-            elif len(fields) == 4:
-                fst.rules[int(fields[0])][fields[2]].append((int(fields[1]), fields[3], 0))
-                fst.symbols.add(fields[2])
-                fst.symbols.add(fields[3])
-
-            elif len(fields) == 5:
-                fst.rules[int(fields[0])][fields[2]].append((int(fields[1]), fields[3], float(fields[4])))
-                fst.symbols.add(fields[2])
-                fst.symbols.add(fields[3])
-
-            else:
-                raise RuntimeError("Cannot parse line:", line)
-
-        return fst
+        return decode_att(att_code)._replace(debug=debug)
 
     @staticmethod
     def from_kfst_file(kfst_file: str | Path, debug: bool = False) -> "FST":
         """
         Parses a transducer in the KFST binary format and returns an FST object.
         The input must be the path to the .kfst file.
 
@@ -129,25 +110,15 @@
         """
         Parses a transducer in the KFST binary format and returns an FST object.
 
         Note that the input must be the content of the .kfst file, not the path to the file.
         For that, use FST.from_kfst_file() instead.
         """
 
-        fst = FST(
-            final_states={},
-            rules=defaultdict(lambda: defaultdict(list)),
-            symbols=set(),
-            debug=debug,
-        )
-
-        reader = KFSTReader(kfst_bytes)
-        reader.read_into(fst)
-        
-        return fst
+        return decode_kfst(kfst_bytes)._replace(debug=debug)
 
     def to_kfst_file(self, path: str | Path):
         """
         Encodes the FST in the KFST binary format and writes it to the given path.
         """
         if not isinstance(path, Path):
             path = Path(path)
@@ -155,64 +126,30 @@
         path.write_bytes(self.to_kfst_bytes())
         
     def to_kfst_bytes(self) -> bytes:
         """
         Encodes the FST in the KFST binary format.
         """
 
-        is_weighted = any(weight != 0 for weight in self.final_states.values()) or any(weight != 0 for state in self.rules.values() for transitions in state.values() for _, _, weight in transitions)
-
-        assert len(self.symbols) <= 2**16, "Too many symbols"
-
-        num_rules = sum(len(transitions) for state in self.rules.values() for transitions in state.values())
-
-        assert num_rules <= 2**32, "Too many rules"
-        assert len(self.final_states) <= 2**32, "Too many final states"
-
-        buffer = bytes()
-        buffer += b"KFST"
-        buffer += struct.pack("!H", 0) # version
-        buffer += struct.pack("!HII?", len(self.symbols), num_rules, len(self.final_states), is_weighted) # header
-
-        # Write symbols
-        symbols_list = sorted(self.symbols)
-        for symbol in symbols_list:
-            buffer += symbol.encode("utf-8") + b"\x00"
-
-        state_bytes = []
-        
-        # Write states
-        for from_state, transitions in self.rules.items():
-            for input_symbol, transitions_list in transitions.items():
-                for to_state, output_symbol, weight in transitions_list:
-                    state_bytes.append(struct.pack("!IIHH", from_state, to_state, symbols_list.index(input_symbol), symbols_list.index(output_symbol)))
-                    if is_weighted:
-                        state_bytes.append(struct.pack("!d", weight))
-        
-        # Write final states
-        for state, weight in self.final_states.items():
-            state_bytes.append(struct.pack("!I", state))
-            if is_weighted:
-                state_bytes.append(struct.pack("!d", weight))
-        
-        data = b"".join(state_bytes)
-        buffer += lzma.compress(data)
-        return buffer
+        return encode_kfst(self)
 
     def split_to_symbols(self, text: str) -> list[str] | None:
         """
         Splits a given string into a list of symbols.
         For each position in the string, greedily selects the longest symbol that matches.
 
         Returns None if the string cannot be split into symbols.
         """
-        slist = sorted(self.symbols, key=lambda x: -len(x))
+        
+        # Symbols are assumed to be sorted in a reverse order by length
+        # See FST.from_rules() implementation
+
         ans = []
         while text:
-            for s in slist:
+            for s in self.symbols:
                 if text.startswith(s):
                     ans.append(s)
                     text = text[len(s):]
                     break
 
             else:
                 return None
@@ -291,81 +228,78 @@
             o = "".join(os)
             if o not in already_seen:
                 yield o, w
                 already_seen.add(o)
     
     def _update_flags(self, symbol: str, flags: frozendict[str, str]) -> frozendict[str, str] | None:
         if self._is_flag(symbol):
+            # Parse flag
+            # Two params: @<flag type>.<flag key>.<flag value>@
+            # One param: @<flag type>.<flag key>@
+            flag = symbol[1]
+            di = symbol.rindex(".")
+            key = symbol[3:di] if di > 3 else symbol[3:-1]
+            value = symbol[di+1:-1] if di > 3 else None
             # unification flag
-            if m := re.fullmatch(r"@U.([^@.]*).([^@.]*)@", symbol):
-                key = m.group(1)
-                value = m.group(2)
+            if flag == "U":
+                assert value is not None
                 if key in flags and flags[key] != value and (not flags[key].startswith("@") or flags[key] == "@" + value):
                     return None # flag mismatch
 
                 else:
                     return flags.set(key, value)
             
             # require flag (2 params)
-            elif m := re.fullmatch(r"@R.([^@.]*).([^@.]*)@", symbol):
-                key = m.group(1)
-                value = m.group(2)
+            elif flag == "R" and value is not None:
                 if key in flags and self._test_flag(flags[key], value):
                     return flags
 
                 else:
                     return None
             
             # require flag (1 param)
-            elif m := re.fullmatch(r"@R.([^@.]*)@", symbol):
-                key = m.group(1)
+            elif flag == "R" and value is None:
                 if key in flags:
                     return flags
 
                 else:
                     return None
             
             # disallow flag (2 params)
-            elif m := re.fullmatch(r"@D.([^@.]*).([^@.]*)@", symbol):
-                key = m.group(1)
-                value = m.group(2)
+            elif flag == "D" and value is not None:
                 if key in flags and self._test_flag(flags[key], value):
                     return None
 
                 else:
                     return flags
             
             # disallow flag (1 param)
-            elif m := re.fullmatch(r"@D.([^@.]*)@", symbol):
-                key = m.group(1)
+            elif flag == "D" and value is None:
                 if key in flags:
                     return None
 
                 else:
                     return flags
             
             # clear flag
-            elif m := re.fullmatch(r"@C.([^@.]*)@", symbol):
-                key = m.group(1)
+            elif flag == "C":
                 if key in flags:
                     return flags.delete(key)
 
                 else:
                     return flags
             
             # positive (re)setting flag (2 params)
-            elif m := re.fullmatch(r"@P.([^@.]*).([^@.]*)@", symbol):
-                key = m.group(1)
-                value = m.group(2)
+            elif flag == "P":
+                assert value is not None
                 return flags.set(key, value)
             
             # negative (re)setting flag (2 params)
-            elif m := re.fullmatch(r"@N.([^@.]*).([^@.]*)@", symbol):
-                key = m.group(1)
-                value = m.group(2)
+            elif flag == "N":
+                assert value is not None
                 return flags.set(key, "@" + value)
         
         return flags
 
     def _test_flag(self, stored_val: str, queried_val: str):
         if stored_val == queried_val:
             return True
@@ -376,78 +310,18 @@
         return False
 
     def _is_epsilon(self, symbol: str) -> bool:
         # flag diacritics are treated like epsilon symbols
         return symbol == "@0@" or symbol == "@_EPSILON_SYMBOL_@" or self._is_flag(symbol)
     
     def _is_flag(self, symbol: str) -> bool:
-        return bool(re.match(r"^@[PNDRCU]\.", symbol))
-
-
-class KFSTReader:
-
-    def __init__(self, buffer):
-        self.buffer = buffer
-        self.pointer = 0
-
-    def read_into(self, fst: FST):
-        # Validate signature
-        assert self.buffer[:4] == b"KFST"
-        self.pointer += 4
-
-        # Parse version
-        (version,) = self.unpack_and_advance("!H")
-
-        assert version == 0, "Unsupported KFST binary file version"
-
-        # Parse header
-        num_symbols, num_states, num_final_states, is_weighted = self.unpack_and_advance("!HII?")
-
-        # Parse symbols
-        symbols_list = []
-        for _ in range(num_symbols):
-            symbol = self.read_null_terminated_string()
-            symbol_string = symbol.decode("utf-8")
-            fst.symbols.add(symbol_string)
-            symbols_list.append(symbol_string)
-        
-        lzma_data = self.buffer[self.pointer:]
-        self.buffer = lzma.decompress(lzma_data)
-        self.pointer = 0
-        
-        # Parse states
-        for _ in range(num_states):
-            from_state, to_state, input_symbol, output_symbol = self.unpack_and_advance("!IIHH")
-            weight = 0
-
-            if is_weighted:
-                (weight,) = self.unpack_and_advance("!d")
-
-            fst.rules[from_state][symbols_list[input_symbol]].append((to_state, symbols_list[output_symbol], weight))
-        
-        # Parse final states
-        for _ in range(num_final_states):
-            (state,) = self.unpack_and_advance("!I")
-            weight = 0
-            if is_weighted:
-                (weight,) = self.unpack_and_advance("!d")
-            
-            fst.final_states[state] = weight
-
-    def unpack_and_advance(self, format: str):
-        size = struct.calcsize(format)
-        ans = struct.unpack(format, self.buffer[self.pointer:self.pointer+size])
-        self.pointer += size
-        return ans
+        return len(symbol) > 4 and symbol[0] == "@" and symbol[-1] == "@" and symbol[1] in "PNDRCU" and symbol[2] == "."
 
-    def read_null_terminated_string(self) -> bytes:
-        i = self.buffer[self.pointer:].find(b"\x00")
-        string = self.buffer[self.pointer:self.pointer+i]
-        self.pointer += i + 1
-        return string
+from .format.att import decode_att
+from .format.kfst import decode_kfst, encode_kfst
 
 
 def main():
     parser = argparse.ArgumentParser(description="Finite State Transducer interpreter written in Python")
     parser.add_argument("fst_file", type=Path, help="FST in AT&T or KFST format")
     parser.add_argument("-d", action="store_true", help="enable debug mode")
     parser.add_argument("-s", action="store_true", help="print symbols in transducer and exit")
```

### Comparing `kfst-1.1.1/kfst.egg-info/PKG-INFO` & `kfst-1.2.0/kfst.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfst
-Version: 1.1.1
+Version: 1.2.0
 Summary: A pure-python finite state transducer library
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU LGPLv3 or later
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

