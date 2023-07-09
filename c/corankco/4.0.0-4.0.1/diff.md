# Comparing `tmp/corankco-4.0.0.tar.gz` & `tmp/corankco-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corankco-4.0.0.tar", last modified: Thu Dec  2 00:31:17 2021, max compression
+gzip compressed data, was "corankco-4.0.1.tar", last modified: Thu Dec  2 00:57:35 2021, max compression
```

## Comparing `corankco-4.0.0.tar` & `corankco-4.0.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.484729 corankco-4.0.0/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1825 2021-05-06 10:10:16.000000 corankco-4.0.0/.gitignore
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.456729 corankco-4.0.0/.idea/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      176 2021-03-25 10:54:24.000000 corankco-4.0.0/.idea/.gitignore
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1081 2021-11-29 17:21:06.000000 corankco-4.0.0/.idea/corankco.iml
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.456729 corankco-4.0.0/.idea/dictionaries/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1004 2021-11-29 17:21:06.000000 corankco-4.0.0/.idea/dictionaries/pierre.xml
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.456729 corankco-4.0.0/.idea/inspectionProfiles/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      174 2021-11-15 10:23:06.000000 corankco-4.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      196 2021-11-15 10:23:06.000000 corankco-4.0.0/.idea/misc.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      268 2021-11-15 10:23:06.000000 corankco-4.0.0/.idea/modules.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      186 2021-11-15 12:46:10.000000 corankco-4.0.0/.idea/other.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      180 2021-11-15 10:23:06.000000 corankco-4.0.0/.idea/vcs.xml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1070 2020-09-29 17:23:28.000000 corankco-4.0.0/LICENSE
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       33 2021-05-20 08:58:41.000000 corankco-4.0.0/MANIFEST.in
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9161 2021-12-02 00:31:17.484729 corankco-4.0.0/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7252 2021-11-29 08:10:43.000000 corankco-4.0.0/README.md
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.456729 corankco-4.0.0/corankco/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-15 10:23:06.000000 corankco-4.0.0/corankco/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.456729 corankco-4.0.0/corankco/algorithms/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2020-09-29 17:23:28.000000 corankco-4.0.0/corankco/algorithms/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2079 2021-11-28 02:51:52.000000 corankco-4.0.0/corankco/algorithms/algorithmChoice.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.456729 corankco-4.0.0/corankco/algorithms/alltied/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-22 13:27:02.000000 corankco-4.0.0/corankco/algorithms/alltied/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2386 2021-11-22 13:29:53.000000 corankco-4.0.0/corankco/algorithms/alltied/all_tied.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.456729 corankco-4.0.0/corankco/algorithms/bioconsert/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2020-09-29 17:23:28.000000 corankco-4.0.0/corankco/algorithms/bioconsert/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      327 2021-03-25 18:12:10.000000 corankco-4.0.0/corankco/algorithms/bioconsert/bioco.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8170 2021-11-27 08:59:50.000000 corankco-4.0.0/corankco/algorithms/bioconsert/bioconsert.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.456729 corankco-4.0.0/corankco/algorithms/borda/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 17:34:22.000000 corankco-4.0.0/corankco/algorithms/borda/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4250 2021-03-25 17:41:45.000000 corankco-4.0.0/corankco/algorithms/borda/borda.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.456729 corankco-4.0.0/corankco/algorithms/copeland/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 18:25:22.000000 corankco-4.0.0/corankco/algorithms/copeland/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6253 2021-03-25 18:41:44.000000 corankco-4.0.0/corankco/algorithms/copeland/copeland.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.456729 corankco-4.0.0/corankco/algorithms/exact/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2020-09-29 17:23:28.000000 corankco-4.0.0/corankco/algorithms/exact/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3242 2021-12-01 11:29:50.000000 corankco-4.0.0/corankco/algorithms/exact/exactalgorithm.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    14111 2021-11-26 14:58:31.000000 corankco-4.0.0/corankco/algorithms/exact/exactalgorithmcplex.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    14072 2021-11-26 15:03:58.000000 corankco-4.0.0/corankco/algorithms/exact/exactalgorithmcplex2.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10110 2021-11-23 10:40:12.000000 corankco-4.0.0/corankco/algorithms/exact/exactalgorithmgeneric.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2306 2021-11-26 14:20:47.000000 corankco-4.0.0/corankco/algorithms/exact/exactpreprocess.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.460729 corankco-4.0.0/corankco/algorithms/kwiksort/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 10:55:48.000000 corankco-4.0.0/corankco/algorithms/kwiksort/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4222 2021-03-25 17:34:56.000000 corankco-4.0.0/corankco/algorithms/kwiksort/kwiksortabs.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2192 2021-03-25 15:57:48.000000 corankco-4.0.0/corankco/algorithms/kwiksort/kwiksortrandom.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2636 2021-12-01 11:47:04.000000 corankco-4.0.0/corankco/algorithms/median_ranking.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.460729 corankco-4.0.0/corankco/algorithms/medrank/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 16:56:02.000000 corankco-4.0.0/corankco/algorithms/medrank/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4838 2021-05-06 12:44:31.000000 corankco-4.0.0/corankco/algorithms/medrank/medrank.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.460729 corankco-4.0.0/corankco/algorithms/parcons/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2020-09-29 17:23:28.000000 corankco-4.0.0/corankco/algorithms/parcons/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7887 2021-11-29 17:21:06.000000 corankco-4.0.0/corankco/algorithms/parcons/parcons.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.460729 corankco-4.0.0/corankco/algorithms/pickaperm/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 15:33:24.000000 corankco-4.0.0/corankco/algorithms/pickaperm/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3176 2021-05-06 07:44:03.000000 corankco-4.0.0/corankco/algorithms/pickaperm/pickaperm.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.460729 corankco-4.0.0/corankco/algorithms/repeatchoice/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 12:34:17.000000 corankco-4.0.0/corankco/algorithms/repeatchoice/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4278 2021-03-25 18:31:27.000000 corankco-4.0.0/corankco/algorithms/repeatchoice/repeatchoice.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5249 2021-11-28 09:00:19.000000 corankco-4.0.0/corankco/consensus.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    11851 2021-11-29 17:21:06.000000 corankco-4.0.0/corankco/dataset.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.460729 corankco-4.0.0/corankco/experimentsVLDB/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-15 10:23:06.000000 corankco-4.0.0/corankco/experimentsVLDB/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    11012 2021-12-01 17:10:03.000000 corankco-4.0.0/corankco/experimentsVLDB/bench.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      476 2021-11-23 11:05:24.000000 corankco-4.0.0/corankco/experimentsVLDB/biological_database.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      243 2021-11-15 10:23:06.000000 corankco-4.0.0/corankco/experimentsVLDB/database_enum.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2760 2021-11-24 06:59:41.000000 corankco-4.0.0/corankco/experimentsVLDB/disease.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2459 2021-12-01 16:58:35.000000 corankco-4.0.0/corankco/experimentsVLDB/experiment.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6523 2021-12-01 17:55:01.000000 corankco-4.0.0/corankco/experimentsVLDB/experimentOrphanet.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1801 2021-11-24 06:48:40.000000 corankco-4.0.0/corankco/experimentsVLDB/gene.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1510 2021-11-23 11:05:24.000000 corankco-4.0.0/corankco/experimentsVLDB/geneNcbiParser.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1784 2021-11-29 17:21:06.000000 corankco-4.0.0/corankco/experimentsVLDB/mapping_ncbi_orphanet.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7395 2021-12-01 15:35:05.000000 corankco-4.0.0/corankco/experimentsVLDB/marksExperiment.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      579 2021-11-22 12:06:43.000000 corankco-4.0.0/corankco/experimentsVLDB/ncbi_query_factory.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6923 2021-11-29 17:21:06.000000 corankco-4.0.0/corankco/experimentsVLDB/orphanet_parser.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.460729 corankco-4.0.0/corankco/experimentsVLDB/reproduce_experiments_vldb/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-30 21:37:49.000000 corankco-4.0.0/corankco/experimentsVLDB/reproduce_experiments_vldb/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    15279 2021-12-02 00:28:04.000000 corankco-4.0.0/corankco/experimentsVLDB/reproduce_experiments_vldb/reproduce_experiments_test_version.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8451 2021-06-12 07:02:12.000000 corankco-4.0.0/corankco/kemeny_computation.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10350 2021-11-29 17:21:06.000000 corankco-4.0.0/corankco/kemeny_computation_these.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.460729 corankco-4.0.0/corankco/partitioning/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-05-06 07:08:56.000000 corankco-4.0.0/corankco/partitioning/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4310 2021-11-15 10:23:06.000000 corankco-4.0.0/corankco/partitioning/parfront.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.460729 corankco-4.0.0/corankco/rankingsgeneration/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-15 10:23:06.000000 corankco-4.0.0/corankco/rankingsgeneration/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6295 2021-11-15 10:23:06.000000 corankco-4.0.0/corankco/rankingsgeneration/rankingsgenerate.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7158 2021-12-01 16:52:51.000000 corankco-4.0.0/corankco/scoringscheme.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4420 2021-11-29 17:21:06.000000 corankco-4.0.0/corankco/utils.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.456729 corankco-4.0.0/corankco.egg-info/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9161 2021-12-02 00:31:17.000000 corankco-4.0.0/corankco.egg-info/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2803 2021-12-02 00:31:17.000000 corankco-4.0.0/corankco.egg-info/SOURCES.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-12-02 00:31:17.000000 corankco-4.0.0/corankco.egg-info/dependency_links.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-03-25 18:56:17.000000 corankco-4.0.0/corankco.egg-info/not-zip-safe
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2021-12-02 00:31:17.000000 corankco-4.0.0/corankco.egg-info/requires.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        9 2021-12-02 00:31:17.000000 corankco-4.0.0/corankco.egg-info/top_level.txt
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.484729 corankco-4.0.0/data/
--rw-r--r--   0 pierre    (1000) pierre    (1000) 13834960 2021-10-25 12:07:07.000000 corankco-4.0.0/data/dataGeneNCBI.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000) 19912787 2021-09-15 09:47:56.000000 corankco-4.0.0/data/en_product6.xml
--rw-r--r--   0 pierre    (1000) pierre    (1000)   331109 2021-06-15 13:27:20.000000 corankco-4.0.0/data/mappingDiseaseID.csv
--rw-r--r--   0 pierre    (1000) pierre    (1000)   236933 2021-11-04 09:13:37.000000 corankco-4.0.0/data/mapping_genes_geneNCBI_orphanet.csv
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       96 2021-11-15 10:23:07.000000 corankco-4.0.0/requirements.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       38 2021-12-02 00:31:17.484729 corankco-4.0.0/setup.cfg
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      853 2021-12-02 00:31:11.000000 corankco-4.0.0/setup.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:31:17.484729 corankco-4.0.0/tests/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2469 2021-11-28 04:07:06.000000 corankco-4.0.0/tests/test.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.738986 corankco-4.0.1/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1825 2021-05-06 10:10:16.000000 corankco-4.0.1/.gitignore
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.698986 corankco-4.0.1/.idea/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      176 2021-03-25 10:54:24.000000 corankco-4.0.1/.idea/.gitignore
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1081 2021-11-29 17:21:06.000000 corankco-4.0.1/.idea/corankco.iml
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/.idea/dictionaries/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1004 2021-11-29 17:21:06.000000 corankco-4.0.1/.idea/dictionaries/pierre.xml
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/.idea/inspectionProfiles/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      174 2021-11-15 10:23:06.000000 corankco-4.0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      196 2021-11-15 10:23:06.000000 corankco-4.0.1/.idea/misc.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      268 2021-11-15 10:23:06.000000 corankco-4.0.1/.idea/modules.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      186 2021-11-15 12:46:10.000000 corankco-4.0.1/.idea/other.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      180 2021-11-15 10:23:06.000000 corankco-4.0.1/.idea/vcs.xml
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1070 2020-09-29 17:23:28.000000 corankco-4.0.1/LICENSE
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       33 2021-05-20 08:58:41.000000 corankco-4.0.1/MANIFEST.in
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9161 2021-12-02 00:57:35.738986 corankco-4.0.1/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     7252 2021-11-29 08:10:43.000000 corankco-4.0.1/README.md
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-15 10:23:06.000000 corankco-4.0.1/corankco/__init__.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2020-09-29 17:23:28.000000 corankco-4.0.1/corankco/algorithms/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2079 2021-11-28 02:51:52.000000 corankco-4.0.1/corankco/algorithms/algorithmChoice.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/alltied/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-22 13:27:02.000000 corankco-4.0.1/corankco/algorithms/alltied/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2386 2021-11-22 13:29:53.000000 corankco-4.0.1/corankco/algorithms/alltied/all_tied.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/bioconsert/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2020-09-29 17:23:28.000000 corankco-4.0.1/corankco/algorithms/bioconsert/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      327 2021-03-25 18:12:10.000000 corankco-4.0.1/corankco/algorithms/bioconsert/bioco.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     8170 2021-11-27 08:59:50.000000 corankco-4.0.1/corankco/algorithms/bioconsert/bioconsert.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/borda/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 17:34:22.000000 corankco-4.0.1/corankco/algorithms/borda/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4250 2021-03-25 17:41:45.000000 corankco-4.0.1/corankco/algorithms/borda/borda.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/copeland/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 18:25:22.000000 corankco-4.0.1/corankco/algorithms/copeland/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6253 2021-03-25 18:41:44.000000 corankco-4.0.1/corankco/algorithms/copeland/copeland.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/exact/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2020-09-29 17:23:28.000000 corankco-4.0.1/corankco/algorithms/exact/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3242 2021-12-01 11:29:50.000000 corankco-4.0.1/corankco/algorithms/exact/exactalgorithm.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14111 2021-11-26 14:58:31.000000 corankco-4.0.1/corankco/algorithms/exact/exactalgorithmcplex.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    14072 2021-11-26 15:03:58.000000 corankco-4.0.1/corankco/algorithms/exact/exactalgorithmcplex2.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10110 2021-11-23 10:40:12.000000 corankco-4.0.1/corankco/algorithms/exact/exactalgorithmgeneric.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2306 2021-11-26 14:20:47.000000 corankco-4.0.1/corankco/algorithms/exact/exactpreprocess.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco/algorithms/kwiksort/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 10:55:48.000000 corankco-4.0.1/corankco/algorithms/kwiksort/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4222 2021-03-25 17:34:56.000000 corankco-4.0.1/corankco/algorithms/kwiksort/kwiksortabs.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2192 2021-03-25 15:57:48.000000 corankco-4.0.1/corankco/algorithms/kwiksort/kwiksortrandom.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2636 2021-12-01 11:47:04.000000 corankco-4.0.1/corankco/algorithms/median_ranking.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/algorithms/medrank/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 16:56:02.000000 corankco-4.0.1/corankco/algorithms/medrank/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4838 2021-05-06 12:44:31.000000 corankco-4.0.1/corankco/algorithms/medrank/medrank.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/algorithms/parcons/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2020-09-29 17:23:28.000000 corankco-4.0.1/corankco/algorithms/parcons/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     7887 2021-11-29 17:21:06.000000 corankco-4.0.1/corankco/algorithms/parcons/parcons.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/algorithms/pickaperm/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 15:33:24.000000 corankco-4.0.1/corankco/algorithms/pickaperm/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     3176 2021-05-06 07:44:03.000000 corankco-4.0.1/corankco/algorithms/pickaperm/pickaperm.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/algorithms/repeatchoice/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-03-25 12:34:17.000000 corankco-4.0.1/corankco/algorithms/repeatchoice/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4278 2021-03-25 18:31:27.000000 corankco-4.0.1/corankco/algorithms/repeatchoice/repeatchoice.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     5249 2021-11-28 09:00:19.000000 corankco-4.0.1/corankco/consensus.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    11851 2021-11-29 17:21:06.000000 corankco-4.0.1/corankco/dataset.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/experimentsVLDB/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-15 10:23:06.000000 corankco-4.0.1/corankco/experimentsVLDB/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10938 2021-12-02 00:56:39.000000 corankco-4.0.1/corankco/experimentsVLDB/bench.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      476 2021-11-23 11:05:24.000000 corankco-4.0.1/corankco/experimentsVLDB/biological_database.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      243 2021-11-15 10:23:06.000000 corankco-4.0.1/corankco/experimentsVLDB/database_enum.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2760 2021-11-24 06:59:41.000000 corankco-4.0.1/corankco/experimentsVLDB/disease.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2459 2021-12-01 16:58:35.000000 corankco-4.0.1/corankco/experimentsVLDB/experiment.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6523 2021-12-01 17:55:01.000000 corankco-4.0.1/corankco/experimentsVLDB/experimentOrphanet.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1801 2021-11-24 06:48:40.000000 corankco-4.0.1/corankco/experimentsVLDB/gene.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1510 2021-11-23 11:05:24.000000 corankco-4.0.1/corankco/experimentsVLDB/geneNcbiParser.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     1784 2021-11-29 17:21:06.000000 corankco-4.0.1/corankco/experimentsVLDB/mapping_ncbi_orphanet.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     7395 2021-12-01 15:35:05.000000 corankco-4.0.1/corankco/experimentsVLDB/marksExperiment.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      579 2021-11-22 12:06:43.000000 corankco-4.0.1/corankco/experimentsVLDB/ncbi_query_factory.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6923 2021-11-29 17:21:06.000000 corankco-4.0.1/corankco/experimentsVLDB/orphanet_parser.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/experimentsVLDB/reproduce_experiments_vldb/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-30 21:37:49.000000 corankco-4.0.1/corankco/experimentsVLDB/reproduce_experiments_vldb/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    15280 2021-12-02 00:41:24.000000 corankco-4.0.1/corankco/experimentsVLDB/reproduce_experiments_vldb/reproduce_experiments_test_version.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     8451 2021-06-12 07:02:12.000000 corankco-4.0.1/corankco/kemeny_computation.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)    10350 2021-11-29 17:21:06.000000 corankco-4.0.1/corankco/kemeny_computation_these.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/partitioning/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-05-06 07:08:56.000000 corankco-4.0.1/corankco/partitioning/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4310 2021-11-15 10:23:06.000000 corankco-4.0.1/corankco/partitioning/parfront.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.706986 corankco-4.0.1/corankco/rankingsgeneration/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-11-15 10:23:06.000000 corankco-4.0.1/corankco/rankingsgeneration/__init__.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     6295 2021-11-15 10:23:06.000000 corankco-4.0.1/corankco/rankingsgeneration/rankingsgenerate.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     7158 2021-12-01 16:52:51.000000 corankco-4.0.1/corankco/scoringscheme.py
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     4420 2021-11-29 17:21:06.000000 corankco-4.0.1/corankco/utils.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.702986 corankco-4.0.1/corankco.egg-info/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     9161 2021-12-02 00:57:35.000000 corankco-4.0.1/corankco.egg-info/PKG-INFO
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2803 2021-12-02 00:57:35.000000 corankco-4.0.1/corankco.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-12-02 00:57:35.000000 corankco-4.0.1/corankco.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2021-03-25 18:56:17.000000 corankco-4.0.1/corankco.egg-info/not-zip-safe
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       75 2021-12-02 00:57:35.000000 corankco-4.0.1/corankco.egg-info/requires.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)        9 2021-12-02 00:57:35.000000 corankco-4.0.1/corankco.egg-info/top_level.txt
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.738986 corankco-4.0.1/data/
+-rw-r--r--   0 pierre    (1000) pierre    (1000) 13834960 2021-10-25 12:07:07.000000 corankco-4.0.1/data/dataGeneNCBI.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000) 19912787 2021-09-15 09:47:56.000000 corankco-4.0.1/data/en_product6.xml
+-rw-r--r--   0 pierre    (1000) pierre    (1000)   331109 2021-06-15 13:27:20.000000 corankco-4.0.1/data/mappingDiseaseID.csv
+-rw-r--r--   0 pierre    (1000) pierre    (1000)   236933 2021-11-04 09:13:37.000000 corankco-4.0.1/data/mapping_genes_geneNCBI_orphanet.csv
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       96 2021-11-15 10:23:07.000000 corankco-4.0.1/requirements.txt
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)       38 2021-12-02 00:57:35.738986 corankco-4.0.1/setup.cfg
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)      853 2021-12-02 00:57:04.000000 corankco-4.0.1/setup.py
+drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2021-12-02 00:57:35.738986 corankco-4.0.1/tests/
+-rw-rw-r--   0 pierre    (1000) pierre    (1000)     2469 2021-11-28 04:07:06.000000 corankco-4.0.1/tests/test.py
```

### Comparing `corankco-4.0.0/.gitignore` & `corankco-4.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/.idea/corankco.iml` & `corankco-4.0.1/.idea/corankco.iml`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/.idea/dictionaries/pierre.xml` & `corankco-4.0.1/.idea/dictionaries/pierre.xml`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/LICENSE` & `corankco-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/PKG-INFO` & `corankco-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: corankco
-Version: 4.0.0
+Version: 4.0.1
 Summary: Kemeny-Young method for rank aggregation of incomplete rankings with ties
 Home-page: https://github.com/pierreandrieu/corankco
 Author: Pierre Andrieu
 Author-email: pierre.andrieu@lilo.org
 License: MIT
 Description: corankco
         ===============
