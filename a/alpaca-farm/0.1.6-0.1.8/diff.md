# Comparing `tmp/alpaca_farm-0.1.6.tar.gz` & `tmp/alpaca_farm-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_farm-0.1.6.tar", last modified: Fri Jun 23 08:08:23 2023, max compression
+gzip compressed data, was "alpaca_farm-0.1.8.tar", last modified: Sun Jul  9 01:33:12 2023, max compression
```

## Comparing `alpaca_farm-0.1.6.tar` & `alpaca_farm-0.1.8.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.609046 alpaca_farm-0.1.6/
--rw-r--r--   0 xuechenli   (501) staff       (20)    11410 2023-05-27 23:57:21.000000 alpaca_farm-0.1.6/LICENSE
--rw-r--r--   0 xuechenli   (501) staff       (20)       64 2023-06-11 03:50:42.000000 alpaca_farm-0.1.6/MANIFEST.in
--rw-r--r--   0 xuechenli   (501) staff       (20)    16786 2023-06-23 08:08:23.608833 alpaca_farm-0.1.6/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)    16132 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/README.md
--rw-r--r--   0 xuechenli   (501) staff       (20)       38 2023-06-23 08:08:23.609084 alpaca_farm-0.1.6/setup.cfg
--rw-r--r--   0 xuechenli   (501) staff       (20)     2599 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/setup.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.591823 alpaca_farm-0.1.6/src/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.597614 alpaca_farm-0.1.6/src/alpaca_farm/
--rw-r--r--   0 xuechenli   (501) staff       (20)      602 2023-06-23 08:07:51.000000 alpaca_farm-0.1.6/src/alpaca_farm/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1190 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/accelerate_patch.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.598757 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/
--rw-r--r--   0 xuechenli   (501) staff       (20)      640 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/__init__.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.592186 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.604102 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     1670 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6020 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5869 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     2605 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     2475 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3852 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3721 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3660 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3423 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7125 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6849 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7073 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6797 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6991 2023-06-10 06:22:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7266 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     1057 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     1016 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     4067 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3969 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6289 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5932 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5559 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5370 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.604616 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)     7664 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7373 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      500 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.604816 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/test/
--rw-r--r--   0 xuechenli   (501) staff       (20)      446 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/test/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     7108 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/eval.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13428 2023-06-12 18:21:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/common.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2652 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/constants.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1565 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/data_postprocessor.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    21184 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/data_preprocessor.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4527 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/data_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2532 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/distributed_utils.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.605680 alpaca_farm-0.1.6/src/alpaca_farm/flash_models/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/flash_models/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1492 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/flash_models/apex_patch.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13316 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/flash_models/flash_llama.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11476 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/flash_models/flash_opt.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1741 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/flash_models/tensor_ops.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.606251 alpaca_farm-0.1.6/src/alpaca_farm/inference/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/inference/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    16279 2023-06-11 21:47:42.000000 alpaca_farm-0.1.6/src/alpaca_farm/inference/decode.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7147 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/inference/score.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3372 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/logging.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.606829 alpaca_farm-0.1.6/src/alpaca_farm/models/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/models/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2523 2023-06-11 04:26:11.000000 alpaca_farm-0.1.6/src/alpaca_farm/models/reward_model.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     8003 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/models/rl_models.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11576 2023-06-23 08:07:43.000000 alpaca_farm-0.1.6/src/alpaca_farm/openai_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3208 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/reward_modeling_trainer.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.607962 alpaca_farm-0.1.6/src/alpaca_farm/rl/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2054 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/kl_controller.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    22890 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/ppo_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7524 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/ppo_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    21692 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/quark_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7932 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/quark_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13749 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/rl/rl_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3088 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/torch_ops.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3507 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/src/alpaca_farm/trainer_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1211 2023-06-11 22:43:54.000000 alpaca_farm-0.1.6/src/alpaca_farm/types.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     6767 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/src/alpaca_farm/utils.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.598364 alpaca_farm-0.1.6/src/alpaca_farm.egg-info/
--rw-r--r--   0 xuechenli   (501) staff       (20)    16786 2023-06-23 08:08:23.000000 alpaca_farm-0.1.6/src/alpaca_farm.egg-info/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)     4168 2023-06-23 08:08:23.000000 alpaca_farm-0.1.6/src/alpaca_farm.egg-info/SOURCES.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)        1 2023-06-23 08:08:23.000000 alpaca_farm-0.1.6/src/alpaca_farm.egg-info/dependency_links.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      307 2023-06-23 08:08:23.000000 alpaca_farm-0.1.6/src/alpaca_farm.egg-info/requires.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)       12 2023-06-23 08:08:23.000000 alpaca_farm-0.1.6/src/alpaca_farm.egg-info/top_level.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-23 08:08:23.608603 alpaca_farm-0.1.6/tests/
--rw-r--r--   0 xuechenli   (501) staff       (20)    12263 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/tests/test_flash_llama.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     8351 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/tests/test_flash_opt.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      899 2023-05-23 16:11:47.000000 alpaca_farm-0.1.6/tests/test_torch_ops.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      581 2023-06-12 23:52:33.000000 alpaca_farm-0.1.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.178722 alpaca_farm-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16786 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 01:33:12.178722 alpaca_farm-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.166723 alpaca_farm-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.166723 alpaca_farm-0.1.8/src/alpaca_farm/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-09 01:33:00.000000 alpaca_farm-0.1.8/src/alpaca_farm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/accelerate_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.170723 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.166723 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.170723 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/test/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/data_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/distributed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/src/alpaca_farm/flash_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/flash_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/flash_models/apex_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/flash_models/flash_llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11476 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/flash_models/flash_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/flash_models/tensor_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/src/alpaca_farm/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/inference/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/inference/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/src/alpaca_farm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/models/reward_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/models/rl_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/openai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/reward_modeling_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/src/alpaca_farm/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/kl_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/ppo_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/ppo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21692 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/quark_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/quark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/rl/rl_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/src/alpaca_farm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.170723 alpaca_farm-0.1.8/src/alpaca_farm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16786 2023-07-09 01:33:12.000000 alpaca_farm-0.1.8/src/alpaca_farm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-09 01:33:12.000000 alpaca_farm-0.1.8/src/alpaca_farm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 01:33:12.000000 alpaca_farm-0.1.8/src/alpaca_farm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-09 01:33:12.000000 alpaca_farm-0.1.8/src/alpaca_farm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 01:33:12.000000 alpaca_farm-0.1.8/src/alpaca_farm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:33:12.174723 alpaca_farm-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/tests/test_flash_llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/tests/test_flash_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/tests/test_torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-09 01:32:51.000000 alpaca_farm-0.1.8/tests/test_utils.py
```

### Comparing `alpaca_farm-0.1.6/LICENSE` & `alpaca_farm-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/PKG-INFO` & `alpaca_farm-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_farm
-Version: 0.1.6
+Version: 0.1.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `alpaca_farm-0.1.6/README.md` & `alpaca_farm-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/__init__.py` & `alpaca_farm-0.1.8/src/alpaca_farm/flash_models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,9 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-__version__ = "0.1.6"
```

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/accelerate_patch.py` & `alpaca_farm-0.1.8/src/alpaca_farm/accelerate_patch.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/__init__.py` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/auto_annotations/eval.py` & `alpaca_farm-0.1.8/src/alpaca_farm/auto_annotations/eval.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/common.py` & `alpaca_farm-0.1.8/src/alpaca_farm/common.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/constants.py` & `alpaca_farm-0.1.8/src/alpaca_farm/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/data_postprocessor.py` & `alpaca_farm-0.1.8/src/alpaca_farm/data_postprocessor.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/data_preprocessor.py` & `alpaca_farm-0.1.8/src/alpaca_farm/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/data_utils.py` & `alpaca_farm-0.1.8/src/alpaca_farm/data_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/distributed_utils.py` & `alpaca_farm-0.1.8/src/alpaca_farm/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/flash_models/__init__.py` & `alpaca_farm-0.1.8/src/alpaca_farm/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/flash_models/apex_patch.py` & `alpaca_farm-0.1.8/src/alpaca_farm/flash_models/apex_patch.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/flash_models/flash_llama.py` & `alpaca_farm-0.1.8/src/alpaca_farm/flash_models/flash_llama.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/flash_models/flash_opt.py` & `alpaca_farm-0.1.8/src/alpaca_farm/flash_models/flash_opt.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/flash_models/tensor_ops.py` & `alpaca_farm-0.1.8/src/alpaca_farm/flash_models/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/inference/__init__.py` & `alpaca_farm-0.1.8/src/alpaca_farm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/inference/decode.py` & `alpaca_farm-0.1.8/src/alpaca_farm/inference/decode.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/inference/score.py` & `alpaca_farm-0.1.8/src/alpaca_farm/inference/score.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/logging.py` & `alpaca_farm-0.1.8/src/alpaca_farm/logging.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/models/__init__.py` & `alpaca_farm-0.1.8/src/alpaca_farm/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/models/reward_model.py` & `alpaca_farm-0.1.8/src/alpaca_farm/models/reward_model.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/models/rl_models.py` & `alpaca_farm-0.1.8/src/alpaca_farm/models/rl_models.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/openai_utils.py` & `alpaca_farm-0.1.8/src/alpaca_farm/openai_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/reward_modeling_trainer.py` & `alpaca_farm-0.1.8/src/alpaca_farm/reward_modeling_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/rl/__init__.py` & `alpaca_farm-0.1.8/src/alpaca_farm/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,7 +7,9 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+__version__ = '0.1.8'
```

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/rl/kl_controller.py` & `alpaca_farm-0.1.8/src/alpaca_farm/rl/kl_controller.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/rl/ppo_trainer.py` & `alpaca_farm-0.1.8/src/alpaca_farm/rl/ppo_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/rl/ppo_utils.py` & `alpaca_farm-0.1.8/src/alpaca_farm/rl/ppo_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/rl/quark_trainer.py` & `alpaca_farm-0.1.8/src/alpaca_farm/rl/quark_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/rl/quark_utils.py` & `alpaca_farm-0.1.8/src/alpaca_farm/rl/quark_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/rl/rl_trainer.py` & `alpaca_farm-0.1.8/src/alpaca_farm/rl/rl_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                     if self.accelerator.sync_gradients:
                         # Gradient norm almost blows up at some point, but stabilizes eventually, even w/o clipping.
                         if self.args.max_grad_norm is not None:
                             self.accelerator.clip_grad_norm_(self.policy.parameters(), self.args.max_grad_norm)
                         stats_for_this_step["loss/grad_norm"] = self._compute_grad_norm()
                         stats_list.append(stats_for_this_step)
                     self.optimizer.step()
