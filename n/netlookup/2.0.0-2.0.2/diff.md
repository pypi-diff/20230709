# Comparing `tmp/netlookup-2.0.0.tar.gz` & `tmp/netlookup-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlookup-2.0.0.tar", max compression
+gzip compressed data, was "netlookup-2.0.2.tar", max compression
```

## Comparing `netlookup-2.0.0.tar` & `netlookup-2.0.2.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     2405 2020-03-04 16:36:37.000000 netlookup-2.0.0/LICENSE
--rw-r--r--   0        0        0     4387 2022-12-02 13:39:20.589744 netlookup-2.0.0/README.md
--rw-r--r--   0        0        0       50 2022-03-13 06:12:30.533694 netlookup-2.0.0/netlookup/__init__.py
--rw-r--r--   0        0        0     1742 2022-11-30 07:46:17.342810 netlookup-2.0.0/netlookup/base.py
--rw-r--r--   0        0        0        0 2019-06-09 16:58:46.000000 netlookup-2.0.0/netlookup/bin/__init__.py
--rw-r--r--   0        0        0        0 2019-06-09 16:58:59.000000 netlookup-2.0.0/netlookup/bin/commands/__init__.py
--rw-r--r--   0        0        0      966 2022-11-30 07:46:17.349021 netlookup-2.0.0/netlookup/bin/commands/base.py
--rw-r--r--   0        0        0     1483 2020-04-23 03:36:02.000000 netlookup-2.0.0/netlookup/bin/commands/info.py
--rw-r--r--   0        0        0     1910 2022-11-30 07:46:17.352270 netlookup-2.0.0/netlookup/bin/commands/prefixes.py
--rw-r--r--   0        0        0     1027 2022-11-30 07:46:17.354927 netlookup-2.0.0/netlookup/bin/commands/split.py
--rw-r--r--   0        0        0     1402 2022-03-13 06:21:26.849710 netlookup-2.0.0/netlookup/bin/commands/substract.py
--rw-r--r--   0        0        0      465 2022-11-30 07:46:17.358375 netlookup-2.0.0/netlookup/bin/netlookup.py
--rw-r--r--   0        0        0      226 2022-12-05 07:03:04.182242 netlookup-2.0.0/netlookup/constants.py
--rw-r--r--   0        0        0      577 2023-01-02 06:28:58.036159 netlookup-2.0.0/netlookup/encoders.py
--rw-r--r--   0        0        0      129 2023-01-02 06:31:00.128430 netlookup-2.0.0/netlookup/exceptions.py
--rw-r--r--   0        0        0     6456 2022-11-30 07:46:17.370550 netlookup-2.0.0/netlookup/network.py
--rw-r--r--   0        0        0        0 2019-06-09 16:58:40.000000 netlookup-2.0.0/netlookup/network_sets/__init__.py
--rw-r--r--   0        0        0     2707 2022-11-30 07:46:17.374062 netlookup-2.0.0/netlookup/network_sets/aws.py
--rw-r--r--   0        0        0     6146 2022-11-30 07:46:17.377338 netlookup-2.0.0/netlookup/network_sets/base.py
--rw-r--r--   0        0        0     2004 2022-11-30 07:46:17.380713 netlookup-2.0.0/netlookup/network_sets/cloudflare.py
--rw-r--r--   0        0        0      154 2022-11-30 07:46:17.383903 netlookup-2.0.0/netlookup/network_sets/constants.py
--rw-r--r--   0        0        0     3179 2022-11-30 07:46:17.388175 netlookup-2.0.0/netlookup/network_sets/google.py
--rw-r--r--   0        0        0     2693 2022-11-30 07:46:17.395396 netlookup-2.0.0/netlookup/prefixes.py
--rw-r--r--   0        0        0     1175 2022-11-30 07:46:17.400562 netlookup-2.0.0/netlookup/protocols.py
--rw-r--r--   0        0        0     2047 2022-11-30 07:46:17.404076 netlookup-2.0.0/netlookup/services.py
--rw-r--r--   0        0        0     1032 2023-01-02 06:35:07.378791 netlookup-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5433 1970-01-01 00:00:00.000000 netlookup-2.0.0/setup.py
--rw-r--r--   0        0        0     5350 1970-01-01 00:00:00.000000 netlookup-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-03-09 21:01:59.883089 netlookup-2.0.2/LICENSE
+-rw-r--r--   0        0        0     4387 2022-12-02 13:39:20.589744 netlookup-2.0.2/README.md
+-rw-r--r--   0        0        0      153 2023-03-09 20:55:42.171065 netlookup-2.0.2/netlookup/__init__.py
+-rw-r--r--   0        0        0     1872 2023-03-09 21:18:31.264879 netlookup-2.0.2/netlookup/base.py
+-rw-r--r--   0        0        0      141 2023-03-09 20:56:25.588887 netlookup-2.0.2/netlookup/bin/__init__.py
+-rw-r--r--   0        0        0      146 2023-03-09 20:56:20.369656 netlookup-2.0.2/netlookup/bin/commands/__init__.py
+-rw-r--r--   0        0        0     1413 2023-03-09 20:55:17.277608 netlookup-2.0.2/netlookup/bin/commands/base.py
+-rw-r--r--   0        0        0     1719 2023-03-09 20:48:42.507691 netlookup-2.0.2/netlookup/bin/commands/info.py
+-rw-r--r--   0        0        0     2227 2023-03-09 20:55:35.465234 netlookup-2.0.2/netlookup/bin/commands/prefixes.py
+-rw-r--r--   0        0        0     1477 2023-03-09 20:52:34.833877 netlookup-2.0.2/netlookup/bin/commands/split.py
+-rw-r--r--   0        0        0     1753 2023-03-09 20:54:05.842225 netlookup-2.0.2/netlookup/bin/commands/substract.py
+-rw-r--r--   0        0        0      608 2023-03-09 20:56:39.612011 netlookup-2.0.2/netlookup/bin/netlookup.py
+-rw-r--r--   0        0        0      329 2023-03-09 20:58:13.851611 netlookup-2.0.2/netlookup/constants.py
+-rw-r--r--   0        0        0      680 2023-03-09 20:58:18.045373 netlookup-2.0.2/netlookup/encoders.py
+-rw-r--r--   0        0        0      232 2023-03-09 20:58:21.059421 netlookup-2.0.2/netlookup/exceptions.py
+-rw-r--r--   0        0        0     7020 2023-03-09 21:30:25.407086 netlookup-2.0.2/netlookup/network.py
+-rw-r--r--   0        0        0      166 2023-03-09 20:57:31.029492 netlookup-2.0.2/netlookup/network_sets/__init__.py
+-rw-r--r--   0        0        0     3034 2023-03-09 21:06:43.442453 netlookup-2.0.2/netlookup/network_sets/aws.py
+-rw-r--r--   0        0        0     6685 2023-03-09 21:17:32.261300 netlookup-2.0.2/netlookup/network_sets/base.py
+-rw-r--r--   0        0        0     2117 2023-03-09 21:14:29.113536 netlookup-2.0.2/netlookup/network_sets/cloudflare.py
+-rw-r--r--   0        0        0      257 2023-03-09 20:58:00.673929 netlookup-2.0.2/netlookup/network_sets/constants.py
+-rw-r--r--   0        0        0     3324 2023-03-09 21:15:31.737961 netlookup-2.0.2/netlookup/network_sets/google.py
+-rw-r--r--   0        0        0     3065 2023-03-09 21:25:47.321195 netlookup-2.0.2/netlookup/prefixes.py
+-rw-r--r--   0        0        0     1342 2023-03-09 21:27:36.860349 netlookup-2.0.2/netlookup/protocols.py
+-rw-r--r--   0        0        0     2237 2023-03-09 21:27:03.618342 netlookup-2.0.2/netlookup/services.py
+-rw-r--r--   0        0        0     1137 2023-07-09 03:01:56.903582 netlookup-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 netlookup-2.0.2/PKG-INFO
```

### Comparing `netlookup-2.0.0/README.md` & `netlookup-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `netlookup-2.0.0/netlookup/base.py` & `netlookup-2.0.2/netlookup/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 Common base classes for network info text file parsers
 """
 import re
 from collections.abc import Sequence
 from pathlib import Path
-from typing import Any, List
+from typing import Any, Iterator, List
 
 
 def match_patterns(patterns: List[re.Pattern], line: str) -> dict:
     """
     Parse fields in line with patterns
     """
     line = line.rstrip()
@@ -43,15 +48,15 @@
 
     def __init__(self, path: str) -> None:
         self.__items__ = self.__load__(Path(path))
 
     def __getitem__(self, index: int):
         return self.__items__.__getitem__(index)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Any]:
         return iter(self.__items__)
 
     def __len__(self) -> int:
         return len(self.__items__)
 
     def __load__(self, path: Path) -> List[Any]:
         """
```

