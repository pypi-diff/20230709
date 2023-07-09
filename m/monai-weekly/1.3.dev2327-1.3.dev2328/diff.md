# Comparing `tmp/monai-weekly-1.3.dev2327.tar.gz` & `tmp/monai-weekly-1.3.dev2328.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai-weekly-1.3.dev2327.tar", last modified: Sun Jul  2 02:35:31 2023, max compression
+gzip compressed data, was "monai-weekly-1.3.dev2328.tar", last modified: Sun Jul  9 02:36:18 2023, max compression
```

## Comparing `monai-weekly-1.3.dev2327.tar` & `monai-weekly-1.3.dev2328.tar`

### file list

```diff
@@ -1,1146 +1,1146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:31.144650 monai-weekly-1.3.dev2327/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-02 02:35:31.144650 monai-weekly-1.3.dev2327/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:31.144650 monai-weekly-1.3.dev2327/monai/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-02 02:33:37.000000 monai-weekly-1.3.dev2327/monai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.536646 monai-weekly-1.3.dev2327/monai/_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.540646 monai-weekly-1.3.dev2327/monai/_extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/_extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/_extensions/gmm/gmm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/_extensions/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-02 02:35:31.144650 monai-weekly-1.3.dev2327/monai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.540646 monai-weekly-1.3.dev2327/monai/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.548646 monai-weekly-1.3.dev2327/monai/apps/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/auto3dseg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37150 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/auto3dseg/auto_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    26038 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27776 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/auto3dseg/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/auto3dseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.552646 monai-weekly-1.3.dev2327/monai/apps/deepedit/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/deepedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/deepedit/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/deepedit/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.556646 monai-weekly-1.3.dev2327/monai/apps/deepgrow/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/deepgrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/deepgrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/deepgrow/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/deepgrow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.556646 monai-weekly-1.3.dev2327/monai/apps/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.560646 monai-weekly-1.3.dev2327/monai/apps/detection/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/metrics/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/metrics/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.560646 monai-weekly-1.3.dev2327/monai/apps/detection/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53640 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/networks/retinanet_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.564646 monai-weekly-1.3.dev2327/monai/apps/detection/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    18051 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/transforms/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    69282 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.572646 monai-weekly-1.3.dev2327/monai/apps/detection/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/utils/anchor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/utils/box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/utils/box_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/utils/detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/detection/utils/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.576646 monai-weekly-1.3.dev2327/monai/apps/mmars/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/mmars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/mmars/mmars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/mmars/model_desc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.576646 monai-weekly-1.3.dev2327/monai/apps/nnunet/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/nnunet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/nnunet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48597 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/nnunet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.580646 monai-weekly-1.3.dev2327/monai/apps/nuclick/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/nuclick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/nuclick/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.580646 monai-weekly-1.3.dev2327/monai/apps/pathology/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.584646 monai-weekly-1.3.dev2327/monai/apps/pathology/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/engines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.584646 monai-weekly-1.3.dev2327/monai/apps/pathology/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/handlers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.584646 monai-weekly-1.3.dev2327/monai/apps/pathology/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/inferers/inferer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.588647 monai-weekly-1.3.dev2327/monai/apps/pathology/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/losses/hovernet_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.588647 monai-weekly-1.3.dev2327/monai/apps/pathology/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/metrics/lesion_froc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.592646 monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.596646 monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37306 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.596646 monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/stain/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/stain/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/pathology/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.600647 monai-weekly-1.3.dev2327/monai/apps/reconstruction/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/mri_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.600647 monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.600647 monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/blocks/varnetblock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.604647 monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/nets/varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.604647 monai-weekly-1.3.dev2327/monai/apps/reconstruction/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/reconstruction/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.604647 monai-weekly-1.3.dev2327/monai/apps/tcia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/tcia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/tcia/label_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/tcia/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.608646 monai-weekly-1.3.dev2327/monai/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/auto3dseg/algo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/auto3dseg/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/auto3dseg/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/auto3dseg/seg_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/auto3dseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.616647 monai-weekly-1.3.dev2327/monai/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/bundle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/bundle/config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/bundle/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/bundle/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/bundle/reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    64632 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/bundle/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/bundle/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/bundle/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.616647 monai-weekly-1.3.dev2327/monai/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/config/deviceconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/config/type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.636647 monai-weekly-1.3.dev2327/monai/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    68912 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/image_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/meta_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    27511 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/test_time_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65554 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/wsi_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49494 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/data/wsi_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.640647 monai-weekly-1.3.dev2327/monai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/engines/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/engines/multi_gpu_supervised_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/engines/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/engines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/engines/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.640647 monai-weekly-1.3.dev2327/monai/fl/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/fl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.640647 monai-weekly-1.3.dev2327/monai/fl/client/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/fl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/fl/client/client_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/fl/client/monai_algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.644647 monai-weekly-1.3.dev2327/monai/fl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/fl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/fl/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/fl/utils/exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/fl/utils/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.656647 monai-weekly-1.3.dev2327/monai/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/clearml_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/earlystop_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/logfile_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/lr_schedule_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/metrics_reloaded_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/nvtx_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/probability_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/smartcache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/stats_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/tensorboard_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/handlers/validation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.660647 monai-weekly-1.3.dev2327/monai/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/inferers/inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/inferers/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/inferers/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/inferers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.668647 monai-weekly-1.3.dev2327/monai/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/deform.py
--rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/image_dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/spatial_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/tversky.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/losses/unified_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.680647 monai-weekly-1.3.dev2327/monai/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/active_learning_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/f_beta_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/metrics/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.680647 monai-weekly-1.3.dev2327/monai/networks/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.692647 monai-weekly-1.3.dev2327/monai/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/acti_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/crf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/dints_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/fft_utils_t.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/blocks/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.700647 monai-weekly-1.3.dev2327/monai/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/layers/convutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/layers/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/layers/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/layers/gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/layers/simplelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/layers/spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/layers/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.720647 monai-weekly-1.3.dev2327/monai/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/daf3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/dints.py
--rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40667 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/netadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/quicknat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/torchvision_fc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/nets/vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    47132 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.720647 monai-weekly-1.3.dev2327/monai/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/optimizers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/optimizers/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/optimizers/novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/optimizers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.732647 monai-weekly-1.3.dev2327/monai/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    37090 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.736647 monai-weekly-1.3.dev2327/monai/transforms/croppad/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/croppad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    74891 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/croppad/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/croppad/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    60872 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/croppad/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/croppad/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.740647 monai-weekly-1.3.dev2327/monai/transforms/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   107785 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/intensity/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/intensity/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    18233 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/inverse_batch_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.744647 monai-weekly-1.3.dev2327/monai/transforms/io/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25374 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/io/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/io/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.748647 monai-weekly-1.3.dev2327/monai/transforms/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/lazy/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/lazy/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/lazy/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/lazy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.748647 monai-weekly-1.3.dev2327/monai/transforms/meta_utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/meta_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/meta_utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/nvtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.752647 monai-weekly-1.3.dev2327/monai/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40802 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.752647 monai-weekly-1.3.dev2327/monai/transforms/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/signal/array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.752647 monai-weekly-1.3.dev2327/monai/transforms/smooth_field/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/smooth_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/smooth_field/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/smooth_field/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.756647 monai-weekly-1.3.dev2327/monai/transforms/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   178796 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/spatial/array.py
--rw-r--r--   0 runner    (1001) docker     (123)   127396 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/spatial/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/spatial/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.760647 monai-weekly-1.3.dev2327/monai/transforms/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70963 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/utility/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    76161 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    81124 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/utils_create_transform_ims.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/transforms/utils_pytorch_numpy_unification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.768648 monai-weekly-1.3.dev2327/monai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/deprecate_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/jupyter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29296 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/utils/type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.776648 monai-weekly-1.3.dev2327/monai/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/visualize/class_activation_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/visualize/gradient_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/visualize/img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/visualize/occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/visualize/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/monai/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:30.776648 monai-weekly-1.3.dev2327/monai_weekly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-02 02:35:30.000000 monai-weekly-1.3.dev2327/monai_weekly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34314 2023-07-02 02:35:30.000000 monai-weekly-1.3.dev2327/monai_weekly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:35:30.000000 monai-weekly-1.3.dev2327/monai_weekly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:35:30.000000 monai-weekly-1.3.dev2327/monai_weekly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-02 02:35:30.000000 monai-weekly-1.3.dev2327/monai_weekly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 02:35:30.000000 monai-weekly-1.3.dev2327/monai_weekly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-02 02:35:31.144650 monai-weekly-1.3.dev2327/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:35:31.144650 monai-weekly-1.3.dev2327/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_acn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_activationsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_add_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_add_coordinate_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_add_coordinate_channelsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_add_extreme_points_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_add_extreme_points_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_adn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_affine_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_anchor_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_apply_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_arraydataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_as_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_as_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_as_channel_last.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_as_channel_lastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_as_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_as_discreted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_atss_box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_auto3dseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_auto3dseg_bundlegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_auto3dseg_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_auto3dseg_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bending_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bilateral_approx_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bilateral_approx_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bilateral_precise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_blend_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_border_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_border_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bounding_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bounding_rectd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_box_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bundle_ckpt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bundle_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bundle_get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bundle_init_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bundle_onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bundle_trt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bundle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bundle_verify_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bundle_verify_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_bundle_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cachedataset_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cachedataset_persistent_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cachentransdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_call_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cast_to_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_center_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_center_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_center_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_center_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_channel_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_check_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_check_missing_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_classes_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_component_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25175 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compose_get_number_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compute_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compute_f_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compute_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compute_generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compute_ho_ver_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compute_ho_ver_maps_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compute_meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compute_meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compute_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compute_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compute_roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_compute_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_concat_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_contrastive_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_convert_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_convert_to_multi_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_convert_to_multi_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_convert_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_convert_to_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_convert_to_trt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_copy_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_copy_model_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_correct_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_create_cross_validation_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_create_grid_and_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_crf_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_crf_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_crop_foreground.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_crop_foregroundd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_csv_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cumulative_average_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_cv2_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_daf3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_data_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dataset_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_decathlondataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_decollate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_deepedit_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_deepedit_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_deepgrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_deepgrow_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_deepgrow_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_delete_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_detect_envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_detection_coco_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_detector_boxselector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dev_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dice_ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dints_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dints_mixop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dints_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_divisible_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_divisible_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_download_and_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_download_url_yandex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_downsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dvf2ddf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_ensure_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_ensure_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_ensure_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_ensure_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_ensure_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_enum_bound_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_eval_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_evenly_divisible_all_gather_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_factorized_increase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_factorized_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fg_bg_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fg_bg_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_file_basename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fill_holes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fill_holesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fl_exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fl_monai_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fl_monai_algo_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fl_monai_algo_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_flatten_sub_keysd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_foreground_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_foreground_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fpn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_from_engine_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_gaussian_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generalized_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generalized_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generalized_wasserstein_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_distance_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_distance_mapd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_instance_border.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_instance_borderd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_instance_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_instance_centroidd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_instance_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_instance_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_instance_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_label_classes_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_param_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_pos_neg_label_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_spatial_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_succinct_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_succinct_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_watershed_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_watershed_markersd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_watershed_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generate_watershed_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_get_equivalent_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_get_extreme_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_get_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_get_package_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_get_unique_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_global_mutual_information_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_globalnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_grid_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_grid_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_grid_splitd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_classification_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_clearml_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_clearml_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_confusion_matrix_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_early_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_logfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_metrics_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_prob_map_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_regression_metrics_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_rocauc_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_smartcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_tb_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_tb_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_hardnegsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_header_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_hilbert_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_histogram_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_histogram_normalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_hovernet_instance_map_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_hovernet_instance_map_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_hovernet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_hovernet_nuclear_type_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_hovernet_nuclear_type_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_identityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_image_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_image_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_init_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_autorunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_bundle_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_classification_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_fast_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_gpu_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_lazy_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_integration_workflows_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_intensity_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_intensity_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18993 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_inverse_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_inverse_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_invert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_invertd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_is_supported_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_itk_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_keep_largest_connected_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_keep_largest_connected_componentd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_kspace_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_label_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_label_filterd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_label_quality_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_label_to_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_label_to_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_label_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_label_to_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_lesion_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_list_data_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_list_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_lltm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_lmdbdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_lmdbdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_load_decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_load_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_load_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_load_spacing_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_loader_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_local_normalized_cross_correlation_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_localnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_look_up_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_make_nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_map_binary_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_map_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_map_label_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_map_label_valued.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_mask_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_mask_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_masked_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_masked_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_masked_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_matshow3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_mean_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_median_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_median_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_median_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_mednistdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_meta_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23538 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_metatensor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_mmar_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_module_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_monai_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_monai_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_mri_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_net_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_network_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_nifti_endianness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_nifti_header_revise.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_nifti_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_normalize_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_npzdictitemdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_nrrd_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_nuclick_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_nvtx_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_nvtx_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_one_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_optim_novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_optional_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_ori_ras_lps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_orientationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_p3d_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_pad_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_pad_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_parallel_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_parallel_execution_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_partition_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_partition_dataset_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_patch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_patch_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_pathology_he_stain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_pathology_he_stain_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_pathology_prob_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_persistentdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_persistentdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_phl_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_phl_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_pil_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_plot_2d_or_3d_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_png_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_polyval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_prepare_batch_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_prepare_batch_default_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_prepare_batch_extra_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_prepare_batch_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_preset_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_print_transform_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_probnms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_probnmsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_pytorch_version_after.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_query_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_quicknat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_axis_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_axis_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_bias_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_bias_fieldd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_coarse_dropoutd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_coarse_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_coarse_shuffled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_crop_by_label_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_crop_by_label_classesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_crop_by_pos_neg_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_crop_by_pos_neg_labeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_deform_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_elastic_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_elastic_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_elasticd_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_elasticd_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_gaussian_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_histogram_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_histogram_shiftd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_rician_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_rician_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_scale_intensity_fixed_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_scale_intensity_fixed_meand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_spatial_crop_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_spatial_crop_samplesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_weighted_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_weighted_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rand_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_randidentity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_random_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_randomizable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_randomizable_transform_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_randtorchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rankfilter_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_recon_net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_reference_based_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_reference_based_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_reg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_remove_repeated_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_remove_repeated_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_remove_small_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_repeat_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_repeat_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_replace_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_require_pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_resample_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_resample_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_resample_to_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_resample_to_matchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_resize_with_pad_or_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_resize_with_pad_or_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_resized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_retinanet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_retinanet_predict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_safe_dtype_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_saliency_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_sample_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_save_classificationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_save_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_save_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_savitzky_golay_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_savitzky_golay_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_scale_intensity_fixed_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_scale_intensity_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_scale_intensity_range_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_scale_intensity_range_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_scale_intensity_ranged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_se_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_se_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_seg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_select_cross_validation_folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_select_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_senet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_separable_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_set_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_set_visible_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_shuffle_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_signal_continuouswavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_signal_fillempty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_signal_rand_add_gaussiannoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_signal_rand_add_sine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_signal_rand_add_sine_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_signal_rand_add_squarepulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_signal_rand_add_squarepulse_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_signal_rand_drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_signal_rand_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_signal_rand_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_signal_remove_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_simple_aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_simulatedelay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_simulatedelayd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_skip_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_slice_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_sliding_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_sliding_window_hovernet_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_sliding_window_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_smartcachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_smooth_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_sobel_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_sobel_gradientd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_some_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_spacingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_spatial_combine_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_spatial_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_spatial_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_spatial_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_spatial_resampled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_split_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_split_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_splitdim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_splitdimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_squeezedim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_squeezedimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_ssim_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_str2bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_str2list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_subpixel_upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    21649 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_tciadataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_testtimeaugmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_text_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_threadcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_threshold_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_threshold_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_timedcall_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_cupy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_cupyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_deviced.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_from_meta_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_numpyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_onehot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_pild.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_to_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_torchvision_fc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_torchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_traceable_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_train_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_trainable_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_trainable_joint_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_transposed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_unified_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_upsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_utils_pytorch_numpy_unification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_varnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_version_leq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_video_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_vis_cam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_vis_gradbased.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_vis_gradcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_vote_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_vote_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_warp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_watershed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_watershedd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_weighted_random_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_with_allow_missing_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_write_metrics_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_wsi_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_wsireader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_zarr_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_zipdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_zoom_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/tests/test_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-07-02 02:33:34.000000 monai-weekly-1.3.dev2327/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.689433 monai-weekly-1.3.dev2328/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-09 02:36:18.689433 monai-weekly-1.3.dev2328/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.689433 monai-weekly-1.3.dev2328/monai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-09 02:34:23.000000 monai-weekly-1.3.dev2328/monai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.297432 monai-weekly-1.3.dev2328/monai/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.297432 monai-weekly-1.3.dev2328/monai/_extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/_extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/_extensions/gmm/gmm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/_extensions/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-09 02:36:18.689433 monai-weekly-1.3.dev2328/monai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.297432 monai-weekly-1.3.dev2328/monai/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.301432 monai-weekly-1.3.dev2328/monai/apps/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/auto3dseg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37154 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26181 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27522 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/auto3dseg/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/auto3dseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.301432 monai-weekly-1.3.dev2328/monai/apps/deepedit/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/deepedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/deepedit/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/deepedit/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.305432 monai-weekly-1.3.dev2328/monai/apps/deepgrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/deepgrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/deepgrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/deepgrow/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/deepgrow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.305432 monai-weekly-1.3.dev2328/monai/apps/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.305432 monai-weekly-1.3.dev2328/monai/apps/detection/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/metrics/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/metrics/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.309432 monai-weekly-1.3.dev2328/monai/apps/detection/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53640 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/networks/retinanet_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.309432 monai-weekly-1.3.dev2328/monai/apps/detection/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18051 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/transforms/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69282 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.313432 monai-weekly-1.3.dev2328/monai/apps/detection/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/utils/box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/utils/box_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/utils/detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/detection/utils/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.313432 monai-weekly-1.3.dev2328/monai/apps/mmars/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/mmars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/mmars/mmars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/mmars/model_desc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.313432 monai-weekly-1.3.dev2328/monai/apps/nnunet/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/nnunet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/nnunet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48577 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/nnunet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.317432 monai-weekly-1.3.dev2328/monai/apps/nuclick/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/nuclick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/nuclick/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.317432 monai-weekly-1.3.dev2328/monai/apps/pathology/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.317432 monai-weekly-1.3.dev2328/monai/apps/pathology/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/engines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.317432 monai-weekly-1.3.dev2328/monai/apps/pathology/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/handlers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.317432 monai-weekly-1.3.dev2328/monai/apps/pathology/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/inferers/inferer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.317432 monai-weekly-1.3.dev2328/monai/apps/pathology/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/losses/hovernet_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.321432 monai-weekly-1.3.dev2328/monai/apps/pathology/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/metrics/lesion_froc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.321432 monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.321432 monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37306 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.321432 monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/stain/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/pathology/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.325432 monai-weekly-1.3.dev2328/monai/apps/reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/mri_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.325432 monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.325432 monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/blocks/varnetblock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.325432 monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/nets/varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.325432 monai-weekly-1.3.dev2328/monai/apps/reconstruction/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/reconstruction/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.329432 monai-weekly-1.3.dev2328/monai/apps/tcia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/tcia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/tcia/label_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/tcia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.329432 monai-weekly-1.3.dev2328/monai/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/auto3dseg/algo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/auto3dseg/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/auto3dseg/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/auto3dseg/seg_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/auto3dseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.333432 monai-weekly-1.3.dev2328/monai/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/bundle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/bundle/config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/bundle/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/bundle/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/bundle/reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64632 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/bundle/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/bundle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/bundle/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.333432 monai-weekly-1.3.dev2328/monai/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/config/deviceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/config/type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.345432 monai-weekly-1.3.dev2328/monai/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68912 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/image_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/meta_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27511 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/test_time_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65554 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/wsi_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49494 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/data/wsi_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.349432 monai-weekly-1.3.dev2328/monai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/engines/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/engines/multi_gpu_supervised_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/engines/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/engines/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.349432 monai-weekly-1.3.dev2328/monai/fl/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/fl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.349432 monai-weekly-1.3.dev2328/monai/fl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/fl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/fl/client/client_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/fl/client/monai_algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.349432 monai-weekly-1.3.dev2328/monai/fl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/fl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/fl/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/fl/utils/exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/fl/utils/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.361432 monai-weekly-1.3.dev2328/monai/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/clearml_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/earlystop_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/logfile_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/lr_schedule_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/nvtx_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/probability_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/smartcache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/stats_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/tensorboard_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/handlers/validation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.361432 monai-weekly-1.3.dev2328/monai/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/inferers/inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/inferers/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/inferers/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/inferers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.365432 monai-weekly-1.3.dev2328/monai/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/deform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/image_dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/spatial_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/tversky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/losses/unified_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.373432 monai-weekly-1.3.dev2328/monai/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/active_learning_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/f_beta_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42254 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/metrics/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.373432 monai-weekly-1.3.dev2328/monai/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.381432 monai-weekly-1.3.dev2328/monai/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/acti_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/crf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/dints_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/fft_utils_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/blocks/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.385432 monai-weekly-1.3.dev2328/monai/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/layers/convutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/layers/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/layers/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/layers/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/layers/simplelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/layers/spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/layers/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.397432 monai-weekly-1.3.dev2328/monai/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/daf3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/dints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40667 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/netadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/quicknat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/torchvision_fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/nets/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47132 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.401433 monai-weekly-1.3.dev2328/monai/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/optimizers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/optimizers/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/optimizers/novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/optimizers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.405433 monai-weekly-1.3.dev2328/monai/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37090 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.405433 monai-weekly-1.3.dev2328/monai/transforms/croppad/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/croppad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74980 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/croppad/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/croppad/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60975 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/croppad/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/croppad/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.409433 monai-weekly-1.3.dev2328/monai/transforms/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107785 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/intensity/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/intensity/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18233 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/inverse_batch_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.409433 monai-weekly-1.3.dev2328/monai/transforms/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25374 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/io/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/io/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.413432 monai-weekly-1.3.dev2328/monai/transforms/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/lazy/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/lazy/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/lazy/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/lazy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.413432 monai-weekly-1.3.dev2328/monai/transforms/meta_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/meta_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/meta_utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/nvtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.413432 monai-weekly-1.3.dev2328/monai/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40802 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.413432 monai-weekly-1.3.dev2328/monai/transforms/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/signal/array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.417433 monai-weekly-1.3.dev2328/monai/transforms/smooth_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/smooth_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/smooth_field/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/smooth_field/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.417433 monai-weekly-1.3.dev2328/monai/transforms/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   178796 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/spatial/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127396 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/spatial/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/spatial/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.421433 monai-weekly-1.3.dev2328/monai/transforms/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70963 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/utility/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76161 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81188 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/utils_create_transform_ims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/transforms/utils_pytorch_numpy_unification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.425433 monai-weekly-1.3.dev2328/monai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/deprecate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/jupyter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29430 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/utils/type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.429432 monai-weekly-1.3.dev2328/monai/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/visualize/class_activation_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/visualize/gradient_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/visualize/img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/visualize/occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/visualize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/monai/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.429432 monai-weekly-1.3.dev2328/monai_weekly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-09 02:36:18.000000 monai-weekly-1.3.dev2328/monai_weekly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34314 2023-07-09 02:36:18.000000 monai-weekly-1.3.dev2328/monai_weekly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 02:36:18.000000 monai-weekly-1.3.dev2328/monai_weekly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 02:36:18.000000 monai-weekly-1.3.dev2328/monai_weekly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-09 02:36:18.000000 monai-weekly-1.3.dev2328/monai_weekly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-09 02:36:18.000000 monai-weekly-1.3.dev2328/monai_weekly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-09 02:36:18.689433 monai-weekly-1.3.dev2328/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:36:18.689433 monai-weekly-1.3.dev2328/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_acn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_activationsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_add_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_add_coordinate_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_add_coordinate_channelsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_add_extreme_points_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_add_extreme_points_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_adn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_affine_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_anchor_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_apply_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_arraydataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_as_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_as_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_as_channel_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_as_channel_lastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_as_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_as_discreted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_atss_box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_auto3dseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_auto3dseg_bundlegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_auto3dseg_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_auto3dseg_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bending_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bilateral_approx_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bilateral_approx_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bilateral_precise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_blend_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_border_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_border_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bounding_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bounding_rectd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_box_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bundle_ckpt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bundle_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bundle_get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bundle_init_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bundle_onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bundle_trt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bundle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bundle_verify_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bundle_verify_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_bundle_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cachedataset_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cachedataset_persistent_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cachentransdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_call_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cast_to_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_center_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_center_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_center_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_center_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_channel_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_check_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_check_missing_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_classes_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_component_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25175 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compose_get_number_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compute_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compute_f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compute_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compute_generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compute_ho_ver_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compute_ho_ver_maps_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compute_meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compute_meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compute_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compute_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compute_roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_compute_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_concat_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_contrastive_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_convert_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_convert_to_multi_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_convert_to_multi_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_convert_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_convert_to_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_convert_to_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_copy_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_copy_model_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_correct_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_create_cross_validation_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_create_grid_and_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_crf_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_crf_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_crop_foreground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_crop_foregroundd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_csv_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cumulative_average_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_cv2_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_daf3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_data_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dataset_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_decathlondataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_decollate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_deepedit_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_deepedit_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_deepgrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_deepgrow_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_deepgrow_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_delete_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_detect_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_detection_coco_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_detector_boxselector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dev_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dice_ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dints_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dints_mixop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dints_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_divisible_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_divisible_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_download_and_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_download_url_yandex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_downsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dvf2ddf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_ensure_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_ensure_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_ensure_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_ensure_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_ensure_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_enum_bound_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_eval_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_evenly_divisible_all_gather_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_factorized_increase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_factorized_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fg_bg_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fg_bg_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_file_basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fill_holes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fill_holesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fl_exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fl_monai_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fl_monai_algo_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fl_monai_algo_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_flatten_sub_keysd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_foreground_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_foreground_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fpn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_from_engine_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_gaussian_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generalized_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generalized_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generalized_wasserstein_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_distance_mapd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_instance_border.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_instance_borderd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_instance_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_instance_centroidd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_instance_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_instance_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_instance_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_label_classes_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_param_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_pos_neg_label_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_spatial_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_succinct_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_succinct_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_watershed_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_watershed_markersd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_watershed_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generate_watershed_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_get_equivalent_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_get_extreme_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_get_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_get_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_get_unique_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_global_mutual_information_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_globalnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_grid_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_grid_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_grid_splitd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_classification_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_clearml_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_clearml_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_confusion_matrix_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_early_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_metrics_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_prob_map_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_regression_metrics_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_rocauc_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_smartcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_tb_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_tb_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_hardnegsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_header_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_hilbert_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_histogram_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_histogram_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_hovernet_instance_map_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_hovernet_instance_map_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_hovernet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_hovernet_nuclear_type_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_hovernet_nuclear_type_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_identityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_image_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_image_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_init_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_autorunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_bundle_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_classification_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_fast_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_gpu_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_lazy_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_sliding_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_integration_workflows_gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_intensity_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_intensity_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18993 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_inverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_inverse_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_invert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_invertd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_is_supported_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_itk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_keep_largest_connected_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_keep_largest_connected_componentd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_kspace_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_label_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_label_filterd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_label_quality_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_label_to_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_label_to_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_label_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_label_to_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_lesion_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_list_data_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_list_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_lltm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_lmdbdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_lmdbdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_load_decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_load_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_load_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_load_spacing_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_loader_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_local_normalized_cross_correlation_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_localnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_look_up_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_make_nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_map_binary_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_map_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_map_label_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_map_label_valued.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_mask_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_mask_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_masked_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_masked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_masked_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_matshow3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_mean_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_median_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_median_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_mednistdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_meta_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23538 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_metatensor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_mmar_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_monai_env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_monai_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_mri_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_net_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_network_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_nifti_endianness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_nifti_header_revise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_nifti_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_normalize_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_npzdictitemdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_nrrd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_nuclick_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_nvtx_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_nvtx_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_optim_novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_optional_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_ori_ras_lps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_orientationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_p3d_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_pad_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_pad_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_parallel_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_parallel_execution_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_partition_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_partition_dataset_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_patch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_patch_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_pathology_he_stain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_pathology_he_stain_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_pathology_prob_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_persistentdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_persistentdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_phl_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_phl_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_pil_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_plot_2d_or_3d_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_png_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_polyval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_prepare_batch_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_prepare_batch_default_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_prepare_batch_extra_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_prepare_batch_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_preset_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_print_transform_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_probnms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_probnmsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_pytorch_version_after.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_query_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_quicknat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_axis_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_axis_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_bias_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_bias_fieldd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_coarse_dropoutd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_coarse_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_coarse_shuffled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_crop_by_label_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_crop_by_label_classesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_crop_by_pos_neg_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_crop_by_pos_neg_labeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_deform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_elastic_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_elastic_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_elasticd_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_elasticd_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_gaussian_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_histogram_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_histogram_shiftd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_rician_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_rician_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_scale_intensity_fixed_meand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_spatial_crop_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_spatial_crop_samplesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_weighted_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_weighted_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rand_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_randidentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_random_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_randomizable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_randomizable_transform_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_randtorchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rankfilter_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_recon_net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_reference_based_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_reference_based_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_reg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_remove_repeated_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_remove_repeated_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_remove_small_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_repeat_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_repeat_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_replace_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_require_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_resample_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_resample_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_resample_to_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_resample_to_matchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_resize_with_pad_or_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_resize_with_pad_or_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_resized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_retinanet_predict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_safe_dtype_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_saliency_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_sample_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_save_classificationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_save_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_save_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_savitzky_golay_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_savitzky_golay_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_scale_intensity_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_scale_intensity_range_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_scale_intensity_range_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_scale_intensity_ranged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_se_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_se_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_seg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_select_cross_validation_folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_select_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_separable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_set_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_set_visible_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_shuffle_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_signal_continuouswavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_signal_fillempty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_signal_rand_add_gaussiannoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_signal_rand_add_sine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_signal_rand_add_sine_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_signal_rand_add_squarepulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_signal_rand_add_squarepulse_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_signal_rand_drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_signal_rand_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_signal_rand_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_signal_remove_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_simple_aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_simulatedelay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_simulatedelayd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_skip_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_slice_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_sliding_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_sliding_window_hovernet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_sliding_window_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_smartcachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_smooth_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_sobel_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_sobel_gradientd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_some_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_spacingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_spatial_combine_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_spatial_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_spatial_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_spatial_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_spatial_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_split_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_split_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_splitdim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_splitdimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_squeezedim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_squeezedimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_ssim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_str2bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_str2list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_subpixel_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_tciadataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_testtimeaugmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_text_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_threadcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_threshold_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_threshold_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_timedcall_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_cupyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_deviced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_from_meta_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_numpyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_onehot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_pild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_to_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_torchvision_fc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_torchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_traceable_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_train_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_trainable_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_trainable_joint_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_transposed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_unified_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_upsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_utils_pytorch_numpy_unification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_varnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_version_leq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_video_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_vis_cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_vis_gradbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_vis_gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_vote_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_vote_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_watershed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_watershedd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_weighted_random_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_with_allow_missing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_write_metrics_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_wsi_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_wsireader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_zarr_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_zipdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_zoom_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/tests/test_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-07-09 02:34:18.000000 monai-weekly-1.3.dev2328/versioneer.py
```

### Comparing `monai-weekly-1.3.dev2327/LICENSE` & `monai-weekly-1.3.dev2328/LICENSE`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/PKG-INFO` & `monai-weekly-1.3.dev2328/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.3.dev2327
+Version: 1.3.dev2328
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai-weekly-1.3.dev2327/README.md` & `monai-weekly-1.3.dev2328/README.md`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/__init__.py` & `monai-weekly-1.3.dev2328/monai/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,8 +74,8 @@
     "metrics",
     "networks",
     "optimizers",
     "transforms",
     "utils",
     "visualize",
 ]
