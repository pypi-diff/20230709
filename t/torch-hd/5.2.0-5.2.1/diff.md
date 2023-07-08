# Comparing `tmp/torch-hd-5.2.0.tar.gz` & `tmp/torch-hd-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-hd-5.2.0.tar", last modified: Fri Jul  7 22:49:30 2023, max compression
+gzip compressed data, was "torch-hd-5.2.1.tar", last modified: Sat Jul  8 22:00:35 2023, max compression
```

## Comparing `torch-hd-5.2.0.tar` & `torch-hd-5.2.1.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.546485 torch-hd-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-07 22:49:20.000000 torch-hd-5.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-07 22:49:30.546485 torch-hd-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-07 22:49:20.000000 torch-hd-5.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 22:49:30.546485 torch-hd-5.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-07 22:49:20.000000 torch-hd-5.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.526485 torch-hd-5.2.0/torch_hd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-07 22:49:30.000000 torch-hd-5.2.0/torch_hd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-07 22:49:30.000000 torch-hd-5.2.0/torch_hd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:49:30.000000 torch-hd-5.2.0/torch_hd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 22:49:30.000000 torch-hd-5.2.0/torch_hd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 22:49:30.000000 torch-hd-5.2.0/torch_hd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.530485 torch-hd-5.2.0/torchhd/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.546485 torch-hd-5.2.0/torchhd/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/abalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/acute_inflammation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/acute_nephritis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/adult.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/airfoil_self_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/annealing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/arrhythmia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/audiology_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/balance_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/balloons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/beijing_air_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/blood.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/breast_cancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/breast_cancer_wisc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/breast_cancer_wisc_diag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/breast_cancer_wisc_prog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/breast_tissue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/car.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/cardiotocography_10clases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/cardiotocography_3clases.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ccpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/chess_krvk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/chess_krvkp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/congressional_voting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/conn_bench_sonar_mines_rocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/conn_bench_vowel_deterding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/connect_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/contrac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/credit_approval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/cylinder_bands.py
--rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/dermatology.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/echocardiogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ecoli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/emg_hand_gestures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/energy_y1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/energy_y2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/european_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/fertility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/glass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/haberman_survival.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/hayes_roth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/heart_cleveland.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/heart_hungarian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/heart_switzerland.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/heart_va.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/hepatitis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/hill_valley.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/horse_colic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ilpd_indian_liver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/image_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ionosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/isolet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/led_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/letter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/libras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/low_res_spect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/lung_cancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/lymphography.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/mammographic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/miniboone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/molec_biol_promoter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/molec_biol_splice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/monks_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/monks_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/monks_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/mushroom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/musk_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/musk_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/nursery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/oocytes_merluccius_nucleus_4d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/oocytes_merluccius_states_2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/oocytes_trisopterus_nucleus_2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/oocytes_trisopterus_states_5b.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/optical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ozone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/page_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pamap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/parkinsons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pendigits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pima.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_rel_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_t_or_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/planning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/plant_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/plant_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/plant_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/post_operative.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/primary_tumor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ringnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/semeion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/soybean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/spambase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/spect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/spectf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_australian_credit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_german_credit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_heart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_landsat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_shuttle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/statlog_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/steel_plates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/synthetic_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/teaching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/thyroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/titanic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/trains.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/twonorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/ucihar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/vertebral_column_2clases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/vertebral_column_3clases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/wall_following.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/waveform_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/wine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/wine_quality_red.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/wine_quality_white.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/yeast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/datasets/zoo.py
--rw-r--r--   0 runner    (1001) docker     (123)    48690 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)    59891 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    38319 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.546485 torch-hd-5.2.0/torchhd/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tensors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tensors/bsc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tensors/fhrr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tensors/hrr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tensors/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.526485 torch-hd-5.2.0/torchhd/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.546485 torch-hd-5.2.0/torchhd/tests/basis_hv/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/test_base_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/test_circular_hv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/test_empty_hv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/test_identity_hv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/test_level_hv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/basis_hv/test_random_hv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:49:30.546485 torch-hd-5.2.0/torchhd/tests/structures/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_distinct_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_hashtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_multiset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/tests/structures/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-07 22:49:20.000000 torch-hd-5.2.0/torchhd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.664175 torch-hd-5.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-08 22:00:25.000000 torch-hd-5.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-08 22:00:35.664175 torch-hd-5.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-08 22:00:25.000000 torch-hd-5.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 22:00:35.664175 torch-hd-5.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-08 22:00:25.000000 torch-hd-5.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.628174 torch-hd-5.2.1/torch_hd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-08 22:00:35.000000 torch-hd-5.2.1/torch_hd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-08 22:00:35.000000 torch-hd-5.2.1/torch_hd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:00:35.000000 torch-hd-5.2.1/torch_hd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-08 22:00:35.000000 torch-hd-5.2.1/torch_hd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 22:00:35.000000 torch-hd-5.2.1/torch_hd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.628174 torch-hd-5.2.1/torchhd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.656175 torch-hd-5.2.1/torchhd/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/abalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/acute_inflammation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/acute_nephritis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/adult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/airfoil_self_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/annealing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/arrhythmia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/audiology_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/balance_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/beijing_air_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/blood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/breast_cancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/breast_cancer_wisc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/breast_cancer_wisc_diag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/breast_cancer_wisc_prog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/breast_tissue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/cardiotocography_10clases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/cardiotocography_3clases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ccpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/chess_krvk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/chess_krvkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/congressional_voting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/conn_bench_sonar_mines_rocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/conn_bench_vowel_deterding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/connect_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/contrac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/credit_approval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/cylinder_bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/dermatology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/echocardiogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ecoli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/emg_hand_gestures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/energy_y1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/energy_y2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/european_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/fertility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/glass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/haberman_survival.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/hayes_roth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/heart_cleveland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/heart_hungarian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/heart_switzerland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/heart_va.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/hepatitis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/hill_valley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/horse_colic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ilpd_indian_liver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/image_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ionosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/isolet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/led_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/letter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/libras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/low_res_spect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/lung_cancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/lymphography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/mammographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/miniboone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/molec_biol_promoter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/molec_biol_splice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/monks_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/monks_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/monks_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/mushroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/musk_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/musk_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/nursery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/oocytes_merluccius_nucleus_4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/oocytes_merluccius_states_2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/oocytes_trisopterus_nucleus_2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/oocytes_trisopterus_states_5b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/optical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ozone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/page_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pamap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/parkinsons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pendigits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_rel_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_t_or_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/planning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/plant_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/plant_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/plant_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/post_operative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/primary_tumor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ringnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/semeion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/soybean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/spambase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/spect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/spectf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_australian_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_german_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_heart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_landsat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_shuttle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/steel_plates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/synthetic_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/teaching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/thyroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/trains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/twonorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ucihar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/vertebral_column_2clases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/vertebral_column_3clases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/wall_following.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/waveform_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/wine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/wine_quality_red.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/wine_quality_white.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/yeast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/zoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49027 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59891 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38319 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.660174 torch-hd-5.2.1/torchhd/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tensors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tensors/bsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tensors/fhrr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tensors/hrr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tensors/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.624174 torch-hd-5.2.1/torchhd/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.660174 torch-hd-5.2.1/torchhd/tests/basis_hv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/test_base_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/test_circular_hv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/test_empty_hv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/test_identity_hv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/test_level_hv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/test_random_hv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.664175 torch-hd-5.2.1/torchhd/tests/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_distinct_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_hashtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_multiset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/version.py
```

### Comparing `torch-hd-5.2.0/LICENSE` & `torch-hd-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/PKG-INFO` & `torch-hd-5.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-hd
-Version: 5.2.0
+Version: 5.2.1
 Summary: Torchhd is a Python library for Hyperdimensional Computing and Vector Symbolic Architectures
 Home-page: https://github.com/hyperdimensional-computing/torchhd
 License: MIT
 Project-URL: Source, https://github.com/hyperdimensional-computing/torchhd
 Project-URL: Documentation, https://torchhd.readthedocs.io
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torch-hd Version: 5.2.0 Summary: Torchhd is a
+Metadata-Version: 2.1 Name: torch-hd Version: 5.2.1 Summary: Torchhd is a
 Python library for Hyperdimensional Computing and Vector Symbolic Architectures
 Home-page: https://github.com/hyperdimensional-computing/torchhd License: MIT
 Project-URL: Source, https://github.com/hyperdimensional-computing/torchhd
 Project-URL: Documentation, https://torchhd.readthedocs.io Requires-Python:
 >=3.6, <4 Description-Content-Type: text/markdown License-File: LICENSE
   [GitHub_license] [pypi_version] [conda_version] [tests_status][PRs Welcome]
                                 [Torchhd_logo]