### Comparing `netlookup-2.0.0/netlookup/bin/commands/base.py` & `netlookup-2.0.2/netlookup/bin/commands/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,44 @@
-
-from cli_toolkit.command import Command
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
+"""
+Common base command for netlookup CLI commands
+"""
+from argparse import Namespace
+from typing import Any, List, Optional
+from cli_toolkit.command import Command, NestedCliCommand
 
 from ...network import Network
 
 
 class BaseCommand(Command):
     """
     Netlookup base command
     """
-    networks = []
+    networks: List[Network] = []
 
-    def __init__(self, parent, usage=None, description=None, epilog=None):
+    def __init__(self,
+                 parent: NestedCliCommand,
+                 usage: Optional[str] = None,
+                 description: Optional[str] = None,
+                 epilog: Optional[str] = None):
         super().__init__(parent, usage, description, epilog)
         self.errors = []
 
-    def error(self, *args) -> None:
+    def error(self, *args: List[Any]) -> None:
         """
         Add error to self.errors and send it to parent class method
         """
         self.errors.append(f'{self.__parse_string_args__(*args)}')
         super().error(*args)
 
-    def parse_args(self, args=None, namespace=None):
+    def parse_args(self, args: Namespace = None, namespace: Namespace = None) -> Namespace:
         """
         Parse common arguments for netlookup commands
         """
         self.networks = []
         for subnet in getattr(args, 'subnets', []):
             try:
                 self.networks.append(Network(subnet))
```

### Comparing `netlookup-2.0.0/netlookup/bin/commands/info.py` & `netlookup-2.0.2/netlookup/bin/commands/info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,29 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
+"""
+CLI command 'netlookup info'
+"""
+from argparse import ArgumentParser, Namespace
 
+from ...network import Network
 from .base import BaseCommand
 
 
 class Info(BaseCommand):
     """
     Command for function for 'netlookup info' CLI command
     """
-
     name = 'info'
     help = 'Show subnet info'
 
-    def print_network_details(self, network):
+    def print_network_details(self, network: Network):
         """
         Show details for specified network
         """
         first = network.first_host
         last = network.last_host
         self.message(f'         CIDR {network.cidr}')
         self.message(f'      Netmask {network.netmask}')
@@ -27,16 +36,16 @@
             self.message(f'    Last host {network.last_host}')
         self.message(f'  Total hosts {network.total_hosts}')
         self.message(f'         Next {network.next()}')  # noqa
         self.message(f'     Previous {network.previous()}')
         self.message(f'         Bits {network.network.bits()}')
         self.message(f'  Reverse DNS {network.network.reverse_dns}')
 
-    def register_parser_arguments(self, parser):
+    def register_parser_arguments(self, parser: ArgumentParser):
         parser.add_argument('subnets', nargs='*', help='Subnets to process')
 