-__commit_id__ = "e7fb74f32b5371bb54bff7a47447df31d06d8edf"
+__commit_id__ = "6f8e63f6cb2932492610515cd9b62f581fcb6d3e"
```

### Comparing `monai-weekly-1.3.dev2327/monai/_extensions/__init__.py` & `monai-weekly-1.3.dev2328/monai/_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/_extensions/gmm/gmm.cpp` & `monai-weekly-1.3.dev2328/monai/_extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/_extensions/gmm/gmm.h` & `monai-weekly-1.3.dev2328/monai/_extensions/gmm/gmm.h`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/_extensions/gmm/gmm_cpu.cpp` & `monai-weekly-1.3.dev2328/monai/_extensions/gmm/gmm_cpu.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/_extensions/gmm/gmm_cuda.cu` & `monai-weekly-1.3.dev2328/monai/_extensions/gmm/gmm_cuda.cu`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/_extensions/gmm/gmm_cuda_linalg.cuh` & `monai-weekly-1.3.dev2328/monai/_extensions/gmm/gmm_cuda_linalg.cuh`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/_extensions/loader.py` & `monai-weekly-1.3.dev2328/monai/_extensions/loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/auto3dseg/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/auto3dseg/__main__.py` & `monai-weekly-1.3.dev2328/monai/apps/auto3dseg/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/auto3dseg/auto_runner.py` & `monai-weekly-1.3.dev2328/monai/apps/auto3dseg/auto_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,15 +521,15 @@
         self.device_setting["NUM_NODES"] = num_nodes
 
         if mn_start_method is None:
             mn_start_method = os.environ.get("MN_START_METHOD", "bcprun")
         self.device_setting["MN_START_METHOD"] = mn_start_method
 
         if cmd_prefix is None:
-            cmd_prefix = os.environ.get("CMD_PREFIX")
+            cmd_prefix = os.environ.get("CMD_PREFIX", "")
         self.device_setting["CMD_PREFIX"] = cmd_prefix
 
         if cmd_prefix is not None:
             logger.info(f"Using user defined command running prefix {cmd_prefix}, will override other settings")
 
     def set_ensemble_method(self, ensemble_method_name: str = "AlgoEnsembleBestByFold", **kwargs: Any) -> None:
         """
```

### Comparing `monai-weekly-1.3.dev2327/monai/apps/auto3dseg/bundle_gen.py` & `monai-weekly-1.3.dev2328/monai/apps/auto3dseg/bundle_gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,35 +9,42 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import importlib
 import os
+import re
 import shutil
 import subprocess
 import sys
 import time
 import warnings
-from collections.abc import Mapping
 from copy import deepcopy
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any
 from urllib.parse import urlparse
 
 import torch
 
 from monai.apps import download_and_extract
 from monai.apps.utils import get_logger
 from monai.auto3dseg.algo_gen import Algo, AlgoGen
-from monai.auto3dseg.utils import algo_to_pickle
+from monai.auto3dseg.utils import (
+    _prepare_cmd_bcprun,
+    _prepare_cmd_default,
+    _prepare_cmd_torchrun,
+    _run_cmd_bcprun,
+    _run_cmd_torchrun,
+    algo_to_pickle,
+)
 from monai.bundle.config_parser import ConfigParser
 from monai.config import PathLike
-from monai.utils import ensure_tuple, run_cmd
+from monai.utils import ensure_tuple, look_up_option, run_cmd
 from monai.utils.enums import AlgoKeys
 
 logger = get_logger(module_name=__name__)
 ALGO_HASH = os.environ.get("MONAI_ALGO_HASH", "e01d67a")
 
 __all__ = ["BundleAlgo", "BundleGen"]
 
@@ -84,15 +91,15 @@
         self.fill_records: dict = {}
         # device_setting set default value and sanity check, in case device_setting not from autorunner
         self.device_setting: dict[str, int | str] = {
             "CUDA_VISIBLE_DEVICES": ",".join([str(x) for x in range(torch.cuda.device_count())]),
             "n_devices": int(torch.cuda.device_count()),
             "NUM_NODES": int(os.environ.get("NUM_NODES", 1)),
             "MN_START_METHOD": os.environ.get("MN_START_METHOD", "bcprun"),
-            "CMD_PREFIX": os.environ.get("CMD_PREFIX"),  # type: ignore
+            "CMD_PREFIX": os.environ.get("CMD_PREFIX", ""),  # type: ignore
         }
 
     def pre_check_skip_algo(self, skip_bundlegen: bool = False, skip_info: str = "") -> tuple[bool, str]:
         """
         Analyse the data analysis report and check if the algorithm needs to be skipped.
         This function is overriden within algo.
         Args:
@@ -171,83 +178,84 @@
         if train_params is None:
             train_params = {}
         params = deepcopy(train_params)
 
         train_py = os.path.join(self.output_path, "scripts", "train.py")
         config_dir = os.path.join(self.output_path, "configs")
 
+        config_files = []
         if os.path.isdir(config_dir):
-            base_cmd = ""
             for file in sorted(os.listdir(config_dir)):
-                if not (file.endswith("yaml") or file.endswith("json")):
-                    continue
-                base_cmd += f"{train_py} run --config_file=" if len(base_cmd) == 0 else ","
-                # Python Fire may be confused by single-quoted WindowsPath
-                config_yaml = Path(os.path.join(config_dir, file)).as_posix()
-                base_cmd += f"'{config_yaml}'"
-        cmd: str | None = self.device_setting["CMD_PREFIX"]  # type: ignore
-        # make sure cmd end with a space
-        if cmd is not None and not cmd.endswith(" "):
-            cmd += " "
-        if (int(self.device_setting["NUM_NODES"]) > 1 and self.device_setting["MN_START_METHOD"] == "bcprun") or (
-            int(self.device_setting["NUM_NODES"]) <= 1 and int(self.device_setting["n_devices"]) <= 1
-        ):
-            cmd = "python " if cmd is None else cmd
-        elif int(self.device_setting["NUM_NODES"]) > 1:
-            raise NotImplementedError(
-                f"{self.device_setting['MN_START_METHOD']} is not supported yet."
-                "Try modify BundleAlgo._create_cmd for your cluster."
+                if file.endswith("yaml") or file.endswith("json"):
+                    # Python Fire may be confused by single-quoted WindowsPath
+                    config_files.append(Path(os.path.join(config_dir, file)).as_posix())
+
+        if int(self.device_setting["NUM_NODES"]) > 1:
+            # multi-node command
+            # only bcprun is supported for now
+            try:
+                look_up_option(self.device_setting["MN_START_METHOD"], ["bcprun"])
+            except ValueError as err:
+                raise NotImplementedError(
+                    f"{self.device_setting['MN_START_METHOD']} is not supported yet."
+                    "Try modify BundleAlgo._create_cmd for your cluster."
+                ) from err
+
+            return (
+                _prepare_cmd_bcprun(
+                    f"{train_py} run",
+                    cmd_prefix=f"{self.device_setting['CMD_PREFIX']}",
+                    config_file=config_files,
+                    **params,
+                ),
+                "",
             )
+        elif int(self.device_setting["n_devices"]) > 1:
+            return _prepare_cmd_torchrun(f"{train_py} run", config_file=config_files, **params), ""
         else:
-            if cmd is None:
-                cmd = f"torchrun --nnodes={1:d} --nproc_per_node={self.device_setting['n_devices']:d} "
-        cmd += base_cmd
-        if params and isinstance(params, Mapping):
-            for k, v in params.items():
-                cmd += f" --{k}={v}"
-        return cmd, ""
+            return (
+                _prepare_cmd_default(
+                    f"{train_py} run",
+                    cmd_prefix=f"{self.device_setting['CMD_PREFIX']}",
+                    config_file=config_files,
+                    **params,
+                ),
+                "",
+            )
 
     def _run_cmd(self, cmd: str, devices_info: str = "") -> subprocess.CompletedProcess:
         """
         Execute the training command with target devices information.
 
         """
         if devices_info:
             warnings.warn(f"input devices_info {devices_info} is deprecated and ignored.")
 
         ps_environ = os.environ.copy()
         ps_environ["CUDA_VISIBLE_DEVICES"] = str(self.device_setting["CUDA_VISIBLE_DEVICES"])
+
+        # delete pattern "VAR=VALUE" at the beginning of the string, with optional leading/trailing whitespaces
+        cmd = re.sub(r"^\s*\w+=.*?\s+", "", cmd)
+
         if int(self.device_setting["NUM_NODES"]) > 1:
-            if self.device_setting["MN_START_METHOD"] == "bcprun":
-                cmd_list = [
-                    "bcprun",
-                    "-n",
-                    str(self.device_setting["NUM_NODES"]),
-                    "-p",
-                    str(self.device_setting["n_devices"]),
-                    "-c",
-                    cmd,
-                ]
-            else:
+            try:
+                look_up_option(self.device_setting["MN_START_METHOD"], ["bcprun"])
+            except ValueError as err:
                 raise NotImplementedError(
-                    f"{self.device_setting['MN_START_METHOD']} is not supported yet. "
+                    f"{self.device_setting['MN_START_METHOD']} is not supported yet."
                     "Try modify BundleAlgo._run_cmd for your cluster."
-                )
-        else:
-            cmd_list = cmd.split()
-
-        _idx = 0
-        for _idx, c in enumerate(cmd_list):
-            if "=" not in c:  # remove variable assignments before the command such as "OMP_NUM_THREADS=1"
-                break
-        cmd_list = cmd_list[_idx:]
-
-        logger.info(f"Launching: {' '.join(cmd_list)}")
+                ) from err
 
-        return run_cmd(cmd_list, env=ps_environ, check=True)
+            return _run_cmd_bcprun(cmd, n=self.device_setting["NUM_NODES"], p=self.device_setting["n_devices"])
+        elif int(self.device_setting["n_devices"]) > 1:
+            return _run_cmd_torchrun(
+                cmd, nnodes=1, nproc_per_node=self.device_setting["n_devices"], env=ps_environ, check=True
+            )
+        else:
+            return run_cmd(cmd.split(), run_cmd_verbose=True, env=ps_environ, check=True)
 
     def train(
         self, train_params: None | dict = None, device_setting: None | dict = None
     ) -> subprocess.CompletedProcess:
         """
         Load the run function in the training script of each model. Training parameter is predefined by the
         algo_config.yaml file, which is pre-filled by the fill_template_config function in the same instance.
```

### Comparing `monai-weekly-1.3.dev2327/monai/apps/auto3dseg/data_analyzer.py` & `monai-weekly-1.3.dev2328/monai/apps/auto3dseg/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/auto3dseg/ensemble_builder.py` & `monai-weekly-1.3.dev2328/monai/apps/auto3dseg/ensemble_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,27 @@
 import torch
 import torch.distributed as dist
 
 from monai.apps.auto3dseg.bundle_gen import BundleAlgo
 from monai.apps.auto3dseg.utils import get_name_from_algo_id, import_bundle_algo_history
 from monai.apps.utils import get_logger
 from monai.auto3dseg import concat_val_to_np
-from monai.auto3dseg.utils import datafold_read
+from monai.auto3dseg.utils import (
+    _prepare_cmd_bcprun,
+    _prepare_cmd_torchrun,
+    _run_cmd_bcprun,
+    _run_cmd_torchrun,
+    datafold_read,
+)
 from monai.bundle import ConfigParser
 from monai.data import partition_dataset
 from monai.transforms import MeanEnsemble, SaveImage, VoteEnsemble
 from monai.utils import RankFilter, deprecated_arg
 from monai.utils.enums import AlgoKeys
-from monai.utils.misc import check_kwargs_exist_in_class_init, prob2class, run_cmd
+from monai.utils.misc import check_kwargs_exist_in_class_init, prob2class
 from monai.utils.module import look_up_option, optional_import
 
 tqdm, has_tqdm = optional_import("tqdm", name="tqdm")
 
 logger = get_logger(module_name=__name__)
 
 
