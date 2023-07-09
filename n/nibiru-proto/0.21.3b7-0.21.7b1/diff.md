# Comparing `tmp/nibiru_proto-0.21.3b7.tar.gz` & `tmp/nibiru_proto-0.21.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nibiru_proto-0.21.3b7.tar", max compression
+gzip compressed data, was "nibiru_proto-0.21.7b1.tar", max compression
```

## Comparing `nibiru_proto-0.21.3b7.tar` & `nibiru_proto-0.21.7b1.tar`

### file list

```diff
@@ -1,544 +1,545 @@
--rw-r--r--   0        0        0     1069 2022-08-17 01:57:49.915436 nibiru_proto-0.21.3b7/LICENSE
--rw-r--r--   0        0        0       84 2023-07-04 00:17:01.407673 nibiru_proto-0.21.3b7/nibiru_proto/__init__.py
--rw-r--r--   0        0        0     2028 2023-07-04 00:16:54.277673 nibiru_proto-0.21.3b7/nibiru_proto/amino/amino_pb2.py
--rw-r--r--   0        0        0     3227 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/amino/amino_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.257673 nibiru_proto-0.21.3b7/nibiru_proto/amino/amino_pb2_grpc.py
--rw-r--r--   0        0        0     2012 2023-07-04 00:16:57.867673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.py
--rw-r--r--   0        0        0     4237 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.887673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1817 2023-07-04 00:16:57.967673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/config_pb2.py
--rw-r--r--   0        0        0     5300 2023-07-04 00:15:50.431751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.037673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/config_pb2_grpc.py
--rw-r--r--   0        0        0     1968 2023-07-04 00:16:57.917673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/module_pb2.py
--rw-r--r--   0        0        0     6817 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.927673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1539 2023-07-04 00:16:57.987673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/query_pb2.py
--rw-r--r--   0        0        0     1426 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/query_pb2.pyi
--rw-r--r--   0        0        0     2603 2023-07-04 00:16:58.017673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1794 2023-07-04 00:16:55.807673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/module/v1/module_pb2.py
--rw-r--r--   0        0        0     2675 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.827673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     4605 2023-07-04 00:16:55.857674 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.py
--rw-r--r--   0        0        0     5282 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.877673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/auth_pb2_grpc.py
--rw-r--r--   0        0        0     1899 2023-07-04 00:16:55.897673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1555 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.927673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    12503 2023-07-04 00:16:55.967673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    14414 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    19125 2023-07-04 00:16:55.997673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2810 2023-07-04 00:16:55.947673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1842 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2743 2023-07-04 00:16:56.017673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1295 2023-07-04 00:16:58.797673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/module/v1/module_pb2.py
--rw-r--r--   0        0        0      578 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.827673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     4039 2023-07-04 00:16:58.887673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     4440 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.857673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0     2402 2023-07-04 00:16:58.947673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/event_pb2.py
--rw-r--r--   0        0        0     2114 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:59.067673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/event_pb2_grpc.py
--rw-r--r--   0        0        0     1717 2023-07-04 00:16:58.917673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1194 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.977673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     5558 2023-07-04 00:16:59.027673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     7628 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6331 2023-07-04 00:16:59.047673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     5129 2023-07-04 00:16:59.007673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     4700 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     6246 2023-07-04 00:16:59.097673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     4201 2023-07-04 00:16:56.977673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/options_pb2.py
--rw-r--r--   0        0        0    12271 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/options_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.997673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/options_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-07-04 00:16:57.017673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/query_pb2.py
--rw-r--r--   0        0        0     2362 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/query_pb2.pyi
--rw-r--r--   0        0        0     2886 2023-07-04 00:16:57.037673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1439 2023-07-04 00:16:56.087673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1637 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.107673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2480 2023-07-04 00:16:56.147673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     1703 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.127673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0     6001 2023-07-04 00:16:56.327673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.py
--rw-r--r--   0        0        0     8210 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.267673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/bank_pb2_grpc.py
--rw-r--r--   0        0        0     4070 2023-07-04 00:16:56.177673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     3902 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.197673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    16803 2023-07-04 00:16:56.237673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    23149 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    21828 2023-07-04 00:16:56.287673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     6511 2023-07-04 00:16:56.217673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     6731 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     8074 2023-07-04 00:16:56.307673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     7125 2023-07-04 00:16:57.657673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.py
--rw-r--r--   0        0        0    13374 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.637673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.py
--rw-r--r--   0        0        0     1570 2023-07-04 00:16:57.237673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.py
--rw-r--r--   0        0        0     1558 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.207673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.py
--rw-r--r--   0        0        0     1868 2023-07-04 00:16:57.267673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     1213 2023-07-04 00:15:50.441751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     2762 2023-07-04 00:16:57.297673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/node/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1598 2023-07-04 00:16:57.457673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.py
--rw-r--r--   0        0        0     3440 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.437673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.py
--rw-r--r--   0        0        0     3071 2023-07-04 00:16:57.407673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.py
--rw-r--r--   0        0        0     3055 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi
--rw-r--r--   0        0        0     5144 2023-07-04 00:16:57.387673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0    10963 2023-07-04 00:16:57.357673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py
--rw-r--r--   0        0        0    23085 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi
--rw-r--r--   0        0        0    13573 2023-07-04 00:16:57.327673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0     4501 2023-07-04 00:16:57.587673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py
--rw-r--r--   0        0        0     8467 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.607673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.py
--rw-r--r--   0        0        0     2626 2023-07-04 00:16:57.507673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.py
--rw-r--r--   0        0        0     3087 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.477673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.py
--rw-r--r--   0        0        0     2508 2023-07-04 00:16:57.537673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.py
--rw-r--r--   0        0        0     5092 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.567673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2_grpc.py
--rw-r--r--   0        0        0    11465 2023-07-04 00:16:57.707673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    18881 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    14492 2023-07-04 00:16:57.727673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4471 2023-07-04 00:16:57.747673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.py
--rw-r--r--   0        0        0     5547 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.677673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2_grpc.py
--rw-r--r--   0        0        0     3165 2023-07-04 00:16:57.777673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/v1beta1/coin_pb2.py
--rw-r--r--   0        0        0     2703 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/v1beta1/coin_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.797673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/v1beta1/coin_pb2_grpc.py
--rw-r--r--   0        0        0     1383 2023-07-04 00:17:00.947673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1020 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:00.967673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2171 2023-07-04 00:17:01.057673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.py
--rw-r--r--   0        0        0     2304 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.007673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/capability_pb2_grpc.py
--rw-r--r--   0        0        0     2274 2023-07-04 00:17:00.987673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2428 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.037673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1370 2023-07-04 00:16:59.437673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/module/v1/module_pb2.py
--rw-r--r--   0        0        0      925 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:59.447673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2013 2023-07-04 00:16:59.347673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/query_pb2.py
--rw-r--r--   0        0        0     1699 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/query_pb2.pyi
--rw-r--r--   0        0        0     2626 2023-07-04 00:16:59.387673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2441 2023-07-04 00:16:59.327673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/tx_pb2.py
--rw-r--r--   0        0        0     2431 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     2734 2023-07-04 00:16:59.417673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1447 2023-07-04 00:16:58.267673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1178 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.287673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1727 2023-07-04 00:16:58.317673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1192 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.337673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3940 2023-07-04 00:16:58.367673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     3256 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4533 2023-07-04 00:16:58.397673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2264 2023-07-04 00:16:55.617673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.py
--rw-r--r--   0        0        0     1690 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.587673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/ed25519/keys_pb2_grpc.py
--rw-r--r--   0        0        0     1796 2023-07-04 00:16:55.637673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.py
--rw-r--r--   0        0        0     1822 2023-07-04 00:15:50.451751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.657673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2_grpc.py
--rw-r--r--   0        0        0     2566 2023-07-04 00:16:55.697673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.py
--rw-r--r--   0        0        0     4311 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.677673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2_grpc.py
--rw-r--r--   0        0        0     2088 2023-07-04 00:16:55.787673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/keys_pb2.py
--rw-r--r--   0        0        0     1351 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.717673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/keys_pb2_grpc.py
--rw-r--r--   0        0        0     1778 2023-07-04 00:16:55.767673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py
--rw-r--r--   0        0        0     2062 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.737673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.py
--rw-r--r--   0        0        0     1893 2023-07-04 00:16:55.567673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.py
--rw-r--r--   0        0        0     1519 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.547673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2_grpc.py
--rw-r--r--   0        0        0     1829 2023-07-04 00:16:55.527673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.py
--rw-r--r--   0        0        0     1523 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.497673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2_grpc.py
--rw-r--r--   0        0        0     1481 2023-07-04 00:16:59.467673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1108 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:59.487673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0    10924 2023-07-04 00:16:59.617673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.py
--rw-r--r--   0        0        0    13195 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:59.507673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.py
--rw-r--r--   0        0        0    13143 2023-07-04 00:16:59.527673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0    13975 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:59.557673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    19296 2023-07-04 00:16:59.627673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    18475 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    20401 2023-07-04 00:16:59.647673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0    10831 2023-07-04 00:16:59.587673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     9210 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0    12766 2023-07-04 00:16:59.667673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1316 2023-07-04 00:16:58.427673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/module/v1/module_pb2.py
--rw-r--r--   0        0        0      581 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.447673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2529 2023-07-04 00:16:58.587673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.py
--rw-r--r--   0        0        0     1725 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.557673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.py
--rw-r--r--   0        0        0     1336 2023-07-04 00:16:58.477673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1155 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.507673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3644 2023-07-04 00:16:58.617673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     4284 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     4459 2023-07-04 00:16:58.637673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     3011 2023-07-04 00:16:58.527673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2009 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2754 2023-07-04 00:16:58.667673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1316 2023-07-04 00:16:55.047673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.py
--rw-r--r--   0        0        0      581 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.067673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     6689 2023-07-04 00:16:55.087674 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.py
--rw-r--r--   0        0        0     6923 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.197673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.py
--rw-r--r--   0        0        0     1735 2023-07-04 00:16:55.107674 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1188 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.127673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     5469 2023-07-04 00:16:55.177673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     6877 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6420 2023-07-04 00:16:55.217673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4183 2023-07-04 00:16:55.157673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     3210 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4601 2023-07-04 00:16:55.237673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1308 2023-07-04 00:16:58.687673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/module/v1/module_pb2.py
--rw-r--r--   0        0        0      581 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.717673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1693 2023-07-04 00:16:58.737673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1086 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.767673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1398 2023-07-04 00:16:56.527673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1211 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.547673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2379 2023-07-04 00:16:56.357673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/genesis_pb2.py
--rw-r--r--   0        0        0     3758 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.377673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    11245 2023-07-04 00:16:56.407673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/gov_pb2.py
--rw-r--r--   0        0        0    20071 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/gov_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.467673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/gov_pb2_grpc.py
--rw-r--r--   0        0        0     9987 2023-07-04 00:16:56.447673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/query_pb2.py
--rw-r--r--   0        0        0    16420 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/query_pb2.pyi
--rw-r--r--   0        0        0    14263 2023-07-04 00:16:56.497673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     9114 2023-07-04 00:16:56.427673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/tx_pb2.py
--rw-r--r--   0        0        0    10599 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/tx_pb2.pyi
--rw-r--r--   0        0        0    11056 2023-07-04 00:16:56.507673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     3409 2023-07-04 00:16:56.567673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     3284 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.597673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    15268 2023-07-04 00:16:56.607673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.py
--rw-r--r--   0        0        0    16658 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.687673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/gov_pb2_grpc.py
--rw-r--r--   0        0        0    12442 2023-07-04 00:16:56.657673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    15960 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    14598 2023-07-04 00:16:56.707673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     7991 2023-07-04 00:16:56.637673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     6779 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     7675 2023-07-04 00:16:56.727673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1999 2023-07-04 00:16:59.987673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1639 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:00.037673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     3952 2023-07-04 00:16:59.777673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/events_pb2.py
--rw-r--r--   0        0        0     7707 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:59.697673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/events_pb2_grpc.py
--rw-r--r--   0        0        0     1830 2023-07-04 00:16:59.747673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/genesis_pb2.py
--rw-r--r--   0        0        0     3456 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:59.817673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    16886 2023-07-04 00:16:59.867673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/query_pb2.py
--rw-r--r--   0        0        0    28391 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/query_pb2.pyi
--rw-r--r--   0        0        0    25990 2023-07-04 00:16:59.887673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0    20486 2023-07-04 00:16:59.837673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/tx_pb2.py
--rw-r--r--   0        0        0    26007 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/tx_pb2.pyi
--rw-r--r--   0        0        0    25421 2023-07-04 00:16:59.957673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0    12444 2023-07-04 00:16:59.917673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/types_pb2.py
--rw-r--r--   0        0        0    26963 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:59.717673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/types_pb2_grpc.py
--rw-r--r--   0        0        0     1433 2023-07-04 00:16:55.267673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1100 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.287673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1969 2023-07-04 00:16:55.337674 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1405 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.367673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3948 2023-07-04 00:16:55.307673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.py
--rw-r--r--   0        0        0     2598 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:55.387673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/mint_pb2_grpc.py
--rw-r--r--   0        0        0     4507 2023-07-04 00:16:55.427673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     3563 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6210 2023-07-04 00:16:55.457673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2810 2023-07-04 00:16:55.407673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1842 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2744 2023-07-04 00:16:55.477673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1477 2023-07-04 00:16:57.827673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/msg/v1/msg_pb2.py
--rw-r--r--   0        0        0     1385 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/msg/v1/msg_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.847673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/msg/v1/msg_pb2_grpc.py
--rw-r--r--   0        0        0     1285 2023-07-04 00:17:00.667673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/module/v1/module_pb2.py
--rw-r--r--   0        0        0      576 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:00.687673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     1734 2023-07-04 00:17:00.737673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/event_pb2.py
--rw-r--r--   0        0        0     2997 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:00.897673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/event_pb2_grpc.py
--rw-r--r--   0        0        0     1600 2023-07-04 00:17:00.707673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2311 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:00.757673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     1901 2023-07-04 00:17:00.787673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.py
--rw-r--r--   0        0        0     3664 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:00.827673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/nft_pb2_grpc.py
--rw-r--r--   0        0        0     6909 2023-07-04 00:17:00.847673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    11302 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    12817 2023-07-04 00:17:00.877673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2352 2023-07-04 00:17:00.807673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1765 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2511 2023-07-04 00:17:00.917673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1307 2023-07-04 00:16:56.797673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.py
--rw-r--r--   0        0        0      712 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.817673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2_grpc.py
--rw-r--r--   0        0        0     4021 2023-07-04 00:16:56.847673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.py
--rw-r--r--   0        0        0    10489 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.pyi
--rw-r--r--   0        0        0     4388 2023-07-04 00:16:56.867673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2416 2023-07-04 00:16:56.767673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1/orm_pb2.py
--rw-r--r--   0        0        0     7527 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1/orm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.747673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1/orm_pb2_grpc.py
--rw-r--r--   0        0        0     2205 2023-07-04 00:16:56.917673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.py
--rw-r--r--   0        0        0     7358 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.887673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2_grpc.py
--rw-r--r--   0        0        0     1303 2023-07-04 00:17:00.507673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/module/v1/module_pb2.py
--rw-r--r--   0        0        0      579 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:00.527673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     2599 2023-07-04 00:17:00.587673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/params_pb2.py
--rw-r--r--   0        0        0     2127 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:00.557673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/params_pb2_grpc.py
--rw-r--r--   0        0        0     3388 2023-07-04 00:17:00.617673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     3996 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     4478 2023-07-04 00:17:00.637673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1337 2023-07-04 00:16:56.937673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/query/v1/query_pb2.py
--rw-r--r--   0        0        0     1548 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/query/v1/query_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:56.957673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/query/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1947 2023-07-04 00:16:56.067673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/reflection/v1/reflection_pb2.py
--rw-r--r--   0        0        0     1551 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/reflection/v1/reflection_pb2.pyi
--rw-r--r--   0        0        0     3070 2023-07-04 00:16:56.037673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/reflection/v1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0     1365 2023-07-04 00:17:01.087673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/module/v1/module_pb2.py
--rw-r--r--   0        0        0      924 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.107673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     4107 2023-07-04 00:17:01.147673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     4850 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.177673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     5207 2023-07-04 00:17:01.217673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     5194 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6284 2023-07-04 00:17:01.237673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4640 2023-07-04 00:17:01.287673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.py
--rw-r--r--   0        0        0     4327 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.127673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.py
--rw-r--r--   0        0        0     3903 2023-07-04 00:17:01.197673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2693 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4596 2023-07-04 00:17:01.267673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1411 2023-07-04 00:17:00.097673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/module/v1/module_pb2.py
--rw-r--r--   0        0        0     1516 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:00.167673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     3300 2023-07-04 00:17:00.227673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     5176 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:00.197673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0     4470 2023-07-04 00:17:00.297673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     4598 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:00.357673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    24823 2023-07-04 00:17:00.427673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    29039 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    27948 2023-07-04 00:17:00.457673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0    26092 2023-07-04 00:17:00.327673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.py
--rw-r--r--   0        0        0    31868 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:00.267673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/staking_pb2_grpc.py
--rw-r--r--   0        0        0    15825 2023-07-04 00:17:00.397673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0    13555 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0    13680 2023-07-04 00:17:00.487673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1429 2023-07-04 00:16:58.067673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/config/v1/config_pb2.py
--rw-r--r--   0        0        0     1349 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/config/v1/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.087673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/config/v1/config_pb2_grpc.py
--rw-r--r--   0        0        0     3253 2023-07-04 00:16:58.137673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.py
--rw-r--r--   0        0        0    10213 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.117673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.py
--rw-r--r--   0        0        0    10601 2023-07-04 00:16:58.187673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/service_pb2.py
--rw-r--r--   0        0        0    20455 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/service_pb2.pyi
--rw-r--r--   0        0        0    16593 2023-07-04 00:16:58.217673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/service_pb2_grpc.py
--rw-r--r--   0        0        0     7188 2023-07-04 00:16:58.167673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0    21980 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:58.237673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1357 2023-07-04 00:16:59.127673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.py
--rw-r--r--   0        0        0      923 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:59.157673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     5663 2023-07-04 00:16:59.257673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     7077 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    10523 2023-07-04 00:16:59.287673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     3740 2023-07-04 00:16:59.227673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2804 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4582 2023-07-04 00:16:59.317673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     4427 2023-07-04 00:16:59.177673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.py
--rw-r--r--   0        0        0     5694 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:59.207673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.py
--rw-r--r--   0        0        0     1318 2023-07-04 00:16:57.067673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/module/v1/module_pb2.py
--rw-r--r--   0        0        0      580 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/module/v1/module_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.087673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/module/v1/module_pb2_grpc.py
--rw-r--r--   0        0        0     6897 2023-07-04 00:16:57.157673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     5521 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     6844 2023-07-04 00:16:57.187673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     7472 2023-07-04 00:16:57.107673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.py
--rw-r--r--   0        0        0     7735 2023-07-04 00:15:50.471751 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:57.137673 nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.py
--rw-r--r--   0        0        0     2961 2023-07-04 00:16:54.307674 nibiru_proto-0.21.3b7/nibiru_proto/cosmos_proto/cosmos_pb2.py
--rw-r--r--   0        0        0     7141 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/cosmos_proto/cosmos_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.327674 nibiru_proto-0.21.3b7/nibiru_proto/cosmos_proto/cosmos_pb2_grpc.py
--rw-r--r--   0        0        0    15929 2023-07-04 00:16:54.217673 nibiru_proto-0.21.3b7/nibiru_proto/gogoproto/gogo_pb2.py
--rw-r--r--   0        0        0    15691 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/gogoproto/gogo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.237673 nibiru_proto-0.21.3b7/nibiru_proto/gogoproto/gogo_pb2_grpc.py
--rw-r--r--   0        0        0     1589 2023-07-04 00:17:01.387673 nibiru_proto-0.21.3b7/nibiru_proto/google/api/annotations_pb2.py
--rw-r--r--   0        0        0     1047 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.337673 nibiru_proto-0.21.3b7/nibiru_proto/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     2335 2023-07-04 00:17:01.317673 nibiru_proto-0.21.3b7/nibiru_proto/google/api/http_pb2.py
--rw-r--r--   0        0        0    18274 2023-07-04 00:15:52.611750 nibiru_proto-0.21.3b7/nibiru_proto/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.367673 nibiru_proto-0.21.3b7/nibiru_proto/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0       83 2023-07-04 00:17:03.357673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:01.667673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:01.637673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/__init__.py
--rw-r--r--   0        0        0     1882 2023-07-04 00:17:01.487673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/event_pb2.py
--rw-r--r--   0        0        0     1813 2023-07-04 00:15:52.621750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.617673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/event_pb2_grpc.py
--rw-r--r--   0        0        0     1826 2023-07-04 00:17:01.467673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1108 2023-07-04 00:15:52.621750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.517673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3232 2023-07-04 00:17:01.567673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/query_pb2.py
--rw-r--r--   0        0        0     2319 2023-07-04 00:15:52.621750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/query_pb2.pyi
--rw-r--r--   0        0        0     4391 2023-07-04 00:17:01.587673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2925 2023-07-04 00:17:01.537673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/state_pb2.py
--rw-r--r--   0        0        0     2806 2023-07-04 00:15:52.621750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.437673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/state_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:02.357673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:02.337673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/__init__.py
--rw-r--r--   0        0        0     2569 2023-07-04 00:17:02.227673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/genesis_pb2.py
--rw-r--r--   0        0        0     3486 2023-07-04 00:15:52.631750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:02.247673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     3400 2023-07-04 00:17:02.197673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/inflation_pb2.py
--rw-r--r--   0        0        0     2746 2023-07-04 00:15:52.621750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/inflation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:02.267673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/inflation_pb2_grpc.py
--rw-r--r--   0        0        0     7156 2023-07-04 00:17:02.297673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/query_pb2.py
--rw-r--r--   0        0        0     7309 2023-07-04 00:15:52.621750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/query_pb2.pyi
--rw-r--r--   0        0        0    11695 2023-07-04 00:17:02.317673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:02.977673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:02.917673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/__init__.py
--rw-r--r--   0        0        0     2972 2023-07-04 00:17:02.727673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/event_pb2.py
--rw-r--r--   0        0        0     4208 2023-07-04 00:15:52.631750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:02.897673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/event_pb2_grpc.py
--rw-r--r--   0        0        0     4412 2023-07-04 00:17:02.707673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/genesis_pb2.py
--rw-r--r--   0        0        0     5191 2023-07-04 00:15:52.631750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:02.757673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0    10133 2023-07-04 00:17:02.847673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/oracle_pb2.py
--rw-r--r--   0        0        0     8950 2023-07-04 00:15:52.631750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/oracle_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:02.677673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/oracle_pb2_grpc.py
--rw-r--r--   0        0        0    14073 2023-07-04 00:17:02.827673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/query_pb2.py
--rw-r--r--   0        0        0    15236 2023-07-04 00:15:52.631750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/query_pb2.pyi
--rw-r--r--   0        0        0    21958 2023-07-04 00:17:02.877673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2322 2023-07-04 00:17:02.777673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/state_pb2.py
--rw-r--r--   0        0        0     1119 2023-07-04 00:15:52.631750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:02.657673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/state_pb2_grpc.py
--rw-r--r--   0        0        0     6507 2023-07-04 00:17:02.807673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/tx_pb2.py
--rw-r--r--   0        0        0     4671 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     6667 2023-07-04 00:17:02.947673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:02.627673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:02.587673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/__init__.py
--rw-r--r--   0        0        0    11256 2023-07-04 00:17:02.427673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/event_pb2.py
--rw-r--r--   0        0        0    13948 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:02.557673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/event_pb2_grpc.py
--rw-r--r--   0        0        0     2580 2023-07-04 00:17:02.407673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/genesis_pb2.py
--rw-r--r--   0        0        0     2048 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:02.457673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     7762 2023-07-04 00:17:02.517673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/query_pb2.py
--rw-r--r--   0        0        0     7284 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/query_pb2.pyi
--rw-r--r--   0        0        0     7831 2023-07-04 00:17:02.537673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/query_pb2_grpc.py
--rw-r--r--   0        0        0    10001 2023-07-04 00:17:02.477673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/state_pb2.py
--rw-r--r--   0        0        0    11123 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:02.377673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/state_pb2_grpc.py
--rw-r--r--   0        0        0    15202 2023-07-04 00:17:02.497673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/tx_pb2.py
--rw-r--r--   0        0        0    15581 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/tx_pb2.pyi
--rw-r--r--   0        0        0    11032 2023-07-04 00:17:02.607673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/tx_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:03.327673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:03.247673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/__init__.py
--rw-r--r--   0        0        0     6658 2023-07-04 00:17:03.067673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/event_pb2.py
--rw-r--r--   0        0        0     8332 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:03.227673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/event_pb2_grpc.py
--rw-r--r--   0        0        0     1913 2023-07-04 00:17:03.047673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1530 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:03.087673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     2113 2023-07-04 00:17:03.027673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/params_pb2.py
--rw-r--r--   0        0        0     1850 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:03.007673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/params_pb2_grpc.py
--rw-r--r--   0        0        0     5491 2023-07-04 00:17:03.197673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/pool_pb2.py
--rw-r--r--   0        0        0     5345 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/pool_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:03.297673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/pool_pb2_grpc.py
--rw-r--r--   0        0        0    19864 2023-07-04 00:17:03.137673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/query_pb2.py
--rw-r--r--   0        0        0    21019 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/query_pb2.pyi
--rw-r--r--   0        0        0    29083 2023-07-04 00:17:03.167673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     8804 2023-07-04 00:17:03.117673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/tx_pb2.py
--rw-r--r--   0        0        0     7873 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     7341 2023-07-04 00:17:03.267673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:01.947673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:01.897673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/__init__.py
--rw-r--r--   0        0        0     5369 2023-07-04 00:17:01.787673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/events_pb2.py
--rw-r--r--   0        0        0     5131 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.717673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/events_pb2_grpc.py
--rw-r--r--   0        0        0     2136 2023-07-04 00:17:01.757673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.py
--rw-r--r--   0        0        0     1434 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.807673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0     2062 2023-07-04 00:17:01.737673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/params_pb2.py
--rw-r--r--   0        0        0     3105 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.687673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/params_pb2_grpc.py
--rw-r--r--   0        0        0     8057 2023-07-04 00:17:01.857673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/query_pb2.py
--rw-r--r--   0        0        0     7591 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/query_pb2.pyi
--rw-r--r--   0        0        0     8241 2023-07-04 00:17:01.877673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     7329 2023-07-04 00:17:01.837673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.py
--rw-r--r--   0        0        0     8386 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     8298 2023-07-04 00:17:01.927673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:02.177673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 00:17:02.127673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/__init__.py
--rw-r--r--   0        0        0     1755 2023-07-04 00:17:01.997673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/event_pb2.py
--rw-r--r--   0        0        0     1190 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:02.107673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/event_pb2_grpc.py
--rw-r--r--   0        0        0     2240 2023-07-04 00:17:02.067673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/query_pb2.py
--rw-r--r--   0        0        0     1336 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/query_pb2.pyi
--rw-r--r--   0        0        0     2621 2023-07-04 00:17:02.087673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1810 2023-07-04 00:17:02.017673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/state_pb2.py
--rw-r--r--   0        0        0     1817 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:17:01.967673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/state_pb2_grpc.py
--rw-r--r--   0        0        0     1982 2023-07-04 00:17:02.037673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/tx_pb2.py
--rw-r--r--   0        0        0     1975 2023-07-04 00:15:52.641750 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/tx_pb2.pyi
--rw-r--r--   0        0        0     3057 2023-07-04 00:17:02.157673 nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/tx_pb2_grpc.py
--rw-r--r--   0        0        0    26856 2023-07-04 00:16:55.007673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/abci/types_pb2.py
--rw-r--r--   0        0        0    56049 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/abci/types_pb2.pyi
--rw-r--r--   0        0        0    27809 2023-07-04 00:16:54.977673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/abci/types_pb2_grpc.py
--rw-r--r--   0        0        0     1508 2023-07-04 00:16:54.517673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/keys_pb2.py
--rw-r--r--   0        0        0     1280 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.487673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/keys_pb2_grpc.py
--rw-r--r--   0        0        0     2340 2023-07-04 00:16:54.457673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/proof_pb2.py
--rw-r--r--   0        0        0     4101 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/proof_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.427673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/proof_pb2_grpc.py
--rw-r--r--   0        0        0     1238 2023-07-04 00:16:54.917673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/libs/bits/types_pb2.py
--rw-r--r--   0        0        0     1049 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/libs/bits/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.877673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/libs/bits/types_pb2_grpc.py
--rw-r--r--   0        0        0     3673 2023-07-04 00:16:54.397673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/p2p/types_pb2.py
--rw-r--r--   0        0        0     3901 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/p2p/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.367673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/p2p/types_pb2_grpc.py
--rw-r--r--   0        0        0     2226 2023-07-04 00:16:54.777673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/block_pb2.py
--rw-r--r--   0        0        0     1707 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/block_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.637673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/block_pb2_grpc.py
--rw-r--r--   0        0        0     3741 2023-07-04 00:16:54.747673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/evidence_pb2.py
--rw-r--r--   0        0        0     5767 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/evidence_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.697673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/evidence_pb2_grpc.py
--rw-r--r--   0        0        0     3323 2023-07-04 00:16:54.607674 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/params_pb2.py
--rw-r--r--   0        0        0     6262 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.547673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/params_pb2_grpc.py
--rw-r--r--   0        0        0    11770 2023-07-04 00:16:54.817674 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/types_pb2.py
--rw-r--r--   0        0        0    18408 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.577674 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/types_pb2_grpc.py
--rw-r--r--   0        0        0     2351 2023-07-04 00:16:54.667673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/validator_pb2.py
--rw-r--r--   0        0        0     3356 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/validator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.717673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/validator_pb2_grpc.py
--rw-r--r--   0        0        0     1597 2023-07-04 00:16:54.957673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/version/types_pb2.py
--rw-r--r--   0        0        0     1793 2023-07-04 00:15:50.481751 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/version/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 00:16:54.937673 nibiru_proto-0.21.3b7/nibiru_proto/tendermint/version/types_pb2_grpc.py
--rw-r--r--   0        0        0      853 2023-07-04 00:18:49.571961 nibiru_proto-0.21.3b7/pyproject.toml
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 nibiru_proto-0.21.3b7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-08-17 01:57:49.915436 nibiru_proto-0.21.7b1/LICENSE
+-rw-r--r--   0        0        0       84 2023-07-09 09:36:58.310314 nibiru_proto-0.21.7b1/nibiru_proto/__init__.py
+-rw-r--r--   0        0        0     2028 2023-07-09 09:36:40.743656 nibiru_proto-0.21.7b1/nibiru_proto/amino/amino_pb2.py
+-rw-r--r--   0        0        0     3227 2023-07-09 09:34:20.978872 nibiru_proto-0.21.7b1/nibiru_proto/amino/amino_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:40.693656 nibiru_proto-0.21.7b1/nibiru_proto/amino/amino_pb2_grpc.py
+-rw-r--r--   0        0        0     2012 2023-07-09 09:36:50.253656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.py
+-rw-r--r--   0        0        0     4237 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:50.433656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1817 2023-07-09 09:36:50.593656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/config_pb2.py
+-rw-r--r--   0        0        0     5300 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:50.963656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/config_pb2_grpc.py
+-rw-r--r--   0        0        0     1968 2023-07-09 09:36:50.493656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/module_pb2.py
+-rw-r--r--   0        0        0     6817 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:50.553656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1539 2023-07-09 09:36:50.663656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/query_pb2.py
+-rw-r--r--   0        0        0     1426 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/query_pb2.pyi
+-rw-r--r--   0        0        0     2603 2023-07-09 09:36:50.783656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1794 2023-07-09 09:36:44.323656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     2675 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:44.383656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     4605 2023-07-09 09:36:44.443656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.py
+-rw-r--r--   0        0        0     5282 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:44.493656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/auth_pb2_grpc.py
+-rw-r--r--   0        0        0     1899 2023-07-09 09:36:44.563656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1555 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:44.623656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    12503 2023-07-09 09:36:44.723656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    14414 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    19125 2023-07-09 09:36:44.793656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2810 2023-07-09 09:36:44.683656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1842 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2743 2023-07-09 09:36:44.883656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1295 2023-07-09 09:36:52.893656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      578 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:52.943656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     4039 2023-07-09 09:36:53.043656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     4440 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:52.993656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0     2402 2023-07-09 09:36:53.153656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/event_pb2.py
+-rw-r--r--   0        0        0     2114 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:53.540314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     1717 2023-07-09 09:36:53.103656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1194 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:53.223656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     5558 2023-07-09 09:36:53.363656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     7628 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6331 2023-07-09 09:36:53.460314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     5129 2023-07-09 09:36:53.293656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     4700 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     6246 2023-07-09 09:36:53.600314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     4201 2023-07-09 09:36:47.243656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/autocli/v1/options_pb2.py
+-rw-r--r--   0        0        0    12271 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/autocli/v1/options_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:47.343656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/autocli/v1/options_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-07-09 09:36:47.423656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/autocli/v1/query_pb2.py
+-rw-r--r--   0        0        0     2362 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/autocli/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     2886 2023-07-09 09:36:47.673656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/autocli/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1439 2023-07-09 09:36:45.053656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1637 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:45.103656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2480 2023-07-09 09:36:45.193656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     1703 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:45.143656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0     6001 2023-07-09 09:36:45.593656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.py
+-rw-r--r--   0        0        0     8210 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:45.443656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/bank_pb2_grpc.py
+-rw-r--r--   0        0        0     4070 2023-07-09 09:36:45.243656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     3902 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:45.293656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    16803 2023-07-09 09:36:45.393656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    23149 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    21828 2023-07-09 09:36:45.483656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     6511 2023-07-09 09:36:45.343656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     6731 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     8074 2023-07-09 09:36:45.533656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     7125 2023-07-09 09:36:49.343656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.py
+-rw-r--r--   0        0        0    13374 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:49.273656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.py
+-rw-r--r--   0        0        0     1570 2023-07-09 09:36:48.313656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.py
+-rw-r--r--   0        0        0     1558 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:48.253656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.py
+-rw-r--r--   0        0        0     1868 2023-07-09 09:36:48.363656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     1213 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     2762 2023-07-09 09:36:48.423656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/node/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1598 2023-07-09 09:36:48.783656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.py
+-rw-r--r--   0        0        0     3440 2023-07-09 09:34:20.978872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:48.723656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.py
+-rw-r--r--   0        0        0     3071 2023-07-09 09:36:48.673656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.py
+-rw-r--r--   0        0        0     3055 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi
+-rw-r--r--   0        0        0     5144 2023-07-09 09:36:48.623656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0    10963 2023-07-09 09:36:48.543656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py
+-rw-r--r--   0        0        0    23085 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi
+-rw-r--r--   0        0        0    13573 2023-07-09 09:36:48.473656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0     4501 2023-07-09 09:36:49.123656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py
+-rw-r--r--   0        0        0     8467 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:49.193656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.py
+-rw-r--r--   0        0        0     2626 2023-07-09 09:36:48.913656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.py
+-rw-r--r--   0        0        0     3087 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:48.843656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.py
+-rw-r--r--   0        0        0     2508 2023-07-09 09:36:48.973656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.py
+-rw-r--r--   0        0        0     5092 2023-07-09 09:34:18.418872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:49.063656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2_grpc.py
+-rw-r--r--   0        0        0    11465 2023-07-09 09:36:49.473656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    18881 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    14492 2023-07-09 09:36:49.553656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4471 2023-07-09 09:36:49.613656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.py
+-rw-r--r--   0        0        0     5547 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:49.413656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2_grpc.py
+-rw-r--r--   0        0        0     3165 2023-07-09 09:36:49.673656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/v1beta1/coin_pb2.py
+-rw-r--r--   0        0        0     2703 2023-07-09 09:34:20.978872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/v1beta1/coin_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:49.723656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/v1beta1/coin_pb2_grpc.py
+-rw-r--r--   0        0        0     1383 2023-07-09 09:36:57.290314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1020 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:57.380313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2171 2023-07-09 09:36:57.640313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.py
+-rw-r--r--   0        0        0     2304 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:57.540314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/v1beta1/capability_pb2_grpc.py
+-rw-r--r--   0        0        0     2274 2023-07-09 09:36:57.470313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2428 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:57.590314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1370 2023-07-09 09:36:54.310314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      925 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:54.360314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2013 2023-07-09 09:36:54.160314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/v1/query_pb2.py
+-rw-r--r--   0        0        0     1699 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     2626 2023-07-09 09:36:54.210314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2441 2023-07-09 09:36:54.110314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/v1/tx_pb2.py
+-rw-r--r--   0        0        0     2431 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2734 2023-07-09 09:36:54.260314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1447 2023-07-09 09:36:51.393656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1178 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:51.553656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1727 2023-07-09 09:36:51.623656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1192 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:51.683656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3940 2023-07-09 09:36:51.733656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     3256 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4533 2023-07-09 09:36:51.863656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2264 2023-07-09 09:36:43.733656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.py
+-rw-r--r--   0        0        0     1690 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:43.683656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/ed25519/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     1796 2023-07-09 09:36:43.773656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.py
+-rw-r--r--   0        0        0     1822 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:43.813656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2_grpc.py
+-rw-r--r--   0        0        0     2566 2023-07-09 09:36:43.933656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.py
+-rw-r--r--   0        0        0     4311 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:43.873656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2_grpc.py
+-rw-r--r--   0        0        0     2088 2023-07-09 09:36:44.263656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/multisig/keys_pb2.py
+-rw-r--r--   0        0        0     1351 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/multisig/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:44.053656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/multisig/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     1778 2023-07-09 09:36:44.193656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py
+-rw-r--r--   0        0        0     2062 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:44.123656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.py
+-rw-r--r--   0        0        0     1893 2023-07-09 09:36:43.623656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.py
+-rw-r--r--   0        0        0     1519 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:43.563656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     1829 2023-07-09 09:36:43.493656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.py
+-rw-r--r--   0        0        0     1523 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:43.443656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     1481 2023-07-09 09:36:54.420314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1108 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:54.470314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0    10924 2023-07-09 09:36:54.750314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.py
+-rw-r--r--   0        0        0    13195 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:54.520314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.py
+-rw-r--r--   0        0        0    13143 2023-07-09 09:36:54.560314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0    13975 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:54.610314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    19296 2023-07-09 09:36:54.830314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    18475 2023-07-09 09:34:18.428872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    20401 2023-07-09 09:36:54.900313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0    10831 2023-07-09 09:36:54.670314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     9210 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0    12766 2023-07-09 09:36:54.960314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1316 2023-07-09 09:36:51.933656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      581 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:52.003656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2529 2023-07-09 09:36:52.433656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.py
+-rw-r--r--   0        0        0     1725 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:52.333656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.py
+-rw-r--r--   0        0        0     1336 2023-07-09 09:36:52.073656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1155 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:52.153656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3644 2023-07-09 09:36:52.503656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     4284 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     4459 2023-07-09 09:36:52.553656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3011 2023-07-09 09:36:52.223656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     2009 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2754 2023-07-09 09:36:52.623656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1316 2023-07-09 09:36:42.123656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      581 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:42.163656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     6689 2023-07-09 09:36:42.203656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.py
+-rw-r--r--   0        0        0     6923 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:42.503656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.py
+-rw-r--r--   0        0        0     1735 2023-07-09 09:36:42.253656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1188 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:42.303656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     5469 2023-07-09 09:36:42.413656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     6877 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6420 2023-07-09 09:36:42.563656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4183 2023-07-09 09:36:42.353656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     3210 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4601 2023-07-09 09:36:42.663656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1308 2023-07-09 09:36:52.683656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/genutil/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      581 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/genutil/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:52.743656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/genutil/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1693 2023-07-09 09:36:52.803656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1086 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:52.853656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1398 2023-07-09 09:36:45.953656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1211 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:46.043656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2379 2023-07-09 09:36:45.633656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     3758 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:45.673656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    11245 2023-07-09 09:36:45.703656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/gov_pb2.py
+-rw-r--r--   0        0        0    20071 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/gov_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:45.823656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/gov_pb2_grpc.py
+-rw-r--r--   0        0        0     9987 2023-07-09 09:36:45.783656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/query_pb2.py
+-rw-r--r--   0        0        0    16420 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    14263 2023-07-09 09:36:45.863656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     9114 2023-07-09 09:36:45.743656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/tx_pb2.py
+-rw-r--r--   0        0        0    10599 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0    11056 2023-07-09 09:36:45.903656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     3409 2023-07-09 09:36:46.103656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     3284 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:46.143656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    15268 2023-07-09 09:36:46.183656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.py
+-rw-r--r--   0        0        0    16658 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:46.323656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/gov_pb2_grpc.py
+-rw-r--r--   0        0        0    12442 2023-07-09 09:36:46.273656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    15960 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    14598 2023-07-09 09:36:46.383656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     7991 2023-07-09 09:36:46.223656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     6779 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     7675 2023-07-09 09:36:46.433656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1999 2023-07-09 09:36:55.670313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1639 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:55.710314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     3952 2023-07-09 09:36:55.250314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/events_pb2.py
+-rw-r--r--   0        0        0     7707 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:55.050314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/events_pb2_grpc.py
+-rw-r--r--   0        0        0     1830 2023-07-09 09:36:55.190314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     3456 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:55.290314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    16886 2023-07-09 09:36:55.400313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/query_pb2.py
+-rw-r--r--   0        0        0    28391 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    25990 2023-07-09 09:36:55.470314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0    20486 2023-07-09 09:36:55.330314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/tx_pb2.py
+-rw-r--r--   0        0        0    26007 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0    25421 2023-07-09 09:36:55.630313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0    12444 2023-07-09 09:36:55.570314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/types_pb2.py
+-rw-r--r--   0        0        0    26963 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:55.120314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/types_pb2_grpc.py
+-rw-r--r--   0        0        0     1433 2023-07-09 09:36:42.763656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1100 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:42.833656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1969 2023-07-09 09:36:42.943656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1405 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:43.003656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3948 2023-07-09 09:36:42.893656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.py
+-rw-r--r--   0        0        0     2598 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:43.053656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/mint_pb2_grpc.py
+-rw-r--r--   0        0        0     4507 2023-07-09 09:36:43.293656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     3563 2023-07-09 09:34:18.438872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6210 2023-07-09 09:36:43.343656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2810 2023-07-09 09:36:43.193656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1842 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2744 2023-07-09 09:36:43.393656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1477 2023-07-09 09:36:49.783656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/msg/v1/msg_pb2.py
+-rw-r--r--   0        0        0     1385 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/msg/v1/msg_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:49.863656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/msg/v1/msg_pb2_grpc.py
+-rw-r--r--   0        0        0     1285 2023-07-09 09:36:56.680313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      576 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:56.730313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     1734 2023-07-09 09:36:56.820314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/event_pb2.py
+-rw-r--r--   0        0        0     2997 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:57.190313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     1600 2023-07-09 09:36:56.780314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2311 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:56.870314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     1901 2023-07-09 09:36:56.920313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.py
+-rw-r--r--   0        0        0     3664 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:57.050314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/nft_pb2_grpc.py
+-rw-r--r--   0        0        0     6909 2023-07-09 09:36:57.100314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    11302 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    12817 2023-07-09 09:36:57.150313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2352 2023-07-09 09:36:57.010314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1765 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2511 2023-07-09 09:36:57.230313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1307 2023-07-09 09:36:46.653656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.py
+-rw-r--r--   0        0        0      712 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:46.723656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     4021 2023-07-09 09:36:46.793656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.py
+-rw-r--r--   0        0        0    10489 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.pyi
+-rw-r--r--   0        0        0     4388 2023-07-09 09:36:46.873656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2416 2023-07-09 09:36:46.583656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/v1/orm_pb2.py
+-rw-r--r--   0        0        0     7527 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/v1/orm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:46.503656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/v1/orm_pb2_grpc.py
+-rw-r--r--   0        0        0     2205 2023-07-09 09:36:47.033656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.py
+-rw-r--r--   0        0        0     7358 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:46.953656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     1303 2023-07-09 09:36:56.330314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      579 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:56.370314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2599 2023-07-09 09:36:56.520314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/v1beta1/params_pb2.py
+-rw-r--r--   0        0        0     2127 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/v1beta1/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:56.460313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/v1beta1/params_pb2_grpc.py
+-rw-r--r--   0        0        0     3388 2023-07-09 09:36:56.570314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     3996 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     4478 2023-07-09 09:36:56.630313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1337 2023-07-09 09:36:47.093656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/query/v1/query_pb2.py
+-rw-r--r--   0        0        0     1548 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/query/v1/query_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:47.173656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/query/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1947 2023-07-09 09:36:45.013656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/reflection/v1/reflection_pb2.py
+-rw-r--r--   0        0        0     1551 2023-07-09 09:34:18.448872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/reflection/v1/reflection_pb2.pyi
+-rw-r--r--   0        0        0     3070 2023-07-09 09:36:44.953656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/reflection/v1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0     1365 2023-07-09 09:36:57.680313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      924 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:57.730313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     4107 2023-07-09 09:36:57.830314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     4850 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:57.880313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     5207 2023-07-09 09:36:57.960313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     5194 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6284 2023-07-09 09:36:58.010313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4640 2023-07-09 09:36:58.100314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.py
+-rw-r--r--   0        0        0     4327 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:57.780314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.py
+-rw-r--r--   0        0        0     3903 2023-07-09 09:36:57.920313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     2693 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4596 2023-07-09 09:36:58.050314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1411 2023-07-09 09:36:55.750314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/module/v1/module_pb2.py
+-rw-r--r--   0        0        0     1516 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:55.800314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     3300 2023-07-09 09:36:55.890313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     5176 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:55.840314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0     4470 2023-07-09 09:36:55.990314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     4598 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:56.110314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    24823 2023-07-09 09:36:56.210313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    29039 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    27948 2023-07-09 09:36:56.250314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0    26092 2023-07-09 09:36:56.050314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.py
+-rw-r--r--   0        0        0    31868 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:55.930313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/staking_pb2_grpc.py
+-rw-r--r--   0        0        0    15825 2023-07-09 09:36:56.170313 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0    13555 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0    13680 2023-07-09 09:36:56.290314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1429 2023-07-09 09:36:51.023656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/config/v1/config_pb2.py
+-rw-r--r--   0        0        0     1349 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/config/v1/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:51.073656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/config/v1/config_pb2_grpc.py
+-rw-r--r--   0        0        0     3253 2023-07-09 09:36:51.153656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.py
+-rw-r--r--   0        0        0    10213 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:51.113656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.py
+-rw-r--r--   0        0        0    10601 2023-07-09 09:36:51.233656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/v1beta1/service_pb2.py
+-rw-r--r--   0        0        0    20455 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/v1beta1/service_pb2.pyi
+-rw-r--r--   0        0        0    16593 2023-07-09 09:36:51.283656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/v1beta1/service_pb2_grpc.py
+-rw-r--r--   0        0        0     7188 2023-07-09 09:36:51.193656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0    21980 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:51.333656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1357 2023-07-09 09:36:53.650314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      923 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:53.710314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     5663 2023-07-09 09:36:53.970314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     7077 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    10523 2023-07-09 09:36:54.020314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3740 2023-07-09 09:36:53.930314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     2804 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4582 2023-07-09 09:36:54.060314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     4427 2023-07-09 09:36:53.780314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.py
+-rw-r--r--   0        0        0     5694 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:53.870314 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.py
+-rw-r--r--   0        0        0     1318 2023-07-09 09:36:47.783656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/module/v1/module_pb2.py
+-rw-r--r--   0        0        0      580 2023-07-09 09:34:18.468872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/module/v1/module_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:47.853656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/module/v1/module_pb2_grpc.py
+-rw-r--r--   0        0        0     6897 2023-07-09 09:36:48.133656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     5521 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     6844 2023-07-09 09:36:48.193656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     7472 2023-07-09 09:36:48.003656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.py
+-rw-r--r--   0        0        0     7735 2023-07-09 09:34:18.458872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:48.073656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.py
+-rw-r--r--   0        0        0     2961 2023-07-09 09:36:40.783656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos_proto/cosmos_pb2.py
+-rw-r--r--   0        0        0     7141 2023-07-09 09:34:20.978872 nibiru_proto-0.21.7b1/nibiru_proto/cosmos_proto/cosmos_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:40.823656 nibiru_proto-0.21.7b1/nibiru_proto/cosmos_proto/cosmos_pb2_grpc.py
+-rw-r--r--   0        0        0    15929 2023-07-09 09:36:40.583656 nibiru_proto-0.21.7b1/nibiru_proto/gogoproto/gogo_pb2.py
+-rw-r--r--   0        0        0    15691 2023-07-09 09:34:20.978872 nibiru_proto-0.21.7b1/nibiru_proto/gogoproto/gogo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:40.633656 nibiru_proto-0.21.7b1/nibiru_proto/gogoproto/gogo_pb2_grpc.py
+-rw-r--r--   0        0        0     1589 2023-07-09 09:36:58.270313 nibiru_proto-0.21.7b1/nibiru_proto/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0     1047 2023-07-09 09:34:20.978872 nibiru_proto-0.21.7b1/nibiru_proto/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:58.170313 nibiru_proto-0.21.7b1/nibiru_proto/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     2335 2023-07-09 09:36:58.130313 nibiru_proto-0.21.7b1/nibiru_proto/google/api/http_pb2.py
+-rw-r--r--   0        0        0    18274 2023-07-09 09:34:20.978872 nibiru_proto-0.21.7b1/nibiru_proto/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:58.220313 nibiru_proto-0.21.7b1/nibiru_proto/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:37:03.120313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:36:58.720313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:36:58.680313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/__init__.py
+-rw-r--r--   0        0        0     1882 2023-07-09 09:36:58.430313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/event_pb2.py
+-rw-r--r--   0        0        0     1813 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:58.630313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     1826 2023-07-09 09:36:58.400313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     1108 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:58.470313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3232 2023-07-09 09:36:58.550314 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/query_pb2.py
+-rw-r--r--   0        0        0     2319 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     4391 2023-07-09 09:36:58.590314 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2925 2023-07-09 09:36:58.510313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/state_pb2.py
+-rw-r--r--   0        0        0     2806 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:58.350314 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/state_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:37:00.570313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:37:00.510313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/__init__.py
+-rw-r--r--   0        0        0     2569 2023-07-09 09:36:59.870314 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     3486 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:59.960313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     3400 2023-07-09 09:36:59.830313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/inflation_pb2.py
+-rw-r--r--   0        0        0     2746 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/inflation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:37:00.190313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/inflation_pb2_grpc.py
+-rw-r--r--   0        0        0     7156 2023-07-09 09:37:00.290313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/query_pb2.py
+-rw-r--r--   0        0        0     7309 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    11695 2023-07-09 09:37:00.400313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:37:01.960313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:37:01.850313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/__init__.py
+-rw-r--r--   0        0        0     2972 2023-07-09 09:37:01.420313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/event_pb2.py
+-rw-r--r--   0        0        0     4208 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:37:01.800313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     4412 2023-07-09 09:37:01.370313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     5191 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:37:01.480313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0    10133 2023-07-09 09:37:01.690313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/oracle_pb2.py
+-rw-r--r--   0        0        0     8950 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/oracle_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:37:01.280313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/oracle_pb2_grpc.py
+-rw-r--r--   0        0        0    14073 2023-07-09 09:37:01.640313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/query_pb2.py
+-rw-r--r--   0        0        0    15236 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    21958 2023-07-09 09:37:01.750313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2322 2023-07-09 09:37:01.530313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/state_pb2.py
+-rw-r--r--   0        0        0     1119 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:37:01.230313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/state_pb2_grpc.py
+-rw-r--r--   0        0        0     6507 2023-07-09 09:37:01.580313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/tx_pb2.py
+-rw-r--r--   0        0        0     4671 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     6667 2023-07-09 09:37:01.910313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:37:01.160313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:37:01.030313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/__init__.py
+-rw-r--r--   0        0        0    11256 2023-07-09 09:37:00.700313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/event_pb2.py
+-rw-r--r--   0        0        0    13948 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:37:00.950313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/event_pb2_grpc.py
+-rw-r--r--   0        0        0     2580 2023-07-09 09:37:00.660313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/genesis_pb2.py
+-rw-r--r--   0        0        0     2048 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:37:00.730313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     7762 2023-07-09 09:37:00.850313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/query_pb2.py
+-rw-r--r--   0        0        0     7284 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/query_pb2.pyi
+-rw-r--r--   0        0        0     7831 2023-07-09 09:37:00.890313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/query_pb2_grpc.py
+-rw-r--r--   0        0        0    10001 2023-07-09 09:37:00.780313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/state_pb2.py
+-rw-r--r--   0        0        0    11123 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:37:00.620314 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/state_pb2_grpc.py
+-rw-r--r--   0        0        0    18127 2023-07-09 09:37:00.810313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/tx_pb2.py
+-rw-r--r--   0        0        0    17904 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/tx_pb2.pyi
+-rw-r--r--   0        0        0    12704 2023-07-09 09:37:01.090313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/tx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:37:03.050313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:37:02.870313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/__init__.py
+-rw-r--r--   0        0        0     6658 2023-07-09 09:37:02.260313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/event_pb2.py
+-rw-r--r--   0        0        0     8332 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:37:02.770313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     1913 2023-07-09 09:37:02.190313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     1530 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:37:02.370313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     2113 2023-07-09 09:37:02.120313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/params_pb2.py
+-rw-r--r--   0        0        0     1850 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:37:02.050313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/params_pb2_grpc.py
+-rw-r--r--   0        0        0     5491 2023-07-09 09:37:02.710313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/pool_pb2.py
+-rw-r--r--   0        0        0     5345 2023-07-09 09:34:20.998872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/pool_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:37:02.980313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/pool_pb2_grpc.py
+-rw-r--r--   0        0        0    19864 2023-07-09 09:37:02.590313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/query_pb2.py
+-rw-r--r--   0        0        0    21019 2023-07-09 09:34:20.988872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/query_pb2.pyi
+-rw-r--r--   0        0        0    29083 2023-07-09 09:37:02.650313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     8804 2023-07-09 09:37:02.460313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/tx_pb2.py
+-rw-r--r--   0        0        0     7873 2023-07-09 09:34:20.998872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     7341 2023-07-09 09:37:02.920313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:36:59.230313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:36:59.150313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/__init__.py
+-rw-r--r--   0        0        0     5369 2023-07-09 09:36:58.950313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/events_pb2.py
+-rw-r--r--   0        0        0     5131 2023-07-09 09:34:20.998872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:58.810314 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/events_pb2_grpc.py
+-rw-r--r--   0        0        0     2136 2023-07-09 09:36:58.900313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.py
+-rw-r--r--   0        0        0     1434 2023-07-09 09:34:20.998872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:58.990313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0     2062 2023-07-09 09:36:58.860314 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/params_pb2.py
+-rw-r--r--   0        0        0     3105 2023-07-09 09:34:20.998872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:58.770313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/params_pb2_grpc.py
+-rw-r--r--   0        0        0     8057 2023-07-09 09:36:59.070314 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/query_pb2.py
+-rw-r--r--   0        0        0     7591 2023-07-09 09:34:20.998872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     8241 2023-07-09 09:36:59.110314 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     7329 2023-07-09 09:36:59.030313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.py
+-rw-r--r--   0        0        0     8386 2023-07-09 09:34:20.998872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     8298 2023-07-09 09:36:59.190313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:36:59.780313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:36:59.660313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/__init__.py
+-rw-r--r--   0        0        0     1755 2023-07-09 09:36:59.310313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/event_pb2.py
+-rw-r--r--   0        0        0     1190 2023-07-09 09:34:20.998872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:59.600314 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/event_pb2_grpc.py
+-rw-r--r--   0        0        0     2240 2023-07-09 09:36:59.490313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/query_pb2.py
+-rw-r--r--   0        0        0     1336 2023-07-09 09:34:20.998872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     2621 2023-07-09 09:36:59.540313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1810 2023-07-09 09:36:59.370314 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/state_pb2.py
+-rw-r--r--   0        0        0     1817 2023-07-09 09:34:20.998872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:59.270313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/state_pb2_grpc.py
+-rw-r--r--   0        0        0     1982 2023-07-09 09:36:59.430313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/tx_pb2.py
+-rw-r--r--   0        0        0     1975 2023-07-09 09:34:20.998872 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/tx_pb2.pyi
+-rw-r--r--   0        0        0     3057 2023-07-09 09:36:59.720313 nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-09 09:34:21.068872 nibiru_proto-0.21.7b1/nibiru_proto/py.typed
+-rw-r--r--   0        0        0    26856 2023-07-09 09:36:42.083656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/abci/types_pb2.py
+-rw-r--r--   0        0        0    56049 2023-07-09 09:34:18.468872 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/abci/types_pb2.pyi
+-rw-r--r--   0        0        0    27809 2023-07-09 09:36:42.033656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/abci/types_pb2_grpc.py
+-rw-r--r--   0        0        0     1508 2023-07-09 09:36:41.103656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/crypto/keys_pb2.py
+-rw-r--r--   0        0        0     1280 2023-07-09 09:34:18.468872 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/crypto/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:41.063656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/crypto/keys_pb2_grpc.py
+-rw-r--r--   0        0        0     2340 2023-07-09 09:36:41.013656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/crypto/proof_pb2.py
+-rw-r--r--   0        0        0     4101 2023-07-09 09:34:18.468872 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/crypto/proof_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:40.963656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/crypto/proof_pb2_grpc.py
+-rw-r--r--   0        0        0     1238 2023-07-09 09:36:41.913656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/libs/bits/types_pb2.py
+-rw-r--r--   0        0        0     1049 2023-07-09 09:34:18.468872 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/libs/bits/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:41.873656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/libs/bits/types_pb2_grpc.py
+-rw-r--r--   0        0        0     3673 2023-07-09 09:36:40.923656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/p2p/types_pb2.py
+-rw-r--r--   0        0        0     3901 2023-07-09 09:34:18.468872 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/p2p/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:40.863656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/p2p/types_pb2_grpc.py
+-rw-r--r--   0        0        0     2226 2023-07-09 09:36:41.753656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/block_pb2.py
+-rw-r--r--   0        0        0     1707 2023-07-09 09:34:18.468872 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/block_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:41.363656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/block_pb2_grpc.py
+-rw-r--r--   0        0        0     3741 2023-07-09 09:36:41.683656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/evidence_pb2.py
+-rw-r--r--   0        0        0     5767 2023-07-09 09:34:18.468872 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/evidence_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:41.483656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/evidence_pb2_grpc.py
+-rw-r--r--   0        0        0     3323 2023-07-09 09:36:41.273656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/params_pb2.py
+-rw-r--r--   0        0        0     6262 2023-07-09 09:34:18.468872 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:41.153656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/params_pb2_grpc.py
+-rw-r--r--   0        0        0    11770 2023-07-09 09:36:41.823656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/types_pb2.py
+-rw-r--r--   0        0        0    18408 2023-07-09 09:34:18.468872 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:41.213656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/types_pb2_grpc.py
+-rw-r--r--   0        0        0     2351 2023-07-09 09:36:41.423656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/validator_pb2.py
+-rw-r--r--   0        0        0     3356 2023-07-09 09:34:18.468872 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/validator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:41.543656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/validator_pb2_grpc.py
+-rw-r--r--   0        0        0     1597 2023-07-09 09:36:42.003656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/version/types_pb2.py
+-rw-r--r--   0        0        0     1793 2023-07-09 09:34:18.468872 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/version/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 09:36:41.953656 nibiru_proto-0.21.7b1/nibiru_proto/tendermint/version/types_pb2_grpc.py
+-rw-r--r--   0        0        0      957 2023-07-09 09:41:11.204947 nibiru_proto-0.21.7b1/pyproject.toml
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 nibiru_proto-0.21.7b1/PKG-INFO
```

### Comparing `nibiru_proto-0.21.3b7/LICENSE` & `nibiru_proto-0.21.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/amino/amino_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/amino/amino_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/amino/amino_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/amino/amino_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/runtime/v1alpha1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/config_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/config_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/app/v1alpha1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/app/v1alpha1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/auth/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/auth/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/event_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/event_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/authz/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/authz/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/options_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/autocli/v1/options_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/options_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/autocli/v1/options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/autocli/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/autocli/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/autocli/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/autocli/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/bank_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/bank/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/bank/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/abci/v1beta1/abci_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/kv/v1beta1/kv_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/node/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/node/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/node/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/query/v1beta1/pagination_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/store/v1beta1/listening_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/tendermint/v1beta1/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/v1beta1/coin_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/v1beta1/coin_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/base/v1beta1/coin_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/base/v1beta1/coin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/v1beta1/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/capability/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/consensus/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/consensus/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/ed25519/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/hd/v1/hd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/keyring/v1/record_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/keys_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/multisig/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/keys_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/multisig/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/secp256k1/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/crypto/secp256r1/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/distribution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/evidence_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/genutil/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/genutil/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/genutil/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/gov_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/gov_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/gov_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/gov_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/gov_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/gov/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/gov/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/events_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/events_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/events_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/types_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/group/v1/types_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/group/v1/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/mint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/mint/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/mint/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/msg/v1/msg_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/msg/v1/msg_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/msg/v1/msg_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/msg/v1/msg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/event_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/event_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/nft_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/nft/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/nft/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/module/v1alpha1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/query/v1alpha1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1/orm_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/v1/orm_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1/orm_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/v1/orm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/orm/v1alpha1/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/params_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/v1beta1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/params_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/v1beta1/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/params/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/params/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/query/v1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/query/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/query/v1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/query/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/reflection/v1/reflection_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/reflection/v1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/reflection/v1/reflection_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/reflection/v1/reflection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/reflection/v1/reflection_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/reflection/v1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/slashing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/authz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/staking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/staking/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/staking/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/config/v1/config_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/config/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/config/v1/config_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/config/v1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/service_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/v1beta1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/service_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/v1beta1/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/service_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/v1beta1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/tx/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/module/v1/module_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/module/v1/module_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/module/v1/module_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/module/v1/module_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos/vesting/v1beta1/vesting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos_proto/cosmos_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos_proto/cosmos_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/cosmos_proto/cosmos_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/cosmos_proto/cosmos_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/gogoproto/gogo_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/gogoproto/gogo_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/gogoproto/gogo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/google/api/annotations_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/google/api/annotations_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/google/api/http_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/google/api/http_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/event_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/event_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/state_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/state_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/epochs/v1/state_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/epochs/v1/state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/inflation_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/inflation_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/inflation_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/inflation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/inflation/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/inflation/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/event_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/event_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/oracle_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/oracle_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/oracle_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/oracle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/state_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/state_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/state_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/oracle/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/oracle/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/event_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/event_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/event_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/state_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/state_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/state_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/tx_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from cosmos.base.v1beta1 import coin_pb2 as cosmos_dot_base_dot_v1beta1_dot_coin__pb2
 from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from nibiru_proto.nibiru.perp.v2 import state_pb2 as nibiru_dot_perp_dot_v2_dot_state__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17nibiru/perp/v2/tx.proto\x12\x0enibiru.perp.v2\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x1anibiru/perp/v2/state.proto\"\xb1\x01\n\x0fMsgRemoveMargin\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12\x37\n\x06margin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x06margin\"\xe8\x01\n\x17MsgRemoveMarginResponse\x12>\n\nmargin_out\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\tmarginOut\x12W\n\x0f\x66unding_payment\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12\x34\n\x08position\x18\x03 \x01(\x0b\x32\x18.nibiru.perp.v2.PositionR\x08position\"\xae\x01\n\x0cMsgAddMargin\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12\x37\n\x06margin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x06margin\"\xa5\x01\n\x14MsgAddMarginResponse\x12W\n\x0f\x66unding_payment\x18\x01 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12\x34\n\x08position\x18\x02 \x01(\x0b\x32\x18.nibiru.perp.v2.PositionR\x08position\"\xf4\x01\n\x11MsgMultiLiquidate\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12Q\n\x0cliquidations\x18\x02 \x03(\x0b\x32-.nibiru.perp.v2.MsgMultiLiquidate.LiquidationR\x0cliquidations\x1at\n\x0bLiquidation\x12M\n\x04pair\x18\x01 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12\x16\n\x06trader\x18\x02 \x01(\tR\x06trader\"\xb6\x03\n\x19MsgMultiLiquidateResponse\x12\x61\n\x0cliquidations\x18\x01 \x03(\x0b\x32=.nibiru.perp.v2.MsgMultiLiquidateResponse.LiquidationResponseR\x0cliquidations\x1a\xb5\x02\n\x13LiquidationResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x02 \x01(\tR\x05\x65rror\x12\x46\n\x0eliquidator_fee\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x01R\rliquidatorFee\x12?\n\x0bperp_ef_fee\x18\x04 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x01R\tperpEfFee\x12\x16\n\x06trader\x18\x05 \x01(\tR\x06trader\x12M\n\x04pair\x18\x06 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\"\xb7\x03\n\x0eMsgMarketOrder\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12-\n\x04side\x18\x03 \x01(\x0e\x32\x19.nibiru.perp.v2.DirectionR\x04side\x12\\\n\x12quote_asset_amount\x18\x04 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.IntR\x10quoteAssetAmount\x12J\n\x08leverage\x18\x05 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x08leverage\x12\x65\n\x17\x62\x61se_asset_amount_limit\x18\x06 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.IntR\x14\x62\x61seAssetAmountLimit\"\xe3\x05\n\x16MsgMarketOrderResponse\x12\x34\n\x08position\x18\x01 \x01(\x0b\x32\x18.nibiru.perp.v2.PositionR\x08position\x12h\n\x18\x65xchanged_notional_value\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x16\x65xchangedNotionalValue\x12\x66\n\x17\x65xchanged_position_size\x18\x03 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x15\x65xchangedPositionSize\x12W\n\x0f\x66unding_payment\x18\x04 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12Q\n\x0crealized_pnl\x18\x05 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0brealizedPnl\x12`\n\x14unrealized_pnl_after\x18\x06 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x12unrealizedPnlAfter\x12V\n\x0fmargin_to_vault\x18\x07 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\rmarginToVault\x12[\n\x11position_notional\x18\x08 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x10positionNotional\"y\n\x10MsgClosePosition\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\"\xf2\x03\n\x18MsgClosePositionResponse\x12h\n\x18\x65xchanged_notional_value\x18\x01 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x16\x65xchangedNotionalValue\x12\x66\n\x17\x65xchanged_position_size\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x15\x65xchangedPositionSize\x12W\n\x0f\x66unding_payment\x18\x03 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12Q\n\x0crealized_pnl\x18\x04 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0brealizedPnl\x12X\n\x10margin_to_trader\x18\x07 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0emarginToTrader\"\x82\x01\n\x18MsgDonateToEcosystemFund\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12N\n\x08\x64onation\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x17\xc8\xde\x1f\x00\xf2\xde\x1f\x0fyaml:\"donation\"R\x08\x64onation\"\"\n MsgDonateToEcosystemFundResponse2\xc5\x04\n\x03Msg\x12Z\n\x0cRemoveMargin\x12\x1f.nibiru.perp.v2.MsgRemoveMargin\x1a\'.nibiru.perp.v2.MsgRemoveMarginResponse\"\x00\x12Q\n\tAddMargin\x12\x1c.nibiru.perp.v2.MsgAddMargin\x1a$.nibiru.perp.v2.MsgAddMarginResponse\"\x00\x12`\n\x0eMultiLiquidate\x12!.nibiru.perp.v2.MsgMultiLiquidate\x1a).nibiru.perp.v2.MsgMultiLiquidateResponse\"\x00\x12W\n\x0bMarketOrder\x12\x1e.nibiru.perp.v2.MsgMarketOrder\x1a&.nibiru.perp.v2.MsgMarketOrderResponse\"\x00\x12]\n\rClosePosition\x12 .nibiru.perp.v2.MsgClosePosition\x1a(.nibiru.perp.v2.MsgClosePositionResponse\"\x00\x12u\n\x15\x44onateToEcosystemFund\x12(.nibiru.perp.v2.MsgDonateToEcosystemFund\x1a\x30.nibiru.perp.v2.MsgDonateToEcosystemFundResponse\"\x00\x42/Z-github.com/NibiruChain/nibiru/x/perp/v2/typesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17nibiru/perp/v2/tx.proto\x12\x0enibiru.perp.v2\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x63osmos/base/v1beta1/coin.proto\x1a\x14gogoproto/gogo.proto\x1a\x1anibiru/perp/v2/state.proto\"\xb1\x01\n\x0fMsgRemoveMargin\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12\x37\n\x06margin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x06margin\"\xe8\x01\n\x17MsgRemoveMarginResponse\x12>\n\nmargin_out\x18\x01 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\tmarginOut\x12W\n\x0f\x66unding_payment\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12\x34\n\x08position\x18\x03 \x01(\x0b\x32\x18.nibiru.perp.v2.PositionR\x08position\"\xae\x01\n\x0cMsgAddMargin\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12\x37\n\x06margin\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x00R\x06margin\"\xa5\x01\n\x14MsgAddMarginResponse\x12W\n\x0f\x66unding_payment\x18\x01 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12\x34\n\x08position\x18\x02 \x01(\x0b\x32\x18.nibiru.perp.v2.PositionR\x08position\"\xf4\x01\n\x11MsgMultiLiquidate\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12Q\n\x0cliquidations\x18\x02 \x03(\x0b\x32-.nibiru.perp.v2.MsgMultiLiquidate.LiquidationR\x0cliquidations\x1at\n\x0bLiquidation\x12M\n\x04pair\x18\x01 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12\x16\n\x06trader\x18\x02 \x01(\tR\x06trader\"\xb6\x03\n\x19MsgMultiLiquidateResponse\x12\x61\n\x0cliquidations\x18\x01 \x03(\x0b\x32=.nibiru.perp.v2.MsgMultiLiquidateResponse.LiquidationResponseR\x0cliquidations\x1a\xb5\x02\n\x13LiquidationResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x02 \x01(\tR\x05\x65rror\x12\x46\n\x0eliquidator_fee\x18\x03 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x01R\rliquidatorFee\x12?\n\x0bperp_ef_fee\x18\x04 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x04\xc8\xde\x1f\x01R\tperpEfFee\x12\x16\n\x06trader\x18\x05 \x01(\tR\x06trader\x12M\n\x04pair\x18\x06 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\"\xb7\x03\n\x0eMsgMarketOrder\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12-\n\x04side\x18\x03 \x01(\x0e\x32\x19.nibiru.perp.v2.DirectionR\x04side\x12\\\n\x12quote_asset_amount\x18\x04 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.IntR\x10quoteAssetAmount\x12J\n\x08leverage\x18\x05 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x08leverage\x12\x65\n\x17\x62\x61se_asset_amount_limit\x18\x06 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.IntR\x14\x62\x61seAssetAmountLimit\"\xe3\x05\n\x16MsgMarketOrderResponse\x12\x34\n\x08position\x18\x01 \x01(\x0b\x32\x18.nibiru.perp.v2.PositionR\x08position\x12h\n\x18\x65xchanged_notional_value\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x16\x65xchangedNotionalValue\x12\x66\n\x17\x65xchanged_position_size\x18\x03 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x15\x65xchangedPositionSize\x12W\n\x0f\x66unding_payment\x18\x04 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12Q\n\x0crealized_pnl\x18\x05 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0brealizedPnl\x12`\n\x14unrealized_pnl_after\x18\x06 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x12unrealizedPnlAfter\x12V\n\x0fmargin_to_vault\x18\x07 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\rmarginToVault\x12[\n\x11position_notional\x18\x08 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x10positionNotional\"y\n\x10MsgClosePosition\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\"\xf2\x03\n\x18MsgClosePositionResponse\x12h\n\x18\x65xchanged_notional_value\x18\x01 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x16\x65xchangedNotionalValue\x12\x66\n\x17\x65xchanged_position_size\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x15\x65xchangedPositionSize\x12W\n\x0f\x66unding_payment\x18\x03 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12Q\n\x0crealized_pnl\x18\x04 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0brealizedPnl\x12X\n\x10margin_to_trader\x18\x05 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0emarginToTrader\"\xbc\x01\n\x0fMsgPartialClose\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12M\n\x04pair\x18\x02 \x01(\tB9\xc8\xde\x1f\x00\xda\xde\x1f\x31github.com/NibiruChain/nibiru/x/common/asset.PairR\x04pair\x12\x42\n\x04size\x18\x03 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x04size\"\xf1\x03\n\x17MsgPartialCloseResponse\x12h\n\x18\x65xchanged_notional_value\x18\x01 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x16\x65xchangedNotionalValue\x12\x66\n\x17\x65xchanged_position_size\x18\x02 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x15\x65xchangedPositionSize\x12W\n\x0f\x66unding_payment\x18\x03 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0e\x66undingPayment\x12Q\n\x0crealized_pnl\x18\x04 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0brealizedPnl\x12X\n\x10margin_to_trader\x18\x05 \x01(\tB.\xc8\xde\x1f\x00\xda\xde\x1f&github.com/cosmos/cosmos-sdk/types.DecR\x0emarginToTrader\"\x82\x01\n\x18MsgDonateToEcosystemFund\x12\x16\n\x06sender\x18\x01 \x01(\tR\x06sender\x12N\n\x08\x64onation\x18\x02 \x01(\x0b\x32\x19.cosmos.base.v1beta1.CoinB\x17\xc8\xde\x1f\x00\xf2\xde\x1f\x0fyaml:\"donation\"R\x08\x64onation\"\"\n MsgDonateToEcosystemFundResponse2\xa1\x05\n\x03Msg\x12Z\n\x0cRemoveMargin\x12\x1f.nibiru.perp.v2.MsgRemoveMargin\x1a\'.nibiru.perp.v2.MsgRemoveMarginResponse\"\x00\x12Q\n\tAddMargin\x12\x1c.nibiru.perp.v2.MsgAddMargin\x1a$.nibiru.perp.v2.MsgAddMarginResponse\"\x00\x12`\n\x0eMultiLiquidate\x12!.nibiru.perp.v2.MsgMultiLiquidate\x1a).nibiru.perp.v2.MsgMultiLiquidateResponse\"\x00\x12W\n\x0bMarketOrder\x12\x1e.nibiru.perp.v2.MsgMarketOrder\x1a&.nibiru.perp.v2.MsgMarketOrderResponse\"\x00\x12]\n\rClosePosition\x12 .nibiru.perp.v2.MsgClosePosition\x1a(.nibiru.perp.v2.MsgClosePositionResponse\"\x00\x12Z\n\x0cPartialClose\x12\x1f.nibiru.perp.v2.MsgPartialClose\x1a\'.nibiru.perp.v2.MsgPartialCloseResponse\"\x00\x12u\n\x15\x44onateToEcosystemFund\x12(.nibiru.perp.v2.MsgDonateToEcosystemFund\x1a\x30.nibiru.perp.v2.MsgDonateToEcosystemFundResponse\"\x00\x42/Z-github.com/NibiruChain/nibiru/x/perp/v2/typesb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nibiru.perp.v2.tx_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z-github.com/NibiruChain/nibiru/x/perp/v2/types'