-    def run(self, args):  # pylint: disable=W0613
+    def run(self, args: Namespace) -> None:
         if not args.subnets:
             self.exit(1, 'No subnets specified')
 
         for network in self.networks:
             self.print_network_details(network)
```

### Comparing `netlookup-2.0.0/netlookup/bin/commands/prefixes.py` & `netlookup-2.0.2/netlookup/bin/commands/prefixes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,37 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 CLI command 'netlookup prefixes'
 """
+from argparse import ArgumentParser, Namespace
 from typing import List, Optional
+
 from ...prefixes import Prefixes
 from .base import BaseCommand
 
 
 class PrefixLookup(BaseCommand):
     """
     Command for function for 'netlookup prefixes' CLI command
     """
-    name = 'prefixes'
-    short_description = 'Lookup prefixes'
+    name: str = 'prefixes'
+    short_description: str = 'Lookup prefixes'
     __prefixes__: Optional[Prefixes] = None
 
-    def register_parser_arguments(self, parser):
+    def register_parser_arguments(self, parser: ArgumentParser) -> ArgumentParser:
+        """
+        Register address list arguments and update flags
+        """
         parser.add_argument('-u', '--update', action='store_true', help='Update prefix cache')
         parser.add_argument('addresses', nargs='*', help='Prefixes to lookup')
+        return parser
 
     @property
     def prefixes(self) -> Prefixes:
         """
         Return  a cached Prefixes object
         """
         if self.__prefixes__ is None:
@@ -45,15 +56,15 @@
             try:
                 address = self.prefixes.find(address)
                 if address:
                     self.message(address)
             except Exception as error:
                 self.error(f'Error looking up address "{address}": {error}')
 
-    def run(self, args):
+    def run(self, args: Namespace) -> None:
         """
         Run 'netlookup prefixes' command
         """
         if not args.update and not args.addresses:
             self.exit(1, 'No prefixes specified')
         if args.update:
             self.update_prefix_cache()
```

### Comparing `netlookup-2.0.0/netlookup/bin/commands/substract.py` & `netlookup-2.0.2/netlookup/bin/commands/substract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,60 @@
-
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
+"""
+CLI utility to split a network from another
+"""
+from argparse import ArgumentParser, Namespace
 from netlookup.network import NetworkError
 from netlookup.network_sets.base import NetworkSet
 
 from .base import BaseCommand
 
 
 class Subtract(BaseCommand):
     """
     Command for function for 'netlookup substract' CLI command
     """
+    name: str = 'subtract'
+    short_description: str = 'Substract subnet from specified subnets'
 
-    name = 'subtract'
-    short_description = 'Substract subnet from specified subnets'
-
-    def register_parser_arguments(self, parser):
+    def register_parser_arguments(self, parser: ArgumentParser) -> ArgumentParser:
         """
         Register arguments for subtracted networks
         """
         parser.add_argument(
             '-n', '--networks',
             action='append',
             required=True,
             help='Subnets to subtract'
         )
         parser.add_argument(
             'subnets',
             nargs='*',
             help='Subnets to subtract from'
         )
+        return parser
 
-    def parse_args(self, args=None, namespace=None):
+    def parse_args(self, args: Namespace = None, namespace: Namespace = None) -> Namespace:
         """
         Parse subnet arguments
         """
         args.networks = [
             network
             for arg in args.networks
             for network in arg.split(',')
         ]
         return args
 
-    def run(self, args):
+    def run(self, args: Namespace) -> None:
         """
-        Substract subnets
+        Substract subnets and print the split ranges
         """
         if not args.subnets:
             self.exit(1, 'No subnets specified')
 
         try:
             networks = NetworkSet(networks=args.subnets).substract(args.networks)
         except NetworkError as error:
```

### Comparing `netlookup-2.0.0/netlookup/encoders.py` & `netlookup-2.0.2/netlookup/encoders.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 Data format encoders
 """
 from typing import Any
 
 from netaddr.ip import IPAddress, IPNetwork, IPRange
```

### Comparing `netlookup-2.0.0/netlookup/network.py` & `netlookup-2.0.2/netlookup/network.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,26 @@
-
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
+"""
+Extensions to netaddr objects as networks
+"""
 from bisect import bisect_left
-from typing import Optional
+from typing import Any, List, Optional, Union
 
 from netaddr.ip import IPNetwork, IPAddress
 from netaddr.core import AddrFormatError
 
 from .constants import IPV4_VERSION, IPV6_VERSION, MAX_PREFIX_LEN_IPV4, MAX_PREFIX_LEN_IPV6
 from .exceptions import NetworkError
 
 
-def find_address_in_networks(networks, value):
+def find_address_in_networks(networks: List['Network'], value: Any) -> Optional['Network']:
     """
     Find given address in networks
     """
     address = parse_address_or_network(value)
     next_address = bisect_left(networks, address)
     if next_address > 0:
         try:
@@ -30,15 +37,15 @@
     for network in networks:
         if address.value == network.value:
             return network
 
     return None
 
 
-def parse_address_or_network(value):
+def parse_address_or_network(value: Any) -> Union[IPAddress, 'Network']:
     """
     Parse value as IPAddress or Network
     """
     if isinstance(value, (IPAddress, Network)):
         return value
     try:
         return IPAddress(value)
@@ -50,60 +57,60 @@
         raise NetworkError(f'Error parsing address or network from {value}') from error
 
 
 class NetworkList(list):
     """
     Base class for a list of networks
     """
-    def clear(self):
+    def clear(self) -> None:
         del self[:len(self)]
 
 
 class Network(IPNetwork):
     """
     Extend IPNetwork with some custom attributes
     """
-    def __eq__(self, other):
+    def __eq__(self, other: Union[str, IPAddress, 'Network']) -> bool:
         if isinstance(other, str):
             other = parse_address_or_network(other)
         if isinstance(other, Network):
             return self.value == other.value and self.prefixlen == other.prefixlen
         if isinstance(other, IPAddress):
             return self.value == other.value
         return self.value == other
 