@@ -443,15 +449,15 @@
         self.rank = 0
         self.world_size = 1
         self.device_setting: dict[str, int | str] = {
             "CUDA_VISIBLE_DEVICES": ",".join([str(x) for x in range(torch.cuda.device_count())]),
             "n_devices": torch.cuda.device_count(),
             "NUM_NODES": int(os.environ.get("NUM_NODES", 1)),
             "MN_START_METHOD": os.environ.get("MN_START_METHOD", "bcprun"),
-            "CMD_PREFIX": os.environ.get("CMD_PREFIX"),  # type: ignore
+            "CMD_PREFIX": os.environ.get("CMD_PREFIX", ""),  # type: ignore
         }
 
     def set_ensemble_method(self, ensemble_method_name: str = "AlgoEnsembleBestByFold", **kwargs: Any) -> None:
         """
         Set the bundle ensemble method
 
         Args:
@@ -638,38 +644,24 @@
 
         if self.kwargs and isinstance(self.kwargs, Mapping):
             for k, v in self.kwargs.items():
                 base_cmd += f" --{k}={v}"
         # define env for subprocess
         ps_environ = os.environ.copy()
         ps_environ["CUDA_VISIBLE_DEVICES"] = str(self.device_setting["CUDA_VISIBLE_DEVICES"])
-        cmd: str | None = self.device_setting["CMD_PREFIX"]  # type: ignore
-        if cmd is not None and not str(cmd).endswith(" "):
-            cmd += " "
         if int(self.device_setting["NUM_NODES"]) > 1:
             if self.device_setting["MN_START_METHOD"] != "bcprun":
                 raise NotImplementedError(
                     f"{self.device_setting['MN_START_METHOD']} is not supported yet. "
                     "Try modify EnsembleRunner._create_cmd for your cluster."
                 )
             logger.info(f"Ensembling on {self.device_setting['NUM_NODES']} nodes!")
-            cmd = "python " if cmd is None else cmd
-            cmd = f"{cmd} -m {base_cmd}"
-            cmd_list = [
-                "bcprun",
-                "-n",
-                str(self.device_setting["NUM_NODES"]),
-                "-p",
-                str(self.device_setting["n_devices"]),
-                "-c",
-                cmd,
-            ]
+            cmd = _prepare_cmd_bcprun("-m " + base_cmd, cmd_prefix=f"{self.device_setting['CMD_PREFIX']}")
+            _run_cmd_bcprun(cmd, n=self.device_setting["NUM_NODES"], p=self.device_setting["n_devices"])
 
         else:
             logger.info(f"Ensembling using {self.device_setting['n_devices']} GPU!")
-            if cmd is None:
-                cmd = f"torchrun --nnodes={1:d} --nproc_per_node={self.device_setting['n_devices']:d} "
-            cmd = f"{cmd} -m {base_cmd}"
-            cmd_list = cmd.split()
-
-        run_cmd(cmd_list, env=ps_environ, check=True)
+            cmd = _prepare_cmd_torchrun("-m " + base_cmd)
+            _run_cmd_torchrun(
+                cmd, nnodes=1, nproc_per_node=self.device_setting["n_devices"], env=ps_environ, check=True
+            )
         return
```

### Comparing `monai-weekly-1.3.dev2327/monai/apps/auto3dseg/hpo_gen.py` & `monai-weekly-1.3.dev2328/monai/apps/auto3dseg/hpo_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/auto3dseg/transforms.py` & `monai-weekly-1.3.dev2328/monai/apps/auto3dseg/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/auto3dseg/utils.py` & `monai-weekly-1.3.dev2328/monai/apps/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/datasets.py` & `monai-weekly-1.3.dev2328/monai/apps/datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/deepedit/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/deepedit/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/deepedit/interaction.py` & `monai-weekly-1.3.dev2328/monai/apps/deepedit/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/deepedit/transforms.py` & `monai-weekly-1.3.dev2328/monai/apps/deepedit/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/deepgrow/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/deepgrow/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/deepgrow/dataset.py` & `monai-weekly-1.3.dev2328/monai/apps/deepgrow/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/deepgrow/interaction.py` & `monai-weekly-1.3.dev2328/monai/apps/deepgrow/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/deepgrow/transforms.py` & `monai-weekly-1.3.dev2328/monai/apps/deepgrow/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/metrics/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/metrics/coco.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/metrics/coco.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/metrics/matching.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/metrics/matching.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/networks/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/networks/retinanet_detector.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/networks/retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/networks/retinanet_network.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/networks/retinanet_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/transforms/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/transforms/array.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/transforms/box_ops.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/transforms/box_ops.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/transforms/dictionary.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/utils/ATSS_matcher.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/utils/ATSS_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/utils/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/utils/anchor_utils.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/utils/anchor_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/utils/box_coder.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/utils/box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/utils/box_selector.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/utils/box_selector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/utils/detector_utils.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/utils/detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/utils/hard_negative_sampler.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/utils/hard_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/detection/utils/predict_utils.py` & `monai-weekly-1.3.dev2328/monai/apps/detection/utils/predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/mmars/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/mmars/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/mmars/mmars.py` & `monai-weekly-1.3.dev2328/monai/apps/mmars/mmars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/mmars/model_desc.py` & `monai-weekly-1.3.dev2328/monai/apps/mmars/model_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/nnunet/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/nnunet/__main__.py` & `monai-weekly-1.3.dev2328/monai/apps/nnunet/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/nnunet/nnunetv2_runner.py` & `monai-weekly-1.3.dev2328/monai/apps/nnunet/nnunetv2_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
             kwargs.pop("trainer_class_name")
             logger.warning("please specify the `trainer_class_name` in the __init__ of `nnUNetV2Runner`.")
 
         if "export_validation_probabilities" in kwargs:
             kwargs.pop("export_validation_probabilities")
             logger.warning("please specify the `export_validation_probabilities` in the __init__ of `nnUNetV2Runner`.")
 
-        if isinstance(gpu_id, tuple) or isinstance(gpu_id, list):
+        if isinstance(gpu_id, (tuple, list)):
             if len(gpu_id) > 1:
                 gpu_ids_str = ""
                 for _i in range(len(gpu_id)):
                     gpu_ids_str += f"{gpu_id[_i]},"
                 os.environ["CUDA_VISIBLE_DEVICES"] = gpu_ids_str[:-1]
             else:
                 os.environ["CUDA_VISIBLE_DEVICES"] = f"{gpu_id[0]}"
```

### Comparing `monai-weekly-1.3.dev2327/monai/apps/nnunet/utils.py` & `monai-weekly-1.3.dev2328/monai/apps/nnunet/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/nuclick/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/nuclick/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/nuclick/transforms.py` & `monai-weekly-1.3.dev2328/monai/apps/nuclick/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/engines/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/engines/utils.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/handlers/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/handlers/utils.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/inferers/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/inferers/inferer.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/losses/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/losses/hovernet_loss.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/losses/hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/metrics/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/metrics/lesion_froc.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/metrics/lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/post/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/post/array.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/post/dictionary.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/stain/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/stain/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/stain/array.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/stain/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/transforms/stain/dictionary.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/transforms/stain/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/pathology/utils.py` & `monai-weekly-1.3.dev2328/monai/apps/pathology/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/complex_utils.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/fastmri_reader.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/mri_utils.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/blocks/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/blocks/varnetblock.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/blocks/varnetblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/nets/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/nets/complex_unet.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/nets/complex_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/nets/utils.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/nets/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/networks/nets/varnet.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/networks/nets/varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/transforms/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/transforms/array.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/reconstruction/transforms/dictionary.py` & `monai-weekly-1.3.dev2328/monai/apps/reconstruction/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/tcia/__init__.py` & `monai-weekly-1.3.dev2328/monai/apps/tcia/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/tcia/label_desc.py` & `monai-weekly-1.3.dev2328/monai/apps/tcia/label_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/tcia/utils.py` & `monai-weekly-1.3.dev2328/monai/apps/tcia/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/apps/utils.py` & `monai-weekly-1.3.dev2328/monai/apps/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/auto3dseg/__init__.py` & `monai-weekly-1.3.dev2328/monai/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/auto3dseg/algo_gen.py` & `monai-weekly-1.3.dev2328/monai/auto3dseg/algo_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/auto3dseg/analyzer.py` & `monai-weekly-1.3.dev2328/monai/auto3dseg/analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/auto3dseg/operations.py` & `monai-weekly-1.3.dev2328/monai/auto3dseg/operations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/auto3dseg/seg_summarizer.py` & `monai-weekly-1.3.dev2328/monai/auto3dseg/seg_summarizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/auto3dseg/utils.py` & `monai-weekly-1.3.dev2328/monai/auto3dseg/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import logging
 import os
 import pickle
+import subprocess
 import sys
 from copy import deepcopy
 from numbers import Number
 from typing import Any, cast
 
 import numpy as np
 import torch
 
 from monai.auto3dseg import Algo
 from monai.bundle.config_parser import ConfigParser
 from monai.bundle.utils import ID_SEP_KEY
 from monai.config import PathLike
 from monai.data.meta_tensor import MetaTensor
 from monai.transforms import CropForeground, ToCupy
-from monai.utils import min_version, optional_import
+from monai.utils import min_version, optional_import, run_cmd
 
 __all__ = [
     "get_foreground_image",
     "get_foreground_label",
     "get_label_ccp",
     "concat_val_to_np",
     "concat_multikeys_to_dict",
@@ -368,7 +369,156 @@
         algo.output_path = pkl_dir
 
     algo_meta_data = {}
     for k, v in data.items():
         algo_meta_data.update({k: v})
 
     return algo, algo_meta_data
+
+
+def list_to_python_fire_arg_str(args: list) -> str:
+    """
+    Convert a list of arguments to a string that can be used in python-fire.
+
+    Args:
+        args: the list of arguments.
+
+    Returns:
+        the string that can be used in python-fire.
+    """
+    args_str = ",".join([str(arg) for arg in args])
+    return f"'{args_str}'"
+
+
+def check_and_set_optional_args(params: dict) -> str:
+    """convert `params` into '--key_1=value_1 --key_2=value_2 ...'"""
+    cmd_mod_opt = ""
+    for k, v in params.items():
+        if isinstance(v, dict):
+            raise ValueError("Nested dict is not supported.")
+        elif isinstance(v, list):
+            v = list_to_python_fire_arg_str(v)
+        cmd_mod_opt += f" --{k}={v}"
+    return cmd_mod_opt
+
+
+def _prepare_cmd_default(cmd: str, cmd_prefix: str | None = None, **kwargs: Any) -> str:
+    """
+    Prepare the command for subprocess to run the script with the given arguments.
+
+    Args:
+        cmd: the command or script to run in the distributed job.
+        cmd_prefix: the command prefix to run the script, e.g., "python", "python -m", "python3", "/opt/conda/bin/python3.8 ".
+        kwargs: the keyword arguments to be passed to the script.
+
+    Returns:
+        the command to run with ``subprocess``.
+
+    Examples:
+        To prepare a subprocess command
+        "python train.py run -k --config 'a,b'", the function can be called as
+        - _prepare_cmd_default("train.py run -k", config=['a','b'])
+        - _prepare_cmd_default("train.py run -k --config 'a,b'")
+
+    """
+    params = kwargs.copy()
+
+    if not cmd_prefix or "None" in cmd_prefix:  # defaulting to 'python'
+        cmd_prefix = "python"
+
+    if not cmd_prefix.endswith(" "):
+        cmd_prefix += " "  # ensure a space after the command prefix so that the script can be appended
+
+    return cmd_prefix + cmd + check_and_set_optional_args(params)
+
+
+def _prepare_cmd_torchrun(cmd: str, **kwargs: Any) -> str:
+    """
+    Prepare the command for multi-gpu/multi-node job execution using torchrun.
+
+    Args:
+        cmd: the command or script to run in the distributed job.
+        kwargs: the keyword arguments to be passed to the script.
+
+    Returns:
+        the command to append to ``torchrun``
+
+    Examples:
+        For command "torchrun --nnodes=1 --nproc_per_node=8 train.py run -k --config 'a,b'",
+        it only prepares command after the torchrun arguments, i.e., "train.py run -k --config 'a,b'".
+        The function can be called as
+        - _prepare_cmd_torchrun("train.py run -k", config=['a','b'])
+        - _prepare_cmd_torchrun("train.py run -k --config 'a,b'")
+    """
+    params = kwargs.copy()
+    return cmd + check_and_set_optional_args(params)
+
+
+def _prepare_cmd_bcprun(cmd: str, cmd_prefix: str | None = None, **kwargs: Any) -> str:
+    """
+    Prepare the command for distributed job running using bcprun.
+
+    Args:
+        script: the script to run in the distributed job.
+        cmd_prefix: the command prefix to run the script, e.g., "python".
+        kwargs: the keyword arguments to be passed to the script.
+
+    Returns:
+        The command to run the script in the distributed job.
+
+    Examples:
+        For command "bcprun -n 2 -p 8 -c python train.py run -k --config 'a,b'",
+        it only prepares command after the bcprun arguments, i.e., "train.py run -k --config 'a,b'".
+        the function can be called as
+        - _prepare_cmd_bcprun("train.py run -k", config=['a','b'], n=2, p=8)
+        - _prepare_cmd_bcprun("train.py run -k --config 'a,b'", n=2, p=8)
+    """
+
+    return _prepare_cmd_default(cmd, cmd_prefix=cmd_prefix, **kwargs)
+
+
+def _run_cmd_torchrun(cmd: str, **kwargs: Any) -> subprocess.CompletedProcess:
+    """
+    Run the command with torchrun.
+
+    Args:
+        cmd: the command to run. Typically it is prepared by ``_prepare_cmd_torchrun``.
+        kwargs: the keyword arguments to be passed to the ``torchrun``.
+
+    Return:
+        the return code of the subprocess command.
+    """
+    params = kwargs.copy()
+
+    cmd_list = cmd.split()
+
+    # append arguments to the command list
+    torchrun_list = ["torchrun"]
+    required_args = ["nnodes", "nproc_per_node"]
+    for arg in required_args:
+        if arg not in params:
+            raise ValueError(f"Missing required argument {arg} for torchrun.")
+        torchrun_list += [f"--{arg}", str(params.pop(arg))]
+    torchrun_list += cmd_list
+    return run_cmd(torchrun_list, run_cmd_verbose=True, **params)
+
+
+def _run_cmd_bcprun(cmd: str, **kwargs: Any) -> subprocess.CompletedProcess:
+    """
+    Run the command with bcprun.
+
+    Args:
+        cmd: the command to run. Typically it is prepared by ``_prepare_cmd_bcprun``.
+        kwargs: the keyword arguments to be passed to the ``bcprun``.
+
+    Returns:
+        the return code of the subprocess command.
+    """
+    params = kwargs.copy()
+    cmd_list = ["bcprun"]
+    required_args = ["n", "p"]
+    for arg in required_args:
+        if arg not in params:
+            raise ValueError(f"Missing required argument {arg} for bcprun.")
+        cmd_list += [f"-{arg}", str(params.pop(arg))]
+    cmd_list.extend(["-c", cmd])
+    return run_cmd(cmd_list, run_cmd_verbose=True, **params)
```

### Comparing `monai-weekly-1.3.dev2327/monai/bundle/__init__.py` & `monai-weekly-1.3.dev2328/monai/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/bundle/__main__.py` & `monai-weekly-1.3.dev2328/monai/bundle/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/bundle/config_item.py` & `monai-weekly-1.3.dev2328/monai/bundle/config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/bundle/config_parser.py` & `monai-weekly-1.3.dev2328/monai/bundle/config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/bundle/properties.py` & `monai-weekly-1.3.dev2328/monai/bundle/properties.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/bundle/reference_resolver.py` & `monai-weekly-1.3.dev2328/monai/bundle/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/bundle/scripts.py` & `monai-weekly-1.3.dev2328/monai/bundle/scripts.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/bundle/utils.py` & `monai-weekly-1.3.dev2328/monai/bundle/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/bundle/workflows.py` & `monai-weekly-1.3.dev2328/monai/bundle/workflows.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/config/__init__.py` & `monai-weekly-1.3.dev2328/monai/config/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/config/deviceconfig.py` & `monai-weekly-1.3.dev2328/monai/config/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/config/type_definitions.py` & `monai-weekly-1.3.dev2328/monai/config/type_definitions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/__init__.py` & `monai-weekly-1.3.dev2328/monai/data/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/box_utils.py` & `monai-weekly-1.3.dev2328/monai/data/box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/csv_saver.py` & `monai-weekly-1.3.dev2328/monai/data/csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/dataloader.py` & `monai-weekly-1.3.dev2328/monai/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/dataset.py` & `monai-weekly-1.3.dev2328/monai/data/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/dataset_summary.py` & `monai-weekly-1.3.dev2328/monai/data/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/decathlon_datalist.py` & `monai-weekly-1.3.dev2328/monai/data/decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/fft_utils.py` & `monai-weekly-1.3.dev2328/monai/data/fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/folder_layout.py` & `monai-weekly-1.3.dev2328/monai/data/folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/grid_dataset.py` & `monai-weekly-1.3.dev2328/monai/data/grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/image_dataset.py` & `monai-weekly-1.3.dev2328/monai/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/image_reader.py` & `monai-weekly-1.3.dev2328/monai/data/image_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/image_writer.py` & `monai-weekly-1.3.dev2328/monai/data/image_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/iterable_dataset.py` & `monai-weekly-1.3.dev2328/monai/data/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/itk_torch_bridge.py` & `monai-weekly-1.3.dev2328/monai/data/itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/meta_obj.py` & `monai-weekly-1.3.dev2328/monai/data/meta_obj.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/meta_tensor.py` & `monai-weekly-1.3.dev2328/monai/data/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/samplers.py` & `monai-weekly-1.3.dev2328/monai/data/samplers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/synthetic.py` & `monai-weekly-1.3.dev2328/monai/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/test_time_augmentation.py` & `monai-weekly-1.3.dev2328/monai/data/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/thread_buffer.py` & `monai-weekly-1.3.dev2328/monai/data/thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/torchscript_utils.py` & `monai-weekly-1.3.dev2328/monai/data/torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/utils.py` & `monai-weekly-1.3.dev2328/monai/data/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/video_dataset.py` & `monai-weekly-1.3.dev2328/monai/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/wsi_datasets.py` & `monai-weekly-1.3.dev2328/monai/data/wsi_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/data/wsi_reader.py` & `monai-weekly-1.3.dev2328/monai/data/wsi_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/engines/__init__.py` & `monai-weekly-1.3.dev2328/monai/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/engines/evaluator.py` & `monai-weekly-1.3.dev2328/monai/engines/evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/engines/multi_gpu_supervised_trainer.py` & `monai-weekly-1.3.dev2328/monai/engines/multi_gpu_supervised_trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/engines/trainer.py` & `monai-weekly-1.3.dev2328/monai/engines/trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/engines/utils.py` & `monai-weekly-1.3.dev2328/monai/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/engines/workflow.py` & `monai-weekly-1.3.dev2328/monai/engines/workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/fl/__init__.py` & `monai-weekly-1.3.dev2328/monai/fl/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/fl/client/__init__.py` & `monai-weekly-1.3.dev2328/monai/fl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/fl/client/client_algo.py` & `monai-weekly-1.3.dev2328/monai/fl/client/client_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/fl/client/monai_algo.py` & `monai-weekly-1.3.dev2328/monai/fl/client/monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/fl/utils/__init__.py` & `monai-weekly-1.3.dev2328/monai/fl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/fl/utils/constants.py` & `monai-weekly-1.3.dev2328/monai/fl/utils/constants.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/fl/utils/exchange_object.py` & `monai-weekly-1.3.dev2328/monai/fl/utils/exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/fl/utils/filters.py` & `monai-weekly-1.3.dev2328/monai/fl/utils/filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/__init__.py` & `monai-weekly-1.3.dev2328/monai/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/checkpoint_loader.py` & `monai-weekly-1.3.dev2328/monai/handlers/checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/checkpoint_saver.py` & `monai-weekly-1.3.dev2328/monai/handlers/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/classification_saver.py` & `monai-weekly-1.3.dev2328/monai/handlers/classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/clearml_handlers.py` & `monai-weekly-1.3.dev2328/monai/handlers/clearml_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/confusion_matrix.py` & `monai-weekly-1.3.dev2328/monai/handlers/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/decollate_batch.py` & `monai-weekly-1.3.dev2328/monai/handlers/decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/earlystop_handler.py` & `monai-weekly-1.3.dev2328/monai/handlers/earlystop_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/garbage_collector.py` & `monai-weekly-1.3.dev2328/monai/handlers/garbage_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             - 20 (INFO)
             - 10 (DEBUG)
             - 0 (NOTSET)
     """
 
     def __init__(self, trigger_event: str | Events | CallableEventWithFilter = "epoch", log_level: int = 10):
         self.trigger_event: Events | CallableEventWithFilter
