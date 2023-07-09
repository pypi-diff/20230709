# Comparing `tmp/corankco-4.0.1.tar.gz` & `tmp/corankco-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corankco-4.0.1.tar", last modified: Thu Dec  2 00:57:35 2021, max compression
+gzip compressed data, was "corankco-6.0.0.tar", last modified: Sun Jul  9 21:54:19 2023, max compression
```

## Comparing `corankco-4.0.1.tar` & `corankco-6.0.0.tar`

### file list

```diff
@@ -1,105 +1,187 @@
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.738986 corankco-4.0.1/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1825 2021-05-06 10:10:16.000000 corankco-4.0.1/.gitignore
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.698986 corankco-4.0.1/.idea/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      176 2021-03-25 10:54:24.000000 corankco-4.0.1/.idea/.gitignore
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1081 2021-11-29 17:21:06.000000 corankco-4.0.1/.idea/corankco.iml
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/.idea/dictionaries/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1004 2021-11-29 17:21:06.000000 corankco-4.0.1/.idea/dictionaries/pierre.xml
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/.idea/inspectionProfiles/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      174 2021-11-15 10:23:06.000000 corankco-4.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      196 2021-11-15 10:23:06.000000 corankco-4.0.1/.idea/misc.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      268 2021-11-15 10:23:06.000000 corankco-4.0.1/.idea/modules.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      186 2021-11-15 12:46:10.000000 corankco-4.0.1/.idea/other.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      180 2021-11-15 10:23:06.000000 corankco-4.0.1/.idea/vcs.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1070 2020-09-29 17:23:28.000000 corankco-4.0.1/LICENSE
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       33 2021-05-20 08:58:41.000000 corankco-4.0.1/MANIFEST.in
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9161 2021-12-02 00:57:35.738986 corankco-4.0.1/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7252 2021-11-29 08:10:43.000000 corankco-4.0.1/README.md
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-15 10:23:06.000000 corankco-4.0.1/corankco/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2020-09-29 17:23:28.000000 corankco-4.0.1/corankco/algorithms/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2079 2021-11-28 02:51:52.000000 corankco-4.0.1/corankco/algorithms/algorithmChoice.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/alltied/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-22 13:27:02.000000 corankco-4.0.1/corankco/algorithms/alltied/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2386 2021-11-22 13:29:53.000000 corankco-4.0.1/corankco/algorithms/alltied/all_tied.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/bioconsert/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2020-09-29 17:23:28.000000 corankco-4.0.1/corankco/algorithms/bioconsert/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      327 2021-03-25 18:12:10.000000 corankco-4.0.1/corankco/algorithms/bioconsert/bioco.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8170 2021-11-27 08:59:50.000000 corankco-4.0.1/corankco/algorithms/bioconsert/bioconsert.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/borda/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 17:34:22.000000 corankco-4.0.1/corankco/algorithms/borda/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4250 2021-03-25 17:41:45.000000 corankco-4.0.1/corankco/algorithms/borda/borda.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/copeland/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 18:25:22.000000 corankco-4.0.1/corankco/algorithms/copeland/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6253 2021-03-25 18:41:44.000000 corankco-4.0.1/corankco/algorithms/copeland/copeland.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/exact/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2020-09-29 17:23:28.000000 corankco-4.0.1/corankco/algorithms/exact/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3242 2021-12-01 11:29:50.000000 corankco-4.0.1/corankco/algorithms/exact/exactalgorithm.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    14111 2021-11-26 14:58:31.000000 corankco-4.0.1/corankco/algorithms/exact/exactalgorithmcplex.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    14072 2021-11-26 15:03:58.000000 corankco-4.0.1/corankco/algorithms/exact/exactalgorithmcplex2.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10110 2021-11-23 10:40:12.000000 corankco-4.0.1/corankco/algorithms/exact/exactalgorithmgeneric.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2306 2021-11-26 14:20:47.000000 corankco-4.0.1/corankco/algorithms/exact/exactpreprocess.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/kwiksort/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 10:55:48.000000 corankco-4.0.1/corankco/algorithms/kwiksort/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4222 2021-03-25 17:34:56.000000 corankco-4.0.1/corankco/algorithms/kwiksort/kwiksortabs.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2192 2021-03-25 15:57:48.000000 corankco-4.0.1/corankco/algorithms/kwiksort/kwiksortrandom.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2636 2021-12-01 11:47:04.000000 corankco-4.0.1/corankco/algorithms/median_ranking.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/algorithms/medrank/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 16:56:02.000000 corankco-4.0.1/corankco/algorithms/medrank/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4838 2021-05-06 12:44:31.000000 corankco-4.0.1/corankco/algorithms/medrank/medrank.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/algorithms/parcons/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2020-09-29 17:23:28.000000 corankco-4.0.1/corankco/algorithms/parcons/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7887 2021-11-29 17:21:06.000000 corankco-4.0.1/corankco/algorithms/parcons/parcons.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/algorithms/pickaperm/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 15:33:24.000000 corankco-4.0.1/corankco/algorithms/pickaperm/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3176 2021-05-06 07:44:03.000000 corankco-4.0.1/corankco/algorithms/pickaperm/pickaperm.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/algorithms/repeatchoice/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 12:34:17.000000 corankco-4.0.1/corankco/algorithms/repeatchoice/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4278 2021-03-25 18:31:27.000000 corankco-4.0.1/corankco/algorithms/repeatchoice/repeatchoice.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5249 2021-11-28 09:00:19.000000 corankco-4.0.1/corankco/consensus.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    11851 2021-11-29 17:21:06.000000 corankco-4.0.1/corankco/dataset.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/experimentsVLDB/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-15 10:23:06.000000 corankco-4.0.1/corankco/experimentsVLDB/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10938 2021-12-02 00:56:39.000000 corankco-4.0.1/corankco/experimentsVLDB/bench.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      476 2021-11-23 11:05:24.000000 corankco-4.0.1/corankco/experimentsVLDB/biological_database.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      243 2021-11-15 10:23:06.000000 corankco-4.0.1/corankco/experimentsVLDB/database_enum.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2760 2021-11-24 06:59:41.000000 corankco-4.0.1/corankco/experimentsVLDB/disease.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2459 2021-12-01 16:58:35.000000 corankco-4.0.1/corankco/experimentsVLDB/experiment.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6523 2021-12-01 17:55:01.000000 corankco-4.0.1/corankco/experimentsVLDB/experimentOrphanet.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1801 2021-11-24 06:48:40.000000 corankco-4.0.1/corankco/experimentsVLDB/gene.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1510 2021-11-23 11:05:24.000000 corankco-4.0.1/corankco/experimentsVLDB/geneNcbiParser.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1784 2021-11-29 17:21:06.000000 corankco-4.0.1/corankco/experimentsVLDB/mapping_ncbi_orphanet.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7395 2021-12-01 15:35:05.000000 corankco-4.0.1/corankco/experimentsVLDB/marksExperiment.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      579 2021-11-22 12:06:43.000000 corankco-4.0.1/corankco/experimentsVLDB/ncbi_query_factory.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6923 2021-11-29 17:21:06.000000 corankco-4.0.1/corankco/experimentsVLDB/orphanet_parser.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/experimentsVLDB/reproduce_experiments_vldb/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-30 21:37:49.000000 corankco-4.0.1/corankco/experimentsVLDB/reproduce_experiments_vldb/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    15280 2021-12-02 00:41:24.000000 corankco-4.0.1/corankco/experimentsVLDB/reproduce_experiments_vldb/reproduce_experiments_test_version.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8451 2021-06-12 07:02:12.000000 corankco-4.0.1/corankco/kemeny_computation.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10350 2021-11-29 17:21:06.000000 corankco-4.0.1/corankco/kemeny_computation_these.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/partitioning/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-05-06 07:08:56.000000 corankco-4.0.1/corankco/partitioning/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4310 2021-11-15 10:23:06.000000 corankco-4.0.1/corankco/partitioning/parfront.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/rankingsgeneration/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-15 10:23:06.000000 corankco-4.0.1/corankco/rankingsgeneration/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6295 2021-11-15 10:23:06.000000 corankco-4.0.1/corankco/rankingsgeneration/rankingsgenerate.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7158 2021-12-01 16:52:51.000000 corankco-4.0.1/corankco/scoringscheme.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4420 2021-11-29 17:21:06.000000 corankco-4.0.1/corankco/utils.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco.egg-info/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9161 2021-12-02 00:57:35.000000 corankco-4.0.1/corankco.egg-info/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2803 2021-12-02 00:57:35.000000 corankco-4.0.1/corankco.egg-info/SOURCES.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-12-02 00:57:35.000000 corankco-4.0.1/corankco.egg-info/dependency_links.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-03-25 18:56:17.000000 corankco-4.0.1/corankco.egg-info/not-zip-safe
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2021-12-02 00:57:35.000000 corankco-4.0.1/corankco.egg-info/requires.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        9 2021-12-02 00:57:35.000000 corankco-4.0.1/corankco.egg-info/top_level.txt
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.738986 corankco-4.0.1/data/
--rw-r--r--   0 pierre    (1000) pierre    (1000) 13834960 2021-10-25 12:07:07.000000 corankco-4.0.1/data/dataGeneNCBI.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000) 19912787 2021-09-15 09:47:56.000000 corankco-4.0.1/data/en_product6.xml
--rw-r--r--   0 pierre    (1000) pierre    (1000)   331109 2021-06-15 13:27:20.000000 corankco-4.0.1/data/mappingDiseaseID.csv
--rw-r--r--   0 pierre    (1000) pierre    (1000)   236933 2021-11-04 09:13:37.000000 corankco-4.0.1/data/mapping_genes_geneNCBI_orphanet.csv
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       96 2021-11-15 10:23:07.000000 corankco-4.0.1/requirements.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       38 2021-12-02 00:57:35.738986 corankco-4.0.1/setup.cfg
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      853 2021-12-02 00:57:04.000000 corankco-4.0.1/setup.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.738986 corankco-4.0.1/tests/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2469 2021-11-28 04:07:06.000000 corankco-4.0.1/tests/test.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.282076 corankco-6.0.0/
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.266076 corankco-6.0.0/.github/
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.266076 corankco-6.0.0/.github/workflows/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1545 2023-07-09 21:49:42.000000 corankco-6.0.0/.github/workflows/python-package.yml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1789 2023-07-07 19:08:46.000000 corankco-6.0.0/.gitignore
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.266076 corankco-6.0.0/.idea/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      176 2021-09-08 13:22:17.000000 corankco-6.0.0/.idea/.gitignore
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      972 2023-07-09 01:49:25.000000 corankco-6.0.0/.idea/corankco.iml
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.266076 corankco-6.0.0/.idea/dictionaries/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1004 2021-11-29 13:49:26.000000 corankco-6.0.0/.idea/dictionaries/pierre.xml
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.266076 corankco-6.0.0/.idea/inspectionProfiles/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      174 2021-09-08 13:23:29.000000 corankco-6.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      196 2021-09-08 13:23:51.000000 corankco-6.0.0/.idea/misc.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      268 2021-09-08 13:23:29.000000 corankco-6.0.0/.idea/modules.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      186 2021-11-27 09:49:32.000000 corankco-6.0.0/.idea/other.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      180 2021-09-08 13:23:29.000000 corankco-6.0.0/.idea/vcs.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      388 2023-07-09 01:51:24.000000 corankco-6.0.0/.idea/webResources.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    18091 2023-07-08 21:25:07.000000 corankco-6.0.0/LICENSE
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2022-05-11 09:31:54.000000 corankco-6.0.0/MANIFEST.in
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3287 2023-07-09 21:54:19.282076 corankco-6.0.0/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2957 2023-07-09 01:26:42.000000 corankco-6.0.0/README.md
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.270076 corankco-6.0.0/corankco/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      104 2023-07-07 19:08:46.000000 corankco-6.0.0/corankco/__init__.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.270076 corankco-6.0.0/corankco/algorithms/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-09-08 13:22:17.000000 corankco-6.0.0/corankco/algorithms/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3112 2023-07-08 23:14:53.000000 corankco-6.0.0/corankco/algorithms/algorithmChoice.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.270076 corankco-6.0.0/corankco/algorithms/bioconsert/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-09-08 13:22:17.000000 corankco-6.0.0/corankco/algorithms/bioconsert/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1130 2023-07-09 01:59:10.000000 corankco-6.0.0/corankco/algorithms/bioconsert/bioco.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    12046 2023-07-09 02:00:30.000000 corankco-6.0.0/corankco/algorithms/bioconsert/bioconsert.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.270076 corankco-6.0.0/corankco/algorithms/borda/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-09-08 13:22:17.000000 corankco-6.0.0/corankco/algorithms/borda/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6728 2023-07-07 22:15:25.000000 corankco-6.0.0/corankco/algorithms/borda/borda.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.270076 corankco-6.0.0/corankco/algorithms/copeland/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-09-08 13:22:17.000000 corankco-6.0.0/corankco/algorithms/copeland/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     5540 2023-07-08 18:15:37.000000 corankco-6.0.0/corankco/algorithms/copeland/copeland.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.270076 corankco-6.0.0/corankco/algorithms/exact/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2023-07-05 22:45:55.000000 corankco-6.0.0/corankco/algorithms/exact/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4239 2023-07-09 21:01:49.000000 corankco-6.0.0/corankco/algorithms/exact/exactalgorithm.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2195 2023-07-07 22:29:01.000000 corankco-6.0.0/corankco/algorithms/exact/exactalgorithmbase.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    26594 2023-07-09 20:31:07.000000 corankco-6.0.0/corankco/algorithms/exact/exactalgorithmcplex.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3832 2023-07-08 22:11:20.000000 corankco-6.0.0/corankco/algorithms/exact/exactalgorithmcplexforpaperoptim1.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    15783 2023-07-08 17:32:07.000000 corankco-6.0.0/corankco/algorithms/exact/exactalgorithmgeneric.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.270076 corankco-6.0.0/corankco/algorithms/kwiksort/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-09-08 13:22:17.000000 corankco-6.0.0/corankco/algorithms/kwiksort/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6790 2023-07-08 23:29:31.000000 corankco-6.0.0/corankco/algorithms/kwiksort/kwiksortabs.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3567 2023-07-08 12:53:53.000000 corankco-6.0.0/corankco/algorithms/kwiksort/kwiksortrandom.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4587 2023-07-07 23:44:32.000000 corankco-6.0.0/corankco/algorithms/median_ranking.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10266 2023-07-08 17:28:20.000000 corankco-6.0.0/corankco/algorithms/pairwisebasedalgorithm.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.270076 corankco-6.0.0/corankco/algorithms/parcons/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-09-08 13:22:17.000000 corankco-6.0.0/corankco/algorithms/parcons/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     7399 2023-07-08 22:11:20.000000 corankco-6.0.0/corankco/algorithms/parcons/parcons.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.270076 corankco-6.0.0/corankco/algorithms/pickaperm/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-09-08 13:22:17.000000 corankco-6.0.0/corankco/algorithms/pickaperm/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     5291 2023-07-08 17:29:47.000000 corankco-6.0.0/corankco/algorithms/pickaperm/pickaperm.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    15940 2023-07-09 14:15:19.000000 corankco-6.0.0/corankco/consensus.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    27494 2023-07-09 14:17:30.000000 corankco-6.0.0/corankco/dataset.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6907 2023-07-07 19:08:46.000000 corankco-6.0.0/corankco/element.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    12515 2023-07-08 23:32:35.000000 corankco-6.0.0/corankco/kemeny_score_computation.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.270076 corankco-6.0.0/corankco/partitioning/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-27 09:49:32.000000 corankco-6.0.0/corankco/partitioning/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6112 2023-07-08 21:03:30.000000 corankco-6.0.0/corankco/partitioning/orderedPartition.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2940 2023-07-08 18:52:18.000000 corankco-6.0.0/corankco/partitioning/parconsPartition.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3598 2023-07-08 20:37:34.000000 corankco-6.0.0/corankco/partitioning/parfront.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14096 2023-07-09 20:26:14.000000 corankco-6.0.0/corankco/ranking.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    17539 2023-07-09 02:03:40.000000 corankco-6.0.0/corankco/scoringscheme.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4885 2023-07-08 20:38:59.000000 corankco-6.0.0/corankco/utils.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.270076 corankco-6.0.0/corankco.egg-info/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3287 2023-07-09 21:54:18.000000 corankco-6.0.0/corankco.egg-info/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     5410 2023-07-09 21:54:19.000000 corankco-6.0.0/corankco.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2023-07-09 21:54:18.000000 corankco-6.0.0/corankco.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-09-08 13:23:38.000000 corankco-6.0.0/corankco.egg-info/not-zip-safe
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       59 2023-07-09 21:54:19.000000 corankco-6.0.0/corankco.egg-info/requires.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        9 2023-07-09 21:54:19.000000 corankco-6.0.0/corankco.egg-info/top_level.txt
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.270076 corankco-6.0.0/docs/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      638 2023-07-09 00:18:13.000000 corankco-6.0.0/docs/Makefile
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.266076 corankco-6.0.0/docs/build/
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.274076 corankco-6.0.0/docs/build/html/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      230 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/.buildinfo
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.278076 corankco-6.0.0/docs/build/html/_sources/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       99 2023-07-09 00:46:18.000000 corankco-6.0.0/docs/build/html/_sources/algorithmChoice.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       80 2023-07-09 00:46:31.000000 corankco-6.0.0/docs/build/html/_sources/bioco.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       95 2023-07-09 00:46:47.000000 corankco-6.0.0/docs/build/html/_sources/bioconsert.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-09 00:46:57.000000 corankco-6.0.0/docs/build/html/_sources/borda.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       81 2023-07-09 00:49:20.000000 corankco-6.0.0/docs/build/html/_sources/consensus.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       87 2023-07-09 00:47:51.000000 corankco-6.0.0/docs/build/html/_sources/copeland.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-09 00:49:31.000000 corankco-6.0.0/docs/build/html/_sources/dataset.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-09 00:49:39.000000 corankco-6.0.0/docs/build/html/_sources/element.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      102 2023-07-09 00:49:59.000000 corankco-6.0.0/docs/build/html/_sources/exactalgorithm.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      114 2023-07-09 00:50:21.000000 corankco-6.0.0/docs/build/html/_sources/exactalgorithmbase.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      117 2023-07-09 00:50:31.000000 corankco-6.0.0/docs/build/html/_sources/exactalgorithmcplex.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      159 2023-07-09 00:50:37.000000 corankco-6.0.0/docs/build/html/_sources/exactalgorithmcplexforpaperoptim1.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      123 2023-07-09 00:50:45.000000 corankco-6.0.0/docs/build/html/_sources/exactalgorithmgeneric.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      663 2023-07-09 01:15:27.000000 corankco-6.0.0/docs/build/html/_sources/index.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      126 2023-07-09 00:51:00.000000 corankco-6.0.0/docs/build/html/_sources/kemeny_score_computation.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       96 2023-07-09 00:51:24.000000 corankco-6.0.0/docs/build/html/_sources/kwiksortabs.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      105 2023-07-09 00:51:37.000000 corankco-6.0.0/docs/build/html/_sources/kwiksortrandom.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       96 2023-07-09 00:51:47.000000 corankco-6.0.0/docs/build/html/_sources/median_ranking.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      104 2023-07-09 00:52:21.000000 corankco-6.0.0/docs/build/html/_sources/orderedPartition.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      120 2023-07-09 00:52:53.000000 corankco-6.0.0/docs/build/html/_sources/pairwisebasedalgorithm.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       83 2023-07-09 00:53:22.000000 corankco-6.0.0/docs/build/html/_sources/parcons.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      104 2023-07-09 00:53:32.000000 corankco-6.0.0/docs/build/html/_sources/parconsPartition.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       80 2023-07-09 00:53:44.000000 corankco-6.0.0/docs/build/html/_sources/parfront.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       91 2023-07-09 00:54:09.000000 corankco-6.0.0/docs/build/html/_sources/pickaperm.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-09 00:54:24.000000 corankco-6.0.0/docs/build/html/_sources/ranking.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       93 2023-07-09 00:54:39.000000 corankco-6.0.0/docs/build/html/_sources/scoringscheme.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       69 2023-07-09 00:54:49.000000 corankco-6.0.0/docs/build/html/_sources/utils.rst.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    13742 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/algorithmChoice.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     7753 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/bioco.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    13906 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/bioconsert.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14456 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/borda.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    33018 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/consensus.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    13149 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/copeland.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    49619 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/dataset.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14026 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/element.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14294 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/exactalgorithm.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    13380 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/exactalgorithmbase.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14307 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/exactalgorithmcplex.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     8435 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/exactalgorithmcplexforpaperoptim1.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    12963 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/exactalgorithmgeneric.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    49384 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/genindex.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    18561 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/index.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10664 2023-07-09 02:03:46.000000 corankco-6.0.0/docs/build/html/kemeny_score_computation.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    13448 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/kwiksortabs.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9405 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/kwiksortrandom.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    17549 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/median_ranking.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2522 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/objects.inv
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    15573 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/orderedPartition.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14523 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/pairwisebasedalgorithm.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    15034 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/parcons.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    11316 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/parconsPartition.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9357 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/parfront.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    15084 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/pickaperm.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    12087 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/py-modindex.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    22085 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/ranking.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    36355 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/scoringscheme.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     5368 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/search.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    64042 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/searchindex.js
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     7961 2023-07-09 02:03:47.000000 corankco-6.0.0/docs/build/html/utils.html
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      804 2023-07-09 00:18:13.000000 corankco-6.0.0/docs/make.bat
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.282076 corankco-6.0.0/docs/source/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       99 2023-07-09 00:46:18.000000 corankco-6.0.0/docs/source/algorithmChoice.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       80 2023-07-09 00:46:31.000000 corankco-6.0.0/docs/source/bioco.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       95 2023-07-09 00:46:47.000000 corankco-6.0.0/docs/source/bioconsert.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-09 00:46:57.000000 corankco-6.0.0/docs/source/borda.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1018 2023-07-09 00:59:06.000000 corankco-6.0.0/docs/source/conf.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       81 2023-07-09 00:49:20.000000 corankco-6.0.0/docs/source/consensus.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       87 2023-07-09 00:47:51.000000 corankco-6.0.0/docs/source/copeland.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-09 00:49:31.000000 corankco-6.0.0/docs/source/dataset.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-09 00:49:39.000000 corankco-6.0.0/docs/source/element.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      102 2023-07-09 00:49:59.000000 corankco-6.0.0/docs/source/exactalgorithm.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      114 2023-07-09 00:50:21.000000 corankco-6.0.0/docs/source/exactalgorithmbase.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      117 2023-07-09 00:50:31.000000 corankco-6.0.0/docs/source/exactalgorithmcplex.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      159 2023-07-09 00:50:37.000000 corankco-6.0.0/docs/source/exactalgorithmcplexforpaperoptim1.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      123 2023-07-09 00:50:45.000000 corankco-6.0.0/docs/source/exactalgorithmgeneric.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      663 2023-07-09 01:15:27.000000 corankco-6.0.0/docs/source/index.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      126 2023-07-09 00:51:00.000000 corankco-6.0.0/docs/source/kemeny_score_computation.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       96 2023-07-09 00:51:24.000000 corankco-6.0.0/docs/source/kwiksortabs.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      105 2023-07-09 00:51:37.000000 corankco-6.0.0/docs/source/kwiksortrandom.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       96 2023-07-09 00:51:47.000000 corankco-6.0.0/docs/source/median_ranking.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      104 2023-07-09 00:52:21.000000 corankco-6.0.0/docs/source/orderedPartition.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      120 2023-07-09 00:52:53.000000 corankco-6.0.0/docs/source/pairwisebasedalgorithm.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       83 2023-07-09 00:53:22.000000 corankco-6.0.0/docs/source/parcons.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      104 2023-07-09 00:53:32.000000 corankco-6.0.0/docs/source/parconsPartition.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       80 2023-07-09 00:53:44.000000 corankco-6.0.0/docs/source/parfront.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       91 2023-07-09 00:54:09.000000 corankco-6.0.0/docs/source/pickaperm.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2023-07-09 00:54:24.000000 corankco-6.0.0/docs/source/ranking.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       93 2023-07-09 00:54:39.000000 corankco-6.0.0/docs/source/scoringscheme.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       69 2023-07-09 00:54:49.000000 corankco-6.0.0/docs/source/utils.rst
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      804 2023-07-01 08:05:34.000000 corankco-6.0.0/make.bat
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       96 2023-07-09 21:39:50.000000 corankco-6.0.0/requirements.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       38 2023-07-09 21:54:19.282076 corankco-6.0.0/setup.cfg
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      815 2023-07-09 20:24:16.000000 corankco-6.0.0/setup.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-09 21:54:19.282076 corankco-6.0.0/tests/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       19 2023-07-07 19:08:46.000000 corankco-6.0.0/tests/dataset_example
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2715 2023-07-09 00:05:33.000000 corankco-6.0.0/tests/exemple.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2143 2023-07-08 21:04:33.000000 corankco-6.0.0/tests/test_BioCo.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1854 2023-07-09 20:37:40.000000 corankco-6.0.0/tests/test_BioConsert.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1742 2023-07-08 23:01:46.000000 corankco-6.0.0/tests/test_Borda.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1964 2023-07-07 19:08:46.000000 corankco-6.0.0/tests/test_Copeland.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2522 2023-07-07 19:08:46.000000 corankco-6.0.0/tests/test_Element.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3382 2023-07-07 19:08:46.000000 corankco-6.0.0/tests/test_Ranking.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4076 2023-07-08 23:00:45.000000 corankco-6.0.0/tests/test_ScoringScheme.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     5138 2023-07-09 21:11:24.000000 corankco-6.0.0/tests/test_dataset.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      971 2023-07-09 20:58:19.000000 corankco-6.0.0/tests/test_exact_algorithms.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6228 2023-07-08 18:59:20.000000 corankco-6.0.0/tests/test_kemenycomputation.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4264 2023-07-09 21:04:11.000000 corankco-6.0.0/tests/test_median_ranking_algorithms.py
```

### Comparing `corankco-4.0.1/.gitignore` & `corankco-6.0.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -64,16 +64,14 @@
 # Flask stuff:
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
-# Sphinx documentation
-docs/_build/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `corankco-4.0.1/.idea/corankco.iml` & `corankco-6.0.0/.idea/corankco.iml`

 * *Files 11% similar despite different names*