```

### Comparing `torch-hd-5.2.0/README.md` & `torch-hd-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/setup.py` & `torch-hd-5.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torch_hd.egg-info/PKG-INFO` & `torch-hd-5.2.1/torch_hd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-hd
-Version: 5.2.0
+Version: 5.2.1
 Summary: Torchhd is a Python library for Hyperdimensional Computing and Vector Symbolic Architectures
 Home-page: https://github.com/hyperdimensional-computing/torchhd
 License: MIT
 Project-URL: Source, https://github.com/hyperdimensional-computing/torchhd
 Project-URL: Documentation, https://torchhd.readthedocs.io
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torch-hd Version: 5.2.0 Summary: Torchhd is a
+Metadata-Version: 2.1 Name: torch-hd Version: 5.2.1 Summary: Torchhd is a
 Python library for Hyperdimensional Computing and Vector Symbolic Architectures
 Home-page: https://github.com/hyperdimensional-computing/torchhd License: MIT
 Project-URL: Source, https://github.com/hyperdimensional-computing/torchhd
 Project-URL: Documentation, https://torchhd.readthedocs.io Requires-Python:
 >=3.6, <4 Description-Content-Type: text/markdown License-File: LICENSE
   [GitHub_license] [pypi_version] [conda_version] [tests_status][PRs Welcome]
                                 [Torchhd_logo]