-    def __ne__(self, other):
+    def __ne__(self, other: Union[str, IPAddress, 'Network']) -> bool:
         return not self.__eq__(other)
 
-    def __lt__(self, other):
+    def __lt__(self, other: Union[str, IPAddress, 'Network']) -> bool:
         if isinstance(other, str):
             return str(self.cidr) < other
         if isinstance(other, (Network, IPAddress)):
             return self.value < other.value
         return self.value < other
 
-    def __le__(self, other):
+    def __le__(self, other: Union[str, IPAddress, 'Network']) -> bool:
         if isinstance(other, str):
             return str(self.cidr) <= other
         if isinstance(other, (Network, IPAddress)):
             return self.value <= other.value
         return self.value <= other
 
-    def __gt__(self, other):
+    def __gt__(self, other: Union[str, IPAddress, 'Network']) -> bool:
         if isinstance(other, (Network, IPAddress)):
             return self.last > other.value
         return self.value > other
 
-    def __ge__(self, other):
+    def __ge__(self, other: Union[str, IPAddress, 'Network']) -> bool:
         if isinstance(other, (Network, IPAddress)):
             return self.value >= other.value
         return self.value >= other
 
     @property
-    def total_hosts(self):
+    def total_hosts(self) -> int:
         """
         Return total number of available hosts in subnet, excluding network and
         broadcast addresses
         """
         if self.version == IPV4_VERSION:
             if self.prefixlen == MAX_PREFIX_LEN_IPV4 - 1:
                 return 2
@@ -113,15 +120,15 @@
             if self.prefixlen == MAX_PREFIX_LEN_IPV6 - 1:
                 return 2
             if self.prefixlen == MAX_PREFIX_LEN_IPV6:
                 return 1
         return self.size - 2
 
     @property
-    def first_host(self):
+    def first_host(self) -> Optional[IPAddress]:
         """
         Return first available host in network, excluding network address
         """
         if self.version == IPV4_VERSION:
             if self.prefixlen == MAX_PREFIX_LEN_IPV4 - 1:
                 return IPAddress(self.first)
             if self.prefixlen == MAX_PREFIX_LEN_IPV4:
@@ -130,15 +137,15 @@
             if self.prefixlen == MAX_PREFIX_LEN_IPV6 - 1:
                 return IPAddress(self.first)
             if self.prefixlen == MAX_PREFIX_LEN_IPV6:
                 return None
         return IPAddress(self.first + 1)
 
     @property
-    def last_host(self):
+    def last_host(self) -> Optional[IPAddress]:
         """
         Return last available host in network, excluding broadcast address
         """
         if self.version == IPV4_VERSION:
             if self.prefixlen == MAX_PREFIX_LEN_IPV4 - 1:
                 return IPAddress(self.last)
             if self.prefixlen == MAX_PREFIX_LEN_IPV4:
```

### Comparing `netlookup-2.0.0/netlookup/network_sets/aws.py` & `netlookup-2.0.2/netlookup/network_sets/aws.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,65 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 AWS address prefix set
 """
 import json
 
 from datetime import datetime
 from http import HTTPStatus
 from operator import attrgetter
+from typing import List, Optional, Tuple, TYPE_CHECKING
 
 import requests
 
 from ..exceptions import NetworkError
 from .base import NetworkSet, NetworkSetItem
 from .constants import REQUEST_TIMEOUT
 
+if TYPE_CHECKING:
+    from ..network import Network
+
 AWS_IP_RANGES_URL = 'https://ip-ranges.amazonaws.com/ip-ranges.json'
 SKIP_SERVICE_NAMES = (
     'AMAZON',
 )
 
 
 class AWSPrefix(NetworkSetItem):
     """
     AWS network prefix with region and service details
     """
-    type = 'aws'
-    extra_attributes = ('region', 'services')
+    type: str = 'aws'
+    network: 'Network'
+    region: Optional[str]
+    extra_attributes: Tuple[str] = ('region', 'services')
 
-    def __init__(self, network, data=None):
+    def __init__(self, network: 'Network', data: dict = None):
         self.region = None
         self.services = []
         super().__init__(network, data)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'{self.type} {self.region} {self.cidr}'
 
 
 class AWS(NetworkSet):
     """
     AWS address networks
     """
-    type = 'aws'
-    cache_filename = 'aws-networks.json'
+    type: str = 'aws'
+    cache_filename: str = 'aws-networks.json'
     loader_class = AWSPrefix
 
     @property
-    def regions(self):
+    def regions(self) -> List[str]:
         """
         Return all detected regions
         """
         return sorted(set(prefix.region for prefix in self))
 
     @staticmethod
     def __get_aws_ip_ranges__() -> str:
```

### Comparing `netlookup-2.0.0/netlookup/network_sets/base.py` & `netlookup-2.0.2/netlookup/network_sets/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,49 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 Base class for network set class
 """
 import json
 
 from datetime import datetime
 from pathlib import Path
-from typing import Optional
+from typing import Any, Dict, Iterator, List, Optional, Tuple
 
 from netaddr.core import AddrFormatError
 from netaddr.ip.sets import IPSet
 
 from ..network import Network, NetworkList, NetworkError, find_address_in_networks
 
 
 class NetworkSetItem(Network):
     """
     Named network prefix for specific vendor and service
     """
-    type = 'generic'
-    extra_attributes = []
+    type: str = 'generic'
+    network: Network
+    extra_attributes: Tuple[str] = ()
 
-    def __init__(self, network, data=None):
+    def __init__(self, network: Network, data=None):
         super().__init__(network)
         if data is not None:
             for attr in self.extra_attributes:
                 if attr in data:
                     setattr(self, attr, data[attr])
 
     def __repr__(self) -> str:
         return f'{self.type} {self.cidr}'
 
     def __str__(self) -> str:
         return self.__repr__()
 
