# Comparing `tmp/gay-1.2.8.tar.gz` & `tmp/gay-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gay-1.2.8.tar", last modified: Fri Jan 15 10:20:55 2021, max compression
+gzip compressed data, was "gay-1.2.9.tar", last modified: Fri Sep 30 04:54:32 2022, max compression
```

## Comparing `gay-1.2.8.tar` & `gay-1.2.9.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 10:20:55.184701 gay-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (116)     1606 2021-01-15 10:20:55.184701 gay-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      914 2021-01-15 10:20:06.000000 gay-1.2.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (116)    13728 2021-01-15 10:20:06.000000 gay-1.2.8/gay
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 10:20:55.180701 gay-1.2.8/gay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1606 2021-01-15 10:20:55.000000 gay-1.2.8/gay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      130 2021-01-15 10:20:55.000000 gay-1.2.8/gay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 10:20:55.000000 gay-1.2.8/gay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 10:20:55.000000 gay-1.2.8/gay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-15 10:20:55.184701 gay-1.2.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)      505 2021-01-15 10:20:06.000000 gay-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 04:54:32.913228 gay-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-30 04:54:08.000000 gay-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-09-30 04:54:32.913228 gay-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-09-30 04:54:08.000000 gay-1.2.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (121)    14399 2022-09-30 04:54:08.000000 gay-1.2.9/gay
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 04:54:32.913228 gay-1.2.9/gay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-09-30 04:54:32.000000 gay-1.2.9/gay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-09-30 04:54:32.000000 gay-1.2.9/gay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 04:54:32.000000 gay-1.2.9/gay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 04:54:32.000000 gay-1.2.9/gay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-30 04:54:32.913228 gay-1.2.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)      522 2022-09-30 04:54:08.000000 gay-1.2.9/setup.py
```

### Comparing `gay-1.2.8/PKG-INFO` & `gay-1.2.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 Metadata-Version: 2.1
 Name: gay
-Version: 1.2.8
+Version: 1.2.9
 Summary: Colour your text / terminal to be more gay. 🏳️‍🌈
 Home-page: https://github.com/ms-jpq/gay
 Author: ms-jpq
 Author-email: github@bigly.dog