```

### Comparing `corankco-4.0.0/README.md` & `corankco-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/algorithmChoice.py` & `corankco-4.0.1/corankco/algorithms/algorithmChoice.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/alltied/all_tied.py` & `corankco-4.0.1/corankco/algorithms/alltied/all_tied.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/bioconsert/bioconsert.py` & `corankco-4.0.1/corankco/algorithms/bioconsert/bioconsert.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/borda/borda.py` & `corankco-4.0.1/corankco/algorithms/borda/borda.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/copeland/copeland.py` & `corankco-4.0.1/corankco/algorithms/copeland/copeland.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/exact/exactalgorithm.py` & `corankco-4.0.1/corankco/algorithms/exact/exactalgorithm.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/exact/exactalgorithmcplex.py` & `corankco-4.0.1/corankco/algorithms/exact/exactalgorithmcplex.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/exact/exactalgorithmcplex2.py` & `corankco-4.0.1/corankco/algorithms/exact/exactalgorithmcplex2.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/exact/exactalgorithmgeneric.py` & `corankco-4.0.1/corankco/algorithms/exact/exactalgorithmgeneric.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/exact/exactpreprocess.py` & `corankco-4.0.1/corankco/algorithms/exact/exactpreprocess.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/kwiksort/kwiksortabs.py` & `corankco-4.0.1/corankco/algorithms/kwiksort/kwiksortabs.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/kwiksort/kwiksortrandom.py` & `corankco-4.0.1/corankco/algorithms/kwiksort/kwiksortrandom.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/median_ranking.py` & `corankco-4.0.1/corankco/algorithms/median_ranking.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/medrank/medrank.py` & `corankco-4.0.1/corankco/algorithms/medrank/medrank.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/parcons/parcons.py` & `corankco-4.0.1/corankco/algorithms/parcons/parcons.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/pickaperm/pickaperm.py` & `corankco-4.0.1/corankco/algorithms/pickaperm/pickaperm.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/algorithms/repeatchoice/repeatchoice.py` & `corankco-4.0.1/corankco/algorithms/repeatchoice/repeatchoice.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/consensus.py` & `corankco-4.0.1/corankco/consensus.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/dataset.py` & `corankco-4.0.1/corankco/dataset.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/experimentsVLDB/bench.py` & `corankco-4.0.1/corankco/experimentsVLDB/bench.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,28 +113,26 @@
     def _run_raw_data(self) -> str:
         res = "dataset;nb_elements"
         for scoring_scheme in self.__scoring_schemes:
             res += ";" + scoring_scheme.get_nickname()
         res += "\n"
         flag = [True] * len(self.__scoring_schemes)
         for dataset in sorted(self.datasets):