-    def as_dict(self):
+    def as_dict(self) -> Dict[str, Any]:
         """
         Format prefix object as dictionary
 
         Extend in child class to get prefix type specific data
         """
         data = {
             'type': self.type,
@@ -48,36 +54,42 @@
         return data
 
 
 class NetworkSet:
     """
     Common base class for network address prefix sets with caching
     """
-    type = 'generic'
-    cache_filename = None
+    type: str = 'generic'
+    cache_directory: Optional[str]
+    cache_filename: Optional[str] = None
+    updated: Optional[str]
+    __networks__: NetworkList
+    __iter_index__: Optional[int]
     loader_class = NetworkSetItem
 
-    def __init__(self, networks=None, cache_directory=None) -> None:
+    def __init__(self,
+                 networks: Optional[List[Network]] = None,
+                 cache_directory: Optional[str] = None) -> None:
         self.cache_directory = cache_directory
         self.updated = None
         self.__networks__ = NetworkList()
         self.__iter_index__ = None
 
         self.load()
         if networks is not None:
             for network in networks:
                 self.add_network(network)
 
     def __len__(self) -> int:
         return len(self.__networks__)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Network]:
         return self
 
-    def __next__(self):
+    def __next__(self) -> Network:
         if not self.__networks__:
             self.fetch()
         if self.__iter_index__ is None:
             self.__iter_index__ = 0
         try:
             item = self.__networks__[self.__iter_index__]
             self.__iter_index__ += 1
@@ -99,61 +111,63 @@
     def ipset(self) -> IPSet:
         """
         IPSet of networks in network set
         """
         return IPSet([item.cidr for item in self.__networks__])
 
     @property
-    def merged(self):
+    def merged(self) -> 'NetworkSet':
         """
         Minimal merged set of IP range set covering network set
         """
-        return self.__class__(networks=[self.loader_class(network) for network in self.ipset.iter_cidrs()])
+        return self.__class__(
+            networks=[self.loader_class(network) for network in self.ipset.iter_cidrs()]
+        )
 
-    def fetch(self):
+    def fetch(self) -> None:
         """
         Fetch information for network
         """
         raise NotImplementedError('fetch() must be implemented in child class')
 
     def as_dict(self) -> dict:
         """
         Return all networks as dictionary
         """
         return {
             'updated': self.updated.isoformat() if self.updated else None,
             'networks': [prefix.as_dict() for prefix in self.__networks__]
         }
 
-    def add_network(self, value) -> None:
+    def add_network(self, value: Any) -> None:
         """
         Add network to cache
         """
         try:
             network = self.loader_class(value)
         except Exception as error:
             raise NetworkError(f'Error parsing network {value}: {error}') from error
         if network not in self.__networks__:
             self.__networks__.append(network)
 
-    def substract(self, networks) -> None:
+    def substract(self, networks: List[Network]) -> 'NetworkSet':
         """
         Return merged network set, with specified network removed
         """
         ipset = self.ipset
         if isinstance(networks, str):
             networks = [networks]
         for network in networks:
             try:
                 ipset.remove(network)
             except AddrFormatError as error:
                 raise NetworkError(f'Error processing network {network}: {error}') from error
         return self.__class__(networks=[self.loader_class(network) for network in ipset.iter_cidrs()])
 
-    def __read_cache_file__(self):
+    def __read_cache_file__(self) -> str:
         """
         Read network set data cache file
         """
         try:
             with self.cache_file.open('r', encoding='utf-8') as filedescriptor:
                 return filedescriptor.read()
         except Exception as error:
```

### Comparing `netlookup-2.0.0/netlookup/network_sets/cloudflare.py` & `netlookup-2.0.2/netlookup/network_sets/cloudflare.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 Network set of cloudflare IP address ranges
 """
 from datetime import datetime
 from http import HTTPStatus
 from operator import attrgetter
 from typing import List
@@ -27,16 +32,16 @@
     type = 'cloudflare'
 
 
 class Cloudflare(NetworkSet):
     """
     Network Set for cloudflare public addresses
     """
-    type = 'cloudflare'
-    cache_filename = 'cloudflare-networks.json'
+    type: str = 'cloudflare'
+    cache_filename: str = 'cloudflare-networks.json'
     loader_class = CloudflarePrefix
 
     def __get_ip_range_data__(self, url: str) -> List[str]:
         """
         Cloudflare IP range data is available as text files from static URLs
         """
         try:
```

### Comparing `netlookup-2.0.0/netlookup/network_sets/google.py` & `netlookup-2.0.2/netlookup/network_sets/google.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 Google services address prefix set
 """
 import re
 
 from datetime import datetime
 from operator import attrgetter
@@ -62,15 +67,15 @@
 
 
 class GoogleNetworkSet(NetworkSet):
     """
     Google network set with data for TXT DNS records
     """
     @property
-    def __address_list_record__(self):
+    def __address_list_record__(self) -> None:
         raise NotImplementedError
 
     def fetch(self) -> None:
         """
         Fetch Google Cloud network records from DNS
         """
         self.__networks__.clear()
@@ -88,34 +93,34 @@
     type = 'google-cloud'
 
 
 class GoogleCloud(GoogleNetworkSet):
     """
     Google Cloud address ranges
     """
-    type = 'google-cloud'
-    cache_filename = 'google-cloud-networks.json'
+    type: str = 'google-cloud'
+    cache_filename: str = 'google-cloud-networks.json'
     loader_class = GoogleCloudPrefix
 
     @property
-    def __address_list_record__(self):
+    def __address_list_record__(self) -> str:
         return GOOGLE_CLOUD_ADDRESS_LIST_RECORD
 
 
 class GoogleServicePrefix(NetworkSetItem):
     """
     Google services network prefix
     """
     type = 'google'
 
 
 class GoogleServices(GoogleNetworkSet):
     """
     Google services address ranges
     """