-                    self.policy.zero_grad(set_to_none=True)
+                    self.optimizer.zero_grad(set_to_none=True)
         return common.merge_dict(stats_list, torch.stack)  # list of dict -> dict: str -> 1-D tensor
 
     def step(self, train_dataloader, step_idx: int):
         queries_batches = [next(train_dataloader) for _ in range(self.args.rollout_accumulation_steps)]
         rollouts = self.rollout(queries_batches)
         train_stats = self.step_with_rollouts(rollouts)
         if self.lr_scheduler is not None:
```

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/torch_ops.py` & `alpaca_farm-0.1.8/src/alpaca_farm/torch_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/trainer_utils.py` & `alpaca_farm-0.1.8/src/alpaca_farm/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/types.py` & `alpaca_farm-0.1.8/src/alpaca_farm/types.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm/utils.py` & `alpaca_farm-0.1.8/src/alpaca_farm/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm.egg-info/PKG-INFO` & `alpaca_farm-0.1.8/src/alpaca_farm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-farm
-Version: 0.1.6
+Version: 0.1.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `alpaca_farm-0.1.6/src/alpaca_farm.egg-info/SOURCES.txt` & `alpaca_farm-0.1.8/src/alpaca_farm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.py
 src/alpaca_farm/__init__.py
 src/alpaca_farm/accelerate_patch.py
 src/alpaca_farm/common.py
 src/alpaca_farm/constants.py
 src/alpaca_farm/data_postprocessor.py
 src/alpaca_farm/data_preprocessor.py
```

### Comparing `alpaca_farm-0.1.6/tests/test_flash_llama.py` & `alpaca_farm-0.1.8/tests/test_flash_llama.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/tests/test_flash_opt.py` & `alpaca_farm-0.1.8/tests/test_flash_opt.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/tests/test_torch_ops.py` & `alpaca_farm-0.1.8/tests/test_torch_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.6/tests/test_utils.py` & `alpaca_farm-0.1.8/tests/test_utils.py`

 * *Files identical despite different names*