@@ -77,14 +77,28 @@
   _MSGCLOSEPOSITIONRESPONSE.fields_by_name['exchanged_position_size']._serialized_options = b'\310\336\037\000\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec'
   _MSGCLOSEPOSITIONRESPONSE.fields_by_name['funding_payment']._options = None
   _MSGCLOSEPOSITIONRESPONSE.fields_by_name['funding_payment']._serialized_options = b'\310\336\037\000\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec'
   _MSGCLOSEPOSITIONRESPONSE.fields_by_name['realized_pnl']._options = None
   _MSGCLOSEPOSITIONRESPONSE.fields_by_name['realized_pnl']._serialized_options = b'\310\336\037\000\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec'
   _MSGCLOSEPOSITIONRESPONSE.fields_by_name['margin_to_trader']._options = None
   _MSGCLOSEPOSITIONRESPONSE.fields_by_name['margin_to_trader']._serialized_options = b'\310\336\037\000\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec'
+  _MSGPARTIALCLOSE.fields_by_name['pair']._options = None
+  _MSGPARTIALCLOSE.fields_by_name['pair']._serialized_options = b'\310\336\037\000\332\336\0371github.com/NibiruChain/nibiru/x/common/asset.Pair'
+  _MSGPARTIALCLOSE.fields_by_name['size']._options = None
+  _MSGPARTIALCLOSE.fields_by_name['size']._serialized_options = b'\310\336\037\000\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec'
+  _MSGPARTIALCLOSERESPONSE.fields_by_name['exchanged_notional_value']._options = None
+  _MSGPARTIALCLOSERESPONSE.fields_by_name['exchanged_notional_value']._serialized_options = b'\310\336\037\000\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec'
+  _MSGPARTIALCLOSERESPONSE.fields_by_name['exchanged_position_size']._options = None
+  _MSGPARTIALCLOSERESPONSE.fields_by_name['exchanged_position_size']._serialized_options = b'\310\336\037\000\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec'
+  _MSGPARTIALCLOSERESPONSE.fields_by_name['funding_payment']._options = None
+  _MSGPARTIALCLOSERESPONSE.fields_by_name['funding_payment']._serialized_options = b'\310\336\037\000\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec'
+  _MSGPARTIALCLOSERESPONSE.fields_by_name['realized_pnl']._options = None
+  _MSGPARTIALCLOSERESPONSE.fields_by_name['realized_pnl']._serialized_options = b'\310\336\037\000\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec'
+  _MSGPARTIALCLOSERESPONSE.fields_by_name['margin_to_trader']._options = None
+  _MSGPARTIALCLOSERESPONSE.fields_by_name['margin_to_trader']._serialized_options = b'\310\336\037\000\332\336\037&github.com/cosmos/cosmos-sdk/types.Dec'
   _MSGDONATETOECOSYSTEMFUND.fields_by_name['donation']._options = None
   _MSGDONATETOECOSYSTEMFUND.fields_by_name['donation']._serialized_options = b'\310\336\037\000\362\336\037\017yaml:\"donation\"'
   _MSGREMOVEMARGIN._serialized_start=156
   _MSGREMOVEMARGIN._serialized_end=333
   _MSGREMOVEMARGINRESPONSE._serialized_start=336
   _MSGREMOVEMARGINRESPONSE._serialized_end=568
   _MSGADDMARGIN._serialized_start=571