-    type = 'google'
-    cache_filename = 'google-service-networks.json'
+    type: str = 'google'
+    cache_filename: str = 'google-service-networks.json'
     loader_class = GoogleServicePrefix
 
     @property
-    def __address_list_record__(self):
+    def __address_list_record__(self) -> str:
         return GOOGLE_SERVICES_ADDRESS_LIST_RECORD
```

### Comparing `netlookup-2.0.0/netlookup/prefixes.py` & `netlookup-2.0.2/netlookup/prefixes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,35 @@
-
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
+"""
+Network prefix cache objects
+"""
 from operator import attrgetter
 from pathlib import Path
+from typing import Any, List, Optional, Union
 
-from .network import NetworkList, NetworkError, find_address_in_networks
+from .network import Network, NetworkList, NetworkError, find_address_in_networks
+from .network_sets.base import NetworkSet
 from .network_sets.constants import DEFAULT_CACHE_DIRECTORY
 from .network_sets.aws import AWS
 from .network_sets.cloudflare import Cloudflare
 from .network_sets.google import GoogleCloud, GoogleServices
 
 
 class Prefixes(NetworkList):
     """
     Loader and lookup for known IP address prefix caches for public clouds
     """
-    def __init__(self, cache_directory=None) -> None:
+    cache_directory: Path
+    vendors: List[NetworkSet]
+
+    def __init__(self, cache_directory: Optional[Union[str, Path]] = None) -> None:
         super().__init__()
         cache_directory = cache_directory if cache_directory is not None else DEFAULT_CACHE_DIRECTORY
         self.cache_directory = Path(cache_directory).expanduser()
 
         if not self.cache_directory.exists():
             try:
                 self.cache_directory.mkdir(parents=True)
@@ -26,15 +38,14 @@
 
         self.vendors = [
             AWS(cache_directory=self.cache_directory),
             Cloudflare(cache_directory=self.cache_directory),
             GoogleCloud(cache_directory=self.cache_directory),
             GoogleServices(cache_directory=self.cache_directory),
         ]
-
         self.load()
 
     def update(self) -> None:
         """
         Fetch and update cached prefix data
         """
         for vendor in self.vendors:
@@ -60,27 +71,27 @@
         for vendor in self.vendors:
             vendor.load()
             # Go directly to attribute, iterating vendor may trigger fetch
             for prefix in vendor.__networks__:
                 self.append(prefix)
         self.sort(key=attrgetter('value'))
 
-    def filter_type(self, value):
+    def filter_type(self, value: Any):
         """
         Filter networks by type
         """
         return [prefix for prefix in self if prefix.type == value]
 
-    def get_vendor(self, name):
+    def get_vendor(self, name: str) -> NetworkSet:
         """
         Get vendor prefix set
         """
         for vendor in self.vendors:
             if vendor.type == name:
                 return vendor
         raise NetworkError(f'No such vendor: {name}')
 
-    def find(self, value):
+    def find(self, value: Any) -> Optional[Network]:
         """
         Find address in networks
         """
         return find_address_in_networks(self, value)