-        if isinstance(trigger_event, Events) or isinstance(trigger_event, CallableEventWithFilter):
+        if isinstance(trigger_event, (Events, CallableEventWithFilter)):
             self.trigger_event = trigger_event
         elif trigger_event.lower() == "epoch":
             self.trigger_event = Events.EPOCH_COMPLETED
         elif trigger_event.lower() == "iteration":
             self.trigger_event = Events.ITERATION_COMPLETED
         else:
             raise ValueError(
```

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/hausdorff_distance.py` & `monai-weekly-1.3.dev2328/monai/handlers/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/ignite_metric.py` & `monai-weekly-1.3.dev2328/monai/handlers/ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/logfile_handler.py` & `monai-weekly-1.3.dev2328/monai/handlers/logfile_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/lr_schedule_handler.py` & `monai-weekly-1.3.dev2328/monai/handlers/lr_schedule_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/mean_dice.py` & `monai-weekly-1.3.dev2328/monai/handlers/mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/mean_iou.py` & `monai-weekly-1.3.dev2328/monai/handlers/mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/metric_logger.py` & `monai-weekly-1.3.dev2328/monai/handlers/metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/metrics_reloaded_handler.py` & `monai-weekly-1.3.dev2328/monai/handlers/metrics_reloaded_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/metrics_saver.py` & `monai-weekly-1.3.dev2328/monai/handlers/metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/mlflow_handler.py` & `monai-weekly-1.3.dev2328/monai/handlers/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/nvtx_handlers.py` & `monai-weekly-1.3.dev2328/monai/handlers/nvtx_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/panoptic_quality.py` & `monai-weekly-1.3.dev2328/monai/handlers/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/parameter_scheduler.py` & `monai-weekly-1.3.dev2328/monai/handlers/parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/postprocessing.py` & `monai-weekly-1.3.dev2328/monai/handlers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/probability_maps.py` & `monai-weekly-1.3.dev2328/monai/handlers/probability_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/regression_metrics.py` & `monai-weekly-1.3.dev2328/monai/handlers/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/roc_auc.py` & `monai-weekly-1.3.dev2328/monai/handlers/roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/smartcache_handler.py` & `monai-weekly-1.3.dev2328/monai/handlers/smartcache_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/stats_handler.py` & `monai-weekly-1.3.dev2328/monai/handlers/stats_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/surface_distance.py` & `monai-weekly-1.3.dev2328/monai/handlers/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/tensorboard_handlers.py` & `monai-weekly-1.3.dev2328/monai/handlers/tensorboard_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/utils.py` & `monai-weekly-1.3.dev2328/monai/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/handlers/validation_handler.py` & `monai-weekly-1.3.dev2328/monai/handlers/validation_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/inferers/__init__.py` & `monai-weekly-1.3.dev2328/monai/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/inferers/inferer.py` & `monai-weekly-1.3.dev2328/monai/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/inferers/merger.py` & `monai-weekly-1.3.dev2328/monai/inferers/merger.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from monai.utils import ensure_tuple_size, optional_import, require_pkg
 
 if TYPE_CHECKING:
     import zarr
 else:
     zarr, _ = optional_import("zarr")
 
-
 __all__ = ["Merger", "AvgMerger", "ZarrAvgMerger"]
 
 
 class Merger(ABC):
     """
     A base class for merging patches.
     Extend this class to support operations for `PatchInference`.
```

### Comparing `monai-weekly-1.3.dev2327/monai/inferers/splitter.py` & `monai-weekly-1.3.dev2328/monai/inferers/splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/inferers/utils.py` & `monai-weekly-1.3.dev2328/monai/inferers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/__init__.py` & `monai-weekly-1.3.dev2328/monai/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/contrastive.py` & `monai-weekly-1.3.dev2328/monai/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/deform.py` & `monai-weekly-1.3.dev2328/monai/losses/deform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/dice.py` & `monai-weekly-1.3.dev2328/monai/losses/dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/ds_loss.py` & `monai-weekly-1.3.dev2328/monai/losses/ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/focal_loss.py` & `monai-weekly-1.3.dev2328/monai/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/giou_loss.py` & `monai-weekly-1.3.dev2328/monai/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/image_dissimilarity.py` & `monai-weekly-1.3.dev2328/monai/losses/image_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/multi_scale.py` & `monai-weekly-1.3.dev2328/monai/losses/multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/spatial_mask.py` & `monai-weekly-1.3.dev2328/monai/losses/spatial_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/ssim_loss.py` & `monai-weekly-1.3.dev2328/monai/losses/ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/tversky.py` & `monai-weekly-1.3.dev2328/monai/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/losses/unified_focal_loss.py` & `monai-weekly-1.3.dev2328/monai/losses/unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/__init__.py` & `monai-weekly-1.3.dev2328/monai/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/active_learning_metrics.py` & `monai-weekly-1.3.dev2328/monai/metrics/active_learning_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/confusion_matrix.py` & `monai-weekly-1.3.dev2328/monai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/cumulative_average.py` & `monai-weekly-1.3.dev2328/monai/metrics/cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/f_beta_score.py` & `monai-weekly-1.3.dev2328/monai/metrics/f_beta_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/froc.py` & `monai-weekly-1.3.dev2328/monai/metrics/froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/generalized_dice.py` & `monai-weekly-1.3.dev2328/monai/metrics/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/hausdorff_distance.py` & `monai-weekly-1.3.dev2328/monai/metrics/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/loss_metric.py` & `monai-weekly-1.3.dev2328/monai/metrics/loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/meandice.py` & `monai-weekly-1.3.dev2328/monai/metrics/meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/meaniou.py` & `monai-weekly-1.3.dev2328/monai/metrics/meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/metric.py` & `monai-weekly-1.3.dev2328/monai/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/panoptic_quality.py` & `monai-weekly-1.3.dev2328/monai/metrics/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/regression.py` & `monai-weekly-1.3.dev2328/monai/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/rocauc.py` & `monai-weekly-1.3.dev2328/monai/metrics/rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/surface_dice.py` & `monai-weekly-1.3.dev2328/monai/metrics/surface_dice.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,16 +31,17 @@
 
 
 class SurfaceDiceMetric(CumulativeIterationMetric):
     """
     Computes the Normalized Surface Dice (NSD) for each batch sample and class of
     predicted segmentations `y_pred` and corresponding reference segmentations `y` according to equation :eq:`nsd`.
     This implementation is based on https://arxiv.org/abs/2111.05408 and supports 2D and 3D images.
-    Be aware that the computation of boundaries is different from DeepMind's implementation
-    https://github.com/deepmind/surface-distance. In this implementation, the length/area of a segmentation boundary is
+    Be aware that by default (`use_subvoxels=False`), the computation of boundaries is different from DeepMind's
+    mplementation https://github.com/deepmind/surface-distance.
+    In this implementation, the length/area of a segmentation boundary is
     interpreted as the number of its edge pixels. In DeepMind's implementation, the length of a segmentation boundary
     depends on the local neighborhood (cf. https://arxiv.org/abs/1809.04430).
     This issue is discussed here: https://github.com/Project-MONAI/MONAI/issues/4103.
 
     The class- and batch sample-wise NSD values can be aggregated with the function `aggregate`.
 
     Example of the typical execution steps of this metric class follows :py:class:`monai.metrics.metric.Cumulative`.
@@ -82,36 +83,39 @@
     def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor, **kwargs: Any) -> torch.Tensor:  # type: ignore[override]
         r"""
         Args:
             y_pred: Predicted segmentation, typically segmentation model output.
                 It must be a one-hot encoded, batch-first tensor [B,C,H,W] or [B,C,H,W,D].
             y: Reference segmentation.
                 It must be a one-hot encoded, batch-first tensor [B,C,H,W] or [B,C,H,W,D].
-            kwargs: additional parameters, e.g. ``spacing`` should be passed to correctly compute the metric.
+            kwargs: additional parameters: ``spacing`` should be passed to correctly compute the metric.
                 ``spacing``: spacing of pixel (or voxel). This parameter is relevant only
                 if ``distance_metric`` is set to ``"euclidean"``.
                 If a single number, isotropic spacing with that value is used for all images in the batch. If a sequence of numbers,
                 the length of the sequence must be equal to the image dimensions.
                 This spacing will be used for all images in the batch.
                 If a sequence of sequences, the length of the outer sequence must be equal to the batch size.
                 If inner sequence has length 1, isotropic spacing with that value is used for all images in the batch,
                 else the inner sequence length must be equal to the image dimensions. If ``None``, spacing of unity is used
                 for all images in batch. Defaults to ``None``.
+                use_subvoxels: Whether to use subvoxel distances. Defaults to ``False``.
+
 
         Returns:
             Pytorch Tensor of shape [B,C], containing the NSD values :math:`\operatorname {NSD}_{b,c}` for each batch
             index :math:`b` and class :math:`c`.
         """
         return compute_surface_dice(
             y_pred=y_pred,
             y=y,
             class_thresholds=self.class_thresholds,
             include_background=self.include_background,
             distance_metric=self.distance_metric,
             spacing=kwargs.get("spacing"),
+            use_subvoxels=kwargs.get("use_subvoxels", False),
         )
 
     def aggregate(
         self, reduction: MetricReduction | str | None = None
     ) -> torch.Tensor | tuple[torch.Tensor, torch.Tensor]:
         r"""
         Aggregates the output of `_compute_tensor`.
@@ -137,50 +141,50 @@
 def compute_surface_dice(
     y_pred: torch.Tensor,
     y: torch.Tensor,
     class_thresholds: list[float],
     include_background: bool = False,
     distance_metric: str = "euclidean",
     spacing: int | float | np.ndarray | Sequence[int | float | np.ndarray | Sequence[int | float]] | None = None,
+    use_subvoxels: bool = False,
 ) -> torch.Tensor:
     r"""
     This function computes the (Normalized) Surface Dice (NSD) between the two tensors `y_pred` (referred to as
     :math:`\hat{Y}`) and `y` (referred to as :math:`Y`). This metric determines which fraction of a segmentation
     boundary is correctly predicted. A boundary element is considered correctly predicted if the closest distance to the
-    reference boundary is smaller than or equal to the specified threshold related to the acceptable amount of deviation in
-    pixels. The NSD is bounded between 0 and 1.
+    reference boundary is smaller than or equal to the specified threshold related to the acceptable amount of deviation
+    in pixels. The NSD is bounded between 0 and 1.
 
     This implementation supports multi-class tasks with an individual threshold :math:`\tau_c` for each class :math:`c`.
     The class-specific NSD for batch index :math:`b`, :math:`\operatorname {NSD}_{b,c}`, is computed using the function:
 
     .. math::
         \operatorname {NSD}_{b,c} \left(Y_{b,c}, \hat{Y}_{b,c}\right) = \frac{\left|\mathcal{D}_{Y_{b,c}}^{'}\right| +
         \left| \mathcal{D}_{\hat{Y}_{b,c}}^{'} \right|}{\left|\mathcal{D}_{Y_{b,c}}\right| +
         \left|\mathcal{D}_{\hat{Y}_{b,c}}\right|}
         :label: nsd
 
     with :math:`\mathcal{D}_{Y_{b,c}}` and :math:`\mathcal{D}_{\hat{Y}_{b,c}}` being two sets of nearest-neighbor
-    distances. :math:`\mathcal{D}_{Y_{b,c}}` is computed from the predicted segmentation boundary towards the reference segmentation
-    boundary and vice-versa for :math:`\mathcal{D}_{\hat{Y}_{b,c}}`. :math:`\mathcal{D}_{Y_{b,c}}^{'}` and
+    distances. :math:`\mathcal{D}_{Y_{b,c}}` is computed from the predicted segmentation boundary towards the reference
+    segmentation boundary and vice-versa for :math:`\mathcal{D}_{\hat{Y}_{b,c}}`. :math:`\mathcal{D}_{Y_{b,c}}^{'}` and
     :math:`\mathcal{D}_{\hat{Y}_{b,c}}^{'}` refer to the subsets of distances that are smaller or equal to the
     acceptable distance :math:`\tau_c`:
 
     .. math::
         \mathcal{D}_{Y_{b,c}}^{'} = \{ d \in \mathcal{D}_{Y_{b,c}} \, | \, d \leq \tau_c \}.
 
 
-    In the case of a class neither being present in the predicted segmentation, nor in the reference segmentation, a nan value
-    will be returned for this class. In the case of a class being present in only one of predicted segmentation or
-    reference segmentation, the class NSD will be 0.
+    In the case of a class neither being present in the predicted segmentation, nor in the reference segmentation,
+    a nan value will be returned for this class. In the case of a class being present in only one of predicted
+    segmentation or reference segmentation, the class NSD will be 0.
 
     This implementation is based on https://arxiv.org/abs/2111.05408 and supports 2D and 3D images.
-    Be aware that the computation of boundaries is different from DeepMind's implementation
-    https://github.com/deepmind/surface-distance. In this implementation, the length of a segmentation boundary is
-    interpreted as the number of its edge pixels. In DeepMind's implementation, the length of a segmentation boundary
-    depends on the local neighborhood (cf. https://arxiv.org/abs/1809.04430).
+    The computation of boundaries follows DeepMind's implementation
+    https://github.com/deepmind/surface-distance when `use_subvoxels=True`; Otherwise the length of a segmentation
+    boundary is interpreted as the number of its edge pixels.
 
     Args:
         y_pred: Predicted segmentation, typically segmentation model output.
             It must be a one-hot encoded, batch-first tensor [B,C,H,W] or [B,C,H,W,D].
         y: Reference segmentation.
             It must be a one-hot encoded, batch-first tensor [B,C,H,W] or [B,C,H,W,D].
         class_thresholds: List of class-specific thresholds.
@@ -194,14 +198,15 @@
         spacing: spacing of pixel (or voxel). This parameter is relevant only if ``distance_metric`` is set to ``"euclidean"``.
             If a single number, isotropic spacing with that value is used for all images in the batch. If a sequence of numbers,
             the length of the sequence must be equal to the image dimensions. This spacing will be used for all images in the batch.
             If a sequence of sequences, the length of the outer sequence must be equal to the batch size.
             If inner sequence has length 1, isotropic spacing with that value is used for all images in the batch,
             else the inner sequence length must be equal to the image dimensions. If ``None``, spacing of unity is used
             for all images in batch. Defaults to ``None``.
+        use_subvoxels: Whether to use subvoxel distances. Defaults to ``False``.
 
     Raises:
         ValueError: If `y_pred` and/or `y` are not PyTorch tensors.
         ValueError: If `y_pred` and/or `y` do not have four dimensions.
         ValueError: If `y_pred` and/or `y` have different shapes.
         ValueError: If `y_pred` and/or `y` are not one-hot encoded
         ValueError: If the number of channels of `y_pred` and/or `y` is different from the number of class thresholds.
@@ -223,19 +228,14 @@
         raise ValueError("y_pred and y should be one-hot encoded: [B,C,H,W] or [B,C,H,W,D].")
 
     if y_pred.shape != y.shape:
         raise ValueError(
             f"y_pred and y should have same shape, but instead, shapes are {y_pred.shape} (y_pred) and {y.shape} (y)."
         )
 
-    if not torch.all(y_pred.byte() == y_pred) or not torch.all(y.byte() == y):
-        raise ValueError("y_pred and y should be binarized tensors (e.g. torch.int64).")
-    if torch.any(y_pred > 1) or torch.any(y > 1):
-        raise ValueError("y_pred and y should be one-hot encoded.")
-
     y = y.float()
     y_pred = y_pred.float()
 
     batch_size, n_class = y_pred.shape[:2]
 
     if n_class != len(class_thresholds):
         raise ValueError(
@@ -250,32 +250,45 @@
 
     nsd = np.empty((batch_size, n_class))
 
     img_dim = y_pred.ndim - 2
     spacing_list = prepare_spacing(spacing=spacing, batch_size=batch_size, img_dim=img_dim)
 
     for b, c in np.ndindex(batch_size, n_class):
-        (edges_pred, edges_gt) = get_mask_edges(y_pred[b, c], y[b, c], crop=False)
+        if not use_subvoxels:
+            (edges_pred, edges_gt) = get_mask_edges(y_pred[b, c], y[b, c], crop=True)
+            distances_pred_gt = get_surface_distance(
+                edges_pred, edges_gt, distance_metric=distance_metric, spacing=spacing_list[b]
+            )
+            distances_gt_pred = get_surface_distance(
+                edges_gt, edges_pred, distance_metric=distance_metric, spacing=spacing_list[b]
+            )
+
+            boundary_complete = len(distances_pred_gt) + len(distances_gt_pred)
+            boundary_correct = np.sum(distances_pred_gt <= class_thresholds[c]) + np.sum(
+                distances_gt_pred <= class_thresholds[c]
+            )
+        else:
+            _spacing = spacing_list[b] if spacing_list[b] is not None else [1] * img_dim
+            areas_pred: np.ndarray
+            areas_gt: np.ndarray
+            edges_pred, edges_gt, areas_pred, areas_gt = get_mask_edges(  # type: ignore
+                y_pred[b, c], y[b, c], crop=True, spacing=_spacing  # type: ignore
+            )
+            dist_pred_to_gt = get_surface_distance(edges_pred, edges_gt, distance_metric, spacing=spacing_list[b])
+            dist_gt_to_pred = get_surface_distance(edges_gt, edges_pred, distance_metric, spacing=spacing_list[b])
+            areas_gt, areas_pred = areas_gt[edges_gt], areas_pred[edges_pred]
+            boundary_complete = areas_gt.sum() + areas_pred.sum()
+            gt_true = areas_gt[dist_gt_to_pred <= class_thresholds[c]].sum() if len(areas_gt) > 0 else 0.0
+            pred_true = areas_pred[dist_pred_to_gt <= class_thresholds[c]].sum() if len(areas_pred) > 0 else 0.0
+            boundary_correct = gt_true + pred_true
         if not np.any(edges_gt):
             warnings.warn(f"the ground truth of class {c} is all 0, this may result in nan/inf distance.")
         if not np.any(edges_pred):
             warnings.warn(f"the prediction of class {c} is all 0, this may result in nan/inf distance.")
-
-        distances_pred_gt = get_surface_distance(
-            edges_pred, edges_gt, distance_metric=distance_metric, spacing=spacing_list[b]
-        )
-        distances_gt_pred = get_surface_distance(
-            edges_gt, edges_pred, distance_metric=distance_metric, spacing=spacing_list[b]
-        )
-
-        boundary_complete = len(distances_pred_gt) + len(distances_gt_pred)
-        boundary_correct = np.sum(distances_pred_gt <= class_thresholds[c]) + np.sum(
-            distances_gt_pred <= class_thresholds[c]
-        )
-
         if boundary_complete == 0:
             # the class is neither present in the prediction, nor in the reference segmentation
             nsd[b, c] = np.nan
         else:
             nsd[b, c] = boundary_correct / boundary_complete
 
     return convert_data_type(nsd, output_type=torch.Tensor, device=y_pred.device, dtype=torch.float)[0]
```

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/surface_distance.py` & `monai-weekly-1.3.dev2328/monai/metrics/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/metrics/wrapper.py` & `monai-weekly-1.3.dev2328/monai/metrics/wrapper.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/__init__.py` & `monai-weekly-1.3.dev2328/monai/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/__init__.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/acti_norm.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/acti_norm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/activation.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/aspp.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/backbone_fpn_utils.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/backbone_fpn_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/convolutions.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/crf.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/crf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/denseblock.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/dints_block.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/dints_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/downsample.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/downsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/dynunet_block.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/encoder.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/encoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/fcn.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/fcn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/feature_pyramid_network.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/feature_pyramid_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/fft_utils_t.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/fft_utils_t.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/localnet_block.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/mlp.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/patchembedding.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/regunet_block.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/segresnet_block.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/selfattention.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/squeeze_and_excitation.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/text_embedding.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/text_embedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/transformerblock.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/unetr_block.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/upsample.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/blocks/warp.py` & `monai-weekly-1.3.dev2328/monai/networks/blocks/warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/layers/__init__.py` & `monai-weekly-1.3.dev2328/monai/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/layers/convutils.py` & `monai-weekly-1.3.dev2328/monai/networks/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/layers/drop_path.py` & `monai-weekly-1.3.dev2328/monai/networks/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/layers/factories.py` & `monai-weekly-1.3.dev2328/monai/networks/layers/factories.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/layers/filtering.py` & `monai-weekly-1.3.dev2328/monai/networks/layers/filtering.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/layers/gmm.py` & `monai-weekly-1.3.dev2328/monai/networks/layers/gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/layers/simplelayers.py` & `monai-weekly-1.3.dev2328/monai/networks/layers/simplelayers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/layers/spatial_transforms.py` & `monai-weekly-1.3.dev2328/monai/networks/layers/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/layers/utils.py` & `monai-weekly-1.3.dev2328/monai/networks/layers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/layers/weight_init.py` & `monai-weekly-1.3.dev2328/monai/networks/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/__init__.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/ahnet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/attentionunet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/autoencoder.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/basic_unet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/basic_unetplusplus.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/classifier.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/classifier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/daf3d.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/daf3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/densenet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/dints.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/dints.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/dynunet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/efficientnet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/flexible_unet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/fullyconnectednet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/generator.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/highresnet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/hovernet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/milmodel.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/netadapter.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/netadapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/quicknat.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/quicknat.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/regressor.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/regressor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/regunet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/resnet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/segresnet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/segresnet_ds.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/senet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/swin_unetr.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/torchvision_fc.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/torchvision_fc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/transchex.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/unet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/unetr.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/varautoencoder.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/vit.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/vitautoenc.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/nets/vnet.py` & `monai-weekly-1.3.dev2328/monai/networks/nets/vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/networks/utils.py` & `monai-weekly-1.3.dev2328/monai/networks/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/optimizers/__init__.py` & `monai-weekly-1.3.dev2328/monai/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/optimizers/lr_finder.py` & `monai-weekly-1.3.dev2328/monai/optimizers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/optimizers/lr_scheduler.py` & `monai-weekly-1.3.dev2328/monai/optimizers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/optimizers/novograd.py` & `monai-weekly-1.3.dev2328/monai/optimizers/novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/optimizers/utils.py` & `monai-weekly-1.3.dev2328/monai/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/__init__.py` & `monai-weekly-1.3.dev2328/monai/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/adaptors.py` & `monai-weekly-1.3.dev2328/monai/transforms/adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/compose.py` & `monai-weekly-1.3.dev2328/monai/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/croppad/__init__.py` & `monai-weekly-1.3.dev2328/monai/transforms/croppad/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/croppad/array.py` & `monai-weekly-1.3.dev2328/monai/transforms/croppad/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -820,30 +820,30 @@
     """
 
     def __init__(
         self,
         select_fn: Callable = is_positive,
         channel_indices: IndexSelection | None = None,
         margin: Sequence[int] | int = 0,
-        allow_smaller: bool = True,
+        allow_smaller: bool = False,
         return_coords: bool = False,
         k_divisible: Sequence[int] | int = 1,
         mode: str = PytorchPadMode.CONSTANT,
         lazy: bool = False,
         **pad_kwargs,
     ) -> None:
         """
         Args:
             select_fn: function to select expected foreground, default is to select values > 0.
             channel_indices: if defined, select foreground only on the specified channels
                 of image. if None, select foreground on the whole image.
             margin: add margin value to spatial dims of the bounding box, if only 1 value provided, use it for all dims.
-            allow_smaller: when computing box size with `margin`, whether allow the image size to be smaller
-                than box size, default to `True`. if the margined size is larger than image size, will pad with
-                specified `mode`.
+            allow_smaller: when computing box size with `margin`, whether to allow the final box edges to be outside of
+                the image edges (the image is smaller than the box). If `True`, part of a padded output box might be outside
+                of the original image, if `False`, the image edges will be used as the box edges.
             return_coords: whether return the coordinates of spatial bounding box for foreground.
             k_divisible: make each spatial dimension to be divisible by k, default to 1.
                 if `k_divisible` is an int, the same `k` be applied to all the input spatial dimensions.
             mode: available modes for numpy array:{``"constant"``, ``"edge"``, ``"linear_ramp"``, ``"maximum"``,
                 ``"mean"``, ``"median"``, ``"minimum"``, ``"reflect"``, ``"symmetric"``, ``"wrap"``, ``"empty"``}
                 available modes for PyTorch Tensor: {``"constant"``, ``"reflect"``, ``"replicate"``, ``"circular"``}.
                 One of the listed string values or a user supplied function. Defaults to ``"constant"``.
```

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/croppad/batch.py` & `monai-weekly-1.3.dev2328/monai/transforms/croppad/batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/croppad/dictionary.py` & `monai-weekly-1.3.dev2328/monai/transforms/croppad/dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -725,35 +725,35 @@
     def __init__(
         self,
         keys: KeysCollection,
         source_key: str,
         select_fn: Callable = is_positive,
         channel_indices: IndexSelection | None = None,
         margin: Sequence[int] | int = 0,
-        allow_smaller: bool = True,
+        allow_smaller: bool = False,
         k_divisible: Sequence[int] | int = 1,
         mode: SequenceStr = PytorchPadMode.CONSTANT,
-        start_coord_key: str = "foreground_start_coord",
-        end_coord_key: str = "foreground_end_coord",
+        start_coord_key: str | None = "foreground_start_coord",
+        end_coord_key: str | None = "foreground_end_coord",
         allow_missing_keys: bool = False,
         lazy: bool = False,
         **pad_kwargs,
     ) -> None:
         """
         Args:
             keys: keys of the corresponding items to be transformed.
                 See also: :py:class:`monai.transforms.compose.MapTransform`
             source_key: data source to generate the bounding box of foreground, can be image or label, etc.
             select_fn: function to select expected foreground, default is to select values > 0.
             channel_indices: if defined, select foreground only on the specified channels
                 of image. if None, select foreground on the whole image.
             margin: add margin value to spatial dims of the bounding box, if only 1 value provided, use it for all dims.
-            allow_smaller: when computing box size with `margin`, whether allow the image size to be smaller
-                than box size, default to `True`. if the margined size is larger than image size, will pad with
-                specified `mode`.
+            allow_smaller: when computing box size with `margin`, whether to allow the final box edges to be outside of
+                the image edges (the image is smaller than the box). If `True`, part of a padded output box might be outside
+                of the original image, if `False`, the image edges will be used as the box edges.
             k_divisible: make each spatial dimension to be divisible by k, default to 1.
                 if `k_divisible` is an int, the same `k` be applied to all the input spatial dimensions.
             mode: available modes for numpy array:{``"constant"``, ``"edge"``, ``"linear_ramp"``, ``"maximum"``,
                 ``"mean"``, ``"median"``, ``"minimum"``, ``"reflect"``, ``"symmetric"``, ``"wrap"``, ``"empty"``}
                 available modes for PyTorch Tensor: {``"constant"``, ``"reflect"``, ``"replicate"``, ``"circular"``}.
                 One of the listed string values or a user supplied function. Defaults to ``"constant"``.
                 See also: https://numpy.org/doc/1.18/reference/generated/numpy.pad.html
```

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/croppad/functional.py` & `monai-weekly-1.3.dev2328/monai/transforms/croppad/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/intensity/__init__.py` & `monai-weekly-1.3.dev2328/monai/transforms/intensity/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/intensity/array.py` & `monai-weekly-1.3.dev2328/monai/transforms/intensity/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/intensity/dictionary.py` & `monai-weekly-1.3.dev2328/monai/transforms/intensity/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/inverse.py` & `monai-weekly-1.3.dev2328/monai/transforms/inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/inverse_batch_transform.py` & `monai-weekly-1.3.dev2328/monai/transforms/inverse_batch_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/io/__init__.py` & `monai-weekly-1.3.dev2328/monai/transforms/io/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/io/array.py` & `monai-weekly-1.3.dev2328/monai/transforms/io/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/io/dictionary.py` & `monai-weekly-1.3.dev2328/monai/transforms/io/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/lazy/__init__.py` & `monai-weekly-1.3.dev2328/monai/transforms/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/lazy/array.py` & `monai-weekly-1.3.dev2328/monai/transforms/lazy/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/lazy/dictionary.py` & `monai-weekly-1.3.dev2328/monai/transforms/lazy/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/lazy/functional.py` & `monai-weekly-1.3.dev2328/monai/transforms/lazy/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/lazy/utils.py` & `monai-weekly-1.3.dev2328/monai/transforms/lazy/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/meta_utility/__init__.py` & `monai-weekly-1.3.dev2328/monai/transforms/meta_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/meta_utility/dictionary.py` & `monai-weekly-1.3.dev2328/monai/transforms/meta_utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/nvtx.py` & `monai-weekly-1.3.dev2328/monai/transforms/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/post/__init__.py` & `monai-weekly-1.3.dev2328/monai/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/post/array.py` & `monai-weekly-1.3.dev2328/monai/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/post/dictionary.py` & `monai-weekly-1.3.dev2328/monai/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/signal/__init__.py` & `monai-weekly-1.3.dev2328/monai/transforms/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/signal/array.py` & `monai-weekly-1.3.dev2328/monai/transforms/signal/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/smooth_field/__init__.py` & `monai-weekly-1.3.dev2328/monai/transforms/smooth_field/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/smooth_field/array.py` & `monai-weekly-1.3.dev2328/monai/transforms/smooth_field/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/smooth_field/dictionary.py` & `monai-weekly-1.3.dev2328/monai/transforms/smooth_field/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/spatial/__init__.py` & `monai-weekly-1.3.dev2328/monai/transforms/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/spatial/array.py` & `monai-weekly-1.3.dev2328/monai/transforms/spatial/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/spatial/dictionary.py` & `monai-weekly-1.3.dev2328/monai/transforms/spatial/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/spatial/functional.py` & `monai-weekly-1.3.dev2328/monai/transforms/spatial/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/traits.py` & `monai-weekly-1.3.dev2328/monai/transforms/traits.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/transform.py` & `monai-weekly-1.3.dev2328/monai/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/utility/__init__.py` & `monai-weekly-1.3.dev2328/monai/transforms/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/utility/array.py` & `monai-weekly-1.3.dev2328/monai/transforms/utility/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/utility/dictionary.py` & `monai-weekly-1.3.dev2328/monai/transforms/utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/utils.py` & `monai-weekly-1.3.dev2328/monai/transforms/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,36 +946,37 @@
 
 
 def generate_spatial_bounding_box(
     img: NdarrayOrTensor,
     select_fn: Callable = is_positive,
     channel_indices: IndexSelection | None = None,
     margin: Sequence[int] | int = 0,
-    allow_smaller: bool = True,
+    allow_smaller: bool = False,
 ) -> tuple[list[int], list[int]]:
     """
     Generate the spatial bounding box of foreground in the image with start-end positions (inclusive).
     Users can define arbitrary function to select expected foreground from the whole image or specified channels.
     And it can also add margin to every dim of the bounding box.
     The output format of the coordinates is:
 
         [1st_spatial_dim_start, 2nd_spatial_dim_start, ..., Nth_spatial_dim_start],
         [1st_spatial_dim_end, 2nd_spatial_dim_end, ..., Nth_spatial_dim_end]
 
-    If `allow_smaller`, the bounding boxes edges are aligned with the input image edges.
     This function returns [0, 0, ...], [0, 0, ...] if there's no positive intensity.
 
     Args:
         img: a "channel-first" image of shape (C, spatial_dim1[, spatial_dim2, ...]) to generate bounding box from.
         select_fn: function to select expected foreground, default is to select values > 0.
         channel_indices: if defined, select foreground only on the specified channels
             of image. if None, select foreground on the whole image.
         margin: add margin value to spatial dims of the bounding box, if only 1 value provided, use it for all dims.
-        allow_smaller: when computing box size with `margin`, whether allow the image size to be smaller
-            than box size, default to `True`.
+        allow_smaller: when computing box size with `margin`, whether to allow the final box edges to be outside of
+                the image edges (the image is smaller than the box). If `False`, the bounding boxes edges are aligned
+                with the input image edges, default to `False`.
+
     """
     check_non_lazy_pending_ops(img, name="generate_spatial_bounding_box")
     spatial_size = img.shape[1:]
     data = img[list(ensure_tuple(channel_indices))] if channel_indices is not None else img
     data = select_fn(data).any(0)
     ndim = len(data.shape)
     margin = ensure_tuple_rep(margin, ndim)
@@ -994,15 +995,15 @@
         if not dt.any():
             # if no foreground, return all zero bounding box coords
             return [0] * ndim, [0] * ndim
 
         arg_max = where(dt == dt.max())[0]
         min_d = arg_max[0] - margin[di]
         max_d = arg_max[-1] + margin[di] + 1
-        if allow_smaller:
+        if not allow_smaller:
             min_d = max(min_d, 0)
             max_d = min(max_d, spatial_size[di])
 
         box_start[di] = min_d.detach().cpu().item() if isinstance(min_d, torch.Tensor) else min_d
         box_end[di] = max_d.detach().cpu().item() if isinstance(max_d, torch.Tensor) else max_d
 
     return box_start, box_end
```

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/utils_create_transform_ims.py` & `monai-weekly-1.3.dev2328/monai/transforms/utils_create_transform_ims.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/transforms/utils_pytorch_numpy_unification.py` & `monai-weekly-1.3.dev2328/monai/transforms/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/utils/__init__.py` & `monai-weekly-1.3.dev2328/monai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/utils/aliases.py` & `monai-weekly-1.3.dev2328/monai/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/utils/decorators.py` & `monai-weekly-1.3.dev2328/monai/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/utils/deprecate_utils.py` & `monai-weekly-1.3.dev2328/monai/utils/deprecate_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/utils/dist.py` & `monai-weekly-1.3.dev2328/monai/utils/dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/utils/enums.py` & `monai-weekly-1.3.dev2328/monai/utils/enums.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/utils/jupyter_utils.py` & `monai-weekly-1.3.dev2328/monai/utils/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/utils/misc.py` & `monai-weekly-1.3.dev2328/monai/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -837,14 +837,18 @@
 
     Returns:
         a CompletedProcess instance after the command completes.
     """
     debug = MONAIEnvVars.debug()
     kwargs["capture_output"] = kwargs.get("capture_output", debug)
 
+    if kwargs.pop("run_cmd_verbose", False):
+        import monai
+
+        monai.apps.utils.get_logger("run_cmd").info(f"{cmd_list}")
     try:
         return subprocess.run(cmd_list, **kwargs)
     except subprocess.CalledProcessError as e:
         if not debug:
             raise
         output = str(e.stdout.decode(errors="replace"))
         errors = str(e.stderr.decode(errors="replace"))
```

### Comparing `monai-weekly-1.3.dev2327/monai/utils/module.py` & `monai-weekly-1.3.dev2328/monai/utils/module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/utils/nvtx.py` & `monai-weekly-1.3.dev2328/monai/utils/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/utils/profiling.py` & `monai-weekly-1.3.dev2328/monai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/utils/state_cacher.py` & `monai-weekly-1.3.dev2328/monai/utils/state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/utils/type_conversion.py` & `monai-weekly-1.3.dev2328/monai/utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/visualize/__init__.py` & `monai-weekly-1.3.dev2328/monai/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/visualize/class_activation_maps.py` & `monai-weekly-1.3.dev2328/monai/visualize/class_activation_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/visualize/gradient_based.py` & `monai-weekly-1.3.dev2328/monai/visualize/gradient_based.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/visualize/img2tensorboard.py` & `monai-weekly-1.3.dev2328/monai/visualize/img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/visualize/occlusion_sensitivity.py` & `monai-weekly-1.3.dev2328/monai/visualize/occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/visualize/utils.py` & `monai-weekly-1.3.dev2328/monai/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai/visualize/visualizer.py` & `monai-weekly-1.3.dev2328/monai/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai_weekly.egg-info/PKG-INFO` & `monai-weekly-1.3.dev2328/monai_weekly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.3.dev2327
+Version: 1.3.dev2328
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai-weekly-1.3.dev2327/monai_weekly.egg-info/SOURCES.txt` & `monai-weekly-1.3.dev2328/monai_weekly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/monai_weekly.egg-info/requires.txt` & `monai-weekly-1.3.dev2328/monai_weekly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/pyproject.toml` & `monai-weekly-1.3.dev2328/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/setup.cfg` & `monai-weekly-1.3.dev2328/setup.cfg`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/setup.py` & `monai-weekly-1.3.dev2328/setup.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_acn_block.py` & `monai-weekly-1.3.dev2328/tests/test_acn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_activations.py` & `monai-weekly-1.3.dev2328/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_activationsd.py` & `monai-weekly-1.3.dev2328/tests/test_activationsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_adaptors.py` & `monai-weekly-1.3.dev2328/tests/test_adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_add_channeld.py` & `monai-weekly-1.3.dev2328/tests/test_add_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_add_coordinate_channels.py` & `monai-weekly-1.3.dev2328/tests/test_add_coordinate_channels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_add_coordinate_channelsd.py` & `monai-weekly-1.3.dev2328/tests/test_add_coordinate_channelsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_add_extreme_points_channel.py` & `monai-weekly-1.3.dev2328/tests/test_add_extreme_points_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_add_extreme_points_channeld.py` & `monai-weekly-1.3.dev2328/tests/test_add_extreme_points_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_adjust_contrast.py` & `monai-weekly-1.3.dev2328/tests/test_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_adjust_contrastd.py` & `monai-weekly-1.3.dev2328/tests/test_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_adn.py` & `monai-weekly-1.3.dev2328/tests/test_adn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_affine.py` & `monai-weekly-1.3.dev2328/tests/test_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_affine_grid.py` & `monai-weekly-1.3.dev2328/tests/test_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_affine_transform.py` & `monai-weekly-1.3.dev2328/tests/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_affined.py` & `monai-weekly-1.3.dev2328/tests/test_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_ahnet.py` & `monai-weekly-1.3.dev2328/tests/test_ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_alias.py` & `monai-weekly-1.3.dev2328/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_anchor_box.py` & `monai-weekly-1.3.dev2328/tests/test_anchor_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_apply.py` & `monai-weekly-1.3.dev2328/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_apply_filter.py` & `monai-weekly-1.3.dev2328/tests/test_apply_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_arraydataset.py` & `monai-weekly-1.3.dev2328/tests/test_arraydataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_as_channel_first.py` & `monai-weekly-1.3.dev2328/tests/test_as_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_as_channel_firstd.py` & `monai-weekly-1.3.dev2328/tests/test_as_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_as_channel_last.py` & `monai-weekly-1.3.dev2328/tests/test_as_channel_last.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_as_channel_lastd.py` & `monai-weekly-1.3.dev2328/tests/test_as_channel_lastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_as_discrete.py` & `monai-weekly-1.3.dev2328/tests/test_as_discrete.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_as_discreted.py` & `monai-weekly-1.3.dev2328/tests/test_as_discreted.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_atss_box_matcher.py` & `monai-weekly-1.3.dev2328/tests/test_atss_box_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_attentionunet.py` & `monai-weekly-1.3.dev2328/tests/test_attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_auto3dseg.py` & `monai-weekly-1.3.dev2328/tests/test_auto3dseg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_auto3dseg_bundlegen.py` & `monai-weekly-1.3.dev2328/tests/test_auto3dseg_bundlegen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_auto3dseg_ensemble.py` & `monai-weekly-1.3.dev2328/tests/test_auto3dseg_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_auto3dseg_hpo.py` & `monai-weekly-1.3.dev2328/tests/test_auto3dseg_hpo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_autoencoder.py` & `monai-weekly-1.3.dev2328/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_avg_merger.py` & `monai-weekly-1.3.dev2328/tests/test_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_basic_unet.py` & `monai-weekly-1.3.dev2328/tests/test_basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_basic_unetplusplus.py` & `monai-weekly-1.3.dev2328/tests/test_basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bending_energy.py` & `monai-weekly-1.3.dev2328/tests/test_bending_energy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bilateral_approx_cpu.py` & `monai-weekly-1.3.dev2328/tests/test_bilateral_approx_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bilateral_approx_cuda.py` & `monai-weekly-1.3.dev2328/tests/test_bilateral_approx_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bilateral_precise.py` & `monai-weekly-1.3.dev2328/tests/test_bilateral_precise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_blend_images.py` & `monai-weekly-1.3.dev2328/tests/test_blend_images.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_border_pad.py` & `monai-weekly-1.3.dev2328/tests/test_border_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_border_padd.py` & `monai-weekly-1.3.dev2328/tests/test_border_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bounding_rect.py` & `monai-weekly-1.3.dev2328/tests/test_bounding_rect.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bounding_rectd.py` & `monai-weekly-1.3.dev2328/tests/test_bounding_rectd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_box_coder.py` & `monai-weekly-1.3.dev2328/tests/test_box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_box_transform.py` & `monai-weekly-1.3.dev2328/tests/test_box_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_box_utils.py` & `monai-weekly-1.3.dev2328/tests/test_box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bundle_ckpt_export.py` & `monai-weekly-1.3.dev2328/tests/test_bundle_ckpt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bundle_download.py` & `monai-weekly-1.3.dev2328/tests/test_bundle_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bundle_get_data.py` & `monai-weekly-1.3.dev2328/tests/test_bundle_get_data.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bundle_init_bundle.py` & `monai-weekly-1.3.dev2328/tests/test_bundle_init_bundle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bundle_onnx_export.py` & `monai-weekly-1.3.dev2328/tests/test_bundle_onnx_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bundle_trt_export.py` & `monai-weekly-1.3.dev2328/tests/test_bundle_trt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bundle_utils.py` & `monai-weekly-1.3.dev2328/tests/test_bundle_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bundle_verify_metadata.py` & `monai-weekly-1.3.dev2328/tests/test_bundle_verify_metadata.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bundle_verify_net.py` & `monai-weekly-1.3.dev2328/tests/test_bundle_verify_net.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_bundle_workflow.py` & `monai-weekly-1.3.dev2328/tests/test_bundle_workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_cachedataset.py` & `monai-weekly-1.3.dev2328/tests/test_cachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_cachedataset_parallel.py` & `monai-weekly-1.3.dev2328/tests/test_cachedataset_parallel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_cachedataset_persistent_workers.py` & `monai-weekly-1.3.dev2328/tests/test_cachedataset_persistent_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_cachentransdataset.py` & `monai-weekly-1.3.dev2328/tests/test_cachentransdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_call_dist.py` & `monai-weekly-1.3.dev2328/tests/test_call_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_cast_to_type.py` & `monai-weekly-1.3.dev2328/tests/test_cast_to_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_cast_to_typed.py` & `monai-weekly-1.3.dev2328/tests/test_cast_to_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_center_scale_crop.py` & `monai-weekly-1.3.dev2328/tests/test_center_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_center_scale_cropd.py` & `monai-weekly-1.3.dev2328/tests/test_center_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_center_spatial_crop.py` & `monai-weekly-1.3.dev2328/tests/test_center_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_center_spatial_cropd.py` & `monai-weekly-1.3.dev2328/tests/test_center_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_channel_pad.py` & `monai-weekly-1.3.dev2328/tests/test_channel_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_check_hash.py` & `monai-weekly-1.3.dev2328/tests/test_check_hash.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_check_missing_files.py` & `monai-weekly-1.3.dev2328/tests/test_check_missing_files.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_classes_to_indices.py` & `monai-weekly-1.3.dev2328/tests/test_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_classes_to_indicesd.py` & `monai-weekly-1.3.dev2328/tests/test_classes_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_complex_utils.py` & `monai-weekly-1.3.dev2328/tests/test_complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_component_locator.py` & `monai-weekly-1.3.dev2328/tests/test_component_locator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compose.py` & `monai-weekly-1.3.dev2328/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compose_get_number_conversions.py` & `monai-weekly-1.3.dev2328/tests/test_compose_get_number_conversions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compute_confusion_matrix.py` & `monai-weekly-1.3.dev2328/tests/test_compute_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compute_f_beta.py` & `monai-weekly-1.3.dev2328/tests/test_compute_f_beta.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compute_froc.py` & `monai-weekly-1.3.dev2328/tests/test_compute_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compute_generalized_dice.py` & `monai-weekly-1.3.dev2328/tests/test_compute_generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compute_ho_ver_maps.py` & `monai-weekly-1.3.dev2328/tests/test_compute_ho_ver_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compute_ho_ver_maps_d.py` & `monai-weekly-1.3.dev2328/tests/test_compute_ho_ver_maps_d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compute_meandice.py` & `monai-weekly-1.3.dev2328/tests/test_compute_meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compute_meaniou.py` & `monai-weekly-1.3.dev2328/tests/test_compute_meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compute_panoptic_quality.py` & `monai-weekly-1.3.dev2328/tests/test_compute_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compute_regression_metrics.py` & `monai-weekly-1.3.dev2328/tests/test_compute_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compute_roc_auc.py` & `monai-weekly-1.3.dev2328/tests/test_compute_roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_compute_variance.py` & `monai-weekly-1.3.dev2328/tests/test_compute_variance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_concat_itemsd.py` & `monai-weekly-1.3.dev2328/tests/test_concat_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_config_item.py` & `monai-weekly-1.3.dev2328/tests/test_config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_config_parser.py` & `monai-weekly-1.3.dev2328/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_contrastive_loss.py` & `monai-weekly-1.3.dev2328/tests/test_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_convert_data_type.py` & `monai-weekly-1.3.dev2328/tests/test_convert_data_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_convert_to_multi_channel.py` & `monai-weekly-1.3.dev2328/tests/test_convert_to_multi_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_convert_to_multi_channeld.py` & `monai-weekly-1.3.dev2328/tests/test_convert_to_multi_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_convert_to_onnx.py` & `monai-weekly-1.3.dev2328/tests/test_convert_to_onnx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_convert_to_torchscript.py` & `monai-weekly-1.3.dev2328/tests/test_convert_to_torchscript.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_convert_to_trt.py` & `monai-weekly-1.3.dev2328/tests/test_convert_to_trt.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_convolutions.py` & `monai-weekly-1.3.dev2328/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_copy_itemsd.py` & `monai-weekly-1.3.dev2328/tests/test_copy_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_copy_model_state.py` & `monai-weekly-1.3.dev2328/tests/test_copy_model_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_correct_crop_centers.py` & `monai-weekly-1.3.dev2328/tests/test_correct_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_create_cross_validation_datalist.py` & `monai-weekly-1.3.dev2328/tests/test_create_cross_validation_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_create_grid_and_affine.py` & `monai-weekly-1.3.dev2328/tests/test_create_grid_and_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_crf_cpu.py` & `monai-weekly-1.3.dev2328/tests/test_crf_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_crf_cuda.py` & `monai-weekly-1.3.dev2328/tests/test_crf_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_crop_foreground.py` & `monai-weekly-1.3.dev2328/tests/test_crop_foreground.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -59,24 +59,24 @@
             p([[[0, 0, 0, 0, 0], [0, 1, 2, 1, 0], [0, 2, 3, 2, 0], [0, 0, 0, 0, 0]]]),
             True,
         ]
     )
 
     TESTS.append(
         [
-            {"select_fn": lambda x: x > 0, "channel_indices": None, "margin": [2, 1], "allow_smaller": True},
+            {"select_fn": lambda x: x > 0, "channel_indices": None, "margin": [2, 1], "allow_smaller": False},
             p([[[0, 0, 0, 0, 0], [0, 1, 2, 1, 0], [0, 2, 3, 2, 0], [0, 0, 0, 0, 0], [0, 0, 0, 0, 0]]]),
             p([[[0, 0, 0, 0, 0], [0, 1, 2, 1, 0], [0, 2, 3, 2, 0], [0, 0, 0, 0, 0], [0, 0, 0, 0, 0]]]),
             True,
         ]
     )
 
     TESTS.append(
         [
-            {"select_fn": lambda x: x > 0, "channel_indices": None, "margin": [2, 1], "allow_smaller": False},
+            {"select_fn": lambda x: x > 0, "channel_indices": None, "margin": [2, 1], "allow_smaller": True},
             p([[[0, 0, 0, 0, 0], [0, 1, 2, 1, 0], [0, 2, 3, 2, 0], [0, 0, 0, 0, 0], [0, 0, 0, 0, 0]]]),
             p([[[0, 0, 0, 0, 0], [0, 0, 0, 0, 0], [0, 1, 2, 1, 0], [0, 2, 3, 2, 0], [0, 0, 0, 0, 0], [0, 0, 0, 0, 0]]]),
             True,
         ]
     )
 
     TESTS.append(
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_crop_foregroundd.py` & `monai-weekly-1.3.dev2328/tests/test_crop_foregroundd.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         [
             {
                 "keys": ["img"],
                 "source_key": "img",
                 "select_fn": lambda x: x > 0,
                 "channel_indices": None,
                 "margin": [2, 1],
-                "allow_smaller": True,
+                "allow_smaller": False,
             },
             {
                 "img": p(
                     np.array([[[0, 0, 0, 0, 0], [0, 1, 2, 1, 0], [0, 2, 3, 2, 0], [0, 1, 2, 1, 0], [0, 0, 0, 0, 0]]])
                 )
             },
             p(np.array([[[0, 0, 0, 0, 0], [0, 1, 2, 1, 0], [0, 2, 3, 2, 0], [0, 1, 2, 1, 0], [0, 0, 0, 0, 0]]])),
@@ -103,15 +103,15 @@
         [
             {
                 "keys": ["img"],
                 "source_key": "img",
                 "select_fn": lambda x: x > 0,
                 "channel_indices": None,
                 "margin": [2, 1],
-                "allow_smaller": False,
+                "allow_smaller": True,
             },
             {
                 "img": p(
                     np.array([[[0, 0, 0, 0, 0], [0, 1, 2, 1, 0], [0, 2, 3, 2, 0], [0, 1, 2, 1, 0], [0, 0, 0, 0, 0]]])
                 )
             },
             p(
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_cross_validation.py` & `monai-weekly-1.3.dev2328/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_csv_dataset.py` & `monai-weekly-1.3.dev2328/tests/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_csv_iterable_dataset.py` & `monai-weekly-1.3.dev2328/tests/test_csv_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_csv_saver.py` & `monai-weekly-1.3.dev2328/tests/test_csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_cucim_dict_transform.py` & `monai-weekly-1.3.dev2328/tests/test_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_cucim_transform.py` & `monai-weekly-1.3.dev2328/tests/test_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_cumulative.py` & `monai-weekly-1.3.dev2328/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_cumulative_average.py` & `monai-weekly-1.3.dev2328/tests/test_cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_cumulative_average_dist.py` & `monai-weekly-1.3.dev2328/tests/test_cumulative_average_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_cv2_dist.py` & `monai-weekly-1.3.dev2328/tests/test_cv2_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_daf3d.py` & `monai-weekly-1.3.dev2328/tests/test_daf3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_data_stats.py` & `monai-weekly-1.3.dev2328/tests/test_data_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_data_statsd.py` & `monai-weekly-1.3.dev2328/tests/test_data_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dataloader.py` & `monai-weekly-1.3.dev2328/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dataset.py` & `monai-weekly-1.3.dev2328/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dataset_func.py` & `monai-weekly-1.3.dev2328/tests/test_dataset_func.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dataset_summary.py` & `monai-weekly-1.3.dev2328/tests/test_dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_decathlondataset.py` & `monai-weekly-1.3.dev2328/tests/test_decathlondataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_decollate.py` & `monai-weekly-1.3.dev2328/tests/test_decollate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_deepedit_interaction.py` & `monai-weekly-1.3.dev2328/tests/test_deepedit_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_deepedit_transforms.py` & `monai-weekly-1.3.dev2328/tests/test_deepedit_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_deepgrow_dataset.py` & `monai-weekly-1.3.dev2328/tests/test_deepgrow_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_deepgrow_interaction.py` & `monai-weekly-1.3.dev2328/tests/test_deepgrow_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_deepgrow_transforms.py` & `monai-weekly-1.3.dev2328/tests/test_deepgrow_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_delete_itemsd.py` & `monai-weekly-1.3.dev2328/tests/test_delete_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_denseblock.py` & `monai-weekly-1.3.dev2328/tests/test_denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_densenet.py` & `monai-weekly-1.3.dev2328/tests/test_densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_deprecated.py` & `monai-weekly-1.3.dev2328/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_detect_envelope.py` & `monai-weekly-1.3.dev2328/tests/test_detect_envelope.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_detection_coco_metrics.py` & `monai-weekly-1.3.dev2328/tests/test_detection_coco_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_detector_boxselector.py` & `monai-weekly-1.3.dev2328/tests/test_detector_boxselector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_detector_utils.py` & `monai-weekly-1.3.dev2328/tests/test_detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dev_collate.py` & `monai-weekly-1.3.dev2328/tests/test_dev_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dice_ce_loss.py` & `monai-weekly-1.3.dev2328/tests/test_dice_ce_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dice_focal_loss.py` & `monai-weekly-1.3.dev2328/tests/test_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dice_loss.py` & `monai-weekly-1.3.dev2328/tests/test_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dints_cell.py` & `monai-weekly-1.3.dev2328/tests/test_dints_cell.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dints_mixop.py` & `monai-weekly-1.3.dev2328/tests/test_dints_mixop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dints_network.py` & `monai-weekly-1.3.dev2328/tests/test_dints_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_discriminator.py` & `monai-weekly-1.3.dev2328/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_divisible_pad.py` & `monai-weekly-1.3.dev2328/tests/test_divisible_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_divisible_padd.py` & `monai-weekly-1.3.dev2328/tests/test_divisible_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_download_and_extract.py` & `monai-weekly-1.3.dev2328/tests/test_download_and_extract.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_download_url_yandex.py` & `monai-weekly-1.3.dev2328/tests/test_download_url_yandex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_downsample_block.py` & `monai-weekly-1.3.dev2328/tests/test_downsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_drop_path.py` & `monai-weekly-1.3.dev2328/tests/test_drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_ds_loss.py` & `monai-weekly-1.3.dev2328/tests/test_ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dvf2ddf.py` & `monai-weekly-1.3.dev2328/tests/test_dvf2ddf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dynunet.py` & `monai-weekly-1.3.dev2328/tests/test_dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_dynunet_block.py` & `monai-weekly-1.3.dev2328/tests/test_dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_efficientnet.py` & `monai-weekly-1.3.dev2328/tests/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_ensemble_evaluator.py` & `monai-weekly-1.3.dev2328/tests/test_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_ensure_channel_first.py` & `monai-weekly-1.3.dev2328/tests/test_ensure_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_ensure_channel_firstd.py` & `monai-weekly-1.3.dev2328/tests/test_ensure_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_ensure_tuple.py` & `monai-weekly-1.3.dev2328/tests/test_ensure_tuple.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_ensure_type.py` & `monai-weekly-1.3.dev2328/tests/test_ensure_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_ensure_typed.py` & `monai-weekly-1.3.dev2328/tests/test_ensure_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_enum_bound_interp.py` & `monai-weekly-1.3.dev2328/tests/test_enum_bound_interp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_eval_mode.py` & `monai-weekly-1.3.dev2328/tests/test_eval_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_evenly_divisible_all_gather_dist.py` & `monai-weekly-1.3.dev2328/tests/test_evenly_divisible_all_gather_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_factorized_increase.py` & `monai-weekly-1.3.dev2328/tests/test_factorized_increase.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_factorized_reduce.py` & `monai-weekly-1.3.dev2328/tests/test_factorized_reduce.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fastmri_reader.py` & `monai-weekly-1.3.dev2328/tests/test_fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fft_utils.py` & `monai-weekly-1.3.dev2328/tests/test_fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fg_bg_to_indices.py` & `monai-weekly-1.3.dev2328/tests/test_fg_bg_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fg_bg_to_indicesd.py` & `monai-weekly-1.3.dev2328/tests/test_fg_bg_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_file_basename.py` & `monai-weekly-1.3.dev2328/tests/test_file_basename.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fill_holes.py` & `monai-weekly-1.3.dev2328/tests/test_fill_holes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fill_holesd.py` & `monai-weekly-1.3.dev2328/tests/test_fill_holesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fl_exchange_object.py` & `monai-weekly-1.3.dev2328/tests/test_fl_exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fl_monai_algo.py` & `monai-weekly-1.3.dev2328/tests/test_fl_monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fl_monai_algo_dist.py` & `monai-weekly-1.3.dev2328/tests/test_fl_monai_algo_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fl_monai_algo_stats.py` & `monai-weekly-1.3.dev2328/tests/test_fl_monai_algo_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_flatten_sub_keysd.py` & `monai-weekly-1.3.dev2328/tests/test_flatten_sub_keysd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_flexible_unet.py` & `monai-weekly-1.3.dev2328/tests/test_flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_flip.py` & `monai-weekly-1.3.dev2328/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_flipd.py` & `monai-weekly-1.3.dev2328/tests/test_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_focal_loss.py` & `monai-weekly-1.3.dev2328/tests/test_focal_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,14 @@
             b = float(output1.cpu().detach())
             if abs(a - b) > max_error:
                 max_error = abs(a - b)
         self.assertAlmostEqual(max_error, 0.0, places=3)
 
     def test_consistency_with_cross_entropy_2d_no_reduction(self):
         """For gamma=0 the focal loss reduces to the cross entropy loss"""
-        import numpy as np
 
         focal_loss = FocalLoss(to_onehot_y=False, gamma=0.0, reduction="none", weight=1.0)
         ce = nn.BCEWithLogitsLoss(reduction="none")
         max_error = 0
         class_num = 10
         batch_size = 128
         for _ in range(100):
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_folder_layout.py` & `monai-weekly-1.3.dev2328/tests/test_folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_foreground_mask.py` & `monai-weekly-1.3.dev2328/tests/test_foreground_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_foreground_maskd.py` & `monai-weekly-1.3.dev2328/tests/test_foreground_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fourier.py` & `monai-weekly-1.3.dev2328/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fpn_block.py` & `monai-weekly-1.3.dev2328/tests/test_fpn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_from_engine_hovernet.py` & `monai-weekly-1.3.dev2328/tests/test_from_engine_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_fullyconnectednet.py` & `monai-weekly-1.3.dev2328/tests/test_fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_gaussian.py` & `monai-weekly-1.3.dev2328/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_gaussian_filter.py` & `monai-weekly-1.3.dev2328/tests/test_gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_gaussian_sharpen.py` & `monai-weekly-1.3.dev2328/tests/test_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_gaussian_sharpend.py` & `monai-weekly-1.3.dev2328/tests/test_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_gaussian_smooth.py` & `monai-weekly-1.3.dev2328/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_gaussian_smoothd.py` & `monai-weekly-1.3.dev2328/tests/test_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generalized_dice_focal_loss.py` & `monai-weekly-1.3.dev2328/tests/test_generalized_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generalized_dice_loss.py` & `monai-weekly-1.3.dev2328/tests/test_generalized_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generalized_wasserstein_dice_loss.py` & `monai-weekly-1.3.dev2328/tests/test_generalized_wasserstein_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_distance_map.py` & `monai-weekly-1.3.dev2328/tests/test_generate_distance_map.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_distance_mapd.py` & `monai-weekly-1.3.dev2328/tests/test_generate_distance_mapd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_instance_border.py` & `monai-weekly-1.3.dev2328/tests/test_generate_instance_border.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_instance_borderd.py` & `monai-weekly-1.3.dev2328/tests/test_generate_instance_borderd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_instance_centroid.py` & `monai-weekly-1.3.dev2328/tests/test_generate_instance_centroid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_instance_centroidd.py` & `monai-weekly-1.3.dev2328/tests/test_generate_instance_centroidd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_instance_contour.py` & `monai-weekly-1.3.dev2328/tests/test_generate_instance_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_instance_contourd.py` & `monai-weekly-1.3.dev2328/tests/test_generate_instance_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_instance_type.py` & `monai-weekly-1.3.dev2328/tests/test_generate_instance_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_instance_typed.py` & `monai-weekly-1.3.dev2328/tests/test_generate_instance_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_label_classes_crop_centers.py` & `monai-weekly-1.3.dev2328/tests/test_generate_label_classes_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_param_groups.py` & `monai-weekly-1.3.dev2328/tests/test_generate_param_groups.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_pos_neg_label_crop_centers.py` & `monai-weekly-1.3.dev2328/tests/test_generate_pos_neg_label_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_spatial_bounding_box.py` & `monai-weekly-1.3.dev2328/tests/test_generate_spatial_bounding_box.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -78,29 +78,29 @@
             {
                 "img": p(
                     np.array([[[0, 0, 0, 0, 0], [0, 1, 2, 1, 0], [0, 2, 3, 2, 0], [0, 1, 2, 1, 0], [0, 0, 0, 0, 0]]])
                 ),
                 "select_fn": lambda x: x > 0,
                 "channel_indices": None,
                 "margin": [2, 1],
-                "allow_smaller": False,
+                "allow_smaller": True,
             },
             ([-1, 0], [6, 5]),
         ]
     )
     TESTS.append(
         [
             {
                 "img": p(
                     np.array([[[0, 0, 0, 0, 0], [0, 1, 2, 1, 0], [0, 2, 3, 2, 0], [0, 1, 2, 1, 0], [0, 0, 0, 0, 0]]])
                 ),
                 "select_fn": lambda x: x > 0,
                 "channel_indices": None,
                 "margin": [2, 1],
-                "allow_smaller": True,
+                "allow_smaller": False,
             },
             ([0, 0], [5, 5]),
         ]
     )
 
 
 class TestGenerateSpatialBoundingBox(unittest.TestCase):
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_succinct_contour.py` & `monai-weekly-1.3.dev2328/tests/test_generate_succinct_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_succinct_contourd.py` & `monai-weekly-1.3.dev2328/tests/test_generate_succinct_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_watershed_markers.py` & `monai-weekly-1.3.dev2328/tests/test_generate_watershed_markers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_watershed_markersd.py` & `monai-weekly-1.3.dev2328/tests/test_generate_watershed_markersd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_watershed_mask.py` & `monai-weekly-1.3.dev2328/tests/test_generate_watershed_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generate_watershed_maskd.py` & `monai-weekly-1.3.dev2328/tests/test_generate_watershed_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_generator.py` & `monai-weekly-1.3.dev2328/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_get_equivalent_dtype.py` & `monai-weekly-1.3.dev2328/tests/test_get_equivalent_dtype.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_get_extreme_points.py` & `monai-weekly-1.3.dev2328/tests/test_get_extreme_points.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_get_layers.py` & `monai-weekly-1.3.dev2328/tests/test_get_layers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_get_package_version.py` & `monai-weekly-1.3.dev2328/tests/test_get_package_version.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_get_unique_labels.py` & `monai-weekly-1.3.dev2328/tests/test_get_unique_labels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_gibbs_noise.py` & `monai-weekly-1.3.dev2328/tests/test_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_gibbs_noised.py` & `monai-weekly-1.3.dev2328/tests/test_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_giou_loss.py` & `monai-weekly-1.3.dev2328/tests/test_giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_global_mutual_information_loss.py` & `monai-weekly-1.3.dev2328/tests/test_global_mutual_information_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_globalnet.py` & `monai-weekly-1.3.dev2328/tests/test_globalnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_gmm.py` & `monai-weekly-1.3.dev2328/tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_grid_dataset.py` & `monai-weekly-1.3.dev2328/tests/test_grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_grid_distortion.py` & `monai-weekly-1.3.dev2328/tests/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_grid_distortiond.py` & `monai-weekly-1.3.dev2328/tests/test_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_grid_patch.py` & `monai-weekly-1.3.dev2328/tests/test_grid_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         output = splitter(input_image)
         self.assertEqual(len(output), len(expected))
         for output_patch, expected_patch in zip(output, expected):
             assert_allclose(
                 output_patch,
                 in_type(expected_patch),
                 type_test=False,
-                device_test=True if isinstance(in_type(expected_patch), torch.Tensor) else False,
+                device_test=bool(isinstance(in_type(expected_patch), torch.Tensor)),
             )
 
     @parameterized.expand([TEST_CASE_META_0, TEST_CASE_META_1])
     @SkipIfBeforePyTorchVersion((1, 9, 1))
     def test_grid_patch_meta(self, input_parameters, image, expected, expected_meta):
         set_track_meta(True)
         splitter = GridPatch(**input_parameters)
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_grid_patchd.py` & `monai-weekly-1.3.dev2328/tests/test_grid_patchd.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,13 +90,13 @@
         output = splitter(input_dict)
         self.assertEqual(len(output[image_key]), len(expected))
         for output_patch, expected_patch in zip(output[image_key], expected):
             assert_allclose(
                 output_patch,
                 in_type(expected_patch),
                 type_test=False,
-                device_test=True if isinstance(in_type(expected_patch), torch.Tensor) else False,
+                device_test=bool(isinstance(in_type(expected_patch), torch.Tensor)),
             )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_grid_pull.py` & `monai-weekly-1.3.dev2328/tests/test_grid_pull.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_grid_split.py` & `monai-weekly-1.3.dev2328/tests/test_grid_split.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_grid_splitd.py` & `monai-weekly-1.3.dev2328/tests/test_grid_splitd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_checkpoint_loader.py` & `monai-weekly-1.3.dev2328/tests/test_handler_checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_checkpoint_saver.py` & `monai-weekly-1.3.dev2328/tests/test_handler_checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_classification_saver.py` & `monai-weekly-1.3.dev2328/tests/test_handler_classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_classification_saver_dist.py` & `monai-weekly-1.3.dev2328/tests/test_handler_classification_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_clearml_image.py` & `monai-weekly-1.3.dev2328/tests/test_handler_clearml_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_clearml_stats.py` & `monai-weekly-1.3.dev2328/tests/test_handler_clearml_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_confusion_matrix.py` & `monai-weekly-1.3.dev2328/tests/test_handler_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_confusion_matrix_dist.py` & `monai-weekly-1.3.dev2328/tests/test_handler_confusion_matrix_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_decollate_batch.py` & `monai-weekly-1.3.dev2328/tests/test_handler_decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_early_stop.py` & `monai-weekly-1.3.dev2328/tests/test_handler_early_stop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_garbage_collector.py` & `monai-weekly-1.3.dev2328/tests/test_handler_garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_hausdorff_distance.py` & `monai-weekly-1.3.dev2328/tests/test_handler_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_logfile.py` & `monai-weekly-1.3.dev2328/tests/test_handler_logfile.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_lr_scheduler.py` & `monai-weekly-1.3.dev2328/tests/test_handler_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_mean_dice.py` & `monai-weekly-1.3.dev2328/tests/test_handler_mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_mean_iou.py` & `monai-weekly-1.3.dev2328/tests/test_handler_mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_metric_logger.py` & `monai-weekly-1.3.dev2328/tests/test_handler_metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_metrics_reloaded.py` & `monai-weekly-1.3.dev2328/tests/test_handler_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_metrics_saver.py` & `monai-weekly-1.3.dev2328/tests/test_handler_metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_metrics_saver_dist.py` & `monai-weekly-1.3.dev2328/tests/test_handler_metrics_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_mlflow.py` & `monai-weekly-1.3.dev2328/tests/test_handler_mlflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_nvtx.py` & `monai-weekly-1.3.dev2328/tests/test_handler_nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_panoptic_quality.py` & `monai-weekly-1.3.dev2328/tests/test_handler_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_parameter_scheduler.py` & `monai-weekly-1.3.dev2328/tests/test_handler_parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_post_processing.py` & `monai-weekly-1.3.dev2328/tests/test_handler_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_prob_map_producer.py` & `monai-weekly-1.3.dev2328/tests/test_handler_prob_map_producer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_regression_metrics.py` & `monai-weekly-1.3.dev2328/tests/test_handler_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_regression_metrics_dist.py` & `monai-weekly-1.3.dev2328/tests/test_handler_regression_metrics_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_rocauc.py` & `monai-weekly-1.3.dev2328/tests/test_handler_rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_rocauc_dist.py` & `monai-weekly-1.3.dev2328/tests/test_handler_rocauc_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_smartcache.py` & `monai-weekly-1.3.dev2328/tests/test_handler_smartcache.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_stats.py` & `monai-weekly-1.3.dev2328/tests/test_handler_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_surface_distance.py` & `monai-weekly-1.3.dev2328/tests/test_handler_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_tb_image.py` & `monai-weekly-1.3.dev2328/tests/test_handler_tb_image.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,21 +19,23 @@
 import torch
 from ignite.engine import Engine, Events
 from parameterized import parameterized
 
 from monai.data import decollate_batch
 from monai.handlers import TensorBoardImageHandler
 from monai.utils import optional_import
+from tests.utils import SkipIfBeforePyTorchVersion
 
 _, has_tb = optional_import("torch.utils.tensorboard", name="SummaryWriter")
 
 TEST_CASES = [[[20, 20]], [[2, 20, 20]], [[3, 20, 20]], [[20, 20, 20]], [[2, 20, 20, 20]], [[2, 2, 20, 20, 20]]]
 
 
 @unittest.skipUnless(has_tb, "Requires SummaryWriter installation")
+@SkipIfBeforePyTorchVersion((1, 13))  # issue 6683
 class TestHandlerTBImage(unittest.TestCase):
     @parameterized.expand(TEST_CASES)
     def test_tb_image_shape(self, shape):
         with tempfile.TemporaryDirectory() as tempdir:
             # set up engine
             def _train_func(engine, batch):
                 engine.state.batch = decollate_batch(list(batch))
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_tb_stats.py` & `monai-weekly-1.3.dev2328/tests/test_handler_tb_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_handler_validation.py` & `monai-weekly-1.3.dev2328/tests/test_handler_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_hardnegsampler.py` & `monai-weekly-1.3.dev2328/tests/test_hardnegsampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_hashing.py` & `monai-weekly-1.3.dev2328/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_hausdorff_distance.py` & `monai-weekly-1.3.dev2328/tests/test_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_header_correct.py` & `monai-weekly-1.3.dev2328/tests/test_header_correct.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_highresnet.py` & `monai-weekly-1.3.dev2328/tests/test_highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_hilbert_transform.py` & `monai-weekly-1.3.dev2328/tests/test_hilbert_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_histogram_normalize.py` & `monai-weekly-1.3.dev2328/tests/test_histogram_normalize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_histogram_normalized.py` & `monai-weekly-1.3.dev2328/tests/test_histogram_normalized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_hovernet.py` & `monai-weekly-1.3.dev2328/tests/test_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_hovernet_instance_map_post_processing.py` & `monai-weekly-1.3.dev2328/tests/test_hovernet_instance_map_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_hovernet_instance_map_post_processingd.py` & `monai-weekly-1.3.dev2328/tests/test_hovernet_instance_map_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_hovernet_loss.py` & `monai-weekly-1.3.dev2328/tests/test_hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_hovernet_nuclear_type_post_processing.py` & `monai-weekly-1.3.dev2328/tests/test_hovernet_nuclear_type_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_hovernet_nuclear_type_post_processingd.py` & `monai-weekly-1.3.dev2328/tests/test_hovernet_nuclear_type_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_identity.py` & `monai-weekly-1.3.dev2328/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_identityd.py` & `monai-weekly-1.3.dev2328/tests/test_identityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_image_dataset.py` & `monai-weekly-1.3.dev2328/tests/test_image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_image_filter.py` & `monai-weekly-1.3.dev2328/tests/test_image_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_image_rw.py` & `monai-weekly-1.3.dev2328/tests/test_image_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_img2tensorboard.py` & `monai-weekly-1.3.dev2328/tests/test_img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_init_reader.py` & `monai-weekly-1.3.dev2328/tests/test_init_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_autorunner.py` & `monai-weekly-1.3.dev2328/tests/test_integration_autorunner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_bundle_run.py` & `monai-weekly-1.3.dev2328/tests/test_integration_bundle_run.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_classification_2d.py` & `monai-weekly-1.3.dev2328/tests/test_integration_classification_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_determinism.py` & `monai-weekly-1.3.dev2328/tests/test_integration_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_fast_train.py` & `monai-weekly-1.3.dev2328/tests/test_integration_fast_train.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_gpu_customization.py` & `monai-weekly-1.3.dev2328/tests/test_integration_gpu_customization.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_lazy_samples.py` & `monai-weekly-1.3.dev2328/tests/test_integration_lazy_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_nnunetv2_runner.py` & `monai-weekly-1.3.dev2328/tests/test_integration_nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_segmentation_3d.py` & `monai-weekly-1.3.dev2328/tests/test_integration_segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_sliding_window.py` & `monai-weekly-1.3.dev2328/tests/test_integration_sliding_window.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_stn.py` & `monai-weekly-1.3.dev2328/tests/test_integration_stn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_unet_2d.py` & `monai-weekly-1.3.dev2328/tests/test_integration_unet_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_workers.py` & `monai-weekly-1.3.dev2328/tests/test_integration_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_workflows.py` & `monai-weekly-1.3.dev2328/tests/test_integration_workflows.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_integration_workflows_gan.py` & `monai-weekly-1.3.dev2328/tests/test_integration_workflows_gan.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_intensity_stats.py` & `monai-weekly-1.3.dev2328/tests/test_intensity_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_intensity_statsd.py` & `monai-weekly-1.3.dev2328/tests/test_intensity_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_inverse.py` & `monai-weekly-1.3.dev2328/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_inverse_array.py` & `monai-weekly-1.3.dev2328/tests/test_inverse_array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_inverse_collation.py` & `monai-weekly-1.3.dev2328/tests/test_inverse_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_invert.py` & `monai-weekly-1.3.dev2328/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_invertd.py` & `monai-weekly-1.3.dev2328/tests/test_invertd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_is_supported_format.py` & `monai-weekly-1.3.dev2328/tests/test_is_supported_format.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_iterable_dataset.py` & `monai-weekly-1.3.dev2328/tests/test_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_itk_torch_bridge.py` & `monai-weekly-1.3.dev2328/tests/test_itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_itk_writer.py` & `monai-weekly-1.3.dev2328/tests/test_itk_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_k_space_spike_noise.py` & `monai-weekly-1.3.dev2328/tests/test_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_k_space_spike_noised.py` & `monai-weekly-1.3.dev2328/tests/test_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_keep_largest_connected_component.py` & `monai-weekly-1.3.dev2328/tests/test_keep_largest_connected_component.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_keep_largest_connected_componentd.py` & `monai-weekly-1.3.dev2328/tests/test_keep_largest_connected_componentd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_kspace_mask.py` & `monai-weekly-1.3.dev2328/tests/test_kspace_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_label_filter.py` & `monai-weekly-1.3.dev2328/tests/test_label_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_label_filterd.py` & `monai-weekly-1.3.dev2328/tests/test_label_filterd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_label_quality_score.py` & `monai-weekly-1.3.dev2328/tests/test_label_quality_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_label_to_contour.py` & `monai-weekly-1.3.dev2328/tests/test_label_to_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_label_to_contourd.py` & `monai-weekly-1.3.dev2328/tests/test_label_to_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_label_to_mask.py` & `monai-weekly-1.3.dev2328/tests/test_label_to_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_label_to_maskd.py` & `monai-weekly-1.3.dev2328/tests/test_label_to_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_lambda.py` & `monai-weekly-1.3.dev2328/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_lambdad.py` & `monai-weekly-1.3.dev2328/tests/test_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_lesion_froc.py` & `monai-weekly-1.3.dev2328/tests/test_lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_list_data_collate.py` & `monai-weekly-1.3.dev2328/tests/test_list_data_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_list_to_dict.py` & `monai-weekly-1.3.dev2328/tests/test_list_to_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_lltm.py` & `monai-weekly-1.3.dev2328/tests/test_lltm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_lmdbdataset.py` & `monai-weekly-1.3.dev2328/tests/test_lmdbdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_lmdbdataset_dist.py` & `monai-weekly-1.3.dev2328/tests/test_lmdbdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_load_decathlon_datalist.py` & `monai-weekly-1.3.dev2328/tests/test_load_decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_load_image.py` & `monai-weekly-1.3.dev2328/tests/test_load_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_load_imaged.py` & `monai-weekly-1.3.dev2328/tests/test_load_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_load_spacing_orientation.py` & `monai-weekly-1.3.dev2328/tests/test_load_spacing_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_loader_semaphore.py` & `monai-weekly-1.3.dev2328/tests/test_loader_semaphore.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_local_normalized_cross_correlation_loss.py` & `monai-weekly-1.3.dev2328/tests/test_local_normalized_cross_correlation_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_localnet.py` & `monai-weekly-1.3.dev2328/tests/test_localnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_localnet_block.py` & `monai-weekly-1.3.dev2328/tests/test_localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_look_up_option.py` & `monai-weekly-1.3.dev2328/tests/test_look_up_option.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_loss_metric.py` & `monai-weekly-1.3.dev2328/tests/test_loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_lr_finder.py` & `monai-weekly-1.3.dev2328/tests/test_lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_lr_scheduler.py` & `monai-weekly-1.3.dev2328/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_make_nifti.py` & `monai-weekly-1.3.dev2328/tests/test_make_nifti.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_map_binary_to_indices.py` & `monai-weekly-1.3.dev2328/tests/test_map_binary_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_map_classes_to_indices.py` & `monai-weekly-1.3.dev2328/tests/test_map_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_map_label_value.py` & `monai-weekly-1.3.dev2328/tests/test_map_label_value.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_map_label_valued.py` & `monai-weekly-1.3.dev2328/tests/test_map_label_valued.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_map_transform.py` & `monai-weekly-1.3.dev2328/tests/test_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_mask_intensity.py` & `monai-weekly-1.3.dev2328/tests/test_mask_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_mask_intensityd.py` & `monai-weekly-1.3.dev2328/tests/test_mask_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_masked_dice_loss.py` & `monai-weekly-1.3.dev2328/tests/test_masked_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_masked_loss.py` & `monai-weekly-1.3.dev2328/tests/test_masked_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_masked_patch_wsi_dataset.py` & `monai-weekly-1.3.dev2328/tests/test_masked_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_matshow3d.py` & `monai-weekly-1.3.dev2328/tests/test_matshow3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_mean_ensemble.py` & `monai-weekly-1.3.dev2328/tests/test_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_mean_ensembled.py` & `monai-weekly-1.3.dev2328/tests/test_mean_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_median_filter.py` & `monai-weekly-1.3.dev2328/tests/test_median_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_median_smooth.py` & `monai-weekly-1.3.dev2328/tests/test_median_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_median_smoothd.py` & `monai-weekly-1.3.dev2328/tests/test_median_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_mednistdataset.py` & `monai-weekly-1.3.dev2328/tests/test_mednistdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_meta_affine.py` & `monai-weekly-1.3.dev2328/tests/test_meta_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_meta_tensor.py` & `monai-weekly-1.3.dev2328/tests/test_meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_metatensor_integration.py` & `monai-weekly-1.3.dev2328/tests/test_metatensor_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_metrics_reloaded.py` & `monai-weekly-1.3.dev2328/tests/test_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_milmodel.py` & `monai-weekly-1.3.dev2328/tests/test_milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_mlp.py` & `monai-weekly-1.3.dev2328/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_mmar_download.py` & `monai-weekly-1.3.dev2328/tests/test_mmar_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_module_list.py` & `monai-weekly-1.3.dev2328/tests/test_module_list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_monai_env_vars.py` & `monai-weekly-1.3.dev2328/tests/test_monai_env_vars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_monai_utils_misc.py` & `monai-weekly-1.3.dev2328/tests/test_monai_utils_misc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_mri_utils.py` & `monai-weekly-1.3.dev2328/tests/test_mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_multi_scale.py` & `monai-weekly-1.3.dev2328/tests/test_multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_net_adapter.py` & `monai-weekly-1.3.dev2328/tests/test_net_adapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_network_consistency.py` & `monai-weekly-1.3.dev2328/tests/test_network_consistency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_nifti_endianness.py` & `monai-weekly-1.3.dev2328/tests/test_nifti_endianness.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_nifti_header_revise.py` & `monai-weekly-1.3.dev2328/tests/test_nifti_header_revise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_nifti_rw.py` & `monai-weekly-1.3.dev2328/tests/test_nifti_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_normalize_intensity.py` & `monai-weekly-1.3.dev2328/tests/test_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_normalize_intensityd.py` & `monai-weekly-1.3.dev2328/tests/test_normalize_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_npzdictitemdataset.py` & `monai-weekly-1.3.dev2328/tests/test_npzdictitemdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_nrrd_reader.py` & `monai-weekly-1.3.dev2328/tests/test_nrrd_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_nuclick_transforms.py` & `monai-weekly-1.3.dev2328/tests/test_nuclick_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_numpy_reader.py` & `monai-weekly-1.3.dev2328/tests/test_numpy_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_nvtx_decorator.py` & `monai-weekly-1.3.dev2328/tests/test_nvtx_decorator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_nvtx_transform.py` & `monai-weekly-1.3.dev2328/tests/test_nvtx_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_occlusion_sensitivity.py` & `monai-weekly-1.3.dev2328/tests/test_occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_one_of.py` & `monai-weekly-1.3.dev2328/tests/test_one_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_optim_novograd.py` & `monai-weekly-1.3.dev2328/tests/test_optim_novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_optional_import.py` & `monai-weekly-1.3.dev2328/tests/test_optional_import.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_ori_ras_lps.py` & `monai-weekly-1.3.dev2328/tests/test_ori_ras_lps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_orientation.py` & `monai-weekly-1.3.dev2328/tests/test_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_orientationd.py` & `monai-weekly-1.3.dev2328/tests/test_orientationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_p3d_block.py` & `monai-weekly-1.3.dev2328/tests/test_p3d_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_pad_collation.py` & `monai-weekly-1.3.dev2328/tests/test_pad_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_pad_mode.py` & `monai-weekly-1.3.dev2328/tests/test_pad_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_parallel_execution.py` & `monai-weekly-1.3.dev2328/tests/test_parallel_execution.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_parallel_execution_dist.py` & `monai-weekly-1.3.dev2328/tests/test_parallel_execution_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_partition_dataset.py` & `monai-weekly-1.3.dev2328/tests/test_partition_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_partition_dataset_classes.py` & `monai-weekly-1.3.dev2328/tests/test_partition_dataset_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_patch_dataset.py` & `monai-weekly-1.3.dev2328/tests/test_patch_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_patch_inferer.py` & `monai-weekly-1.3.dev2328/tests/test_patch_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_patch_wsi_dataset.py` & `monai-weekly-1.3.dev2328/tests/test_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_patchembedding.py` & `monai-weekly-1.3.dev2328/tests/test_patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_pathology_he_stain.py` & `monai-weekly-1.3.dev2328/tests/test_pathology_he_stain.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_pathology_he_stain_dict.py` & `monai-weekly-1.3.dev2328/tests/test_pathology_he_stain_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_pathology_prob_nms.py` & `monai-weekly-1.3.dev2328/tests/test_pathology_prob_nms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_persistentdataset.py` & `monai-weekly-1.3.dev2328/tests/test_persistentdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_persistentdataset_dist.py` & `monai-weekly-1.3.dev2328/tests/test_persistentdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_phl_cpu.py` & `monai-weekly-1.3.dev2328/tests/test_phl_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_phl_cuda.py` & `monai-weekly-1.3.dev2328/tests/test_phl_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_pil_reader.py` & `monai-weekly-1.3.dev2328/tests/test_pil_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_plot_2d_or_3d_image.py` & `monai-weekly-1.3.dev2328/tests/test_plot_2d_or_3d_image.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import unittest
 
 import torch
 from parameterized import parameterized
 
 from monai.utils import optional_import
 from monai.visualize import plot_2d_or_3d_image
-from tests.utils import SkipIfNoModule
+from tests.utils import SkipIfBeforePyTorchVersion, SkipIfNoModule
 
 SummaryWriter, has_tb = optional_import("torch.utils.tensorboard", name="SummaryWriter")
 
 SummaryWriterX, _ = optional_import("tensorboardX", name="SummaryWriter")
 
 TEST_CASE_1 = [(1, 1, 10, 10)]
 
@@ -34,14 +34,15 @@
 
 TEST_CASE_4 = [(1, 1, 10, 10, 10)]
 
 TEST_CASE_5 = [(1, 3, 10, 10, 10)]
 
 
 @unittest.skipUnless(has_tb, "Requires SummaryWriter installation")
+@SkipIfBeforePyTorchVersion((1, 13))  # issue 6683
 class TestPlot2dOr3dImage(unittest.TestCase):
     @parameterized.expand([TEST_CASE_1, TEST_CASE_2, TEST_CASE_3, TEST_CASE_4, TEST_CASE_5])
     def test_tb_image(self, shape):
         with tempfile.TemporaryDirectory() as tempdir:
             writer = SummaryWriter(log_dir=tempdir)
             plot_2d_or_3d_image(torch.zeros(shape), 0, writer, max_channels=3, frame_dim=-1)
             writer.flush()
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_png_rw.py` & `monai-weekly-1.3.dev2328/tests/test_png_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_polyval.py` & `monai-weekly-1.3.dev2328/tests/test_polyval.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_prepare_batch_default.py` & `monai-weekly-1.3.dev2328/tests/test_prepare_batch_default.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_prepare_batch_default_dist.py` & `monai-weekly-1.3.dev2328/tests/test_prepare_batch_default_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_prepare_batch_extra_input.py` & `monai-weekly-1.3.dev2328/tests/test_prepare_batch_extra_input.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_prepare_batch_hovernet.py` & `monai-weekly-1.3.dev2328/tests/test_prepare_batch_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_preset_filters.py` & `monai-weekly-1.3.dev2328/tests/test_preset_filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_print_info.py` & `monai-weekly-1.3.dev2328/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_print_transform_backends.py` & `monai-weekly-1.3.dev2328/tests/test_print_transform_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_probnms.py` & `monai-weekly-1.3.dev2328/tests/test_probnms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_probnmsd.py` & `monai-weekly-1.3.dev2328/tests/test_probnmsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_profiling.py` & `monai-weekly-1.3.dev2328/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_pytorch_version_after.py` & `monai-weekly-1.3.dev2328/tests/test_pytorch_version_after.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_query_memory.py` & `monai-weekly-1.3.dev2328/tests/test_query_memory.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_quicknat.py` & `monai-weekly-1.3.dev2328/tests/test_quicknat.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_adjust_contrast.py` & `monai-weekly-1.3.dev2328/tests/test_rand_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_adjust_contrastd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_affine.py` & `monai-weekly-1.3.dev2328/tests/test_rand_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_affine_grid.py` & `monai-weekly-1.3.dev2328/tests/test_rand_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_affined.py` & `monai-weekly-1.3.dev2328/tests/test_rand_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_axis_flip.py` & `monai-weekly-1.3.dev2328/tests/test_rand_axis_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_axis_flipd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_axis_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_bias_field.py` & `monai-weekly-1.3.dev2328/tests/test_rand_bias_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_bias_fieldd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_bias_fieldd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_coarse_dropout.py` & `monai-weekly-1.3.dev2328/tests/test_rand_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_coarse_dropoutd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_coarse_dropoutd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_coarse_shuffle.py` & `monai-weekly-1.3.dev2328/tests/test_rand_coarse_shuffle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_coarse_shuffled.py` & `monai-weekly-1.3.dev2328/tests/test_rand_coarse_shuffled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_crop_by_label_classes.py` & `monai-weekly-1.3.dev2328/tests/test_rand_crop_by_label_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_crop_by_label_classesd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_crop_by_label_classesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_crop_by_pos_neg_label.py` & `monai-weekly-1.3.dev2328/tests/test_rand_crop_by_pos_neg_label.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_crop_by_pos_neg_labeld.py` & `monai-weekly-1.3.dev2328/tests/test_rand_crop_by_pos_neg_labeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_cucim_dict_transform.py` & `monai-weekly-1.3.dev2328/tests/test_rand_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_cucim_transform.py` & `monai-weekly-1.3.dev2328/tests/test_rand_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_deform_grid.py` & `monai-weekly-1.3.dev2328/tests/test_rand_deform_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_elastic_2d.py` & `monai-weekly-1.3.dev2328/tests/test_rand_elastic_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_elastic_3d.py` & `monai-weekly-1.3.dev2328/tests/test_rand_elastic_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_elasticd_2d.py` & `monai-weekly-1.3.dev2328/tests/test_rand_elasticd_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_elasticd_3d.py` & `monai-weekly-1.3.dev2328/tests/test_rand_elasticd_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_flip.py` & `monai-weekly-1.3.dev2328/tests/test_rand_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_flipd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_gaussian_noise.py` & `monai-weekly-1.3.dev2328/tests/test_rand_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_gaussian_noised.py` & `monai-weekly-1.3.dev2328/tests/test_rand_gaussian_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_gaussian_sharpen.py` & `monai-weekly-1.3.dev2328/tests/test_rand_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_gaussian_sharpend.py` & `monai-weekly-1.3.dev2328/tests/test_rand_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_gaussian_smooth.py` & `monai-weekly-1.3.dev2328/tests/test_rand_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_gaussian_smoothd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_gibbs_noise.py` & `monai-weekly-1.3.dev2328/tests/test_rand_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_gibbs_noised.py` & `monai-weekly-1.3.dev2328/tests/test_rand_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_grid_distortion.py` & `monai-weekly-1.3.dev2328/tests/test_rand_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_grid_distortiond.py` & `monai-weekly-1.3.dev2328/tests/test_rand_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_grid_patch.py` & `monai-weekly-1.3.dev2328/tests/test_rand_grid_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         output = splitter(input_image)
         self.assertEqual(len(output), len(expected))
         for output_patch, expected_patch in zip(output, expected):
             assert_allclose(
                 output_patch,
                 in_type(expected_patch),
                 type_test=False,
-                device_test=True if isinstance(in_type(expected_patch), torch.Tensor) else False,
+                device_test=bool(isinstance(in_type(expected_patch), torch.Tensor)),
             )
 
     @parameterized.expand([TEST_CASE_META_0, TEST_CASE_META_1])
     @SkipIfBeforePyTorchVersion((1, 9, 1))
     def test_rand_grid_patch_meta(self, input_parameters, image, expected, expected_meta):
         set_track_meta(True)
         splitter = RandGridPatch(**input_parameters)
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_grid_patchd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_grid_patchd.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,13 +95,13 @@
         output = splitter(input_dict)
         self.assertEqual(len(output[image_key]), len(expected))
         for output_patch, expected_patch in zip(output[image_key], expected):
             assert_allclose(
                 output_patch,
                 in_type(expected_patch),
                 type_test=False,
-                device_test=True if isinstance(in_type(expected_patch), torch.Tensor) else False,
+                device_test=bool(isinstance(in_type(expected_patch), torch.Tensor)),
             )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_histogram_shift.py` & `monai-weekly-1.3.dev2328/tests/test_rand_histogram_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_histogram_shiftd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_histogram_shiftd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_k_space_spike_noise.py` & `monai-weekly-1.3.dev2328/tests/test_rand_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_k_space_spike_noised.py` & `monai-weekly-1.3.dev2328/tests/test_rand_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_lambda.py` & `monai-weekly-1.3.dev2328/tests/test_rand_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_lambdad.py` & `monai-weekly-1.3.dev2328/tests/test_rand_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_rician_noise.py` & `monai-weekly-1.3.dev2328/tests/test_rand_rician_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_rician_noised.py` & `monai-weekly-1.3.dev2328/tests/test_rand_rician_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_rotate.py` & `monai-weekly-1.3.dev2328/tests/test_rand_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_rotate90.py` & `monai-weekly-1.3.dev2328/tests/test_rand_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_rotate90d.py` & `monai-weekly-1.3.dev2328/tests/test_rand_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_rotated.py` & `monai-weekly-1.3.dev2328/tests/test_rand_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_scale_crop.py` & `monai-weekly-1.3.dev2328/tests/test_rand_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_scale_cropd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_scale_intensity.py` & `monai-weekly-1.3.dev2328/tests/test_rand_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_scale_intensity_fixed_mean.py` & `monai-weekly-1.3.dev2328/tests/test_rand_scale_intensity_fixed_mean.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_scale_intensity_fixed_meand.py` & `monai-weekly-1.3.dev2328/tests/test_rand_scale_intensity_fixed_meand.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_scale_intensityd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_shift_intensity.py` & `monai-weekly-1.3.dev2328/tests/test_rand_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_shift_intensityd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_spatial_crop.py` & `monai-weekly-1.3.dev2328/tests/test_rand_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_spatial_crop_samples.py` & `monai-weekly-1.3.dev2328/tests/test_rand_spatial_crop_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_spatial_crop_samplesd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_spatial_crop_samplesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_spatial_cropd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_std_shift_intensity.py` & `monai-weekly-1.3.dev2328/tests/test_rand_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_std_shift_intensityd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_weighted_crop.py` & `monai-weekly-1.3.dev2328/tests/test_rand_weighted_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_weighted_cropd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_weighted_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_zoom.py` & `monai-weekly-1.3.dev2328/tests/test_rand_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rand_zoomd.py` & `monai-weekly-1.3.dev2328/tests/test_rand_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_randidentity.py` & `monai-weekly-1.3.dev2328/tests/test_randidentity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_random_order.py` & `monai-weekly-1.3.dev2328/tests/test_random_order.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_randomizable.py` & `monai-weekly-1.3.dev2328/tests/test_randomizable.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_randomizable_transform_type.py` & `monai-weekly-1.3.dev2328/tests/test_randomizable_transform_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_randtorchvisiond.py` & `monai-weekly-1.3.dev2328/tests/test_randtorchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rankfilter_dist.py` & `monai-weekly-1.3.dev2328/tests/test_rankfilter_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_recon_net_utils.py` & `monai-weekly-1.3.dev2328/tests/test_recon_net_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_reference_based_normalize_intensity.py` & `monai-weekly-1.3.dev2328/tests/test_reference_based_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_reference_based_spatial_cropd.py` & `monai-weekly-1.3.dev2328/tests/test_reference_based_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_reference_resolver.py` & `monai-weekly-1.3.dev2328/tests/test_reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_reg_loss_integration.py` & `monai-weekly-1.3.dev2328/tests/test_reg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_regunet.py` & `monai-weekly-1.3.dev2328/tests/test_regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_regunet_block.py` & `monai-weekly-1.3.dev2328/tests/test_regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_remove_repeated_channel.py` & `monai-weekly-1.3.dev2328/tests/test_remove_repeated_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_remove_repeated_channeld.py` & `monai-weekly-1.3.dev2328/tests/test_remove_repeated_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_remove_small_objects.py` & `monai-weekly-1.3.dev2328/tests/test_remove_small_objects.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_repeat_channel.py` & `monai-weekly-1.3.dev2328/tests/test_repeat_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_repeat_channeld.py` & `monai-weekly-1.3.dev2328/tests/test_repeat_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_replace_module.py` & `monai-weekly-1.3.dev2328/tests/test_replace_module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_require_pkg.py` & `monai-weekly-1.3.dev2328/tests/test_require_pkg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_resample.py` & `monai-weekly-1.3.dev2328/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_resample_backends.py` & `monai-weekly-1.3.dev2328/tests/test_resample_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_resample_datalist.py` & `monai-weekly-1.3.dev2328/tests/test_resample_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_resample_to_match.py` & `monai-weekly-1.3.dev2328/tests/test_resample_to_match.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_resample_to_matchd.py` & `monai-weekly-1.3.dev2328/tests/test_resample_to_matchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_resampler.py` & `monai-weekly-1.3.dev2328/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_resize.py` & `monai-weekly-1.3.dev2328/tests/test_resize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_resize_with_pad_or_crop.py` & `monai-weekly-1.3.dev2328/tests/test_resize_with_pad_or_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_resize_with_pad_or_cropd.py` & `monai-weekly-1.3.dev2328/tests/test_resize_with_pad_or_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_resized.py` & `monai-weekly-1.3.dev2328/tests/test_resized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_resnet.py` & `monai-weekly-1.3.dev2328/tests/test_resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_retinanet.py` & `monai-weekly-1.3.dev2328/tests/test_retinanet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_retinanet_detector.py` & `monai-weekly-1.3.dev2328/tests/test_retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_retinanet_predict_utils.py` & `monai-weekly-1.3.dev2328/tests/test_retinanet_predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rotate.py` & `monai-weekly-1.3.dev2328/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rotate90.py` & `monai-weekly-1.3.dev2328/tests/test_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rotate90d.py` & `monai-weekly-1.3.dev2328/tests/test_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_rotated.py` & `monai-weekly-1.3.dev2328/tests/test_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_safe_dtype_range.py` & `monai-weekly-1.3.dev2328/tests/test_safe_dtype_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_saliency_inferer.py` & `monai-weekly-1.3.dev2328/tests/test_saliency_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_sample_slices.py` & `monai-weekly-1.3.dev2328/tests/test_sample_slices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_sampler_dist.py` & `monai-weekly-1.3.dev2328/tests/test_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_save_classificationd.py` & `monai-weekly-1.3.dev2328/tests/test_save_classificationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_save_image.py` & `monai-weekly-1.3.dev2328/tests/test_save_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_save_imaged.py` & `monai-weekly-1.3.dev2328/tests/test_save_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_save_state.py` & `monai-weekly-1.3.dev2328/tests/test_save_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_savitzky_golay_filter.py` & `monai-weekly-1.3.dev2328/tests/test_savitzky_golay_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_savitzky_golay_smooth.py` & `monai-weekly-1.3.dev2328/tests/test_savitzky_golay_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_savitzky_golay_smoothd.py` & `monai-weekly-1.3.dev2328/tests/test_savitzky_golay_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_scale_intensity.py` & `monai-weekly-1.3.dev2328/tests/test_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_scale_intensity_fixed_mean.py` & `monai-weekly-1.3.dev2328/tests/test_scale_intensity_fixed_mean.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_scale_intensity_range.py` & `monai-weekly-1.3.dev2328/tests/test_scale_intensity_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_scale_intensity_range_percentiles.py` & `monai-weekly-1.3.dev2328/tests/test_scale_intensity_range_percentiles.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_scale_intensity_range_percentilesd.py` & `monai-weekly-1.3.dev2328/tests/test_scale_intensity_range_percentilesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_scale_intensity_ranged.py` & `monai-weekly-1.3.dev2328/tests/test_scale_intensity_ranged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_scale_intensityd.py` & `monai-weekly-1.3.dev2328/tests/test_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_se_block.py` & `monai-weekly-1.3.dev2328/tests/test_se_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_se_blocks.py` & `monai-weekly-1.3.dev2328/tests/test_se_blocks.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_seg_loss_integration.py` & `monai-weekly-1.3.dev2328/tests/test_seg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_segresnet.py` & `monai-weekly-1.3.dev2328/tests/test_segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_segresnet_block.py` & `monai-weekly-1.3.dev2328/tests/test_segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_segresnet_ds.py` & `monai-weekly-1.3.dev2328/tests/test_segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_select_cross_validation_folds.py` & `monai-weekly-1.3.dev2328/tests/test_select_cross_validation_folds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_select_itemsd.py` & `monai-weekly-1.3.dev2328/tests/test_select_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_selfattention.py` & `monai-weekly-1.3.dev2328/tests/test_selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_senet.py` & `monai-weekly-1.3.dev2328/tests/test_senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_separable_filter.py` & `monai-weekly-1.3.dev2328/tests/test_separable_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_set_determinism.py` & `monai-weekly-1.3.dev2328/tests/test_set_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_set_visible_devices.py` & `monai-weekly-1.3.dev2328/tests/test_set_visible_devices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_shift_intensity.py` & `monai-weekly-1.3.dev2328/tests/test_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_shift_intensityd.py` & `monai-weekly-1.3.dev2328/tests/test_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_shuffle_buffer.py` & `monai-weekly-1.3.dev2328/tests/test_shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_signal_continuouswavelet.py` & `monai-weekly-1.3.dev2328/tests/test_signal_continuouswavelet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_signal_fillempty.py` & `monai-weekly-1.3.dev2328/tests/test_signal_fillempty.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_signal_rand_add_gaussiannoise.py` & `monai-weekly-1.3.dev2328/tests/test_signal_rand_add_gaussiannoise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_signal_rand_add_sine.py` & `monai-weekly-1.3.dev2328/tests/test_signal_rand_add_sine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_signal_rand_add_sine_partial.py` & `monai-weekly-1.3.dev2328/tests/test_signal_rand_add_sine_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_signal_rand_add_squarepulse.py` & `monai-weekly-1.3.dev2328/tests/test_signal_rand_add_squarepulse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_signal_rand_add_squarepulse_partial.py` & `monai-weekly-1.3.dev2328/tests/test_signal_rand_add_squarepulse_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_signal_rand_drop.py` & `monai-weekly-1.3.dev2328/tests/test_signal_rand_drop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_signal_rand_scale.py` & `monai-weekly-1.3.dev2328/tests/test_signal_rand_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_signal_rand_shift.py` & `monai-weekly-1.3.dev2328/tests/test_signal_rand_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_signal_remove_frequency.py` & `monai-weekly-1.3.dev2328/tests/test_signal_remove_frequency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_simple_aspp.py` & `monai-weekly-1.3.dev2328/tests/test_simple_aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_simulatedelay.py` & `monai-weekly-1.3.dev2328/tests/test_simulatedelay.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_simulatedelayd.py` & `monai-weekly-1.3.dev2328/tests/test_simulatedelayd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_skip_connection.py` & `monai-weekly-1.3.dev2328/tests/test_skip_connection.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_slice_inferer.py` & `monai-weekly-1.3.dev2328/tests/test_slice_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_sliding_patch_wsi_dataset.py` & `monai-weekly-1.3.dev2328/tests/test_sliding_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_sliding_window_hovernet_inference.py` & `monai-weekly-1.3.dev2328/tests/test_sliding_window_hovernet_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_sliding_window_inference.py` & `monai-weekly-1.3.dev2328/tests/test_sliding_window_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_sliding_window_splitter.py` & `monai-weekly-1.3.dev2328/tests/test_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_smartcachedataset.py` & `monai-weekly-1.3.dev2328/tests/test_smartcachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_smooth_field.py` & `monai-weekly-1.3.dev2328/tests/test_smooth_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_sobel_gradient.py` & `monai-weekly-1.3.dev2328/tests/test_sobel_gradient.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_sobel_gradientd.py` & `monai-weekly-1.3.dev2328/tests/test_sobel_gradientd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_some_of.py` & `monai-weekly-1.3.dev2328/tests/test_some_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_spacing.py` & `monai-weekly-1.3.dev2328/tests/test_spacing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_spacingd.py` & `monai-weekly-1.3.dev2328/tests/test_spacingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_spatial_combine_transforms.py` & `monai-weekly-1.3.dev2328/tests/test_spatial_combine_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_spatial_crop.py` & `monai-weekly-1.3.dev2328/tests/test_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_spatial_cropd.py` & `monai-weekly-1.3.dev2328/tests/test_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_spatial_pad.py` & `monai-weekly-1.3.dev2328/tests/test_spatial_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_spatial_padd.py` & `monai-weekly-1.3.dev2328/tests/test_spatial_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_spatial_resample.py` & `monai-weekly-1.3.dev2328/tests/test_spatial_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_spatial_resampled.py` & `monai-weekly-1.3.dev2328/tests/test_spatial_resampled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_split_channel.py` & `monai-weekly-1.3.dev2328/tests/test_split_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_split_channeld.py` & `monai-weekly-1.3.dev2328/tests/test_split_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_splitdim.py` & `monai-weekly-1.3.dev2328/tests/test_splitdim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_splitdimd.py` & `monai-weekly-1.3.dev2328/tests/test_splitdimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_squeezedim.py` & `monai-weekly-1.3.dev2328/tests/test_squeezedim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_squeezedimd.py` & `monai-weekly-1.3.dev2328/tests/test_squeezedimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_ssim_loss.py` & `monai-weekly-1.3.dev2328/tests/test_ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_ssim_metric.py` & `monai-weekly-1.3.dev2328/tests/test_ssim_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_state_cacher.py` & `monai-weekly-1.3.dev2328/tests/test_state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_std_shift_intensity.py` & `monai-weekly-1.3.dev2328/tests/test_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_std_shift_intensityd.py` & `monai-weekly-1.3.dev2328/tests/test_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_str2bool.py` & `monai-weekly-1.3.dev2328/tests/test_str2bool.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_str2list.py` & `monai-weekly-1.3.dev2328/tests/test_str2list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_subpixel_upsample.py` & `monai-weekly-1.3.dev2328/tests/test_subpixel_upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_surface_dice.py` & `monai-weekly-1.3.dev2328/tests/test_surface_dice.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 import unittest
 
 import numpy as np
 import torch
 import torch.nn.functional as F
 
-from monai.metrics.surface_dice import SurfaceDiceMetric
+from monai.metrics.surface_dice import SurfaceDiceMetric, compute_surface_dice
+from tests.utils import assert_allclose
 
 _device = "cuda:0" if torch.cuda.is_available() else "cpu"
 
 
 class TestAllSurfaceDiceMetrics(unittest.TestCase):
     def test_tolerance_euclidean_distance_with_spacing(self):
         batch_size = 2
@@ -322,34 +323,14 @@
             SurfaceDiceMetric(class_thresholds=[1, 1], include_background=True)(predictions_hot, input_bad_shape)
         self.assertEqual(
             "y_pred and y should have same shape, but instead, shapes are torch.Size([1, 2, 80, 80]) (y_pred) and "
             "torch.Size([1, 2, 80, 50]) (y).",
             str(context.exception),
         )
 
-        # input tensors not one-hot encoded
-        predictions_no_hot = torch.clone(predictions_hot)
-        predictions_no_hot[0, :, 0, 0] = torch.tensor([2, 0])
-
-        with self.assertRaises(ValueError) as context:
-            SurfaceDiceMetric(class_thresholds=[1, 1], include_background=True)(predictions_no_hot, predictions_hot)
-        self.assertEqual("y_pred and y should be one-hot encoded.", str(context.exception))
-        with self.assertRaises(ValueError) as context:
-            SurfaceDiceMetric(class_thresholds=[1, 1], include_background=True)(predictions_hot, predictions_no_hot)
-        self.assertEqual("y_pred and y should be one-hot encoded.", str(context.exception))
-
-        predictions_no_hot = predictions_no_hot.float()
-        predictions_no_hot[0, :, 0, 0] = torch.tensor([0.5, 0])
-        with self.assertRaises(ValueError) as context:
-            SurfaceDiceMetric(class_thresholds=[1, 1], include_background=True)(predictions_no_hot, predictions_hot)
-        self.assertEqual("y_pred and y should be binarized tensors (e.g. torch.int64).", str(context.exception))
-        with self.assertRaises(ValueError) as context:
-            SurfaceDiceMetric(class_thresholds=[1, 1], include_background=True)(predictions_hot, predictions_no_hot)
-        self.assertEqual("y_pred and y should be binarized tensors (e.g. torch.int64).", str(context.exception))
-
         # wrong number of class thresholds
         with self.assertRaises(ValueError) as context:
             SurfaceDiceMetric(class_thresholds=[1, 1, 1], include_background=True)(predictions_hot, labels_hot)
         self.assertEqual("number of classes (2) does not match number of class thresholds (3).", str(context.exception))
 
         # inf and nan values in class thresholds
         with self.assertRaises(ValueError) as context:
@@ -397,10 +378,39 @@
         sur_metric_nans = SurfaceDiceMetric(class_thresholds=[1, 1, 1], include_background=True, get_not_nans=True)
         res_classes = sur_metric_nans(predictions_empty, predictions_empty)
         res, not_nans = sur_metric_nans.aggregate()
         np.testing.assert_array_equal(res_classes, [[np.nan, np.nan, np.nan], [np.nan, np.nan, np.nan]])
         np.testing.assert_equal(res, torch.tensor([0], dtype=torch.float))
         np.testing.assert_equal(not_nans, torch.tensor([0], dtype=torch.float))
 
+    def test_compute_surface_dice_subvoxel(self):
+        mask_gt, mask_pred = torch.zeros(1, 1, 128, 128, 128), torch.zeros(1, 1, 128, 128, 128)
+        mask_gt[0, 0, 50, 60, 70] = 1
+        res = compute_surface_dice(
+            mask_pred, mask_gt, [1.0], include_background=True, spacing=(3, 2, 1), use_subvoxels=True
+        )
+        assert_allclose(res, 0.0, type_test=False)
+        mask_gt[0, 0, 50, 60, 70] = 0
+        mask_pred[0, 0, 50, 60, 72] = 1
+        res = compute_surface_dice(
+            mask_pred, mask_gt, [1.0], include_background=True, spacing=(3, 2, 1), use_subvoxels=True
+        )
+        assert_allclose(res, 0.0, type_test=False)
+        mask_gt[0, 0, 50, 60, 70] = 1
+        mask_pred[0, 0, 50, 60, 72] = 1
+        res = compute_surface_dice(
+            mask_pred, mask_gt, [1.0], include_background=True, spacing=(3, 2, 1), use_subvoxels=True
+        )
+        assert_allclose(res, 0.5, type_test=False)
+
+        d = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+        mask_gt, mask_pred = torch.zeros(1, 1, 100, 100, 100, device=d), torch.zeros(1, 1, 100, 100, 100, device=d)
+        mask_gt[0, 0, 0:50, :, :] = 1
+        mask_pred[0, 0, 0:51, :, :] = 1
+        res = compute_surface_dice(
+            mask_pred, mask_gt, [1.0], include_background=True, spacing=(2, 1, 1), use_subvoxels=True
+        )
+        assert_allclose(res, 0.836145, type_test=False, atol=1e-3, rtol=1e-3)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_surface_distance.py` & `monai-weekly-1.3.dev2328/tests/test_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_swin_unetr.py` & `monai-weekly-1.3.dev2328/tests/test_swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_synthetic.py` & `monai-weekly-1.3.dev2328/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_tciadataset.py` & `monai-weekly-1.3.dev2328/tests/test_tciadataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_testtimeaugmentation.py` & `monai-weekly-1.3.dev2328/tests/test_testtimeaugmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_text_encoding.py` & `monai-weekly-1.3.dev2328/tests/test_text_encoding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_thread_buffer.py` & `monai-weekly-1.3.dev2328/tests/test_thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_threadcontainer.py` & `monai-weekly-1.3.dev2328/tests/test_threadcontainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_threshold_intensity.py` & `monai-weekly-1.3.dev2328/tests/test_threshold_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_threshold_intensityd.py` & `monai-weekly-1.3.dev2328/tests/test_threshold_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_timedcall_dist.py` & `monai-weekly-1.3.dev2328/tests/test_timedcall_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_contiguous.py` & `monai-weekly-1.3.dev2328/tests/test_to_contiguous.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_cupy.py` & `monai-weekly-1.3.dev2328/tests/test_to_cupy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_cupyd.py` & `monai-weekly-1.3.dev2328/tests/test_to_cupyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_device.py` & `monai-weekly-1.3.dev2328/tests/test_to_device.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_deviced.py` & `monai-weekly-1.3.dev2328/tests/test_to_deviced.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_from_meta_tensord.py` & `monai-weekly-1.3.dev2328/tests/test_to_from_meta_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_numpy.py` & `monai-weekly-1.3.dev2328/tests/test_to_numpy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_numpyd.py` & `monai-weekly-1.3.dev2328/tests/test_to_numpyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_onehot.py` & `monai-weekly-1.3.dev2328/tests/test_to_onehot.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_pil.py` & `monai-weekly-1.3.dev2328/tests/test_to_pil.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_pild.py` & `monai-weekly-1.3.dev2328/tests/test_to_pild.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_tensor.py` & `monai-weekly-1.3.dev2328/tests/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_to_tensord.py` & `monai-weekly-1.3.dev2328/tests/test_to_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_torchscript_utils.py` & `monai-weekly-1.3.dev2328/tests/test_torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_torchvision.py` & `monai-weekly-1.3.dev2328/tests/test_torchvision.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_torchvision_fc_model.py` & `monai-weekly-1.3.dev2328/tests/test_torchvision_fc_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_torchvisiond.py` & `monai-weekly-1.3.dev2328/tests/test_torchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_traceable_transform.py` & `monai-weekly-1.3.dev2328/tests/test_traceable_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_train_mode.py` & `monai-weekly-1.3.dev2328/tests/test_train_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_trainable_bilateral.py` & `monai-weekly-1.3.dev2328/tests/test_trainable_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_trainable_joint_bilateral.py` & `monai-weekly-1.3.dev2328/tests/test_trainable_joint_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_transchex.py` & `monai-weekly-1.3.dev2328/tests/test_transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_transform.py` & `monai-weekly-1.3.dev2328/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_transformerblock.py` & `monai-weekly-1.3.dev2328/tests/test_transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_transpose.py` & `monai-weekly-1.3.dev2328/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_transposed.py` & `monai-weekly-1.3.dev2328/tests/test_transposed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_tversky_loss.py` & `monai-weekly-1.3.dev2328/tests/test_tversky_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_unet.py` & `monai-weekly-1.3.dev2328/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_unetr.py` & `monai-weekly-1.3.dev2328/tests/test_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_unetr_block.py` & `monai-weekly-1.3.dev2328/tests/test_unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_unified_focal_loss.py` & `monai-weekly-1.3.dev2328/tests/test_unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_upsample_block.py` & `monai-weekly-1.3.dev2328/tests/test_upsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_utils_pytorch_numpy_unification.py` & `monai-weekly-1.3.dev2328/tests/test_utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_varautoencoder.py` & `monai-weekly-1.3.dev2328/tests/test_varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_varnet.py` & `monai-weekly-1.3.dev2328/tests/test_varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_version_leq.py` & `monai-weekly-1.3.dev2328/tests/test_version_leq.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_video_datasets.py` & `monai-weekly-1.3.dev2328/tests/test_video_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_vis_cam.py` & `monai-weekly-1.3.dev2328/tests/test_vis_cam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_vis_gradbased.py` & `monai-weekly-1.3.dev2328/tests/test_vis_gradbased.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_vis_gradcam.py` & `monai-weekly-1.3.dev2328/tests/test_vis_gradcam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_vit.py` & `monai-weekly-1.3.dev2328/tests/test_vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_vitautoenc.py` & `monai-weekly-1.3.dev2328/tests/test_vitautoenc.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import unittest
 
 import torch
 from parameterized import parameterized
 
 from monai.networks import eval_mode
 from monai.networks.nets.vitautoenc import ViTAutoEnc
-from tests.utils import skip_if_windows
+from tests.utils import skip_if_quick, skip_if_windows
 
 TEST_CASE_Vitautoenc = []
 for in_channels in [1, 4]:
     for img_size in [64, 96, 128]:
         for patch_size in [16]:
             for pos_embed in ["conv", "perceptron"]:
                 for nd in [2, 3]:
@@ -60,15 +60,16 @@
         },
         (2, 1, 512, 512, 32),
         (2, 1, 512, 512, 32),
     ]
 )
 
 
-class TestPatchEmbeddingBlock(unittest.TestCase):
+@skip_if_quick
+class TestVitAutoenc(unittest.TestCase):
     def setUp(self):
         self.threads = torch.get_num_threads()
         torch.set_num_threads(4)
 
     def tearDown(self):
         torch.set_num_threads(self.threads)
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_vnet.py` & `monai-weekly-1.3.dev2328/tests/test_vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_vote_ensemble.py` & `monai-weekly-1.3.dev2328/tests/test_vote_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_vote_ensembled.py` & `monai-weekly-1.3.dev2328/tests/test_vote_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_warp.py` & `monai-weekly-1.3.dev2328/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_watershed.py` & `monai-weekly-1.3.dev2328/tests/test_watershed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_watershedd.py` & `monai-weekly-1.3.dev2328/tests/test_watershedd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_weight_init.py` & `monai-weekly-1.3.dev2328/tests/test_weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_weighted_random_sampler_dist.py` & `monai-weekly-1.3.dev2328/tests/test_weighted_random_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_with_allow_missing_keys.py` & `monai-weekly-1.3.dev2328/tests/test_with_allow_missing_keys.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_write_metrics_reports.py` & `monai-weekly-1.3.dev2328/tests/test_write_metrics_reports.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_wsi_sliding_window_splitter.py` & `monai-weekly-1.3.dev2328/tests/test_wsi_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_wsireader.py` & `monai-weekly-1.3.dev2328/tests/test_wsireader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_zarr_avg_merger.py` & `monai-weekly-1.3.dev2328/tests/test_zarr_avg_merger.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,28 +136,26 @@
         (TENSOR_4x4[..., :2, 2:], (0, 2)),
         (TENSOR_4x4[..., 2:, :2], (2, 0)),
         (TENSOR_4x4[..., 2:, 2:], (2, 2)),
     ],
     TENSOR_4x4,
 ]
 
-
 # shape larger than what is covered by patches
 TEST_CASE_9_LARGER_SHAPE = [
     dict(merged_shape=(2, 3, 4, 6)),
     [
         (TENSOR_4x4[..., :2, :2], (0, 0)),
         (TENSOR_4x4[..., :2, 2:], (0, 2)),
         (TENSOR_4x4[..., 2:, :2], (2, 0)),
         (TENSOR_4x4[..., 2:, 2:], (2, 2)),
     ],
     pad(TENSOR_4x4, (0, 2), value=float("nan")),
 ]
 
-
 # explicit directory store
 TEST_CASE_10_DIRECTORY_STORE = [
     dict(merged_shape=TENSOR_4x4.shape, store=zarr.storage.DirectoryStore("test.zarr")),
     [
         (TENSOR_4x4[..., :2, :2], (0, 0)),
         (TENSOR_4x4[..., :2, 2:], (0, 2)),
         (TENSOR_4x4[..., 2:, :2], (2, 0)),
@@ -179,28 +177,26 @@
         (TENSOR_4x4[..., :2, 2:], (0, 2)),
         (TENSOR_4x4[..., 2:, :2], (2, 0)),
         (TENSOR_4x4[..., 2:, 2:], (2, 2)),
     ],
     TENSOR_4x4,
 ]
 
-
 # explicit chunk size
 TEST_CASE_12_CHUNKS = [
     dict(merged_shape=TENSOR_4x4.shape, chunks=(1, 1, 2, 2)),
     [
         (TENSOR_4x4[..., :2, :2], (0, 0)),
         (TENSOR_4x4[..., :2, 2:], (0, 2)),
         (TENSOR_4x4[..., 2:, :2], (2, 0)),
         (TENSOR_4x4[..., 2:, 2:], (2, 2)),
     ],
     TENSOR_4x4,
 ]
 
-
 # test for LZ4 compressor
 TEST_CASE_13_COMPRESSOR_LZ4 = [
     dict(merged_shape=TENSOR_4x4.shape, compressor="LZ4"),
     [
         (TENSOR_4x4[..., :2, :2], (0, 0)),
         (TENSOR_4x4[..., :2, 2:], (0, 2)),
         (TENSOR_4x4[..., 2:, :2], (2, 0)),
@@ -229,15 +225,14 @@
         (TENSOR_4x4[..., :2, 2:], (0, 2)),
         (TENSOR_4x4[..., 2:, :2], (2, 0)),
         (TENSOR_4x4[..., 2:, 2:], (2, 2)),
     ],
     TENSOR_4x4,
 ]
 
-
 # test with thread locking
 TEST_CASE_16_WITH_LOCK = [
     dict(merged_shape=TENSOR_4x4.shape, thread_locking=True),
     [
         (TENSOR_4x4[..., :2, :2], (0, 0)),
         (TENSOR_4x4[..., :2, 2:], (0, 2)),
         (TENSOR_4x4[..., 2:, :2], (2, 0)),
```

### Comparing `monai-weekly-1.3.dev2327/tests/test_zipdataset.py` & `monai-weekly-1.3.dev2328/tests/test_zipdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_zoom.py` & `monai-weekly-1.3.dev2328/tests/test_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_zoom_affine.py` & `monai-weekly-1.3.dev2328/tests/test_zoom_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/tests/test_zoomd.py` & `monai-weekly-1.3.dev2328/tests/test_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2327/versioneer.py` & `monai-weekly-1.3.dev2328/versioneer.py`

 * *Files identical despite different names*