-            print(dataset.name + " " + str(dataset.n))
             res += dataset.name + ";" + str(dataset.n)
             id_scoring_scheme = 0
             for scoring_scheme in self.__scoring_schemes:
                 if flag[id_scoring_scheme]:
                     time_computation = self.__alg.bench_time_consensus(dataset, scoring_scheme, True)
                     if time_computation > self.__max_time:
                         flag[id_scoring_scheme] = False
                 else:
                     time_computation = float('inf')
                 res += ";" + str(time_computation)
                 id_scoring_scheme += 1
             res += "\n"
-        print(res)
         return res
 
     def _run_final_data(self, raw_data: str) -> str:
         res = "size_datasets"
         for sc in self.__scoring_schemes:
             res += ";"+sc.get_nickname() + "_mean_time"
         res += "\n"
```

### Comparing `corankco-4.0.0/corankco/experimentsVLDB/disease.py` & `corankco-4.0.1/corankco/experimentsVLDB/disease.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/experimentsVLDB/experiment.py` & `corankco-4.0.1/corankco/experimentsVLDB/experiment.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/experimentsVLDB/experimentOrphanet.py` & `corankco-4.0.1/corankco/experimentsVLDB/experimentOrphanet.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/experimentsVLDB/gene.py` & `corankco-4.0.1/corankco/experimentsVLDB/gene.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/experimentsVLDB/geneNcbiParser.py` & `corankco-4.0.1/corankco/experimentsVLDB/geneNcbiParser.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/experimentsVLDB/mapping_ncbi_orphanet.py` & `corankco-4.0.1/corankco/experimentsVLDB/mapping_ncbi_orphanet.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/experimentsVLDB/marksExperiment.py` & `corankco-4.0.1/corankco/experimentsVLDB/marksExperiment.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/experimentsVLDB/ncbi_query_factory.py` & `corankco-4.0.1/corankco/experimentsVLDB/ncbi_query_factory.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/experimentsVLDB/orphanet_parser.py` & `corankco-4.0.1/corankco/experimentsVLDB/orphanet_parser.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/experimentsVLDB/reproduce_experiments_vldb/reproduce_experiments_test_version.py` & `corankco-4.0.1/corankco/experimentsVLDB/reproduce_experiments_vldb/reproduce_experiments_test_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         top_k_to_test=[10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110],
         # algorithm to compute the consensus
         algo=get_algorithm(alg=Algorithm.ParCons, parameters={"bound_for_exact": 150,
                                                               "auxiliary_algorithm":
                                                                   get_algorithm(alg=Algorithm.BioConsert)}),
         # selects all the tuples of rankings with at least 100 elements and 3 rankings
         # dataset_selector=DatasetSelector(nb_elem_min=100, nb_rankings_min=3)