```

### Comparing `netlookup-2.0.0/netlookup/protocols.py` & `netlookup-2.0.2/netlookup/protocols.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 Parser for /etc/protocols file
 """
 import re
 from typing import List, Optional
 
 from .base import FileItem, NetworkDataTextFile
@@ -14,14 +19,18 @@
 )
 
 
 class Protocol(FileItem):
     """
     Single protocol in the protocols file
     """
+    name: str
+    number: str
+    aliases: str
+    comment: str
     __patterns__: List[re.Pattern] = PROTOCOL_LINE_PATTERNS
 
     def __init__(self,
                  name: str,
                  number: str,
                  aliases: str = '',
                  comment: str = '') -> None:
```

### Comparing `netlookup-2.0.0/netlookup/services.py` & `netlookup-2.0.2/netlookup/services.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+#
+# Copyright (C) 2020-2023 by Ilkka Tuohela <hile@iki.fi>
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 """
 Parser for /etc/services file
 """
 import re
 
 from typing import List, Optional
 
@@ -41,14 +46,19 @@
 )
 
 
 class Service(FileItem):
     """
     Single service in the services file
     """
+    port_number: str
+    protocol: str
+    name: str
+    aliases: str
+    comment: str
     __patterns__: List[re.Pattern] = SERVICE_LINE_PATTERNS
 
     def __init__(self,
                  port_number: str,
                  protocol: str,
                  name: str = '',
                  aliases: str = '',
```

### Comparing `netlookup-2.0.0/pyproject.toml` & `netlookup-2.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "netlookup"
-version = "2.0.0"
+version = "2.0.2"
 description = "Python tools to look up information about networks"
 authors = ["Ilkka Tuohela <hile@iki.fi>"]
+homepage = "https://github.com/hile/netlookup"
 readme = "README.md"
 include = [
     "LICENSE",
 ]
-license = "BSD"
+license = "BSD-3-Clause"
 classifiers = [
     "Environment :: Console",
     "License :: OSI Approved :: BSD License",
     "Operating System :: MacOS",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Programming Language :: Python :: 3.9",
@@ -34,14 +35,18 @@
 pycodestyle = "^2"
 pyflakes = "^3"
 pylint = "^2"
 pytest = "^7"
 requests-mock = "^1"
 tox = "^4"
 ipython = "^8.7.0"
+ruff = "^0.0.261"
 
 [tool.poetry.scripts]
 netlookup = "netlookup.bin.netlookup:main"
 
+[tool.ruff]
+line-length = 120
+
 [build-system]
-requires = ["poetry-core>=1.3.2"]
+requires = ["poetry-core>=1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `netlookup-2.0.0/setup.py` & `netlookup-2.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,191 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: netlookup
+Version: 2.0.2
+Summary: Python tools to look up information about networks
+Home-page: https://github.com/hile/netlookup
+License: BSD-3-Clause
+Author: Ilkka Tuohela
+Author-email: hile@iki.fi
+Requires-Python: >=3.9,<4.0
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Dist: cli-toolkit (>=2,<3)
+Requires-Dist: dnspython (>=2,<3)
+Requires-Dist: netaddr (>=0.8,<0.9)
+Requires-Dist: requests (>=2,<3)
+Description-Content-Type: text/markdown
+
+![Unit Tests](https://github.com/hile/netlookup/actions/workflows/unittest.yml/badge.svg)
+![Style Checks](https://github.com/hile/netlookup/actions/workflows/lint.yml/badge.svg)
+
+# Command line network lookups and operations
+
+This python tool implements pretty much same things as `netcalc` and `netblocks` libraries, but
+with minor differences in the way things are done.
+
+The library is intended to be usable both as a command line tool `netlookup` and as a library from
+server code. Personally I use it for splitting IP ranges to subnets.
+
+## Installing
+
+```bash
+pip install netlookup
+```
+
+# Command line tool `netlookup` basic usage
+
+Following examples illustrate Usage of netlookup tool.
+
+Lookup details for IPv4 host with CIDR mask and IPv6 subnet:
+
+```bash
+netlookup info 172.31.1.19/17 2c0f:fb50:4000::/56
+             CIDR 172.31.0.0/17
+          Netmask 255.255.128.0
+          Network 172.31.0.0
+        Broadcast 172.31.127.255
+       First host 172.31.0.1
+        Last host 172.31.127.254
+      Total hosts 32766
+             Next 172.31.128.0/17
+         Previous 172.30.128.0/17
+             Bits 10101100.00011111.00000000.00000000
+      Reverse DNS 0.0.31.172.in-addr.arpa.
+             CIDR 2c0f:fb50:4000::/56
+          Netmask ffff:ffff:ffff:ff00::
+          Network 2c0f:fb50:4000::
+        Broadcast 2c0f:fb50:4000:ff:ffff:ffff:ffff:ffff
+       First host 2c0f:fb50:4000::1
+        Last host 2c0f:fb50:4000:ff:ffff:ffff:ffff:fffe
+      Total hosts 4722366482869645213694
+             Next 2c0f:fb50:4000:100::/56
+         Previous 2c0f:fb50:3fff:ff00::/56
+             Bits 0010110000001111:1111101101010000:0100000000000000:0000000000000000:0000000000000000:0000000000000000:0000000000000000:0000000000000000
+      Reverse DNS 0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.4.0.5.b.f.f.0.c.2.ip6.arpa.
+```
+
+Split subnet with defaults (to next smaller subnet / larger prefix):
+
+```bash
+netlookup split 172.31.1.19/17 2c0f:fb50:4000::/56
+    172.31.0.0/18
+    172.31.64.0/18
+    2c0f:fb50:4000::/57
+    2c0f:fb50:4000:80::/57
+```
+
+Split IPv4 subnets with specific prefix:
+
+```bash
+netlookup split --mask 19 172.31.1.19/17 172.31.5.39/17
+    172.31.0.0/19
+    172.31.32.0/19
+    172.31.64.0/19
+    172.31.96.0/19
+    172.31.0.0/19
+    172.31.32.0/19
+    172.31.64.0/19
+    172.31.96.0/19
+```
+
+Using the python library
+------------------------
+
+Some practical examples for using the API where a CLI command is not yet available.
+
+Create set of networks and show minimal merged CIDR prefixes to cover this range:
+
+```python
+from netlookup.network_sets.base import NetworkSet
+ns = NetworkSet()
+ns.add_network('172.31.0.0/23')
+ns.add_network('172.31.4.0/22')
+ns.add_network('172.31.8.0/24')
+ns.add_network('172.31.9.0/25')
+ns.add_network('172.31.9.128/25')
+print('\n'.join(str(x.cidr) for x in ns.merged))
+```
+
+Previous example returns
+
+```bash
+172.31.0.0/23
+172.31.4.0/22
+172.31.8.0/23
+```
+
+Using same example, remove one /29 from the result set
+
+```python
+from netlookup.network_sets.base import NetworkSet
+ns = NetworkSet()
+ns.add_network('172.31.0.0/23')
+ns.add_network('172.31.4.0/22')
+ns.add_network('172.31.8.0/24')
+ns.add_network('172.31.9.0/25')
+ns.add_network('172.31.9.128/25')
+print('\n'.join(str(x.cidr) for x in ns.substract('172.31.8.64/29')))
+```
+
+This example returns
+
+```bash
+172.31.0.0/23
+172.31.4.0/22
+172.31.8.0/26
+172.31.8.72/29
+172.31.8.80/28
+172.31.8.96/27
+172.31.8.128/25
+172.31.9.0/24
+````
+
+# Cloud vendor prefixes
+
+This tool contains lookup caches for some cloud vendors. Currently supported vendors are:
+
+- AWS
+- Cloudflare
+- Google Cloud
+- Google Services
+
+Note: Azure support was removed because their data is in a silly URL and I just don't
+care about them.
+
+Example to load data for cloud vendor IP prefix lookups and save it to user specific cache
+directory `~/.config/netlookup`.
+
+Following command requires internet connection to update the prefix lists.
+
+```python
+from netlookup.prefixes import Prefixes
+ns = Prefixes()
+print(ns.cache_directory)
+ns.update()
+ns.save()
+````
+
+## Get prefixes for cloud vendors
+
+Use the previously loaded cached cloud vendor IP prefix lookup and find some addresses.
+
+```python
+>>> ns.find('3.81.2.1')
+aws us-east-1 3.80.0.0/12
+````
+
+Similarly, you can get specific vendor network set and lookup address from there:
+
+```python
+>>> ns.get_vendor('google').find('216.58.210.142')
+google 216.58.192.0/19
+```
 
-packages = \
-['netlookup',
- 'netlookup.bin',
- 'netlookup.bin.commands',
- 'netlookup.network_sets']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cli-toolkit>=2,<3', 'dnspython>=2,<3', 'netaddr>=0.8,<0.9', 'requests>=2,<3']
-
-entry_points = \
-{'console_scripts': ['netlookup = netlookup.bin.netlookup:main']}
-
-setup_kwargs = {
-    'name': 'netlookup',
-    'version': '2.0.0',
-    'description': 'Python tools to look up information about networks',
-    'long_description': "![Unit Tests](https://github.com/hile/netlookup/actions/workflows/unittest.yml/badge.svg)\n![Style Checks](https://github.com/hile/netlookup/actions/workflows/lint.yml/badge.svg)\n\n# Command line network lookups and operations\n\nThis python tool implements pretty much same things as `netcalc` and `netblocks` libraries, but\nwith minor differences in the way things are done.\n\nThe library is intended to be usable both as a command line tool `netlookup` and as a library from\nserver code. Personally I use it for splitting IP ranges to subnets.\n\n## Installing\n\n```bash\npip install netlookup\n```\n\n# Command line tool `netlookup` basic usage\n\nFollowing examples illustrate Usage of netlookup tool.\n\nLookup details for IPv4 host with CIDR mask and IPv6 subnet:\n\n```bash\nnetlookup info 172.31.1.19/17 2c0f:fb50:4000::/56\n             CIDR 172.31.0.0/17\n          Netmask 255.255.128.0\n          Network 172.31.0.0\n        Broadcast 172.31.127.255\n       First host 172.31.0.1\n        Last host 172.31.127.254\n      Total hosts 32766\n             Next 172.31.128.0/17\n         Previous 172.30.128.0/17\n             Bits 10101100.00011111.00000000.00000000\n      Reverse DNS 0.0.31.172.in-addr.arpa.\n             CIDR 2c0f:fb50:4000::/56\n          Netmask ffff:ffff:ffff:ff00::\n          Network 2c0f:fb50:4000::\n        Broadcast 2c0f:fb50:4000:ff:ffff:ffff:ffff:ffff\n       First host 2c0f:fb50:4000::1\n        Last host 2c0f:fb50:4000:ff:ffff:ffff:ffff:fffe\n      Total hosts 4722366482869645213694\n             Next 2c0f:fb50:4000:100::/56\n         Previous 2c0f:fb50:3fff:ff00::/56\n             Bits 0010110000001111:1111101101010000:0100000000000000:0000000000000000:0000000000000000:0000000000000000:0000000000000000:0000000000000000\n      Reverse DNS 0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.4.0.5.b.f.f.0.c.2.ip6.arpa.\n```\n\nSplit subnet with defaults (to next smaller subnet / larger prefix):\n\n```bash\nnetlookup split 172.31.1.19/17 2c0f:fb50:4000::/56\n    172.31.0.0/18\n    172.31.64.0/18\n    2c0f:fb50:4000::/57\n    2c0f:fb50:4000:80::/57\n```\n\nSplit IPv4 subnets with specific prefix:\n\n```bash\nnetlookup split --mask 19 172.31.1.19/17 172.31.5.39/17\n    172.31.0.0/19\n    172.31.32.0/19\n    172.31.64.0/19\n    172.31.96.0/19\n    172.31.0.0/19\n    172.31.32.0/19\n    172.31.64.0/19\n    172.31.96.0/19\n```\n\nUsing the python library\n------------------------\n\nSome practical examples for using the API where a CLI command is not yet available.\n\nCreate set of networks and show minimal merged CIDR prefixes to cover this range:\n\n```python\nfrom netlookup.network_sets.base import NetworkSet\nns = NetworkSet()\nns.add_network('172.31.0.0/23')\nns.add_network('172.31.4.0/22')\nns.add_network('172.31.8.0/24')\nns.add_network('172.31.9.0/25')\nns.add_network('172.31.9.128/25')\nprint('\\n'.join(str(x.cidr) for x in ns.merged))\n```\n\nPrevious example returns\n\n```bash\n172.31.0.0/23\n172.31.4.0/22\n172.31.8.0/23\n```\n\nUsing same example, remove one /29 from the result set\n\n```python\nfrom netlookup.network_sets.base import NetworkSet\nns = NetworkSet()\nns.add_network('172.31.0.0/23')\nns.add_network('172.31.4.0/22')\nns.add_network('172.31.8.0/24')\nns.add_network('172.31.9.0/25')\nns.add_network('172.31.9.128/25')\nprint('\\n'.join(str(x.cidr) for x in ns.substract('172.31.8.64/29')))\n```\n\nThis example returns\n\n```bash\n172.31.0.0/23\n172.31.4.0/22\n172.31.8.0/26\n172.31.8.72/29\n172.31.8.80/28\n172.31.8.96/27\n172.31.8.128/25\n172.31.9.0/24\n````\n\n# Cloud vendor prefixes\n\nThis tool contains lookup caches for some cloud vendors. Currently supported vendors are:\n\n- AWS\n- Cloudflare\n- Google Cloud\n- Google Services\n\nNote: Azure support was removed because their data is in a silly URL and I just don't\ncare about them.\n\nExample to load data for cloud vendor IP prefix lookups and save it to user specific cache\ndirectory `~/.config/netlookup`.\n\nFollowing command requires internet connection to update the prefix lists.\n\n```python\nfrom netlookup.prefixes import Prefixes\nns = Prefixes()\nprint(ns.cache_directory)\nns.update()\nns.save()\n````\n\n## Get prefixes for cloud vendors\n\nUse the previously loaded cached cloud vendor IP prefix lookup and find some addresses.\n\n```python\n>>> ns.find('3.81.2.1')\naws us-east-1 3.80.0.0/12\n````\n\nSimilarly, you can get specific vendor network set and lookup address from there:\n\n```python\n>>> ns.get_vendor('google').find('216.58.210.142')\ngoogle 216.58.192.0/19\n```\n",
-    'author': 'Ilkka Tuohela',
-    'author_email': 'hile@iki.fi',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