-License: UNKNOWN
-Description: # [GAY 🏳️‍🌈](https://ms-jpq.github.io/gay)
-        
-        Colour your text / terminal to be more gay.
-        
-        Gayer version of [`lolcat`](https://github.com/busyloop/lolcat)
-        
-        ## [Get Gay](https://pypi.org/project/gay)
-        
-        `pip3 install -U gay`
-        
-        ## Show me
-        
-        ### Text
-        
-        ```sh
-        echo 'message' | gay
-        ```
-        
-        ![help.png](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/help.png)
-        
-        ```sh
-        -i 1d, --interpolation 1d
-        ```
-        
-        ![1d.png](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/1d.png)
-        
-        ```sh
-        -i 2d, --interpolation 2d
-        ```
-        
-        ![2d.png](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/2d.png)
-        
-        ### Flag
-        
-        ```sh
-        gay --flag
-        ```
-        
-        Unlike the demo, it shows 1 flag and 1 flag only.
-        
-        ![flags.gif](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/flags.gif)
-        
-        ## Thank yous
-        
-        [nshepperd](https://github.com/nshepperd) for helping with 2D gradient
-        
-        [wrennnnnn](https://github.com/wrennnnnn) for helping with windows
-        
-Platform: UNKNOWN
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# [GAY 🏳️‍🌈](https://ms-jpq.github.io/gay)
+
+Colour your text / terminal to be more gay.
+
+Gayer version of [`lolcat`](https://github.com/busyloop/lolcat)
+
+## [Get Gay](https://pypi.org/project/gay)
+
+`pip3 install -U gay`
+
+## Show me
+
+### Text
+
+```sh
+echo 'message' | gay
+```
+
+![help.png](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/help.png)
+
+```sh
+-i 1d, --interpolation 1d
+```
+
+![1d.png](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/1d.png)
+
+```sh
+-i 2d, --interpolation 2d
+```
+
+![2d.png](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/2d.png)
+
+### Flag
+
+```sh
+gay --flag
+```
+
+Unlike the demo, it shows 1 flag and 1 flag only.
+
+![flags.gif](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/flags.gif)
+
+## Thank yous
+
+[nshepperd](https://github.com/nshepperd) for helping with 2D gradient
+
+[wrennnnnn](https://github.com/wrennnnnn) for helping with windows
```

### Comparing `gay-1.2.8/README.md` & `gay-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `gay-1.2.8/gay` & `gay-1.2.9/gay`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #!/usr/bin/env python3
 
 from argparse import ArgumentParser, Namespace
-from atexit import register
+from contextlib import contextmanager
 from enum import Enum, auto
 from itertools import chain, count, cycle, islice, repeat
 from math import pi, sin
 from os import environ, linesep
 from os import name as os_name
 from random import choice, randint
 from shutil import get_terminal_size
-from sys import stdin
-from typing import Callable, Dict, Iterator, List, Optional, Tuple, cast
+from sys import stdin, stdout
+from typing import Callable, Iterator, Mapping, Optional, Sequence, Tuple, cast
 from unicodedata import east_asian_width
 
 
-class ColourSpace(Enum):
+class _ColourSpace(Enum):
     EIGHT = "8"
     TRUE = "24"
 
     def __str__(self) -> str:
-        return cast(str, self.value)
+        return self.value
 
 
-class Gradient(Enum):
+class _Gradient(Enum):
     D1 = "1d"
     D2 = "2d"
 
     def __str__(self) -> str:
-        return cast(str, self.value)
+        return self.value
 
 
-class Flags(Enum):
+class _Flags(Enum):
     LES = auto()
     GAY = auto()
     BI = auto()
     TRANS = auto()
     ACE = auto()
     PAN = auto()
     NB = auto()
@@ -48,482 +48,528 @@
     BIGENDER = auto()
     GENDERFLUID = auto()
     ABRO = auto()
     NEUTROIS = auto()
     TRIGENDER = auto()
 
 
-HexColour = str
-RGB = Tuple[int, int, int]
-RawPalette = List[HexColour]
-Palette = List[RGB]
+_HexColour = str
+_RGB = Tuple[int, int, int]
+_RawPalette = Sequence[_HexColour]
+_Palette = Sequence[_RGB]
 
-WINDOWS = os_name == "nt"
-COLS, ROWS = get_terminal_size((80, 80))
+_WINDOWS = os_name == "nt"
+_COLS, _ROWS = get_terminal_size((80, 80))
 
-UNICODE_WIDTH_LOOKUP = {
+_UNICODE_WIDTH_LOOKUP = {
     "W": 2,  # CJK
     "N": 0,  # Non printable
 }
 
-ASPECT_RATIO = (3, 5)
-FLAG_SPECS: Dict[Flags, RawPalette] = {
-    Flags.LES: ["#D62E02", "#FD9855", "#FFFFFF", "#D161A2", "#A20160"],
-    Flags.GAY: ["#FF0018", "#FFA52C", "#FFFF41", "#008018", "#0000F9", "#86007D"],
-    Flags.BI: ["#D60270", "#D60270", "#9B4F96", "#0038A8", "#0038A8"],
-    Flags.TRANS: ["#55CDFC", "#F7A8B8", "#FFFFFF", "#F7A8B8", "#55CDFC"],
-    Flags.ACE: ["#000000", "#A4A4A4", "#FFFFFF", "#810081"],
-    Flags.PAN: ["#FF1B8D", "#FFDA00", "#1BB3FF"],
-    Flags.NB: ["#FFF430", "#FFFFFF", "#9C59D1", "#000000"],
-    Flags.GQ: ["#B77FDD", "#FFFFFF", "#48821E"],
-    Flags.MLM: [
+_ASPECT_RATIO = (3, 5)
+_FLAG_SPECS: Mapping[_Flags, _RawPalette] = {
+    _Flags.LES: ["#D62E02", "#FD9855", "#FFFFFF", "#D161A2", "#A20160"],
+    _Flags.GAY: ["#FF0018", "#FFA52C", "#FFFF41", "#008018", "#0000F9", "#86007D"],
+    _Flags.BI: ["#D60270", "#D60270", "#9B4F96", "#0038A8", "#0038A8"],
+    _Flags.TRANS: ["#55CDFC", "#F7A8B8", "#FFFFFF", "#F7A8B8", "#55CDFC"],
+    _Flags.ACE: ["#000000", "#A4A4A4", "#FFFFFF", "#810081"],
+    _Flags.PAN: ["#FF1B8D", "#FFDA00", "#1BB3FF"],
+    _Flags.NB: ["#FFF430", "#FFFFFF", "#9C59D1", "#000000"],
+    _Flags.GQ: ["#B77FDD", "#FFFFFF", "#48821E"],
+    _Flags.MLM: [
         "#078D70",
         "#27CEAA",
         "#98E8C1",
         "#ffffff",
         "#7bade2",
         "#5049cc",
         "#3d1a78",
     ],
-    Flags.ARO: ["#3AA63F", "#A8D47A", "#FFFFFF", "#AAAAAA", "#000000"],
-    Flags.POLY: ["#F61BB9", "#07D669", "#1C92F5"],
-    Flags.DEMIBOY: ["#7F7F7F", "#C3C3C3", "#9AD9EA", "#FFFFFF", "#9AD9EA", "#C3C3C3", "#7F7F7F"],
-    Flags.DEMIGIRL: ["#7F7F7F", "#C3C3C3", "#FEAEC9", "#FFFFFF", "#FEAEC9", "#C3C3C3", "#7F7F7F"],
-    Flags.AGENDER: ["#000000", "#BCC5C6", "#FFFFFF", "#B5F582", "#FFFFFF", "#BCC5C6", "#000000"],
-    Flags.BIGENDER: ["#C479A0", "#ECA6CB", "#D5C7E8", "#FFFFFF", "#D5C7E8", "#9AC7E8", "#6C83CF"],
-    Flags.GENDERFLUID: ["#FE75A1", "#FFFFFF", "#BE18D6", "#000000", "#333EBC"],
-    Flags.ABRO: ["#75CA92", "#B2E4C5", "#FFFFFF", "#E695B5", "#DA446C"],
-    Flags.NEUTROIS: ["#FFFFFF", "#2F9C1D", "#000000"],
-    Flags.TRIGENDER: ["#FF95C5", "#9580FF", "#67D967", "#9580FF", "#FF95C5"]
+    _Flags.ARO: ["#3AA63F", "#A8D47A", "#FFFFFF", "#AAAAAA", "#000000"],
+    _Flags.POLY: ["#F61BB9", "#07D669", "#1C92F5"],
+    _Flags.DEMIBOY: [
+        "#7F7F7F",
+        "#C3C3C3",
+        "#9AD9EA",
+        "#FFFFFF",
+        "#9AD9EA",
+        "#C3C3C3",
+        "#7F7F7F",
+    ],
+    _Flags.DEMIGIRL: [
+        "#7F7F7F",
+        "#C3C3C3",
+        "#FEAEC9",
+        "#FFFFFF",
+        "#FEAEC9",
+        "#C3C3C3",
+        "#7F7F7F",
+    ],
+    _Flags.AGENDER: [
+        "#000000",
+        "#BCC5C6",
+        "#FFFFFF",
+        "#B5F582",
+        "#FFFFFF",
+        "#BCC5C6",
+        "#000000",
+    ],
+    _Flags.BIGENDER: [
+        "#C479A0",
+        "#ECA6CB",
+        "#D5C7E8",
+        "#FFFFFF",
+        "#D5C7E8",
+        "#9AC7E8",
+        "#6C83CF",
+    ],
+    _Flags.GENDERFLUID: ["#FE75A1", "#FFFFFF", "#BE18D6", "#000000", "#333EBC"],
+    _Flags.ABRO: ["#75CA92", "#B2E4C5", "#FFFFFF", "#E695B5", "#DA446C"],
+    _Flags.NEUTROIS: ["#FFFFFF", "#2F9C1D", "#000000"],
+    _Flags.TRIGENDER: ["#FF95C5", "#9580FF", "#67D967", "#9580FF", "#FF95C5"],
 }
 
 
-def parse_args() -> Namespace:
+def _parse_args() -> Namespace:
     colour_space = (
-        ColourSpace.TRUE
+        _ColourSpace.TRUE
         if environ.get("COLORTERM") in {"truecolor", "24bit"}
-        else ColourSpace.EIGHT
+        else _ColourSpace.EIGHT
     )
-    rand_flag = choice(tuple(Flags))
+    rand_flag = choice(tuple(_Flags))
     namespace = Namespace(flag=rand_flag)
     parser = ArgumentParser()
 
     mode_group = parser.add_argument_group()
     mode_group.add_argument("-f", "--flag", dest="flag_only", action="store_true")
 
     flag_group = parser.add_argument_group()
     flag_group.add_argument(
         "-l",
         "--les",
         "--lesbian",
         "--wlw",
         action="store_const",
         dest="flag",
-        const=Flags.LES,
+        const=_Flags.LES,
     )
     flag_group.add_argument(
         "-g",
         "--gay",
         action="store_const",
         dest="flag",
-        const=Flags.GAY,
+        const=_Flags.GAY,
     )
     flag_group.add_argument(
         "-b",
         "--bi",
         "--bisexual",
         action="store_const",
         dest="flag",
-        const=Flags.BI,
+        const=_Flags.BI,
     )
     flag_group.add_argument(
         "-t",
         "--trans",
         "--transgender",
         action="store_const",
         dest="flag",
-        const=Flags.TRANS,
+        const=_Flags.TRANS,
     )
     flag_group.add_argument(
         "-a",
         "--ace",
         "--asexual",
         action="store_const",
         dest="flag",
-        const=Flags.ACE,
+        const=_Flags.ACE,
     )
     flag_group.add_argument(
         "-p",
         "--pan",
         "--pansexual",
         action="store_const",
         dest="flag",
-        const=Flags.PAN,
+        const=_Flags.PAN,
     )
     flag_group.add_argument(
         "-n",
         "--nb",
         "--non-binary",
         action="store_const",
         dest="flag",
-        const=Flags.NB,
+        const=_Flags.NB,
     )
     flag_group.add_argument(
         "--gq",
         "--gender-queer",
         action="store_const",
         dest="flag",
-        const=Flags.GQ,
+        const=_Flags.GQ,
     )
     flag_group.add_argument(
         "--mlm",
         action="store_const",
         dest="flag",
-        const=Flags.MLM,
+        const=_Flags.MLM,
     )
     flag_group.add_argument(
         "--aro",
         "--aromantic",
         action="store_const",
         dest="flag",
-        const=Flags.ARO,
+        const=_Flags.ARO,
     )
     flag_group.add_argument(
         "--poly",
         "--polysexual",
         action="store_const",
         dest="flag",
-        const=Flags.POLY,
+        const=_Flags.POLY,
     )
     flag_group.add_argument(
         "--db",
         "--demiboy",
         action="store_const",
         dest="flag",
-        const=Flags.DEMIBOY,
+        const=_Flags.DEMIBOY,
     )
     flag_group.add_argument(
         "--dg",
         "--demigirl",
         action="store_const",
         dest="flag",
-        const=Flags.DEMIGIRL,
+        const=_Flags.DEMIGIRL,
     )
     flag_group.add_argument(
         "--ag",
         "--agender",
         action="store_const",
         dest="flag",
-        const=Flags.AGENDER,
+        const=_Flags.AGENDER,
     )
     flag_group.add_argument(
         "--bg",
         "--bigender",
         action="store_const",
         dest="flag",
-        const=Flags.BIGENDER,
+        const=_Flags.BIGENDER,
     )
     flag_group.add_argument(
         "--gf",
         "--genderfluid",
         action="store_const",
         dest="flag",
-        const=Flags.GENDERFLUID,
+        const=_Flags.GENDERFLUID,
     )
     flag_group.add_argument(
         "--abro",
         "--abrosexual",
         action="store_const",
         dest="flag",
-        const=Flags.ABRO,
+        const=_Flags.ABRO,
     )
     flag_group.add_argument(
         "--nt",
         "--neut",
         "--neutrois",
         action="store_const",
         dest="flag",
-        const=Flags.NEUTROIS,
+        const=_Flags.NEUTROIS,
     )
     flag_group.add_argument(
         "--tri",
         "--trigender",
         action="store_const",
         dest="flag",
-        const=Flags.TRIGENDER,
+        const=_Flags.TRIGENDER,
     )
 
     opt_group = parser.add_argument_group()
     opt_group.add_argument(
         "-c",
         "--colour",
-        type=ColourSpace,
-        choices=tuple(ColourSpace),
+        type=_ColourSpace,
+        choices=tuple(_ColourSpace),
         default=colour_space,
     )
     opt_group.add_argument(
         "-i",
         "--interpolation",
-        type=Gradient,
-        choices=tuple(Gradient),
-        default=choice(tuple(Gradient)),
+        type=_Gradient,
+        choices=tuple(_Gradient),
+        default=choice(tuple(_Gradient)),
     )
     opt_group.add_argument("--period", type=lambda i: max(abs(int(i)), 1))
     opt_group.add_argument(
         "--tabs", "--tab-width", type=lambda i: max(abs(int(i)), 1), default=4
     )
 
     return parser.parse_args(namespace=namespace)
 
 
-def trap_sig() -> None:
-    if not WINDOWS:
+def _trap_sig() -> None:
+    if not _WINDOWS:
         from signal import SIG_DFL, SIGPIPE, signal
 
         signal(SIGPIPE, SIG_DFL)
 
 
-def on_exit() -> None:
-    print("\033[0m", end="", flush=True)
-
-
-def stdin_stream() -> Iterator[str]:
+def _stdin_stream() -> Iterator[str]:
     while True:
-        size = COLS * 4
-        line = stdin.read(size)
+        line = stdin.read(696969)
         if line:
-            yield from iter(line)
+            yield from line
         else:
             break
 
 
-def normalize_width(tab_width: int, stream: Iterator[str]) -> Iterator[str]:
+def _normalize_width(tab_width: int, stream: Iterator[str]) -> Iterator[str]:
     for char in stream:
         if char == "\t":
             yield from repeat(" ", tab_width)
         else:
             yield char
 
 
-def unicode_width(stream: Iterator[str]) -> Iterator[Tuple[int, str]]:
+def _unicode_width(stream: Iterator[str]) -> Iterator[Tuple[int, str]]:
     def char_width(char: str) -> int:
         try:
             code = east_asian_width(char)
-            return UNICODE_WIDTH_LOOKUP.get(code, 1)
+            return _UNICODE_WIDTH_LOOKUP.get(code, 1)
         except Exception:
             return 1
 
     for char in stream:
         yield char_width(char), char
 
 
-def parse_raw_palette(raw: RawPalette) -> Palette:
-    def parse_colour(colour: HexColour) -> RGB:
+def _parse_raw_palette(raw: _RawPalette) -> _Palette:
+    def parse_colour(colour: _HexColour) -> _RGB:
         hexc = colour[1:]
         it = iter(hexc)
         parsed = tuple(
             int(f"{h1}{h2}", 16) for h1, h2 in iter(lambda: tuple(islice(it, 2)), ())
         )
-        return cast(RGB, parsed)
+        return cast(_RGB, parsed)
 
     return [parse_colour(p) for p in raw]
 
 
-DecorateChar = Callable[[RGB], Iterator[str]]
-DecorateReset = Callable[[], Iterator[str]]
+_DecorateChar = Callable[[_RGB], Iterator[str]]
+_DecorateReset = Callable[[], Iterator[str]]
 
 
-def decor_for(space: ColourSpace) -> Tuple[DecorateChar, DecorateChar, DecorateReset]:
+def _decor_for(
+    space: _ColourSpace,
+) -> Tuple[_DecorateChar, _DecorateChar, _DecorateReset]:
     def reset() -> Iterator[str]:
-        yield "\033[0m"
+        yield "\x1B[0m"
 
-    def decor_8(rgb: RGB) -> Iterator[str]:
+    def decor_8(rgb: _RGB) -> Iterator[str]:
         r, g, b = map(lambda c: int(round(c / 255 * 5)), rgb)
         yield ";"
         yield str(16 + 36 * r + 6 * g + b)
 
-    def decor_24(rgb: RGB) -> Iterator[str]:
+    def decor_24(rgb: _RGB) -> Iterator[str]:
         yield from chain(*zip(repeat(";"), map(str, rgb)))
 
-    if space == ColourSpace.EIGHT:
+    if space == _ColourSpace.EIGHT:
 
-        def fg(colour: RGB) -> Iterator[str]:
-            yield "\033[38;5"
+        def fg(colour: _RGB) -> Iterator[str]:
+            yield "\x1B[38;5"
             yield from decor_8(colour)
             yield "m"
 
-        def bg(colour: RGB) -> Iterator[str]:
-            yield "\033[48;5"
+        def bg(colour: _RGB) -> Iterator[str]:
+            yield "\x1B[48;5"
             yield from decor_8(colour)
             yield "m"
 
         return fg, bg, reset
-    elif space == ColourSpace.TRUE:
+    elif space == _ColourSpace.TRUE:
 
-        def fg(colour: RGB) -> Iterator[str]:
-            yield "\033[38;2"
+        def fg(colour: _RGB) -> Iterator[str]:
+            yield "\x1B[38;2"
             yield from decor_24(colour)
             yield "m"
 
-        def bg(colour: RGB) -> Iterator[str]:
-            yield "\033[48;2"
+        def bg(colour: _RGB) -> Iterator[str]:
+            yield "\x1B[48;2"
             yield from decor_24(colour)
             yield "m"
 
         return fg, bg, reset
     else:
         raise ValueError()
 
 
-def paint_flag(colour_space: ColourSpace, palette: Palette) -> Iterator[str]:
-    r, c = ASPECT_RATIO
-    _, bg, reset = decor_for(colour_space)
+def _paint_flag(colour_space: _ColourSpace, palette: _Palette) -> Iterator[str]:
+    r, c = _ASPECT_RATIO
+    _, bg, reset = _decor_for(colour_space)
     height = len(palette)
     ratio = r / c * 0.5
-    multiplier = max(int(min((ROWS - 4) / height, COLS / height * ratio)), 1)
-    line = " " * COLS
+    multiplier = max(int(min((_ROWS - 4) / height, _COLS / height * ratio)), 1)
+    line = " " * _COLS
     for colour in palette:
         for _ in range(multiplier):
             yield from bg(colour)
             yield line
             yield from reset()
             yield linesep
 
 
-def enumerate_lines(stream: Iterator[str]) -> Iterator[Tuple[bool, int, str]]:
+def _enumerate_lines(stream: Iterator[str]) -> Iterator[Tuple[bool, int, str]]:
 
-    l_stream = unicode_width(stream)
+    l_stream = _unicode_width(stream)
     prev: Optional[Tuple[int, str]] = next(l_stream, None)
     x = 0 if prev is None else 1
 
     def drain(ret: bool) -> Iterator[Tuple[bool, int, str]]:
         nonlocal prev
         if prev is not None:
             yield (ret, *prev)
             prev = None
 
     for width, char in l_stream:
         new = x + width
-        if new > COLS:
+        if new > _COLS:
             yield from drain(True)
             prev = (width, char)
             x = width
-        elif new == COLS or char == linesep:
+        elif new == _COLS or char == linesep:
             yield from drain(False)
             yield True, width, char
             x = 0
         else:
             yield from drain(False)
             prev = (width, char)
             x = new
 
     yield from drain(False)
 
 
-def lerp(c1: RGB, c2: RGB, mix: float) -> RGB:
+def _lerp(c1: _RGB, c2: _RGB, mix: float) -> _RGB:
     lhs = map(lambda c: c * mix, c1)
     rhs = map(lambda c: c * (1 - mix), c2)
     new = map(lambda c: int(round(sum(c))), zip(lhs, rhs))
-    return cast(RGB, tuple(new))
+    return cast(_RGB, tuple(new))
 
 
-def sine_wave(t: float) -> float:
+def _sine_wave(t: float) -> float:
     period = pi * pi
     x = t * period
     return (sin(x / pi + pi / 2) + 1) / 2
 
 
-def interpolate_1d(palette: Palette, rep: int) -> Iterator[Iterator[RGB]]:
+def _interpolate_1d(palette: _Palette, rep: int) -> Iterator[Iterator[_RGB]]:
     colours = cycle(palette)
 
-    def once() -> Iterator[RGB]:
+    def once() -> Iterator[_RGB]:
         prev = next(colours)
         while True:
             curr = next(colours)
             for t in range(rep + 1):
-                mix = sine_wave(t / rep)
-                yield lerp(prev, curr, mix)
+                mix = _sine_wave(t / rep)
+                yield _lerp(prev, curr, mix)
             prev = curr
 
     yield from repeat(once())
 
 
 # contributed by https://github.com/nshepperd
 # https://github.com/ms-jpq/gay/issues/2
-def interpolate_2d(palette: Palette, rep: int) -> Iterator[Iterator[RGB]]:
+def _interpolate_2d(palette: _Palette, rep: int) -> Iterator[Iterator[_RGB]]:
     num = len(palette)
 
     for y in count():
 
-        def line() -> Iterator[RGB]:
+        def line() -> Iterator[_RGB]:
             for x in count():
                 p = (x + 1.5 * y) / rep
                 i = int(p)
                 prev = palette[i % num]
                 curr = palette[(i + 1) % num]
-                mix = sine_wave(p - i)
-                yield lerp(prev, curr, mix)
+                mix = _sine_wave(p - i)
+                yield _lerp(prev, curr, mix)
 
         yield line()
 
 
-def interpolation_for(
-    mode: Gradient, palette: Palette, rep: Optional[int]
-) -> Iterator[Iterator[RGB]]:
-    if mode == Gradient.D1:
+def _interpolation_for(
+    mode: _Gradient, palette: _Palette, rep: Optional[int]
+) -> Iterator[Iterator[_RGB]]:
+    if mode == _Gradient.D1:
         period = rep or randint(10, 20)
-        return interpolate_1d(palette, period)
-    if mode == Gradient.D2:
+        return _interpolate_1d(palette, period)
+    if mode == _Gradient.D2:
         period = rep or randint(10, 15)
-        return interpolate_2d(palette, period)
+        return _interpolate_2d(palette, period)
     else:
         raise ValueError()
 
 
-def colourize(
-    colour_space: ColourSpace,
-    rgb_gen: Iterator[Iterator[RGB]],
+def _colourize(
+    colour_space: _ColourSpace,
+    rgb_gen: Iterator[Iterator[_RGB]],
     stream: Iterator[str],
 ) -> Iterator[str]:
-    fg, _, reset = decor_for(colour_space)
+    fg, _, reset = _decor_for(colour_space)
     colour_gen = next(rgb_gen)
-    for new_line, width, char in enumerate_lines(stream):
+    for new_line, width, char in _enumerate_lines(stream):
         if width:
             colour = next(colour_gen)
             yield from fg(colour)
         yield char
         if new_line:
             yield from reset()
             colour_gen = next(rgb_gen)
 
 
-def main() -> None:
-    trap_sig()
-    args = parse_args()
-    register(on_exit)
-    palette = parse_raw_palette(FLAG_SPECS[args.flag])
-
-    if args.flag_only:
-        flag_stripes = paint_flag(colour_space=args.colour, palette=palette)
-        print(*flag_stripes, sep="", end="")
-    else:
-        stream = stdin_stream()
-        normalized_stream = normalize_width(args.tabs, stream)
+@contextmanager
+def _title() -> Iterator[None]:
+    def cont(title: str) -> None:
+        stdout.write("\x1B[0m")
+        if "TMUX" in environ:
+            stdout.write(f"\x1Bk{title}\x1B\\")
+        else:
+            stdout.write(f"\x1B]0;{title}\x1B\\")
 
-        rgb_gen = interpolation_for(
-            mode=args.interpolation, palette=palette, rep=args.period
-        )
-        gen = colourize(
-            colour_space=args.colour,
-            rgb_gen=rgb_gen,
-            stream=normalized_stream,
-        )
-        for chunk in iter(lambda: tuple(islice(gen, COLS)), ()):
-            print(*chunk, sep="", end="")
+        stdout.flush()
+
+    cont("GAY")
+    try:
+        yield None
+    finally:
+        cont("")
+
+
+def _main() -> None:
+    with _title():
+        _trap_sig()
+        args = _parse_args()
+        palette = _parse_raw_palette(_FLAG_SPECS[args.flag])
+
+        if args.flag_only:
+            flag_stripes = _paint_flag(colour_space=args.colour, palette=palette)
+            stdout.writelines(flag_stripes)
+        else:
+            stream = _stdin_stream()
+            normalized_stream = _normalize_width(args.tabs, stream)
+
+            rgb_gen = _interpolation_for(
+                mode=args.interpolation, palette=palette, rep=args.period
+            )
+            gen = _colourize(
+                colour_space=args.colour,
+                rgb_gen=rgb_gen,
+                stream=normalized_stream,
+            )
+            stdout.writelines(gen)
 
 
 try:
-    main()
+    _main()
 except KeyboardInterrupt:
     exit(130)
 except BrokenPipeError:
     exit(13)
```

### Comparing `gay-1.2.8/gay.egg-info/PKG-INFO` & `gay-1.2.9/gay.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 Metadata-Version: 2.1
 Name: gay
-Version: 1.2.8
+Version: 1.2.9
 Summary: Colour your text / terminal to be more gay. 🏳️‍🌈
 Home-page: https://github.com/ms-jpq/gay
 Author: ms-jpq
 Author-email: github@bigly.dog
-License: UNKNOWN
-Description: # [GAY 🏳️‍🌈](https://ms-jpq.github.io/gay)
-        
-        Colour your text / terminal to be more gay.
-        
-        Gayer version of [`lolcat`](https://github.com/busyloop/lolcat)
-        
-        ## [Get Gay](https://pypi.org/project/gay)
-        
-        `pip3 install -U gay`
-        
-        ## Show me
-        
-        ### Text
-        
-        ```sh
-        echo 'message' | gay
-        ```
-        
-        ![help.png](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/help.png)
-        
-        ```sh
-        -i 1d, --interpolation 1d
-        ```
-        
-        ![1d.png](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/1d.png)
-        
-        ```sh
-        -i 2d, --interpolation 2d
-        ```
-        
-        ![2d.png](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/2d.png)
-        
-        ### Flag
-        
-        ```sh
-        gay --flag
-        ```
-        
-        Unlike the demo, it shows 1 flag and 1 flag only.
-        
-        ![flags.gif](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/flags.gif)
-        
-        ## Thank yous
-        
-        [nshepperd](https://github.com/nshepperd) for helping with 2D gradient
-        
-        [wrennnnnn](https://github.com/wrennnnnn) for helping with windows
-        
-Platform: UNKNOWN
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# [GAY 🏳️‍🌈](https://ms-jpq.github.io/gay)
+
+Colour your text / terminal to be more gay.
+
+Gayer version of [`lolcat`](https://github.com/busyloop/lolcat)
+
+## [Get Gay](https://pypi.org/project/gay)
+
+`pip3 install -U gay`
+
+## Show me
+
+### Text
+
+```sh
+echo 'message' | gay
+```
+
+![help.png](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/help.png)
+
+```sh
+-i 1d, --interpolation 1d
+```
+
+![1d.png](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/1d.png)
+
+```sh
+-i 2d, --interpolation 2d
+```
+
+![2d.png](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/2d.png)
+
+### Flag
+
+```sh
+gay --flag
+```
+
+Unlike the demo, it shows 1 flag and 1 flag only.
+
+![flags.gif](https://raw.githubusercontent.com/ms-jpq/gay/%3C3/preview/flags.gif)
+
+## Thank yous
+
+[nshepperd](https://github.com/nshepperd) for helping with 2D gradient
+
+[wrennnnnn](https://github.com/wrennnnnn) for helping with windows
```