@@ -103,14 +117,18 @@
   _MSGMARKETORDER._serialized_end=2043
   _MSGMARKETORDERRESPONSE._serialized_start=2046
   _MSGMARKETORDERRESPONSE._serialized_end=2785
   _MSGCLOSEPOSITION._serialized_start=2787
   _MSGCLOSEPOSITION._serialized_end=2908
   _MSGCLOSEPOSITIONRESPONSE._serialized_start=2911
   _MSGCLOSEPOSITIONRESPONSE._serialized_end=3409
-  _MSGDONATETOECOSYSTEMFUND._serialized_start=3412
-  _MSGDONATETOECOSYSTEMFUND._serialized_end=3542
-  _MSGDONATETOECOSYSTEMFUNDRESPONSE._serialized_start=3544
-  _MSGDONATETOECOSYSTEMFUNDRESPONSE._serialized_end=3578
-  _MSG._serialized_start=3581
-  _MSG._serialized_end=4162
+  _MSGPARTIALCLOSE._serialized_start=3412
+  _MSGPARTIALCLOSE._serialized_end=3600
+  _MSGPARTIALCLOSERESPONSE._serialized_start=3603
+  _MSGPARTIALCLOSERESPONSE._serialized_end=4100
+  _MSGDONATETOECOSYSTEMFUND._serialized_start=4103
+  _MSGDONATETOECOSYSTEMFUND._serialized_end=4233
+  _MSGDONATETOECOSYSTEMFUNDRESPONSE._serialized_start=4235
+  _MSGDONATETOECOSYSTEMFUNDRESPONSE._serialized_end=4269
+  _MSG._serialized_start=4272
+  _MSG._serialized_end=4945
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/tx_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -350,14 +350,73 @@
         margin_to_trader: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["exchanged_notional_value", b"exchanged_notional_value", "exchanged_position_size", b"exchanged_position_size", "funding_payment", b"funding_payment", "margin_to_trader", b"margin_to_trader", "realized_pnl", b"realized_pnl"]) -> None: ...
 
 global___MsgClosePositionResponse = MsgClosePositionResponse
 
 @typing_extensions.final