#### Comparing `corankco-4.0.1/.idea/corankco.iml` & `corankco-6.0.0/.idea/corankco.iml`

```diff
@@ -1,26 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <module type="PYTHON_MODULE" version="4">
   <component name="NewModuleRootManager">
     <content url="file://$MODULE_DIR$">
       <sourceFolder url="file://$MODULE_DIR$/corankco" isTestSource="false"/>
+      <sourceFolder url="file://$MODULE_DIR$/corankco/partitioning" isTestSource="false"/>
+      <sourceFolder url="file://$MODULE_DIR$/corankco/algorithms" isTestSource="false"/>
       <excludeFolder url="file://$MODULE_DIR$/build"/>
     </content>
-    <content url="file:///opt/ibm/ILOG/CPLEX_Studio201/cplex/python/3.8/x86-64_linux"/>
+    <content url="file:///opt/ibm/ILOG/CPLEX_Studio2211/cplex/python/3.8/x86-64_linux"/>
     <orderEntry type="inheritedJdk"/>
     <orderEntry type="sourceFolder" forTests="false"/>
   </component>
-  <component name="PyDocumentationSettings">
-    <option name="format" value="PLAIN"/>
-    <option name="myDocStringFormat" value="Plain"/>
-  </component>
   <component name="PyNamespacePackagesService">
     <option name="namespacePackageFolders">
       <list>
         <option value="$MODULE_DIR$/corankco/algorithms"/>
-        <option value="$MODULE_DIR$/corankco/experimentsVLDB"/>
-        <option value="$MODULE_DIR$/corankco/rankingsgeneration"/>
-        <option value="$MODULE_DIR$/corankco/partitioning"/>
+        <option value="$MODULE_DIR$/corankco/algorithms"/>
       </list>
     </option>
   </component>
 </module>
```