-        dataset_selector=DatasetSelector(nb_elem_min=100, nb_rankings_min=3)
+        dataset_selector=DatasetSelector(nb_elem_min=100, nb_rankings_min=3),
 
     )
 
     # run experiment and print results. If raw_data is true: also print all parameters of experiment (readme)
     # and the raw data that was used to compute the final data. If parameter is false, only final data is displayed
     exp1.run(raw_data, figures=figures)
```

### Comparing `corankco-4.0.0/corankco/kemeny_computation.py` & `corankco-4.0.1/corankco/kemeny_computation.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/kemeny_computation_these.py` & `corankco-4.0.1/corankco/kemeny_computation_these.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/partitioning/parfront.py` & `corankco-4.0.1/corankco/partitioning/parfront.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/rankingsgeneration/rankingsgenerate.py` & `corankco-4.0.1/corankco/rankingsgeneration/rankingsgenerate.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/scoringscheme.py` & `corankco-4.0.1/corankco/scoringscheme.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco/utils.py` & `corankco-4.0.1/corankco/utils.py`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/corankco.egg-info/PKG-INFO` & `corankco-4.0.1/corankco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: corankco
-Version: 4.0.0
+Version: 4.0.1
 Summary: Kemeny-Young method for rank aggregation of incomplete rankings with ties
 Home-page: https://github.com/pierreandrieu/corankco
 Author: Pierre Andrieu
 Author-email: pierre.andrieu@lilo.org
 License: MIT
 Description: corankco
         ===============
```

### Comparing `corankco-4.0.0/corankco.egg-info/SOURCES.txt` & `corankco-4.0.1/corankco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/data/dataGeneNCBI.txt` & `corankco-4.0.1/data/dataGeneNCBI.txt`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/data/en_product6.xml` & `corankco-4.0.1/data/en_product6.xml`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/data/mappingDiseaseID.csv` & `corankco-4.0.1/data/mappingDiseaseID.csv`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/data/mapping_genes_geneNCBI_orphanet.csv` & `corankco-4.0.1/data/mapping_genes_geneNCBI_orphanet.csv`

 * *Files identical despite different names*

### Comparing `corankco-4.0.0/setup.py` & `corankco-4.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(name='corankco',
-      version='4.0.0',
+      version='4.0.1',
       description='Kemeny-Young method for rank aggregation of incomplete rankings with ties',
       long_description=readme(),
       url='https://github.com/pierreandrieu/corankco',
       author='Pierre Andrieu',
       author_email='pierre.andrieu@lilo.org',
       license='MIT',
       packages=find_packages(include=['corankco', 'corankco.*']),
```

### Comparing `corankco-4.0.0/tests/test.py` & `corankco-4.0.1/tests/test.py`

 * *Files identical despite different names*

