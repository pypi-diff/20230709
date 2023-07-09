# Comparing `tmp/minswap_py-0.2.0.tar.gz` & `tmp/minswap_py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minswap_py-0.2.0.tar", max compression
+gzip compressed data, was "minswap_py-0.2.1.tar", max compression
```

## Comparing `minswap_py-0.2.0.tar` & `minswap_py-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-01-23 21:36:51.427567 minswap_py-0.2.0/LICENSE
--rw-r--r--   0        0        0     1271 2023-06-29 12:52:22.149307 minswap_py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1645 2023-06-29 12:52:22.151307 minswap_py-0.2.0/README.md
--rw-r--r--   0        0        0      167 2023-05-24 02:47:34.932526 minswap_py-0.2.0/src/minswap/__init__.py
--rw-r--r--   0        0        0    17447 2023-06-29 12:29:11.317311 minswap_py-0.2.0/src/minswap/addr.py
--rw-r--r--   0        0        0    29962 2023-06-29 12:29:11.328310 minswap_py-0.2.0/src/minswap/assets.py
--rw-r--r--   0        0        0      382 2023-05-04 19:06:27.065397 minswap_py-0.2.0/src/minswap/models/__init__.py
--rw-r--r--   0        0        0    92403 2023-06-29 02:38:21.320380 minswap_py-0.2.0/src/minswap/models/blockfrost_models.py
--rw-r--r--   0        0        0     8715 2023-06-29 11:57:19.580680 minswap_py-0.2.0/src/minswap/models/common.py
--rw-r--r--   0        0        0    12147 2023-05-24 01:37:34.553330 minswap_py-0.2.0/src/minswap/pools.py
--rw-r--r--   0        0        0    13096 2023-06-29 12:03:25.120634 minswap_py-0.2.0/src/minswap/transactions.py
--rw-r--r--   0        0        0     8849 2023-06-29 11:59:53.375600 minswap_py-0.2.0/src/minswap/utils.py
--rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 minswap_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-01-23 21:36:51.427567 minswap_py-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1325 2023-07-09 00:06:49.111301 minswap_py-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2526 2023-07-09 00:10:54.817138 minswap_py-0.2.1/README.md
+-rw-r--r--   0        0        0      170 2023-06-29 13:18:21.012654 minswap_py-0.2.1/src/minswap/__init__.py
+-rw-r--r--   0        0        0    18209 2023-07-08 23:42:48.126153 minswap_py-0.2.1/src/minswap/addr.py
+-rw-r--r--   0        0        0    30826 2023-06-29 13:17:59.623510 minswap_py-0.2.1/src/minswap/assets.py
+-rw-r--r--   0        0        0      397 2023-06-29 13:18:21.014655 minswap_py-0.2.1/src/minswap/models/__init__.py
+-rw-r--r--   0        0        0    95901 2023-06-29 13:17:59.626508 minswap_py-0.2.1/src/minswap/models/blockfrost_models.py
+-rw-r--r--   0        0        0     9044 2023-06-29 13:17:59.627509 minswap_py-0.2.1/src/minswap/models/common.py
+-rw-r--r--   0        0        0    12574 2023-07-08 23:54:30.655576 minswap_py-0.2.1/src/minswap/pools.py
+-rw-r--r--   0        0        0    13458 2023-06-29 13:17:59.630510 minswap_py-0.2.1/src/minswap/transactions.py
+-rw-r--r--   0        0        0     9145 2023-06-29 13:17:59.631509 minswap_py-0.2.1/src/minswap/utils.py
+-rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 minswap_py-0.2.1/PKG-INFO
```

### Comparing `minswap_py-0.2.0/LICENSE` & `minswap_py-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `minswap_py-0.2.0/pyproject.toml` & `minswap_py-0.2.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-[tool.poetry]
-name = "minswap-py"
-version = "0.2.0"
-description = ""
-authors = ["eldermillenial <eldermillenial@protonmail.com>"]
-readme = "README.md"
-packages = [{include = "minswap", from = "src"}]
-license = "MIT"
-repository = "https://github.com/theeldermillenial/minswap-py"
-
-[tool.poetry.urls]
-"Issues" = "https://github.com/theeldermillenial/minswap-py/issues"
-
-[tool.poetry.dependencies]
-python = "^3.8.1"
-blockfrost-python = "0.5.2"
-pycardano = "0.7.2"
-pydantic = "1.10.4"
-python-dotenv = "0.21.1"
-llvmlite = "^0.39.1"
-numba = "^0.56.4"
-vaex = "^4.16.0"
-tqdm = "^4.65.0"
-
-[tool.poetry.group.dev.dependencies]
-nox = "2022.11.21"
-poetry = "^1.3.2"
-nox-poetry = "1.0.2"
-pytest = "7.2.1"
-black = "22.12.0"
-datamodel-code-generator = {extras = ["http"], version = "^0.16.1"}
-bump2version = "^1.0.1"
-mypy = "^0.991"
-flake8 = "^6.0.0"
-flake8-docstrings = "^1.7.0"
-mkdocs = "^1.4.2"
-mkdocs-material = "^9.0.6"
-mkdocstrings = "^0.20.0"
-mkdocs-gen-files = "^0.4.0"
-mkdocstrings-python = "^0.8.3"
-mkdocs-literate-nav = "^0.6.0"
-semver = "^2.13.0"
-packaging = "^23.0"
-pre-commit = "^3.0.1"
-
-[tool.isort]
-profile = "black"
-
-[tool.mypy]
-exclude = ['^blockfrost\.py$', 'tests/', 'examples/*']
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "minswap-py"
+version = "0.2.1"
+description = ""
+authors = ["eldermillenial <eldermillenial@protonmail.com>"]
+readme = "README.md"
+packages = [{include = "minswap", from = "src"}]
+license = "MIT"
+repository = "https://github.com/theeldermillenial/minswap-py"
+
+[tool.poetry.urls]
+"Issues" = "https://github.com/theeldermillenial/minswap-py/issues"
+
+[tool.poetry.dependencies]
+python = "^3.8.1"
+blockfrost-python = "0.5.2"
+pycardano = "0.7.2"
+pydantic = "1.10.4"
+python-dotenv = "0.21.1"
+llvmlite = "^0.39.1"
+numba = "^0.56.4"
+vaex = "^4.16.0"
+tqdm = "^4.65.0"
+
+[tool.poetry.group.dev.dependencies]
+nox = "2022.11.21"
+poetry = "^1.3.2"
+nox-poetry = "1.0.2"
+pytest = "7.2.1"
+black = "22.12.0"
+datamodel-code-generator = {extras = ["http"], version = "^0.16.1"}
+bump2version = "^1.0.1"
+mypy = "^0.991"
+flake8 = "^6.0.0"
+flake8-docstrings = "^1.7.0"
+mkdocs = "^1.4.2"
+mkdocs-material = "^9.0.6"
+mkdocstrings = "^0.20.0"
+mkdocs-gen-files = "^0.4.0"
+mkdocstrings-python = "^0.8.3"
+mkdocs-literate-nav = "^0.6.0"
+semver = "^2.13.0"
+packaging = "^23.0"
+pre-commit = "^3.0.1"
+
+[tool.isort]
+profile = "black"
+
+[tool.mypy]
+exclude = ['^blockfrost\.py$', 'tests/', 'examples/*']
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `minswap_py-0.2.0/README.md` & `minswap_py-0.2.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,48 @@
-# minswap-py (v0.2.0)
+# minswap-py (v0.2.1)
 <p align="center">
     <img src="https://img.shields.io/pypi/status/minswap-py?style=flat-square" />
     <img src="https://img.shields.io/pypi/dm/minswap-py?style=flat-square" />
     <img src="https://img.shields.io/pypi/l/minswap-py?style=flat-square"/>
     <img src="https://img.shields.io/pypi/v/minswap-py?style=flat-square"/>
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 `minswap-py` is a tool to interact with [Minswap](https://minswap.org/).  The current version has feature parity with the minswap [blockfrost-adapter](https://github.com/minswap/blockfrost-adapter).
 
 Documentation and additional features coming soon.
 
+This tool was recently used to help generate data for the Minswap DAO Emissions and
+Treasury report. You can read the report here:
+
+https://minswap.org/storage/2023/06/31-3-2023_Emissions_and_Treasury_Report.pdf
+
+## Have a question?
+
+Reach out to me on the Minswap discord. You can usually find me on`#technical`, and I'm happy to respond to questions there.
+
+https://discord.com/channels/829060079248343090/845208119729979402
+
+## Support
+
+If you find this project useful, please consider supporting the project by buying me a
+beer in the form of ADA or MIN:
+
+```bash
+addr1q9hw8fuex09vr3rqwtn4fzh9qxjlzjzh8aww684ln0rv0cfu3f0de6qkmh7c7yysfz808978wwe6ll30wu8l3cgvgdjqa7egnl
+```
+
 ## Changelog
 
+### 0.2.1
+
+There are now multiple Minswap pool addresses. This patch updates the code to read all of them when using `minswap.get_pools` and subsequent functions that require pool addresses.
+
+### v0.2.0
+
 Added CHANGELOG.md :)
 
 Improvements:
 1. Added a blockfrost rate limiter. Every call to blockfrost adds to a time delayed counter, and prevents running into rate limits. This helps to prevent abuse of the blockfrost API.
 2. Added significant transaction and asset functionality. It is now possible to pull in asset historys.
 
 Changes:
```

#### html2text {}

```diff
@@ -1,20 +1,31 @@
-# minswap-py (v0.2.0)
+# minswap-py (v0.2.1)
   [https://img.shields.io/pypi/status/minswap-py?style=flat-square] [https://
  img.shields.io/pypi/dm/minswap-py?style=flat-square] [https://img.shields.io/
  pypi/l/minswap-py?style=flat-square] [https://img.shields.io/pypi/v/minswap-
                    py?style=flat-square] [Code_style:_black]
 `minswap-py` is a tool to interact with [Minswap](https://minswap.org/). The
 current version has feature parity with the minswap [blockfrost-adapter](https:
 //github.com/minswap/blockfrost-adapter). Documentation and additional features
-coming soon. ## Changelog Added CHANGELOG.md :) Improvements: 1. Added a
-blockfrost rate limiter. Every call to blockfrost adds to a time delayed
-counter, and prevents running into rate limits. This helps to prevent abuse of
-the blockfrost API. 2. Added significant transaction and asset functionality.
-It is now possible to pull in asset historys. Changes: 1. There was an
-inconsistency in how time values were being cached. See the `examples/
-rename_time.py` for a way to translate previously cached data to the new
-standard. ## Quickstart In order to use this package: 1. Install with `pip
+coming soon. This tool was recently used to help generate data for the Minswap
+DAO Emissions and Treasury report. You can read the report here: https://
+minswap.org/storage/2023/06/31-3-2023_Emissions_and_Treasury_Report.pdf ## Have
+a question? Reach out to me on the Minswap discord. You can usually find me
+on`#technical`, and I'm happy to respond to questions there. https://
+discord.com/channels/829060079248343090/845208119729979402 ## Support If you
+find this project useful, please consider supporting the project by buying me a
+beer in the form of ADA or MIN: ```bash
+addr1q9hw8fuex09vr3rqwtn4fzh9qxjlzjzh8aww684ln0rv0cfu3f0de6qkmh7c7yysfz808978wwe6ll30wu8l3cgvgdjqa7egnl
+``` ## Changelog ### 0.2.1 There are now multiple Minswap pool addresses. This
+patch updates the code to read all of them when using `minswap.get_pools` and
+subsequent functions that require pool addresses. ### v0.2.0 Added CHANGELOG.md
+:) Improvements: 1. Added a blockfrost rate limiter. Every call to blockfrost
+adds to a time delayed counter, and prevents running into rate limits. This
+helps to prevent abuse of the blockfrost API. 2. Added significant transaction
+and asset functionality. It is now possible to pull in asset historys. Changes:
+1. There was an inconsistency in how time values were being cached. See the
+`examples/rename_time.py` for a way to translate previously cached data to the
+new standard. ## Quickstart In order to use this package: 1. Install with `pip
 install minswap-py` 2. Sign up for blockfrost and get an API key. 3. In your
 working directory, save a `.env` file. In this file, save your blockfrost API
 key as follows: ```bash PROJECT_ID=YOUR_BLOCKFROST_ID ``` Once you do this, you
 can try out the code in the `examples` folder on the Github repository.
```

### Comparing `minswap_py-0.2.0/src/minswap/addr.py` & `minswap_py-0.2.1/src/minswap/addr.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,17 +24,34 @@
 from pyarrow import TimestampScalar
 
 from minswap.models import Address, PoolTransactionReference
 from minswap.utils import get_utxo, save_timestamp
 
 logger = logging.getLogger(__name__)
 
-POOL = Address(
-    bech32="addr1z8snz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxz2j2c79gy9l76sdg0xwhd7r0c0kna0tycz4y5s6mlenh8pq0xmsha"  # noqa
-)
+POOL = [
+    Address(
+        bech32="addr1z8snz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxz2j2c79gy9l76sdg0xwhd7r0c0kna0tycz4y5s6mlenh8pq0xmsha"  # noqa
+    ),
+    Address(
+        bech32="addr1z8snz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxzfgf0jgfz5xdvg2pges20usxhw8zwnkggheqrxwmxd6huuqss46eh"  # noqa
+    ),
+    Address(
+        bech32="addr1z8snz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxzwccf8ywaly0m99ngq68lus48lmafut7ku9geawu8u6k49suv42qq"  # noqa
+    ),
+    Address(
+        bech32="addr1z8snz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxz02znpd777wgl9wwpk0dvdzuxn93mqh82q7vv6s9jn25rws52z94g"  # noqa
+    ),
+    Address(
+        bech32="addr1z8snz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxz2jyskd3y6etkv8ye450545xu6q4jfq5hv4e0uxwkpf8lsq048y90"  # noqa
+    ),
+    Address(
+        bech32="addr1z8snz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxztnqm37tpj0q63s0qns5wfe4flqzqqg55760472n7yt4v8skpaj3k"  # noqa
+    ),
+]
 ORDER = Address(
     bech32="addr1zxn9efv2f6w82hagxqtn62ju4m293tqvw0uhmdl64ch8uw6j2c79gy9l76sdg0xwhd7r0c0kna0tycz4y5s6mlenh8pq6s3z70"  # noqa
 )
 
 POOL_TEST = Address(
     bech32="addr_test1zrsnz7c4974vzdpxu65ruphl3zjdvtxw8strf2c2tmqnxzvrajt8r8wqtygrfduwgukk73m5gcnplmztc5tl5ngy0upqs8q93k"  # noqa
 )
```

### Comparing `minswap_py-0.2.0/src/minswap/models/blockfrost_models.py` & `minswap_py-0.2.1/src/minswap/models/blockfrost_models.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,3498 +1,3498 @@
-# generated by datamodel-codegen:
-#   filename:  openapi.yaml
-#   timestamp: 2023-06-02T01:54:33+00:00
-
-from __future__ import annotations
-
-from enum import Enum
-from typing import Any, Dict, List, Optional, Union
-
-from pydantic import BaseModel, Extra, Field
-
-
-class BlockContent(BaseModel):
-    time: int = Field(..., example=1641338934)
-    """
-    Block creation time in UNIX time
-    """
-    height: Optional[int] = Field(..., example=15243593)
-    """
-    Block number
-    """
-    hash: str = Field(
-        ..., example="4ea1ba291e8eef538635a53e59fddba7810d1679631cc3aed7c8e6c4091a516a"
-    )
-    """
-    Hash of the block
-    """
-    slot: Optional[int] = Field(..., example=412162133)
-    """
-    Slot number
-    """
-    epoch: Optional[int] = Field(..., example=425)
-    """
-    Epoch number
-    """
-    epoch_slot: Optional[int] = Field(..., example=12)
-    """
-    Slot within the epoch
-    """
-    slot_leader: str = Field(
-        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2qnikdy"
-    )
-    """
-    Bech32 ID of the slot leader or specific block description in case there is no slot leader
-    """
-    size: int = Field(..., example=3)
-    """
-    Block size in Bytes
-    """
-    tx_count: int = Field(..., example=1)
-    """
-    Number of transactions in the block
-    """
-    output: Optional[str] = Field(..., example="128314491794")
-    """
-    Total output within the block in Lovelaces
-    """
-    fees: Optional[str] = Field(..., example="592661")
-    """
-    Total fees within the block in Lovelaces
-    """
-    block_vrf: Optional[str] = Field(
-        ...,
-        example="vrf_vk1wf2k6lhujezqcfe00l6zetxpnmh9n6mwhpmhm0dvfh3fxgmdnrfqkms8ty",
-        max_length=65,
-        min_length=65,
-    )
-    """
-    VRF key of the block
-    """
-    op_cert: Optional[str] = Field(
-        ..., example="da905277534faf75dae41732650568af545134ee08a3c0392dbefc8096ae177c"
-    )
-    """
-    The hash of the operational certificate of the block producer
-    """
-    op_cert_counter: Optional[str] = Field(..., example="18")
-    """
-    The value of the counter used to produce the operational certificate
-    """
-    previous_block: Optional[str] = Field(
-        ..., example="43ebccb3ac72c7cebd0d9b755a4b08412c9f5dcb81b8a0ad1e3c197d29d47b05"
-    )
-    """
-    Hash of the previous block
-    """
-    next_block: Optional[str] = Field(
-        ..., example="8367f026cf4b03e116ff8ee5daf149b55ba5a6ec6dec04803b8dc317721d15fa"
-    )
-    """
-    Hash of the next block
-    """
-    confirmations: int = Field(..., example=4698)
-    """
-    Number of block confirmations
-    """
-
-
-class BlockContentTxs(BaseModel):
-    __root__: List[str] = Field(
-        ...,
-        example=[
-            "8788591983aa73981fc92d6cddbbe643959f5a784e84b8bee0db15823f575a5b",
-            "4eef6bb7755d8afbeac526b799f3e32a624691d166657e9d862aaeb66682c036",
-            "52e748c4dec58b687b90b0b40d383b9fe1f24c1a833b7395cdf07dd67859f46f",
-            "e8073fd5318ff43eca18a852527166aa8008bee9ee9e891f585612b7e4ba700b",
-        ],
-    )
-
-
-class BlockContentArray(BaseModel):
-    __root__: List[BlockContent]
-
-
-class Transaction(BaseModel):
-    tx_hash: str
-
-
-class BlockContentAddress(BaseModel):
-    address: str
-    """
-    Address that was affected in the specified block
-    """
-    transactions: List[Transaction]
-    """
-    List of transactions containing the address either in their inputs or outputs. Sorted by transaction index within a block, ascending.
-    """
-
-
-class BlockContentAddresses(BaseModel):
-    __root__: List[BlockContentAddress] = Field(
-        ...,
-        example=[
-            {
-                "address": "addr1q9ld26v2lv8wvrxxmvg90pn8n8n5k6tdst06q2s856rwmvnueldzuuqmnsye359fqrk8hwvenjnqultn7djtrlft7jnq7dy7wv",
-                "transactions": [
-                    {
-                        "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157f0"
-                    }
-                ],
-            },
-            {
-                "address": "addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
-                "transactions": [
-                    {
-                        "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157d0"
-                    }
-                ],
-            },
-        ],
-    )
-
-
-class GenesisContent(BaseModel):
-    active_slots_coefficient: float = Field(..., example=0.05)
-    """
-    The proportion of slots in which blocks should be issued
-    """
-    update_quorum: int = Field(..., example=5)
-    """
-    Determines the quorum needed for votes on the protocol parameter updates
-    """
-    max_lovelace_supply: str = Field(..., example="45000000000000000")
-    """
-    The total number of lovelace in the system
-    """
-    network_magic: int = Field(..., example=764824073)
-    """
-    Network identifier
-    """
-    epoch_length: int = Field(..., example=432000)
-    """
-    Number of slots in an epoch
-    """
-    system_start: int = Field(..., example=1506203091)
-    """
-    Time of slot 0 in UNIX time
-    """
-    slots_per_kes_period: int = Field(..., example=129600)
-    """
-    Number of slots in an KES period
-    """
-    slot_length: int = Field(..., example=1)
-    """
-    Duration of one slot in seconds
-    """
-    max_kes_evolutions: int = Field(..., example=62)
-    """
-    The maximum number of time a KES key can be evolved before a pool operator must create a new operational certificate
-    """
-    security_param: int = Field(..., example=2160)
-    """
-    Security parameter k
-    """
-
-
-class EpochContent(BaseModel):
-    epoch: int = Field(..., example=225)
-    """
-    Epoch number
-    """
-    start_time: int = Field(..., example=1603403091)
-    """
-    Unix time of the start of the epoch
-    """
-    end_time: int = Field(..., example=1603835086)
-    """
-    Unix time of the end of the epoch
-    """
-    first_block_time: int = Field(..., example=1603403092)
-    """
-    Unix time of the first block of the epoch
-    """
-    last_block_time: int = Field(..., example=1603835084)
-    """
-    Unix time of the last block of the epoch
-    """
-    block_count: int = Field(..., example=21298)
-    """
-    Number of blocks within the epoch
-    """
-    tx_count: int = Field(..., example=17856)
-    """
-    Number of transactions within the epoch
-    """
-    output: str = Field(..., example="7849943934049314")
-    """
-    Sum of all the transactions within the epoch in Lovelaces
-    """
-    fees: str = Field(..., example="4203312194")
-    """
-    Sum of all the fees within the epoch in Lovelaces
-    """
-    active_stake: Optional[str] = Field(..., example="784953934049314")
-    """
-    Sum of all the active stakes within the epoch in Lovelaces
-    """
-
-
-class EpochParamContent(BaseModel):
-    epoch: int = Field(..., example=225)
-    """
-    Epoch number
-    """
-    min_fee_a: int = Field(..., example=44)
-    """
-    The linear factor for the minimum fee calculation for given epoch
-    """
-    min_fee_b: int = Field(..., example=155381)
-    """
-    The constant factor for the minimum fee calculation
-    """
-    max_block_size: int = Field(..., example=65536)
-    """
-    Maximum block body size in Bytes
-    """
-    max_tx_size: int = Field(..., example=16384)
-    """
-    Maximum transaction size
-    """
-    max_block_header_size: int = Field(..., example=1100)
-    """
-    Maximum block header size
-    """
-    key_deposit: str = Field(..., example="2000000")
-    """
-    The amount of a key registration deposit in Lovelaces
-    """
-    pool_deposit: str = Field(..., example="500000000")
-    """
-    The amount of a pool registration deposit in Lovelaces
-    """
-    e_max: int = Field(..., example=18)
-    """
-    Epoch bound on pool retirement
-    """
-    n_opt: int = Field(..., example=150)
-    """
-    Desired number of pools
-    """
-    a0: float = Field(..., example=0.3)
-    """
-    Pool pledge influence
-    """
-    rho: float = Field(..., example=0.003)
-    """
-    Monetary expansion
-    """
-    tau: float = Field(..., example=0.2)
-    """
-    Treasury expansion
-    """
-    decentralisation_param: float = Field(..., example=0.5)
-    """
-    Percentage of blocks produced by federated nodes
-    """
-    extra_entropy: Optional[str]
-    """
-    Seed for extra entropy
-    """
-    protocol_major_ver: int = Field(..., example=2)
-    """
-    Accepted protocol major version
-    """
-    protocol_minor_ver: int = Field(..., example=0)
-    """
-    Accepted protocol minor version
-    """
-    min_utxo: str = Field(..., example="1000000")
-    """
-    Minimum UTXO value
-    """
-    min_pool_cost: str = Field(..., example="340000000")
-    """
-    Minimum stake cost forced on the pool
-    """
-    nonce: str = Field(
-        ..., example="1a3be38bcbb7911969283716ad7aa550250226b76a61fc51cc9a9a35d9276d81"
-    )
-    """
-    Epoch number only used once
-    """
-    cost_models: Optional[Dict[str, Any]] = Field(
-        ...,
-        example={
-            "PlutusV1": {
-                "addInteger-cpu-arguments-intercept": 197209,
-                "addInteger-cpu-arguments-slope": 0,
-            },
-            "PlutusV2": {
-                "addInteger-cpu-arguments-intercept": 197209,
-                "addInteger-cpu-arguments-slope": 0,
-            },
-        },
-    )
-    """
-    Cost models parameters for Plutus Core scripts
-    """
-    price_mem: Optional[float] = Field(..., example=0.0577)
-    """
-    The per word cost of script memory usage
-    """
-    price_step: Optional[float] = Field(..., example=7.21e-05)
-    """
-    The cost of script execution step usage
-    """
-    max_tx_ex_mem: Optional[str] = Field(..., example="10000000")
-    """
-    The maximum number of execution memory allowed to be used in a single transaction
-    """
-    max_tx_ex_steps: Optional[str] = Field(..., example="10000000000")
-    """
-    The maximum number of execution steps allowed to be used in a single transaction
-    """
-    max_block_ex_mem: Optional[str] = Field(..., example="50000000")
-    """
-    The maximum number of execution memory allowed to be used in a single block
-    """
-    max_block_ex_steps: Optional[str] = Field(..., example="40000000000")
-    """
-    The maximum number of execution steps allowed to be used in a single block
-    """
-    max_val_size: Optional[str] = Field(..., example="5000")
-    """
-    The maximum Val size
-    """
-    collateral_percent: Optional[int] = Field(..., example=150)
-    """
-    The percentage of the transactions fee which must be provided as collateral when including non-native scripts
-    """
-    max_collateral_inputs: Optional[int] = Field(..., example=3)
-    """
-    The maximum number of collateral inputs allowed in a transaction
-    """
-    coins_per_utxo_size: Optional[str] = Field(..., example="34482")
-    """
-    Cost per UTxO word for Alonzo. Cost per UTxO byte for Babbage and later.
-    """
-    coins_per_utxo_word: Optional[str] = Field(..., example="34482")
-    """
-    Cost per UTxO word for Alonzo. Cost per UTxO byte for Babbage and later.
-    """
-
-
-class EpochContentArray(BaseModel):
-    __root__: List[EpochContent]
-
-
-class EpochStakeContentItem(BaseModel):
-    stake_address: str = Field(
-        ..., example="stake1u9l5q5jwgelgagzyt6nuaasefgmn8pd25c8e9qpeprq0tdcp0e3uk"
-    )
-    """
-    Stake address
-    """
-    pool_id: str = Field(
-        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
-    )
-    """
-    Bech32 prefix of the pool delegated to
-    """
-    amount: str = Field(..., example="4440295078")
-    """
-    Amount of active delegated stake in Lovelaces
-    """
-
-
-class EpochStakeContent(BaseModel):
-    __root__: List[EpochStakeContentItem]
-
-
-class EpochStakePoolContentItem(BaseModel):
-    stake_address: str = Field(
-        ..., example="stake1u9l5q5jwgelgagzyt6nuaasefgmn8pd25c8e9qpeprq0tdcp0e3uk"
-    )
-    """
-    Stake address
-    """
-    amount: str = Field(..., example="4440295078")
-    """
-    Amount of active delegated stake in Lovelaces
-    """
-
-
-class EpochStakePoolContent(BaseModel):
-    __root__: List[EpochStakePoolContentItem]
-
-
-class EpochBlockContent(BaseModel):
-    __root__: List[str] = Field(
-        ...,
-        example=[
-            "d0fa315687e99ccdc96b14cc2ea74a767405d64427b648c470731a9b69e4606e",
-            "38bc6efb92a830a0ed22a64f979d120d26483fd3c811f6622a8c62175f530878",
-            "f3258fcd8b975c061b4fcdcfcbb438807134d6961ec278c200151274893b6b7d",
-        ],
-    )
-
-
-class OutputAmountItem(BaseModel):
-    """
-    The sum of all the UTXO per asset
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-
-
-class TxContent(BaseModel):
-    hash: str = Field(
-        ..., example="1e043f100dce12d107f679685acd2fc0610e10f72a92d412794c9773d11d8477"
-    )
-    """
-    Transaction hash
-    """
-    block: str = Field(
-        ..., example="356b7d7dbb696ccd12775c016941057a9dc70898d87a63fc752271bb46856940"
-    )
-    """
-    Block hash
-    """
-    block_height: int = Field(..., example=123456)
-    """
-    Block number
-    """
-    block_time: int = Field(..., example=1635505891)
-    """
-    Block creation time in UNIX time
-    """
-    slot: int = Field(..., example=42000000)
-    """
-    Slot number
-    """
-    index: int = Field(..., example=1)
-    """
-    Transaction index within the block
-    """
-    output_amount: List[OutputAmountItem] = Field(
-        ...,
-        example=[
-            {"unit": "lovelace", "quantity": "42000000"},
-            {
-                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "12",
-            },
-        ],
-    )
-    fees: str = Field(..., example="182485")
-    """
-    Fees of the transaction in Lovelaces
-    """
-    deposit: str = Field(..., example="0")
-    """
-    Deposit within the transaction in Lovelaces
-    """
-    size: int = Field(..., example=433)
-    """
-    Size of the transaction in Bytes
-    """
-    invalid_before: Optional[str]
-    """
-    Left (included) endpoint of the timelock validity intervals
-    """
-    invalid_hereafter: Optional[str] = Field(..., example="13885913")
-    """
-    Right (excluded) endpoint of the timelock validity intervals
-    """
-    utxo_count: int = Field(..., example=4)
-    """
-    Count of UTXOs within the transaction
-    """
-    withdrawal_count: int = Field(..., example=0)
-    """
-    Count of the withdrawals within the transaction
-    """
-    mir_cert_count: int = Field(..., example=0)
-    """
-    Count of the MIR certificates within the transaction
-    """
-    delegation_count: int = Field(..., example=0)
-    """
-    Count of the delegations within the transaction
-    """
-    stake_cert_count: int = Field(..., example=0)
-    """
-    Count of the stake keys (de)registration within the transaction
-    """
-    pool_update_count: int = Field(..., example=0)
-    """
-    Count of the stake pool registration and update certificates within the transaction
-    """
-    pool_retire_count: int = Field(..., example=0)
-    """
-    Count of the stake pool retirement certificates within the transaction
-    """
-    asset_mint_or_burn_count: int = Field(..., example=0)
-    """
-    Count of asset mints and burns within the transaction
-    """
-    redeemer_count: int = Field(..., example=0)
-    """
-    Count of redeemers within the transaction
-    """
-    valid_contract: bool = Field(..., example=True)
-    """
-    True if contract script passed validation
-    """
-
-
-class AmountItem(BaseModel):
-    """
-    The sum of all the UTXO per asset
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-
-
-class Input(BaseModel):
-    address: str = Field(
-        ...,
-        example="addr1q9ld26v2lv8wvrxxmvg90pn8n8n5k6tdst06q2s856rwmvnueldzuuqmnsye359fqrk8hwvenjnqultn7djtrlft7jnq7dy7wv",
-    )
-    """
-    Input address
-    """
-    amount: List[AmountItem] = Field(
-        ...,
-        example=[
-            {"unit": "lovelace", "quantity": "42000000"},
-            {
-                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "12",
-            },
-        ],
-    )
-    tx_hash: str = Field(
-        ..., example="1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157f0"
-    )
-    """
-    Hash of the UTXO transaction
-    """
-    output_index: int = Field(..., example=0)
-    """
-    UTXO index in the transaction
-    """
-    data_hash: Optional[str] = Field(
-        ..., example="9e478573ab81ea7a8e31891ce0648b81229f408d596a3483e6f4f9b92d3cf710"
-    )
-    """
-    The hash of the transaction output datum
-    """
-    inline_datum: Optional[str] = Field(..., example="19a6aa")
-    """
-    CBOR encoded inline datum
-    """
-    reference_script_hash: Optional[str] = Field(
-        ..., example="13a3efd825703a352a8f71f4e2758d08c28c564e8dfcce9f77776ad1"
-    )
-    """
-    The hash of the reference script of the input
-    """
-    collateral: bool = Field(..., example=False)
-    """
-    Whether the input is a collateral consumed on script validation failure
-    """
-    reference: Optional[bool] = Field(None, example=False)
-    """
-    Whether the input is a reference transaction input
-    """
-
-
-class AmountItem1(BaseModel):
-    """
-    The sum of all the UTXO per asset
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-
-
-class Output(BaseModel):
-    address: str = Field(
-        ...,
-        example="addr1q9ld26v2lv8wvrxxmvg90pn8n8n5k6tdst06q2s856rwmvnueldzuuqmnsye359fqrk8hwvenjnqultn7djtrlft7jnq7dy7wv",
-    )
-    """
-    Output address
-    """
-    amount: List[AmountItem1] = Field(
-        ...,
-        example=[
-            {"unit": "lovelace", "quantity": "42000000"},
-            {
-                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "12",
-            },
-        ],
-    )
-    output_index: int = Field(..., example=0)
-    """
-    UTXO index in the transaction
-    """
-    data_hash: Optional[str] = Field(
-        ..., example="9e478573ab81ea7a8e31891ce0648b81229f408d596a3483e6f4f9b92d3cf710"
-    )
-    """
-    The hash of the transaction output datum
-    """
-    inline_datum: Optional[str] = Field(..., example="19a6aa")
-    """
-    CBOR encoded inline datum
-    """
-    collateral: bool = Field(..., example=False)
-    """
-    Whether the output is a collateral output
-    """
-    reference_script_hash: Optional[str] = Field(
-        ..., example="13a3efd825703a352a8f71f4e2758d08c28c564e8dfcce9f77776ad1"
-    )
-    """
-    The hash of the reference script of the output
-    """
-
-
-class TxContentUtxo(BaseModel):
-    hash: str = Field(
-        ..., example="1e043f100dce12d107f679685acd2fc0610e10f72a92d412794c9773d11d8477"
-    )
-    """
-    Transaction hash
-    """
-    inputs: List[Input]
-    outputs: List[Output]
-
-
-class TxContentStakeAddrItem(BaseModel):
-    cert_index: int = Field(..., example=0)
-    """
-    Index of the certificate within the transaction
-    """
-    address: str = Field(
-        ..., example="stake1u9t3a0tcwune5xrnfjg4q7cpvjlgx9lcv0cuqf5mhfjwrvcwrulda"
-    )
-    """
-    Delegation stake address
-    """
-    registration: bool = Field(..., example=True)
-    """
-    Registration boolean, false if deregistration
-    """
-
-
-class TxContentStakeAddr(BaseModel):
-    __root__: List[TxContentStakeAddrItem]
-
-
-class TxContentDelegation(BaseModel):
-    index: int = Field(..., example=0)
-    """
-    Index of the certificate within the transaction
-    """
-    cert_index: int = Field(..., example=0)
-    """
-    Index of the certificate within the transaction
-    """
-    address: str = Field(
-        ..., example="stake1u9r76ypf5fskppa0cmttas05cgcswrttn6jrq4yd7jpdnvc7gt0yc"
-    )
-    """
-    Bech32 delegation stake address
-    """
-    pool_id: str = Field(
-        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
-    )
-    """
-    Bech32 ID of delegated stake pool
-    """
-    active_epoch: int = Field(..., example=210)
-    """
-    Epoch in which the delegation becomes active
-    """
-
-
-class TxContentDelegations(BaseModel):
-    __root__: List[TxContentDelegation]
-
-
-class TxContentWithdrawal(BaseModel):
-    address: str = Field(
-        ..., example="stake1u9r76ypf5fskppa0cmttas05cgcswrttn6jrq4yd7jpdnvc7gt0yc"
-    )
-    """
-    Bech32 withdrawal address
-    """
-    amount: str = Field(..., example="431833601")
-    """
-    Withdrawal amount in Lovelaces
-    """
-
-
-class TxContentWithdrawals(BaseModel):
-    __root__: List[TxContentWithdrawal]
-
-
-class Pot(Enum):
-    """
-    Source of MIR funds
-    """
-
-    reserve = "reserve"
-    treasury = "treasury"
-
-
-class TxContentMir(BaseModel):
-    pot: Pot = Field(..., example="reserve")
-    """
-    Source of MIR funds
-    """
-    cert_index: int = Field(..., example=0)
-    """
-    Index of the certificate within the transaction
-    """
-    address: str = Field(
-        ..., example="stake1u9r76ypf5fskppa0cmttas05cgcswrttn6jrq4yd7jpdnvc7gt0yc"
-    )
-    """
-    Bech32 stake address
-    """
-    amount: str = Field(..., example="431833601")
-    """
-    MIR amount in Lovelaces
-    """
-
-
-class TxContentMirs(BaseModel):
-    __root__: List[TxContentMir]
-
-
-class Metadata(BaseModel):
-    url: Optional[str] = Field(..., example="https://stakenuts.com/mainnet.json")
-    """
-    URL to the stake pool metadata
-    """
-    hash: Optional[str] = Field(
-        ..., example="47c0c68cb57f4a5b4a87bad896fc274678e7aea98e200fa14a1cb40c0cab1d8c"
-    )
-    """
-    Hash of the metadata file
-    """
-    ticker: Optional[str] = Field(..., example="NUTS")
-    """
-    Ticker of the stake pool
-    """
-    name: Optional[str] = Field(..., example="Stake Nuts")
-    """
-    Name of the stake pool
-    """
-    description: Optional[str] = Field(..., example="The best pool ever")
-    """
-    Description of the stake pool
-    """
-    homepage: Optional[str] = Field(..., example="https://stakentus.com/")
-    """
-    Home page of the stake pool
-    """
-
-
-class Relay(BaseModel):
-    ipv4: Optional[str] = Field(..., example="4.4.4.4")
-    """
-    IPv4 address of the relay
-    """
-    ipv6: Optional[str] = Field(..., example="https://stakenuts.com/mainnet.json")
-    """
-    IPv6 address of the relay
-    """
-    dns: Optional[str] = Field(..., example="relay1.stakenuts.com")
-    """
-    DNS name of the relay
-    """
-    dns_srv: Optional[str] = Field(..., example="_relays._tcp.relays.stakenuts.com")
-    """
-    DNS SRV entry of the relay
-    """
-    port: int = Field(..., example=3001)
-    """
-    Network port of the relay
-    """
-
-
-class TxContentPoolCert(BaseModel):
-    cert_index: int = Field(..., example=0)
-    """
-    Index of the certificate within the transaction
-    """
-    pool_id: str = Field(
-        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
-    )
-    """
-    Bech32 encoded pool ID
-    """
-    vrf_key: str = Field(
-        ..., example="0b5245f9934ec2151116fb8ec00f35fd00e0aa3b075c4ed12cce440f999d8233"
-    )
-    """
-    VRF key hash
-    """
-    pledge: str = Field(..., example="5000000000")
-    """
-    Stake pool certificate pledge in Lovelaces
-    """
-    margin_cost: float = Field(..., example=0.05)
-    """
-    Margin tax cost of the stake pool
-    """
-    fixed_cost: str = Field(..., example="340000000")
-    """
-    Fixed tax cost of the stake pool in Lovelaces
-    """
-    reward_account: str = Field(
-        ..., example="stake1uxkptsa4lkr55jleztw43t37vgdn88l6ghclfwuxld2eykgpgvg3f"
-    )
-    """
-    Bech32 reward account of the stake pool
-    """
-    owners: List[str] = Field(
-        ..., example=["stake1u98nnlkvkk23vtvf9273uq7cph5ww6u2yq2389psuqet90sv4xv9v"]
-    )
-    metadata: Optional[Metadata]
-    relays: List[Relay]
-    active_epoch: int = Field(..., example=210)
-    """
-    Epoch in which the update becomes active
-    """
-
-
-class TxContentPoolCerts(BaseModel):
-    __root__: List[TxContentPoolCert]
-
-
-class TxContentPoolRetire(BaseModel):
-    cert_index: int = Field(..., example=0)
-    """
-    Index of the certificate within the transaction
-    """
-    pool_id: str = Field(
-        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
-    )
-    """
-    Bech32 stake pool ID
-    """
-    retiring_epoch: int = Field(..., example=216)
-    """
-    Epoch in which the pool becomes retired
-    """
-
-
-class TxContentPoolRetires(BaseModel):
-    __root__: List[TxContentPoolRetire]
-
-
-class TxContentMetadatum(BaseModel):
-    label: str
-    """
-    Metadata label
-    """
-    json_metadata: Union[str, Dict[str, Any]]
-    """
-    Content of the metadata
-    """
-
-
-class TxContentMetadata(BaseModel):
-    __root__: List[TxContentMetadatum] = Field(
-        ...,
-        example=[
-            {
-                "label": "1967",
-                "json_metadata": {
-                    "metadata": "https://nut.link/metadata.json",
-                    "hash": "6bf124f217d0e5a0a8adb1dbd8540e1334280d49ab861127868339f43b3948af",
-                },
-            },
-            {
-                "label": "1968",
-                "json_metadata": {
-                    "ADAUSD": [
-                        {"value": "0.10409800535729975", "source": "ergoOracles"}
-                    ]
-                },
-            },
-        ],
-    )
-
-
-class TxContentMetadataCborItem(BaseModel):
-    label: str
-    """
-    Metadata label
-    """
-    cbor_metadata: Optional[str]
-    """
-    Content of the CBOR metadata
-    """
-    metadata: Optional[str]
-    """
-    Content of the CBOR metadata in hex
-    """
-
-
-class TxContentMetadataCbor(BaseModel):
-    __root__: List[TxContentMetadataCborItem] = Field(
-        ...,
-        example=[
-            {
-                "label": "1968",
-                "cbor_metadata": "\\xa100a16b436f6d62696e6174696f6e8601010101010c",
-                "metadata": "a100a16b436f6d62696e6174696f6e8601010101010c",
-            }
-        ],
-    )
-
-
-class Purpose(Enum):
-    """
-    Validation purpose
-    """
-
-    spend = "spend"
-    mint = "mint"
-    cert = "cert"
-    reward = "reward"
-
-
-class TxContentRedeemer(BaseModel):
-    tx_index: int = Field(..., example=0)
-    """
-    Index of the redeemer within the transaction
-    """
-    purpose: Purpose = Field(..., example="spend")
-    """
-    Validation purpose
-    """
-    script_hash: str = Field(
-        ..., example="ec26b89af41bef0f7585353831cb5da42b5b37185e0c8a526143b824"
-    )
-    """
-    Script hash
-    """
-    redeemer_data_hash: str = Field(
-        ..., example="923918e403bf43c34b4ef6b48eb2ee04babed17320d8d1b9ff9ad086e86f44ec"
-    )
-    """
-    Redeemer data hash
-    """
-    datum_hash: str = Field(
-        ..., example="923918e403bf43c34b4ef6b48eb2ee04babed17320d8d1b9ff9ad086e86f44ec"
-    )
-    """
-    Datum hash
-    """
-    unit_mem: str = Field(..., example="1700")
-    """
-    The budget in Memory to run a script
-    """
-    unit_steps: str = Field(..., example="476468")
-    """
-    The budget in CPU steps to run a script
-    """
-    fee: str = Field(..., example="172033")
-    """
-    The fee consumed to run the script
-    """
-
-
-class TxContentRedeemers(BaseModel):
-    __root__: List[TxContentRedeemer]
-
-
-class AccountContent(BaseModel):
-    stake_address: str = Field(
-        ..., example="stake1ux3g2c9dx2nhhehyrezyxpkstartcqmu9hk63qgfkccw5rqttygt7"
-    )
-    """
-    Bech32 stake address
-    """
-    active: bool = Field(..., example=True)
-    """
-    Registration state of an account
-    """
-    active_epoch: Optional[int] = Field(..., example=412)
-    """
-    Epoch of the most recent action - registration or deregistration
-    """
-    controlled_amount: str = Field(..., example="619154618165")
-    """
-    Balance of the account in Lovelaces
-    """
-    rewards_sum: str = Field(..., example="319154618165")
-    """
-    Sum of all rewards for the account in the Lovelaces
-    """
-    withdrawals_sum: str = Field(..., example="12125369253")
-    """
-    Sum of all the withdrawals for the account in Lovelaces
-    """
-    reserves_sum: str = Field(..., example="319154618165")
-    """
-    Sum of all  funds from reserves for the account in the Lovelaces
-    """
-    treasury_sum: str = Field(..., example="12000000")
-    """
-    Sum of all funds from treasury for the account in the Lovelaces
-    """
-    withdrawable_amount: str = Field(..., example="319154618165")
-    """
-    Sum of available rewards that haven't been withdrawn yet for the account in the Lovelaces
-    """
-    pool_id: Optional[str] = Field(
-        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
-    )
-    """
-    Bech32 pool ID that owns the account
-    """
-
-
-class Type(Enum):
-    """
-    Type of the reward
-    """
-
-    leader = "leader"
-    member = "member"
-    pool_deposit_refund = "pool_deposit_refund"
-
-
-class AccountRewardContentItem(BaseModel):
-    epoch: int
-    """
-    Epoch of the associated reward
-    """
-    amount: str
-    """
-    Rewards for given epoch in Lovelaces
-    """
-    pool_id: str
-    """
-    Bech32 pool ID being delegated to
-    """
-    type: Type
-    """
-    Type of the reward
-    """
-
-
-class AccountRewardContent(BaseModel):
-    __root__: List[AccountRewardContentItem] = Field(
-        ...,
-        example=[
-            {
-                "epoch": 215,
-                "amount": "12695385",
-                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
-                "type": "member",
-            },
-            {
-                "epoch": 216,
-                "amount": "3586329",
-                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
-                "type": "member",
-            },
-            {
-                "epoch": 217,
-                "amount": "1",
-                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
-                "type": "member",
-            },
-            {
-                "epoch": 217,
-                "amount": "1337",
-                "pool_id": "pool1cytwr0n7eas6du2h2xshl8ypa1yqr18f0erlhhjcuczysiunjcs",
-                "type": "leader",
-            },
-            {
-                "epoch": 218,
-                "amount": "1395265",
-                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
-                "type": "member",
-            },
-            {
-                "epoch": 218,
-                "amount": "500000000",
-                "pool_id": "pool1cytwr0n7eas6du2h2xshl8ypa1yqr18f0erlhhjcuczysiunjcs",
-                "type": "pool_deposit_refund",
-            },
-        ],
-    )
-
-
-class AccountHistoryContentItem(BaseModel):
-    active_epoch: int = Field(..., example=210)
-    """
-    Epoch in which the stake was active
-    """
-    amount: str
-    """
-    Stake amount in Lovelaces
-    """
-    pool_id: str
-    """
-    Bech32 ID of pool being delegated to
-    """
-
-
-class AccountHistoryContent(BaseModel):
-    __root__: List[AccountHistoryContentItem] = Field(
-        ...,
-        example=[
-            {
-                "active_epoch": 210,
-                "amount": "12695385",
-                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
-            },
-            {
-                "active_epoch": 211,
-                "amount": "22695385",
-                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
-            },
-        ],
-    )
-
-
-class AccountDelegationContentItem(BaseModel):
-    active_epoch: int = Field(..., example=210)
-    """
-    Epoch in which the delegation becomes active
-    """
-    tx_hash: str
-    """
-    Hash of the transaction containing the delegation
-    """
-    amount: str
-    """
-    Rewards for given epoch in Lovelaces
-    """
-    pool_id: str
-    """
-    Bech32 ID of pool being delegated to
-    """
-
-
-class AccountDelegationContent(BaseModel):
-    __root__: List[AccountDelegationContentItem] = Field(
-        ...,
-        example=[
-            {
-                "active_epoch": 210,
-                "tx_hash": "2dd15e0ef6e6a17841cb9541c27724072ce4d4b79b91e58432fbaa32d9572531",
-                "amount": "12695385",
-                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
-            },
-            {
-                "active_epoch": 242,
-                "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dde628516157f0",
-                "amount": "12691385",
-                "pool_id": "pool1kchver88u3kygsak8wgll7htr8uxn5v35lfrsyy842nkscrzyvj",
-            },
-        ],
-    )
-
-
-class Action(Enum):
-    """
-    Action in the certificate
-    """
-
-    registered = "registered"
-    deregistered = "deregistered"
-
-
-class AccountRegistrationContentItem(BaseModel):
-    tx_hash: str
-    """
-    Hash of the transaction containing the (de)registration certificate
-    """
-    action: Action
-    """
-    Action in the certificate
-    """
-
-
-class AccountRegistrationContent(BaseModel):
-    __root__: List[AccountRegistrationContentItem] = Field(
-        ...,
-        example=[
-            {
-                "tx_hash": "2dd15e0ef6e6a17841cb9541c27724072ce4d4b79b91e58432fbaa32d9572531",
-                "action": "registered",
-            },
-            {
-                "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dde628516157f0",
-                "action": "deregistered",
-            },
-        ],
-    )
-
-
-class AccountWithdrawalContentItem(BaseModel):
-    tx_hash: str
-    """
-    Hash of the transaction containing the withdrawal
-    """
-    amount: str
-    """
-    Withdrawal amount in Lovelaces
-    """
-
-
-class AccountWithdrawalContent(BaseModel):
-    __root__: List[AccountWithdrawalContentItem] = Field(
-        ...,
-        example=[
-            {
-                "tx_hash": "48a9625c841eea0dd2bb6cf551eabe6523b7290c9ce34be74eedef2dd8f7ecc5",
-                "amount": "454541212442",
-            },
-            {
-                "tx_hash": "4230b0cbccf6f449f0847d8ad1d634a7a49df60d8c142bb8cc2dbc8ca03d9e34",
-                "amount": "97846969",
-            },
-        ],
-    )
-
-
-class AccountMirContentItem(BaseModel):
-    tx_hash: str
-    """
-    Hash of the transaction containing the MIR
-    """
-    amount: str
-    """
-    MIR amount in Lovelaces
-    """
-
-
-class AccountMirContent(BaseModel):
-    __root__: List[AccountMirContentItem] = Field(
-        ...,
-        example=[
-            {
-                "tx_hash": "69705bba1d687a816ff5a04ec0c358a1f1ef075ab7f9c6cc2763e792581cec6d",
-                "amount": "2193707473",
-            },
-            {
-                "tx_hash": "baaa77b63d4d7d2bb3ab02c9b85978c2092c336dede7f59e31ad65452d510c13",
-                "amount": "14520198574",
-            },
-        ],
-    )
-
-
-class AccountAddressesContentItem(BaseModel):
-    address: str
-    """
-    Address associated with the stake key
-    """
-
-
-class AccountAddressesContent(BaseModel):
-    __root__: List[AccountAddressesContentItem] = Field(
-        ...,
-        example=[
-            {
-                "address": "addr1qx2kd28nq8ac5prwg32hhvudlwggpgfp8utlyqxu6wqgz62f79qsdmm5dsknt9ecr5w468r9ey0fxwkdrwh08ly3tu9sy0f4qd"
-            },
-            {
-                "address": "addr1qys3czp8s9thc6u2fqed9yq3h24nyw28uk0m6mkgn9dkckjf79qsdmm5dsknt9ecr5w468r9ey0fxwkdrwh08ly3tu9suth4w4"
-            },
-            {
-                "address": "addr1q8j55h253zcvl326sk5qdt2n8z7eghzspe0ekxgncr796s2f79qsdmm5dsknt9ecr5w468r9ey0fxwkdrwh08ly3tu9sjmd35m"
-            },
-            {
-                "address": "addr1q8f7gxrprank3drhx8k5grlux7ene0nlwun8y9thu8mc3yjf79qsdmm5dsknt9ecr5w468r9ey0fxwkdrwh08ly3tu9sls6vnt"
-            },
-        ],
-    )
-
-
-class AccountAddressesAsset(BaseModel):
-    """
-    The sum of all assets of all addresses associated with a given account
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-
-
-class AccountAddressesAssets(BaseModel):
-    __root__: List[AccountAddressesAsset] = Field(
-        ...,
-        example=[
-            {
-                "unit": "d5e6bf0500378d4f0da4e8dde6becec7621cd8cbf5cbb9b87013d4cc537061636542756433343132",
-                "quantity": "1",
-            },
-            {
-                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "125",
-            },
-        ],
-    )
-
-
-class ReceivedSumItem(BaseModel):
-    """
-    The sum of all the UTXO per asset for all addresses associated with the account
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-
-
-class SentSumItem(BaseModel):
-    """
-    The sum of all the UTXO per asset for all addresses associated with the account
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-
-
-class AccountAddressesTotal(BaseModel):
-    stake_address: str = Field(
-        ..., example="stake1u9l5q5jwgelgagzyt6nuaasefgmn8pd25c8e9qpeprq0tdcp0e3uk"
-    )
-    """
-    Bech32 encoded stake address
-    """
-    received_sum: List[ReceivedSumItem] = Field(
-        ...,
-        example=[
-            {"unit": "lovelace", "quantity": "42000000"},
-            {
-                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "12",
-            },
-        ],
-    )
-    sent_sum: List[SentSumItem] = Field(
-        ...,
-        example=[
-            {"unit": "lovelace", "quantity": "42000000"},
-            {
-                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "12",
-            },
-        ],
-    )
-    tx_count: int = Field(..., example=12)
-    """
-    Count of all transactions for all addresses associated with the account
-    """
-
-
-class MempoolContentItem(BaseModel):
-    tx_hash: str
-    """
-    Hash of the transaction
-    """
-
-
-class MempoolContent(BaseModel):
-    __root__: List[MempoolContentItem] = Field(
-        ...,
-        example=[
-            {
-                "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157f0"
-            }
-        ],
-    )
-
-
-class OutputAmountItem1(BaseModel):
-    """
-    The sum of all the UTXO per asset
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-
-
-class Tx(BaseModel):
-    hash: str = Field(
-        ..., example="1e043f100dce12d107f679685acd2fc0610e10f72a92d412794c9773d11d8477"
-    )
-    """
-    Transaction hash
-    """
-    output_amount: List[OutputAmountItem1] = Field(
-        ...,
-        example=[
-            {"unit": "lovelace", "quantity": "42000000"},
-            {
-                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "12",
-            },
-        ],
-    )
-    fees: str = Field(..., example="182485")
-    """
-    Fees of the transaction in Lovelaces
-    """
-    deposit: str = Field(..., example="0")
-    """
-    Deposit within the transaction in Lovelaces
-    """
-    size: int = Field(..., example=433)
-    """
-    Size of the transaction in Bytes
-    """
-    invalid_before: Optional[str]
-    """
-    Left (included) endpoint of the timelock validity intervals
-    """
-    invalid_hereafter: Optional[str] = Field(..., example="13885913")
-    """
-    Right (excluded) endpoint of the timelock validity intervals
-    """
-    utxo_count: int = Field(..., example=4)
-    """
-    Count of UTXOs within the transaction
-    """
-    withdrawal_count: int = Field(..., example=0)
-    """
-    Count of the withdrawals within the transaction
-    """
-    mir_cert_count: int = Field(..., example=0)
-    """
-    Count of the MIR certificates within the transaction
-    """
-    delegation_count: int = Field(..., example=0)
-    """
-    Count of the delegations within the transaction
-    """
-    stake_cert_count: int = Field(..., example=0)
-    """
-    Count of the stake keys (de)registration within the transaction
-    """
-    pool_update_count: int = Field(..., example=0)
-    """
-    Count of the stake pool registration and update certificates within the transaction
-    """
-    pool_retire_count: int = Field(..., example=0)
-    """
-    Count of the stake pool retirement certificates within the transaction
-    """
-    asset_mint_or_burn_count: int = Field(..., example=0)
-    """
-    Count of asset mints and burns within the transaction
-    """
-    redeemer_count: int = Field(..., example=0)
-    """
-    Count of redeemers within the transaction
-    """
-    valid_contract: bool = Field(..., example=True)
-    """
-    True if contract script passed validation
-    """
-
-
-class Input1(BaseModel):
-    address: Optional[str] = Field(
-        None,
-        example="addr1q9ld26v2lv8wvrxxmvg90pn8n8n5k6tdst06q2s856rwmvnueldzuuqmnsye359fqrk8hwvenjnqultn7djtrlft7jnq7dy7wv",
-    )
-    """
-    Input address
-    """
-    tx_hash: str = Field(
-        ..., example="1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157f0"
-    )
-    """
-    Hash of the UTXO transaction
-    """
-    output_index: int = Field(..., example=0)
-    """
-    UTXO index in the transaction
-    """
-    collateral: bool = Field(..., example=False)
-    """
-    Whether the input is a collateral consumed on script validation failure
-    """
-    reference: Optional[bool] = Field(None, example=False)
-    """
-    Whether the input is a reference transaction input
-    """
-
-
-class AmountItem2(BaseModel):
-    """
-    The sum of all the UTXO per asset
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-
-
-class Output1(BaseModel):
-    address: str = Field(
-        ...,
-        example="addr1q9ld26v2lv8wvrxxmvg90pn8n8n5k6tdst06q2s856rwmvnueldzuuqmnsye359fqrk8hwvenjnqultn7djtrlft7jnq7dy7wv",
-    )
-    """
-    Output address
-    """
-    amount: List[AmountItem2] = Field(
-        ...,
-        example=[
-            {"unit": "lovelace", "quantity": "42000000"},
-            {
-                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "12",
-            },
-        ],
-    )
-    output_index: int = Field(..., example=0)
-    """
-    UTXO index in the transaction
-    """
-    data_hash: Optional[str] = Field(
-        ..., example="9e478573ab81ea7a8e31891ce0648b81229f408d596a3483e6f4f9b92d3cf710"
-    )
-    """
-    The hash of the transaction output datum
-    """
-    inline_datum: Optional[str] = Field(..., example="19a6aa")
-    """
-    CBOR encoded inline datum
-    """
-    collateral: bool = Field(..., example=False)
-    """
-    Whether the output is a collateral output
-    """
-    reference_script_hash: Optional[str] = Field(
-        ..., example="13a3efd825703a352a8f71f4e2758d08c28c564e8dfcce9f77776ad1"
-    )
-    """
-    The hash of the reference script of the output
-    """
-
-
-class Purpose1(Enum):
-    """
-    Validation purpose
-    """
-
-    spend = "spend"
-    mint = "mint"
-    cert = "cert"
-    reward = "reward"
-
-
-class Redeemer(BaseModel):
-    tx_index: int = Field(..., example=0)
-    """
-    Index of the redeemer within the transaction
-    """
-    purpose: Purpose1 = Field(..., example="spend")
-    """
-    Validation purpose
-    """
-    unit_mem: str = Field(..., example="1700")
-    """
-    The budget in Memory to run a script
-    """
-    unit_steps: str = Field(..., example="476468")
-    """
-    The budget in CPU steps to run a script
-    """
-
-
-class MempoolTxContent(BaseModel):
-    tx: Tx
-    inputs: List[Input1]
-    outputs: List[Output1]
-    redeemers: Optional[List[Redeemer]] = None
-
-
-class MempoolAddressesContentItem(BaseModel):
-    tx_hash: str
-    """
-    Hash of the transaction
-    """
-
-
-class MempoolAddressesContent(BaseModel):
-    __root__: List[MempoolAddressesContentItem] = Field(
-        ...,
-        example=[
-            {
-                "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157f0"
-            }
-        ],
-    )
-
-
-class TxMetadataLabel(BaseModel):
-    label: str
-    """
-    Metadata label
-    """
-    cip10: Optional[str]
-    """
-    CIP10 defined description
-    """
-    count: str
-    """
-    The count of metadata entries with a specific label
-    """
-
-
-class TxMetadataLabels(BaseModel):
-    __root__: List[TxMetadataLabel] = Field(
-        ...,
-        example=[
-            {"label": "1990", "cip10": None, "count": "1"},
-            {
-                "label": "1967",
-                "cip10": "nut.link metadata oracles registry",
-                "count": "3",
-            },
-            {
-                "label": "1968",
-                "cip10": "nut.link metadata oracles data points",
-                "count": "16321",
-            },
-        ],
-    )
-
-
-class TxMetadataLabelJsonItem(BaseModel):
-    tx_hash: str
-    """
-    Transaction hash that contains the specific metadata
-    """
-    json_metadata: Optional[Union[str, Dict[str, Any], List, int, float, bool]]
-    """
-    Content of the JSON metadata
-    """
-
-
-class TxMetadataLabelJson(BaseModel):
-    __root__: List[TxMetadataLabelJsonItem] = Field(
-        ...,
-        example=[
-            {
-                "tx_hash": "257d75c8ddb0434e9b63e29ebb6241add2b835a307aa33aedba2effe09ed4ec8",
-                "json_metadata": {
-                    "ADAUSD": [
-                        {"value": "0.10409800535729975", "source": "ergoOracles"}
-                    ]
-                },
-            },
-            {
-                "tx_hash": "e865f2cc01ca7381cf98dcdc4de07a5e8674b8ea16e6a18e3ed60c186fde2b9c",
-                "json_metadata": {
-                    "ADAUSD": [
-                        {"value": "0.15409850555139935", "source": "ergoOracles"}
-                    ]
-                },
-            },
-            {
-                "tx_hash": "4237501da3cfdd53ade91e8911e764bd0699d88fd43b12f44a1f459b89bc91be",
-                "json_metadata": None,
-            },
-        ],
-    )
-
-
-class TxMetadataLabelCborItem(BaseModel):
-    tx_hash: str
-    """
-    Transaction hash that contains the specific metadata
-    """
-    cbor_metadata: Optional[str]
-    """
-    Content of the CBOR metadata
-    """
-    metadata: Optional[str]
-    """
-    Content of the CBOR metadata in hex
-    """
-
-
-class TxMetadataLabelCbor(BaseModel):
-    __root__: List[TxMetadataLabelCborItem] = Field(
-        ...,
-        example=[
-            {
-                "tx_hash": "257d75c8ddb0434e9b63e29ebb6241add2b835a307aa33aedba2effe09ed4ec8",
-                "cbor_metadata": None,
-                "metadata": None,
-            },
-            {
-                "tx_hash": "e865f2cc01ca7381cf98dcdc4de07a5e8674b8ea16e6a18e3ed60c186fde2b9c",
-                "cbor_metadata": None,
-                "metadata": None,
-            },
-            {
-                "tx_hash": "4237501da3cfdd53ade91e8911e764bd0699d88fd43b12f44a1f459b89bc91be",
-                "cbor_metadata": "\\xa100a16b436f6d62696e6174696f6e8601010101010c",
-                "metadata": "a100a16b436f6d62696e6174696f6e8601010101010c",
-            },
-        ],
-    )
-
-
-class AmountItem3(BaseModel):
-    """
-    The sum of all the UTXO per asset
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-
-
-class Type1(Enum):
-    """
-    Address era
-    """
-
-    byron = "byron"
-    shelley = "shelley"
-
-
-class AddressContent(BaseModel):
-    address: str = Field(
-        ...,
-        example="addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
-    )
-    """
-    Bech32 encoded addresses
-    """
-    amount: List[AmountItem3] = Field(
-        ...,
-        example=[
-            {"unit": "lovelace", "quantity": "42000000"},
-            {
-                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "12",
-            },
-        ],
-    )
-    stake_address: Optional[str] = Field(
-        ..., example="stake1ux3g2c9dx2nhhehyrezyxpkstartcqmu9hk63qgfkccw5rqttygt7"
-    )
-    """
-    Stake address that controls the key
-    """
-    type: Type1 = Field(..., example="shelley")
-    """
-    Address era
-    """
-    script: bool = Field(..., example=False)
-    """
-    True if this is a script address
-    """
-
-
-class AmountItem4(BaseModel):
-    """
-    The sum of all the UTXO per asset
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-    decimals: Optional[int]
-    """
-    Number of decimal places of the asset unit. Primary data source is CIP68 reference NFT with a fallback to off-chain metadata.
-    """
-    has_nft_onchain_metadata: bool
-    """
-    True if the latest minting transaction includes metadata (best-effort)
-    """
-
-
-class Type2(Enum):
-    """
-    Address era
-    """
-
-    byron = "byron"
-    shelley = "shelley"
-
-
-class AddressContentExtended(BaseModel):
-    address: str = Field(
-        ...,
-        example="addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
-    )
-    """
-    Bech32 encoded addresses
-    """
-    amount: List[AmountItem4] = Field(
-        ...,
-        example=[
-            {
-                "unit": "lovelace",
-                "quantity": "42000000",
-                "decimals": 6,
-                "has_nft_onchain_metadata": False,
-            },
-            {
-                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "12",
-                "decimals": None,
-                "has_nft_onchain_metadata": True,
-            },
-        ],
-    )
-    stake_address: Optional[str] = Field(
-        ..., example="stake1ux3g2c9dx2nhhehyrezyxpkstartcqmu9hk63qgfkccw5rqttygt7"
-    )
-    """
-    Stake address that controls the key
-    """
-    type: Type2 = Field(..., example="shelley")
-    """
-    Address era
-    """
-    script: bool = Field(..., example=False)
-    """
-    True if this is a script address
-    """
-
-
-class ReceivedSumItem1(BaseModel):
-    """
-    The sum of all the UTXO per asset
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-
-
-class SentSumItem1(BaseModel):
-    """
-    The sum of all the UTXO per asset
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-
-
-class AddressContentTotal(BaseModel):
-    address: str = Field(
-        ...,
-        example="addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
-    )
-    """
-    Bech32 encoded address
-    """
-    received_sum: List[ReceivedSumItem1] = Field(
-        ...,
-        example=[
-            {"unit": "lovelace", "quantity": "42000000"},
-            {
-                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "12",
-            },
-        ],
-    )
-    sent_sum: List[SentSumItem1] = Field(
-        ...,
-        example=[
-            {"unit": "lovelace", "quantity": "42000000"},
-            {
-                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "12",
-            },
-        ],
-    )
-    tx_count: int = Field(..., example=12)
-    """
-    Count of all transactions on the address
-    """
-
-
-class AmountItem5(BaseModel):
-    """
-    The sum of all the UTXO per asset
-    """
-
-    unit: str
-    """
-    The unit of the value
-    """
-    quantity: str
-    """
-    The quantity of the unit
-    """
-
-
-class AddressUtxoContentItem(BaseModel):
-    address: str = Field(
-        ...,
-        example="addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
-    )
-    """
-    Bech32 encoded addresses - useful when querying by payment_cred
-    """
-    tx_hash: str
-    """
-    Transaction hash of the UTXO
-    """
-    tx_index: int
-    """
-    UTXO index in the transaction
-    """
-    output_index: int
-    """
-    UTXO index in the transaction
-    """
-    amount: List[AmountItem5]
-    block: str
-    """
-    Block hash of the UTXO
-    """
-    data_hash: Optional[str]
-    """
-    The hash of the transaction output datum
-    """
-    inline_datum: Optional[str] = Field(..., example="19a6aa")
-    """
-    CBOR encoded inline datum
-    """
-    reference_script_hash: Optional[str] = Field(
-        ..., example="13a3efd825703a352a8f71f4e2758d08c28c564e8dfcce9f77776ad1"
-    )
-    """
-    The hash of the reference script of the output
-    """
-
-
-class AddressUtxoContent(BaseModel):
-    __root__: List[AddressUtxoContentItem] = Field(
-        ...,
-        example=[
-            {
-                "address": "addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
-                "tx_hash": "39a7a284c2a0948189dc45dec670211cd4d72f7b66c5726c08d9b3df11e44d58",
-                "output_index": 0,
-                "amount": [{"unit": "lovelace", "quantity": "42000000"}],
-                "block": "7eb8e27d18686c7db9a18f8bbcfe34e3fed6e047afaa2d969904d15e934847e6",
-                "data_hash": "9e478573ab81ea7a8e31891ce0648b81229f408d596a3483e6f4f9b92d3cf710",
-                "inline_datum": None,
-                "reference_script_hash": None,
-            },
-            {
-                "address": "addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
-                "tx_hash": "4c4e67bafa15e742c13c592b65c8f74c769cd7d9af04c848099672d1ba391b49",
-                "output_index": 0,
-                "amount": [{"unit": "lovelace", "quantity": "729235000"}],
-                "block": "953f1b80eb7c11a7ffcd67cbd4fde66e824a451aca5a4065725e5174b81685b7",
-                "data_hash": None,
-                "inline_datum": None,
-                "reference_script_hash": None,
-            },
-            {
-                "address": "addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
-                "tx_hash": "768c63e27a1c816a83dc7b07e78af673b2400de8849ea7e7b734ae1333d100d2",
-                "output_index": 1,
-                "amount": [
-                    {"unit": "lovelace", "quantity": "42000000"},
-                    {
-                        "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                        "quantity": "12",
-                    },
-                ],
-                "block": "5c571f83fe6c784d3fbc223792627ccf0eea96773100f9aedecf8b1eda4544d7",
-                "data_hash": None,
-                "inline_datum": None,
-                "reference_script_hash": None,
-            },
-        ],
-    )
-
-
-class AddressTxsContent(BaseModel):
-    __root__: List[str] = Field(
-        ...,
-        example=[
-            "2dd15e0ef6e6a17841cb9541c27724072ce4d4b79b91e58432fbaa32d9572531",
-            "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dde628516157f0",
-        ],
-    )
-
-
-class AddressTransactionsContentItem(BaseModel):
-    tx_hash: str
-    """
-    Hash of the transaction
-    """
-    tx_index: int
-    """
-    Transaction index within the block
-    """
-    block_height: int
-    """
-    Block height
-    """
-    block_time: int
-    """
-    Block creation time in UNIX time
-    """
-
-
-class AddressTransactionsContent(BaseModel):
-    __root__: List[AddressTransactionsContentItem] = Field(
-        ...,
-        example=[
-            {
-                "tx_hash": "8788591983aa73981fc92d6cddbbe643959f5a784e84b8bee0db15823f575a5b",
-                "tx_index": 6,
-                "block_height": 69,
-                "block_time": 1635505891,
-            },
-            {
-                "tx_hash": "52e748c4dec58b687b90b0b40d383b9fe1f24c1a833b7395cdf07dd67859f46f",
-                "tx_index": 9,
-                "block_height": 4547,
-                "block_time": 1635505987,
-            },
-            {
-                "tx_hash": "e8073fd5318ff43eca18a852527166aa8008bee9ee9e891f585612b7e4ba700b",
-                "tx_index": 0,
-                "block_height": 564654,
-                "block_time": 1834505492,
-            },
-        ],
-    )
-
-
-class PoolList(BaseModel):
-    __root__: List[str] = Field(
-        ...,
-        example=[
-            "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
-            "pool1hn7hlwrschqykupwwrtdfkvt2u4uaxvsgxyh6z63703p2knj288",
-            "pool1ztjyjfsh432eqetadf82uwuxklh28xc85zcphpwq6mmezavzad2",
-        ],
-    )
-
-
-class PoolListExtendedItem(BaseModel):
-    pool_id: str = Field(
-        ..., example="pool1z5uqdk7dzdxaae5633fqfcu2eqzy3a3rgtuvy087fdld7yws0xt"
-    )
-    """
-    Bech32 encoded pool ID
-    """
-    hex: str = Field(
-        ..., example="0f292fcaa02b8b2f9b3c8f9fd8e0bb21abedb692a6d5058df3ef2735"
-    )
-    """
-    Hexadecimal pool ID.
-    """
-    active_stake: str = Field(..., example="4200000000")
-    """
-    Active delegated amount
-    """
-    live_stake: str = Field(..., example="6900000000")
-    """
-    Currently delegated amount
-    """
-
-
-class PoolListExtended(BaseModel):
-    __root__: List[PoolListExtendedItem] = Field(
-        ...,
-        example=[
-            {
-                "pool_id": "pool19u64770wqp6s95gkajc8udheske5e6ljmpq33awxk326zjaza0q",
-                "hex": "2f355f79ee007502d116ecb07e36f985b34cebf2d84118f5c6b455a1",
-                "active_stake": "1541200000",
-                "live_stake": "1541400000",
-            },
-            {
-                "pool_id": "pool1dvla4zq98hpvacv20snndupjrqhuc79zl6gjap565nku6et5zdx",
-                "hex": "6b3fda88053dc2cee18a7c2736f032182fcc78a2fe912e869aa4edcd",
-                "active_stake": "22200000",
-                "live_stake": "48955550",
-            },
-            {
-                "pool_id": "pool1wvccajt4eugjtf3k0ja3exjqdj7t8egsujwhcw4tzj4rzsxzw5w",
-                "hex": "73318ec975cf1125a6367cbb1c9a406cbcb3e510e49d7c3aab14aa31",
-                "active_stake": "9989541215",
-                "live_stake": "168445464878",
-            },
-        ],
-    )
-
-
-class PoolListRetireItem(BaseModel):
-    pool_id: str = Field(
-        ..., example="pool1z5uqdk7dzdxaae5633fqfcu2eqzy3a3rgtuvy087fdld7yws0xt"
-    )
-    """
-    Bech32 encoded pool ID
-    """
-    epoch: int = Field(..., example=242)
-    """
-    Retirement epoch number
-    """
-
-
-class PoolListRetire(BaseModel):
-    __root__: List[PoolListRetireItem] = Field(
-        ...,
-        example=[
-            {
-                "pool_id": "pool19u64770wqp6s95gkajc8udheske5e6ljmpq33awxk326zjaza0q",
-                "epoch": 225,
-            },
-            {
-                "pool_id": "pool1dvla4zq98hpvacv20snndupjrqhuc79zl6gjap565nku6et5zdx",
-                "epoch": 215,
-            },
-            {
-                "pool_id": "pool1wvccajt4eugjtf3k0ja3exjqdj7t8egsujwhcw4tzj4rzsxzw5w",
-                "epoch": 231,
-            },
-        ],
-    )
-
-
-class Pool(BaseModel):
-    pool_id: str = Field(
-        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
-    )
-    """
-    Bech32 pool ID
-    """
-    hex: str = Field(
-        ..., example="0f292fcaa02b8b2f9b3c8f9fd8e0bb21abedb692a6d5058df3ef2735"
-    )
-    """
-    Hexadecimal pool ID.
-    """
-    vrf_key: str = Field(
-        ..., example="0b5245f9934ec2151116fb8ec00f35fd00e0aa3b075c4ed12cce440f999d8233"
-    )
-    """
-    VRF key hash
-    """
-    blocks_minted: int = Field(..., example=69)
-    """
-    Total minted blocks
-    """
-    blocks_epoch: int = Field(..., example=4)
-    """
-    Number of blocks minted in the current epoch
-    """
-    live_stake: str = Field(..., example="6900000000")
-    live_size: float = Field(..., example=0.42)
-    live_saturation: float = Field(..., example=0.93)
-    live_delegators: float = Field(..., example=127)
-    active_stake: str = Field(..., example="4200000000")
-    active_size: float = Field(..., example=0.43)
-    declared_pledge: str = Field(..., example="5000000000")
-    """
-    Stake pool certificate pledge
-    """
-    live_pledge: str = Field(..., example="5000000001")
-    """
-    Stake pool current pledge
-    """
-    margin_cost: float = Field(..., example=0.05)
-    """
-    Margin tax cost of the stake pool
-    """
-    fixed_cost: str = Field(..., example="340000000")
-    """
-    Fixed tax cost of the stake pool
-    """
-    reward_account: str = Field(
-        ..., example="stake1uxkptsa4lkr55jleztw43t37vgdn88l6ghclfwuxld2eykgpgvg3f"
-    )
-    """
-    Bech32 reward account of the stake pool
-    """
-    owners: List[str] = Field(
-        ..., example=["stake1u98nnlkvkk23vtvf9273uq7cph5ww6u2yq2389psuqet90sv4xv9v"]
-    )
-    registration: List[str] = Field(
-        ...,
-        example=[
-            "9f83e5484f543e05b52e99988272a31da373f3aab4c064c76db96643a355d9dc",
-            "7ce3b8c433bf401a190d58c8c483d8e3564dfd29ae8633c8b1b3e6c814403e95",
-            "3e6e1200ce92977c3fe5996bd4d7d7e192bcb7e231bc762f9f240c76766535b9",
-        ],
-    )
-    retirement: List[str]
-
-
-class PoolHistoryItem(BaseModel):
-    epoch: int = Field(..., example=233)
-    """
-    Epoch number
-    """
-    blocks: int = Field(..., example=22)
-    """
-    Number of blocks created by pool
-    """
-    active_stake: str = Field(..., example="20485965693569")
-    """
-    Active (Snapshot of live stake 2 epochs ago) stake in Lovelaces
-    """
-    active_size: float = Field(..., example=1.2345)
-    """
-    Pool size (percentage) of overall active stake at that epoch
-    """
-    delegators_count: int = Field(..., example=115)
-    """
-    Number of delegators for epoch
-    """
-    rewards: str = Field(..., example="206936253674159")
-    """
-    Total rewards received before distribution to delegators
-    """
-    fees: str = Field(..., example="1290968354")
-    """
-    Pool operator rewards
-    """
-
-
-class PoolHistory(BaseModel):
-    __root__: List[PoolHistoryItem]
-
-
-class PoolMetadata(BaseModel):
-    pool_id: str = Field(
-        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
-    )
-    """
-    Bech32 pool ID
-    """
-    hex: str = Field(
-        ..., example="0f292fcaa02b8b2f9b3c8f9fd8e0bb21abedb692a6d5058df3ef2735"
-    )
-    """
-    Hexadecimal pool ID
-    """
-    url: Optional[str] = Field(..., example="https://stakenuts.com/mainnet.json")
-    """
-    URL to the stake pool metadata
-    """
-    hash: Optional[str] = Field(
-        ..., example="47c0c68cb57f4a5b4a87bad896fc274678e7aea98e200fa14a1cb40c0cab1d8c"
-    )
-    """
-    Hash of the metadata file
-    """
-    ticker: Optional[str] = Field(..., example="NUTS")
-    """
-    Ticker of the stake pool
-    """
-    name: Optional[str] = Field(..., example="Stake Nuts")
-    """
-    Name of the stake pool
-    """
-    description: Optional[str] = Field(..., example="The best pool ever")
-    """
-    Description of the stake pool
-    """
-    homepage: Optional[str] = Field(..., example="https://stakentus.com/")
-    """
-    Home page of the stake pool
-    """
-
-
-class EmptyObject(BaseModel):
-    pass
-
-
-class PoolRelay(BaseModel):
-    ipv4: Optional[str] = Field(..., example="4.4.4.4")
-    """
-    IPv4 address of the relay
-    """
-    ipv6: Optional[str] = Field(..., example="https://stakenuts.com/mainnet.json")
-    """
-    IPv6 address of the relay
-    """
-    dns: Optional[str] = Field(..., example="relay1.stakenuts.com")
-    """
-    DNS name of the relay
-    """
-    dns_srv: Optional[str] = Field(..., example="_relays._tcp.relays.stakenuts.com")
-    """
-    DNS SRV entry of the relay
-    """
-    port: int = Field(..., example=3001)
-    """
-    Network port of the relay
-    """
-
-
-class PoolRelays(BaseModel):
-    __root__: List[PoolRelay]
-
-
-class PoolDelegator(BaseModel):
-    address: str
-    """
-    Bech32 encoded stake addresses
-    """
-    live_stake: str
-    """
-    Currently delegated amount
-    """
-
-
-class PoolDelegators(BaseModel):
-    __root__: List[PoolDelegator] = Field(
-        ...,
-        example=[
-            {
-                "address": "stake1ux4vspfvwuus9uwyp5p3f0ky7a30jq5j80jxse0fr7pa56sgn8kha",
-                "live_stake": "1137959159981411",
-            },
-            {
-                "address": "stake1uylayej7esmarzd4mk4aru37zh9yz0luj3g9fsvgpfaxulq564r5u",
-                "live_stake": "16958865648",
-            },
-            {
-                "address": "stake1u8lr2pnrgf8f7vrs9lt79hc3sxm8s2w4rwvgpncks3axx6q93d4ck",
-                "live_stake": "18605647",
-            },
-        ],
-    )
-
-
-class PoolBlocks(BaseModel):
-    __root__: List[str] = Field(
-        ...,
-        example=[
-            "d8982ca42cfe76b747cc681d35d671050a9e41e9cfe26573eb214e94fe6ff21d",
-            "026436c539e2ce84c7f77ffe669f4e4bbbb3b9c53512e5857dcba8bb0b4e9a8c",
-            "bcc8487f419b8c668a18ea2120822a05df6dfe1de1f0fac3feba88cf760f303c",
-            "86bf7b4a274e0f8ec9816171667c1b4a0cfc661dc21563f271acea9482b62df7",
-        ],
-    )
-
-
-class Action1(Enum):
-    """
-    Action in the certificate
-    """
-
-    registered = "registered"
-    deregistered = "deregistered"
-
-
-class PoolUpdate(BaseModel):
-    tx_hash: str
-    """
-    Transaction ID
-    """
-    cert_index: int
-    """
-    Certificate within the transaction
-    """
-    action: Action1
-    """
-    Action in the certificate
-    """
-
-
-class PoolUpdates(BaseModel):
-    __root__: List[PoolUpdate] = Field(
-        ...,
-        example=[
-            {
-                "tx_hash": "6804edf9712d2b619edb6ac86861fe93a730693183a262b165fcc1ba1bc99cad",
-                "cert_index": 0,
-                "action": "registered",
-            },
-            {
-                "tx_hash": "9c190bc1ac88b2ab0c05a82d7de8b71b67a9316377e865748a89d4426c0d3005",
-                "cert_index": 0,
-                "action": "deregistered",
-            },
-            {
-                "tx_hash": "e14a75b0eb2625de7055f1f580d70426311b78e0d36dd695a6bdc96c7b3d80e0",
-                "cert_index": 1,
-                "action": "registered",
-            },
-        ],
-    )
-
-
-class Asset(BaseModel):
-    asset: str
-    """
-    Asset identifier
-    """
-    quantity: str
-    """
-    Current asset quantity
-    """
-
-
-class Assets(BaseModel):
-    __root__: List[Asset] = Field(
-        ...,
-        example=[
-            {
-                "asset": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "1",
-            },
-            {
-                "asset": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e75d",
-                "quantity": "100000",
-            },
-            {
-                "asset": "6804edf9712d2b619edb6ac86861fe93a730693183a262b165fcc1ba1bc99cad",
-                "quantity": "18605647",
-            },
-        ],
-    )
-
-
-class OnchainMetadataStandard(Enum):
-    """
-    If on-chain metadata passes validation, we display the standard
-    under which it is valid
-
-    """
-
-    CIP25v1 = "CIP25v1"
-    CIP25v2 = "CIP25v2"
-    CIP68v1 = "CIP68v1"
-
-
-class Metadata1(BaseModel):
-    """
-    Off-chain metadata fetched from GitHub based on network.
-    Mainnet: https://github.com/cardano-foundation/cardano-token-registry/
-    Testnet: https://github.com/input-output-hk/metadata-registry-testnet/
-
-    """
-
-    name: str = Field(..., example="nutcoin")
-    """
-    Asset name
-    """
-    description: str = Field(..., example="The Nut Coin")
-    """
-    Asset description
-    """
-    ticker: Optional[str] = Field(..., example="nutc")
-    url: Optional[str] = Field(..., example="https://www.stakenuts.com/")
-    """
-    Asset website
-    """
-    logo: Optional[str] = Field(
-        ...,
-        example="iVBORw0KGgoAAAANSUhEUgAAADAAAAAoCAYAAAC4h3lxAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAABmJLR0QA/wD/AP+gvaeTAAAAB3RJTUUH5QITCDUPjqwFHwAAB9xJREFUWMPVWXtsU9cZ/8499/r6dZ3E9rUdO7ZDEgglFWO8KaOsJW0pCLRKrN1AqqYVkqoqrYo0ja7bpElru1WairStFKY9WzaE1E1tx+jokKqwtqFNyhKahEJJyJNgJ37E9r1+3HvO/sFR4vhx7SBtfH/F3/l93/f7ne/4PBxEKYU72dj/ZfH772v1TU+HtqbTaX8wOO01GPQpRVH7JEm+vGHDuq6z7/8jUSoHKtaBKkEUFUXdajDy1hUrmrs6zn/wWS7m7pZVjMUirKGUTnzc+e9xLcTrPPVfZzDz06Sc2lyQGEIyAPzT7Xa+dvE/3e+XLaCxoflHsVj8MAAYs74aa/WHoenwvpkZKeFy2Z5NJlOPUkqXZccFwSSrKjlyffjLH+TL6XTUGTGL/6hklD3ldIrj2M5MRmkLBMcvaRLQ1Nj88sxM/HCBfMP+eu/OYGDqe6l0WmpoqJ/88upgrU7HrQNA/cFg6MlkKiLlBtVUO40cx54BgHvLIT/HJLvdeqh/4NKxogKWN7fsCoUi7xTLxLJ4vLq6ak//wKVOrdXtttrTDMPsqJA8AAAwDErdu3VL3alTf5ma9eWCpoKhn5dKpCiqJxicPucQPVu0FHaInn35yHMcKwPAa4SQ3QCwFgDWUko3qSr5vqqSgTypuEg4Mo/zvA74/Y0rZSnZU8akSHV17k2fXfy0txjI5224kEym1s/1EUI7LBbztweHrkzkizn49LP6U6feepFSeggAQK/n04SQZ8bGrxdeQjZrbRvGzLH5hcibRqOhPplMfS1fIY5jz4xPDBdcGggho2h3z9sOLRazdG3wqp9SMgUlzGZ17SSEPsRx7J8CwfGu3PF57WhqqjfN/VxVJUxKUrIdITAXKpDJKFscosdfaFy0u+/K9aXTmXe0kAcAmA5Nng5Hbj6Tj/wCAYFAcN7uEY3GXGazMSHLqVVFapgBoMPna9yqhRAAgCTJMa3YUjZPgNFkSlWYx5eUkx+0tKx83V3rF+cVYJjruWCe133DIXqMmrNrFSDabRcWkywYmG5XFOW6aHcfb9324CoAgMmbo9MIoXkneCajiAihV/c/8eSiBSw4BxyiZxQA6m7H7FBKT2CMn2MY5jFFUX6ZO+5w2j8aHZ7YH40FByrJD5DnHGAY5uTtIA8AgBDaR4F2Yxb3WizCgmtA4ObUPSazodduqz3Suu0hf0U1cjvgdNSJ1dWWveFwdDUAtAiC2Uopdcdi8c9Zlh3GmDGl05mtAKAvo47EcdwThJCjqqpWFxALlNITomg73tff21GRAJez7iVK4WGGYfoJIQduBsbm7UrLm1ueCoUiv65kpiilw1ZbzcFoZOYoIcRTAn6eYZgXJm+Oni+Vd3YJbdyweSch9HlK6SpVVfcyDDq7Yf3m2XPBIXraKyV/a4b9UkLawbLsZgB4rwR8CyGkw13r+5fX27BckwBAEJ47oKpk8+DgUIdod7fV1vqOAMDrlZLPmqKoB+rrvXIgOP6w0WjYy3Ls5RL4bUk52bVm9fqnCk7M3CXU2ND8+MxM7BcIIftiyRYyntcdHh0bmr0wfmXl6p2SJB2KRmP3l4j7zejYUFtRAQAAgslm1Bv4nyGEDpYiIwjmjw0G/RjP866JiclNqqqWfKLq9fyZkdHBBXcnl9O71GDgD8bj0ncRQqZ8sRgzL9yYHH2pqICsOUTPLgA4CXNeZFmzWIS/YhYfjUZmvqPjuceSckrz25pS2h2cmlhbaBwhzr6kfsnL8Xhif55YYFl23Y3Jkdl7EVMoUSA4/q6qqNsBIPd11e52u45FwtG3CSH7yiEPAGC1Vt9dXGBmanDoygFLlbAjtzZCCMyC6VeaOpA1l9N7l1kwtauKaozHE28YTQaQpeR7+TqjxXheR0fHhhgt2CX1S3clEtKC16HL5djYe+niBU0CcmYA2W21/Qih5ZqDcoxlMZ24MaJJAABA87IVJ8Lh6N65Pr1B/+LIyLUfAhRZQvnM6ah7ZDHkAQB0vK6/HHxNTc2ruT5Zkldn/y5LACFk+2LIAwAwCGl6yGSt88KHXbmrBCHkqEgAz+vWLFZALJb4qNwYhFDhCSknkSwnQ4sVgDFeWg7+gQe2r1tAmkGTFQlACHWVg89nhJA9ot3dphV/eeCLp/Pw6K5IQP0S39uLFXCLwDG7zf1cKZxD9LSlUunHc/12u/2t2Vzl/rzu8zb8PZlM7bwdQgDgPK/nX2nddt+53//ht3LW2dS0fF0iLj2vquojuQFmwXRucPBKa8UCmpe1iOFwpAsAfLdJBFBKwVIlXJ2JxqKCxbwyHkvoCkAlv9/71U+7Oq+UJWDZ0hViJBL1cRynbNq0sSeeiPl6ei4NqIqq6TSmlB7X6bjuTEY5pgWfzwxGPZhMpt39/b3vzvWXFGCzulZjjM/DrauDwcAr8bjcgzGjZUuVBMH8k2uDX7wCAFDr8n2LEPI7SqmhTP6SzVbz6MDlz0/nDpT8EmOM22HOvUeWU2wp8iyLgRL6hk7Hrc2SBwC4MTlykmXZRozxn00mbVcphNA5jJmV+chr6oDd5l6jN/A/TqfSuwEAGITGMIsvGo3GTwTB3Dc2NjGSxdZYq4VIOOoNBANnKE0XPXE3brjHOTQ08k2MmVZOxzVJCbkFIQSCYEphzPaFQuGzTpfjb319PZ8UFXin/5OvrHPg/9HueAH/BSUqOuNZm4fyAAAAJXRFWHRkYXRlOmNyZWF0ZQAyMDIxLTAyLTE5VDA4OjUyOjI1KzAwOjAwCmFGlgAAACV0RVh0ZGF0ZTptb2RpZnkAMjAyMS0wMi0xOVQwODo1MjoyMyswMDowMBjsyxAAAAAASUVORK5CYII=",
-    )
-    """
-    Base64 encoded logo of the asset
-    """
-    decimals: Optional[int] = Field(..., example=6, le=255.0)
-    """
-    Number of decimal places of the asset unit
-    """
-
-
-class Asset1(BaseModel):
-    asset: str = Field(
-        ...,
-        example="b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-    )
-    """
-    Hex-encoded asset full name
-    """
-    policy_id: str = Field(
-        ..., example="b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a7"
-    )
-    """
-    Policy ID of the asset
-    """
-    asset_name: Optional[str] = Field(..., example="6e7574636f696e")
-    """
-    Hex-encoded asset name of the asset
-    """
-    fingerprint: str = Field(
-        ..., example="asset1pkpwyknlvul7az0xx8czhl60pyel45rpje4z8w"
-    )
-    """
-    CIP14 based user-facing fingerprint
-    """
-    quantity: str = Field(..., example="12000")
-    """
-    Current asset quantity
-    """
-    initial_mint_tx_hash: str = Field(
-        ..., example="6804edf9712d2b619edb6ac86861fe93a730693183a262b165fcc1ba1bc99cad"
-    )
-    """
-    ID of the initial minting transaction
-    """
-    mint_or_burn_count: int = Field(..., example=1)
-    """
-    Count of mint and burn transactions
-    """
-    onchain_metadata: Optional[Dict[str, Any]]
-    """
-    On-chain metadata which SHOULD adhere to the valid standards,
-    based on which we perform the look up and display the asset
-    (best effort)
-
-    """
-    onchain_metadata_standard: Optional[OnchainMetadataStandard] = None
-    """
-    If on-chain metadata passes validation, we display the standard
-    under which it is valid
-
-    """
-    onchain_metadata_extra: Optional[str] = None
-    """
-    Arbitrary plutus data (CIP68).
-
-    """
-    metadata: Optional[Metadata1]
-    """
-    Off-chain metadata fetched from GitHub based on network.
-    Mainnet: https://github.com/cardano-foundation/cardano-token-registry/
-    Testnet: https://github.com/input-output-hk/metadata-registry-testnet/
-
-    """
-
-
-class Action2(Enum):
-    """
-    Action executed upon the asset policy
-    """
-
-    minted = "minted"
-    burned = "burned"
-
-
-class AssetHistoryItem(BaseModel):
-    tx_hash: str
-    """
-    Hash of the transaction containing the asset action
-    """
-    action: Action2
-    """
-    Action executed upon the asset policy
-    """
-    amount: str
-    """
-    Asset amount of the specific action
-    """
-
-
-class AssetHistory(BaseModel):
-    __root__: List[AssetHistoryItem] = Field(
-        ...,
-        example=[
-            {
-                "tx_hash": "2dd15e0ef6e6a17841cb9541c27724072ce4d4b79b91e58432fbaa32d9572531",
-                "amount": "10",
-                "action": "minted",
-            },
-            {
-                "tx_hash": "9c190bc1ac88b2ab0c05a82d7de8b71b67a9316377e865748a89d4426c0d3005",
-                "amount": "5",
-                "action": "burned",
-            },
-            {
-                "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dde628516157f0",
-                "amount": "5",
-                "action": "burned",
-            },
-        ],
-    )
-
-
-class AssetTxs(BaseModel):
-    __root__: List[str] = Field(
-        ...,
-        example=[
-            "8788591983aa73981fc92d6cddbbe643959f5a784e84b8bee0db15823f575a5b",
-            "52e748c4dec58b687b90b0b40d383b9fe1f24c1a833b7395cdf07dd67859f46f",
-            "e8073fd5318ff43eca18a852527166aa8008bee9ee9e891f585612b7e4ba700b",
-        ],
-    )
-
-
-class AssetTransaction(BaseModel):
-    tx_hash: str
-    """
-    Hash of the transaction
-    """
-    tx_index: int
-    """
-    Transaction index within the block
-    """
-    block_height: int
-    """
-    Block height
-    """
-    block_time: int = Field(..., example=1635505891)
-    """
-    Block creation time in UNIX time
-    """
-
-
-class AssetTransactions(BaseModel):
-    __root__: List[AssetTransaction] = Field(
-        ...,
-        example=[
-            {
-                "tx_hash": "8788591983aa73981fc92d6cddbbe643959f5a784e84b8bee0db15823f575a5b",
-                "tx_index": 6,
-                "block_height": 69,
-                "block_time": 1635505891,
-            },
-            {
-                "tx_hash": "52e748c4dec58b687b90b0b40d383b9fe1f24c1a833b7395cdf07dd67859f46f",
-                "tx_index": 9,
-                "block_height": 4547,
-                "block_time": 1635505987,
-            },
-            {
-                "tx_hash": "e8073fd5318ff43eca18a852527166aa8008bee9ee9e891f585612b7e4ba700b",
-                "tx_index": 0,
-                "block_height": 564654,
-                "block_time": 1834505492,
-            },
-        ],
-    )
-
-
-class AssetAddress(BaseModel):
-    address: str
-    """
-    Address containing the specific asset
-    """
-    quantity: str
-    """
-    Asset quantity on the specific address
-    """
-
-
-class AssetAddresses(BaseModel):
-    __root__: List[AssetAddress] = Field(
-        ...,
-        example=[
-            {
-                "address": "addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
-                "quantity": "1",
-            },
-            {
-                "address": "addr1qyhr4exrgavdcn3qhfcc9f939fzsch2re5ry9cwvcdyh4x4re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qdpvhza",
-                "quantity": "100000",
-            },
-            {
-                "address": "addr1q8zup8m9ue3p98kxlxl9q8rnyan8hw3ul282tsl9s326dfj088lvedv4zckcj24arcpasr0gua4c5gq4zw2rpcpjk2lq8cmd9l",
-                "quantity": "18605647",
-            },
-        ],
-    )
-
-
-class AssetPolicyItem(BaseModel):
-    asset: str
-    """
-    Concatenation of the policy_id and hex-encoded asset_name
-    """
-    quantity: str
-    """
-    Current asset quantity
-    """
-
-
-class AssetPolicy(BaseModel):
-    __root__: List[AssetPolicyItem] = Field(
-        ...,
-        example=[
-            {
-                "asset": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
-                "quantity": "1",
-            },
-            {
-                "asset": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a766e",
-                "quantity": "100000",
-            },
-            {
-                "asset": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb574636f696e",
-                "quantity": "18605647",
-            },
-        ],
-    )
-
-
-class Script(BaseModel):
-    script_hash: str
-    """
-    Script hash
-    """
-
-
-class Scripts(BaseModel):
-    __root__: List[Script] = Field(
-        ...,
-        example=[
-            {"script_hash": "13a3efd825703a352a8f71f4e2758d08c28c564e8dfcce9f77776ad1"},
-            {"script_hash": "e1457a0c47dfb7a2f6b8fbb059bdceab163c05d34f195b87b9f2b30e"},
-            {"script_hash": "a6e63c0ff05c96943d1cc30bf53112ffff0f34b45986021ca058ec54"},
-        ],
-    )
-
-
-class Type3(Enum):
-    """
-    Type of the script language
-    """
-
-    timelock = "timelock"
-    plutusV1 = "plutusV1"
-    plutusV2 = "plutusV2"
-
-
-class Script1(BaseModel):
-    script_hash: str = Field(
-        ..., example="13a3efd825703a352a8f71f4e2758d08c28c564e8dfcce9f77776ad1"
-    )
-    """
-    Script hash
-    """
-    type: Type3 = Field(..., example="plutusV1")
-    """
-    Type of the script language
-    """
-    serialised_size: Optional[int] = Field(..., example=3119)
-    """
-    The size of the CBOR serialised script, if a Plutus script
-    """
-
-
-class ScriptJson(BaseModel):
-    json_: Optional[Union[str, Dict[str, Any], List, int, float, bool]] = Field(
-        ..., alias="json"
-    )
-    """
-    JSON contents of the `timelock` script, null for `plutus` scripts
-    """
-
-
-class ScriptCbor(BaseModel):
-    cbor: Optional[str]
-    """
-    CBOR contents of the `plutus` script, null for `timelocks`
-    """
-
-
-class Purpose2(Enum):
-    """
-    Validation purpose
-    """
-
-    spend = "spend"
-    mint = "mint"
-    cert = "cert"
-    reward = "reward"
-
-
-class ScriptRedeemer(BaseModel):
-    tx_hash: str = Field(
-        ..., example="1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157f0"
-    )
-    """
-    Hash of the transaction
-    """
-    tx_index: int = Field(..., example=0)
-    """
-    The index of the redeemer pointer in the transaction
-    """
-    purpose: Purpose2 = Field(..., example="spend")
-    """
-    Validation purpose
-    """
-    redeemer_data_hash: str = Field(
-        ..., example="923918e403bf43c34b4ef6b48eb2ee04babed17320d8d1b9ff9ad086e86f44ec"
-    )
-    """
-    Datum hash of the redeemer
-    """
-    datum_hash: str = Field(
-        ..., example="923918e403bf43c34b4ef6b48eb2ee04babed17320d8d1b9ff9ad086e86f44ec"
-    )
-    """
-    Datum hash
-    """
-    unit_mem: str = Field(..., example="1700")
-    """
-    The budget in Memory to run a script
-    """
-    unit_steps: str = Field(..., example="476468")
-    """
-    The budget in CPU steps to run a script
-    """
-    fee: str = Field(..., example="172033")
-    """
-    The fee consumed to run the script
-    """
-
-
-class ScriptRedeemers(BaseModel):
-    __root__: List[ScriptRedeemer]
-
-
-class ScriptDatum(BaseModel):
-    json_value: Dict[str, Any]
-    """
-    JSON content of the datum
-    """
-
-
-class ScriptDatumCbor(BaseModel):
-    cbor: str
-    """
-    CBOR serialized datum
-    """
-
-
-class UtilsAddressesXpub(BaseModel):
-    xpub: str
-    """
-    Script hash
-    """
-    role: int
-    """
-    Account role
-    """
-    index: int
-    """
-    Address index
-    """
-    address: str
-    """
-    Derived address
-    """
-
-
-class Metric(BaseModel):
-    time: int
-    """
-    Starting time of the call count interval (ends midnight UTC) in UNIX time
-    """
-    calls: int
-    """
-    Sum of all calls for a particular day
-    """
-
-
-class Metrics(BaseModel):
-    __root__: List[Metric] = Field(
-        ...,
-        example=[
-            {"time": 1612543884, "calls": 42},
-            {"time": 1614523884, "calls": 6942},
-        ],
-    )
-
-
-class MetricsEndpoint(BaseModel):
-    time: int
-    """
-    Starting time of the call count interval (ends midnight UTC) in UNIX time
-    """
-    calls: int
-    """
-    Sum of all calls for a particular day and endpoint
-    """
-    endpoint: str
-    """
-    Endpoint parent name
-    """
-
-
-class MetricsEndpoints(BaseModel):
-    __root__: List[MetricsEndpoint] = Field(
-        ...,
-        example=[
-            {"time": 1612543814, "calls": 182, "endpoint": "block"},
-            {"time": 1612543814, "calls": 42, "endpoint": "epoch"},
-            {"time": 1612543812, "calls": 775, "endpoint": "block"},
-            {"time": 1612523884, "calls": 4, "endpoint": "epoch"},
-            {"time": 1612553884, "calls": 89794, "endpoint": "block"},
-        ],
-    )
-
-
-class Supply(BaseModel):
-    max: str = Field(..., example="45000000000000000")
-    """
-    Maximum supply in Lovelaces
-    """
-    total: str = Field(..., example="32890715183299160")
-    """
-    Current total (max supply - reserves) supply in Lovelaces
-    """
-    circulating: str = Field(..., example="32412601976210393")
-    """
-    Current circulating (UTXOs + withdrawables) supply in Lovelaces
-    """
-    locked: str = Field(..., example="125006953355")
-    """
-    Current supply locked by scripts in Lovelaces
-    """
-    treasury: str = Field(..., example="98635632000000")
-    """
-    Current supply locked in treasury
-    """
-    reserves: str = Field(..., example="46635632000000")
-    """
-    Current supply locked in reserves
-    """
-
-
-class Stake(BaseModel):
-    live: str = Field(..., example="23204950463991654")
-    """
-    Current live stake in Lovelaces
-    """
-    active: str = Field(..., example="22210233523456321")
-    """
-    Current active stake in Lovelaces
-    """
-
-
-class Network(BaseModel):
-    supply: Supply
-    stake: Stake
-
-
-class Start(BaseModel):
-    """
-    Start of the blockchain era,
-    relative to the start of the network
-
-    """
-
-    time: float
-    """
-    Time in seconds relative to the start time of the network
-    """
-    slot: int
-    """
-    Absolute slot number
-    """
-    epoch: int
-    """
-    Epoch number
-    """
-
-
-class End(BaseModel):
-    """
-    End of the blockchain era,
-    relative to the start of the network
-
-    """
-
-    time: float
-    """
-    Time in seconds relative to the start time of the network
-    """
-    slot: int
-    """
-    Absolute slot number
-    """
-    epoch: int
-    """
-    Epoch number
-    """
-
-
-class Parameters(BaseModel):
-    """
-    Era parameters
-    """
-
-    epoch_length: int
-    """
-    Epoch length in number of slots
-    """
-    slot_length: float
-    """
-    Slot length in seconds
-    """
-    safe_zone: int
-    """
-    Zone in which it is guaranteed that no hard fork can take place
-    """
-
-
-class NetworkEra(BaseModel):
-    start: Start
-    """
-    Start of the blockchain era,
-    relative to the start of the network
-
-    """
-    end: End
-    """
-    End of the blockchain era,
-    relative to the start of the network
-
-    """
-    parameters: Parameters
-    """
-    Era parameters
-    """
-
-
-class NetworkEras(BaseModel):
-    __root__: List[NetworkEra] = Field(
-        ...,
-        example=[
-            {
-                "start": {"time": 0, "slot": 0, "epoch": 0},
-                "end": {"time": 89856000, "slot": 4492800, "epoch": 208},
-                "parameters": {
-                    "epoch_length": 21600,
-                    "slot_length": 20,
-                    "safe_zone": 4320,
-                },
-            },
-            {
-                "start": {"time": 89856000, "slot": 4492800, "epoch": 208},
-                "end": {"time": 101952000, "slot": 16588800, "epoch": 236},
-                "parameters": {
-                    "epoch_length": 432000,
-                    "slot_length": 1,
-                    "safe_zone": 129600,
-                },
-            },
-        ],
-    )
-
-
-class NutlinkAddress(BaseModel):
-    address: str = Field(
-        ...,
-        example="addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
-    )
-    """
-    Bech32 encoded address
-    """
-    metadata_url: str = Field(..., example="https://nut.link/metadata.json")
-    """
-    URL of the specific metadata file
-    """
-    metadata_hash: str = Field(
-        ..., example="6bf124f217d0e5a0a8adb1dbd8540e1334280d49ab861127868339f43b3948af"
-    )
-    """
-    Hash of the metadata file
-    """
-    metadata: Optional[Dict[str, Any]]
-    """
-    The cached metadata of the `metadata_url` file.
-    """
-
-
-class NutlinkAddressTicker(BaseModel):
-    name: str
-    """
-    Name of the ticker
-    """
-    count: int
-    """
-    Number of ticker records
-    """
-    latest_block: int
-    """
-    Block height of the latest record
-    """
-
-
-class NutlinkAddressTickers(BaseModel):
-    __root__: List[NutlinkAddressTicker] = Field(
-        ...,
-        example=[
-            {"name": "ADAUSD", "count": 1980038, "latest_block": 2657092},
-            {"name": "ADAEUR", "count": 1980038, "latest_block": 2657092},
-            {"name": "ADABTC", "count": 1980038, "latest_block": 2657092},
-        ],
-    )
-
-
-class NutlinkAddressTickerItem(BaseModel):
-    tx_hash: str
-    """
-    Hash of the transaction
-    """
-    block_height: int
-    """
-    Block height of the record
-    """
-    tx_index: int
-    """
-    Transaction index within the block
-    """
-    payload: Union[str, Dict[str, Any], List, int, float, bool]
-    """
-    Content of the ticker
-    """
-
-
-class NutlinkAddressTicker1(BaseModel):
-    __root__: List[NutlinkAddressTickerItem] = Field(
-        ...,
-        example=[
-            {
-                "tx_hash": "e8073fd5318ff43eca18a852527166aa8008bee9ee9e891f585612b7e4ba700b",
-                "block_height": 2657092,
-                "tx_index": 8,
-                "payload": [
-                    {"source": "coinGecko", "value": "1.29"},
-                    {"source": "cryptoCompare", "value": "1.283"},
-                ],
-            }
-        ],
-    )
-
-
-class NutlinkTickersTickerItem(BaseModel):
-    address: str
-    """
-    Address of a metadata oracle
-    """
-    tx_hash: str
-    """
-    Hash of the transaction
-    """
-    block_height: int
-    """
-    Block height of the record
-    """
-    tx_index: int
-    """
-    Transaction index within the block
-    """
-    payload: Union[str, Dict[str, Any], List, int, float, bool]
-    """
-    Content of the ticker
-    """
-
-
-class NutlinkTickersTicker(BaseModel):
-    __root__: List[NutlinkTickersTickerItem] = Field(
-        ...,
-        example=[
-            {
-                "address": "addr_test1qpmtp5t0t5y6cqkaz7rfsyrx7mld77kpvksgkwm0p7en7qum7a589n30e80tclzrrnj8qr4qvzj6al0vpgtnmrkkksnqd8upj0",
-                "tx_hash": "e8073fd5318ff43eca18a852527166aa8008bee9ee9e891f585612b7e4ba700b",
-                "block_height": 2657092,
-                "tx_index": 8,
-                "payload": [
-                    {"source": "coinGecko", "value": "1.29"},
-                    {"source": "cryptoCompare", "value": "1.283"},
-                ],
-            }
-        ],
-    )
-
-
-class File(BaseModel):
-    class Config:
-        extra = Extra.allow
-
-    name: Optional[str] = Field(None, example="myimage")
-    """
-    Name of the file
-    """
-    mediaType: str = Field(..., example="image/jpeg")
-    """
-    Mime sub-type of image
-    """
-    src: Union[str, List[str]] = Field(..., example="My NFT token description")
-    """
-    URI pointing to a resource of this mime type
-    """
-
-
-class AssetOnchainMetadataCip25(BaseModel):
-    """
-    On-chain metadata stored in the minting transaction under label 721,
-    which adheres to https://cips.cardano.org/cips/cip25/
-
-    """
-
-    class Config:
-        extra = Extra.allow
-
-    name: str = Field(..., example="My NFT token")
-    """
-    Name of the asset
-    """
-    image: Union[str, List[str]] = Field(
-        ..., example="ipfs://ipfs/QmfKyJ4tuvHowwKQCbCHj4L5T3fSj8cjs7Aau8V7BWv226"
-    )
-    """
-    URI(s) of the associated asset
-    """
-    description: Optional[Union[str, List[str]]] = Field(
-        None, example="My NFT token description"
-    )
-    """
-    Additional description
-    """
-    mediaType: Optional[str] = Field(None, example="image/jpeg")
-    """
-    Mime sub-type of image
-    """
-    files: Optional[List[File]] = None
-
-
-class AssetOnchainMetadataCip68Ft333(BaseModel):
-    """
-    On-chain metadata stored in the datum of the reference NFT output
-    which adheres to 333 FT Standard https://cips.cardano.org/cips/cip68/
-
-    """
-
-    class Config:
-        extra = Extra.allow
-
-    name: str = Field(..., example="My FT token")
-    """
-    Name of the asset
-    """
-    description: str = Field(..., example="My FT token description")
-    """
-    Additional description
-    """
-    logo: Optional[str] = Field(
-        None, example="ipfs://ipfs/QmfKyJ4tuvHowwKQCbCHj4L5T3fSj8cjs7Aau8V7BWv226"
-    )
-    """
-    URI(s) of the associated asset
-    """
-    ticker: Optional[str] = Field(None, example="TOK")
-    """
-    Ticker
-    """
-    decimals: Optional[float] = Field(None, example=8)
-    """
-    Number of decimals
-    """
-
-
-class File1(BaseModel):
-    class Config:
-        extra = Extra.allow
-
-    name: Optional[str] = Field(None, example="myimage")
-    """
-    Name of the file
-    """
-    mediaType: str = Field(..., example="image/jpeg")
-    """
-    Mime sub-type of image
-    """
-    src: Union[str, List[str]] = Field(..., example="My NFT token description")
-    """
-    URI pointing to a resource of this mime type
-    """
-
-
-class AssetOnchainMetadataCip68Nft222(BaseModel):
-    """
-    On-chain metadata stored in the datum of the reference NFT output
-    which adheres to 222 NFT Standard https://cips.cardano.org/cips/cip68/
-
-    """
-
-    class Config:
-        extra = Extra.allow
-
-    name: str = Field(..., example="My NFT token")
-    """
-    Name of the asset
-    """
-    image: str = Field(
-        ..., example="ipfs://ipfs/QmfKyJ4tuvHowwKQCbCHj4L5T3fSj8cjs7Aau8V7BWv226"
-    )
-    """
-    URI(s) of the associated asset
-    """
-    description: Optional[str] = Field(None, example="My NFT token description")
-    """
-    Additional description
-    """
-    mediaType: Optional[str] = Field(None, example="image/jpeg")
-    """
-    Mime sub-type of image
-    """
-    files: Optional[List[File1]] = None
-
-
-class File2(BaseModel):
-    class Config:
-        extra = Extra.allow
-
-    name: Optional[str] = Field(None, example="myimage")
-    """
-    Name of the file
-    """
-    mediaType: str = Field(..., example="image/jpeg")
-    """
-    Mime sub-type of image
-    """
-    src: Union[str, List[str]] = Field(..., example="My NFT token description")
-    """
-    URI pointing to a resource of this mime type
-    """
-
-
-class AssetOnchainMetadataCip68Rft444(BaseModel):
-    """
-    On-chain metadata stored in the datum of the reference NFT output
-    which adheres to 222 NFT Standard https://cips.cardano.org/cips/cip68/
-
-    """
-
-    class Config:
-        extra = Extra.allow
-
-    name: str = Field(..., example="My NFT token")
-    """
-    Name of the asset
-    """
-    image: str = Field(
-        ..., example="ipfs://ipfs/QmfKyJ4tuvHowwKQCbCHj4L5T3fSj8cjs7Aau8V7BWv226"
-    )
-    """
-    URI(s) of the associated asset
-    """
-    description: Optional[str] = Field(None, example="My NFT token description")
-    """
-    Additional description
-    """
-    mediaType: Optional[str] = Field(None, example="image/jpeg")
-    """
-    Mime sub-type of image
-    """
-    decimals: Optional[float] = Field(None, example=8)
-    """
-    Number of decimals
-    """
-    files: Optional[List[File2]] = None
-
-
-class OnchainMetadataCip25(BaseModel):
-    __root__: AssetOnchainMetadataCip25
-
-
-class OnchainMetadataCip68Ft333(BaseModel):
-    __root__: AssetOnchainMetadataCip68Ft333
-
-
-class OnchainMetadataCip68Nft222(BaseModel):
-    __root__: AssetOnchainMetadataCip68Nft222
-
-
-class OnchainMetadataCip68Rft444(BaseModel):
-    __root__: AssetOnchainMetadataCip68Rft444
+# generated by datamodel-codegen:
+#   filename:  openapi.yaml
+#   timestamp: 2023-06-02T01:54:33+00:00
+
+from __future__ import annotations
+
+from enum import Enum
+from typing import Any, Dict, List, Optional, Union
+
+from pydantic import BaseModel, Extra, Field
+
+
+class BlockContent(BaseModel):
+    time: int = Field(..., example=1641338934)
+    """
+    Block creation time in UNIX time
+    """
+    height: Optional[int] = Field(..., example=15243593)
+    """
+    Block number
+    """
+    hash: str = Field(
+        ..., example="4ea1ba291e8eef538635a53e59fddba7810d1679631cc3aed7c8e6c4091a516a"
+    )
+    """
+    Hash of the block
+    """
+    slot: Optional[int] = Field(..., example=412162133)
+    """
+    Slot number
+    """
+    epoch: Optional[int] = Field(..., example=425)
+    """
+    Epoch number
+    """
+    epoch_slot: Optional[int] = Field(..., example=12)
+    """
+    Slot within the epoch
+    """
+    slot_leader: str = Field(
+        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2qnikdy"
+    )
+    """
+    Bech32 ID of the slot leader or specific block description in case there is no slot leader
+    """
+    size: int = Field(..., example=3)
+    """
+    Block size in Bytes
+    """
+    tx_count: int = Field(..., example=1)
+    """
+    Number of transactions in the block
+    """
+    output: Optional[str] = Field(..., example="128314491794")
+    """
+    Total output within the block in Lovelaces
+    """
+    fees: Optional[str] = Field(..., example="592661")
+    """
+    Total fees within the block in Lovelaces
+    """
+    block_vrf: Optional[str] = Field(
+        ...,
+        example="vrf_vk1wf2k6lhujezqcfe00l6zetxpnmh9n6mwhpmhm0dvfh3fxgmdnrfqkms8ty",
+        max_length=65,
+        min_length=65,
+    )
+    """
+    VRF key of the block
+    """
+    op_cert: Optional[str] = Field(
+        ..., example="da905277534faf75dae41732650568af545134ee08a3c0392dbefc8096ae177c"
+    )
+    """
+    The hash of the operational certificate of the block producer
+    """
+    op_cert_counter: Optional[str] = Field(..., example="18")
+    """
+    The value of the counter used to produce the operational certificate
+    """
+    previous_block: Optional[str] = Field(
+        ..., example="43ebccb3ac72c7cebd0d9b755a4b08412c9f5dcb81b8a0ad1e3c197d29d47b05"
+    )
+    """
+    Hash of the previous block
+    """
+    next_block: Optional[str] = Field(
+        ..., example="8367f026cf4b03e116ff8ee5daf149b55ba5a6ec6dec04803b8dc317721d15fa"
+    )
+    """
+    Hash of the next block
+    """
+    confirmations: int = Field(..., example=4698)
+    """
+    Number of block confirmations
+    """
+
+
+class BlockContentTxs(BaseModel):
+    __root__: List[str] = Field(
+        ...,
+        example=[
+            "8788591983aa73981fc92d6cddbbe643959f5a784e84b8bee0db15823f575a5b",
+            "4eef6bb7755d8afbeac526b799f3e32a624691d166657e9d862aaeb66682c036",
+            "52e748c4dec58b687b90b0b40d383b9fe1f24c1a833b7395cdf07dd67859f46f",
+            "e8073fd5318ff43eca18a852527166aa8008bee9ee9e891f585612b7e4ba700b",
+        ],
+    )
+
+
+class BlockContentArray(BaseModel):
+    __root__: List[BlockContent]
+
+
+class Transaction(BaseModel):
+    tx_hash: str
+
+
+class BlockContentAddress(BaseModel):
+    address: str
+    """
+    Address that was affected in the specified block
+    """
+    transactions: List[Transaction]
+    """
+    List of transactions containing the address either in their inputs or outputs. Sorted by transaction index within a block, ascending.
+    """
+
+
+class BlockContentAddresses(BaseModel):
+    __root__: List[BlockContentAddress] = Field(
+        ...,
+        example=[
+            {
+                "address": "addr1q9ld26v2lv8wvrxxmvg90pn8n8n5k6tdst06q2s856rwmvnueldzuuqmnsye359fqrk8hwvenjnqultn7djtrlft7jnq7dy7wv",
+                "transactions": [
+                    {
+                        "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157f0"
+                    }
+                ],
+            },
+            {
+                "address": "addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
+                "transactions": [
+                    {
+                        "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157d0"
+                    }
+                ],
+            },
+        ],
+    )
+
+
+class GenesisContent(BaseModel):
+    active_slots_coefficient: float = Field(..., example=0.05)
+    """
+    The proportion of slots in which blocks should be issued
+    """
+    update_quorum: int = Field(..., example=5)
+    """
+    Determines the quorum needed for votes on the protocol parameter updates
+    """
+    max_lovelace_supply: str = Field(..., example="45000000000000000")
+    """
+    The total number of lovelace in the system
+    """
+    network_magic: int = Field(..., example=764824073)
+    """
+    Network identifier
+    """
+    epoch_length: int = Field(..., example=432000)
+    """
+    Number of slots in an epoch
+    """
+    system_start: int = Field(..., example=1506203091)
+    """
+    Time of slot 0 in UNIX time
+    """
+    slots_per_kes_period: int = Field(..., example=129600)
+    """
+    Number of slots in an KES period
+    """
+    slot_length: int = Field(..., example=1)
+    """
+    Duration of one slot in seconds
+    """
+    max_kes_evolutions: int = Field(..., example=62)
+    """
+    The maximum number of time a KES key can be evolved before a pool operator must create a new operational certificate
+    """
+    security_param: int = Field(..., example=2160)
+    """
+    Security parameter k
+    """
+
+
+class EpochContent(BaseModel):
+    epoch: int = Field(..., example=225)
+    """
+    Epoch number
+    """
+    start_time: int = Field(..., example=1603403091)
+    """
+    Unix time of the start of the epoch
+    """
+    end_time: int = Field(..., example=1603835086)
+    """
+    Unix time of the end of the epoch
+    """
+    first_block_time: int = Field(..., example=1603403092)
+    """
+    Unix time of the first block of the epoch
+    """
+    last_block_time: int = Field(..., example=1603835084)
+    """
+    Unix time of the last block of the epoch
+    """
+    block_count: int = Field(..., example=21298)
+    """
+    Number of blocks within the epoch
+    """
+    tx_count: int = Field(..., example=17856)
+    """
+    Number of transactions within the epoch
+    """
+    output: str = Field(..., example="7849943934049314")
+    """
+    Sum of all the transactions within the epoch in Lovelaces
+    """
+    fees: str = Field(..., example="4203312194")
+    """
+    Sum of all the fees within the epoch in Lovelaces
+    """
+    active_stake: Optional[str] = Field(..., example="784953934049314")
+    """
+    Sum of all the active stakes within the epoch in Lovelaces
+    """
+
+
+class EpochParamContent(BaseModel):
+    epoch: int = Field(..., example=225)
+    """
+    Epoch number
+    """
+    min_fee_a: int = Field(..., example=44)
+    """
+    The linear factor for the minimum fee calculation for given epoch
+    """
+    min_fee_b: int = Field(..., example=155381)
+    """
+    The constant factor for the minimum fee calculation
+    """
+    max_block_size: int = Field(..., example=65536)
+    """
+    Maximum block body size in Bytes
+    """
+    max_tx_size: int = Field(..., example=16384)
+    """
+    Maximum transaction size
+    """
+    max_block_header_size: int = Field(..., example=1100)
+    """
+    Maximum block header size
+    """
+    key_deposit: str = Field(..., example="2000000")
+    """
+    The amount of a key registration deposit in Lovelaces
+    """
+    pool_deposit: str = Field(..., example="500000000")
+    """
+    The amount of a pool registration deposit in Lovelaces
+    """
+    e_max: int = Field(..., example=18)
+    """
+    Epoch bound on pool retirement
+    """
+    n_opt: int = Field(..., example=150)
+    """
+    Desired number of pools
+    """
+    a0: float = Field(..., example=0.3)
+    """
+    Pool pledge influence
+    """
+    rho: float = Field(..., example=0.003)
+    """
+    Monetary expansion
+    """
+    tau: float = Field(..., example=0.2)
+    """
+    Treasury expansion
+    """
+    decentralisation_param: float = Field(..., example=0.5)
+    """
+    Percentage of blocks produced by federated nodes
+    """
+    extra_entropy: Optional[str]
+    """
+    Seed for extra entropy
+    """
+    protocol_major_ver: int = Field(..., example=2)
+    """
+    Accepted protocol major version
+    """
+    protocol_minor_ver: int = Field(..., example=0)
+    """
+    Accepted protocol minor version
+    """
+    min_utxo: str = Field(..., example="1000000")
+    """
+    Minimum UTXO value
+    """
+    min_pool_cost: str = Field(..., example="340000000")
+    """
+    Minimum stake cost forced on the pool
+    """
+    nonce: str = Field(
+        ..., example="1a3be38bcbb7911969283716ad7aa550250226b76a61fc51cc9a9a35d9276d81"
+    )
+    """
+    Epoch number only used once
+    """
+    cost_models: Optional[Dict[str, Any]] = Field(
+        ...,
+        example={
+            "PlutusV1": {
+                "addInteger-cpu-arguments-intercept": 197209,
+                "addInteger-cpu-arguments-slope": 0,
+            },
+            "PlutusV2": {
+                "addInteger-cpu-arguments-intercept": 197209,
+                "addInteger-cpu-arguments-slope": 0,
+            },
+        },
+    )
+    """
+    Cost models parameters for Plutus Core scripts
+    """
+    price_mem: Optional[float] = Field(..., example=0.0577)
+    """
+    The per word cost of script memory usage
+    """
+    price_step: Optional[float] = Field(..., example=7.21e-05)
+    """
+    The cost of script execution step usage
+    """
+    max_tx_ex_mem: Optional[str] = Field(..., example="10000000")
+    """
+    The maximum number of execution memory allowed to be used in a single transaction
+    """
+    max_tx_ex_steps: Optional[str] = Field(..., example="10000000000")
+    """
+    The maximum number of execution steps allowed to be used in a single transaction
+    """
+    max_block_ex_mem: Optional[str] = Field(..., example="50000000")
+    """
+    The maximum number of execution memory allowed to be used in a single block
+    """
+    max_block_ex_steps: Optional[str] = Field(..., example="40000000000")
+    """
+    The maximum number of execution steps allowed to be used in a single block
+    """
+    max_val_size: Optional[str] = Field(..., example="5000")
+    """
+    The maximum Val size
+    """
+    collateral_percent: Optional[int] = Field(..., example=150)
+    """
+    The percentage of the transactions fee which must be provided as collateral when including non-native scripts
+    """
+    max_collateral_inputs: Optional[int] = Field(..., example=3)
+    """
+    The maximum number of collateral inputs allowed in a transaction
+    """
+    coins_per_utxo_size: Optional[str] = Field(..., example="34482")
+    """
+    Cost per UTxO word for Alonzo. Cost per UTxO byte for Babbage and later.
+    """
+    coins_per_utxo_word: Optional[str] = Field(..., example="34482")
+    """
+    Cost per UTxO word for Alonzo. Cost per UTxO byte for Babbage and later.
+    """
+
+
+class EpochContentArray(BaseModel):
+    __root__: List[EpochContent]
+
+
+class EpochStakeContentItem(BaseModel):
+    stake_address: str = Field(
+        ..., example="stake1u9l5q5jwgelgagzyt6nuaasefgmn8pd25c8e9qpeprq0tdcp0e3uk"
+    )
+    """
+    Stake address
+    """
+    pool_id: str = Field(
+        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
+    )
+    """
+    Bech32 prefix of the pool delegated to
+    """
+    amount: str = Field(..., example="4440295078")
+    """
+    Amount of active delegated stake in Lovelaces
+    """
+
+
+class EpochStakeContent(BaseModel):
+    __root__: List[EpochStakeContentItem]
+
+
+class EpochStakePoolContentItem(BaseModel):
+    stake_address: str = Field(
+        ..., example="stake1u9l5q5jwgelgagzyt6nuaasefgmn8pd25c8e9qpeprq0tdcp0e3uk"
+    )
+    """
+    Stake address
+    """
+    amount: str = Field(..., example="4440295078")
+    """
+    Amount of active delegated stake in Lovelaces
+    """
+
+
+class EpochStakePoolContent(BaseModel):
+    __root__: List[EpochStakePoolContentItem]
+
+
+class EpochBlockContent(BaseModel):
+    __root__: List[str] = Field(
+        ...,
+        example=[
+            "d0fa315687e99ccdc96b14cc2ea74a767405d64427b648c470731a9b69e4606e",
+            "38bc6efb92a830a0ed22a64f979d120d26483fd3c811f6622a8c62175f530878",
+            "f3258fcd8b975c061b4fcdcfcbb438807134d6961ec278c200151274893b6b7d",
+        ],
+    )
+
+
+class OutputAmountItem(BaseModel):
+    """
+    The sum of all the UTXO per asset
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+
+
+class TxContent(BaseModel):
+    hash: str = Field(
+        ..., example="1e043f100dce12d107f679685acd2fc0610e10f72a92d412794c9773d11d8477"
+    )
+    """
+    Transaction hash
+    """
+    block: str = Field(
+        ..., example="356b7d7dbb696ccd12775c016941057a9dc70898d87a63fc752271bb46856940"
+    )
+    """
+    Block hash
+    """
+    block_height: int = Field(..., example=123456)
+    """
+    Block number
+    """
+    block_time: int = Field(..., example=1635505891)
+    """
+    Block creation time in UNIX time
+    """
+    slot: int = Field(..., example=42000000)
+    """
+    Slot number
+    """
+    index: int = Field(..., example=1)
+    """
+    Transaction index within the block
+    """
+    output_amount: List[OutputAmountItem] = Field(
+        ...,
+        example=[
+            {"unit": "lovelace", "quantity": "42000000"},
+            {
+                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "12",
+            },
+        ],
+    )
+    fees: str = Field(..., example="182485")
+    """
+    Fees of the transaction in Lovelaces
+    """
+    deposit: str = Field(..., example="0")
+    """
+    Deposit within the transaction in Lovelaces
+    """
+    size: int = Field(..., example=433)
+    """
+    Size of the transaction in Bytes
+    """
+    invalid_before: Optional[str]
+    """
+    Left (included) endpoint of the timelock validity intervals
+    """
+    invalid_hereafter: Optional[str] = Field(..., example="13885913")
+    """
+    Right (excluded) endpoint of the timelock validity intervals
+    """
+    utxo_count: int = Field(..., example=4)
+    """
+    Count of UTXOs within the transaction
+    """
+    withdrawal_count: int = Field(..., example=0)
+    """
+    Count of the withdrawals within the transaction
+    """
+    mir_cert_count: int = Field(..., example=0)
+    """
+    Count of the MIR certificates within the transaction
+    """
+    delegation_count: int = Field(..., example=0)
+    """
+    Count of the delegations within the transaction
+    """
+    stake_cert_count: int = Field(..., example=0)
+    """
+    Count of the stake keys (de)registration within the transaction
+    """
+    pool_update_count: int = Field(..., example=0)
+    """
+    Count of the stake pool registration and update certificates within the transaction
+    """
+    pool_retire_count: int = Field(..., example=0)
+    """
+    Count of the stake pool retirement certificates within the transaction
+    """
+    asset_mint_or_burn_count: int = Field(..., example=0)
+    """
+    Count of asset mints and burns within the transaction
+    """
+    redeemer_count: int = Field(..., example=0)
+    """
+    Count of redeemers within the transaction
+    """
+    valid_contract: bool = Field(..., example=True)
+    """
+    True if contract script passed validation
+    """
+
+
+class AmountItem(BaseModel):
+    """
+    The sum of all the UTXO per asset
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+
+
+class Input(BaseModel):
+    address: str = Field(
+        ...,
+        example="addr1q9ld26v2lv8wvrxxmvg90pn8n8n5k6tdst06q2s856rwmvnueldzuuqmnsye359fqrk8hwvenjnqultn7djtrlft7jnq7dy7wv",
+    )
+    """
+    Input address
+    """
+    amount: List[AmountItem] = Field(
+        ...,
+        example=[
+            {"unit": "lovelace", "quantity": "42000000"},
+            {
+                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "12",
+            },
+        ],
+    )
+    tx_hash: str = Field(
+        ..., example="1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157f0"
+    )
+    """
+    Hash of the UTXO transaction
+    """
+    output_index: int = Field(..., example=0)
+    """
+    UTXO index in the transaction
+    """
+    data_hash: Optional[str] = Field(
+        ..., example="9e478573ab81ea7a8e31891ce0648b81229f408d596a3483e6f4f9b92d3cf710"
+    )
+    """
+    The hash of the transaction output datum
+    """
+    inline_datum: Optional[str] = Field(..., example="19a6aa")
+    """
+    CBOR encoded inline datum
+    """
+    reference_script_hash: Optional[str] = Field(
+        ..., example="13a3efd825703a352a8f71f4e2758d08c28c564e8dfcce9f77776ad1"
+    )
+    """
+    The hash of the reference script of the input
+    """
+    collateral: bool = Field(..., example=False)
+    """
+    Whether the input is a collateral consumed on script validation failure
+    """
+    reference: Optional[bool] = Field(None, example=False)
+    """
+    Whether the input is a reference transaction input
+    """
+
+
+class AmountItem1(BaseModel):
+    """
+    The sum of all the UTXO per asset
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+
+
+class Output(BaseModel):
+    address: str = Field(
+        ...,
+        example="addr1q9ld26v2lv8wvrxxmvg90pn8n8n5k6tdst06q2s856rwmvnueldzuuqmnsye359fqrk8hwvenjnqultn7djtrlft7jnq7dy7wv",
+    )
+    """
+    Output address
+    """
+    amount: List[AmountItem1] = Field(
+        ...,
+        example=[
+            {"unit": "lovelace", "quantity": "42000000"},
+            {
+                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "12",
+            },
+        ],
+    )
+    output_index: int = Field(..., example=0)
+    """
+    UTXO index in the transaction
+    """
+    data_hash: Optional[str] = Field(
+        ..., example="9e478573ab81ea7a8e31891ce0648b81229f408d596a3483e6f4f9b92d3cf710"
+    )
+    """
+    The hash of the transaction output datum
+    """
+    inline_datum: Optional[str] = Field(..., example="19a6aa")
+    """
+    CBOR encoded inline datum
+    """
+    collateral: bool = Field(..., example=False)
+    """
+    Whether the output is a collateral output
+    """
+    reference_script_hash: Optional[str] = Field(
+        ..., example="13a3efd825703a352a8f71f4e2758d08c28c564e8dfcce9f77776ad1"
+    )
+    """
+    The hash of the reference script of the output
+    """
+
+
+class TxContentUtxo(BaseModel):
+    hash: str = Field(
+        ..., example="1e043f100dce12d107f679685acd2fc0610e10f72a92d412794c9773d11d8477"
+    )
+    """
+    Transaction hash
+    """
+    inputs: List[Input]
+    outputs: List[Output]
+
+
+class TxContentStakeAddrItem(BaseModel):
+    cert_index: int = Field(..., example=0)
+    """
+    Index of the certificate within the transaction
+    """
+    address: str = Field(
+        ..., example="stake1u9t3a0tcwune5xrnfjg4q7cpvjlgx9lcv0cuqf5mhfjwrvcwrulda"
+    )
+    """
+    Delegation stake address
+    """
+    registration: bool = Field(..., example=True)
+    """
+    Registration boolean, false if deregistration
+    """
+
+
+class TxContentStakeAddr(BaseModel):
+    __root__: List[TxContentStakeAddrItem]
+
+
+class TxContentDelegation(BaseModel):
+    index: int = Field(..., example=0)
+    """
+    Index of the certificate within the transaction
+    """
+    cert_index: int = Field(..., example=0)
+    """
+    Index of the certificate within the transaction
+    """
+    address: str = Field(
+        ..., example="stake1u9r76ypf5fskppa0cmttas05cgcswrttn6jrq4yd7jpdnvc7gt0yc"
+    )
+    """
+    Bech32 delegation stake address
+    """
+    pool_id: str = Field(
+        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
+    )
+    """
+    Bech32 ID of delegated stake pool
+    """
+    active_epoch: int = Field(..., example=210)
+    """
+    Epoch in which the delegation becomes active
+    """
+
+
+class TxContentDelegations(BaseModel):
+    __root__: List[TxContentDelegation]
+
+
+class TxContentWithdrawal(BaseModel):
+    address: str = Field(
+        ..., example="stake1u9r76ypf5fskppa0cmttas05cgcswrttn6jrq4yd7jpdnvc7gt0yc"
+    )
+    """
+    Bech32 withdrawal address
+    """
+    amount: str = Field(..., example="431833601")
+    """
+    Withdrawal amount in Lovelaces
+    """
+
+
+class TxContentWithdrawals(BaseModel):
+    __root__: List[TxContentWithdrawal]
+
+
+class Pot(Enum):
+    """
+    Source of MIR funds
+    """
+
+    reserve = "reserve"
+    treasury = "treasury"
+
+
+class TxContentMir(BaseModel):
+    pot: Pot = Field(..., example="reserve")
+    """
+    Source of MIR funds
+    """
+    cert_index: int = Field(..., example=0)
+    """
+    Index of the certificate within the transaction
+    """
+    address: str = Field(
+        ..., example="stake1u9r76ypf5fskppa0cmttas05cgcswrttn6jrq4yd7jpdnvc7gt0yc"
+    )
+    """
+    Bech32 stake address
+    """
+    amount: str = Field(..., example="431833601")
+    """
+    MIR amount in Lovelaces
+    """
+
+
+class TxContentMirs(BaseModel):
+    __root__: List[TxContentMir]
+
+
+class Metadata(BaseModel):
+    url: Optional[str] = Field(..., example="https://stakenuts.com/mainnet.json")
+    """
+    URL to the stake pool metadata
+    """
+    hash: Optional[str] = Field(
+        ..., example="47c0c68cb57f4a5b4a87bad896fc274678e7aea98e200fa14a1cb40c0cab1d8c"
+    )
+    """
+    Hash of the metadata file
+    """
+    ticker: Optional[str] = Field(..., example="NUTS")
+    """
+    Ticker of the stake pool
+    """
+    name: Optional[str] = Field(..., example="Stake Nuts")
+    """
+    Name of the stake pool
+    """
+    description: Optional[str] = Field(..., example="The best pool ever")
+    """
+    Description of the stake pool
+    """
+    homepage: Optional[str] = Field(..., example="https://stakentus.com/")
+    """
+    Home page of the stake pool
+    """
+
+
+class Relay(BaseModel):
+    ipv4: Optional[str] = Field(..., example="4.4.4.4")
+    """
+    IPv4 address of the relay
+    """
+    ipv6: Optional[str] = Field(..., example="https://stakenuts.com/mainnet.json")
+    """
+    IPv6 address of the relay
+    """
+    dns: Optional[str] = Field(..., example="relay1.stakenuts.com")
+    """
+    DNS name of the relay
+    """
+    dns_srv: Optional[str] = Field(..., example="_relays._tcp.relays.stakenuts.com")
+    """
+    DNS SRV entry of the relay
+    """
+    port: int = Field(..., example=3001)
+    """
+    Network port of the relay
+    """
+
+
+class TxContentPoolCert(BaseModel):
+    cert_index: int = Field(..., example=0)
+    """
+    Index of the certificate within the transaction
+    """
+    pool_id: str = Field(
+        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
+    )
+    """
+    Bech32 encoded pool ID
+    """
+    vrf_key: str = Field(
+        ..., example="0b5245f9934ec2151116fb8ec00f35fd00e0aa3b075c4ed12cce440f999d8233"
+    )
+    """
+    VRF key hash
+    """
+    pledge: str = Field(..., example="5000000000")
+    """
+    Stake pool certificate pledge in Lovelaces
+    """
+    margin_cost: float = Field(..., example=0.05)
+    """
+    Margin tax cost of the stake pool
+    """
+    fixed_cost: str = Field(..., example="340000000")
+    """
+    Fixed tax cost of the stake pool in Lovelaces
+    """
+    reward_account: str = Field(
+        ..., example="stake1uxkptsa4lkr55jleztw43t37vgdn88l6ghclfwuxld2eykgpgvg3f"
+    )
+    """
+    Bech32 reward account of the stake pool
+    """
+    owners: List[str] = Field(
+        ..., example=["stake1u98nnlkvkk23vtvf9273uq7cph5ww6u2yq2389psuqet90sv4xv9v"]
+    )
+    metadata: Optional[Metadata]
+    relays: List[Relay]
+    active_epoch: int = Field(..., example=210)
+    """
+    Epoch in which the update becomes active
+    """
+
+
+class TxContentPoolCerts(BaseModel):
+    __root__: List[TxContentPoolCert]
+
+
+class TxContentPoolRetire(BaseModel):
+    cert_index: int = Field(..., example=0)
+    """
+    Index of the certificate within the transaction
+    """
+    pool_id: str = Field(
+        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
+    )
+    """
+    Bech32 stake pool ID
+    """
+    retiring_epoch: int = Field(..., example=216)
+    """
+    Epoch in which the pool becomes retired
+    """
+
+
+class TxContentPoolRetires(BaseModel):
+    __root__: List[TxContentPoolRetire]
+
+
+class TxContentMetadatum(BaseModel):
+    label: str
+    """
+    Metadata label
+    """
+    json_metadata: Union[str, Dict[str, Any]]
+    """
+    Content of the metadata
+    """
+
+
+class TxContentMetadata(BaseModel):
+    __root__: List[TxContentMetadatum] = Field(
+        ...,
+        example=[
+            {
+                "label": "1967",
+                "json_metadata": {
+                    "metadata": "https://nut.link/metadata.json",
+                    "hash": "6bf124f217d0e5a0a8adb1dbd8540e1334280d49ab861127868339f43b3948af",
+                },
+            },
+            {
+                "label": "1968",
+                "json_metadata": {
+                    "ADAUSD": [
+                        {"value": "0.10409800535729975", "source": "ergoOracles"}
+                    ]
+                },
+            },
+        ],
+    )
+
+
+class TxContentMetadataCborItem(BaseModel):
+    label: str
+    """
+    Metadata label
+    """
+    cbor_metadata: Optional[str]
+    """
+    Content of the CBOR metadata
+    """
+    metadata: Optional[str]
+    """
+    Content of the CBOR metadata in hex
+    """
+
+
+class TxContentMetadataCbor(BaseModel):
+    __root__: List[TxContentMetadataCborItem] = Field(
+        ...,
+        example=[
+            {
+                "label": "1968",
+                "cbor_metadata": "\\xa100a16b436f6d62696e6174696f6e8601010101010c",
+                "metadata": "a100a16b436f6d62696e6174696f6e8601010101010c",
+            }
+        ],
+    )
+
+
+class Purpose(Enum):
+    """
+    Validation purpose
+    """
+
+    spend = "spend"
+    mint = "mint"
+    cert = "cert"
+    reward = "reward"
+
+
+class TxContentRedeemer(BaseModel):
+    tx_index: int = Field(..., example=0)
+    """
+    Index of the redeemer within the transaction
+    """
+    purpose: Purpose = Field(..., example="spend")
+    """
+    Validation purpose
+    """
+    script_hash: str = Field(
+        ..., example="ec26b89af41bef0f7585353831cb5da42b5b37185e0c8a526143b824"
+    )
+    """
+    Script hash
+    """
+    redeemer_data_hash: str = Field(
+        ..., example="923918e403bf43c34b4ef6b48eb2ee04babed17320d8d1b9ff9ad086e86f44ec"
+    )
+    """
+    Redeemer data hash
+    """
+    datum_hash: str = Field(
+        ..., example="923918e403bf43c34b4ef6b48eb2ee04babed17320d8d1b9ff9ad086e86f44ec"
+    )
+    """
+    Datum hash
+    """
+    unit_mem: str = Field(..., example="1700")
+    """
+    The budget in Memory to run a script
+    """
+    unit_steps: str = Field(..., example="476468")
+    """
+    The budget in CPU steps to run a script
+    """
+    fee: str = Field(..., example="172033")
+    """
+    The fee consumed to run the script
+    """
+
+
+class TxContentRedeemers(BaseModel):
+    __root__: List[TxContentRedeemer]
+
+
+class AccountContent(BaseModel):
+    stake_address: str = Field(
+        ..., example="stake1ux3g2c9dx2nhhehyrezyxpkstartcqmu9hk63qgfkccw5rqttygt7"
+    )
+    """
+    Bech32 stake address
+    """
+    active: bool = Field(..., example=True)
+    """
+    Registration state of an account
+    """
+    active_epoch: Optional[int] = Field(..., example=412)
+    """
+    Epoch of the most recent action - registration or deregistration
+    """
+    controlled_amount: str = Field(..., example="619154618165")
+    """
+    Balance of the account in Lovelaces
+    """
+    rewards_sum: str = Field(..., example="319154618165")
+    """
+    Sum of all rewards for the account in the Lovelaces
+    """
+    withdrawals_sum: str = Field(..., example="12125369253")
+    """
+    Sum of all the withdrawals for the account in Lovelaces
+    """
+    reserves_sum: str = Field(..., example="319154618165")
+    """
+    Sum of all  funds from reserves for the account in the Lovelaces
+    """
+    treasury_sum: str = Field(..., example="12000000")
+    """
+    Sum of all funds from treasury for the account in the Lovelaces
+    """
+    withdrawable_amount: str = Field(..., example="319154618165")
+    """
+    Sum of available rewards that haven't been withdrawn yet for the account in the Lovelaces
+    """
+    pool_id: Optional[str] = Field(
+        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
+    )
+    """
+    Bech32 pool ID that owns the account
+    """
+
+
+class Type(Enum):
+    """
+    Type of the reward
+    """
+
+    leader = "leader"
+    member = "member"
+    pool_deposit_refund = "pool_deposit_refund"
+
+
+class AccountRewardContentItem(BaseModel):
+    epoch: int
+    """
+    Epoch of the associated reward
+    """
+    amount: str
+    """
+    Rewards for given epoch in Lovelaces
+    """
+    pool_id: str
+    """
+    Bech32 pool ID being delegated to
+    """
+    type: Type
+    """
+    Type of the reward
+    """
+
+
+class AccountRewardContent(BaseModel):
+    __root__: List[AccountRewardContentItem] = Field(
+        ...,
+        example=[
+            {
+                "epoch": 215,
+                "amount": "12695385",
+                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
+                "type": "member",
+            },
+            {
+                "epoch": 216,
+                "amount": "3586329",
+                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
+                "type": "member",
+            },
+            {
+                "epoch": 217,
+                "amount": "1",
+                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
+                "type": "member",
+            },
+            {
+                "epoch": 217,
+                "amount": "1337",
+                "pool_id": "pool1cytwr0n7eas6du2h2xshl8ypa1yqr18f0erlhhjcuczysiunjcs",
+                "type": "leader",
+            },
+            {
+                "epoch": 218,
+                "amount": "1395265",
+                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
+                "type": "member",
+            },
+            {
+                "epoch": 218,
+                "amount": "500000000",
+                "pool_id": "pool1cytwr0n7eas6du2h2xshl8ypa1yqr18f0erlhhjcuczysiunjcs",
+                "type": "pool_deposit_refund",
+            },
+        ],
+    )
+
+
+class AccountHistoryContentItem(BaseModel):
+    active_epoch: int = Field(..., example=210)
+    """
+    Epoch in which the stake was active
+    """
+    amount: str
+    """
+    Stake amount in Lovelaces
+    """
+    pool_id: str
+    """
+    Bech32 ID of pool being delegated to
+    """
+
+
+class AccountHistoryContent(BaseModel):
+    __root__: List[AccountHistoryContentItem] = Field(
+        ...,
+        example=[
+            {
+                "active_epoch": 210,
+                "amount": "12695385",
+                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
+            },
+            {
+                "active_epoch": 211,
+                "amount": "22695385",
+                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
+            },
+        ],
+    )
+
+
+class AccountDelegationContentItem(BaseModel):
+    active_epoch: int = Field(..., example=210)
+    """
+    Epoch in which the delegation becomes active
+    """
+    tx_hash: str
+    """
+    Hash of the transaction containing the delegation
+    """
+    amount: str
+    """
+    Rewards for given epoch in Lovelaces
+    """
+    pool_id: str
+    """
+    Bech32 ID of pool being delegated to
+    """
+
+
+class AccountDelegationContent(BaseModel):
+    __root__: List[AccountDelegationContentItem] = Field(
+        ...,
+        example=[
+            {
+                "active_epoch": 210,
+                "tx_hash": "2dd15e0ef6e6a17841cb9541c27724072ce4d4b79b91e58432fbaa32d9572531",
+                "amount": "12695385",
+                "pool_id": "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
+            },
+            {
+                "active_epoch": 242,
+                "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dde628516157f0",
+                "amount": "12691385",
+                "pool_id": "pool1kchver88u3kygsak8wgll7htr8uxn5v35lfrsyy842nkscrzyvj",
+            },
+        ],
+    )
+
+
+class Action(Enum):
+    """
+    Action in the certificate
+    """
+
+    registered = "registered"
+    deregistered = "deregistered"
+
+
+class AccountRegistrationContentItem(BaseModel):
+    tx_hash: str
+    """
+    Hash of the transaction containing the (de)registration certificate
+    """
+    action: Action
+    """
+    Action in the certificate
+    """
+
+
+class AccountRegistrationContent(BaseModel):
+    __root__: List[AccountRegistrationContentItem] = Field(
+        ...,
+        example=[
+            {
+                "tx_hash": "2dd15e0ef6e6a17841cb9541c27724072ce4d4b79b91e58432fbaa32d9572531",
+                "action": "registered",
+            },
+            {
+                "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dde628516157f0",
+                "action": "deregistered",
+            },
+        ],
+    )
+
+
+class AccountWithdrawalContentItem(BaseModel):
+    tx_hash: str
+    """
+    Hash of the transaction containing the withdrawal
+    """
+    amount: str
+    """
+    Withdrawal amount in Lovelaces
+    """
+
+
+class AccountWithdrawalContent(BaseModel):
+    __root__: List[AccountWithdrawalContentItem] = Field(
+        ...,
+        example=[
+            {
+                "tx_hash": "48a9625c841eea0dd2bb6cf551eabe6523b7290c9ce34be74eedef2dd8f7ecc5",
+                "amount": "454541212442",
+            },
+            {
+                "tx_hash": "4230b0cbccf6f449f0847d8ad1d634a7a49df60d8c142bb8cc2dbc8ca03d9e34",
+                "amount": "97846969",
+            },
+        ],
+    )
+
+
+class AccountMirContentItem(BaseModel):
+    tx_hash: str
+    """
+    Hash of the transaction containing the MIR
+    """
+    amount: str
+    """
+    MIR amount in Lovelaces
+    """
+
+
+class AccountMirContent(BaseModel):
+    __root__: List[AccountMirContentItem] = Field(
+        ...,
+        example=[
+            {
+                "tx_hash": "69705bba1d687a816ff5a04ec0c358a1f1ef075ab7f9c6cc2763e792581cec6d",
+                "amount": "2193707473",
+            },
+            {
+                "tx_hash": "baaa77b63d4d7d2bb3ab02c9b85978c2092c336dede7f59e31ad65452d510c13",
+                "amount": "14520198574",
+            },
+        ],
+    )
+
+
+class AccountAddressesContentItem(BaseModel):
+    address: str
+    """
+    Address associated with the stake key
+    """
+
+
+class AccountAddressesContent(BaseModel):
+    __root__: List[AccountAddressesContentItem] = Field(
+        ...,
+        example=[
+            {
+                "address": "addr1qx2kd28nq8ac5prwg32hhvudlwggpgfp8utlyqxu6wqgz62f79qsdmm5dsknt9ecr5w468r9ey0fxwkdrwh08ly3tu9sy0f4qd"
+            },
+            {
+                "address": "addr1qys3czp8s9thc6u2fqed9yq3h24nyw28uk0m6mkgn9dkckjf79qsdmm5dsknt9ecr5w468r9ey0fxwkdrwh08ly3tu9suth4w4"
+            },
+            {
+                "address": "addr1q8j55h253zcvl326sk5qdt2n8z7eghzspe0ekxgncr796s2f79qsdmm5dsknt9ecr5w468r9ey0fxwkdrwh08ly3tu9sjmd35m"
+            },
+            {
+                "address": "addr1q8f7gxrprank3drhx8k5grlux7ene0nlwun8y9thu8mc3yjf79qsdmm5dsknt9ecr5w468r9ey0fxwkdrwh08ly3tu9sls6vnt"
+            },
+        ],
+    )
+
+
+class AccountAddressesAsset(BaseModel):
+    """
+    The sum of all assets of all addresses associated with a given account
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+
+
+class AccountAddressesAssets(BaseModel):
+    __root__: List[AccountAddressesAsset] = Field(
+        ...,
+        example=[
+            {
+                "unit": "d5e6bf0500378d4f0da4e8dde6becec7621cd8cbf5cbb9b87013d4cc537061636542756433343132",
+                "quantity": "1",
+            },
+            {
+                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "125",
+            },
+        ],
+    )
+
+
+class ReceivedSumItem(BaseModel):
+    """
+    The sum of all the UTXO per asset for all addresses associated with the account
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+
+
+class SentSumItem(BaseModel):
+    """
+    The sum of all the UTXO per asset for all addresses associated with the account
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+
+
+class AccountAddressesTotal(BaseModel):
+    stake_address: str = Field(
+        ..., example="stake1u9l5q5jwgelgagzyt6nuaasefgmn8pd25c8e9qpeprq0tdcp0e3uk"
+    )
+    """
+    Bech32 encoded stake address
+    """
+    received_sum: List[ReceivedSumItem] = Field(
+        ...,
+        example=[
+            {"unit": "lovelace", "quantity": "42000000"},
+            {
+                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "12",
+            },
+        ],
+    )
+    sent_sum: List[SentSumItem] = Field(
+        ...,
+        example=[
+            {"unit": "lovelace", "quantity": "42000000"},
+            {
+                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "12",
+            },
+        ],
+    )
+    tx_count: int = Field(..., example=12)
+    """
+    Count of all transactions for all addresses associated with the account
+    """
+
+
+class MempoolContentItem(BaseModel):
+    tx_hash: str
+    """
+    Hash of the transaction
+    """
+
+
+class MempoolContent(BaseModel):
+    __root__: List[MempoolContentItem] = Field(
+        ...,
+        example=[
+            {
+                "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157f0"
+            }
+        ],
+    )
+
+
+class OutputAmountItem1(BaseModel):
+    """
+    The sum of all the UTXO per asset
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+
+
+class Tx(BaseModel):
+    hash: str = Field(
+        ..., example="1e043f100dce12d107f679685acd2fc0610e10f72a92d412794c9773d11d8477"
+    )
+    """
+    Transaction hash
+    """
+    output_amount: List[OutputAmountItem1] = Field(
+        ...,
+        example=[
+            {"unit": "lovelace", "quantity": "42000000"},
+            {
+                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "12",
+            },
+        ],
+    )
+    fees: str = Field(..., example="182485")
+    """
+    Fees of the transaction in Lovelaces
+    """
+    deposit: str = Field(..., example="0")
+    """
+    Deposit within the transaction in Lovelaces
+    """
+    size: int = Field(..., example=433)
+    """
+    Size of the transaction in Bytes
+    """
+    invalid_before: Optional[str]
+    """
+    Left (included) endpoint of the timelock validity intervals
+    """
+    invalid_hereafter: Optional[str] = Field(..., example="13885913")
+    """
+    Right (excluded) endpoint of the timelock validity intervals
+    """
+    utxo_count: int = Field(..., example=4)
+    """
+    Count of UTXOs within the transaction
+    """
+    withdrawal_count: int = Field(..., example=0)
+    """
+    Count of the withdrawals within the transaction
+    """
+    mir_cert_count: int = Field(..., example=0)
+    """
+    Count of the MIR certificates within the transaction
+    """
+    delegation_count: int = Field(..., example=0)
+    """
+    Count of the delegations within the transaction
+    """
+    stake_cert_count: int = Field(..., example=0)
+    """
+    Count of the stake keys (de)registration within the transaction
+    """
+    pool_update_count: int = Field(..., example=0)
+    """
+    Count of the stake pool registration and update certificates within the transaction
+    """
+    pool_retire_count: int = Field(..., example=0)
+    """
+    Count of the stake pool retirement certificates within the transaction
+    """
+    asset_mint_or_burn_count: int = Field(..., example=0)
+    """
+    Count of asset mints and burns within the transaction
+    """
+    redeemer_count: int = Field(..., example=0)
+    """
+    Count of redeemers within the transaction
+    """
+    valid_contract: bool = Field(..., example=True)
+    """
+    True if contract script passed validation
+    """
+
+
+class Input1(BaseModel):
+    address: Optional[str] = Field(
+        None,
+        example="addr1q9ld26v2lv8wvrxxmvg90pn8n8n5k6tdst06q2s856rwmvnueldzuuqmnsye359fqrk8hwvenjnqultn7djtrlft7jnq7dy7wv",
+    )
+    """
+    Input address
+    """
+    tx_hash: str = Field(
+        ..., example="1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157f0"
+    )
+    """
+    Hash of the UTXO transaction
+    """
+    output_index: int = Field(..., example=0)
+    """
+    UTXO index in the transaction
+    """
+    collateral: bool = Field(..., example=False)
+    """
+    Whether the input is a collateral consumed on script validation failure
+    """
+    reference: Optional[bool] = Field(None, example=False)
+    """
+    Whether the input is a reference transaction input
+    """
+
+
+class AmountItem2(BaseModel):
+    """
+    The sum of all the UTXO per asset
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+
+
+class Output1(BaseModel):
+    address: str = Field(
+        ...,
+        example="addr1q9ld26v2lv8wvrxxmvg90pn8n8n5k6tdst06q2s856rwmvnueldzuuqmnsye359fqrk8hwvenjnqultn7djtrlft7jnq7dy7wv",
+    )
+    """
+    Output address
+    """
+    amount: List[AmountItem2] = Field(
+        ...,
+        example=[
+            {"unit": "lovelace", "quantity": "42000000"},
+            {
+                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "12",
+            },
+        ],
+    )
+    output_index: int = Field(..., example=0)
+    """
+    UTXO index in the transaction
+    """
+    data_hash: Optional[str] = Field(
+        ..., example="9e478573ab81ea7a8e31891ce0648b81229f408d596a3483e6f4f9b92d3cf710"
+    )
+    """
+    The hash of the transaction output datum
+    """
+    inline_datum: Optional[str] = Field(..., example="19a6aa")
+    """
+    CBOR encoded inline datum
+    """
+    collateral: bool = Field(..., example=False)
+    """
+    Whether the output is a collateral output
+    """
+    reference_script_hash: Optional[str] = Field(
+        ..., example="13a3efd825703a352a8f71f4e2758d08c28c564e8dfcce9f77776ad1"
+    )
+    """
+    The hash of the reference script of the output
+    """
+
+
+class Purpose1(Enum):
+    """
+    Validation purpose
+    """
+
+    spend = "spend"
+    mint = "mint"
+    cert = "cert"
+    reward = "reward"
+
+
+class Redeemer(BaseModel):
+    tx_index: int = Field(..., example=0)
+    """
+    Index of the redeemer within the transaction
+    """
+    purpose: Purpose1 = Field(..., example="spend")
+    """
+    Validation purpose
+    """
+    unit_mem: str = Field(..., example="1700")
+    """
+    The budget in Memory to run a script
+    """
+    unit_steps: str = Field(..., example="476468")
+    """
+    The budget in CPU steps to run a script
+    """
+
+
+class MempoolTxContent(BaseModel):
+    tx: Tx
+    inputs: List[Input1]
+    outputs: List[Output1]
+    redeemers: Optional[List[Redeemer]] = None
+
+
+class MempoolAddressesContentItem(BaseModel):
+    tx_hash: str
+    """
+    Hash of the transaction
+    """
+
+
+class MempoolAddressesContent(BaseModel):
+    __root__: List[MempoolAddressesContentItem] = Field(
+        ...,
+        example=[
+            {
+                "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157f0"
+            }
+        ],
+    )
+
+
+class TxMetadataLabel(BaseModel):
+    label: str
+    """
+    Metadata label
+    """
+    cip10: Optional[str]
+    """
+    CIP10 defined description
+    """
+    count: str
+    """
+    The count of metadata entries with a specific label
+    """
+
+
+class TxMetadataLabels(BaseModel):
+    __root__: List[TxMetadataLabel] = Field(
+        ...,
+        example=[
+            {"label": "1990", "cip10": None, "count": "1"},
+            {
+                "label": "1967",
+                "cip10": "nut.link metadata oracles registry",
+                "count": "3",
+            },
+            {
+                "label": "1968",
+                "cip10": "nut.link metadata oracles data points",
+                "count": "16321",
+            },
+        ],
+    )
+
+
+class TxMetadataLabelJsonItem(BaseModel):
+    tx_hash: str
+    """
+    Transaction hash that contains the specific metadata
+    """
+    json_metadata: Optional[Union[str, Dict[str, Any], List, int, float, bool]]
+    """
+    Content of the JSON metadata
+    """
+
+
+class TxMetadataLabelJson(BaseModel):
+    __root__: List[TxMetadataLabelJsonItem] = Field(
+        ...,
+        example=[
+            {
+                "tx_hash": "257d75c8ddb0434e9b63e29ebb6241add2b835a307aa33aedba2effe09ed4ec8",
+                "json_metadata": {
+                    "ADAUSD": [
+                        {"value": "0.10409800535729975", "source": "ergoOracles"}
+                    ]
+                },
+            },
+            {
+                "tx_hash": "e865f2cc01ca7381cf98dcdc4de07a5e8674b8ea16e6a18e3ed60c186fde2b9c",
+                "json_metadata": {
+                    "ADAUSD": [
+                        {"value": "0.15409850555139935", "source": "ergoOracles"}
+                    ]
+                },
+            },
+            {
+                "tx_hash": "4237501da3cfdd53ade91e8911e764bd0699d88fd43b12f44a1f459b89bc91be",
+                "json_metadata": None,
+            },
+        ],
+    )
+
+
+class TxMetadataLabelCborItem(BaseModel):
+    tx_hash: str
+    """
+    Transaction hash that contains the specific metadata
+    """
+    cbor_metadata: Optional[str]
+    """
+    Content of the CBOR metadata
+    """
+    metadata: Optional[str]
+    """
+    Content of the CBOR metadata in hex
+    """
+
+
+class TxMetadataLabelCbor(BaseModel):
+    __root__: List[TxMetadataLabelCborItem] = Field(
+        ...,
+        example=[
+            {
+                "tx_hash": "257d75c8ddb0434e9b63e29ebb6241add2b835a307aa33aedba2effe09ed4ec8",
+                "cbor_metadata": None,
+                "metadata": None,
+            },
+            {
+                "tx_hash": "e865f2cc01ca7381cf98dcdc4de07a5e8674b8ea16e6a18e3ed60c186fde2b9c",
+                "cbor_metadata": None,
+                "metadata": None,
+            },
+            {
+                "tx_hash": "4237501da3cfdd53ade91e8911e764bd0699d88fd43b12f44a1f459b89bc91be",
+                "cbor_metadata": "\\xa100a16b436f6d62696e6174696f6e8601010101010c",
+                "metadata": "a100a16b436f6d62696e6174696f6e8601010101010c",
+            },
+        ],
+    )
+
+
+class AmountItem3(BaseModel):
+    """
+    The sum of all the UTXO per asset
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+
+
+class Type1(Enum):
+    """
+    Address era
+    """
+
+    byron = "byron"
+    shelley = "shelley"
+
+
+class AddressContent(BaseModel):
+    address: str = Field(
+        ...,
+        example="addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
+    )
+    """
+    Bech32 encoded addresses
+    """
+    amount: List[AmountItem3] = Field(
+        ...,
+        example=[
+            {"unit": "lovelace", "quantity": "42000000"},
+            {
+                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "12",
+            },
+        ],
+    )
+    stake_address: Optional[str] = Field(
+        ..., example="stake1ux3g2c9dx2nhhehyrezyxpkstartcqmu9hk63qgfkccw5rqttygt7"
+    )
+    """
+    Stake address that controls the key
+    """
+    type: Type1 = Field(..., example="shelley")
+    """
+    Address era
+    """
+    script: bool = Field(..., example=False)
+    """
+    True if this is a script address
+    """
+
+
+class AmountItem4(BaseModel):
+    """
+    The sum of all the UTXO per asset
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+    decimals: Optional[int]
+    """
+    Number of decimal places of the asset unit. Primary data source is CIP68 reference NFT with a fallback to off-chain metadata.
+    """
+    has_nft_onchain_metadata: bool
+    """
+    True if the latest minting transaction includes metadata (best-effort)
+    """
+
+
+class Type2(Enum):
+    """
+    Address era
+    """
+
+    byron = "byron"
+    shelley = "shelley"
+
+
+class AddressContentExtended(BaseModel):
+    address: str = Field(
+        ...,
+        example="addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
+    )
+    """
+    Bech32 encoded addresses
+    """
+    amount: List[AmountItem4] = Field(
+        ...,
+        example=[
+            {
+                "unit": "lovelace",
+                "quantity": "42000000",
+                "decimals": 6,
+                "has_nft_onchain_metadata": False,
+            },
+            {
+                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "12",
+                "decimals": None,
+                "has_nft_onchain_metadata": True,
+            },
+        ],
+    )
+    stake_address: Optional[str] = Field(
+        ..., example="stake1ux3g2c9dx2nhhehyrezyxpkstartcqmu9hk63qgfkccw5rqttygt7"
+    )
+    """
+    Stake address that controls the key
+    """
+    type: Type2 = Field(..., example="shelley")
+    """
+    Address era
+    """
+    script: bool = Field(..., example=False)
+    """
+    True if this is a script address
+    """
+
+
+class ReceivedSumItem1(BaseModel):
+    """
+    The sum of all the UTXO per asset
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+
+
+class SentSumItem1(BaseModel):
+    """
+    The sum of all the UTXO per asset
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+
+
+class AddressContentTotal(BaseModel):
+    address: str = Field(
+        ...,
+        example="addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
+    )
+    """
+    Bech32 encoded address
+    """
+    received_sum: List[ReceivedSumItem1] = Field(
+        ...,
+        example=[
+            {"unit": "lovelace", "quantity": "42000000"},
+            {
+                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "12",
+            },
+        ],
+    )
+    sent_sum: List[SentSumItem1] = Field(
+        ...,
+        example=[
+            {"unit": "lovelace", "quantity": "42000000"},
+            {
+                "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "12",
+            },
+        ],
+    )
+    tx_count: int = Field(..., example=12)
+    """
+    Count of all transactions on the address
+    """
+
+
+class AmountItem5(BaseModel):
+    """
+    The sum of all the UTXO per asset
+    """
+
+    unit: str
+    """
+    The unit of the value
+    """
+    quantity: str
+    """
+    The quantity of the unit
+    """
+
+
+class AddressUtxoContentItem(BaseModel):
+    address: str = Field(
+        ...,
+        example="addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
+    )
+    """
+    Bech32 encoded addresses - useful when querying by payment_cred
+    """
+    tx_hash: str
+    """
+    Transaction hash of the UTXO
+    """
+    tx_index: int
+    """
+    UTXO index in the transaction
+    """
+    output_index: int
+    """
+    UTXO index in the transaction
+    """
+    amount: List[AmountItem5]
+    block: str
+    """
+    Block hash of the UTXO
+    """
+    data_hash: Optional[str]
+    """
+    The hash of the transaction output datum
+    """
+    inline_datum: Optional[str] = Field(..., example="19a6aa")
+    """
+    CBOR encoded inline datum
+    """
+    reference_script_hash: Optional[str] = Field(
+        ..., example="13a3efd825703a352a8f71f4e2758d08c28c564e8dfcce9f77776ad1"
+    )
+    """
+    The hash of the reference script of the output
+    """
+
+
+class AddressUtxoContent(BaseModel):
+    __root__: List[AddressUtxoContentItem] = Field(
+        ...,
+        example=[
+            {
+                "address": "addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
+                "tx_hash": "39a7a284c2a0948189dc45dec670211cd4d72f7b66c5726c08d9b3df11e44d58",
+                "output_index": 0,
+                "amount": [{"unit": "lovelace", "quantity": "42000000"}],
+                "block": "7eb8e27d18686c7db9a18f8bbcfe34e3fed6e047afaa2d969904d15e934847e6",
+                "data_hash": "9e478573ab81ea7a8e31891ce0648b81229f408d596a3483e6f4f9b92d3cf710",
+                "inline_datum": None,
+                "reference_script_hash": None,
+            },
+            {
+                "address": "addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
+                "tx_hash": "4c4e67bafa15e742c13c592b65c8f74c769cd7d9af04c848099672d1ba391b49",
+                "output_index": 0,
+                "amount": [{"unit": "lovelace", "quantity": "729235000"}],
+                "block": "953f1b80eb7c11a7ffcd67cbd4fde66e824a451aca5a4065725e5174b81685b7",
+                "data_hash": None,
+                "inline_datum": None,
+                "reference_script_hash": None,
+            },
+            {
+                "address": "addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
+                "tx_hash": "768c63e27a1c816a83dc7b07e78af673b2400de8849ea7e7b734ae1333d100d2",
+                "output_index": 1,
+                "amount": [
+                    {"unit": "lovelace", "quantity": "42000000"},
+                    {
+                        "unit": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                        "quantity": "12",
+                    },
+                ],
+                "block": "5c571f83fe6c784d3fbc223792627ccf0eea96773100f9aedecf8b1eda4544d7",
+                "data_hash": None,
+                "inline_datum": None,
+                "reference_script_hash": None,
+            },
+        ],
+    )
+
+
+class AddressTxsContent(BaseModel):
+    __root__: List[str] = Field(
+        ...,
+        example=[
+            "2dd15e0ef6e6a17841cb9541c27724072ce4d4b79b91e58432fbaa32d9572531",
+            "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dde628516157f0",
+        ],
+    )
+
+
+class AddressTransactionsContentItem(BaseModel):
+    tx_hash: str
+    """
+    Hash of the transaction
+    """
+    tx_index: int
+    """
+    Transaction index within the block
+    """
+    block_height: int
+    """
+    Block height
+    """
+    block_time: int
+    """
+    Block creation time in UNIX time
+    """
+
+
+class AddressTransactionsContent(BaseModel):
+    __root__: List[AddressTransactionsContentItem] = Field(
+        ...,
+        example=[
+            {
+                "tx_hash": "8788591983aa73981fc92d6cddbbe643959f5a784e84b8bee0db15823f575a5b",
+                "tx_index": 6,
+                "block_height": 69,
+                "block_time": 1635505891,
+            },
+            {
+                "tx_hash": "52e748c4dec58b687b90b0b40d383b9fe1f24c1a833b7395cdf07dd67859f46f",
+                "tx_index": 9,
+                "block_height": 4547,
+                "block_time": 1635505987,
+            },
+            {
+                "tx_hash": "e8073fd5318ff43eca18a852527166aa8008bee9ee9e891f585612b7e4ba700b",
+                "tx_index": 0,
+                "block_height": 564654,
+                "block_time": 1834505492,
+            },
+        ],
+    )
+
+
+class PoolList(BaseModel):
+    __root__: List[str] = Field(
+        ...,
+        example=[
+            "pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy",
+            "pool1hn7hlwrschqykupwwrtdfkvt2u4uaxvsgxyh6z63703p2knj288",
+            "pool1ztjyjfsh432eqetadf82uwuxklh28xc85zcphpwq6mmezavzad2",
+        ],
+    )
+
+
+class PoolListExtendedItem(BaseModel):
+    pool_id: str = Field(
+        ..., example="pool1z5uqdk7dzdxaae5633fqfcu2eqzy3a3rgtuvy087fdld7yws0xt"
+    )
+    """
+    Bech32 encoded pool ID
+    """
+    hex: str = Field(
+        ..., example="0f292fcaa02b8b2f9b3c8f9fd8e0bb21abedb692a6d5058df3ef2735"
+    )
+    """
+    Hexadecimal pool ID.
+    """
+    active_stake: str = Field(..., example="4200000000")
+    """
+    Active delegated amount
+    """
+    live_stake: str = Field(..., example="6900000000")
+    """
+    Currently delegated amount
+    """
+
+
+class PoolListExtended(BaseModel):
+    __root__: List[PoolListExtendedItem] = Field(
+        ...,
+        example=[
+            {
+                "pool_id": "pool19u64770wqp6s95gkajc8udheske5e6ljmpq33awxk326zjaza0q",
+                "hex": "2f355f79ee007502d116ecb07e36f985b34cebf2d84118f5c6b455a1",
+                "active_stake": "1541200000",
+                "live_stake": "1541400000",
+            },
+            {
+                "pool_id": "pool1dvla4zq98hpvacv20snndupjrqhuc79zl6gjap565nku6et5zdx",
+                "hex": "6b3fda88053dc2cee18a7c2736f032182fcc78a2fe912e869aa4edcd",
+                "active_stake": "22200000",
+                "live_stake": "48955550",
+            },
+            {
+                "pool_id": "pool1wvccajt4eugjtf3k0ja3exjqdj7t8egsujwhcw4tzj4rzsxzw5w",
+                "hex": "73318ec975cf1125a6367cbb1c9a406cbcb3e510e49d7c3aab14aa31",
+                "active_stake": "9989541215",
+                "live_stake": "168445464878",
+            },
+        ],
+    )
+
+
+class PoolListRetireItem(BaseModel):
+    pool_id: str = Field(
+        ..., example="pool1z5uqdk7dzdxaae5633fqfcu2eqzy3a3rgtuvy087fdld7yws0xt"
+    )
+    """
+    Bech32 encoded pool ID
+    """
+    epoch: int = Field(..., example=242)
+    """
+    Retirement epoch number
+    """
+
+
+class PoolListRetire(BaseModel):
+    __root__: List[PoolListRetireItem] = Field(
+        ...,
+        example=[
+            {
+                "pool_id": "pool19u64770wqp6s95gkajc8udheske5e6ljmpq33awxk326zjaza0q",
+                "epoch": 225,
+            },
+            {
+                "pool_id": "pool1dvla4zq98hpvacv20snndupjrqhuc79zl6gjap565nku6et5zdx",
+                "epoch": 215,
+            },
+            {
+                "pool_id": "pool1wvccajt4eugjtf3k0ja3exjqdj7t8egsujwhcw4tzj4rzsxzw5w",
+                "epoch": 231,
+            },
+        ],
+    )
+
+
+class Pool(BaseModel):
+    pool_id: str = Field(
+        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
+    )
+    """
+    Bech32 pool ID
+    """
+    hex: str = Field(
+        ..., example="0f292fcaa02b8b2f9b3c8f9fd8e0bb21abedb692a6d5058df3ef2735"
+    )
+    """
+    Hexadecimal pool ID.
+    """
+    vrf_key: str = Field(
+        ..., example="0b5245f9934ec2151116fb8ec00f35fd00e0aa3b075c4ed12cce440f999d8233"
+    )
+    """
+    VRF key hash
+    """
+    blocks_minted: int = Field(..., example=69)
+    """
+    Total minted blocks
+    """
+    blocks_epoch: int = Field(..., example=4)
+    """
+    Number of blocks minted in the current epoch
+    """
+    live_stake: str = Field(..., example="6900000000")
+    live_size: float = Field(..., example=0.42)
+    live_saturation: float = Field(..., example=0.93)
+    live_delegators: float = Field(..., example=127)
+    active_stake: str = Field(..., example="4200000000")
+    active_size: float = Field(..., example=0.43)
+    declared_pledge: str = Field(..., example="5000000000")
+    """
+    Stake pool certificate pledge
+    """
+    live_pledge: str = Field(..., example="5000000001")
+    """
+    Stake pool current pledge
+    """
+    margin_cost: float = Field(..., example=0.05)
+    """
+    Margin tax cost of the stake pool
+    """
+    fixed_cost: str = Field(..., example="340000000")
+    """
+    Fixed tax cost of the stake pool
+    """
+    reward_account: str = Field(
+        ..., example="stake1uxkptsa4lkr55jleztw43t37vgdn88l6ghclfwuxld2eykgpgvg3f"
+    )
+    """
+    Bech32 reward account of the stake pool
+    """
+    owners: List[str] = Field(
+        ..., example=["stake1u98nnlkvkk23vtvf9273uq7cph5ww6u2yq2389psuqet90sv4xv9v"]
+    )
+    registration: List[str] = Field(
+        ...,
+        example=[
+            "9f83e5484f543e05b52e99988272a31da373f3aab4c064c76db96643a355d9dc",
+            "7ce3b8c433bf401a190d58c8c483d8e3564dfd29ae8633c8b1b3e6c814403e95",
+            "3e6e1200ce92977c3fe5996bd4d7d7e192bcb7e231bc762f9f240c76766535b9",
+        ],
+    )
+    retirement: List[str]
+
+
+class PoolHistoryItem(BaseModel):
+    epoch: int = Field(..., example=233)
+    """
+    Epoch number
+    """
+    blocks: int = Field(..., example=22)
+    """
+    Number of blocks created by pool
+    """
+    active_stake: str = Field(..., example="20485965693569")
+    """
+    Active (Snapshot of live stake 2 epochs ago) stake in Lovelaces
+    """
+    active_size: float = Field(..., example=1.2345)
+    """
+    Pool size (percentage) of overall active stake at that epoch
+    """
+    delegators_count: int = Field(..., example=115)
+    """
+    Number of delegators for epoch
+    """
+    rewards: str = Field(..., example="206936253674159")
+    """
+    Total rewards received before distribution to delegators
+    """
+    fees: str = Field(..., example="1290968354")
+    """
+    Pool operator rewards
+    """
+
+
+class PoolHistory(BaseModel):
+    __root__: List[PoolHistoryItem]
+
+
+class PoolMetadata(BaseModel):
+    pool_id: str = Field(
+        ..., example="pool1pu5jlj4q9w9jlxeu370a3c9myx47md5j5m2str0naunn2q3lkdy"
+    )
+    """
+    Bech32 pool ID
+    """
+    hex: str = Field(
+        ..., example="0f292fcaa02b8b2f9b3c8f9fd8e0bb21abedb692a6d5058df3ef2735"
+    )
+    """
+    Hexadecimal pool ID
+    """
+    url: Optional[str] = Field(..., example="https://stakenuts.com/mainnet.json")
+    """
+    URL to the stake pool metadata
+    """
+    hash: Optional[str] = Field(
+        ..., example="47c0c68cb57f4a5b4a87bad896fc274678e7aea98e200fa14a1cb40c0cab1d8c"
+    )
+    """
+    Hash of the metadata file
+    """
+    ticker: Optional[str] = Field(..., example="NUTS")
+    """
+    Ticker of the stake pool
+    """
+    name: Optional[str] = Field(..., example="Stake Nuts")
+    """
+    Name of the stake pool
+    """
+    description: Optional[str] = Field(..., example="The best pool ever")
+    """
+    Description of the stake pool
+    """
+    homepage: Optional[str] = Field(..., example="https://stakentus.com/")
+    """
+    Home page of the stake pool
+    """
+
+
+class EmptyObject(BaseModel):
+    pass
+
+
+class PoolRelay(BaseModel):
+    ipv4: Optional[str] = Field(..., example="4.4.4.4")
+    """
+    IPv4 address of the relay
+    """
+    ipv6: Optional[str] = Field(..., example="https://stakenuts.com/mainnet.json")
+    """
+    IPv6 address of the relay
+    """
+    dns: Optional[str] = Field(..., example="relay1.stakenuts.com")
+    """
+    DNS name of the relay
+    """
+    dns_srv: Optional[str] = Field(..., example="_relays._tcp.relays.stakenuts.com")
+    """
+    DNS SRV entry of the relay
+    """
+    port: int = Field(..., example=3001)
+    """
+    Network port of the relay
+    """
+
+
+class PoolRelays(BaseModel):
+    __root__: List[PoolRelay]
+
+
+class PoolDelegator(BaseModel):
+    address: str
+    """
+    Bech32 encoded stake addresses
+    """
+    live_stake: str
+    """
+    Currently delegated amount
+    """
+
+
+class PoolDelegators(BaseModel):
+    __root__: List[PoolDelegator] = Field(
+        ...,
+        example=[
+            {
+                "address": "stake1ux4vspfvwuus9uwyp5p3f0ky7a30jq5j80jxse0fr7pa56sgn8kha",
+                "live_stake": "1137959159981411",
+            },
+            {
+                "address": "stake1uylayej7esmarzd4mk4aru37zh9yz0luj3g9fsvgpfaxulq564r5u",
+                "live_stake": "16958865648",
+            },
+            {
+                "address": "stake1u8lr2pnrgf8f7vrs9lt79hc3sxm8s2w4rwvgpncks3axx6q93d4ck",
+                "live_stake": "18605647",
+            },
+        ],
+    )
+
+
+class PoolBlocks(BaseModel):
+    __root__: List[str] = Field(
+        ...,
+        example=[
+            "d8982ca42cfe76b747cc681d35d671050a9e41e9cfe26573eb214e94fe6ff21d",
+            "026436c539e2ce84c7f77ffe669f4e4bbbb3b9c53512e5857dcba8bb0b4e9a8c",
+            "bcc8487f419b8c668a18ea2120822a05df6dfe1de1f0fac3feba88cf760f303c",
+            "86bf7b4a274e0f8ec9816171667c1b4a0cfc661dc21563f271acea9482b62df7",
+        ],
+    )
+
+
+class Action1(Enum):
+    """
+    Action in the certificate
+    """
+
+    registered = "registered"
+    deregistered = "deregistered"
+
+
+class PoolUpdate(BaseModel):
+    tx_hash: str
+    """
+    Transaction ID
+    """
+    cert_index: int
+    """
+    Certificate within the transaction
+    """
+    action: Action1
+    """
+    Action in the certificate
+    """
+
+
+class PoolUpdates(BaseModel):
+    __root__: List[PoolUpdate] = Field(
+        ...,
+        example=[
+            {
+                "tx_hash": "6804edf9712d2b619edb6ac86861fe93a730693183a262b165fcc1ba1bc99cad",
+                "cert_index": 0,
+                "action": "registered",
+            },
+            {
+                "tx_hash": "9c190bc1ac88b2ab0c05a82d7de8b71b67a9316377e865748a89d4426c0d3005",
+                "cert_index": 0,
+                "action": "deregistered",
+            },
+            {
+                "tx_hash": "e14a75b0eb2625de7055f1f580d70426311b78e0d36dd695a6bdc96c7b3d80e0",
+                "cert_index": 1,
+                "action": "registered",
+            },
+        ],
+    )
+
+
+class Asset(BaseModel):
+    asset: str
+    """
+    Asset identifier
+    """
+    quantity: str
+    """
+    Current asset quantity
+    """
+
+
+class Assets(BaseModel):
+    __root__: List[Asset] = Field(
+        ...,
+        example=[
+            {
+                "asset": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "1",
+            },
+            {
+                "asset": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e75d",
+                "quantity": "100000",
+            },
+            {
+                "asset": "6804edf9712d2b619edb6ac86861fe93a730693183a262b165fcc1ba1bc99cad",
+                "quantity": "18605647",
+            },
+        ],
+    )
+
+
+class OnchainMetadataStandard(Enum):
+    """
+    If on-chain metadata passes validation, we display the standard
+    under which it is valid
+
+    """
+
+    CIP25v1 = "CIP25v1"
+    CIP25v2 = "CIP25v2"
+    CIP68v1 = "CIP68v1"
+
+
+class Metadata1(BaseModel):
+    """
+    Off-chain metadata fetched from GitHub based on network.
+    Mainnet: https://github.com/cardano-foundation/cardano-token-registry/
+    Testnet: https://github.com/input-output-hk/metadata-registry-testnet/
+
+    """
+
+    name: str = Field(..., example="nutcoin")
+    """
+    Asset name
+    """
+    description: str = Field(..., example="The Nut Coin")
+    """
+    Asset description
+    """
+    ticker: Optional[str] = Field(..., example="nutc")
+    url: Optional[str] = Field(..., example="https://www.stakenuts.com/")
+    """
+    Asset website
+    """
+    logo: Optional[str] = Field(
+        ...,
+        example="iVBORw0KGgoAAAANSUhEUgAAADAAAAAoCAYAAAC4h3lxAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAABmJLR0QA/wD/AP+gvaeTAAAAB3RJTUUH5QITCDUPjqwFHwAAB9xJREFUWMPVWXtsU9cZ/8499/r6dZ3E9rUdO7ZDEgglFWO8KaOsJW0pCLRKrN1AqqYVkqoqrYo0ja7bpElru1WairStFKY9WzaE1E1tx+jokKqwtqFNyhKahEJJyJNgJ37E9r1+3HvO/sFR4vhx7SBtfH/F3/l93/f7ne/4PBxEKYU72dj/ZfH772v1TU+HtqbTaX8wOO01GPQpRVH7JEm+vGHDuq6z7/8jUSoHKtaBKkEUFUXdajDy1hUrmrs6zn/wWS7m7pZVjMUirKGUTnzc+e9xLcTrPPVfZzDz06Sc2lyQGEIyAPzT7Xa+dvE/3e+XLaCxoflHsVj8MAAYs74aa/WHoenwvpkZKeFy2Z5NJlOPUkqXZccFwSSrKjlyffjLH+TL6XTUGTGL/6hklD3ldIrj2M5MRmkLBMcvaRLQ1Nj88sxM/HCBfMP+eu/OYGDqe6l0WmpoqJ/88upgrU7HrQNA/cFg6MlkKiLlBtVUO40cx54BgHvLIT/HJLvdeqh/4NKxogKWN7fsCoUi7xTLxLJ4vLq6ak//wKVOrdXtttrTDMPsqJA8AAAwDErdu3VL3alTf5ma9eWCpoKhn5dKpCiqJxicPucQPVu0FHaInn35yHMcKwPAa4SQ3QCwFgDWUko3qSr5vqqSgTypuEg4Mo/zvA74/Y0rZSnZU8akSHV17k2fXfy0txjI5224kEym1s/1EUI7LBbztweHrkzkizn49LP6U6feepFSeggAQK/n04SQZ8bGrxdeQjZrbRvGzLH5hcibRqOhPplMfS1fIY5jz4xPDBdcGggho2h3z9sOLRazdG3wqp9SMgUlzGZ17SSEPsRx7J8CwfGu3PF57WhqqjfN/VxVJUxKUrIdITAXKpDJKFscosdfaFy0u+/K9aXTmXe0kAcAmA5Nng5Hbj6Tj/wCAYFAcN7uEY3GXGazMSHLqVVFapgBoMPna9yqhRAAgCTJMa3YUjZPgNFkSlWYx5eUkx+0tKx83V3rF+cVYJjruWCe133DIXqMmrNrFSDabRcWkywYmG5XFOW6aHcfb9324CoAgMmbo9MIoXkneCajiAihV/c/8eSiBSw4BxyiZxQA6m7H7FBKT2CMn2MY5jFFUX6ZO+5w2j8aHZ7YH40FByrJD5DnHGAY5uTtIA8AgBDaR4F2Yxb3WizCgmtA4ObUPSazodduqz3Suu0hf0U1cjvgdNSJ1dWWveFwdDUAtAiC2Uopdcdi8c9Zlh3GmDGl05mtAKAvo47EcdwThJCjqqpWFxALlNITomg73tff21GRAJez7iVK4WGGYfoJIQduBsbm7UrLm1ueCoUiv65kpiilw1ZbzcFoZOYoIcRTAn6eYZgXJm+Oni+Vd3YJbdyweSch9HlK6SpVVfcyDDq7Yf3m2XPBIXraKyV/a4b9UkLawbLsZgB4rwR8CyGkw13r+5fX27BckwBAEJ47oKpk8+DgUIdod7fV1vqOAMDrlZLPmqKoB+rrvXIgOP6w0WjYy3Ls5RL4bUk52bVm9fqnCk7M3CXU2ND8+MxM7BcIIftiyRYyntcdHh0bmr0wfmXl6p2SJB2KRmP3l4j7zejYUFtRAQAAgslm1Bv4nyGEDpYiIwjmjw0G/RjP866JiclNqqqWfKLq9fyZkdHBBXcnl9O71GDgD8bj0ncRQqZ8sRgzL9yYHH2pqICsOUTPLgA4CXNeZFmzWIS/YhYfjUZmvqPjuceSckrz25pS2h2cmlhbaBwhzr6kfsnL8Xhif55YYFl23Y3Jkdl7EVMoUSA4/q6qqNsBIPd11e52u45FwtG3CSH7yiEPAGC1Vt9dXGBmanDoygFLlbAjtzZCCMyC6VeaOpA1l9N7l1kwtauKaozHE28YTQaQpeR7+TqjxXheR0fHhhgt2CX1S3clEtKC16HL5djYe+niBU0CcmYA2W21/Qih5ZqDcoxlMZ24MaJJAABA87IVJ8Lh6N65Pr1B/+LIyLUfAhRZQvnM6ah7ZDHkAQB0vK6/HHxNTc2ruT5Zkldn/y5LACFk+2LIAwAwCGl6yGSt88KHXbmrBCHkqEgAz+vWLFZALJb4qNwYhFDhCSknkSwnQ4sVgDFeWg7+gQe2r1tAmkGTFQlACHWVg89nhJA9ot3dphV/eeCLp/Pw6K5IQP0S39uLFXCLwDG7zf1cKZxD9LSlUunHc/12u/2t2Vzl/rzu8zb8PZlM7bwdQgDgPK/nX2nddt+53//ht3LW2dS0fF0iLj2vquojuQFmwXRucPBKa8UCmpe1iOFwpAsAfLdJBFBKwVIlXJ2JxqKCxbwyHkvoCkAlv9/71U+7Oq+UJWDZ0hViJBL1cRynbNq0sSeeiPl6ei4NqIqq6TSmlB7X6bjuTEY5pgWfzwxGPZhMpt39/b3vzvWXFGCzulZjjM/DrauDwcAr8bjcgzGjZUuVBMH8k2uDX7wCAFDr8n2LEPI7SqmhTP6SzVbz6MDlz0/nDpT8EmOM22HOvUeWU2wp8iyLgRL6hk7Hrc2SBwC4MTlykmXZRozxn00mbVcphNA5jJmV+chr6oDd5l6jN/A/TqfSuwEAGITGMIsvGo3GTwTB3Dc2NjGSxdZYq4VIOOoNBANnKE0XPXE3brjHOTQ08k2MmVZOxzVJCbkFIQSCYEphzPaFQuGzTpfjb319PZ8UFXin/5OvrHPg/9HueAH/BSUqOuNZm4fyAAAAJXRFWHRkYXRlOmNyZWF0ZQAyMDIxLTAyLTE5VDA4OjUyOjI1KzAwOjAwCmFGlgAAACV0RVh0ZGF0ZTptb2RpZnkAMjAyMS0wMi0xOVQwODo1MjoyMyswMDowMBjsyxAAAAAASUVORK5CYII=",
+    )
+    """
+    Base64 encoded logo of the asset
+    """
+    decimals: Optional[int] = Field(..., example=6, le=255.0)
+    """
+    Number of decimal places of the asset unit
+    """
+
+
+class Asset1(BaseModel):
+    asset: str = Field(
+        ...,
+        example="b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+    )
+    """
+    Hex-encoded asset full name
+    """
+    policy_id: str = Field(
+        ..., example="b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a7"
+    )
+    """
+    Policy ID of the asset
+    """
+    asset_name: Optional[str] = Field(..., example="6e7574636f696e")
+    """
+    Hex-encoded asset name of the asset
+    """
+    fingerprint: str = Field(
+        ..., example="asset1pkpwyknlvul7az0xx8czhl60pyel45rpje4z8w"
+    )
+    """
+    CIP14 based user-facing fingerprint
+    """
+    quantity: str = Field(..., example="12000")
+    """
+    Current asset quantity
+    """
+    initial_mint_tx_hash: str = Field(
+        ..., example="6804edf9712d2b619edb6ac86861fe93a730693183a262b165fcc1ba1bc99cad"
+    )
+    """
+    ID of the initial minting transaction
+    """
+    mint_or_burn_count: int = Field(..., example=1)
+    """
+    Count of mint and burn transactions
+    """
+    onchain_metadata: Optional[Dict[str, Any]]
+    """
+    On-chain metadata which SHOULD adhere to the valid standards,
+    based on which we perform the look up and display the asset
+    (best effort)
+
+    """
+    onchain_metadata_standard: Optional[OnchainMetadataStandard] = None
+    """
+    If on-chain metadata passes validation, we display the standard
+    under which it is valid
+
+    """
+    onchain_metadata_extra: Optional[str] = None
+    """
+    Arbitrary plutus data (CIP68).
+
+    """
+    metadata: Optional[Metadata1]
+    """
+    Off-chain metadata fetched from GitHub based on network.
+    Mainnet: https://github.com/cardano-foundation/cardano-token-registry/
+    Testnet: https://github.com/input-output-hk/metadata-registry-testnet/
+
+    """
+
+
+class Action2(Enum):
+    """
+    Action executed upon the asset policy
+    """
+
+    minted = "minted"
+    burned = "burned"
+
+
+class AssetHistoryItem(BaseModel):
+    tx_hash: str
+    """
+    Hash of the transaction containing the asset action
+    """
+    action: Action2
+    """
+    Action executed upon the asset policy
+    """
+    amount: str
+    """
+    Asset amount of the specific action
+    """
+
+
+class AssetHistory(BaseModel):
+    __root__: List[AssetHistoryItem] = Field(
+        ...,
+        example=[
+            {
+                "tx_hash": "2dd15e0ef6e6a17841cb9541c27724072ce4d4b79b91e58432fbaa32d9572531",
+                "amount": "10",
+                "action": "minted",
+            },
+            {
+                "tx_hash": "9c190bc1ac88b2ab0c05a82d7de8b71b67a9316377e865748a89d4426c0d3005",
+                "amount": "5",
+                "action": "burned",
+            },
+            {
+                "tx_hash": "1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dde628516157f0",
+                "amount": "5",
+                "action": "burned",
+            },
+        ],
+    )
+
+
+class AssetTxs(BaseModel):
+    __root__: List[str] = Field(
+        ...,
+        example=[
+            "8788591983aa73981fc92d6cddbbe643959f5a784e84b8bee0db15823f575a5b",
+            "52e748c4dec58b687b90b0b40d383b9fe1f24c1a833b7395cdf07dd67859f46f",
+            "e8073fd5318ff43eca18a852527166aa8008bee9ee9e891f585612b7e4ba700b",
+        ],
+    )
+
+
+class AssetTransaction(BaseModel):
+    tx_hash: str
+    """
+    Hash of the transaction
+    """
+    tx_index: int
+    """
+    Transaction index within the block
+    """
+    block_height: int
+    """
+    Block height
+    """
+    block_time: int = Field(..., example=1635505891)
+    """
+    Block creation time in UNIX time
+    """
+
+
+class AssetTransactions(BaseModel):
+    __root__: List[AssetTransaction] = Field(
+        ...,
+        example=[
+            {
+                "tx_hash": "8788591983aa73981fc92d6cddbbe643959f5a784e84b8bee0db15823f575a5b",
+                "tx_index": 6,
+                "block_height": 69,
+                "block_time": 1635505891,
+            },
+            {
+                "tx_hash": "52e748c4dec58b687b90b0b40d383b9fe1f24c1a833b7395cdf07dd67859f46f",
+                "tx_index": 9,
+                "block_height": 4547,
+                "block_time": 1635505987,
+            },
+            {
+                "tx_hash": "e8073fd5318ff43eca18a852527166aa8008bee9ee9e891f585612b7e4ba700b",
+                "tx_index": 0,
+                "block_height": 564654,
+                "block_time": 1834505492,
+            },
+        ],
+    )
+
+
+class AssetAddress(BaseModel):
+    address: str
+    """
+    Address containing the specific asset
+    """
+    quantity: str
+    """
+    Asset quantity on the specific address
+    """
+
+
+class AssetAddresses(BaseModel):
+    __root__: List[AssetAddress] = Field(
+        ...,
+        example=[
+            {
+                "address": "addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
+                "quantity": "1",
+            },
+            {
+                "address": "addr1qyhr4exrgavdcn3qhfcc9f939fzsch2re5ry9cwvcdyh4x4re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qdpvhza",
+                "quantity": "100000",
+            },
+            {
+                "address": "addr1q8zup8m9ue3p98kxlxl9q8rnyan8hw3ul282tsl9s326dfj088lvedv4zckcj24arcpasr0gua4c5gq4zw2rpcpjk2lq8cmd9l",
+                "quantity": "18605647",
+            },
+        ],
+    )
+
+
+class AssetPolicyItem(BaseModel):
+    asset: str
+    """
+    Concatenation of the policy_id and hex-encoded asset_name
+    """
+    quantity: str
+    """
+    Current asset quantity
+    """
+
+
+class AssetPolicy(BaseModel):
+    __root__: List[AssetPolicyItem] = Field(
+        ...,
+        example=[
+            {
+                "asset": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a76e7574636f696e",
+                "quantity": "1",
+            },
+            {
+                "asset": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb38a766e",
+                "quantity": "100000",
+            },
+            {
+                "asset": "b0d07d45fe9514f80213f4020e5a61241458be626841cde717cb574636f696e",
+                "quantity": "18605647",
+            },
+        ],
+    )
+
+
+class Script(BaseModel):
+    script_hash: str
+    """
+    Script hash
+    """
+
+
+class Scripts(BaseModel):
+    __root__: List[Script] = Field(
+        ...,
+        example=[
+            {"script_hash": "13a3efd825703a352a8f71f4e2758d08c28c564e8dfcce9f77776ad1"},
+            {"script_hash": "e1457a0c47dfb7a2f6b8fbb059bdceab163c05d34f195b87b9f2b30e"},
+            {"script_hash": "a6e63c0ff05c96943d1cc30bf53112ffff0f34b45986021ca058ec54"},
+        ],
+    )
+
+
+class Type3(Enum):
+    """
+    Type of the script language
+    """
+
+    timelock = "timelock"
+    plutusV1 = "plutusV1"
+    plutusV2 = "plutusV2"
+
+
+class Script1(BaseModel):
+    script_hash: str = Field(
+        ..., example="13a3efd825703a352a8f71f4e2758d08c28c564e8dfcce9f77776ad1"
+    )
+    """
+    Script hash
+    """
+    type: Type3 = Field(..., example="plutusV1")
+    """
+    Type of the script language
+    """
+    serialised_size: Optional[int] = Field(..., example=3119)
+    """
+    The size of the CBOR serialised script, if a Plutus script
+    """
+
+
+class ScriptJson(BaseModel):
+    json_: Optional[Union[str, Dict[str, Any], List, int, float, bool]] = Field(
+        ..., alias="json"
+    )
+    """
+    JSON contents of the `timelock` script, null for `plutus` scripts
+    """
+
+
+class ScriptCbor(BaseModel):
+    cbor: Optional[str]
+    """
+    CBOR contents of the `plutus` script, null for `timelocks`
+    """
+
+
+class Purpose2(Enum):
+    """
+    Validation purpose
+    """
+
+    spend = "spend"
+    mint = "mint"
+    cert = "cert"
+    reward = "reward"
+
+
+class ScriptRedeemer(BaseModel):
+    tx_hash: str = Field(
+        ..., example="1a0570af966fb355a7160e4f82d5a80b8681b7955f5d44bec0dce628516157f0"
+    )
+    """
+    Hash of the transaction
+    """
+    tx_index: int = Field(..., example=0)
+    """
+    The index of the redeemer pointer in the transaction
+    """
+    purpose: Purpose2 = Field(..., example="spend")
+    """
+    Validation purpose
+    """
+    redeemer_data_hash: str = Field(
+        ..., example="923918e403bf43c34b4ef6b48eb2ee04babed17320d8d1b9ff9ad086e86f44ec"
+    )
+    """
+    Datum hash of the redeemer
+    """
+    datum_hash: str = Field(
+        ..., example="923918e403bf43c34b4ef6b48eb2ee04babed17320d8d1b9ff9ad086e86f44ec"
+    )
+    """
+    Datum hash
+    """
+    unit_mem: str = Field(..., example="1700")
+    """
+    The budget in Memory to run a script
+    """
+    unit_steps: str = Field(..., example="476468")
+    """
+    The budget in CPU steps to run a script
+    """
+    fee: str = Field(..., example="172033")
+    """
+    The fee consumed to run the script
+    """
+
+
+class ScriptRedeemers(BaseModel):
+    __root__: List[ScriptRedeemer]
+
+
+class ScriptDatum(BaseModel):
+    json_value: Dict[str, Any]
+    """
+    JSON content of the datum
+    """
+
+
+class ScriptDatumCbor(BaseModel):
+    cbor: str
+    """
+    CBOR serialized datum
+    """
+
+
+class UtilsAddressesXpub(BaseModel):
+    xpub: str
+    """
+    Script hash
+    """
+    role: int
+    """
+    Account role
+    """
+    index: int
+    """
+    Address index
+    """
+    address: str
+    """
+    Derived address
+    """
+
+
+class Metric(BaseModel):
+    time: int
+    """
+    Starting time of the call count interval (ends midnight UTC) in UNIX time
+    """
+    calls: int
+    """
+    Sum of all calls for a particular day
+    """
+
+
+class Metrics(BaseModel):
+    __root__: List[Metric] = Field(
+        ...,
+        example=[
+            {"time": 1612543884, "calls": 42},
+            {"time": 1614523884, "calls": 6942},
+        ],
+    )
+
+
+class MetricsEndpoint(BaseModel):
+    time: int
+    """
+    Starting time of the call count interval (ends midnight UTC) in UNIX time
+    """
+    calls: int
+    """
+    Sum of all calls for a particular day and endpoint
+    """
+    endpoint: str
+    """
+    Endpoint parent name
+    """
+
+
+class MetricsEndpoints(BaseModel):
+    __root__: List[MetricsEndpoint] = Field(
+        ...,
+        example=[
+            {"time": 1612543814, "calls": 182, "endpoint": "block"},
+            {"time": 1612543814, "calls": 42, "endpoint": "epoch"},
+            {"time": 1612543812, "calls": 775, "endpoint": "block"},
+            {"time": 1612523884, "calls": 4, "endpoint": "epoch"},
+            {"time": 1612553884, "calls": 89794, "endpoint": "block"},
+        ],
+    )
+
+
+class Supply(BaseModel):
+    max: str = Field(..., example="45000000000000000")
+    """
+    Maximum supply in Lovelaces
+    """
+    total: str = Field(..., example="32890715183299160")
+    """
+    Current total (max supply - reserves) supply in Lovelaces
+    """
+    circulating: str = Field(..., example="32412601976210393")
+    """
+    Current circulating (UTXOs + withdrawables) supply in Lovelaces
+    """
+    locked: str = Field(..., example="125006953355")
+    """
+    Current supply locked by scripts in Lovelaces
+    """
+    treasury: str = Field(..., example="98635632000000")
+    """
+    Current supply locked in treasury
+    """
+    reserves: str = Field(..., example="46635632000000")
+    """
+    Current supply locked in reserves
+    """
+
+
+class Stake(BaseModel):
+    live: str = Field(..., example="23204950463991654")
+    """
+    Current live stake in Lovelaces
+    """
+    active: str = Field(..., example="22210233523456321")
+    """
+    Current active stake in Lovelaces
+    """
+
+
+class Network(BaseModel):
+    supply: Supply
+    stake: Stake
+
+
+class Start(BaseModel):
+    """
+    Start of the blockchain era,
+    relative to the start of the network
+
+    """
+
+    time: float
+    """
+    Time in seconds relative to the start time of the network
+    """
+    slot: int
+    """
+    Absolute slot number
+    """
+    epoch: int
+    """
+    Epoch number
+    """
+
+
+class End(BaseModel):
+    """
+    End of the blockchain era,
+    relative to the start of the network
+
+    """
+
+    time: float
+    """
+    Time in seconds relative to the start time of the network
+    """
+    slot: int
+    """
+    Absolute slot number
+    """
+    epoch: int
+    """
+    Epoch number
+    """
+
+
+class Parameters(BaseModel):
+    """
+    Era parameters
+    """
+
+    epoch_length: int
+    """
+    Epoch length in number of slots
+    """
+    slot_length: float
+    """
+    Slot length in seconds
+    """
+    safe_zone: int
+    """
+    Zone in which it is guaranteed that no hard fork can take place
+    """
+
+
+class NetworkEra(BaseModel):
+    start: Start
+    """
+    Start of the blockchain era,
+    relative to the start of the network
+
+    """
+    end: End
+    """
+    End of the blockchain era,
+    relative to the start of the network
+
+    """
+    parameters: Parameters
+    """
+    Era parameters
+    """
+
+
+class NetworkEras(BaseModel):
+    __root__: List[NetworkEra] = Field(
+        ...,
+        example=[
+            {
+                "start": {"time": 0, "slot": 0, "epoch": 0},
+                "end": {"time": 89856000, "slot": 4492800, "epoch": 208},
+                "parameters": {
+                    "epoch_length": 21600,
+                    "slot_length": 20,
+                    "safe_zone": 4320,
+                },
+            },
+            {
+                "start": {"time": 89856000, "slot": 4492800, "epoch": 208},
+                "end": {"time": 101952000, "slot": 16588800, "epoch": 236},
+                "parameters": {
+                    "epoch_length": 432000,
+                    "slot_length": 1,
+                    "safe_zone": 129600,
+                },
+            },
+        ],
+    )
+
+
+class NutlinkAddress(BaseModel):
+    address: str = Field(
+        ...,
+        example="addr1qxqs59lphg8g6qndelq8xwqn60ag3aeyfcp33c2kdp46a09re5df3pzwwmyq946axfcejy5n4x0y99wqpgtp2gd0k09qsgy6pz",
+    )
+    """
+    Bech32 encoded address
+    """
+    metadata_url: str = Field(..., example="https://nut.link/metadata.json")
+    """
+    URL of the specific metadata file
+    """
+    metadata_hash: str = Field(
+        ..., example="6bf124f217d0e5a0a8adb1dbd8540e1334280d49ab861127868339f43b3948af"
+    )
+    """
+    Hash of the metadata file
+    """
+    metadata: Optional[Dict[str, Any]]
+    """
+    The cached metadata of the `metadata_url` file.
+    """
+
+
+class NutlinkAddressTicker(BaseModel):
+    name: str
+    """
+    Name of the ticker
+    """
+    count: int
+    """
+    Number of ticker records
+    """
+    latest_block: int
+    """
+    Block height of the latest record
+    """
+
+
+class NutlinkAddressTickers(BaseModel):
+    __root__: List[NutlinkAddressTicker] = Field(
+        ...,
+        example=[
+            {"name": "ADAUSD", "count": 1980038, "latest_block": 2657092},
+            {"name": "ADAEUR", "count": 1980038, "latest_block": 2657092},
+            {"name": "ADABTC", "count": 1980038, "latest_block": 2657092},
+        ],
+    )
+
+
+class NutlinkAddressTickerItem(BaseModel):
+    tx_hash: str
+    """
+    Hash of the transaction
+    """
+    block_height: int
+    """
+    Block height of the record
+    """
+    tx_index: int
+    """
+    Transaction index within the block
+    """
+    payload: Union[str, Dict[str, Any], List, int, float, bool]
+    """
+    Content of the ticker
+    """
+
+
+class NutlinkAddressTicker1(BaseModel):
+    __root__: List[NutlinkAddressTickerItem] = Field(
+        ...,
+        example=[
+            {
+                "tx_hash": "e8073fd5318ff43eca18a852527166aa8008bee9ee9e891f585612b7e4ba700b",
+                "block_height": 2657092,
+                "tx_index": 8,
+                "payload": [
+                    {"source": "coinGecko", "value": "1.29"},
+                    {"source": "cryptoCompare", "value": "1.283"},
+                ],
+            }
+        ],
+    )
+
+
+class NutlinkTickersTickerItem(BaseModel):
+    address: str
+    """
+    Address of a metadata oracle
+    """
+    tx_hash: str
+    """
+    Hash of the transaction
+    """
+    block_height: int
+    """
+    Block height of the record
+    """
+    tx_index: int
+    """
+    Transaction index within the block
+    """
+    payload: Union[str, Dict[str, Any], List, int, float, bool]
+    """
+    Content of the ticker
+    """
+
+
+class NutlinkTickersTicker(BaseModel):
+    __root__: List[NutlinkTickersTickerItem] = Field(
+        ...,
+        example=[
+            {
+                "address": "addr_test1qpmtp5t0t5y6cqkaz7rfsyrx7mld77kpvksgkwm0p7en7qum7a589n30e80tclzrrnj8qr4qvzj6al0vpgtnmrkkksnqd8upj0",
+                "tx_hash": "e8073fd5318ff43eca18a852527166aa8008bee9ee9e891f585612b7e4ba700b",
+                "block_height": 2657092,
+                "tx_index": 8,
+                "payload": [
+                    {"source": "coinGecko", "value": "1.29"},
+                    {"source": "cryptoCompare", "value": "1.283"},
+                ],
+            }
+        ],
+    )
+
+
+class File(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    name: Optional[str] = Field(None, example="myimage")
+    """
+    Name of the file
+    """
+    mediaType: str = Field(..., example="image/jpeg")
+    """
+    Mime sub-type of image
+    """
+    src: Union[str, List[str]] = Field(..., example="My NFT token description")
+    """
+    URI pointing to a resource of this mime type
+    """
+
+
+class AssetOnchainMetadataCip25(BaseModel):
+    """
+    On-chain metadata stored in the minting transaction under label 721,
+    which adheres to https://cips.cardano.org/cips/cip25/
+
+    """
+
+    class Config:
+        extra = Extra.allow
+
+    name: str = Field(..., example="My NFT token")
+    """
+    Name of the asset
+    """
+    image: Union[str, List[str]] = Field(
+        ..., example="ipfs://ipfs/QmfKyJ4tuvHowwKQCbCHj4L5T3fSj8cjs7Aau8V7BWv226"
+    )
+    """
+    URI(s) of the associated asset
+    """
+    description: Optional[Union[str, List[str]]] = Field(
+        None, example="My NFT token description"
+    )
+    """
+    Additional description
+    """
+    mediaType: Optional[str] = Field(None, example="image/jpeg")
+    """
+    Mime sub-type of image
+    """
+    files: Optional[List[File]] = None
+
+
+class AssetOnchainMetadataCip68Ft333(BaseModel):
+    """
+    On-chain metadata stored in the datum of the reference NFT output
+    which adheres to 333 FT Standard https://cips.cardano.org/cips/cip68/
+
+    """
+
+    class Config:
+        extra = Extra.allow
+
+    name: str = Field(..., example="My FT token")
+    """
+    Name of the asset
+    """
+    description: str = Field(..., example="My FT token description")
+    """
+    Additional description
+    """
+    logo: Optional[str] = Field(
+        None, example="ipfs://ipfs/QmfKyJ4tuvHowwKQCbCHj4L5T3fSj8cjs7Aau8V7BWv226"
+    )
+    """
+    URI(s) of the associated asset
+    """
+    ticker: Optional[str] = Field(None, example="TOK")
+    """
+    Ticker
+    """
+    decimals: Optional[float] = Field(None, example=8)
+    """
+    Number of decimals
+    """
+
+
+class File1(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    name: Optional[str] = Field(None, example="myimage")
+    """
+    Name of the file
+    """
+    mediaType: str = Field(..., example="image/jpeg")
+    """
+    Mime sub-type of image
+    """
+    src: Union[str, List[str]] = Field(..., example="My NFT token description")
+    """
+    URI pointing to a resource of this mime type
+    """
+
+
+class AssetOnchainMetadataCip68Nft222(BaseModel):
+    """
+    On-chain metadata stored in the datum of the reference NFT output
+    which adheres to 222 NFT Standard https://cips.cardano.org/cips/cip68/
+
+    """
+
+    class Config:
+        extra = Extra.allow
+
+    name: str = Field(..., example="My NFT token")
+    """
+    Name of the asset
+    """
+    image: str = Field(
+        ..., example="ipfs://ipfs/QmfKyJ4tuvHowwKQCbCHj4L5T3fSj8cjs7Aau8V7BWv226"
+    )
+    """
+    URI(s) of the associated asset
+    """
+    description: Optional[str] = Field(None, example="My NFT token description")
+    """
+    Additional description
+    """
+    mediaType: Optional[str] = Field(None, example="image/jpeg")
+    """
+    Mime sub-type of image
+    """
+    files: Optional[List[File1]] = None
+
+
+class File2(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    name: Optional[str] = Field(None, example="myimage")
+    """
+    Name of the file
+    """
+    mediaType: str = Field(..., example="image/jpeg")
+    """
+    Mime sub-type of image
+    """
+    src: Union[str, List[str]] = Field(..., example="My NFT token description")
+    """
+    URI pointing to a resource of this mime type
+    """
+
+
+class AssetOnchainMetadataCip68Rft444(BaseModel):
+    """
+    On-chain metadata stored in the datum of the reference NFT output
+    which adheres to 222 NFT Standard https://cips.cardano.org/cips/cip68/
+
+    """
+
+    class Config:
+        extra = Extra.allow
+
+    name: str = Field(..., example="My NFT token")
+    """
+    Name of the asset
+    """
+    image: str = Field(
+        ..., example="ipfs://ipfs/QmfKyJ4tuvHowwKQCbCHj4L5T3fSj8cjs7Aau8V7BWv226"
+    )
+    """
+    URI(s) of the associated asset
+    """
+    description: Optional[str] = Field(None, example="My NFT token description")
+    """
+    Additional description
+    """
+    mediaType: Optional[str] = Field(None, example="image/jpeg")
+    """
+    Mime sub-type of image
+    """
+    decimals: Optional[float] = Field(None, example=8)
+    """
+    Number of decimals
+    """
+    files: Optional[List[File2]] = None
+
+
+class OnchainMetadataCip25(BaseModel):
+    __root__: AssetOnchainMetadataCip25
+
+
+class OnchainMetadataCip68Ft333(BaseModel):
+    __root__: AssetOnchainMetadataCip68Ft333
+
+
+class OnchainMetadataCip68Nft222(BaseModel):
+    __root__: AssetOnchainMetadataCip68Nft222
+
+
+class OnchainMetadataCip68Rft444(BaseModel):
+    __root__: AssetOnchainMetadataCip68Rft444
```

### Comparing `minswap_py-0.2.0/src/minswap/models/common.py` & `minswap_py-0.2.1/src/minswap/models/common.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,329 +1,329 @@
-"""Standard models and model conversion functions.
-
-This module contains common models used throughout minswap-py as well as utility
-functions for converting data types.
-"""
-
-from collections.abc import Iterable
-from datetime import datetime
-from enum import Enum
-from typing import Any, Dict, List, Optional, Union
-
-import pycardano
-from blockfrost import Namespace
-from pydantic import BaseModel, root_validator
-
-from minswap.models import blockfrost_models
-
-
-def to_dict(
-    values: Union[Namespace, List[Any], Dict[str, Any]]
-) -> Union[List[Any], Dict[str, Any]]:
-    """Traverse a dictionary and convert blockfrost.Namespace objects to dictionaries.
-
-    When using `blockfrost.Namespace.to_dict` function to convert a `Namespace` object
-    to a `dict`, child values that are `Namespace` objects are not converted to a
-    `dict`. This function traverse a `Namespace`, `List`, or `Dict` and converts any
-    child values from `Namespace` to `dict`. This is necessary for casting to
-    `pydantic` models for proper error checking and validation.
-
-    Traversel of the input is recursive, ensuring all children are converted.
-
-    Args:
-        values: A `Namespace`, `List`, or `Dict` to be recursively traversed.
-
-    Returns:
-        Union[List[Any], Dict[Any, Any], Dict[str, Any]]
-    """
-    iterator: Optional[Iterable] = None
-
-    if isinstance(values, (Namespace)):
-        values = values.to_dict()
-
-    if isinstance(values, list):
-        iterator = enumerate(values)
-    elif isinstance(values, dict):
-        iterator = values.items()
-
-    if iterator is not None:
-        for k, v in iterator:
-            if isinstance(v, Namespace):
-                values[k] = to_dict(v.to_dict())
-            elif isinstance(v, (list, dict)):
-                values[k] = to_dict(v)
-
-        assert isinstance(values, (list, dict)), f"Error: {values}"
-
-    return values
-
-
-class PoolHistory(BaseModel):
-    """A historical point in the pool."""
-
-    tx_hash: str
-    tx_index: int
-    block_height: int
-    time: datetime
-
-
-class PoolTransactionReference(BaseModel):
-    """A reference to a pool transaction state."""
-
-    tx_index: int
-    tx_hash: str
-    block_height: int
-    block_time: datetime
-
-    @root_validator(pre=True)
-    def _validator(cls, values):
-        values["block_time"] = datetime.utcfromtimestamp(values["block_time"])
-
-        return values
-
-    class Config:  # noqa: D106
-        allow_mutation = False
-        extra = "forbid"
-
-
-class Transaction(blockfrost_models.TxContent):
-    """Transaction Content."""
-
-    block_time: datetime = blockfrost_models.TxContent.__fields__[
-        "block_time"
-    ]  # type: ignore
-
-    @root_validator(pre=True)
-    def _validator(cls, values):
-        values["block_time"] = datetime.utcfromtimestamp(values["block_time"])
-
-        return values
-
-
-class AssetHistoryReference(BaseModel):
-    """A reference to a pool transaction state."""
-
-    tx_hash: str
-    action: str
-    amount: int
-
-    class Config:  # noqa: D106
-        allow_mutation = False
-        extra = "forbid"
-
-
-class BaseList(BaseModel):
-    """Utility class for list models."""
-
-    def __iter__(self):  # noqa
-        return iter(self.__root__)
-
-    def __getitem__(self, item):  # noqa
-        return self.__root__[item]
-
-    def __len__(self):  # noqa
-        return len(self.__root__)
-
-
-class BaseDict(BaseList):
-    """Utility class for dict models."""
-
-    def items(self):
-        """Return iterable of key-value pairs."""
-        return self.__root__.items()
-
-    def keys(self):
-        """Return iterable of keys."""
-        return self.__root__.keys()
-
-    def values(self):
-        """Return iterable of values."""
-        return self.__root__.values()
-
-    def __getitem__(self, item):  # noqa
-        return self.__root__.get(item, 0)
-
-
-class TxIn(BaseModel):
-    """A quantity of a blockchain asset."""
-
-    tx_hash: str
-    tx_index: int
-
-
-def _unit_alias(unit: str) -> str:
-    """Rename unit alias.
-
-    If a unit alias is input, it changes it to "unit". Otherwise, passes the value
-    through.
-
-    Arg:
-        unit: The unit alias, or passthrough.
-    """
-    if unit in ["asset"]:
-        return "unit"
-    else:
-        return unit
-
-
-class Assets(BaseDict):
-    """Contains all tokens and quantities."""
-
-    __root__: Dict[str, int]
-
-    def unit(self, index: int = 0):
-        """Units of asset at `index`."""
-        return list(self.keys())[index]
-
-    def quantity(self, index: int = 0):
-        """Quantity of the asset at `index`."""
-        return list(self.values())[index]
-
-    @root_validator(pre=True)
-    def _digest_assets(cls, values):
-        if "__root__" in values:
-            root = values["__root__"]
-        elif "values" in values and isinstance(values["values"], list):
-            root = {v.unit: v.quantity for v in values["values"]}
-        else:
-            root = {k: v for k, v in values.items()}
-        root = dict(
-            sorted(root.items(), key=lambda x: "" if x[0] == "lovelace" else x[0])
-        )
-
-        return {"__root__": root}
-
-    def __add__(a, b):
-        """Add two assets."""
-        intersection = set(a.keys()) | set(b.keys())
-
-        result = {key: a[key] + b[key] for key in intersection}
-
-        return Assets(**result)
-
-    def __sub__(a, b):
-        """Add two assets."""
-        intersection = set(a.keys()) | set(b.keys())
-
-        result = {key: a[key] - b[key] for key in intersection}
-
-        return Assets(**result)
-
-
-class Address(BaseModel):
-    """A Cardano address.
-
-    This class holds Cardano address information, including payment, stake, and script
-    addresses. The input should be the `bech32` encoded address.
-    """
-
-    bech32: str
-    address: pycardano.Address
-    payment: Optional[pycardano.Address]
-    stake: Optional[pycardano.Address]
-
-    class Config:  # noqa: D106
-        arbitrary_types_allowed = True
-
-    @root_validator(pre=True)
-    def translate_address(cls, values):  # noqa: D102
-        assert "bech32" in values
-
-        values["address"] = pycardano.Address.decode(values["bech32"])
-
-        if values["address"].staking_part is not None:
-            values["stake"] = pycardano.Address(
-                staking_part=values["address"].staking_part
-            )
-        else:
-            values["stake"] = None
-
-        if values["address"].payment_part is not None:
-            values["payment"] = pycardano.Address(
-                payment_part=values["address"].payment_part
-            )
-        else:
-            values["payment"] = None
-
-        return values
-
-
-class OnchainMetadata(blockfrost_models.AssetOnchainMetadataCip25):
-    """Data class to hold on chain metadata for an asset."""
-
-
-class Metadata(blockfrost_models.Metadata1):
-    """Asset metadata.
-
-    TODO: Remove this in the future.
-    """
-
-
-class OnchainMetadataStandard(Enum):
-    """On chain metadata standard version.
-
-    This class only exists because Genius Yield follows CIP68, and the blockfrost API
-    doesn't handle it well.
-
-    https://cips.cardano.org/cips/cip25/
-    https://cips.cardano.org/cips/cip68/
-    """
-
-    CIP25v1 = "CIP25v1"
-    CIP25v2 = "CIP25v2"
-    CIP68v1 = "CIP68v1"
-
-
-class AssetIdentity(blockfrost_models.Asset1):
-    """A blockchain asset."""
-
-    @root_validator(pre=True)
-    def _validate_asset_name(cls, values):
-        """Handle missing asset metadata.
-
-        Liqwid's qADA did not include asset_name in their metadata. This attempts to
-        find the asset name in another piece of metadata.
-
-        qADA policy: a04ce7a52545e5e33c2867e148898d9e667a69602285f6a1298f9d68
-        """
-        if values["asset_name"] is None:
-            if values["metadata"] is not None:
-                values["asset_name"] = values["metadata"]["name"]
-
-        return values
-
-    class Config:  # noqa: D106
-        use_enum_values = True
-
-    @property
-    def decimals(self) -> int:
-        """Decimal precision of the asset."""
-        if self.metadata is not None and self.metadata.decimals is not None:
-            return self.metadata.decimals
-        else:
-            return 0
-
-
-class AddressUtxoContentItem(blockfrost_models.AddressUtxoContentItem):
-    """An address UTxO item."""
-
-
-class AddressUtxoContent(blockfrost_models.AddressUtxoContent, BaseList):
-    """An address UTxO list of items."""
-
-    __root__: List[
-        AddressUtxoContentItem
-    ] = blockfrost_models.AddressUtxoContent.__fields__[
-        "__root__"
-    ]  # type:ignore
-
-
-class Input(blockfrost_models.Input):
-    """An input to a transaction."""
-
-
-class Output(blockfrost_models.Output):
-    """An output to a transaction."""
-
-
-class TxContentUtxo(blockfrost_models.TxContentUtxo):
-    """A Transaction, containing all inputs and outputs."""
+"""Standard models and model conversion functions.
+
+This module contains common models used throughout minswap-py as well as utility
+functions for converting data types.
+"""
+
+from collections.abc import Iterable
+from datetime import datetime
+from enum import Enum
+from typing import Any, Dict, List, Optional, Union
+
+import pycardano
+from blockfrost import Namespace
+from pydantic import BaseModel, root_validator
+
+from minswap.models import blockfrost_models
+
+
+def to_dict(
+    values: Union[Namespace, List[Any], Dict[str, Any]]
+) -> Union[List[Any], Dict[str, Any]]:
+    """Traverse a dictionary and convert blockfrost.Namespace objects to dictionaries.
+
+    When using `blockfrost.Namespace.to_dict` function to convert a `Namespace` object
+    to a `dict`, child values that are `Namespace` objects are not converted to a
+    `dict`. This function traverse a `Namespace`, `List`, or `Dict` and converts any
+    child values from `Namespace` to `dict`. This is necessary for casting to
+    `pydantic` models for proper error checking and validation.
+
+    Traversel of the input is recursive, ensuring all children are converted.
+
+    Args:
+        values: A `Namespace`, `List`, or `Dict` to be recursively traversed.
+
+    Returns:
+        Union[List[Any], Dict[Any, Any], Dict[str, Any]]
+    """
+    iterator: Optional[Iterable] = None
+
+    if isinstance(values, (Namespace)):
+        values = values.to_dict()
+
+    if isinstance(values, list):
+        iterator = enumerate(values)
+    elif isinstance(values, dict):
+        iterator = values.items()
+
+    if iterator is not None:
+        for k, v in iterator:
+            if isinstance(v, Namespace):
+                values[k] = to_dict(v.to_dict())
+            elif isinstance(v, (list, dict)):
+                values[k] = to_dict(v)
+
+        assert isinstance(values, (list, dict)), f"Error: {values}"
+
+    return values
+
+
+class PoolHistory(BaseModel):
+    """A historical point in the pool."""
+
+    tx_hash: str
+    tx_index: int
+    block_height: int
+    time: datetime
+
+
+class PoolTransactionReference(BaseModel):
+    """A reference to a pool transaction state."""
+
+    tx_index: int
+    tx_hash: str
+    block_height: int
+    block_time: datetime
+
+    @root_validator(pre=True)
+    def _validator(cls, values):
+        values["block_time"] = datetime.utcfromtimestamp(values["block_time"])
+
+        return values
+
+    class Config:  # noqa: D106
+        allow_mutation = False
+        extra = "forbid"
+
+
+class Transaction(blockfrost_models.TxContent):
+    """Transaction Content."""
+
+    block_time: datetime = blockfrost_models.TxContent.__fields__[
+        "block_time"
+    ]  # type: ignore
+
+    @root_validator(pre=True)
+    def _validator(cls, values):
+        values["block_time"] = datetime.utcfromtimestamp(values["block_time"])
+
+        return values
+
+
+class AssetHistoryReference(BaseModel):
+    """A reference to a pool transaction state."""
+
+    tx_hash: str
+    action: str
+    amount: int
+
+    class Config:  # noqa: D106
+        allow_mutation = False
+        extra = "forbid"
+
+
+class BaseList(BaseModel):
+    """Utility class for list models."""
+
+    def __iter__(self):  # noqa
+        return iter(self.__root__)
+
+    def __getitem__(self, item):  # noqa
+        return self.__root__[item]
+
+    def __len__(self):  # noqa
+        return len(self.__root__)
+
+
+class BaseDict(BaseList):
+    """Utility class for dict models."""
+
+    def items(self):
+        """Return iterable of key-value pairs."""
+        return self.__root__.items()
+
+    def keys(self):
+        """Return iterable of keys."""
+        return self.__root__.keys()
+
+    def values(self):
+        """Return iterable of values."""
+        return self.__root__.values()
+
+    def __getitem__(self, item):  # noqa
+        return self.__root__.get(item, 0)
+
+
+class TxIn(BaseModel):
+    """A quantity of a blockchain asset."""
+
+    tx_hash: str
+    tx_index: int
+
+
+def _unit_alias(unit: str) -> str:
+    """Rename unit alias.
+
+    If a unit alias is input, it changes it to "unit". Otherwise, passes the value
+    through.
+
+    Arg:
+        unit: The unit alias, or passthrough.
+    """
+    if unit in ["asset"]:
+        return "unit"
+    else:
+        return unit
+
+
+class Assets(BaseDict):
+    """Contains all tokens and quantities."""
+
+    __root__: Dict[str, int]
+
+    def unit(self, index: int = 0):
+        """Units of asset at `index`."""
+        return list(self.keys())[index]
+
+    def quantity(self, index: int = 0):
+        """Quantity of the asset at `index`."""
+        return list(self.values())[index]
+
+    @root_validator(pre=True)
+    def _digest_assets(cls, values):
+        if "__root__" in values:
+            root = values["__root__"]
+        elif "values" in values and isinstance(values["values"], list):
+            root = {v.unit: v.quantity for v in values["values"]}
+        else:
+            root = {k: v for k, v in values.items()}
+        root = dict(
+            sorted(root.items(), key=lambda x: "" if x[0] == "lovelace" else x[0])
+        )
+
+        return {"__root__": root}
+
+    def __add__(a, b):
+        """Add two assets."""
+        intersection = set(a.keys()) | set(b.keys())
+
+        result = {key: a[key] + b[key] for key in intersection}
+
+        return Assets(**result)
+
+    def __sub__(a, b):
+        """Add two assets."""
+        intersection = set(a.keys()) | set(b.keys())
+
+        result = {key: a[key] - b[key] for key in intersection}
+
+        return Assets(**result)
+
+
+class Address(BaseModel):
+    """A Cardano address.
+
+    This class holds Cardano address information, including payment, stake, and script
+    addresses. The input should be the `bech32` encoded address.
+    """
+
+    bech32: str
+    address: pycardano.Address
+    payment: Optional[pycardano.Address]
+    stake: Optional[pycardano.Address]
+
+    class Config:  # noqa: D106
+        arbitrary_types_allowed = True
+
+    @root_validator(pre=True)
+    def translate_address(cls, values):  # noqa: D102
+        assert "bech32" in values
+
+        values["address"] = pycardano.Address.decode(values["bech32"])
+
+        if values["address"].staking_part is not None:
+            values["stake"] = pycardano.Address(
+                staking_part=values["address"].staking_part
+            )
+        else:
+            values["stake"] = None
+
+        if values["address"].payment_part is not None:
+            values["payment"] = pycardano.Address(
+                payment_part=values["address"].payment_part
+            )
+        else:
+            values["payment"] = None
+
+        return values
+
+
+class OnchainMetadata(blockfrost_models.AssetOnchainMetadataCip25):
+    """Data class to hold on chain metadata for an asset."""
+
+
+class Metadata(blockfrost_models.Metadata1):
+    """Asset metadata.
+
+    TODO: Remove this in the future.
+    """
+
+
+class OnchainMetadataStandard(Enum):
+    """On chain metadata standard version.
+
+    This class only exists because Genius Yield follows CIP68, and the blockfrost API
+    doesn't handle it well.
+
+    https://cips.cardano.org/cips/cip25/
+    https://cips.cardano.org/cips/cip68/
+    """
+
+    CIP25v1 = "CIP25v1"
+    CIP25v2 = "CIP25v2"
+    CIP68v1 = "CIP68v1"
+
+
+class AssetIdentity(blockfrost_models.Asset1):
+    """A blockchain asset."""
+
+    @root_validator(pre=True)
+    def _validate_asset_name(cls, values):
+        """Handle missing asset metadata.
+
+        Liqwid's qADA did not include asset_name in their metadata. This attempts to
+        find the asset name in another piece of metadata.
+
+        qADA policy: a04ce7a52545e5e33c2867e148898d9e667a69602285f6a1298f9d68
+        """
+        if values["asset_name"] is None:
+            if values["metadata"] is not None:
+                values["asset_name"] = values["metadata"]["name"]
+
+        return values
+
+    class Config:  # noqa: D106
+        use_enum_values = True
+
+    @property
+    def decimals(self) -> int:
+        """Decimal precision of the asset."""
+        if self.metadata is not None and self.metadata.decimals is not None:
+            return self.metadata.decimals
+        else:
+            return 0
+
+
+class AddressUtxoContentItem(blockfrost_models.AddressUtxoContentItem):
+    """An address UTxO item."""
+
+
+class AddressUtxoContent(blockfrost_models.AddressUtxoContent, BaseList):
+    """An address UTxO list of items."""
+
+    __root__: List[
+        AddressUtxoContentItem
+    ] = blockfrost_models.AddressUtxoContent.__fields__[
+        "__root__"
+    ]  # type:ignore
+
+
+class Input(blockfrost_models.Input):
+    """An input to a transaction."""
+
+
+class Output(blockfrost_models.Output):
+    """An output to a transaction."""
+
+
+class TxContentUtxo(blockfrost_models.TxContentUtxo):
+    """A Transaction, containing all inputs and outputs."""
```

### Comparing `minswap_py-0.2.0/src/minswap/pools.py` & `minswap_py-0.2.1/src/minswap/pools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Functions for processing minswap pools.
 
 This mostly reflects the pool functionality in the minswap-blockfrostadapter.
 """
 import logging
+from concurrent.futures import ThreadPoolExecutor
 from decimal import Decimal
 from typing import List, Optional, Tuple, Union
 
 from pydantic import BaseModel, root_validator
 
 from minswap import addr
 from minswap.assets import naturalize_assets
@@ -40,17 +41,20 @@
         utxo: A list of UTxOs.
 
     Raises:
         ValueError: Invalid `address`.
         ValueError: No factory token found in utxos.
     """
     # Check to make sure the pool address is correct
-    correct_address: bool = utxo.address == addr.POOL.address.encode()
+    correct_address: bool = utxo.address in [a.address.encode() for a in addr.POOL]
     if not correct_address:
-        message = f"Invalid pool address. Expected {addr.POOL}"
+        message = (
+            "Invalid pool address. Expected one of "
+            + f"{[a.address.encode() for a in addr.POOL]}"
+        )
         logger.debug(message)
         raise InvalidPool(message)
 
     # Check to make sure the pool has 1 factory token
     for asset in utxo.amount:
         has_factory: bool = (
             f"{addr.FACTORY_POLICY_ID}{addr.FACTORY_ASSET_NAME}" == asset.unit
@@ -298,17 +302,28 @@
     Args:
         return_non_pools: If True, returns UTxOs not belonging to pools as a second
             output. Default is False.
 
     Returns:
         A list of pools, and a list of non-pool UTxOs (if specified)
     """
-    utxos_raw = BlockfrostBackend.api().address_utxos(
-        addr.POOL.address.encode(), gather_pages=True, order="asc", return_type="json"
-    )
+    utxos_raw = []
+
+    with ThreadPoolExecutor() as executor:
+        threads = executor.map(
+            lambda x: BlockfrostBackend.api().address_utxos(
+                x.address.encode(),
+                gather_pages=True,
+                order="desc",
+                return_type="json",
+            ),
+            addr.POOL,
+        )
+        for pool_addr in threads:
+            utxos_raw.extend(pool_addr)
 
     utxos = AddressUtxoContent.parse_obj(utxos_raw)
 
     pools: List[PoolState] = []
     non_pools: List[AddressUtxoContentItem] = []
 
     for utxo in utxos:
@@ -340,15 +355,15 @@
 
     Returns:
         A `PoolState` if a pool is token is found, and `None` otherwise.
     """
     pool_tx = BlockfrostBackend.api().transaction_utxos(tx_hash, return_type="json")
     pool_utxo = None
     for utxo in TxContentUtxo.parse_obj(pool_tx).outputs:
-        if utxo.address == addr.POOL.bech32:
+        if utxo.address in [pool.bech32 for pool in addr.POOL]:
             pool_utxo = utxo
             break
 
     if pool_utxo is None:
         return None
 
     check_valid_pool_output(pool_utxo)
```

### Comparing `minswap_py-0.2.0/src/minswap/utils.py` & `minswap_py-0.2.1/src/minswap/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,296 +1,296 @@
-"""Utility functions."""
-import logging
-import os
-import time
-from datetime import datetime
-from pathlib import Path
-from threading import Lock
-from typing import Callable, List, Optional, Union
-
-import blockfrost
-import pandas
-import vaex
-from dotenv import load_dotenv
-
-import minswap
-
-logger = logging.getLogger(__name__)
-
-CACHE_GLOB = "[0-9][0-9][0-9][0-9][0-9][0-9].arrow"
-
-# Load the project information
-load_dotenv()
-PROJECT_ID = os.environ["PROJECT_ID"]
-MAX_CALLS = int(os.environ["MAX_CALLS"])
-call_lock = Lock()
-
-
-class BlockfrostCallLimit(Exception):
-    """Error when the Blockfrost call limit is reached."""
-
-
-class BlockfrostBackend:
-    """A class to enforce stall calls to Blockfrost when a rate limit is hit."""
-
-    last_call: float = time.time()
-    num_limit_calls: float = 0.0
-    max_limit_calls: int = 500
-    total_calls = 0
-    max_total_calls = MAX_CALLS
-    backoff_time: int = 10
-    _api = blockfrost.BlockFrostApi(PROJECT_ID)
-
-    @classmethod
-    def remaining_calls(cls) -> int:
-        """Remaining calls before rate limit."""
-        return cls.max_total_calls - cls.total_calls
-
-    @classmethod
-    def reset_total_calls(cls) -> None:
-        """Reset the call count."""
-        cls.total_calls = 0
-
-    @classmethod
-    def _limiter(cls):
-        with call_lock:
-            cls.num_limit_calls += 1
-            cls.total_calls += 1
-            if cls.total_calls >= cls.max_total_calls:
-                raise BlockfrostCallLimit(
-                    f"Made {cls.total_calls}, "
-                    + f"only {cls.max_total_calls} are allowed."
-                )
-            elif cls.num_limit_calls >= cls.max_limit_calls:
-                logger.warning(
-                    "At or near blockfrost rate limit. "
-                    + f"Waiting {cls.backoff_time}s..."
-                )
-                time.sleep(cls.backoff_time)
-                logger.info("Finished sleeping, resuming...")
-
-        now = time.time()
-        cls.num_limit_calls = max(0, cls.num_limit_calls - (now - cls.last_call) * 10)
-        cls.last_call = now
-
-    @classmethod
-    def api(cls):
-        """Blockfrost API with rate limits."""
-        cls._limiter()
-        return cls._api
-
-    @classmethod
-    def rate_limit(cls, func):
-        """Wrap with rate limit.
-
-        This can probably be removed. It might have utility in the future for
-        customizing imposing rate limits on a function.
-
-        """
-
-        def wrapper(*args, **kwargs):
-            cls._limiter()
-            try:
-                return func(*args, **kwargs)
-            except blockfrost.ApiError:
-                print(f"cls.num_limit_calls: {cls.num_limit_calls}")
-                raise
-
-        return wrapper
-
-
-def save_timestamp(
-    basepath: Path, arg_num: int, kwarg_key: str, func: Optional[Callable] = None
-) -> Callable:
-    """Timestamp cache decorator.
-
-    Args:
-        basepath: Path to save the timestamp to.
-        arg_num: Argument position that should be used to append to basepath.
-        kwarg_key: Alternative to arg_num, in case kwarg is supplied instead of an arg.
-        func: Function to wrap. Defaults to None.
-
-    Returns:
-        Wrapped function that will have a timestamp dumped to disk.
-    """
-    if func is None:
-        return lambda x: save_timestamp(
-            basepath=basepath, arg_num=arg_num, kwarg_key=kwarg_key, func=x
-        )
-
-    def wrapper(*args, **kwargs):
-        if len(args) - 1 >= arg_num:
-            key = args[arg_num]
-        else:
-            key = kwargs[kwarg_key]
-
-        if hasattr(key, "id"):
-            identifier = key.id
-        else:
-            identifier = key
-
-        path = basepath.joinpath(identifier)
-
-        path.mkdir(exist_ok=True, parents=True)
-
-        with open(path.joinpath("TIMESTAMP"), "w") as fw:
-            fw.write(str(time.time()))
-
-        return func(*args, **kwargs)
-
-    return wrapper
-
-
-def load_timestamp(path: Path) -> datetime:
-    """Load a timestamp for a cache.
-
-    Args:
-        path: Path to cache.
-
-    Returns:
-        A datetime object for when the function was called.
-    """
-    with open(path.joinpath("TIMESTAMP")) as fr:
-        timestamp = datetime.utcfromtimestamp(float(fr.read()))
-
-    return timestamp
-
-
-def _get_cache(cache_path: Path, glob: str = CACHE_GLOB) -> Optional[vaex.DataFrame]:
-    if len(list(cache_path.glob(glob))) > 0:
-        df = vaex.open(cache_path.joinpath(glob))
-    else:
-        df = None
-
-    return df
-
-
-def _cache_timestamp_data(
-    data: Union[
-        List[minswap.models.PoolTransactionReference],
-        List[minswap.models.Transaction],
-        List[pandas.DataFrame],
-    ],
-    cache_path: Path,
-    hash_filter: bool = False,
-) -> Union[
-    List[minswap.models.PoolTransactionReference],
-    List[minswap.models.Transaction],
-    List[pandas.DataFrame],
-]:
-    """Cache a list of objects.
-
-    This is a utility function to cache a list of objects containing a timestamp. It
-    searches the list for a change in the timestamp month, caches data for the first
-    occurring month, and returns the rest.
-
-    Args:
-        data: A list of objects containing a time element.
-        cache_path: The path to where the data should be stored.
-
-    Raises:
-        TypeError: `data` must be one of [PoolTransactionReference, pandas.DataFrame]
-
-    Returns:
-        _description_
-    """
-    # Convert data to a vaex dataframe
-    if isinstance(
-        data[0], (minswap.models.PoolTransactionReference, minswap.models.Transaction)
-    ):
-        if data[0].block_time.month == data[-1].block_time.month:
-            index = len(data)
-        else:
-            for index in range(len(data) - 1):
-                if data[index].block_time.month != data[index + 1].block_time.month:
-                    index += 1
-                    break
-        df = pandas.DataFrame([d.dict() for d in data[:index]])
-    elif isinstance(data[0], pandas.DataFrame):
-        if data[0].block_time[0].month == data[-1].block_time[0].month:  # type: ignore
-            index = len(data)
-        else:
-            for index in range(len(data) - 1):
-                if (
-                    data[index].block_time[0].month  # type:ignore
-                    != data[index + 1].block_time[0].month  # type: ignore
-                ):
-                    index += 1
-                    break
-        df = pandas.concat(data, ignore_index=True)
-    else:
-        raise TypeError(
-            "Transactions should be one of [pydantic.BaseModel, pandas.DataFrame]"
-        )
-
-    df["block_time"] = df.block_time.astype("datetime64[s]")
-    df.sort_values(by="block_time", inplace=True)
-
-    # Define the output path
-    cache_name = (
-        f"{df.block_time[0].year}" + f"{str(df.block_time[0].month).zfill(2)}.arrow"
-    )
-    path = cache_path.joinpath(cache_name)
-
-    # If the cache exists, append to it
-    if path.exists():
-        cache_df = pandas.read_feather(path)
-        tmp_path = path.with_name(path.name.replace(".arrow", "_temp.arrow"))
-        if hash_filter:
-            unique_hashes = list(
-                set(df.hash.values.tolist()) - set(cache_df.hash.values.tolist())
-            )
-            filtered = df[df.hash.isin(unique_hashes)]
-        else:
-            threshold = cache_df.block_time.astype("datetime64[s]").values[-1]
-            filtered = df[df.block_time > threshold]
-
-        logger.info(len(filtered))
-        if len(filtered) > 0:
-            pandas.concat([cache_df, filtered], ignore_index=True).sort_values(
-                by="block_time"
-            ).reset_index(drop=True).to_feather(tmp_path)
-            path.unlink()
-            tmp_path.rename(path)
-
-    # Otherwise, just dump the whole dataframe to cache
-    else:
-        df.sort_values(by="block_time", inplace=True)
-        df.reset_index(drop=True, inplace=True)
-        df.to_feather(path)
-
-    return data[index:]
-
-
-def get_utxo(
-    tx_hash: str,
-) -> pandas.DataFrame:
-    """Get a list of pool history transactions.
-
-    This returns a pandas dataframe containing all inputs and UTXOs for a particular
-    transaction.
-
-    Args:
-        pool_id: The unique pool id.
-        page: The index of paginated results to return. Defaults to 1.
-        count: The total number of results to return. Defaults to 100.
-        order: Must be "asc" or "desc". Defaults to "desc".
-
-    Returns:
-        A list of `PoolHistory` items.
-    """
-    tx = BlockfrostBackend.api().transaction_utxos(tx_hash, return_type="json")
-
-    # TODO: Need to create a pydantic model for this
-    df = (
-        pandas.concat(
-            [pandas.DataFrame(tx["inputs"]), pandas.DataFrame(tx["outputs"])],
-            keys=["input", "output"],
-        )
-        .reset_index(level=0)
-        .reset_index(drop=True)
-    )
-
-    df.rename(columns={"level_0": "side"}, inplace=True)
-    df["hash"] = tx["hash"]
-
-    return df
+"""Utility functions."""
+import logging
+import os
+import time
+from datetime import datetime
+from pathlib import Path
+from threading import Lock
+from typing import Callable, List, Optional, Union
+
+import blockfrost
+import pandas
+import vaex
+from dotenv import load_dotenv
+
+import minswap
+
+logger = logging.getLogger(__name__)
+
+CACHE_GLOB = "[0-9][0-9][0-9][0-9][0-9][0-9].arrow"
+
+# Load the project information
+load_dotenv()
+PROJECT_ID = os.environ["PROJECT_ID"]
+MAX_CALLS = int(os.environ["MAX_CALLS"])
+call_lock = Lock()
+
+
+class BlockfrostCallLimit(Exception):
+    """Error when the Blockfrost call limit is reached."""
+
+
+class BlockfrostBackend:
+    """A class to enforce stall calls to Blockfrost when a rate limit is hit."""
+
+    last_call: float = time.time()
+    num_limit_calls: float = 0.0
+    max_limit_calls: int = 500
+    total_calls = 0
+    max_total_calls = MAX_CALLS
+    backoff_time: int = 10
+    _api = blockfrost.BlockFrostApi(PROJECT_ID)
+
+    @classmethod
+    def remaining_calls(cls) -> int:
+        """Remaining calls before rate limit."""
+        return cls.max_total_calls - cls.total_calls
+
+    @classmethod
+    def reset_total_calls(cls) -> None:
+        """Reset the call count."""
+        cls.total_calls = 0
+
+    @classmethod
+    def _limiter(cls):
+        with call_lock:
+            cls.num_limit_calls += 1
+            cls.total_calls += 1
+            if cls.total_calls >= cls.max_total_calls:
+                raise BlockfrostCallLimit(
+                    f"Made {cls.total_calls}, "
+                    + f"only {cls.max_total_calls} are allowed."
+                )
+            elif cls.num_limit_calls >= cls.max_limit_calls:
+                logger.warning(
+                    "At or near blockfrost rate limit. "
+                    + f"Waiting {cls.backoff_time}s..."
+                )
+                time.sleep(cls.backoff_time)
+                logger.info("Finished sleeping, resuming...")
+
+        now = time.time()
+        cls.num_limit_calls = max(0, cls.num_limit_calls - (now - cls.last_call) * 10)
+        cls.last_call = now
+
+    @classmethod
+    def api(cls):
+        """Blockfrost API with rate limits."""
+        cls._limiter()
+        return cls._api
+
+    @classmethod
+    def rate_limit(cls, func):
+        """Wrap with rate limit.
+
+        This can probably be removed. It might have utility in the future for
+        customizing imposing rate limits on a function.
+
+        """
+
+        def wrapper(*args, **kwargs):
+            cls._limiter()
+            try:
+                return func(*args, **kwargs)
+            except blockfrost.ApiError:
+                print(f"cls.num_limit_calls: {cls.num_limit_calls}")
+                raise
+
+        return wrapper
+
+
+def save_timestamp(
+    basepath: Path, arg_num: int, kwarg_key: str, func: Optional[Callable] = None
+) -> Callable:
+    """Timestamp cache decorator.
+
+    Args:
+        basepath: Path to save the timestamp to.
+        arg_num: Argument position that should be used to append to basepath.
+        kwarg_key: Alternative to arg_num, in case kwarg is supplied instead of an arg.
+        func: Function to wrap. Defaults to None.
+
+    Returns:
+        Wrapped function that will have a timestamp dumped to disk.
+    """
+    if func is None:
+        return lambda x: save_timestamp(
+            basepath=basepath, arg_num=arg_num, kwarg_key=kwarg_key, func=x
+        )
+
+    def wrapper(*args, **kwargs):
+        if len(args) - 1 >= arg_num:
+            key = args[arg_num]
+        else:
+            key = kwargs[kwarg_key]
+
+        if hasattr(key, "id"):
+            identifier = key.id
+        else:
+            identifier = key
+
+        path = basepath.joinpath(identifier)
+
+        path.mkdir(exist_ok=True, parents=True)
+
+        with open(path.joinpath("TIMESTAMP"), "w") as fw:
+            fw.write(str(time.time()))
+
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+def load_timestamp(path: Path) -> datetime:
+    """Load a timestamp for a cache.
+
+    Args:
+        path: Path to cache.
+
+    Returns:
+        A datetime object for when the function was called.
+    """
+    with open(path.joinpath("TIMESTAMP")) as fr:
+        timestamp = datetime.utcfromtimestamp(float(fr.read()))
+
+    return timestamp
+
+
+def _get_cache(cache_path: Path, glob: str = CACHE_GLOB) -> Optional[vaex.DataFrame]:
+    if len(list(cache_path.glob(glob))) > 0:
+        df = vaex.open(cache_path.joinpath(glob))
+    else:
+        df = None
+
+    return df
+
+
+def _cache_timestamp_data(
+    data: Union[
+        List[minswap.models.PoolTransactionReference],
+        List[minswap.models.Transaction],
+        List[pandas.DataFrame],
+    ],
+    cache_path: Path,
+    hash_filter: bool = False,
+) -> Union[
+    List[minswap.models.PoolTransactionReference],
+    List[minswap.models.Transaction],
+    List[pandas.DataFrame],
+]:
+    """Cache a list of objects.
+
+    This is a utility function to cache a list of objects containing a timestamp. It
+    searches the list for a change in the timestamp month, caches data for the first
+    occurring month, and returns the rest.
+
+    Args:
+        data: A list of objects containing a time element.
+        cache_path: The path to where the data should be stored.
+
+    Raises:
+        TypeError: `data` must be one of [PoolTransactionReference, pandas.DataFrame]
+
+    Returns:
+        _description_
+    """
+    # Convert data to a vaex dataframe
+    if isinstance(
+        data[0], (minswap.models.PoolTransactionReference, minswap.models.Transaction)
+    ):
+        if data[0].block_time.month == data[-1].block_time.month:
+            index = len(data)
+        else:
+            for index in range(len(data) - 1):
+                if data[index].block_time.month != data[index + 1].block_time.month:
+                    index += 1
+                    break
+        df = pandas.DataFrame([d.dict() for d in data[:index]])
+    elif isinstance(data[0], pandas.DataFrame):
+        if data[0].block_time[0].month == data[-1].block_time[0].month:  # type: ignore
+            index = len(data)
+        else:
+            for index in range(len(data) - 1):
+                if (
+                    data[index].block_time[0].month  # type:ignore
+                    != data[index + 1].block_time[0].month  # type: ignore
+                ):
+                    index += 1
+                    break
+        df = pandas.concat(data, ignore_index=True)
+    else:
+        raise TypeError(
+            "Transactions should be one of [pydantic.BaseModel, pandas.DataFrame]"
+        )
+
+    df["block_time"] = df.block_time.astype("datetime64[s]")
+    df.sort_values(by="block_time", inplace=True)
+
+    # Define the output path
+    cache_name = (
+        f"{df.block_time[0].year}" + f"{str(df.block_time[0].month).zfill(2)}.arrow"
+    )
+    path = cache_path.joinpath(cache_name)
+
+    # If the cache exists, append to it
+    if path.exists():
+        cache_df = pandas.read_feather(path)
+        tmp_path = path.with_name(path.name.replace(".arrow", "_temp.arrow"))
+        if hash_filter:
+            unique_hashes = list(
+                set(df.hash.values.tolist()) - set(cache_df.hash.values.tolist())
+            )
+            filtered = df[df.hash.isin(unique_hashes)]
+        else:
+            threshold = cache_df.block_time.astype("datetime64[s]").values[-1]
+            filtered = df[df.block_time > threshold]
+
+        logger.info(len(filtered))
+        if len(filtered) > 0:
+            pandas.concat([cache_df, filtered], ignore_index=True).sort_values(
+                by="block_time"
+            ).reset_index(drop=True).to_feather(tmp_path)
+            path.unlink()
+            tmp_path.rename(path)
+
+    # Otherwise, just dump the whole dataframe to cache
+    else:
+        df.sort_values(by="block_time", inplace=True)
+        df.reset_index(drop=True, inplace=True)
+        df.to_feather(path)
+
+    return data[index:]
+
+
+def get_utxo(
+    tx_hash: str,
+) -> pandas.DataFrame:
+    """Get a list of pool history transactions.
+
+    This returns a pandas dataframe containing all inputs and UTXOs for a particular
+    transaction.
+
+    Args:
+        pool_id: The unique pool id.
+        page: The index of paginated results to return. Defaults to 1.
+        count: The total number of results to return. Defaults to 100.
+        order: Must be "asc" or "desc". Defaults to "desc".
+
+    Returns:
+        A list of `PoolHistory` items.
+    """
+    tx = BlockfrostBackend.api().transaction_utxos(tx_hash, return_type="json")
+
+    # TODO: Need to create a pydantic model for this
+    df = (
+        pandas.concat(
+            [pandas.DataFrame(tx["inputs"]), pandas.DataFrame(tx["outputs"])],
+            keys=["input", "output"],
+        )
+        .reset_index(level=0)
+        .reset_index(drop=True)
+    )
+
+    df.rename(columns={"level_0": "side"}, inplace=True)
+    df["hash"] = tx["hash"]
+
+    return df
```

### Comparing `minswap_py-0.2.0/PKG-INFO` & `minswap_py-0.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minswap-py
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Home-page: https://github.com/theeldermillenial/minswap-py
 License: MIT
 Author: eldermillenial
 Author-email: eldermillenial@protonmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,29 +20,55 @@
 Requires-Dist: python-dotenv (==0.21.1)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: vaex (>=4.16.0,<5.0.0)
 Project-URL: Issues, https://github.com/theeldermillenial/minswap-py/issues
 Project-URL: Repository, https://github.com/theeldermillenial/minswap-py
 Description-Content-Type: text/markdown
 
-# minswap-py (v0.2.0)
+# minswap-py (v0.2.1)
 <p align="center">
     <img src="https://img.shields.io/pypi/status/minswap-py?style=flat-square" />
     <img src="https://img.shields.io/pypi/dm/minswap-py?style=flat-square" />
     <img src="https://img.shields.io/pypi/l/minswap-py?style=flat-square"/>
     <img src="https://img.shields.io/pypi/v/minswap-py?style=flat-square"/>
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 `minswap-py` is a tool to interact with [Minswap](https://minswap.org/).  The current version has feature parity with the minswap [blockfrost-adapter](https://github.com/minswap/blockfrost-adapter).
 
 Documentation and additional features coming soon.
 
+This tool was recently used to help generate data for the Minswap DAO Emissions and
+Treasury report. You can read the report here:
+
+https://minswap.org/storage/2023/06/31-3-2023_Emissions_and_Treasury_Report.pdf
+
+## Have a question?
+
+Reach out to me on the Minswap discord. You can usually find me on`#technical`, and I'm happy to respond to questions there.
+
+https://discord.com/channels/829060079248343090/845208119729979402
+
+## Support
+
+If you find this project useful, please consider supporting the project by buying me a
+beer in the form of ADA or MIN:
+
+```bash
+addr1q9hw8fuex09vr3rqwtn4fzh9qxjlzjzh8aww684ln0rv0cfu3f0de6qkmh7c7yysfz808978wwe6ll30wu8l3cgvgdjqa7egnl
+```
+
 ## Changelog
 
+### 0.2.1
+
+There are now multiple Minswap pool addresses. This patch updates the code to read all of them when using `minswap.get_pools` and subsequent functions that require pool addresses.
+
+### v0.2.0
+
 Added CHANGELOG.md :)
 
 Improvements:
 1. Added a blockfrost rate limiter. Every call to blockfrost adds to a time delayed counter, and prevents running into rate limits. This helps to prevent abuse of the blockfrost API.
 2. Added significant transaction and asset functionality. It is now possible to pull in asset historys.
 
 Changes:
```

#### html2text {}

```diff
@@ -1,33 +1,44 @@
-Metadata-Version: 2.1 Name: minswap-py Version: 0.2.0 Summary: Home-page:
+Metadata-Version: 2.1 Name: minswap-py Version: 0.2.1 Summary: Home-page:
 https://github.com/theeldermillenial/minswap-py License: MIT Author:
 eldermillenial Author-email: eldermillenial@protonmail.com Requires-Python:
 >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: blockfrost-python
 (==0.5.2) Requires-Dist: llvmlite (>=0.39.1,<0.40.0) Requires-Dist: numba
 (>=0.56.4,<0.57.0) Requires-Dist: pycardano (==0.7.2) Requires-Dist: pydantic
 (==1.10.4) Requires-Dist: python-dotenv (==0.21.1) Requires-Dist: tqdm
 (>=4.65.0,<5.0.0) Requires-Dist: vaex (>=4.16.0,<5.0.0) Project-URL: Issues,
 https://github.com/theeldermillenial/minswap-py/issues Project-URL: Repository,
 https://github.com/theeldermillenial/minswap-py Description-Content-Type: text/
-markdown # minswap-py (v0.2.0)
+markdown # minswap-py (v0.2.1)
   [https://img.shields.io/pypi/status/minswap-py?style=flat-square] [https://
  img.shields.io/pypi/dm/minswap-py?style=flat-square] [https://img.shields.io/
  pypi/l/minswap-py?style=flat-square] [https://img.shields.io/pypi/v/minswap-
                    py?style=flat-square] [Code_style:_black]
 `minswap-py` is a tool to interact with [Minswap](https://minswap.org/). The
 current version has feature parity with the minswap [blockfrost-adapter](https:
 //github.com/minswap/blockfrost-adapter). Documentation and additional features
-coming soon. ## Changelog Added CHANGELOG.md :) Improvements: 1. Added a
-blockfrost rate limiter. Every call to blockfrost adds to a time delayed
-counter, and prevents running into rate limits. This helps to prevent abuse of
-the blockfrost API. 2. Added significant transaction and asset functionality.
-It is now possible to pull in asset historys. Changes: 1. There was an
-inconsistency in how time values were being cached. See the `examples/
-rename_time.py` for a way to translate previously cached data to the new
-standard. ## Quickstart In order to use this package: 1. Install with `pip
+coming soon. This tool was recently used to help generate data for the Minswap
+DAO Emissions and Treasury report. You can read the report here: https://
+minswap.org/storage/2023/06/31-3-2023_Emissions_and_Treasury_Report.pdf ## Have
+a question? Reach out to me on the Minswap discord. You can usually find me
+on`#technical`, and I'm happy to respond to questions there. https://
+discord.com/channels/829060079248343090/845208119729979402 ## Support If you
+find this project useful, please consider supporting the project by buying me a
+beer in the form of ADA or MIN: ```bash
+addr1q9hw8fuex09vr3rqwtn4fzh9qxjlzjzh8aww684ln0rv0cfu3f0de6qkmh7c7yysfz808978wwe6ll30wu8l3cgvgdjqa7egnl
+``` ## Changelog ### 0.2.1 There are now multiple Minswap pool addresses. This
+patch updates the code to read all of them when using `minswap.get_pools` and
+subsequent functions that require pool addresses. ### v0.2.0 Added CHANGELOG.md
+:) Improvements: 1. Added a blockfrost rate limiter. Every call to blockfrost
+adds to a time delayed counter, and prevents running into rate limits. This
+helps to prevent abuse of the blockfrost API. 2. Added significant transaction
+and asset functionality. It is now possible to pull in asset historys. Changes:
+1. There was an inconsistency in how time values were being cached. See the
+`examples/rename_time.py` for a way to translate previously cached data to the
+new standard. ## Quickstart In order to use this package: 1. Install with `pip
 install minswap-py` 2. Sign up for blockfrost and get an API key. 3. In your
 working directory, save a `.env` file. In this file, save your blockfrost API
 key as follows: ```bash PROJECT_ID=YOUR_BLOCKFROST_ID ``` Once you do this, you
 can try out the code in the `examples` folder on the Github repository.
```