```

### Comparing `torch-hd-5.2.0/torch_hd.egg-info/SOURCES.txt` & `torch-hd-5.2.1/torch_hd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/__init__.py` & `torch-hd-5.2.1/torchhd/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/__init__.py` & `torch-hd-5.2.1/torchhd/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/abalone.py` & `torch-hd-5.2.1/torchhd/datasets/abalone.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/acute_inflammation.py` & `torch-hd-5.2.1/torchhd/datasets/acute_inflammation.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/acute_nephritis.py` & `torch-hd-5.2.1/torchhd/datasets/acute_nephritis.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/adult.py` & `torch-hd-5.2.1/torchhd/datasets/adult.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/airfoil_self_noise.py` & `torch-hd-5.2.1/torchhd/datasets/airfoil_self_noise.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/annealing.py` & `torch-hd-5.2.1/torchhd/datasets/annealing.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/arrhythmia.py` & `torch-hd-5.2.1/torchhd/datasets/arrhythmia.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/audiology_std.py` & `torch-hd-5.2.1/torchhd/datasets/audiology_std.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/balance_scale.py` & `torch-hd-5.2.1/torchhd/datasets/balance_scale.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/balloons.py` & `torch-hd-5.2.1/torchhd/datasets/balloons.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/bank.py` & `torch-hd-5.2.1/torchhd/datasets/bank.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/beijing_air_quality.py` & `torch-hd-5.2.1/torchhd/datasets/beijing_air_quality.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/blood.py` & `torch-hd-5.2.1/torchhd/datasets/blood.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/breast_cancer.py` & `torch-hd-5.2.1/torchhd/datasets/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/breast_cancer_wisc.py` & `torch-hd-5.2.1/torchhd/datasets/breast_cancer_wisc.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/breast_cancer_wisc_diag.py` & `torch-hd-5.2.1/torchhd/datasets/breast_cancer_wisc_diag.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/breast_cancer_wisc_prog.py` & `torch-hd-5.2.1/torchhd/datasets/breast_cancer_wisc_prog.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/breast_tissue.py` & `torch-hd-5.2.1/torchhd/datasets/breast_tissue.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/car.py` & `torch-hd-5.2.1/torchhd/datasets/car.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/cardiotocography_10clases.py` & `torch-hd-5.2.1/torchhd/datasets/cardiotocography_10clases.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/cardiotocography_3clases.py` & `torch-hd-5.2.1/torchhd/datasets/cardiotocography_3clases.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/ccpp.py` & `torch-hd-5.2.1/torchhd/datasets/ccpp.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/chess_krvk.py` & `torch-hd-5.2.1/torchhd/datasets/chess_krvk.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/chess_krvkp.py` & `torch-hd-5.2.1/torchhd/datasets/chess_krvkp.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/congressional_voting.py` & `torch-hd-5.2.1/torchhd/datasets/congressional_voting.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/conn_bench_sonar_mines_rocks.py` & `torch-hd-5.2.1/torchhd/datasets/conn_bench_sonar_mines_rocks.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/conn_bench_vowel_deterding.py` & `torch-hd-5.2.1/torchhd/datasets/conn_bench_vowel_deterding.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/connect_4.py` & `torch-hd-5.2.1/torchhd/datasets/connect_4.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/contrac.py` & `torch-hd-5.2.1/torchhd/datasets/contrac.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/credit_approval.py` & `torch-hd-5.2.1/torchhd/datasets/credit_approval.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/cylinder_bands.py` & `torch-hd-5.2.1/torchhd/datasets/cylinder_bands.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/dataset.py` & `torch-hd-5.2.1/torchhd/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/dermatology.py` & `torch-hd-5.2.1/torchhd/datasets/dermatology.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/echocardiogram.py` & `torch-hd-5.2.1/torchhd/datasets/echocardiogram.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/ecoli.py` & `torch-hd-5.2.1/torchhd/datasets/ecoli.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/emg_hand_gestures.py` & `torch-hd-5.2.1/torchhd/datasets/emg_hand_gestures.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/energy_y1.py` & `torch-hd-5.2.1/torchhd/datasets/energy_y1.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/energy_y2.py` & `torch-hd-5.2.1/torchhd/datasets/energy_y2.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/european_languages.py` & `torch-hd-5.2.1/torchhd/datasets/european_languages.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/fertility.py` & `torch-hd-5.2.1/torchhd/datasets/fertility.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/flags.py` & `torch-hd-5.2.1/torchhd/datasets/flags.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/glass.py` & `torch-hd-5.2.1/torchhd/datasets/glass.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/haberman_survival.py` & `torch-hd-5.2.1/torchhd/datasets/haberman_survival.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/hayes_roth.py` & `torch-hd-5.2.1/torchhd/datasets/hayes_roth.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/heart_cleveland.py` & `torch-hd-5.2.1/torchhd/datasets/heart_cleveland.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/heart_hungarian.py` & `torch-hd-5.2.1/torchhd/datasets/heart_hungarian.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/heart_switzerland.py` & `torch-hd-5.2.1/torchhd/datasets/heart_switzerland.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/heart_va.py` & `torch-hd-5.2.1/torchhd/datasets/heart_va.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/hepatitis.py` & `torch-hd-5.2.1/torchhd/datasets/hepatitis.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/hill_valley.py` & `torch-hd-5.2.1/torchhd/datasets/hill_valley.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/horse_colic.py` & `torch-hd-5.2.1/torchhd/datasets/horse_colic.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/ilpd_indian_liver.py` & `torch-hd-5.2.1/torchhd/datasets/ilpd_indian_liver.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/image_segmentation.py` & `torch-hd-5.2.1/torchhd/datasets/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/ionosphere.py` & `torch-hd-5.2.1/torchhd/datasets/ionosphere.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/iris.py` & `torch-hd-5.2.1/torchhd/datasets/iris.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/isolet.py` & `torch-hd-5.2.1/torchhd/datasets/isolet.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/led_display.py` & `torch-hd-5.2.1/torchhd/datasets/led_display.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/lenses.py` & `torch-hd-5.2.1/torchhd/datasets/lenses.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/letter.py` & `torch-hd-5.2.1/torchhd/datasets/letter.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/libras.py` & `torch-hd-5.2.1/torchhd/datasets/libras.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/low_res_spect.py` & `torch-hd-5.2.1/torchhd/datasets/low_res_spect.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/lung_cancer.py` & `torch-hd-5.2.1/torchhd/datasets/lung_cancer.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/lymphography.py` & `torch-hd-5.2.1/torchhd/datasets/lymphography.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/magic.py` & `torch-hd-5.2.1/torchhd/datasets/magic.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/mammographic.py` & `torch-hd-5.2.1/torchhd/datasets/mammographic.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/miniboone.py` & `torch-hd-5.2.1/torchhd/datasets/miniboone.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/molec_biol_promoter.py` & `torch-hd-5.2.1/torchhd/datasets/molec_biol_promoter.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/molec_biol_splice.py` & `torch-hd-5.2.1/torchhd/datasets/molec_biol_splice.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/monks_1.py` & `torch-hd-5.2.1/torchhd/datasets/monks_1.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/monks_2.py` & `torch-hd-5.2.1/torchhd/datasets/monks_2.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/monks_3.py` & `torch-hd-5.2.1/torchhd/datasets/monks_3.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/mushroom.py` & `torch-hd-5.2.1/torchhd/datasets/mushroom.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/musk_1.py` & `torch-hd-5.2.1/torchhd/datasets/musk_1.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/musk_2.py` & `torch-hd-5.2.1/torchhd/datasets/musk_2.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/nursery.py` & `torch-hd-5.2.1/torchhd/datasets/nursery.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/oocytes_merluccius_nucleus_4d.py` & `torch-hd-5.2.1/torchhd/datasets/oocytes_merluccius_nucleus_4d.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/oocytes_merluccius_states_2f.py` & `torch-hd-5.2.1/torchhd/datasets/oocytes_merluccius_states_2f.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/oocytes_trisopterus_nucleus_2f.py` & `torch-hd-5.2.1/torchhd/datasets/oocytes_trisopterus_nucleus_2f.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/oocytes_trisopterus_states_5b.py` & `torch-hd-5.2.1/torchhd/datasets/oocytes_trisopterus_states_5b.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/optical.py` & `torch-hd-5.2.1/torchhd/datasets/optical.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/ozone.py` & `torch-hd-5.2.1/torchhd/datasets/ozone.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/page_blocks.py` & `torch-hd-5.2.1/torchhd/datasets/page_blocks.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/pamap.py` & `torch-hd-5.2.1/torchhd/datasets/pamap.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/parkinsons.py` & `torch-hd-5.2.1/torchhd/datasets/parkinsons.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/pendigits.py` & `torch-hd-5.2.1/torchhd/datasets/pendigits.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/pima.py` & `torch-hd-5.2.1/torchhd/datasets/pima.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_material.py` & `torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_material.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_rel_l.py` & `torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_rel_l.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_span.py` & `torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_span.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_t_or_d.py` & `torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_t_or_d.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/pittsburg_bridges_type.py` & `torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_type.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/planning.py` & `torch-hd-5.2.1/torchhd/datasets/planning.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/plant_margin.py` & `torch-hd-5.2.1/torchhd/datasets/plant_margin.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/plant_shape.py` & `torch-hd-5.2.1/torchhd/datasets/plant_shape.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/plant_texture.py` & `torch-hd-5.2.1/torchhd/datasets/plant_texture.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/post_operative.py` & `torch-hd-5.2.1/torchhd/datasets/post_operative.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/primary_tumor.py` & `torch-hd-5.2.1/torchhd/datasets/primary_tumor.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/ringnorm.py` & `torch-hd-5.2.1/torchhd/datasets/ringnorm.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/seeds.py` & `torch-hd-5.2.1/torchhd/datasets/seeds.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/semeion.py` & `torch-hd-5.2.1/torchhd/datasets/semeion.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/soybean.py` & `torch-hd-5.2.1/torchhd/datasets/soybean.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/spambase.py` & `torch-hd-5.2.1/torchhd/datasets/spambase.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/spect.py` & `torch-hd-5.2.1/torchhd/datasets/spect.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/spectf.py` & `torch-hd-5.2.1/torchhd/datasets/spectf.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/statlog_australian_credit.py` & `torch-hd-5.2.1/torchhd/datasets/statlog_australian_credit.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/statlog_german_credit.py` & `torch-hd-5.2.1/torchhd/datasets/statlog_german_credit.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/statlog_heart.py` & `torch-hd-5.2.1/torchhd/datasets/statlog_heart.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/statlog_image.py` & `torch-hd-5.2.1/torchhd/datasets/statlog_image.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/statlog_landsat.py` & `torch-hd-5.2.1/torchhd/datasets/statlog_landsat.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/statlog_shuttle.py` & `torch-hd-5.2.1/torchhd/datasets/statlog_shuttle.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/statlog_vehicle.py` & `torch-hd-5.2.1/torchhd/datasets/statlog_vehicle.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/steel_plates.py` & `torch-hd-5.2.1/torchhd/datasets/steel_plates.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/synthetic_control.py` & `torch-hd-5.2.1/torchhd/datasets/synthetic_control.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/teaching.py` & `torch-hd-5.2.1/torchhd/datasets/teaching.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/thyroid.py` & `torch-hd-5.2.1/torchhd/datasets/thyroid.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/tic_tac_toe.py` & `torch-hd-5.2.1/torchhd/datasets/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/titanic.py` & `torch-hd-5.2.1/torchhd/datasets/titanic.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/trains.py` & `torch-hd-5.2.1/torchhd/datasets/trains.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/twonorm.py` & `torch-hd-5.2.1/torchhd/datasets/twonorm.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/ucihar.py` & `torch-hd-5.2.1/torchhd/datasets/ucihar.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/utils.py` & `torch-hd-5.2.1/torchhd/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/vertebral_column_2clases.py` & `torch-hd-5.2.1/torchhd/datasets/vertebral_column_2clases.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/vertebral_column_3clases.py` & `torch-hd-5.2.1/torchhd/datasets/vertebral_column_3clases.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/wall_following.py` & `torch-hd-5.2.1/torchhd/datasets/wall_following.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/waveform.py` & `torch-hd-5.2.1/torchhd/datasets/waveform.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/waveform_noise.py` & `torch-hd-5.2.1/torchhd/datasets/waveform_noise.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/wine.py` & `torch-hd-5.2.1/torchhd/datasets/wine.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/wine_quality_red.py` & `torch-hd-5.2.1/torchhd/datasets/wine_quality_red.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/wine_quality_white.py` & `torch-hd-5.2.1/torchhd/datasets/wine_quality_white.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/yeast.py` & `torch-hd-5.2.1/torchhd/datasets/yeast.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/datasets/zoo.py` & `torch-hd-5.2.1/torchhd/datasets/zoo.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/embeddings.py` & `torch-hd-5.2.1/torchhd/embeddings.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import torch.nn.functional as F
 from torch import Tensor
 from torch.nn.parameter import Parameter
 
 import torchhd.functional as functional
 from torchhd.tensors.base import VSATensor
 from torchhd.tensors.map import MAPTensor