### Comparing `corankco-4.0.1/.idea/dictionaries/pierre.xml` & `corankco-6.0.0/.idea/dictionaries/pierre.xml`

 * *Files identical despite different names*

### Comparing `corankco-4.0.1/corankco/algorithms/alltied/all_tied.py` & `corankco-6.0.0/corankco/algorithms/exact/exactalgorithmbase.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,63 @@
-from corankco.algorithms.median_ranking import MedianRanking
+from abc import ABC, abstractmethod
 from corankco.dataset import Dataset
+from corankco.consensus import Consensus
 from corankco.scoringscheme import ScoringScheme
-from corankco.consensus import Consensus, ConsensusFeature
+from corankco.algorithms.median_ranking import MedianRanking
 
 
-class AllTied(MedianRanking):
-    def __init__(self):
-        pass
+class IncompatibleArgumentsException(Exception):
+    pass
+
+
+class ExactAlgorithmBase(ABC, MedianRanking):
+    """
+    An abstract base class for exact algorithms. This class outlines the interface that all exact algorithms must
+    implement.
+    """
 
+    def __init__(self, optimize: bool = True):
+        """
+        Initialize the exact algorithm.
+
+        :param optimize: Boolean for whether to use the graph-based preprocess of ParCons algorithm. Defaults to True.
+        WARNING: if optimize = True, then, we cannot ensure that all the optimal consensus will be returned
+        """
+        self._optimize: bool = optimize
+
+    @abstractmethod
     def compute_consensus_rankings(
             self,
             dataset: Dataset,
             scoring_scheme: ScoringScheme,
-            return_at_most_one_ranking=False,
+            return_at_most_one_ranking=True,
             bench_mode=False
     ) -> Consensus:
         """
-        :param dataset: A dataset containing the rankings to aggregate
-        :type dataset: Dataset (class Dataset in package 'datasets')
-        :param scoring_scheme: The penalty vectors to consider
-        :type scoring_scheme: ScoringScheme (class ScoringScheme in package 'distances')
-        :param return_at_most_one_ranking: the algorithm should not return more than one ranking
-        :type return_at_most_one_ranking: bool
-        :param bench_mode: is bench mode activated. If False, the algorithm may return more information
-        :type bench_mode: bool
-        :return one or more rankings if the underlying algorithm can find several equivalent consensus rankings
-        If the algorithm is not able to provide multiple consensus, or if return_at_most_one_ranking is True then, it
-        should return a list made of the only / the first consensus found.
-        In all scenario, the algorithm returns a list of consensus rankings
-        :raise ScoringSchemeNotHandledException when the algorithm cannot compute the consensus because the
-        implementation of the algorithm does not fit with the scoring scheme
-        """
-        elems = set()
-        for ranking in dataset.rankings:
-            for bucket in ranking:
-                for elem in bucket:
-                    elems.add(elem)
-        consensus = [list(elems)]
-        return Consensus(consensus_rankings=[consensus],
-                         dataset=dataset,
-                         scoring_scheme=scoring_scheme,
-                         att={
-                              ConsensusFeature.AssociatedAlgorithm: self.get_full_name()
-                              }
-                         )
+        Abstract method to compute consensus rankings.
+
+        :param dataset: A dataset containing the rankings to aggregate.
+        :param scoring_scheme: The penalty vectors to consider.
+        :param return_at_most_one_ranking: The algorithm should not return more than one ranking.
+        :param bench_mode: Is bench mode activated. If False, the algorithm may return more information.
+        :return: One or more consensus rankings.
+        """
+        pass
 
+    @abstractmethod
     def get_full_name(self) -> str:
-        return "AllTied"
+        """
+        Abstract method to get the full name of the algorithm.
+
+        :return: The full name of the algorithm as a string.
+        """
+        pass
 
+    @abstractmethod
     def is_scoring_scheme_relevant_when_incomplete_rankings(self, scoring_scheme: ScoringScheme) -> bool:
-        return True
+        """
+        Abstract method to check if the scoring scheme is relevant when rankings are incomplete.
+
+        :param scoring_scheme: The scoring scheme to check.
+        :return: True if the scoring scheme is relevant, False otherwise.
+        """
+        pass
```

### Comparing `corankco-4.0.1/corankco/algorithms/borda/borda.py` & `corankco-6.0.0/corankco/algorithms/pickaperm/pickaperm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,39 @@
-from corankco.algorithms.median_ranking import MedianRanking, ScoringSchemeNotHandledException
+from corankco.algorithms.median_ranking import MedianRanking
 from corankco.dataset import Dataset
 from corankco.scoringscheme import ScoringScheme
 from corankco.consensus import Consensus, ConsensusFeature
-
-
-class BordaCount(MedianRanking):
-    def __init__(self,  use_bucket_id=False):
-        self.useBucketIdAndNotBucketSize = use_bucket_id
+from corankco.kemeny_score_computation import KemenyComputingFactory
+from corankco.ranking import Ranking
+from typing import List, Dict
+
+
+class InompleteRankingsIncompatibleWithScoringSchemeException(Exception):
+    pass
+
+
+class PickAPerm(MedianRanking):
+    """
+    Algorithm for rank aggregation initially defined in N.Ailon, M.Charikar, A.Newman. Aggregating inconsistent
+    information : ranking and clustering. Journal of the ACM (JACM) 55.5 (2008), p. 23.
+    This algorithm has been designed as a 2-approximation algorithm of the Kemeny-Young method when rankings are
+    complete and without ties. It selects the input ranking which minimizes the Kemeny score with the input rankings.
+
+    Generalization to incomplete rankings (with ties): Within the framework designed by P.Andrieu, S.Cohen-Boulakia,
+    M.Couceiro, A.Denise, A.Pierrot. A Unifying Rank Aggregation Model to Suitably and Efficiently Aggregate Any Kind of
+    Rankings. https://dx.doi.org/10.2139/ssrn.4353494, this algorithm can only be used with one ScoringScheme
+    (see is_scoring_scheme_relevant_when_incomplete_rankings docstring, and ScoringScheme class)
+    """
 
     def compute_consensus_rankings(
             self,
             dataset: Dataset,
             scoring_scheme: ScoringScheme,
-            return_at_most_one_ranking=False,
-            bench_mode=False
+            return_at_most_one_ranking: bool = True,
+            bench_mode: bool = False
     ) -> Consensus:
         """
         :param dataset: A dataset containing the rankings to aggregate
         :type dataset: Dataset (class Dataset in package 'datasets')
         :param scoring_scheme: The penalty vectors to consider
         :type scoring_scheme: ScoringScheme (class ScoringScheme in package 'distances')
         :param return_at_most_one_ranking: the algorithm should not return more than one ranking
