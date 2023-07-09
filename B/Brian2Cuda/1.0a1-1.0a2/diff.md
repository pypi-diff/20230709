# Comparing `tmp/Brian2CUDA-1.0a1.tar.gz` & `tmp/Brian2Cuda-1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Brian2CUDA-1.0a1.tar", last modified: Wed Jun 29 10:04:30 2022, max compression
+gzip compressed data, was "Brian2Cuda-1.0a2.tar", last modified: Sun Jul  9 11:51:08 2023, max compression
```

## Comparing `Brian2CUDA-1.0a1.tar` & `Brian2Cuda-1.0a2.tar`

### file list

```diff
@@ -1,108 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 10:04:30.306173 Brian2CUDA-1.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 10:04:30.298174 Brian2CUDA-1.0a1/Brian2CUDA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-06-29 10:04:29.000000 Brian2CUDA-1.0a1/Brian2CUDA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-06-29 10:04:30.000000 Brian2CUDA-1.0a1/Brian2CUDA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 10:04:29.000000 Brian2CUDA-1.0a1/Brian2CUDA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-29 10:04:30.000000 Brian2CUDA-1.0a1/Brian2CUDA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-29 10:04:30.000000 Brian2CUDA-1.0a1/Brian2CUDA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)    35130 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-06-29 10:04:30.306173 Brian2CUDA-1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 10:04:30.306173 Brian2CUDA-1.0a1/brian2cuda/
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-06-29 10:04:30.306173 Brian2CUDA-1.0a1/brian2cuda/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4192 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/binomial.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 10:04:30.302173 Brian2CUDA-1.0a1/brian2cuda/brianlib/
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/brianlib/clocks.h
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/brianlib/common_math.h
--rw-r--r--   0 runner    (1001) docker     (121)     4291 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/brianlib/cudaVector.h
--rw-r--r--   0 runner    (1001) docker     (121)     5369 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/brianlib/cuda_utils.h
--rw-r--r--   0 runner    (1001) docker     (121)     6701 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/brianlib/curand_buffer.h
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/brianlib/dynamic_array.h
--rw-r--r--   0 runner    (1001) docker     (121)    22818 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/brianlib/spikequeue.h
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/brianlib/stdint_compat.h
--rw-r--r--   0 runner    (1001) docker     (121)     4462 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/codeobject.py
--rw-r--r--   0 runner    (1001) docker     (121)    45760 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/cuda_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    11671 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/cuda_prefs.py
--rw-r--r--   0 runner    (1001) docker     (121)   103041 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/device.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 10:04:30.302173 Brian2CUDA-1.0a1/brian2cuda/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9577 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/sphinxext/briandoc.py
--rw-r--r--   0 runner    (1001) docker     (121)    15909 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/sphinxext/docscrape.py
--rw-r--r--   0 runner    (1001) docker     (121)     8470 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/sphinxext/docscrape_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/sphinxext/examplefinder.py
--rw-r--r--   0 runner    (1001) docker     (121)     7704 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/sphinxext/generate_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     9655 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/sphinxext/generate_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 10:04:30.302173 Brian2CUDA-1.0a1/brian2cuda/templates/
--rw-r--r--   0 runner    (1001) docker     (121)    11090 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/common_group.cu
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/common_synapses.cu
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/group_variable_set.cu
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/group_variable_set_conditional.cu
--rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/main.cu
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5179 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/network.cu
--rw-r--r--   0 runner    (1001) docker     (121)    27500 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/objects.cu
--rw-r--r--   0 runner    (1001) docker     (121)    21643 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/rand.cu
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/ratemonitor.cu
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/reset.cu
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/run.cu
--rw-r--r--   0 runner    (1001) docker     (121)    20100 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/spatialstateupdate.cu
--rw-r--r--   0 runner    (1001) docker     (121)     5664 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/spikegenerator.cu
--rw-r--r--   0 runner    (1001) docker     (121)     6937 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/spikemonitor.cu
--rw-r--r--   0 runner    (1001) docker     (121)     3685 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/statemonitor.cu
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/stateupdate.cu
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/summed_variable.cu
--rw-r--r--   0 runner    (1001) docker     (121)    12892 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/synapses.cu
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/synapses_classes.cu
--rw-r--r--   0 runner    (1001) docker     (121)     4905 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/synapses_create_array.cu
--rw-r--r--   0 runner    (1001) docker     (121)    14508 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/synapses_create_generator.cu
--rw-r--r--   0 runner    (1001) docker     (121)    47224 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/synapses_push_spikes.cu
--rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/threshold.cu
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/templates/win_makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 10:04:30.306173 Brian2CUDA-1.0a1/brian2cuda/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     8154 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 10:04:30.306173 Brian2CUDA-1.0a1/brian2cuda/tests/features/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19764 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/features/cuda_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)    33044 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/features/speed.py
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/func_def_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/func_def_cuda.h
--rw-r--r--   0 runner    (1001) docker     (121)     7021 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_cpp_cuda_consistency.py
--rw-r--r--   0 runner    (1001) docker     (121)    10456 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_cuda_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    14077 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_cuda_standalone.py
--rw-r--r--   0 runner    (1001) docker     (121)     6220 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6340 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_gpu_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     5420 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_network_multiple_runs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2733 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_neurongroup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (121)    47363 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_random_number_generation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3403 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_spikegenerator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9678 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_stateupdaters.py
--rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_stringtools.py
--rw-r--r--   0 runner    (1001) docker     (121)    15757 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/tests/test_synaptic_propagations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/timedarray.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 10:04:30.306173 Brian2CUDA-1.0a1/brian2cuda/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21225 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/utils/gputools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/brian2cuda/utils/stringtools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 10:04:30.306173 Brian2CUDA-1.0a1/docs_sphinx/
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/docs_sphinx/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    11360 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/docs_sphinx/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/docs_sphinx/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 10:04:30.306173 Brian2CUDA-1.0a1/docs_sphinx/introduction/
--rw-r--r--   0 runner    (1001) docker     (121)     5357 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/docs_sphinx/introduction/cuda_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/docs_sphinx/introduction/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4468 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/docs_sphinx/introduction/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5024 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/docs_sphinx/introduction/known_issues.rst
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/docs_sphinx/introduction/performance.rst
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/docs_sphinx/introduction/preferences.rst
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/docs_sphinx/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-06-29 10:04:30.306173 Brian2CUDA-1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    81180 2022-06-29 10:04:16.000000 Brian2CUDA-1.0a1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.946671 Brian2Cuda-1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.922670 Brian2Cuda-1.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.926670 Brian2Cuda-1.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      763 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.926670 Brian2Cuda-1.0a2/Brian2Cuda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-07-09 11:51:08.000000 Brian2Cuda-1.0a2/Brian2Cuda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4520 2023-07-09 11:51:08.000000 Brian2Cuda-1.0a2/Brian2Cuda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-09 11:51:08.000000 Brian2Cuda-1.0a2/Brian2Cuda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-07-09 11:51:08.000000 Brian2Cuda-1.0a2/Brian2Cuda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-09 11:51:08.000000 Brian2Cuda-1.0a2/Brian2Cuda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (122)    35130 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-07-09 11:51:08.946671 Brian2Cuda-1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.930670 Brian2Cuda-1.0a2/brian2cuda/
+-rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-09 11:51:08.000000 Brian2Cuda-1.0a2/brian2cuda/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4192 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/binomial.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.930670 Brian2Cuda-1.0a2/brian2cuda/brianlib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/clocks.h
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/common_math.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/cudaVector.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/cuda_utils.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/curand_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/dynamic_array.h
+-rw-r--r--   0 runner    (1001) docker     (122)    22818 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/spikequeue.h
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/brianlib/stdint_compat.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4462 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/codeobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45760 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/cuda_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11671 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/cuda_prefs.py
+-rw-r--r--   0 runner    (1001) docker     (122)   105791 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/device.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.930670 Brian2Cuda-1.0a2/brian2cuda/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9577 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/briandoc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15909 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/docscrape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8470 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/docscrape_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/examplefinder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7704 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/generate_examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9655 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/sphinxext/generate_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.934671 Brian2Cuda-1.0a2/brian2cuda/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)    11160 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/common_group.cu
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/common_synapses.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/group_variable_set.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/group_variable_set_conditional.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/main.cu
+-rw-r--r--   0 runner    (1001) docker     (122)      553 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     5179 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/network.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    27500 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/objects.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    21643 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/rand.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     3240 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/ratemonitor.cu
+-rw-r--r--   0 runner    (1001) docker     (122)      718 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/reset.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/run.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    19800 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/spatialstateupdate.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/spikegenerator.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/spikemonitor.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     3685 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/statemonitor.cu
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/stateupdate.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/summed_variable.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    12745 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/synapses.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/synapses_classes.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/synapses_create_array.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    18225 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/synapses_create_generator.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    47020 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/synapses_push_spikes.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     4272 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/threshold.cu
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/templates/win_makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.938671 Brian2Cuda-1.0a2/brian2cuda/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.938671 Brian2Cuda-1.0a2/brian2cuda/tests/features/
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19764 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/features/cuda_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33044 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/features/speed.py
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/func_def_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/func_def_cuda.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7021 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_cpp_cuda_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10456 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_cuda_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14513 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_cuda_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6378 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_gpu_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5420 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_network_multiple_runs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2733 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_neurongroup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47363 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_random_number_generation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_spikegenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9678 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_stateupdaters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3455 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_stringtools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15757 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/tests/test_synaptic_propagations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/timedarray.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.938671 Brian2Cuda-1.0a2/brian2cuda/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21225 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/utils/gputools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4201 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/brian2cuda/utils/stringtools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.938671 Brian2Cuda-1.0a2/docs_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (122)      580 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)    11360 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.938671 Brian2Cuda-1.0a2/docs_sphinx/introduction/
+-rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/introduction/cuda_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/introduction/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4468 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/introduction/install.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5024 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/introduction/known_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/introduction/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/introduction/preferences.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/docs_sphinx/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.942671 Brian2Cuda-1.0a2/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/TODO.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7242 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/brunelhakim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7993 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/cobahh.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.942671 Brian2Cuda-1.0a2/examples/compartmental/
+-rw-r--r--   0 runner    (1001) docker     (122)     1976 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/bipolar_cell_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/bipolar_cell_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/bipolar_with_inputs2_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/bipolar_with_inputs2_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/bipolar_with_inputs_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/bipolar_with_inputs_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3107 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/hh_with_spikes_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/hh_with_spikes_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/hodgkin_huxley_1952_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/hodgkin_huxley_1952_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3384 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/lfp_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3428 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/lfp_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.942671 Brian2Cuda-1.0a2/examples/compartmental/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/plots/all_plots_combined.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/plots/hh_with_spikes_checkresults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/rall_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2741 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/rall_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/spike_initiation_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/compartmental/spike_initiation_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4869 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/cuba.py
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/figures.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (122)    10691 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/mushroombody.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/run_examples.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     8794 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/stdp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5443 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-09 11:51:08.942671 Brian2Cuda-1.0a2/frozen_repos/
+-rw-r--r--   0 runner    (1001) docker     (122)    21214 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/frozen_repos/brian2.diff
+-rw-r--r--   0 runner    (1001) docker     (122)     4490 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/frozen_repos/brian2genn.diff
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/frozen_repos/init_genn.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/frozen_repos/submodules_update.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/frozen_repos/update_brian2.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/frozen_repos/update_brian2genn.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-07-09 11:50:56.000000 Brian2Cuda-1.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-09 11:51:08.946671 Brian2Cuda-1.0a2/setup.cfg
```

### Comparing `Brian2CUDA-1.0a1/Brian2CUDA.egg-info/PKG-INFO` & `Brian2Cuda-1.0a2/Brian2Cuda.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
-Name: Brian2CUDA
-Version: 1.0a1
-Summary: A Brian2 extention to simulate spiking neural networks on GPUs
-Home-page: http://github.com/brian-team/brian2cuda
-Author: Denis Alevi, Moritz Augustin and Marcel Stimberg
-Author-email: mail@denisalevi.de
-Project-URL: Documentation, https://brian2cuda.readthedocs.io/en/latest/
-Project-URL: Bug tracker, https://github.com/brian-team/brian2cuda/issues
-Keywords: computational neuroscience simulation
-Classifier: Development Status :: 4 - Beta
+Name: Brian2Cuda
+Version: 1.0a2
+Summary: A Brian2 extension to simulate spiking neural networks on GPUs
+Author: Denis Alevi, Moritz Augustin, Marcel Stimberg
+Project-URL: Documentation, https://brian2cuda.readthedocs.io/
+Project-URL: Source, https://github.com/brian-team/brian2cuda
+Project-URL: Tracker, https://github.com/brian-team/brian2cuda/issues
+Keywords: computational neuroscience,simulation,neural networks,spiking neurons,gpu,cuda
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Provides: brian2cuda
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 Brian2CUDA
 ==========