+class MsgPartialClose(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    SENDER_FIELD_NUMBER: builtins.int
+    PAIR_FIELD_NUMBER: builtins.int
+    SIZE_FIELD_NUMBER: builtins.int
+    sender: builtins.str
+    pair: builtins.str
+    size: builtins.str
+    def __init__(
+        self,
+        *,
+        sender: builtins.str = ...,
+        pair: builtins.str = ...,
+        size: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pair", b"pair", "sender", b"sender", "size", b"size"]) -> None: ...
+
+global___MsgPartialClose = MsgPartialClose
+
+@typing_extensions.final
+class MsgPartialCloseResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    EXCHANGED_NOTIONAL_VALUE_FIELD_NUMBER: builtins.int
+    EXCHANGED_POSITION_SIZE_FIELD_NUMBER: builtins.int
+    FUNDING_PAYMENT_FIELD_NUMBER: builtins.int
+    REALIZED_PNL_FIELD_NUMBER: builtins.int
+    MARGIN_TO_TRADER_FIELD_NUMBER: builtins.int
+    exchanged_notional_value: builtins.str
+    """The amount of quote assets exchanged."""
+    exchanged_position_size: builtins.str
+    """The amount of base assets exchanged."""
+    funding_payment: builtins.str
+    """The funding payment applied on this position change, measured in quote
+    units.
+    """
+    realized_pnl: builtins.str
+    """The amount of PnL realized on this position changed, measured in quote
+    units.
+    """
+    margin_to_trader: builtins.str
+    """The amount of margin the trader receives after closing the position, from
+    the vault. Should never be negative.
+    """
+    def __init__(
+        self,
+        *,
+        exchanged_notional_value: builtins.str = ...,
+        exchanged_position_size: builtins.str = ...,
+        funding_payment: builtins.str = ...,
+        realized_pnl: builtins.str = ...,
+        margin_to_trader: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["exchanged_notional_value", b"exchanged_notional_value", "exchanged_position_size", b"exchanged_position_size", "funding_payment", b"funding_payment", "margin_to_trader", b"margin_to_trader", "realized_pnl", b"realized_pnl"]) -> None: ...
+
+global___MsgPartialCloseResponse = MsgPartialCloseResponse
+
+@typing_extensions.final
 class MsgDonateToEcosystemFund(google.protobuf.message.Message):
     """-------------------------- DonateToEcosystemFund --------------------------"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     DONATION_FIELD_NUMBER: builtins.int
```

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/perp/v2/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/perp/v2/tx_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,19 @@
                 response_deserializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgMarketOrderResponse.FromString,
                 )
         self.ClosePosition = channel.unary_unary(
                 '/nibiru.perp.v2.Msg/ClosePosition',
                 request_serializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgClosePosition.SerializeToString,
                 response_deserializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgClosePositionResponse.FromString,
                 )
+        self.PartialClose = channel.unary_unary(
+                '/nibiru.perp.v2.Msg/PartialClose',
+                request_serializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgPartialClose.SerializeToString,
+                response_deserializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgPartialCloseResponse.FromString,
+                )
         self.DonateToEcosystemFund = channel.unary_unary(
                 '/nibiru.perp.v2.Msg/DonateToEcosystemFund',
                 request_serializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgDonateToEcosystemFund.SerializeToString,
                 response_deserializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgDonateToEcosystemFundResponse.FromString,
                 )
 
 
@@ -77,14 +82,20 @@
 
     def ClosePosition(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def PartialClose(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def DonateToEcosystemFund(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
@@ -111,14 +122,19 @@
                     response_serializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgMarketOrderResponse.SerializeToString,
             ),
             'ClosePosition': grpc.unary_unary_rpc_method_handler(
                     servicer.ClosePosition,
                     request_deserializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgClosePosition.FromString,
                     response_serializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgClosePositionResponse.SerializeToString,
             ),
+            'PartialClose': grpc.unary_unary_rpc_method_handler(
+                    servicer.PartialClose,
+                    request_deserializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgPartialClose.FromString,
+                    response_serializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgPartialCloseResponse.SerializeToString,
+            ),
             'DonateToEcosystemFund': grpc.unary_unary_rpc_method_handler(
                     servicer.DonateToEcosystemFund,
                     request_deserializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgDonateToEcosystemFund.FromString,
                     response_serializer=nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgDonateToEcosystemFundResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -213,14 +229,31 @@
         return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v2.Msg/ClosePosition',
             nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgClosePosition.SerializeToString,
             nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgClosePositionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def PartialClose(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/nibiru.perp.v2.Msg/PartialClose',
+            nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgPartialClose.SerializeToString,
+            nibiru_dot_perp_dot_v2_dot_tx__pb2.MsgPartialCloseResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def DonateToEcosystemFund(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/event_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/event_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/params_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/params_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/pool_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/pool_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/pool_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/pool_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/spot/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/spot/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/events_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/events_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/events_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/genesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/params_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/params_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/stablecoin/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/stablecoin/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/event_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/event_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/query_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/query_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/query_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/state_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/state_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/state_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/tx_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/tx_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/tx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/nibiru/sudo/v1/tx_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/nibiru/sudo/v1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/abci/types_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/abci/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/abci/types_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/abci/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/abci/types_pb2_grpc.py` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/abci/types_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/keys_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/crypto/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/keys_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/crypto/keys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/proof_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/crypto/proof_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/crypto/proof_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/crypto/proof_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/libs/bits/types_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/libs/bits/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/libs/bits/types_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/libs/bits/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/p2p/types_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/p2p/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/p2p/types_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/p2p/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/block_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/block_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/block_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/evidence_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/evidence_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/evidence_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/evidence_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/params_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/params_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/params_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/params_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/types_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/types_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/validator_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/types/validator_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/types/validator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/version/types_pb2.py` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/version/types_pb2.py`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/nibiru_proto/tendermint/version/types_pb2.pyi` & `nibiru_proto-0.21.7b1/nibiru_proto/tendermint/version/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nibiru_proto-0.21.3b7/pyproject.toml` & `nibiru_proto-0.21.7b1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tool.poetry]
 name = "nibiru-proto"
-version = "0.21.3b7"
+version = "0.21.7b1" 
+# nibiru commit: https://github.com/NibiruChain/nibiru/commit/27c75034a74e37adfc438c5cbc90588101d875c8
 description = "Nibiru Chain Python SDK"
 authors = ["Nibiru Chain <dev@nibiru.fi>"]
 packages = [{ include = "nibiru_proto" }]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nibiru_proto-0.21.3b7/PKG-INFO` & `nibiru_proto-0.21.7b1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibiru-proto
-Version: 0.21.3b7
+Version: 0.21.7b1
 Summary: Nibiru Chain Python SDK
 License: MIT
 Author: Nibiru Chain
 Author-email: dev@nibiru.fi
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