@@ -27,62 +43,62 @@
         :return one or more rankings if the underlying algorithm can find several equivalent consensus rankings
         If the algorithm is not able to provide multiple consensus, or if return_at_most_one_ranking is True then, it
         should return a list made of the only / the first consensus found.
         In all scenario, the algorithm returns a list of consensus rankings
         :raise ScoringSchemeNotHandledException when the algorithm cannot compute the consensus because the
         implementation of the algorithm does not fit with the scoring scheme
         """
-
-        if not dataset.is_complete and not self.is_scoring_scheme_relevant_when_incomplete_rankings(scoring_scheme):
-            raise ScoringSchemeNotHandledException
-
-        if scoring_scheme.is_equivalent_to(ScoringScheme.get_unifying_scoring_scheme().penalty_vectors) or \
-                scoring_scheme.is_equivalent_to(ScoringScheme.get_unifying_scoring_scheme_p(0.5).penalty_vectors):
-            rankings_to_use = dataset.unified_rankings()
+        if not dataset.is_complete:
+            if not scoring_scheme.is_equivalent_to(ScoringScheme.get_unifying_scoring_scheme()):
+                raise InompleteRankingsIncompatibleWithScoringSchemeException
+            else:
+                rankings_to_use = dataset.unified_rankings()
         else:
             rankings_to_use = dataset.rankings
 
-        points = {}
+        mapping_ranking_score: Dict[str, float] = {}
+        kemeny_computation: KemenyComputingFactory = KemenyComputingFactory(scoring_scheme)
+
+        dst_min = float('inf')
+        consensus: List[Ranking] = []
         for ranking in rankings_to_use:
-            id_bucket = 1
-            for bucket in ranking:
-                for elem in bucket:
-                    if elem not in points:
-                        points[elem] = {}
-                        points[elem][0] = 0
-                        points[elem][1] = 0
-
-                    points[elem][0] += id_bucket
-                    points[elem][1] += 1
-                if self.useBucketIdAndNotBucketSize:
-                    id_bucket += 1
-                else:
-                    id_bucket += len(bucket)
-        lis = []
-        for elem in points.keys():
-            lis.append((elem, points[elem][0] * 1.0 / points[elem][1]))
-        tri = sorted(lis, key=lambda col: col[1])
-        consensus = []
-        bucket = []
-        last = -1
-        for duo in tri:
-            if duo[1] != last:
-                last = duo[1]
-                bucket = []
-                consensus.append(bucket)
-            bucket.append(duo[0])
-        return Consensus(consensus_rankings=[consensus],
+            ranking_str = str(ranking)
+            if ranking_str not in mapping_ranking_score:
+                dist: float = kemeny_computation.get_kemeny_score(ranking, dataset)
+            else:
+                dist: float = mapping_ranking_score[ranking_str]
+            if dist < dst_min:
+                dst_min = dist
+                consensus.clear()
+                consensus.append(ranking)
+            elif dist == dst_min and not return_at_most_one_ranking:
+                consensus.append(ranking)
+
+        return Consensus(consensus_rankings=consensus,
                          dataset=dataset,
                          scoring_scheme=scoring_scheme,
-                         att={
+                         att={ConsensusFeature.KemenyScore: dst_min,
                               ConsensusFeature.AssociatedAlgorithm: self.get_full_name()
                               }
                          )
 
     def get_full_name(self) -> str:
-        return "BordaCount"
+        """
+        Return the full name of the algorithm.
+
+        :return: The string 'Pick a Perm'.
+        :rtype: str
+        """
+        return "Pick a Perm"
 
     def is_scoring_scheme_relevant_when_incomplete_rankings(self, scoring_scheme: ScoringScheme) -> bool:
-        return scoring_scheme.is_equivalent_to(ScoringScheme.get_induced_measure_scoring_scheme().penalty_vectors) or \
-               scoring_scheme.is_equivalent_to(ScoringScheme.get_unifying_scoring_scheme().penalty_vectors) or \
-               scoring_scheme.is_equivalent_to(ScoringScheme.get_induced_measure_scoring_scheme_p(0.5).penalty_vectors)\
-               or scoring_scheme.is_equivalent_to(ScoringScheme.get_unifying_scoring_scheme_p(0.5).penalty_vectors)
+        """
+        Check if the scoring scheme is relevant when the rankings are incomplete.
+
+        :param scoring_scheme: The scoring scheme to be checked.
+        :type scoring_scheme: ScoringScheme
+        :return: True if the scoring scheme is equivalent to unifying scoring scheme
+        Otherwise, False. Indeed, the consensus ranking need to be complete in this framework. Selecting this
+        ScoringScheme mean that the user agrees with considering all the missing elements of an input ranking r can be
+        considered as tied in a unifying bucket at the end of r, which makes the input rankings "virtually complete".
+        """
+        return scoring_scheme.is_equivalent_to(ScoringScheme.get_unifying_scoring_scheme())
```

### Comparing `corankco-4.0.1/corankco/algorithms/kwiksort/kwiksortabs.py` & `corankco-6.0.0/corankco/algorithms/exact/exactalgorithm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,49 @@
-from typing import List
-from numpy import ndarray, asarray
-from corankco.algorithms.median_ranking import MedianRanking
-from corankco.dataset import Dataset
+from corankco.algorithms.exact.exactalgorithmbase import ExactAlgorithmBase
+from corankco.algorithms.exact.exactalgorithmcplex import ExactAlgorithmCplex
+from corankco.algorithms.exact.exactalgorithmgeneric import ExactAlgorithmGeneric
 from corankco.scoringscheme import ScoringScheme
-from corankco.consensus import Consensus, ConsensusFeature
+from corankco.dataset import Dataset
+from corankco.consensus import Consensus
 
 
-class KwikSortAbs(MedianRanking):
+class ExactAlgorithm(ExactAlgorithmBase):
+    """
+    This class provides a wrapper for exact ranking algorithms. It intelligently selects an appropriate exact algorithm
+    depending on the availability of the Cplex library. If Cplex is not installed, the class defaults to a free solver.
+
+    The complexity of this algorithm is exponential. In practical use cases, it is expected to execute within a few
+    seconds for ranking tasks involving fewer than 80 elements. For larger sets of elements, the performance will be
+    significantly influenced by specific characteristics of the input rankings.
+
+    Particularly, if the size of the largest strongly connected component (as described in the research paper
+    "Efficient, robust, and effective rank aggregation for massive biological datasets"
+    (https://www.researchgate.net/publication/352277711_Efficient_robust_and_effective_rank_aggregation_for_massive_biological_datasets))
+    exceeds 100, the algorithm may not complete in a reasonable timeframe or may require excessive memory.
+    This information can be determined using ParConsPartition class.
+    """
+
+    def __init__(self, optimize=True):
+        """
+        Initialize the exact algorithm.
 
-    def compute_consensus_rankings(
-            self,
-            dataset: Dataset,
-            scoring_scheme: ScoringScheme,
-            return_at_most_one_ranking=False,
-            bench_mode=False
-    ) -> Consensus:
+        :param optimize: Boolean for whether to optimize the algorithm or not by adding constraints thanks tu sufficient
+        conditions. Defaults to True.
+        """
+        super().__init__(optimize)
+        try:
+            import cplex
+            self._alg = ExactAlgorithmCplex(optimize=optimize)
+        except ModuleNotFoundError:
+            self._alg = ExactAlgorithmGeneric()
+        except ImportError:
+            self._alg = ExactAlgorithmGeneric()
+
+    def compute_consensus_rankings(self, dataset: Dataset, scoring_scheme: ScoringScheme,
+                                   return_at_most_one_ranking: bool = True, bench_mode: bool = False) -> Consensus:
         """
         :param dataset: A dataset containing the rankings to aggregate
         :type dataset: Dataset (class Dataset in package 'datasets')
         :param scoring_scheme: The penalty vectors to consider
         :type scoring_scheme: ScoringScheme (class ScoringScheme in package 'distances')
         :param return_at_most_one_ranking: the algorithm should not return more than one ranking
         :type return_at_most_one_ranking: bool
@@ -27,66 +52,26 @@
         :return one or more rankings if the underlying algorithm can find several equivalent consensus rankings
         If the algorithm is not able to provide multiple consensus, or if return_at_most_one_ranking is True then, it
         should return a list made of the only / the first consensus found.
         In all scenario, the algorithm returns a list of consensus rankings
         :raise ScoringSchemeNotHandledException when the algorithm cannot compute the consensus because the
         implementation of the algorithm does not fit with the scoring scheme
         """
-        sc = asarray(scoring_scheme.penalty_vectors)
-
-        consensus = []
-        elements_translated_target = []
-        var = self.prepare_internal_vars(elements_translated_target, dataset.rankings)
-        self.kwik_sort(consensus, elements_translated_target, var, sc)
-        return Consensus(consensus_rankings=[consensus],
-                         dataset=dataset,
-                         scoring_scheme=scoring_scheme,
-                         att={ConsensusFeature.AssociatedAlgorithm: self.get_full_name()}
-                         )
-
-    def prepare_internal_vars(self, elements_translated_target: List, rankings: List[List[List[int]]]):
-        raise NotImplementedError("The method not implemented")
-    # protected abstract U prepareInternalVars(
-    # List < V > elementsTranslatedTarget, Collection < List < Collection < T >> > rankings);
-
-    def get_pivot(self, elements: List[int], var):
-        raise NotImplementedError("The method not implemented")
-    # public abstract V getPivot(List < V > elements, U var);
-
-    def where_should_it_be(self, element: int, pivot: int, elements: List[int], var, scoring_scheme: ndarray):
-        raise NotImplementedError("The method not implemented")
-    # public abstract int whereShouldItBe(V element, V pivot, List < V > elements, U var);
-
-    def kwik_sort(self, consensus: List[List[int]], elements: List[int], var, scoring_scheme: ndarray):
-        after = []
-        before = []
-        same = []
-        pivot = -1
-        if len(elements) > 0:
-            pivot = self.get_pivot(elements, var)
-            same.append(pivot)
-        for element in elements:
-            if element != pivot:
-                pos = self.where_should_it_be(element, pivot, elements, var, scoring_scheme)
-                if pos < 0:
-                    before.append(element)
-                elif pos > 0:
-                    after.append(element)
-                else:
-                    same.append(element)
-
-        if len(before) == 1:
-            consensus.append(before)
-        elif len(before) > 0:
-            self.kwik_sort(consensus, before, var, scoring_scheme)
-        if len(same) > 0:
-            consensus.append(same)
-        if len(after) == 1:
-            consensus.append(after)
-        elif len(after) > 0:
-            self.kwik_sort(consensus, after, var, scoring_scheme)
+        return self._alg.compute_consensus_rankings(dataset, scoring_scheme, return_at_most_one_ranking, bench_mode)
 
     def get_full_name(self) -> str:
-        return "KwikSortAbs"
+        """
+
+        :return: The name of the algorithm, depends on which has been used between Cplex and PULP
+        """
+        return self._alg.get_full_name()
 
-    def is_scoring_scheme_relevant_when_incomplete_rankings(self, scoring_scheme: ScoringScheme) -> bool:
-        return True
+    def is_scoring_scheme_relevant_when_incomplete_rankings(self, scoring_scheme: ScoringScheme):
+        """
+        Check if the scoring scheme is relevant when the rankings are incomplete.
+
+        :param scoring_scheme: The scoring scheme to be checked.
+        :type scoring_scheme: ScoringScheme
+        :return: True as ExactAlgorithmCplex can handle any ScoringScheme
+        :rtype: bool
+        """
+        return self._alg.is_scoring_scheme_relevant_when_incomplete_rankings(scoring_scheme)
```

### Comparing `corankco-4.0.1/corankco/algorithms/medrank/medrank.py` & `corankco-6.0.0/corankco/algorithms/median_ranking.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,101 +1,104 @@
-from itertools import zip_longest
-
-from corankco.algorithms.median_ranking import MedianRanking, ScoringSchemeNotHandledException
 from corankco.dataset import Dataset
 from corankco.scoringscheme import ScoringScheme
-from corankco.consensus import Consensus, ConsensusFeature
+from corankco.consensus import Consensus
+from time import time
+
+
+class ScoringSchemeNotHandledException(Exception):
+    pass
 
 
-class MedRank(MedianRanking):
-    def __init__(self,  h=0.5):
-        if h < 0:
-            h = 0
-        elif h > 1:
-            h = 1
-        self.__h = h
+class MedianRanking:
 
-    # Complexity : 0 (2 * n) with adaptation for induced measure
+    """
+    The MedianRanking class serves as an interface for implementing consensus ranking algorithms. It defines
+    several methods that each consensus ranking algorithm should implement, including the computation of
+    consensus rankings, determining whether a given scoring scheme is relevant for incomplete rankings,
+    and benchmarking the consensus computation time. An algorithm implemented using this interface should
+    also provide a full name and a string representation of itself.
+    """
     def compute_consensus_rankings(
             self,
             dataset: Dataset,
             scoring_scheme: ScoringScheme,
-            return_at_most_one_ranking=False,
-            bench_mode=False
+            return_at_most_one_ranking: bool = True,
+            bench_mode: bool = False
     ) -> Consensus:
         """
-        :param dataset: A dataset containing the rankings to aggregate
-        :type dataset: Dataset (class Dataset in package 'datasets')
-        :param scoring_scheme: The penalty vectors to consider
-        :type scoring_scheme: ScoringScheme (class ScoringScheme in package 'distances')
-        :param return_at_most_one_ranking: the algorithm should not return more than one ranking
+        Calculate and return the consensus rankings based on the given dataset and scoring scheme.
+
+        :param dataset: The dataset of rankings to be aggregated.
+        :type dataset: Dataset
+        :param scoring_scheme: The scoring scheme to be used for calculating consensus.
+        :type scoring_scheme: ScoringScheme
+        :param return_at_most_one_ranking: If True, the algorithm should return at most one ranking.
         :type return_at_most_one_ranking: bool
-        :param bench_mode: is bench mode activated. If False, the algorithm may return more information
+        :param bench_mode: If True, the algorithm may return additional information for benchmarking purposes.
         :type bench_mode: bool
-        :return one or more rankings if the underlying algorithm can find several equivalent consensus rankings
-        If the algorithm is not able to provide multiple consensus, or if return_at_most_one_ranking is True then, it
-        should return a list made of the only / the first consensus found.
-        In all scenario, the algorithm returns a list of consensus rankings
-        :raise ScoringSchemeNotHandledException when the algorithm cannot compute the consensus because the
-        implementation of the algorithm does not fit with the scoring scheme
-        """
-
-        if not dataset.is_complete and not self.is_scoring_scheme_relevant_when_incomplete_rankings(scoring_scheme):
-            raise ScoringSchemeNotHandledException
-
-        if scoring_scheme.is_equivalent_to(ScoringScheme.get_unifying_scoring_scheme().penalty_vectors) or \
-                scoring_scheme.is_equivalent_to(ScoringScheme.get_unifying_scoring_scheme_p(0.5).penalty_vectors):
-            rankings_to_use = dataset.unified_rankings()
-        else:
-            rankings_to_use = dataset.rankings
-        has = {}
-
-        nb_rankings_needed = {}
-        already_put = set()
-
-        for ranking in rankings_to_use:
-            for bucket in ranking:
-                for element in bucket:
-                    if element not in nb_rankings_needed:
-                        nb_rankings_needed[element] = self.__h
-                    else:
-                        nb_rankings_needed[element] += self.__h
-
-        bucket_res = []
-        ranking_res = []
-
-        for reorganized in zip_longest(*rankings_to_use):
-            for bucket in reorganized:
-                if bucket is not None:
-                    for element in bucket:
-                        if element not in already_put:
-                            if element not in has:
-                                has[element] = 1
-                                if nb_rankings_needed[element] <= 1:
-                                    bucket_res.append(element)
-                                    already_put.add(element)
-                            else:
-                                has[element] += 1
-                                if has[element] >= nb_rankings_needed[element]:
-                                    bucket_res.append(element)
-                                    already_put.add(element)
-            if len(bucket_res) > 0:
-                ranking_res.append(bucket_res)
-                bucket_res = []
-
-        rankings_consensus = [ranking_res] if len(ranking_res) > 0 else [[]]
-        return Consensus(consensus_rankings=rankings_consensus,
-                         dataset=dataset,
-                         scoring_scheme=scoring_scheme,
-                         att={
-                              ConsensusFeature.AssociatedAlgorithm: self.get_full_name()
-                              }
-                         )
+        :return: Consensus rankings. If the algorithm is unable to provide multiple consensuses or
+        return_at_most_one_ranking is True, a single consensus ranking is returned.
+        :rtype: Consensus
+        :raise ScoringSchemeNotHandledException: When the algorithm cannot compute the consensus because the
+        implementation does not support the given scoring scheme.
+        """
+        raise NotImplementedError("The method not implemented")
 
     def get_full_name(self) -> str:
-        return "MedRank"
+        """
+        Get the full name of the algorithm.
+
+        :return: The full name of the algorithm.
+        :rtype: str
+        """
+        raise NotImplementedError("The method not implemented")
+
+    def bench_time_consensus(self,
+                             dataset: Dataset,
+                             scoring_scheme: ScoringScheme,
+                             return_at_most_one_ranking: bool = True,
+                             lower_bound_time: float = 1.) -> float:
+        """
+        Calculate and return the average computation time for a given dataset and scoring scheme
+
+        :param dataset: The dataset of rankings to be aggregated.
+        :type dataset: Dataset
+        :param scoring_scheme: The scoring scheme to be used for calculating consensus.
+        :type scoring_scheme: ScoringScheme
+        :param return_at_most_one_ranking: If True, the algorithm should return at most one ranking.
+        :type return_at_most_one_ranking: bool
+        :param lower_bound_time: The lower bound on the total computation time.
+        :type lower_bound_time: float
+        :return: The average computation time.
+        :rtype: float
+        """
+        sum_time: float = 0
+        nb_computation: int = 0
+        while sum_time <= lower_bound_time:
+            begin = time()
+            self.compute_consensus_rankings(
+                dataset, scoring_scheme, return_at_most_one_ranking, True)
+            end = time()
+            sum_time += end - begin
+            nb_computation += 1
+        return sum_time / nb_computation
 
     def is_scoring_scheme_relevant_when_incomplete_rankings(self, scoring_scheme: ScoringScheme) -> bool:
-        return scoring_scheme.is_equivalent_to(ScoringScheme.get_induced_measure_scoring_scheme().penalty_vectors) or \
-               scoring_scheme.is_equivalent_to(ScoringScheme.get_unifying_scoring_scheme().penalty_vectors) or \
-               scoring_scheme.is_equivalent_to(ScoringScheme.get_induced_measure_scoring_scheme_p(0.5).penalty_vectors)\
-               or scoring_scheme.is_equivalent_to(ScoringScheme.get_unifying_scoring_scheme_p(0.5).penalty_vectors)
+        """
+        Determine whether the provided scoring scheme is relevant when dealing with incomplete rankings.
+
+        :param scoring_scheme: The scoring scheme to be evaluated.
+        :type scoring_scheme: ScoringScheme
+        :return: True if the scoring scheme is relevant for incomplete rankings, False otherwise.
+        :rtype: bool
+        """
+        raise NotImplementedError("The method not implemented")
+
+    def __repr__(self):
+        """
+        Return a string representation of the object, including the class name and all instance variables.
+        The instance variables can be specific parameters for a given MedianRanking algorithm
+
+        :return: A string representation of the object.
+        :rtype: str
+        """
+        return self.__class__.__name__ + " " + str(self.__dict__)
```

### Comparing `corankco-4.0.1/corankco/kemeny_computation_these.py` & `corankco-6.0.0/corankco/kemeny_score_computation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,126 @@
-from typing import Dict, List, Set
+from typing import Dict, List, Tuple, Set
 from numpy import zeros, vdot, ndarray, sort, asarray, cumsum, concatenate
+from corankco.scoringscheme import ScoringScheme
+from corankco.ranking import Ranking
+from corankco.element import Element
+from corankco.dataset import Dataset
+
+
+class InvalidRankingsForComputingDistance(Exception):
+    pass
+
+
+class KemenyComputingFactory:
+    """
+    Class to compute Kemeny scores given a ScoringScheme, according to the framework defined in P.Andrieu,
+    S.Cohen-Boulakia, M.Couceiro, A.Denise, A.Pierrot. A Unifying Rank Aggregation Model to Suitably and Efficiently
+    Aggregate Any Kind of Rankings. https://dx.doi.org/10.2139/ssrn.4353494
+    The Kemeny score is generalized within a framework to handle incomplete rankings with ties
+    """
+    def __init__(self, sc: ScoringScheme):
+        self.__scoring_scheme: ScoringScheme = sc
 
+    @property
+    def scoring_scheme(self):
+        """
 
-class KemenyComputation:
-    def __init__(self, b_vector: ndarray or List, t_vector: ndarray or List):
-        self.__b_vector = asarray(b_vector)
-        self.__t_vector = asarray(t_vector)
-
-    def kemeny_score(self, consensus: List[List or Set[int or str]],
-                     rankings: List[List or Set[List or Set[int or str]]]) -> float:
-
-        # hashmap : keys = elements of dom(consensus) and values = bucket id of associated element
-        mapping_elem_consensus_id_bucket = {}
-        id_bucket = 0
+        :return: the scoring scheme used for the computation of kemeny scores
+        :rtype: ScoringScheme
+        """
+        return self.__scoring_scheme
 
-        for bucket_consensus in consensus:
+    def get_kemeny_score(self, ranking: Ranking, dataset: Dataset) -> float:
+        """
+        Note that a Consensus object can be defined by several consensus rankings. Only the first one will be considered
+        to compute the score. All consensus rankings of a Consensus object should be equivalent in quality
+        """
+        # dict : keys = elements of dom(consensus) and values = bucket id of associated element
+        b_vector: ndarray = asarray(self.__scoring_scheme.b_vector)
+        t_vector: ndarray = asarray(self.__scoring_scheme.t_vector)
+
+        mapping_elem_consensus_id_bucket: Dict[Element, int] = {}
+        id_bucket: int = 0
+
+        for bucket_consensus in ranking:
             for elem_consensus in bucket_consensus:
                 mapping_elem_consensus_id_bucket[elem_consensus] = id_bucket
             id_bucket += 1
+        # check if consensus is complete towards dataset
+        for ranking_dataset in dataset:
+            for bucket_ranking_dataset in ranking_dataset:
+                for element in bucket_ranking_dataset:
+                    if element not in mapping_elem_consensus_id_bucket:
+                        raise InvalidRankingsForComputingDistance("The consensus must be compete towards the Dataset."
+                                                                  "Elem " + str(element) + "found in Dataset and "
+                                                                                           "not in consensus")
 
-        # initialisation of sums s_1 and s_2.
         """"
-         s_1 (resp. s_2) must contain the number of pairs of elements (x,y) such that x < y 
-         (resp. x is tied with y) in the consensus and 
-         rank 0: x < y in input rankings 
-         rank 1: x > y in input rankings 
-         rank 2: x is tied with y in input rankings 
-         rank 3: x is present and y is missing in input rankings 
-         rank 4: x is missing and y is present in input rankings 
-         rank 5: x and y are missing in input rankings 
+        initialisation of sums s_1 and s_2.
+        s_1 is the cost due to pairs x, y of elements such that x < y in the target consensus
+        s_2 is the cost due to pairs x, y of elements such that x and y are tied in the consensus
+        """
         """
-        s_1 = zeros(6, dtype=int)
-        s_2 = zeros(6, dtype=int)
+        s_1 (resp. s_2) must contain the number of pairs of elements (x,y) such that x < y 
+        (resp. x is tied with y) in the consensus and 
+        rank 0: x < y in input rankings 
+        rank 1: x > y in input rankings 
+        rank 2: x is tied with y in input rankings 
+        rank 3: x is present and y is missing in input rankings 
+        rank 4: x is missing and y is present in input rankings 
+        rank 5: x and y are missing in input rankings 
+        """
+
+        s_1: ndarray = zeros(6, dtype=int)
+        s_2: ndarray = zeros(6, dtype=int)
 
         # the cost induced by each ranking
-        for ranking in rankings:
-            cost_ranking = self.__cost_by_ranking(
-                consensus, mapping_elem_consensus_id_bucket, ranking
-            )
+        for input_ranking in dataset:
+            cost_ranking: Tuple[float, float] = self.__cost_by_ranking(
+                ranking, mapping_elem_consensus_id_bucket, input_ranking)
             s_1 += cost_ranking[0]
             s_2 += cost_ranking[1]
-        return vdot(s_1, self.__b_vector) + vdot(s_2, self.__t_vector)
+
+        return vdot(s_1, b_vector) + vdot(s_2, t_vector)
 
     @staticmethod
-    def __cost_by_ranking(consensus: List[List or Set[int or str]],
-                          mapping_elem_consensus_id_bucket: Dict[int or str, int],
-                          r: List[List or Set[int or str]]) -> tuple:
-
-        nb_buckets_consensus = len(consensus)
-        s_1 = zeros(6, dtype=int)
-        s_2 = zeros(6, dtype=int)
+    def __cost_by_ranking(ranking_consensus: Ranking,
+                          mapping_elem_consensus_id_bucket: Dict[Element, int],
+                          r_input: Ranking) -> tuple:
+        nb_buckets_consensus: int = len(ranking_consensus)
+
+        s_1: ndarray = zeros(6, dtype=int)
+        s_2: ndarray = zeros(6, dtype=int)
 
         # t_3[i] is the number of elements in consensus[i] missing in input ranking r
-        t_3 = zeros(nb_buckets_consensus, dtype=int)
+        t_3: ndarray = zeros(nb_buckets_consensus, dtype=int)
 
-        missing_elements = set(mapping_elem_consensus_id_bucket.keys())
-        domain_ranking = set()
+        missing_elements: Set[Element] = set(mapping_elem_consensus_id_bucket.keys())
+        domain_ranking: Set[Element] = set()
         # r_prime is the following list of arrays : each element of each bucket of r becomes the
         # number of the bucket where this element is in the consensus ranking (mapping dict)
-        r_prime = []
+        r_prime: List[ndarray] = []
 
-        for bucket in r:
-            bucket_mapped = []
+        for bucket in r_input:
+            bucket_mapped: List[int] = []
 
             for element in bucket:
                 bucket_mapped.append(mapping_elem_consensus_id_bucket.get(element))
                 missing_elements.remove(element)
                 domain_ranking.add(element)
             # the arrays must be sorted for the merging procedure
             r_prime.append(sort(asarray(bucket_mapped), kind='mergesort'))
-
         # getting values of t_1, t_2 and t_3.
         # t_1[i] is the number of elements missing in r and before the bucket i in the consensus
         # t_2[i] is the number of elements missing in r and after the bucket i in the consensus
         for element in missing_elements:
             id_bucket_consensus = mapping_elem_consensus_id_bucket[element]
             t_3[id_bucket_consensus] += 1
 
-        # t_1 is the cumulated sum of (t_3 with a 0 added as first element and without the
-        # last element)
+        # t_1 is the cumulated sum of (t_3 with a 0 added as first element and without the last element)
         t_1 = cumsum(concatenate((zeros(1), t_3[:-1])))
         # t_2[i] = nb of missing elements in r - sum on j < i (t_3[j])
         t_2 = len(missing_elements) - cumsum(t_3)
 
         """ 
         computation of s_1[3] 
         To get the number of pairs of elements (x,y) such that x < y in consensus and x is 
@@ -99,32 +137,32 @@
         for each k of r_prime.
         """
         for bucket in r_prime:
             for elem_r_prime in bucket:
                 s_1[3] += t_2[elem_r_prime]
                 s_1[4] += t_1[elem_r_prime]
 
-        nb_missing_remaining = len(missing_elements)
+        nb_missing_remaining: int = len(missing_elements)
 
         """ 
         computation of s_1[2] 
         To get the number of pairs of elements (x,y) such that x < y in consensus and x is tied 
         with y in r, we use r_prime. The value of s_1[2] is the number of distinct pairs of 
         r_prime that is the sum of the product ( cardinal of each distinct value x in r_prime * 
         the number of elements higher than x in r_prime).
         """
 
         for i in range(len(r_prime)):
             # increments s_1[2]
-            s_1_2 = 0
-            cursor = 0
-            bucket_i_r = r_prime[i]
-            bucket_size_r = len(bucket_i_r)
+            s_1_2: int = 0
+            cursor: int = 0
+            bucket_i_r: ndarray = r_prime[i]
+            bucket_size_r: int = len(bucket_i_r)
             while cursor < bucket_size_r - 1:
-                repetition = 1
+                repetition: int = 1
                 while cursor < bucket_size_r - 1 and bucket_i_r[cursor] == bucket_i_r[cursor + 1]:
                     repetition += 1
                     cursor += 1
                 cursor += 1
                 s_1_2 += repetition * (bucket_size_r - cursor)
             s_1[2] += s_1_2
 
@@ -141,66 +179,68 @@
 
         computation of s_2[3] + s_2[4] induced by ranking (s_2[3] and s_2[4] induce same costs).
         To get the number of pairs of elements (x,y) such that x is tied with y in consensus 
         and (x is present whereas y is missing or x is missing whereas y is present in r), 
         we use t_3 again. This number is the sum on i of the number of pairs (x,y) of elements 
         in the bucket i of consensus such that x is present and y is missing.
         """
-        for i in range(len(consensus)):
+
+        for i in range(len(ranking_consensus)):
             # increments s_1[5], s_2[3] + s_2[4], s_2[5]
-            nb_missing_elements_in_bucket_i_consensus = t_3[i]
+            nb_missing_elements_in_bucket_i_consensus: int = t_3[i]
             if nb_missing_elements_in_bucket_i_consensus > 0:
                 # increments s_1[5]
                 nb_missing_remaining -= nb_missing_elements_in_bucket_i_consensus
+
                 s_1[5] += nb_missing_remaining * nb_missing_elements_in_bucket_i_consensus
 
                 # increments s_2[3] (could be s_2[4] as well, they represent the same
                 # cases / same penalty)
-                s_2[3] += (len(consensus[i]) - nb_missing_elements_in_bucket_i_consensus) * \
-                          nb_missing_elements_in_bucket_i_consensus
 
+                s_2[3] += (len(ranking_consensus[i]) -
+                           nb_missing_elements_in_bucket_i_consensus) * nb_missing_elements_in_bucket_i_consensus
                 if nb_missing_elements_in_bucket_i_consensus > 1:
                     # increments s_2[5]
                     s_2[5] += nb_missing_elements_in_bucket_i_consensus * (
                             nb_missing_elements_in_bucket_i_consensus - 1) / 2
 
-        KemenyComputation.__mergesortlike(r_prime, 0, len(r_prime) - 1, s_1, s_2)
+        KemenyComputingFactory.__mergesortlike(r_prime, 0, len(r_prime) - 1, s_1, s_2)
 
         return s_1, s_2
 
     @staticmethod
     def __mergesortlike(r_prime: List[ndarray], left: int, right: int, s_1: ndarray,
                         s_2: ndarray) -> ndarray:
         # if input ranking is empty
         if not r_prime:
             return asarray([])
         # case end of recursion
         if right <= left:
             return r_prime[right]
         # divide problem into two sub-problems of same size and merge
         else:
-            middle = (right - left) // 2
-            begin = middle + left + 1
-            return KemenyComputation.__merge(KemenyComputation.__mergesortlike(
+            middle: int = (right - left) // 2
+            begin: int = middle + left + 1
+            return KemenyComputingFactory.__merge(KemenyComputingFactory.__mergesortlike(
                 r_prime, left, middle + left, s_1, s_2),
-                KemenyComputation.__mergesortlike(
+                KemenyComputingFactory.__mergesortlike(
                     r_prime, begin, right, s_1, s_2),
                 s_1, s_2)
 
     @staticmethod
     def __merge(left: ndarray, right: ndarray, s_1: ndarray, s_2: ndarray):
         res = zeros(len(left) + len(right), dtype=int)
-        n = len(left)
-        m = len(right)
-        i = 0
-        j = 0
-        k = 0
+        n: int = len(left)
+        m: int = len(right)
+        i: int = 0
+        j: int = 0
+        k: int = 0
         while i < n and j < m:
-            nb = left[i]
-            nb2 = right[j]
+            nb: int = left[i]
+            nb2: int = right[j]
 
             # no inversion
             if nb < nb2:
                 res[k] = nb
                 k += 1
                 i += 1
             # inversion
@@ -208,16 +248,16 @@
                 s_1[1] += n - i
                 res[k] = nb2
                 k += 1
                 j += 1
 
             # here, case where two elements were tied in the consensus and not tied in r
             else:
-                cpt1 = 0
-                cpt2 = 0
+                cpt1: int = 0
+                cpt2: int = 0
                 while i < n and left[i] == nb:
                     res[k] = nb
                     k += 1
                     i += 1
                     cpt1 += 1
                 while j < m and right[j] == nb:
                     res[k] = nb
```

### Comparing `corankco-4.0.1/setup.py` & `corankco-6.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(name='corankco',
-      version='4.0.1',
+      version='6.0.0',
       description='Kemeny-Young method for rank aggregation of incomplete rankings with ties',
       long_description=readme(),
       url='https://github.com/pierreandrieu/corankco',
       author='Pierre Andrieu',
       author_email='pierre.andrieu@lilo.org',
-      license='MIT',
+      license='GPLv2',
       packages=find_packages(include=['corankco', 'corankco.*']),
-      package_data={'corankco': ['data/*']},
-      python_requires='>=3.6',
+      # package_data={'corankco': ['data/*']},
+      python_requires='>=3.8',
       zip_safe=False,
-      install_requires=['numpy~=1.21.2',
+      install_requires=['numpy~=1.22.0',
                         'python-igraph',
                         'pulp~=2.3',
                         'bioconsertinc>=1.0.0',
-                        'biopython~=1.79'
                         ]
       )
```

### Comparing `corankco-4.0.1/tests/test.py` & `corankco-6.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,99 @@
-from corankco.dataset import Dataset
-from corankco.scoringscheme import ScoringScheme
-from corankco.algorithms.algorithmChoice import get_algorithm
-from corankco.algorithms.algorithmChoice import Algorithm
-from corankco.kemeny_computation import KemenyComputingFactory
-
-dataset = Dataset([
-              [[1], [2, 3]],
-              [[3, 1], [4]],
-              [[1], [5], [3, 2]]
-             ])
-# or d = Dataset.get_rankings_from_file(file_path), with file_path is the path to fhe file
-# import a list of datasets in a same folder : Dataset.get_rankings_from_folder(path_folder)
-
-# print information about the dataset
-print(dataset.description())
-# choose your scoring scheme (or sc = ScoringScheme() for default scoring scheme)
-sc = ScoringScheme([[0., 1., 1., 0., 1., 1.], [1., 1., 0., 1., 1., 0.]])
-
-print("scoring scheme : " + str(sc))
-# scoring scheme description
-print(sc.description())
-
-print("\n### Consensus computation ###\n")
-
-algorithm = get_algorithm(alg=Algorithm.ParCons, parameters={"bound_for_exact": 90})
-# compute consensus ranking
-consensus = algorithm.compute_consensus_rankings(dataset=dataset, scoring_scheme=sc, return_at_most_one_ranking=False)
-
-print(consensus.description())
-
-# if you want the consensus ranking only : print(consensus)
-# to get the consensus rankings : consensus.consensus_rankings
-
-# list of rank aggregation algorithms to use among  BioConsert, ParCons, ExactAlgorithm, KwikSortRandom, RepeatChoice,
-# PickAPerm, MedRank, BordaCount, BioCo, CopelandMethod
-
-algorithms_to_execute = [get_algorithm(alg=Algorithm.KwikSortRandom),
-                         get_algorithm(alg=Algorithm.BioConsert, parameters={"starting_algorithms": []}),
-                         get_algorithm(alg=Algorithm.ParCons, parameters={"bound_for_exact": 90,
-                                                                          "auxiliary_algorithm": get_algorithm(alg=Algorithm.KwikSortRandom)}),
-                         get_algorithm(alg=Algorithm.Exact, parameters={"limit_time_sec": 5})
-                         ]
-
-for alg in algorithms_to_execute:
-    print(alg.get_full_name())
-    consensus = alg.compute_consensus_rankings(dataset=dataset, scoring_scheme=sc, return_at_most_one_ranking=False)
-    print(consensus.description())
-
-# prepare computation
-kemeny = KemenyComputingFactory(sc)
-
-# example of computing score ('distance') between two ranking
-r1 = [[1], [2], [3, 4]]
-r2 = [[3], [2]]
+Metadata-Version: 2.1
+Name: corankco
+Version: 6.0.0
+Summary: Kemeny-Young method for rank aggregation of incomplete rankings with ties
+Home-page: https://github.com/pierreandrieu/corankco
+Author: Pierre Andrieu
+Author-email: pierre.andrieu@lilo.org
+License: GPLv2
+Platform: UNKNOWN
+Requires-Python: >=3.8
+License-File: LICENSE
+
+corankco
+===============
+
+This package implements methods for rank aggregation of incomplete rankings with ties 
+
+Installation
+------------
+
+Install from PyPI:
+
+.. code-block:: bash
+
+    pip3 install --user corankco
+
+Example usage
+-------------
+
+.. code-block:: python
+
+    from corankco.ranking import Ranking
+    from corankco.dataset import Dataset
+    from corankco.scoringscheme import ScoringScheme
+    from corankco.algorithms.algorithmChoice import get_algorithm
+    from corankco.algorithms.algorithmChoice import Algorithm
+
+    # create a ranking from a list of sets
+    ranking1 = Ranking.from_list([{1}, {2, 3}])
+
+    # or from a string
+    ranking2 = Ranking.from_string("[{3, 1}, {4}]")
+
+    # also in this format
+    ranking3 = Ranking.from_string("[[1], [5], [3], [2]]")
+
+    # now, create a Dataset object. A Dataset is a list of rankings
+    dataset = Dataset([ranking1, ranking2, ranking3])
+
+    # or, create a Dataset object from a file where your rankings are stored
+    # format file: each line is a list of either set, or list of int / str.
+    d = Dataset.from_file(path="dataset_example")
+
+    # print information about the dataset
+    print(dataset.description())
+
+    # get all datasets in a folder
+    # list_datasets = Dataset.get_datasets_from_folder(path_folder="folder_path")
+
+    # choose your scoring scheme
+    sc = ScoringScheme([[0., 1., 1., 0., 1., 1.], [1., 1., 0., 1., 1., 0.]])
+
+    print("scoring scheme : " + str(sc))
+    # scoring scheme description
+    print(sc.description())
+
+    print("\n### Consensus computation ###\n")
+
+    # list of rank aggregation algorithms to use among  BioConsert, ParCons, ExactAlgorithm, KwikSortRandom,
+    # PickAPerm, MedRank, BordaCount, BioCo, CopelandMethod
+
+    algorithms_to_execute = [
+        get_algorithm(alg=Algorithm.Exact, parameters={"optimize": True}),
+        get_algorithm(alg=Algorithm.KwikSortRandom),
+        get_algorithm(alg=Algorithm.BioConsert, parameters={"starting_algorithms": []}),
+        get_algorithm(alg=Algorithm.ParCons,
+                      parameters={"bound_for_exact": 90,
+                                  "auxiliary_algorithm": get_algorithm(alg=Algorithm.KwikSortRandom)}),
+        get_algorithm(alg=Algorithm.Exact, parameters={"optimize": True}),
+        get_algorithm(alg=Algorithm.CopelandMethod),
+        get_algorithm(alg=Algorithm.BioCo),
+        get_algorithm(alg=Algorithm.BordaCount)
+    ]
+
+    for alg in algorithms_to_execute:
+        print(alg.get_full_name())
+        consensus = alg.compute_consensus_rankings(dataset=dataset, scoring_scheme=sc, return_at_most_one_ranking=True)
+
+        # to get the consensus rankings: consensus.consensus_rankings
+        # description() will display supplementary information
+
+        print(consensus.description())
+        # if you want the consensus ranking only: print(consensus)
+
+        # get the Kemeny score associated with the consensus:
+        print(consensus.kemeny_score)
+
+
 
-print(kemeny.score_between_rankings(r1, r2))
```