@@ -36,41 +34,41 @@
 [GitHub issue tracker](https://github.com/brian-team/brian2cuda/issues).
 
 For **installation and usage instructions**, check out the
 [Brian2CUDA documentation](https://brian2cuda.readthedocs.io).
 For information on general Brian2 usage, check out the
 [Brian2 documentation](http://brian2.readthedocs.io).
 
-### Quick start
-#### Installation
+## Quick start
+### Installation
 
 You can install Brian2CUDA via `pip`:
 
 ```bash
 python -m pip install brian2cuda
 ```
 
 This will install a compatible version of Brian2 as dependency. For installation requirements and GPU configuration, check out the [Brian2CUDA documentation](https://brian2cuda.readthedocs.io/en/latest/index.html).
 
-#### Usage
+### Usage
 Use your Brian2 code (see [Brian2 documentation](http://brian2.readthedocs.io/en/stable/index.html)) and modify the imports to:
 
 ```python
 # Standard Brian2 import
 from brian2 import *
 
 # Enable GPU usage via Brian2CUDA
 import brian2cuda
 set_device("cuda_standalone")
 ```
 
 See [Brian2's standalone code generation](https://brian2.readthedocs.io/en/stable/user/computation.html?highlight=set_device#standalone-code-generation) for more options for the `set_device` call.
 
 
-### Citation
+## Citation
 If you use this software in a published article, please cite
 [our Brian2CUDA publication](https://www.frontiersin.org/articles/10.3389/fninf.2022.883700):
 
 > Alevi, D, Stimberg, M, Sprekeler, H, Obermayer, K, Augustin, M. “Brian2CUDA: flexible and efficient simulation of spiking neural network models on GPUs” Frontiers in Neuroinformatics (2022). doi: 10.3389/fninf.2022.883700.
 
-### License
+## License
 Brian2CUDA is free software licensed under the [GNU General Public License v3 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).
```

### Comparing `Brian2CUDA-1.0a1/CITATION.cff` & `Brian2Cuda-1.0a2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/LICENSE` & `Brian2Cuda-1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/PKG-INFO` & `Brian2Cuda-1.0a2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
-Name: Brian2CUDA
-Version: 1.0a1
-Summary: A Brian2 extention to simulate spiking neural networks on GPUs
-Home-page: http://github.com/brian-team/brian2cuda
-Author: Denis Alevi, Moritz Augustin and Marcel Stimberg
-Author-email: mail@denisalevi.de
-Project-URL: Documentation, https://brian2cuda.readthedocs.io/en/latest/
-Project-URL: Bug tracker, https://github.com/brian-team/brian2cuda/issues
-Keywords: computational neuroscience simulation
-Classifier: Development Status :: 4 - Beta
+Name: Brian2Cuda
+Version: 1.0a2
+Summary: A Brian2 extension to simulate spiking neural networks on GPUs
+Author: Denis Alevi, Moritz Augustin, Marcel Stimberg
+Project-URL: Documentation, https://brian2cuda.readthedocs.io/
+Project-URL: Source, https://github.com/brian-team/brian2cuda
+Project-URL: Tracker, https://github.com/brian-team/brian2cuda/issues
+Keywords: computational neuroscience,simulation,neural networks,spiking neurons,gpu,cuda
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Provides: brian2cuda
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 Brian2CUDA
 ==========
@@ -36,41 +34,41 @@
 [GitHub issue tracker](https://github.com/brian-team/brian2cuda/issues).
 
 For **installation and usage instructions**, check out the
 [Brian2CUDA documentation](https://brian2cuda.readthedocs.io).
 For information on general Brian2 usage, check out the
 [Brian2 documentation](http://brian2.readthedocs.io).
 
-### Quick start
-#### Installation
+## Quick start
+### Installation
 
 You can install Brian2CUDA via `pip`:
 
 ```bash
 python -m pip install brian2cuda
 ```
 
 This will install a compatible version of Brian2 as dependency. For installation requirements and GPU configuration, check out the [Brian2CUDA documentation](https://brian2cuda.readthedocs.io/en/latest/index.html).
 
-#### Usage
+### Usage
 Use your Brian2 code (see [Brian2 documentation](http://brian2.readthedocs.io/en/stable/index.html)) and modify the imports to:
 
 ```python
 # Standard Brian2 import
 from brian2 import *
 
 # Enable GPU usage via Brian2CUDA
 import brian2cuda
 set_device("cuda_standalone")
 ```
 
 See [Brian2's standalone code generation](https://brian2.readthedocs.io/en/stable/user/computation.html?highlight=set_device#standalone-code-generation) for more options for the `set_device` call.
 
 
-### Citation
+## Citation
 If you use this software in a published article, please cite
 [our Brian2CUDA publication](https://www.frontiersin.org/articles/10.3389/fninf.2022.883700):
 
 > Alevi, D, Stimberg, M, Sprekeler, H, Obermayer, K, Augustin, M. “Brian2CUDA: flexible and efficient simulation of spiking neural network models on GPUs” Frontiers in Neuroinformatics (2022). doi: 10.3389/fninf.2022.883700.
 
-### License
+## License
 Brian2CUDA is free software licensed under the [GNU General Public License v3 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).
```

### Comparing `Brian2CUDA-1.0a1/README.md` & `Brian2Cuda-1.0a2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,41 +10,41 @@
 [GitHub issue tracker](https://github.com/brian-team/brian2cuda/issues).
 
 For **installation and usage instructions**, check out the
 [Brian2CUDA documentation](https://brian2cuda.readthedocs.io).
 For information on general Brian2 usage, check out the
 [Brian2 documentation](http://brian2.readthedocs.io).
 
-### Quick start
-#### Installation
+## Quick start
+### Installation
 
 You can install Brian2CUDA via `pip`:
 
 ```bash
 python -m pip install brian2cuda
 ```
 
 This will install a compatible version of Brian2 as dependency. For installation requirements and GPU configuration, check out the [Brian2CUDA documentation](https://brian2cuda.readthedocs.io/en/latest/index.html).
 
-#### Usage
+### Usage
 Use your Brian2 code (see [Brian2 documentation](http://brian2.readthedocs.io/en/stable/index.html)) and modify the imports to:
 
 ```python
 # Standard Brian2 import
 from brian2 import *
 
 # Enable GPU usage via Brian2CUDA
 import brian2cuda
 set_device("cuda_standalone")
 ```
 
 See [Brian2's standalone code generation](https://brian2.readthedocs.io/en/stable/user/computation.html?highlight=set_device#standalone-code-generation) for more options for the `set_device` call.
 
 
-### Citation
+## Citation
 If you use this software in a published article, please cite
 [our Brian2CUDA publication](https://www.frontiersin.org/articles/10.3389/fninf.2022.883700):
 
 > Alevi, D, Stimberg, M, Sprekeler, H, Obermayer, K, Augustin, M. “Brian2CUDA: flexible and efficient simulation of spiking neural network models on GPUs” Frontiers in Neuroinformatics (2022). doi: 10.3389/fninf.2022.883700.
 
-### License
+## License
 Brian2CUDA is free software licensed under the [GNU General Public License v3 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/__init__.py` & `Brian2Cuda-1.0a2/brian2cuda/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,17 +5,34 @@
 from . import cuda_prefs
 from .codeobject import CUDAStandaloneCodeObject
 from .device import cuda_standalone_device
 from . import binomial
 from . import timedarray
 
 
-from . import _version
-
-__version__ = _version.get_versions()["version"]
+try:
+    from ._version import __version__, __version_tuple__
+except ImportError:
+    try:
+        from setuptools_scm import get_version
+
+        __version__ = get_version(
+            root="..",
+            relative_to=__file__,
+            version_scheme="post-release",
+            local_scheme="no-local-version",
+        )
+        __version_tuple__ = tuple(int(x) for x in __version__.split(".")[:3])
+    except ImportError:
+        logging.getLogger("brian2cuda").warn(
+            "Cannot determine Brian2CUDA version, running from source and "
+            "setuptools_scm is not installed."
+        )
+        __version__ = "unknown"
+        __version_tuple__ = (0, 0, 0)
 
 
 # make the test suite available via brian2cuda.test()
 from .tests import run as test
 
 
 def example_run(device_name="cuda_standalone", directory=None, **build_options):
@@ -52,8 +69,8 @@
     )
     G.v = "i / 100."
     run(1 * ms)
     device.build(direct_call=False, directory=directory, **build_options)
     assert_allclose(G.v, np.arange(N) / N * np.exp(-1 * ms / tau))
     device.reinit()
     device.activate()
-    print("\nExample run was successful.")
+    print("\nExample run was successful.")
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/binomial.py` & `Brian2Cuda-1.0a2/brian2cuda/binomial.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/brianlib/clocks.h` & `Brian2Cuda-1.0a2/brian2cuda/brianlib/clocks.h`

 * *Files 9% similar despite different names*

```diff
@@ -2,50 +2,50 @@
 #define _BRIAN_CLOCKS_H
 #include<stdlib.h>
 #include<iostream>
 #include<brianlib/stdint_compat.h>
 #include<math.h>
 
 namespace {
-    inline int fround(double x)
+    inline int64_t fround(double x)
     {
-        return (int)(x+0.5);
+        return (int64_t)(x+0.5);
     };
 };
 
 class Clock
 {
 public:
     double epsilon;
     double *dt;
     int64_t *timestep;
-    double *t;
     int64_t i_end;
+    double *t;
     Clock(double _epsilon=1e-14) : epsilon(_epsilon) { i_end = 0;};
     inline void tick()
     {
         timestep[0] += 1;
         t[0] = timestep[0] * dt[0];
     }
     inline bool running() { return timestep[0]<i_end; };
     void set_interval(double start, double end)
     {
-        int i_start = fround(start/dt[0]);
+        int64_t i_start = fround(start/dt[0]);
         double t_start = i_start*dt[0];
         if(t_start==start || fabs(t_start-start)<=epsilon*fabs(t_start))
         {
             timestep[0] = i_start;
         } else
         {
-            timestep[0] = (int)ceil(start/dt[0]);
+            timestep[0] = (int64_t)ceil(start/dt[0]);
         }
         i_end = fround(end/dt[0]);
         double t_end = i_end*dt[0];
         if(!(t_end==end || fabs(t_end-end)<=epsilon*fabs(t_end)))
         {
-            i_end = (int)ceil(end/dt[0]);
+            i_end = (int64_t)ceil(end/dt[0]);
         }
     }
 };
 
 #endif
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/brianlib/cudaVector.h` & `Brian2Cuda-1.0a2/brian2cuda/brianlib/cudaVector.h`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/brianlib/cuda_utils.h` & `Brian2Cuda-1.0a2/brian2cuda/brianlib/cuda_utils.h`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/brianlib/curand_buffer.h` & `Brian2Cuda-1.0a2/brian2cuda/brianlib/curand_buffer.h`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/brianlib/dynamic_array.h` & `Brian2Cuda-1.0a2/brian2cuda/brianlib/dynamic_array.h`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/brianlib/spikequeue.h` & `Brian2Cuda-1.0a2/brian2cuda/brianlib/spikequeue.h`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/codeobject.py` & `Brian2Cuda-1.0a2/brian2cuda/codeobject.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/cuda_generator.py` & `Brian2Cuda-1.0a2/brian2cuda/cuda_generator.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/cuda_prefs.py` & `Brian2Cuda-1.0a2/brian2cuda/cuda_prefs.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/device.py` & `Brian2Cuda-1.0a2/brian2cuda/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import numpy as np
 
 from brian2.codegen.cpp_prefs import get_compiler_and_args
 from brian2.codegen.translation import make_statements
 from brian2.core.clocks import Clock, defaultclock
 from brian2.core.namespace import get_local_namespace
 from brian2.core.preferences import prefs, PreferenceError
-from brian2.core.variables import ArrayVariable, DynamicArrayVariable
+from brian2.core.variables import ArrayVariable, DynamicArrayVariable, Constant
 from brian2.parsing.rendering import CPPNodeRenderer
 from brian2.devices.device import all_devices
 from brian2.synapses.synapses import Synapses, SynapticPathway
 from brian2.utils.filetools import copy_directory, ensure_directory
 from brian2.utils.stringtools import get_identifiers, stripped_deindented_lines
 from brian2.codegen.generators.cpp_generator import c_data_type
 from brian2.utils.logger import get_logger
@@ -80,15 +80,14 @@
         self.include_dirs.remove('brianlib/randomkit')
         self.library_dirs.remove('brianlib/randomkit')
 
         # Add code line slots used in our benchmarks
         # TODO: Add to brian2 and remove here
         self.code_lines.update({'before_network_run': [],
                                 'after_network_run': []})
-
         ### Attributes specific to CUDAStandaloneDevice:
         # only true during first run call (relevant for synaptic pre/post ID deletion)
         self.first_run = True
         # the minimal supported GPU compute capability
         self.minimal_compute_capability = 3.5
         # store the ID of the used GPU and it's compute capability
         self.gpu_id = None
@@ -338,15 +337,14 @@
                     self.delete_synaptic_post[synaptic_post_array_name] = False
                     if prefs['devices.cuda_standalone.no_post_references']:
                         raise PreferenceError(error_msg.format(prepost='post',
                                                                varname=varname,
                                                                owner=owner))
                 if idx == '_syaptic_post':
                     self.delete_synaptic_post[synaptic_post_array_name] = False
-
         # Collect all variables written to in group_variable_set_templates so they can
         # be copied from device to host after being changed on device
         if template_name in group_variable_set_templates:
             read, write = self.get_array_read_write(abstract_code, variables)
             written_variables = {}
             for variable_name in write:
                 var = variables[variable_name]
@@ -364,15 +362,14 @@
                 read_write = read.union(write)
                 varname = owner.variables['delay'].name
                 if varname in read_write:
                     synaptic_delay_array_name = self.get_array_name(
                         owner.variables['delay'], access_data=False
                     )
                     self.delete_synaptic_delay[synaptic_delay_array_name] = False
-
         if template_name == "synapses":
             prepost = template_kwds['pathway'].prepost
             synaptic_effects = "synapse"
             for varname in variables.keys():
                 if varname in write:
                     idx = variable_indices[varname]
                     if (prepost == 'pre' and idx == '_postsynaptic_idx') or (prepost == 'post' and idx == '_presynaptic_idx'):
@@ -415,14 +412,18 @@
                 template_kwds["no_post_references"] = True
         template_kwds["launch_bounds"] = prefs["devices.cuda_standalone.launch_bounds"]
         template_kwds["sm_multiplier"] = prefs["devices.cuda_standalone.SM_multiplier"]
         template_kwds["syn_launch_bounds"] = prefs["devices.cuda_standalone.syn_launch_bounds"]
         template_kwds["calc_occupancy"] = prefs["devices.cuda_standalone.calc_occupancy"]
         if template_name in ["threshold", "spikegenerator"]:
             template_kwds["extra_threshold_kernel"] = prefs["devices.cuda_standalone.extra_threshold_kernel"]
+        if template_name == "spikemonitor" and '_source_start' in variables:
+            # Provide subgroup start/stop as template keywords for hardcoding into is_in_subgroup
+            template_kwds.update({'_source_start': variables['_source_start'].get_value(),
+                                  '_source_stop': variables['_source_stop'].get_value()})
         codeobj = super(CUDAStandaloneDevice, self).code_object(owner, name, abstract_code, variables,
                                                                 template_name, variable_indices,
                                                                 codeobj_class=codeobj_class,
                                                                 template_kwds=template_kwds,
                                                                 override_conditional_write=override_conditional_write,
                                                                 compiler_kwds=compiler_kwds,
                                                                 )
@@ -568,45 +569,45 @@
                     {{
                         {arrayname}[i] = {rendered_value};
                     }}
                 '''
                 if arrayname not in self.variables_on_host_only:
                     # Copy to device
                     code += f'''
-                        CUDA_SAFE_CALL(
-                            cudaMemcpy(
-                                {pointer_arrayname},
-                                &{arrayname}[0],
-                                sizeof({arrayname}[0])*{size_str},
-                                cudaMemcpyHostToDevice
-                            )
-                        );
-                    '''
+                    CUDA_SAFE_CALL(
+                        cudaMemcpy(
+                            {pointer_arrayname},
+                            &{arrayname}[0],
+                            sizeof({arrayname}[0])*{size_str},
+                            cudaMemcpyHostToDevice
+                        )
+                    );
+                '''
                 main_lines.extend(stripped_deindented_lines(code))
             elif func=='set_by_single_value':
                 arrayname, item, value = args
                 pointer_arrayname = f"dev{arrayname}"
                 if arrayname.endswith('space'):  # eventspace
                     pointer_arrayname += f'[current_idx{arrayname}]'
                 if arrayname in self.dynamic_arrays.values():
                     pointer_arrayname = f"thrust::raw_pointer_cast(&dev{arrayname}[0])"
                 # Set on host
                 code = f"{arrayname}[{item}] = {value};"
                 if arrayname not in self.variables_on_host_only:
                     # Copy to device
                     code += f'''
-                        CUDA_SAFE_CALL(
-                            cudaMemcpy(
-                                {pointer_arrayname} + {item},
-                                &{arrayname}[{item}],
-                                sizeof({arrayname}[{item}]),
-                                cudaMemcpyHostToDevice
-                            )
-                        );
-                    '''
+                    CUDA_SAFE_CALL(
+                        cudaMemcpy(
+                            {pointer_arrayname} + {item},
+                            &{arrayname}[{item}],
+                            sizeof({arrayname}[{item}]),
+                            cudaMemcpyHostToDevice
+                        )
+                    );
+                '''
                 main_lines.extend(stripped_deindented_lines(code))
             elif func=='set_by_array':
                 arrayname, staticarrayname, is_dynamic = args
                 size_str = "_num_" + arrayname
                 if is_dynamic:
                     size_str = arrayname + ".size()"
                 pointer_arrayname = f"dev{arrayname}"
@@ -618,45 +619,45 @@
                     {{
                         {arrayname}[i] = {staticarrayname}[i];
                     }}
                 '''
                 if arrayname not in self.variables_on_host_only:
                     # Copy to device
                     code += f'''
-                        CUDA_SAFE_CALL(
-                            cudaMemcpy(
-                                {pointer_arrayname},
-                                &{arrayname}[0],
-                                sizeof({arrayname}[0])*{size_str},
-                                cudaMemcpyHostToDevice
-                            )
-                        );
-                    '''
+                    CUDA_SAFE_CALL(
+                        cudaMemcpy(
+                            {pointer_arrayname},
+                            &{arrayname}[0],
+                            sizeof({arrayname}[0])*{size_str},
+                            cudaMemcpyHostToDevice
+                        )
+                    );
+                '''
                 main_lines.extend(stripped_deindented_lines(code))
             elif func=='set_array_by_array':
                 arrayname, staticarrayname_index, staticarrayname_value = args
                 # Set on host
                 code = f'''
                     for(int i=0; i<_num_{staticarrayname_index}; i++)
                     {{
                         {arrayname}[{staticarrayname_index}[i]] = {staticarrayname_value}[i];
                     }}
                 '''
                 if arrayname not in self.variables_on_host_only:
                     # Copy to device
                     code += f'''
-                        CUDA_SAFE_CALL(
-                            cudaMemcpy(
-                                dev{arrayname},
-                                &{arrayname}[0],
-                                sizeof({arrayname}[0])*_num_{arrayname},
-                                cudaMemcpyHostToDevice
-                            )
-                        );
-                    '''
+                    CUDA_SAFE_CALL(
+                        cudaMemcpy(
+                            dev{arrayname},
+                            &{arrayname}[0],
+                            sizeof({arrayname}[0])*_num_{arrayname},
+                            cudaMemcpyHostToDevice
+                        )
+                    );
+                '''
                 main_lines.extend(stripped_deindented_lines(code))
             elif func=='resize_array':
                 array_name, new_size = args
                 code = f'''
                     {array_name}.resize({new_size});
                     THRUST_CHECK_ERROR(dev{array_name}.resize({new_size}));
                 '''
@@ -706,24 +707,25 @@
         writer.write('main.cu', main_tmp)
 
     def generate_codeobj_source(self, writer):
         code_object_defs = defaultdict(list)
         host_parameters = defaultdict(list)
         kernel_parameters = defaultdict(list)
         kernel_constants = defaultdict(list)
+        additional_host_code = defaultdict(list)
         c_float_dtype = c_data_type(prefs['core.default_float_dtype'])
         c_int_dtype = 'unsigned int'
         # Generate data for non-constant values
         for codeobj in self.code_objects.values():
             code_object_defs_lines = []
             code_object_defs_lines_host_only = []
             host_parameters_lines = []
             kernel_parameters_lines = []
             kernel_constants_lines = []
-            additional_code = []
+            additional_host_code_lines = []
             number_elements = ""
             if hasattr(codeobj, 'owner') and hasattr(codeobj.owner, '_N') and codeobj.owner._N != 0:
                 number_elements = str(codeobj.owner._N)
             else:
                 number_elements = "_N"
             # We need the functions to be sorted by keys for reproducable rng with a
             # given seed: For codeobjects that are only run once, we generate the random
@@ -762,15 +764,15 @@
                                     dev_array_randn,
                                     _randn_N*{num_calls},
                                     0,  // mean
                                     1   // stddev
                                 )
                             );
                         '''
-                        additional_code.append(code)
+                        additional_host_code_lines.append(code)
                         kernel_parameters_lines.append(
                             f"{c_float_dtype}* _ptr_array_{codeobj.name}_randn"
                         )
                         host_parameters_lines.append("dev_array_randn")
                     elif k == "rand":
                         num_calls = codeobj.rng_calls["rand"]
                         code = f'''
@@ -788,15 +790,15 @@
                                 curandGenerateUniform{curand_suffix}(
                                     curand_generator,
                                     dev_array_rand,
                                     _rand_N*{num_calls}
                                 )
                             );
                         '''
-                        additional_code.append(code)
+                        additional_host_code_lines.append(code)
                         kernel_parameters_lines.append(
                             f"{c_float_dtype}* _ptr_array_{codeobj.name}_rand"
                         )
                         host_parameters_lines.append("dev_array_rand")
                     elif k == "poisson":
                         # We are assuming that there can be at most one poisson call per expression,
                         # else brian2 should raise a NotImplementedError due to multiple stateful function calls.
@@ -832,15 +834,15 @@
                                         curand_generator,
                                         dev_array_{poisson_name},
                                         _{poisson_name}_N*{num_calls},
                                         {lamda}
                                     )
                                 );
                             '''
-                            additional_code.append(code)
+                            additional_host_code_lines.append(code)
                             kernel_parameters_lines.append(
                                 f"{c_int_dtype}* _ptr_array_{codeobj.name}_{poisson_name}"
                             )
                             host_parameters_lines.append(f"dev_array_{poisson_name}")
                 # Clock variables (t, dt, timestep)
                 elif hasattr(v, 'owner') and isinstance(v.owner, Clock):
                     # Clocks only run on the host and the corresponding device variables are copied
@@ -922,19 +924,27 @@
                                         bare_array_name = self.get_array_name(v)
                                         idx = f'[current_idx{bare_array_name}]'
                                     host_parameters_lines.append(f"{array_name}{idx}")
                                     kernel_parameters_lines.append(f'{dtype}* {ptr_array_name}')
 
                                 # Add size variables `_num{array}` only once
                                 if n_prefix == 0:
-                                    code_object_defs_lines.append(f'const int _num{k} = {v.size};')
-                                    kernel_constants_lines.append(f'const int _num{k} = {v.size};')
+                                    line = f'const int _num{k} = {v.size};'
+                                    code_object_defs_lines.append(line)
+                                    kernel_constants_lines.append(line)
 
                         except TypeError:
                             pass
+                # Constant variables
+                elif isinstance(v, Constant):
+                    rendered_value = CPPNodeRenderer().render_expr(repr(v.value))
+                    c_type = c_data_type(v.dtype)
+                    line = f'const {c_type} {k} = {rendered_value};'
+                    code_object_defs_lines.append(line)
+                    kernel_constants_lines.append(line)
 
             # This rand stuff got a little messy... we pass a device pointer as kernel variable and have a hash define for rand() -> _ptr_..._rand[]
             # The device pointer is advanced every clock cycle in rand.cu and reset when the random number buffer is refilled (also in rand.cu)
             # TODO can we just include this in the k == 'rand' test above?
             # RAND
             if codeobj.rng_calls["rand"] >= 1 and codeobj.runs_every_tick:
                 host_parameters_lines.append(f"dev_{codeobj.name}_rand")
@@ -973,49 +983,48 @@
                     host_parameters[codeobj.name].append(line)
             for line in kernel_parameters_lines:
                 if not line in kernel_parameters[codeobj.name]:
                     kernel_parameters[codeobj.name].append(line)
             for line in chain(kernel_constants_lines):
                 if not line in kernel_constants[codeobj.name]:
                     kernel_constants[codeobj.name].append(line)
-
-            for line in additional_code:
-                if not line in code_object_defs[codeobj.name]:
-                    code_object_defs[codeobj.name].append(line)
+            for line in additional_host_code_lines:
+                if not line in additional_host_code[codeobj.name]:
+                    additional_host_code[codeobj.name].append(line)
 
         # Generate the code objects
         for codeobj in self.code_objects.values():
             ns = codeobj.variables
 
             def _replace_constants_and_parameters(code):
                 # HOST_CONSTANTS are equivalent to C++ Standalone's CONSTANTS
                 code = code.replace('%HOST_CONSTANTS%', '\n\t\t'.join(code_object_defs[codeobj.name]))
+                # ADDITIONAL_HOST_CODE is extra code, which needs `_N`
+                code = code.replace('%ADDITIONAL_HOST_CODE%', '\n\t\t'.join(additional_host_code[codeobj.name]))
                 # KERNEL_CONSTANTS are the same for inside device kernels
                 code = code.replace('%KERNEL_CONSTANTS%', '\n\t'.join(kernel_constants[codeobj.name]))
                 # HOST_PARAMETERS are parameters that device kernels are called with from host code
                 code = code.replace('%HOST_PARAMETERS%', ',\n\t\t\t'.join(host_parameters[codeobj.name]))
                 # KERNEL_PARAMETERS are the same names of the same parameters inside the device kernels
                 code = code.replace('%KERNEL_PARAMETERS%', ',\n\t'.join(kernel_parameters[codeobj.name]))
                 code = code.replace('%CODEOBJ_NAME%', codeobj.name)
                 return code
 
             # Before/after run code
             for block in codeobj.before_after_blocks:
                 cu_code = getattr(codeobj.code, block + '_cu_file')
-                cu_code = self.freeze(cu_code, ns)
                 cu_code = _replace_constants_and_parameters(cu_code)
                 h_code = getattr(codeobj.code, block + '_h_file')
                 writer.write('code_objects/' + block + '_' + codeobj.name + '.cu',
                              cu_code)
                 writer.write('code_objects/' + block + '_' + codeobj.name + '.h',
                              h_code)
 
             # Main code
-            # TODO: fix these freeze/HOST_CONSTANTS hacks somehow - they work but not elegant.
-            code = self.freeze(codeobj.code.cu_file, ns)
+            code = codeobj.code.cu_file
 
             if len(host_parameters[codeobj.name]) == 0:
                 host_parameters[codeobj.name].append("0")
                 kernel_parameters[codeobj.name].append("int dummy")
 
             code = _replace_constants_and_parameters(code)
 
@@ -1376,21 +1385,17 @@
         if len(non_unique_names):
             formatted_names = ', '.join(f"'{name}'"
                                         for name in non_unique_names)
             raise ValueError('All objects need to have unique names in '
                              'standalone mode, the following name(s) were used '
                              'more than once: %s' % formatted_names)
 
-        net_synapses = [s for net in self.networks
-                        for s in net.objects
-                        if isinstance(s, Synapses)]
-
         # Collect all multisynaptic indices in all Synapses (that have them)
         self.multisyn_vars = []
-        for syn in net_synapses:
+        for syn in self.synapses:
             if syn.multisynaptic_index is not None:
                 self.multisyn_vars.append(syn.variables[syn.multisynaptic_index])
 
         # Collect all variables that are stored on host only and should not be copied
         # from device to host at all (e.g. when set by constant or array or at the end
         # of the simulation)
         self.variables_on_host_only = []
@@ -1423,15 +1428,14 @@
                 # set to be deleted during variable set calls (in
                 # self.variableview_set_with_index_array and self.fill_with_array)
                 if varname not in self.delete_synaptic_delay:
                     self.delete_synaptic_delay[varname] = True
                     # This avoids copying the delted delay array from device to host
                     # at the end of the simulation
                     self.variables_on_host_only.append(varname)
-
         self.generate_main_source(self.writer)
 
         # Create lists of codobjects using rand, randn, poisson or binomial across all
         # runs (needed for variable declarations).
         #   - Variables needed for device side rand/randn/poisson are declared in objects.cu:
         #     codeobjects_with_rng["host_api"]["all_runs"]['rand'/'rand'/'poisson'] are needed in `generate_objects_source`
         #   - Variables needed for device side binomial functions are initialized in rand.cu:
@@ -1440,42 +1444,46 @@
             for key in run_codeobj.keys():
                 # keys: 'rand', 'randn', 'poisson-<idx>'
                 self.codeobjects_with_rng["host_api"]["all_runs"][key].extend(run_codeobj[key])
 
         self.generate_codeobj_source(self.writer)
 
         self.generate_objects_source(self.writer, self.arange_arrays,
-                                     net_synapses, self.static_array_specs,
+                                     self.synapses, self.static_array_specs,
                                      self.networks)
         self.generate_network_source(self.writer)
         self.generate_synapses_classes_source(self.writer)
         self.generate_run_source(self.writer)
         self.generate_rand_source(self.writer)
         self.copy_source_files(self.writer, directory)
 
         self.writer.source_files.update(additional_source_files)
 
         self.generate_makefile(self.writer, cpp_compiler,
                                cpp_compiler_flags,
                                cpp_linker_flags,
                                debug,
                                disable_asserts)
-
         # Not sure what the best place is to call Network.after_run -- at the
         # moment the only important thing it does is to clear the objects stored
         # in magic_network. If this is not done, this might lead to problems
         # for repeated runs of standalone (e.g. in the test suite).
         for net in self.networks:
             net.after_run()
 
         logger.info("Using the following preferences for CUDA standalone:")
         for pref_name in prefs:
             if "devices.cuda_standalone" in pref_name:
                 logger.info(f"\t{pref_name} = {prefs[pref_name]}")
 
+        logger.debug("Using the following brian preferences:")
+        for pref_name in prefs:
+            if "devices.cuda_standalone" not in pref_name:
+                logger.debug(f"\t{pref_name} = {prefs[pref_name]}")
+
         if compile:
             self.compile_source(directory, cpp_compiler, debug, clean)
             if run:
                 self.run(directory, with_output, run_args)
 
     def network_run(self, net, duration, report=None, report_period=10*second,
                     namespace=None, profile=False, level=0, **kwds):
@@ -1492,27 +1500,27 @@
 
         # Allow setting `profile` in the `set_device` call (used e.g. in brian2cuda
         # SpeedTest configurations)
         if 'profile' in self.build_options:
             build_profile = self.build_options.pop('profile')
             if build_profile:
                 self.enable_profiling = True
-
         all_objects = net.sorted_objects
         net._clocks = {obj.clock for obj in all_objects}
         t_end = net.t+duration
         for clock in net._clocks:
             clock.set_interval(net.t, t_end)
 
         # Get the local namespace
         if namespace is None:
             namespace = get_local_namespace(level=level+2)
 
         net.before_run(namespace)
-
+        self.synapses |= {s for s in net.objects
+                          if isinstance(s, Synapses)}
         self.clocks.update(net._clocks)
         net.t_ = float(t_end)
 
         # TODO: remove this horrible hack
         for clock in self.clocks:
             if clock.name=='clock':
                 clock._name = '_clock'
@@ -1667,36 +1675,67 @@
         # run everything that is run on a clock
         run_lines.append(
             f'{net.name}.run({float(duration)!r}, {report_call}, {float(report_period)!r});'
         )
         run_lines.extend(self.code_lines['after_network_run'])
         # for multiple runs, the random number buffer needs to be reset
         run_lines.append('random_number_buffer.run_finished();')
+        # nvprof stuff
+        run_lines.append('CUDA_SAFE_CALL(cudaDeviceSynchronize());')
+        run_lines.append('CUDA_SAFE_CALL(cudaProfilerStop());')
 
         self.main_queue.append(('run_network', (net, run_lines)))
 
+        net.after_run()
+
         # Manually set the cache for the clocks, simulation scripts might
         # want to access the time (which has been set in code and is therefore
         # not accessible by the normal means until the code has been built and
         # run)
         for clock in net._clocks:
             self.array_cache[clock.variables['timestep']] = np.array([clock._i_end])
             self.array_cache[clock.variables['t']] = np.array([clock._i_end * clock.dt_])
 
+        # Initialize eventspaces with -1 before the network runs
+        for codeobj in self.code_objects.values():
+            if codeobj.template_name == "threshold" or codeobj.template_name == "spikegenerator":
+                for key in codeobj.variables.keys():
+                    if key.endswith('space'):  # get the correct eventspace name
+                        eventspace_name = self.get_array_name(codeobj.variables[key], False)
+                        # In case of custom scheduling, the thresholder might come after synapses or monitors
+                        # and needs to be initialized in the beginning of the simulation
+
+                        # See generate_main_source() for main_queue formats
+
+                        # Initialize entire eventspace array with -1 at beginning of main
+                        self.main_queue.insert(
+                            0,  # list insert position
+                            # func            , (arrayname, value, is_dynamic)
+                            ('set_by_constant', (eventspace_name, -1, False))
+                        )
+                        # Set the last value (index N) in the eventspace array to 0 (-> event counter)
+                        self.main_queue.insert(
+                            1,  # list insert position
+                            (
+                                'set_by_single_value',  # func
+                                # arrayname     , item,                                , value
+                                (eventspace_name, f"_num_{eventspace_name} - 1", 0)
+                            )
+                        )
+
         if self.build_on_run:
             if self.has_been_run:
                 raise RuntimeError('The network has already been built and run '
                                    'before. Use set_device with '
                                    'build_on_run=False and an explicit '
                                    'device.build call to use multiple run '
                                    'statements with this device.')
             self.build(direct_call=False, **self.build_options)
 
         self.first_run = False
-
     def fill_with_array(self, var, *args, **kwargs):
         # If the delay variable is set after the first run call, do not delete it on the
         # device (which is happening by default)
         if not self.first_run and var.name == 'delay':
             synaptic_delay_array_name = self.get_array_name(var, access_data=False)
             self.delete_synaptic_delay[synaptic_delay_array_name] = False
         super().fill_with_array(var, *args, **kwargs)
@@ -1706,15 +1745,14 @@
         # device (which is happening by default)
         if not self.first_run and variableview.name == 'delay':
             synaptic_delay_array_name = self.get_array_name(variableview.variable,
                                                             access_data=False)
             self.delete_synaptic_delay[synaptic_delay_array_name] = False
         super().variableview_set_with_index_array(variableview, *args, **kwargs)
 
-
     def network_store(self, net, *args, **kwds):
         raise NotImplementedError(('The store/restore mechanism is not '
                                    'supported in CUDA standalone'))
 
     def network_restore(self, net, *args, **kwds):
         raise NotImplementedError(('The store/restore mechanism is not '
                                    'supported in CUDA standalone'))
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/sphinxext/briandoc.py` & `Brian2Cuda-1.0a2/brian2cuda/sphinxext/briandoc.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/sphinxext/docscrape.py` & `Brian2Cuda-1.0a2/brian2cuda/sphinxext/docscrape.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/sphinxext/docscrape_sphinx.py` & `Brian2Cuda-1.0a2/brian2cuda/sphinxext/docscrape_sphinx.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/sphinxext/examplefinder.py` & `Brian2Cuda-1.0a2/brian2cuda/sphinxext/examplefinder.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/sphinxext/generate_examples.py` & `Brian2Cuda-1.0a2/brian2cuda/sphinxext/generate_examples.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/sphinxext/generate_reference.py` & `Brian2Cuda-1.0a2/brian2cuda/sphinxext/generate_reference.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/common_group.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/common_group.cu`

 * *Files 2% similar despite different names*

```diff
@@ -115,26 +115,23 @@
     %KERNEL_PARAMETERS%
     )
 {
     using namespace brian;
 
     int tid = threadIdx.x;
     int bid = blockIdx.x;
-
-    int _idx = bid * THREADS_PER_BLOCK + tid;
+    int _idx = bid * blockDim.x + tid;
     int _vectorisation_idx = _idx;
 
     ///// KERNEL_CONSTANTS /////
     %KERNEL_CONSTANTS%
 
     ///// kernel_lines /////
     {{kernel_lines|autoindent}}
 
-    assert(THREADS_PER_BLOCK == blockDim.x);
-
     {% block additional_variables %}
     {% endblock %}
 
     if(_vectorisation_idx >= _N)
     {
         return;
     }
@@ -154,34 +151,40 @@
         {% block extra_vector_code %}
         {% endblock %}
     }
     {% endblock kernel_maincode %}
 }
 {% endblock kernel %}
 
+{% block extra_kernel_definitions %}
+{% endblock %}
+
 
 void _run_{{codeobj_name}}()
 {
     using namespace brian;
 
     {% block profiling_start %}
     {% if profiled %}
     const std::clock_t _start_time = std::clock();
     {% endif %}
     {% endblock %}
 
+    ///// HOST_CONSTANTS ///////////
+    %HOST_CONSTANTS%
+
     {% block define_N %}
     {# N is a constant in most cases (NeuronGroup, etc.), but a scalar array for
-       synapses, we therefore have to take care to get its value in the right
-       way. #}
+        synapses, we therefore have to take care to get its value in the right
+            way. #}
     const int _N = {{constant_or_scalar('N', variables['N'])}};
     {% endblock %}
 
-    ///// HOST_CONSTANTS ///////////
-    %HOST_CONSTANTS%
+    ///// ADDITIONAL_HOST_CODE /////
+    %ADDITIONAL_HOST_CODE%
 
     {% block host_maincode %}
     {% endblock %}
 
     {% block prepare_kernel %}
     {% block static_kernel_dimensions %}
     static int num_threads, num_blocks;
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/group_variable_set.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/group_variable_set.cu`

 * *Files 6% similar despite different names*

```diff
@@ -40,17 +40,14 @@
     );
     {% endif %}
     {% endfor %}
 {% endblock %}
 
 {# _num_group_idx is defined in HOST_CONSTANTS, so we can't set _N before #}
 {% block define_N %}
-{% endblock %}
-
-{% block host_maincode %}
 const int _N = _num_group_idx;
 {% endblock %}
 
 {% block profiling_start %}
 {% endblock %}
 
 {% block profiling_stop %}
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/group_variable_set_conditional.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/group_variable_set_conditional.cu`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/main.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/main.cu`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/makefile` & `Brian2Cuda-1.0a2/brian2cuda/templates/makefile`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/network.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/network.cu`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/objects.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/objects.cu`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/rand.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/rand.cu`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/ratemonitor.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/ratemonitor.cu`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/reset.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/reset.cu`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/run.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/run.cu`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/spatialstateupdate.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/spatialstateupdate.cu`

 * *Files 4% similar despite different names*

```diff
@@ -16,40 +16,46 @@
 
 {### BEFORE RUN ###}
 {% block before_run_host_maincode %}
 
     ///// HOST_CONSTANTS ///////////
     %HOST_CONSTANTS%
 
+    // Number of group units in stateupdate is always N (no subgroups)
+    const int _N = N;
+
+    ///// ADDITIONAL_HOST_CODE /////
+    %ADDITIONAL_HOST_CODE%
+
     {# needed to translate _array... to _ptr_array... #}
     ///// pointers_lines /////
     {{pointers_lines|autoindent}}
 
     // The following code is simply copied from spatialneuron_prepare.cpp
     // of the cpp_standalone device (except for copying to GPU memory at bottom of file)
 
     const double _Ri = {{Ri}};  // Ri is a shared variable
 
     // Inverse axial resistance
     {# {{ openmp_pragma('parallel-static') }} #}
-    for (int _i=1; _i<N; _i++)
+    for (int _i=1; _i<_N; _i++)
         {{_invr}}[_i] = 1.0/(_Ri*(1/{{r_length_2}}[_i-1] + 1/{{r_length_1}}[_i]));
     // Cut sections
     {# {{ openmp_pragma('parallel-static') }} #}
     for (int _i=0; _i<_num_starts; _i++)
         {{_invr}}[{{_starts}}[_i]] = 0;
 
     // Linear systems
     // The particular solution
     // a[i,j]=ab[u+i-j,j]   --  u is the number of upper diagonals = 1
     {# {{ openmp_pragma('parallel-static') }} #}
-    for (int _i=0; _i<N; _i++)
+    for (int _i=0; _i<_N; _i++)
         {{_ab_star1}}[_i] = (-({{Cm}}[_i] / {{dt}}) - {{_invr}}[_i] / {{area}}[_i]);
     {# {{ openmp_pragma('parallel-static') }} #}
-    for (int _i=1; _i<N; _i++)
+    for (int _i=1; _i<_N; _i++)
     {
         {{_ab_star0}}[_i] = {{_invr}}[_i] / {{area}}[_i-1];
         {{_ab_star2}}[_i-1] = {{_invr}}[_i] / {{area}}[_i];
         {{_ab_star1}}[_i-1] -= {{_invr}}[_i] / {{area}}[_i-1];
     }
 
     // Set the boundary conditions
@@ -117,33 +123,30 @@
 //         runtime complexity O(compartments) but is inherently sequential
 //         => run no as many blocks as branches with one thread each
 //         => trivial optimization possible by using three threads (one per rhs)
 //         => optimization possible e.g. by using cyclic reduction [more parallel]
 
 __global__ void _tridiagsolve_kernel_{{codeobj_name}}(
     int _N,
-    int THREADS_PER_BLOCK,
     ///// KERNEL_PARAMETERS /////
     %KERNEL_PARAMETERS%
     )
 {
     using namespace brian;
 
     int tid = threadIdx.x;
     int bid = blockIdx.x;
-    int _idx = bid * THREADS_PER_BLOCK + tid;
+    int _idx = bid * blockDim.x + tid;
 
     ///// KERNEL_CONSTANTS /////
     %KERNEL_CONSTANTS%
 
     ///// kernel_lines /////
     {{kernel_lines|autoindent}}
 
-    assert(THREADS_PER_BLOCK == blockDim.x);
-
     // we need to run the kernel with 1 thread per block (to be changed by optimization)
     assert(tid == 0 && bid == _idx);
 
     // each thread processes the tridiagsystem of one branch
     const int _i = _idx;
 
     // below all the code is simply copied from spatialstateupdate.cpp
@@ -157,15 +160,15 @@
     // upper triangularization of tridiagonal system for _v_star, _u_plus, and _u_minus
     for(int _j=_j_start; _j<_j_end; _j++)
     {
         {{_v_star}}[_j]=-({{Cm}}[_j]/{{dt}}*{{v}}[_j])-{{_I0_all}}[_j]; // RHS -> _v_star (solution)
         {{_u_plus}}[_j]={{_b_plus}}[_j]; // RHS -> _u_plus (solution)
         {{_u_minus}}[_j]={{_b_minus}}[_j]; // RHS -> _u_minus (solution)
         _bi={{_ab_star1}}[_j]-{{_gtot_all}}[_j]; // main diagonal
-        if (_j<N-1)
+        if (_j<_N-1)
             {{_c}}[_j]={{_ab_star0}}[_j+1]; // superdiagonal
         if (_j>0)
         {
             _ai={{_ab_star2}}[_j-1]; // subdiagonal
             _m=1.0/(_bi-_ai*{{_c}}[_j-1]);
             {{_c}}[_j]={{_c}}[_j]*_m;
             {{_v_star}}[_j]=({{_v_star}}[_j] - _ai*{{_v_star}}[_j-1])*_m;
@@ -194,33 +197,30 @@
 // kernel 3: solve the coupling system (one matrix of size branches)
 // (no independence)
 // remark: applies the Hines algorithm having O(branches) complexity
 //         => run with one block one thread
 
 __global__ void _coupling_kernel_{{codeobj_name}}(
     int _N,
-    int THREADS_PER_BLOCK,
     ///// KERNEL_PARAMETERS /////
     %KERNEL_PARAMETERS%
     )
 {
     using namespace brian;
 
     int tid = threadIdx.x;
     int bid = blockIdx.x;
-    int _idx = bid * THREADS_PER_BLOCK + tid;
+    int _idx = bid * blockDim.x + tid;
 
     ///// KERNEL_CONSTANTS /////
     %KERNEL_CONSTANTS%
 
     ///// kernel_lines /////
     {{kernel_lines|autoindent}}
 
-    assert(THREADS_PER_BLOCK == blockDim.x);
-
     // we need to run the kernel with 1 thread, 1 block
     assert(_idx == 0);
 
     // below all the code is simply copied from spatialstateupdate.cpp
 
         // indexing for _P_children which contains the elements above the diagonal of the coupling matrix _P
     const int _children_rowlength = _num_morph_children/_num_morph_children_num;
@@ -311,33 +311,30 @@
 // kernel 4: for each section compute the final solution by linear
 //           combination of the general solution
 // (independent: everything, i.e., compartments and branches)
 // remark: branch granularity in implementation used since parents/children are combined for each branch
 
 __global__ void _combine_kernel_{{codeobj_name}}(
     int _N,
-    int THREADS_PER_BLOCK,
     ///// KERNEL_PARAMETERS /////
     %KERNEL_PARAMETERS%
     )
 {
     using namespace brian;
 
     int tid = threadIdx.x;
     int bid = blockIdx.x;
-    int _idx = bid * THREADS_PER_BLOCK + tid;
+    int _idx = bid * blockDim.x + tid;
 
     ///// KERNEL_CONSTANTS /////
     %KERNEL_CONSTANTS%
 
     ///// kernel_lines /////
     {{kernel_lines|autoindent}}
 
-    assert(THREADS_PER_BLOCK == blockDim.x);
-
     // we need to run the kernel with 1 thread per block (to be changed by optimization)
     assert(tid == 0 && bid == _idx);
 
     // each thread combines the tridiagsystem of one branch
     const int _i = _idx;
 
     // below all the code is simply copied from spatialstateupdate.cpp
@@ -357,33 +354,30 @@
 
 /////////////////////////////////////////////////////
 // kernel 5: update currents
 // (independent: everything, i.e., compartments and branches)
 
 __global__ void _currents_kernel_{{codeobj_name}}(
     int _N,
-    int THREADS_PER_BLOCK,
     ///// KERNEL_PARAMETERS /////
     %KERNEL_PARAMETERS%
     )
 {
     using namespace brian;
 
     int tid = threadIdx.x;
     int bid = blockIdx.x;
-    int _idx = bid * THREADS_PER_BLOCK + tid;
+    int _idx = bid * blockDim.x + tid;
 
     ///// KERNEL_CONSTANTS /////
     %KERNEL_CONSTANTS%
 
     ///// kernel_lines /////
     {{kernel_lines|autoindent}}
 
-    assert(THREADS_PER_BLOCK == blockDim.x);
-
     if(_idx >= _N)
     {
         return;
     }
 
     // each thread processes the tridiagsystem of one branch
     const int _i = _idx;
@@ -419,15 +413,14 @@
     std::clock_t _start_time_tridiagsolve = std::clock();
     {% endif %}
 #}
     int num_blocks_tridiagsolve = _num_B-1;
     int num_threads_tridiagsolve = 1;
     _tridiagsolve_kernel_{{codeobj_name}}<<<num_blocks_tridiagsolve, num_threads_tridiagsolve>>>(
             _N,
-            num_threads_tridiagsolve,
             ///// HOST_PARAMETERS /////
             %HOST_PARAMETERS%
         );
     CUDA_CHECK_ERROR("_tridiagsolve_kernel_{{codeobj_name}}");
 {#
     {% if profiled %}
     CUDA_SAFE_CALL(cudaDeviceSynchronize());
@@ -441,15 +434,14 @@
     std::clock_t _start_time_coupling = std::clock();
     {% endif %}
 #}
     int num_blocks_coupling = 1;
     int num_threads_coupling = 1;
     _coupling_kernel_{{codeobj_name}}<<<num_blocks_coupling, num_threads_coupling>>>(
             _N,
-            num_threads_coupling,
             ///// HOST_PARAMETERS /////
             %HOST_PARAMETERS%
         );
     CUDA_CHECK_ERROR("_coupling_kernel_{{codeobj_name}}");
 {#
     {% if profiled %}
     CUDA_SAFE_CALL(cudaDeviceSynchronize());
@@ -463,15 +455,14 @@
     std::clock_t _start_time_combine = std::clock();
     {% endif %}
 #}
     int num_blocks_combine = _num_B-1;
     int num_threads_combine = 1;
     _combine_kernel_{{codeobj_name}}<<<num_blocks_combine, num_threads_combine>>>(
             _N,
-            num_threads_combine,
             ///// HOST_PARAMETERS /////
             %HOST_PARAMETERS%
         );
     CUDA_CHECK_ERROR("_combine_kernel_{{codeobj_name}}");
 {#
     {% if profiled %}
     CUDA_SAFE_CALL(cudaDeviceSynchronize());
@@ -540,15 +531,14 @@
         {% if profiled %}
         std::clock_t _start_time_currents = std::clock();
         {% endif %}
 #}
         // run kernel 5
         _currents_kernel_{{codeobj_name}}<<<num_blocks_currents, num_threads_currents>>>(
                 _N,
-                num_threads_currents,
                 ///// HOST_PARAMETERS /////
                 %HOST_PARAMETERS%
             );
         CUDA_CHECK_ERROR("_currents_kernel_{{codeobj_name}}");
 
 {#
     {% if profiled %}
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/spikegenerator.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/spikegenerator.cu`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         %KERNEL_PARAMETERS%
         )
     {
         using namespace brian;
 
         int _idx = blockIdx.x * blockDim.x + threadIdx.x;
 
+        const int N = {{owner.N}};
+
         // We need kernel_lines for time variables
         ///// kernel_lines /////
         {{kernel_lines|autoindent}}
 
         if (_idx >= N) {
             return;
         }
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/spikemonitor.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/spikemonitor.cu`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {% block extra_device_helper %}
 {% if owner.source.__class__.__name__ == 'Subgroup' %}
 struct is_in_subgroup
 {
   __device__
   bool operator()(const int32_t &neuron)
   {
-    return (_source_start <= neuron && neuron < _source_stop);
+    return ({{_source_start}} <= neuron && neuron < {{_source_stop}});
   }
 };
 {% endif %}{# Subgroup #}
 {% endblock extra_device_helper %}
 
 
 {# We change _N depending on number of events and subgroups #}
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/statemonitor.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/statemonitor.cu`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/summed_variable.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/summed_variable.cu`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/synapses.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/synapses.cu`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,17 @@
 {% block kernel %}
 
 __global__ void
 {% if launch_bounds or syn_launch_bounds %}
 __launch_bounds__(1024, {{sm_multiplier}})
 {% endif %}
 _run_kernel_{{codeobj_name}}(
-    {# TODO: we only need _N if we have random numbers per synapse, add a if test here #}
     int _N,
     int bid_offset,
     int timestep,
-    int THREADS_PER_BLOCK,
     {% if bundle_mode %}
     int threads_per_bundle,
     {% endif %}
     int32_t* eventspace,
     {% if uses_atomics or synaptic_effects == "synapse" %}
     int num_spiking_neurons,
     {% else %}
@@ -32,22 +30,21 @@
     {% endif %}
     ///// KERNEL_PARAMETERS /////
     %KERNEL_PARAMETERS%
     )
 {
     using namespace brian;
 
-    assert(THREADS_PER_BLOCK == blockDim.x);
-
     int tid = threadIdx.x;
     int bid = blockIdx.x + bid_offset;
     //TODO: do we need _idx here? if no, get also rid of scoping after scalar code
     // scalar_code can depend on _idx (e.g. if the state update depends on a
     // subexpression that is the same for all synapses, ?)
-    int _idx = bid * THREADS_PER_BLOCK + tid;
+    int _threads_per_block = blockDim.x;
+    int _idx = bid * _threads_per_block + tid;
     int _vectorisation_idx = _idx;
 
     ///// KERNEL_CONSTANTS /////
     %KERNEL_CONSTANTS%
 
     ///// kernel_lines /////
     {{kernel_lines|autoindent}}
@@ -98,15 +95,15 @@
 
                     // apply effects if event neuron is in sources of current SynapticPathway
                     if(spikes_start <= spiking_neuron && spiking_neuron < spikes_stop)
                     {
                         int pre_post_block_id = (spiking_neuron - spikes_start) * num_parallel_blocks + post_block_idx;
                         int num_synapses = {{pathway.name}}_num_synapses_by_pre[pre_post_block_id];
                         int32_t* propagating_synapses = {{pathway.name}}_synapse_ids_by_pre[pre_post_block_id];
-                        for(int j = tid; j < num_synapses; j+=THREADS_PER_BLOCK)
+                        for(int j = tid; j < num_synapses; j+=_threads_per_block)
                         {
                             // _idx is the synapse id
                             int32_t _idx = propagating_synapses[j];
                             _vectorisation_idx = j;
 
                             ///// vector_code /////
                             {{vector_code|autoindent}}
@@ -123,15 +120,15 @@
             {{pathway.name}}.queue->peek(&synapses_queue);
 
             int queue_size = synapses_queue[bid].size();
 
             {% if bundle_mode %}
             // use a fixed number of threads per bundle, i runs through all those threads of all bundles
             // for threads_per_bundle == 1, we have one thread per bundle (parallel)
-            for (int i = tid; i < queue_size*threads_per_bundle; i+=THREADS_PER_BLOCK)
+            for (int i = tid; i < queue_size*threads_per_bundle; i+=_threads_per_block)
             {
                 // bundle_idx runs through all bundles
                 int bundle_idx = i / threads_per_bundle;
                 // syn_in_bundle_idx runs through all threads in a single bundle
                 int syn_in_bundle_idx = i % threads_per_bundle;
 
                 int bundle_id = synapses_queue[bid].at(bundle_idx);
@@ -145,15 +142,15 @@
                 for (int j = syn_in_bundle_idx; j < bundle_size; j+=threads_per_bundle)
                 {
                     int32_t _idx = synapse_bundle[j];
 
             {% else %}{# no bundle_mode #}
 
                     // use one thread per synapse
-                    for(int j = tid; j < queue_size; j+=THREADS_PER_BLOCK)
+                    for(int j = tid; j < queue_size; j+=_threads_per_block)
                     {
                         int32_t _idx = synapses_queue[bid].at(j);
                         {
 
             {% endif %}{# bundle_mode #}
 
                             ///// vector_code /////
@@ -299,15 +296,14 @@
     {% endif %}
         for(int bid_offset = 0; bid_offset < num_loops; bid_offset++)
         {
             _run_kernel_{{codeobj_name}}<<<num_blocks, num_threads>>>(
                 _N,
                 bid_offset,
                 {{owner.clock.name}}.timestep[0],
-                num_threads,
                 {% if bundle_mode %}
                 num_threads_per_bundle,
                 {% endif %}
                 dev{{_eventspace}}[{{pathway.name}}_eventspace_idx],
                 {% if uses_atomics or synaptic_effects == "synapse" %}
                 num_spiking_neurons,
                 {% else %}
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/synapses_classes.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/synapses_classes.cu`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/synapses_create_array.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/synapses_create_array.cu`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/synapses_create_generator.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/synapses_create_generator.cu`

 * *Files 19% similar despite different names*

```diff
@@ -139,17 +139,14 @@
 
 {% block update_occupancy %}
 {% endblock %}
 
 {% block kernel_info %}
 {% endblock %}
 
-{% block define_N %}
-{% endblock %}
-
 {% block profiling_start %}
 std::clock_t start_timer = std::clock();
 
 CUDA_CHECK_MEMORY();
 size_t used_device_memory_start = used_device_memory;
 {% endblock %}
 
@@ -167,36 +164,41 @@
 {% block host_maincode %}
 
     ///// pointers_lines /////
     {{pointers_lines|autoindent}}
 
     {# Get N_post and N_pre in the correct way, regardless of whether they are
     constants or scalar arrays#}
-    const int _N_pre = {{constant_or_scalar('N_pre', variables['N_pre'])}};
-    const int _N_post = {{constant_or_scalar('N_post', variables['N_post'])}};
+    const size_t _N_pre = {{constant_or_scalar('N_pre', variables['N_pre'])}};
+    const size_t _N_post = {{constant_or_scalar('N_post', variables['N_post'])}};
     {{_dynamic_N_incoming}}.resize(_N_post + _target_offset);
     {{_dynamic_N_outgoing}}.resize(_N_pre + _source_offset);
 
-    int _raw_pre_idx, _raw_post_idx;
-    const int _vectorisation_idx = -1;
+    size_t _raw_pre_idx, _raw_post_idx;
+    {# For a connect call j='k+i for k in range(0, N_post, 2) if k+i < N_post'
+    "j" is called the "result index" (and "_post_idx" the "result index array", etc.)
+    "i" is called the "outer index" (and "_pre_idx" the "outer index array", etc.)
+    "k" is called the inner variable #}
+
+    const size_t _vectorisation_idx = -1;
     ///// scalar_code['setup_iterator'] /////
     {{scalar_code['setup_iterator']|autoindent}}
-    ///// scalar_code['create_j'] /////
-    {{scalar_code['create_j']|autoindent}}
+    ///// scalar_code['generator_expr'] /////
+    {{scalar_code['generator_expr']|autoindent}}
     ///// scalar_code['create_cond'] /////
     {{scalar_code['create_cond']|autoindent}}
-    ///// scalar_code['update_post'] /////
-    {{scalar_code['update_post']|autoindent}}
+    ///// scalar_code['update'] /////
+    {{scalar_code['update']|autoindent}}
 
-    for(int _i = 0; _i < _N_pre; _i++)
+    for(size_t _{{outer_index}}=0; _{{outer_index}}<_{{outer_index_size}}; _{{outer_index}}++)
     {
 
         bool __cond, _cond;
-        _raw_pre_idx = _i + _source_offset;
-        {% if not postsynaptic_condition %}
+        _raw{{outer_index_array}} = _{{outer_index}} + {{outer_index_offset}};
+        {% if not result_index_condition %}
         {
             ///// vector_code['create_cond'] /////
             {{vector_code['create_cond']|autoindent}}
             __cond = _cond;
         }
         _cond = __cond;
         if(!_cond) continue;
@@ -215,71 +217,147 @@
         // _j to __j in the inner scope (using the inner scope version of _j), and then
         // __j to _j in the outer scope (to the outer scope version of _j). This outer scope
         // version of _j will then be used in subsequent blocks.
         long _uiter_low;
         long _uiter_high;
         long _uiter_step;
         {% if iterator_func=='sample' %}
+        long _uiter_size;
         double _uiter_p;
         {% endif %}
         {
             ///// vector_code['setup_iterator'] /////
             {{vector_code['setup_iterator']|autoindent}}
             _uiter_low = _iter_low;
             _uiter_high = _iter_high;
             _uiter_step = _iter_step;
             {% if iterator_func=='sample' %}
+            {% if iterator_kwds['sample_size'] == 'fixed' %}
+            _uiter_size = _iter_size;
+            {% else %}
             _uiter_p = _iter_p;
             {% endif %}
+            {% endif %}
         }
         {% if iterator_func=='range' %}
-        for(int {{iteration_variable}}=_uiter_low; {{iteration_variable}}<_uiter_high; {{iteration_variable}}+=_uiter_step)
+        for(long {{inner_variable}}=_uiter_low; {{inner_variable}}<_uiter_high; {{inner_variable}}+=_uiter_step)
         {
         {% elif iterator_func=='sample' %}
+        const int _iter_sign = _uiter_step > 0 ? 1 : -1;
+        {% if iterator_kwds['sample_size'] == 'fixed' %}
+        std::set<int> _selected_set = std::set<int>();
+        std::set<int>::iterator _selected_it;
+        int _n_selected = 0;
+        int _n_dealt_with = 0;
+        int _n_total;
+        if (_uiter_step > 0)
+            _n_total = (_uiter_high - _uiter_low - 1) / _uiter_step + 1;
+        else
+            _n_total = (_uiter_low - _uiter_high - 1) / -_uiter_step + 1;
+        // Value determined by benchmarking, see github PR #1280
+        const bool _selection_algo = 1.0*_uiter_size / _n_total > 0.06;
+        if (_uiter_size > _n_total)
+        {
+            {% if skip_if_invalid %}
+            _uiter_size = _n_total;
+            {% else %}
+            cout << "Error: Requested sample size " << _uiter_size << " is bigger than the " <<
+                    "population size " << _n_total << "." << endl;
+            exit(1);
+            {% endif %}
+        } else if (_uiter_size < 0)
+        {
+            {% if skip_if_invalid %}
+            continue;
+            {% else %}
+            cout << "Error: Requested sample size " << _uiter_size << " is negative." << endl;
+            exit(1);
+            {% endif %}
+        } else if (_uiter_size == 0)
+            continue;
+        long {{inner_variable}};
+
+        if (_selection_algo)
+        {
+            {{inner_variable}} = _uiter_low - _uiter_step;
+        } else
+        {
+            // For the tracking algorithm, we have to first create all values
+            // to make sure they will be iterated in sorted order
+            _selected_set.clear();
+            while (_n_selected < _uiter_size)
+            {
+                int _r = (int)(_rand(_vectorisation_idx) * _n_total);
+                while (! _selected_set.insert(_r).second)
+                    _r = (int)(_rand(_vectorisation_idx) * _n_total);
+                _n_selected++;
+            }
+            _n_selected = 0;
+            _selected_it = _selected_set.begin();
+        }
+        while (_n_selected < _uiter_size)
+        {
+            if (_selection_algo)
+            {
+                // Selection sampling technique
+                // See section 3.4.2 of Donald E. Knuth, AOCP, Vol 2, Seminumerical Algorithms
+                {{inner_variable}} += _uiter_step;
+                _n_dealt_with++;
+                const double _U = _rand(_vectorisation_idx);
+                if ((_n_total - _n_dealt_with) * _U >= _uiter_size - _n_selected)
+                    continue;
+            } else
+            {
+                {{inner_variable}} = _uiter_low + (*_selected_it)*_uiter_step;
+                _selected_it++;
+            }
+            _n_selected++;
+        {% else %}
         if(_uiter_p==0) continue;
         const bool _jump_algo = _uiter_p<0.25;
         double _log1p;
         if(_jump_algo)
             _log1p = log(1-_uiter_p);
         else
             _log1p = 1.0; // will be ignored
         const double _pconst = 1.0/log(1-_uiter_p);
-        for(int {{iteration_variable}}=_uiter_low; {{iteration_variable}}<_uiter_high; {{iteration_variable}}++)
+        for(long {{inner_variable}}=_uiter_low; _iter_sign*{{inner_variable}}<_iter_sign*_uiter_high; {{inner_variable}} += _uiter_step)
         {
             if(_jump_algo) {
                 const double _r = _rand(_vectorisation_idx);
                 if(_r==0.0) break;
                 const int _jump = floor(log(_r)*_pconst)*_uiter_step;
-                {{iteration_variable}} += _jump;
-                if({{iteration_variable}}>=_uiter_high) continue;
+                {{inner_variable}} += _jump;
+                if (_iter_sign*{{inner_variable}} >= _iter_sign * _uiter_high) continue;
             } else {
-                if(_rand(_vectorisation_idx)>=_uiter_p) continue;
+                if (_rand(_vectorisation_idx)>=_uiter_p) continue;
             }
         {% endif %}
-            long __j, _j, _pre_idx, __pre_idx;
+        {% endif %}
+            long __{{result_index}}, _{{result_index}}, {{outer_index_array}}, _{{outer_index_array}};
             {
-            ///// vector_code['create_j'] /////
-                {{vector_code['create_j']|autoindent}}
-                __j = _j; // pick up the locally scoped _j and store in __j
-                __pre_idx = _pre_idx;
-            }
-            _j = __j; // make the previously locally scoped _j available
-            _pre_idx = __pre_idx;
-            _raw_post_idx = _j + _target_offset;
-            {% if postsynaptic_condition %}
+                ///// vector_code['generator_expr'] /////
+                {{vector_code['generator_expr']|autoindent}}
+                __{{result_index}} = _{{result_index}}; // pick up the locally scoped var and store in outer var
+                _{{outer_index_array}} = {{outer_index_array}};
+            }
+            _{{result_index}} = __{{result_index}}; // make the previously locally scoped var available
+            {{outer_index_array}} = _{{outer_index_array}};
+            _raw{{result_index_array}} = _{{result_index}} + {{result_index_offset}};
+            {% if result_index_condition %}
             {
-                {% if postsynaptic_variable_used %}
+                {% if result_index_used %}
                 {# The condition could index outside of array range #}
-                if(_j<0 || _j>=_N_post)
+                if(_{{result_index}}<0 || _{{result_index}}>=_{{result_index_size}})
                 {
                     {% if skip_if_invalid %}
                     continue;
                     {% else %}
-                    cout << "Error: tried to create synapse to neuron j=" << _j << " outside range 0 to " <<
-                            _N_post-1 << endl;
+                    cout << "Error: tried to create synapse to neuron {{result_index}}=" << _{{result_index}} << " outside range 0 to " <<
+                                            _{{result_index_size}}-1 << endl;
                     exit(1);
                     {% endif %}
                 }
                 {% endif %}
                 ///// vector_code['create_cond'] /////
                 {{vector_code['create_cond']|autoindent}}
                 __cond = _cond;
@@ -287,32 +365,32 @@
             _cond = __cond;
             {% endif %}
 
             {% if if_expression!='True' %}
             if(!_cond) continue;
             {% endif %}
 
-            {% if not postsynaptic_variable_used %}
+            {% if not result_index_used %}
             {# Otherwise, we already checked before #}
-            if(_j<0 || _j>=_N_post)
+            if(_{{result_index}}<0 || _{{result_index}}>=_{{result_index_size}})
             {
                 {% if skip_if_invalid %}
                 continue;
                 {% else %}
-                cout << "Error: tried to create synapse to neuron j=" << _j << " outside range 0 to " <<
-                        _N_post-1 << endl;
+                cout << "Error: tried to create synapse to neuron {{result_index}}=" << _{{result_index}} <<
+                        " outside range 0 to " << _{{result_index_size}}-1 << endl;
                 exit(1);
                 {% endif %}
             }
             {% endif %}
 
-            ///// vector_code['update_post'] /////
-            {{vector_code['update_post']|autoindent}}
+            ///// vector_code['update'] /////
+            {{vector_code['update']|autoindent}}
 
-            for (int _repetition=0; _repetition<_n; _repetition++) {
+            for (size_t _repetition=0; _repetition<_n; _repetition++) {
                 {{_dynamic_N_outgoing}}[_pre_idx] += 1;
                 {{_dynamic_N_incoming}}[_post_idx] += 1;
                 {{_dynamic__synaptic_pre}}.push_back(_pre_idx);
                 {{_dynamic__synaptic_post}}.push_back(_post_idx);
             }
         }
     }
@@ -340,16 +418,15 @@
                     dev{{varname}}.resize(newsize)
                     );
             {% endif %}
             {# //TODO: do we actually need to resize varname? #}
             {{varname}}.resize(newsize);
         {% endif %}
     {% endfor %}
-
-    // update the total number of synapses
+    // Also update the total number of synapses
     {{N}} = newsize;
 
     // Check for occurrence of multiple source-target pairs in synapses ("synapse number")
     std::map<std::pair<int32_t, int32_t>, int32_t> source_target_count;
     for (int _i=0; _i<newsize; _i++)
     {
         // Note that source_target_count will create a new entry initialized
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/templates/synapses_push_spikes.cu` & `Brian2Cuda-1.0a2/brian2cuda/templates/synapses_push_spikes.cu`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,18 @@
         );
     }
     {{owner.name}}.no_or_const_delay_mode = scalar_delay;
 }
 {% endblock before_run_defines %}
 
 
+{% block define_N %}
+{% endblock %}
+
+
 {% block before_run_host_maincode %}
     std::clock_t start_timer = std::clock();
     const double to_MB = 1.0 / (1024.0 * 1024.0);
     static bool first_run = true;
 
     CUDA_CHECK_MEMORY();
     size_t used_device_memory_start = used_device_memory;
@@ -1045,31 +1049,14 @@
             _num_threads,
             spiking_neuron - {{owner.name}}.spikes_start);
     }
 }
 {% endblock kernel %}
 
 
-{% block define_N %}
-{% endblock %}
-
-
-void _run_{{codeobj_name}}()
-{
-    using namespace brian;
-
-    {% if profiled %}
-    const std::clock_t _start_time = std::clock();
-    {% endif %}
-
-    ///// HOST_CONSTANTS /////
-    %HOST_CONSTANTS%
-
-
-
 {% block host_maincode %}
     if ({{owner.name}}_scalar_delay)
     {
         int num_eventspaces = dev{{_eventspace}}.size();
         {{owner.name}}_eventspace_idx = (current_idx{{_eventspace}} - {{owner.name}}_delay + num_eventspaces) % num_eventspaces;
 
         //////////////////////////////////////////////
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/__init__.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/conftest.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/features/cuda_configuration.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/features/cuda_configuration.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/features/speed.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/features/speed.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_cpp_cuda_consistency.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_cpp_cuda_consistency.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_cuda_generator.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_cuda_generator.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_cuda_standalone.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_cuda_standalone.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,14 +383,26 @@
     # Spike has not been delivered yet
     run(2*ms)
 
     device.build(directory=None)
     assert target.v[0] == 1  # Make sure the spike got delivered
 
 
+@pytest.mark.cuda_standalone
+@pytest.mark.standalone_only
+def test_constant_replacement():
+    # see github issue #1276
+    set_device('cuda_standalone', directory=None)
+    x = 42
+    G = NeuronGroup(1, 'y : 1')
+    G.y = 'x'
+    run(0*ms)
+    assert G.y[0] == 42.
+
+
 if __name__=='__main__':
     tests = [
         test_cuda_standalone,
         test_multiple_connects,
         test_storing_loading,
         test_duplicate_names_across_nets,
         test_cuda_scalar_writes,
@@ -398,11 +410,16 @@
         test_array_cache,
         test_run_with_debug,
         test_changing_profile_arg,
         test_delete_code_data,
         test_delete_directory,
         test_multiple_standalone_runs,
         test_continued_standalone_runs,
+        test_constant_replacement,
     ]
     for t in tests:
-        t()
+        try:
+            t()
+        except Exception:
+            print(f"\nProject directory: {get_device().project_dir}\n")
+            raise
         reinit_and_delete()
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_functions.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,43 +3,19 @@
 import pytest
 from numpy.testing import assert_equal
 
 from brian2 import *
 from brian2.core.functions import timestep
 from brian2.parsing.sympytools import str_to_sympy, sympy_to_str
 from brian2.utils.logger import catch_logs
-from brian2.tests.utils import assert_allclose
+from brian2.tests.utils import exc_isinstance, assert_allclose
 from brian2.codegen.generators import CodeGenerator
 from brian2.codegen.codeobject import CodeObject
 
 
-# TODO: Remove this and import from brian2.tests.utils once we track brian2 version
-# with merged PR brian2#1315
-def exc_isinstance(exc_info, expected_exception, raise_not_implemented=False):
-    # XXX: This will fails once the function is importable from brian2
-    try:
-        from brian2.tests.utils import exc_isinstance as _
-    except ImportError:
-        pass
-    else:
-        raise AssertionError("Remove this function and import from brian2")
-
-    if exc_info is None:
-        return False
-    if hasattr(exc_info, 'value'):
-        exc_info = exc_info.value
-
-    if isinstance(exc_info, expected_exception):
-        return True
-    elif raise_not_implemented and isinstance(exc_info, NotImplementedError):
-        raise exc_info
-
-    return exc_isinstance(exc_info.__cause__, expected_exception,
-                          raise_not_implemented=raise_not_implemented)
-
 @pytest.mark.cuda_standalone
 @pytest.mark.standalone_only
 def test_user_defined_function():
     set_device('cuda_standalone', directory=None)
 
     @implementation('cuda',"""
     __host__ __device__ inline double usersin(double x)
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_gpu_detection.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_gpu_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import logging
 from io import StringIO
 
 import pytest
 from numpy.testing import assert_equal
 
-from brian2 import prefs, ms, run, set_device
+from brian2 import prefs, ms, run, set_device, device
 from brian2.utils.logger import catch_logs
 from brian2.core.preferences import PreferenceError
 from brian2cuda.utils.gputools import (
     reset_cuda_installation,
     get_cuda_installation,
     restore_cuda_installation,
     reset_gpu_selection,
@@ -167,9 +167,9 @@
 @pytest.mark.cuda_standalone
 @pytest.mark.standalone_only
 def test_no_gpu_detection_preference(reset_gpu_detection, use_default_prefs):
     set_device("cuda_standalone", directory=None)
     # Test that disabling gpu detection works when setting gpu_id and compute_capability
     prefs.devices.cuda_standalone.cuda_backend.detect_gpus = False
     prefs.devices.cuda_standalone.cuda_backend.gpu_id = 0
-    prefs.devices.cuda_standalone.cuda_backend.compute_capability = 6.1
+    prefs.devices.cuda_standalone.cuda_backend.compute_capability = device.minimal_compute_capability
     run(0*ms)
```

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_monitor.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_network.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_network_multiple_runs.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_network_multiple_runs.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_neurongroup.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_neurongroup.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_profiling.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_random_number_generation.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_random_number_generation.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_spikegenerator.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_spikegenerator.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_stateupdaters.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_stateupdaters.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_stringtools.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_stringtools.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/tests/test_synaptic_propagations.py` & `Brian2Cuda-1.0a2/brian2cuda/tests/test_synaptic_propagations.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/timedarray.py` & `Brian2Cuda-1.0a2/brian2cuda/timedarray.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/utils/gputools.py` & `Brian2Cuda-1.0a2/brian2cuda/utils/gputools.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/utils/logger.py` & `Brian2Cuda-1.0a2/brian2cuda/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/brian2cuda/utils/stringtools.py` & `Brian2Cuda-1.0a2/brian2cuda/utils/stringtools.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/docs_sphinx/Makefile` & `Brian2Cuda-1.0a2/docs_sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/docs_sphinx/conf.py` & `Brian2Cuda-1.0a2/docs_sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/docs_sphinx/introduction/cuda_configuration.rst` & `Brian2Cuda-1.0a2/docs_sphinx/introduction/cuda_configuration.rst`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/docs_sphinx/introduction/index.rst` & `Brian2Cuda-1.0a2/docs_sphinx/introduction/index.rst`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/docs_sphinx/introduction/install.rst` & `Brian2Cuda-1.0a2/docs_sphinx/introduction/install.rst`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/docs_sphinx/introduction/known_issues.rst` & `Brian2Cuda-1.0a2/docs_sphinx/introduction/known_issues.rst`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/docs_sphinx/introduction/preferences.rst` & `Brian2Cuda-1.0a2/docs_sphinx/introduction/preferences.rst`

 * *Files identical despite different names*

### Comparing `Brian2CUDA-1.0a1/docs_sphinx/make.bat` & `Brian2Cuda-1.0a2/docs_sphinx/make.bat`

 * *Files identical despite different names*