-from torchhd.tensors.fhrr import FHRRTensor
+from torchhd.tensors.fhrr import FHRRTensor, type_conversion as fhrr_type_conversion
 from torchhd.tensors.hrr import HRRTensor
 from torchhd.types import VSAOptions
 
 
 __all__ = [
     "Empty",
     "Identity",
@@ -1013,32 +1013,38 @@
         ] = "sinc",
         bandwidth: float = 1.0,
         vsa: Literal["HRR", "FHRR"] = "FHRR",
         device=None,
         dtype=None,
         requires_grad: bool = False,
     ) -> None:
-        factory_kwargs = {"device": device, "dtype": dtype}
         super(FractionalPower, self).__init__()
 
         self.in_features = in_features  # data dimensions
         self.out_features = out_features  # hypervector dimensions
         self.bandwidth = bandwidth
         self.requires_grad = requires_grad
 
         if vsa not in {"HRR", "FHRR"}:
             raise ValueError(
                 f"FractionalPower embedding only supports HRR and FHRR but provided: {vsa}"
             )
 
         self.vsa_tensor = functional.get_vsa_tensor_class(vsa)
 
-        if dtype not in self.vsa_tensor.supported_dtypes:
+        # If a specific dtype is specified make sure it is supported by the VSA model
+        if dtype != None and dtype not in self.vsa_tensor.supported_dtypes:
             raise ValueError(f"dtype {dtype} not supported by {vsa}")
 
+        # The internal weights/phases are stored as floats even if the output is a complex tensor
+        if dtype != None and vsa == "FHRR":
+            dtype = fhrr_type_conversion[dtype]
+
+        factory_kwargs = {"device": device, "dtype": dtype}
+
         # If the distribution is a string use the presets in predefined_kernels
         if isinstance(distribution, str):
             try:
                 self.distribution = self.predefined_kernels[distribution]
             except KeyError:
                 available_names = ", ".join(list(self.predefined_kernels.keys()))
                 raise ValueError(
```

### Comparing `torch-hd-5.2.0/torchhd/functional.py` & `torch-hd-5.2.1/torchhd/functional.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/memory.py` & `torch-hd-5.2.1/torchhd/memory.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/models.py` & `torch-hd-5.2.1/torchhd/models.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/structures.py` & `torch-hd-5.2.1/torchhd/structures.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tensors/__init__.py` & `torch-hd-5.2.1/torchhd/tensors/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tensors/base.py` & `torch-hd-5.2.1/torchhd/tensors/base.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tensors/bsc.py` & `torch-hd-5.2.1/torchhd/tensors/bsc.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tensors/fhrr.py` & `torch-hd-5.2.1/torchhd/tensors/fhrr.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tensors/hrr.py` & `torch-hd-5.2.1/torchhd/tensors/hrr.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tensors/map.py` & `torch-hd-5.2.1/torchhd/tensors/map.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/basis_hv/__init__.py` & `torch-hd-5.2.1/torchhd/tests/basis_hv/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/basis_hv/test_base_tensor.py` & `torch-hd-5.2.1/torchhd/tests/basis_hv/test_base_tensor.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/basis_hv/test_circular_hv.py` & `torch-hd-5.2.1/torchhd/tests/basis_hv/test_circular_hv.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/basis_hv/test_empty_hv.py` & `torch-hd-5.2.1/torchhd/tests/basis_hv/test_empty_hv.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/basis_hv/test_identity_hv.py` & `torch-hd-5.2.1/torchhd/tests/basis_hv/test_identity_hv.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/basis_hv/test_level_hv.py` & `torch-hd-5.2.1/torchhd/tests/basis_hv/test_level_hv.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/basis_hv/test_random_hv.py` & `torch-hd-5.2.1/torchhd/tests/basis_hv/test_random_hv.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/structures/__init__.py` & `torch-hd-5.2.1/torchhd/tests/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/structures/test_distinct_sequence.py` & `torch-hd-5.2.1/torchhd/tests/structures/test_distinct_sequence.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/structures/test_fsa.py` & `torch-hd-5.2.1/torchhd/tests/structures/test_fsa.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/structures/test_graph.py` & `torch-hd-5.2.1/torchhd/tests/structures/test_graph.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/structures/test_hashtable.py` & `torch-hd-5.2.1/torchhd/tests/structures/test_hashtable.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/structures/test_memory.py` & `torch-hd-5.2.1/torchhd/tests/structures/test_memory.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/structures/test_multiset.py` & `torch-hd-5.2.1/torchhd/tests/structures/test_multiset.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/structures/test_sequence.py` & `torch-hd-5.2.1/torchhd/tests/structures/test_sequence.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/tests/structures/test_tree.py` & `torch-hd-5.2.1/torchhd/tests/structures/test_tree.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/types.py` & `torch-hd-5.2.1/torchhd/types.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/utils.py` & `torch-hd-5.2.1/torchhd/utils.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.0/torchhd/version.py` & `torch-hd-5.2.1/torchhd/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-__version__ = "5.2.0"
+__version__ = "5.2.1"
```

