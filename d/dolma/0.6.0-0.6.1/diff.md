# Comparing `tmp/dolma-0.6.0.tar.gz` & `tmp/dolma-0.6.1.tar.gz`

## Comparing `dolma-0.6.0.tar` & `dolma-0.6.1.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 dolma-0.6.0/Cargo.toml
--rw-r--r--   0      502       20      475 2023-06-27 20:15:25.000000 dolma-0.6.0/.flake8
--rw-r--r--   0      502       20     2791 2023-07-03 03:39:51.000000 dolma-0.6.0/.github/workflows/CI.yml
--rw-r--r--   0      502       20      549 2023-06-22 18:02:39.000000 dolma-0.6.0/.gitignore
--rw-r--r--   0      502       20     1813 2023-07-06 05:35:16.000000 dolma-0.6.0/CITATION.cff
--rw-r--r--   0      502       20    11357 2023-06-20 21:37:30.000000 dolma-0.6.0/LICENSE
--rw-r--r--   0      502       20     2255 2023-07-09 03:50:09.000000 dolma-0.6.0/Makefile
--rw-r--r--   0      502       20     1345 2023-07-06 05:35:30.000000 dolma-0.6.0/README.md
--rw-r--r--   0      502       20     3217 2023-07-09 03:51:34.000000 dolma-0.6.0/pyproject.toml
--rw-r--r--   0      502       20      594 2023-07-06 05:13:47.000000 dolma-0.6.0/python/dolma/__init__.py
--rw-r--r--   0      502       20     4302 2023-07-04 20:11:47.000000 dolma-0.6.0/python/dolma/cli/__init__.py
--rw-r--r--   0      502       20     1494 2023-07-04 03:24:17.000000 dolma-0.6.0/python/dolma/cli/__main__.py
--rw-r--r--   0      502       20     4689 2023-07-04 20:11:46.000000 dolma-0.6.0/python/dolma/cli/deduper.py
--rw-r--r--   0      502       20     4589 2023-07-04 20:11:47.000000 dolma-0.6.0/python/dolma/cli/mixer.py
--rw-r--r--   0      502       20      473 2023-07-03 18:00:09.000000 dolma-0.6.0/python/dolma/cli/shared.py
--rw-r--r--   0      502       20     1343 2023-07-04 20:12:42.000000 dolma-0.6.0/python/dolma/cli/tagger.py
--rw-r--r--   0      502       20      219 2023-06-22 18:00:45.000000 dolma-0.6.0/python/dolma/core/__init__.py
--rw-r--r--   0      502       20     6111 2023-07-09 03:04:39.000000 dolma-0.6.0/python/dolma/core/data_types.py
--rw-r--r--   0      502       20      337 2023-07-04 18:53:34.000000 dolma-0.6.0/python/dolma/core/errors.py
--rw-r--r--   0      502       20     6482 2023-07-02 19:19:48.000000 dolma-0.6.0/python/dolma/core/ft_dataset.py
--rw-r--r--   0      502       20     5557 2023-07-06 01:39:42.000000 dolma-0.6.0/python/dolma/core/ft_tagger.py
--rw-r--r--   0      502       20    15342 2023-07-06 05:16:17.000000 dolma-0.6.0/python/dolma/core/parallel.py
--rw-r--r--   0      502       20     6326 2023-07-09 03:04:39.000000 dolma-0.6.0/python/dolma/core/paths.py
--rw-r--r--   0      502       20     1254 2023-06-22 18:00:45.000000 dolma-0.6.0/python/dolma/core/registry.py
--rw-r--r--   0      502       20     9931 2023-07-09 03:04:39.000000 dolma-0.6.0/python/dolma/core/runtime.py
--rw-r--r--   0      502       20     1032 2023-06-22 18:00:45.000000 dolma-0.6.0/python/dolma/core/taggers.py
--rw-r--r--   0      502       20       42 2023-06-22 18:00:45.000000 dolma-0.6.0/python/dolma/core/trainer.py
--rw-r--r--   0      502       20     2031 2023-07-04 20:11:47.000000 dolma-0.6.0/python/dolma/core/utils.py
--rw-r--r--   0      502       20     9484 2023-07-09 03:04:39.000000 dolma-0.6.0/python/dolma/core/vizualizer.py
--rw-r--r--   0      502       20     3777 2023-06-22 18:00:53.000000 dolma-0.6.0/python/dolma/data/naughty_words_en.txt
--rw-r--r--   0      502       20        0 2023-06-21 16:42:48.000000 dolma-0.6.0/python/dolma/py.typed
--rw-r--r--   0      502       20       72 2023-07-06 01:39:42.000000 dolma-0.6.0/python/dolma/taggers/__init__.py
--rw-r--r--   0      502       20     3277 2023-06-22 18:02:34.000000 dolma-0.6.0/python/dolma/taggers/c4.py
--rw-r--r--   0      502       20     6433 2023-07-09 03:04:39.000000 dolma-0.6.0/python/dolma/taggers/code.py
--rw-r--r--   0      502       20     6857 2023-07-09 03:04:39.000000 dolma-0.6.0/python/dolma/taggers/gopher.py
--rw-r--r--   0      502       20     1898 2023-06-22 18:02:47.000000 dolma-0.6.0/python/dolma/taggers/jigsaw.py
--rw-r--r--   0      502       20     6391 2023-06-23 22:30:50.000000 dolma-0.6.0/python/dolma/taggers/language.py
--rw-r--r--   0      502       20     4876 2023-06-22 18:02:44.000000 dolma-0.6.0/python/dolma/taggers/length.py
--rw-r--r--   0      502       20    10494 2023-07-02 19:19:48.000000 dolma-0.6.0/python/dolma/taggers/pii.py
--rw-r--r--   0      502       20      744 2023-06-22 18:02:42.000000 dolma-0.6.0/python/dolma/taggers/sampling.py
--rw-r--r--   0      502       20      232 2023-06-22 18:32:09.000000 dolma-0.6.0/res/logo.md
--rw-r--r--   0      502       20  1813803 2023-06-22 18:39:27.000000 dolma-0.6.0/res/logo.png
--rw-r--r--   0      502       20     9277 2023-06-21 23:41:09.000000 dolma-0.6.0/src/bloom_filter.rs
--rw-r--r--   0      502       20    14421 2023-07-03 23:10:59.000000 dolma-0.6.0/src/deduper.rs
--rw-r--r--   0      502       20     1124 2023-07-03 23:11:41.000000 dolma-0.6.0/src/lib.rs
--rw-r--r--   0      502       20     7176 2023-07-04 03:15:49.000000 dolma-0.6.0/src/mixer.rs
--rw-r--r--   0      502       20    11131 2023-07-04 03:17:09.000000 dolma-0.6.0/src/s3_util.rs
--rw-r--r--   0      502       20    23416 2023-07-04 04:08:09.000000 dolma-0.6.0/src/shard.rs
--rw-r--r--   0      502       20      863 2023-07-04 04:09:36.000000 dolma-0.6.0/tests/config/c4-cleaned.json
--rw-r--r--   0      502       20      564 2023-07-04 03:02:00.000000 dolma-0.6.0/tests/config/dedupe-by-url.json
--rw-r--r--   0      502       20      553 2023-07-04 03:02:00.000000 dolma-0.6.0/tests/config/dedupe-paragraphs.json
--rw-r--r--   0      502       20      815 2023-07-04 03:02:00.000000 dolma-0.6.0/tests/config/email-spans.json
--rw-r--r--   0      502       20      799 2023-07-04 04:09:14.000000 dolma-0.6.0/tests/config/filter-by-spans.json
--rw-r--r--   0      502       20      792 2023-07-04 03:02:00.000000 dolma-0.6.0/tests/config/mixer.json
--rw-r--r--   0      502       20      716 2023-07-04 03:02:00.000000 dolma-0.6.0/tests/config/paragraph-spans.json
--rw-r--r--   0      502       20    25985 2023-07-03 20:49:57.000000 dolma-0.6.0/tests/data/documents.json.gz
--rw-r--r--   0      502       20      702 2023-07-03 20:49:57.000000 dolma-0.6.0/tests/data/duplicate-paragraphs.json.gz
--rw-r--r--   0      502       20      489 2023-07-05 18:48:05.000000 dolma-0.6.0/tests/data/expected/dedupe-by-url.json.gz
--rw-r--r--   0      502       20      746 2023-07-05 18:48:05.000000 dolma-0.6.0/tests/data/expected/dedupe-paragraphs.json.gz
--rw-r--r--   0      502       20    26447 2023-07-05 18:48:05.000000 dolma-0.6.0/tests/data/expected/email-spans.json.gz
--rw-r--r--   0      502       20    14879 2023-07-05 18:48:05.000000 dolma-0.6.0/tests/data/expected/filter-by-spans.json.gz
--rw-r--r--   0      502       20    15748 2023-07-05 18:48:05.000000 dolma-0.6.0/tests/data/expected/mixer.json.gz
--rw-r--r--   0      502       20    26524 2023-07-05 18:48:05.000000 dolma-0.6.0/tests/data/expected/remove-paragraphs.json.gz
--rw-r--r--   0      502       20      614 2023-07-03 20:49:57.000000 dolma-0.6.0/tests/data/pii-attributes.json.gz
--rw-r--r--   0      502       20      570 2023-07-03 20:49:57.000000 dolma-0.6.0/tests/data/sample-attributes.json.gz
--rw-r--r--   0      502       20      543 2023-07-03 20:49:57.000000 dolma-0.6.0/tests/data/toxicity-attributes.json.gz
--rw-r--r--   0      502       20      352 2023-07-06 05:14:01.000000 dolma-0.6.0/tests/python/__init__.py
--rw-r--r--   0      502       20     3342 2023-07-09 03:04:40.000000 dolma-0.6.0/tests/python/test_data_types.py
--rw-r--r--   0      502       20      471 2023-07-04 03:31:40.000000 dolma-0.6.0/tests/python/test_deduper.py
--rw-r--r--   0      502       20      820 2023-07-04 04:09:57.000000 dolma-0.6.0/tests/python/test_mixer.py
--rw-r--r--   0      502       20     1395 2023-07-04 03:31:40.000000 dolma-0.6.0/tests/python/test_omegaconf.py
--rw-r--r--   0      502       20     8972 2023-07-09 03:04:40.000000 dolma-0.6.0/tests/python/test_paths.py
--rw-r--r--   0      502       20     2459 2023-07-06 05:18:34.000000 dolma-0.6.0/tests/python/test_runtime.py
--rw-r--r--   0      502       20     9701 2023-07-05 18:38:13.000000 dolma-0.6.0/tests/python/test_taggers.py
--rw-r--r--   0      502       20     4043 2023-07-09 03:04:40.000000 dolma-0.6.0/tests/python/test_utils.py
--rw-r--r--   0      502       20    57199 2023-07-03 19:18:47.000000 dolma-0.6.0/Cargo.lock
--rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 dolma-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 dolma-0.6.1/Cargo.toml
+-rw-r--r--   0      502       20      475 2023-06-27 20:15:25.000000 dolma-0.6.1/.flake8
+-rw-r--r--   0      502       20     2791 2023-07-09 05:40:50.000000 dolma-0.6.1/.github/workflows/CI.yml
+-rw-r--r--   0      502       20      549 2023-06-22 18:02:39.000000 dolma-0.6.1/.gitignore
+-rw-r--r--   0      502       20     1813 2023-07-09 05:40:50.000000 dolma-0.6.1/CITATION.cff
+-rw-r--r--   0      502       20    11357 2023-06-20 21:37:30.000000 dolma-0.6.1/LICENSE
+-rw-r--r--   0      502       20     2294 2023-07-09 05:51:44.000000 dolma-0.6.1/Makefile
+-rw-r--r--   0      502       20     3093 2023-07-09 05:51:23.000000 dolma-0.6.1/README.md
+-rw-r--r--   0      502       20     3217 2023-07-09 05:42:06.000000 dolma-0.6.1/pyproject.toml
+-rw-r--r--   0      502       20      736 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/__init__.py
+-rw-r--r--   0      502       20     4401 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/cli/__init__.py
+-rw-r--r--   0      502       20     1494 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/cli/__main__.py
+-rw-r--r--   0      502       20     4689 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/cli/deduper.py
+-rw-r--r--   0      502       20     4589 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/cli/mixer.py
+-rw-r--r--   0      502       20      473 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/cli/shared.py
+-rw-r--r--   0      502       20     1957 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/cli/tagger.py
+-rw-r--r--   0      502       20      219 2023-06-22 18:00:45.000000 dolma-0.6.1/python/dolma/core/__init__.py
+-rw-r--r--   0      502       20     6111 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/data_types.py
+-rw-r--r--   0      502       20      337 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/errors.py
+-rw-r--r--   0      502       20     6482 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/ft_dataset.py
+-rw-r--r--   0      502       20     5557 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/ft_tagger.py
+-rw-r--r--   0      502       20    15587 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/parallel.py
+-rw-r--r--   0      502       20     6326 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/paths.py
+-rw-r--r--   0      502       20     1254 2023-06-22 18:00:45.000000 dolma-0.6.1/python/dolma/core/registry.py
+-rw-r--r--   0      502       20    11812 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/runtime.py
+-rw-r--r--   0      502       20     1032 2023-06-22 18:00:45.000000 dolma-0.6.1/python/dolma/core/taggers.py
+-rw-r--r--   0      502       20       42 2023-06-22 18:00:45.000000 dolma-0.6.1/python/dolma/core/trainer.py
+-rw-r--r--   0      502       20     2031 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/utils.py
+-rw-r--r--   0      502       20     9484 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/core/vizualizer.py
+-rw-r--r--   0      502       20     3777 2023-06-22 18:00:53.000000 dolma-0.6.1/python/dolma/data/naughty_words_en.txt
+-rw-r--r--   0      502       20        0 2023-06-21 16:42:48.000000 dolma-0.6.1/python/dolma/py.typed
+-rw-r--r--   0      502       20       72 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/taggers/__init__.py
+-rw-r--r--   0      502       20     3277 2023-06-22 18:02:34.000000 dolma-0.6.1/python/dolma/taggers/c4.py
+-rw-r--r--   0      502       20     6433 2023-07-09 05:39:12.000000 dolma-0.6.1/python/dolma/taggers/code.py
+-rw-r--r--   0      502       20     6857 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/taggers/gopher.py
+-rw-r--r--   0      502       20     1898 2023-06-22 18:02:47.000000 dolma-0.6.1/python/dolma/taggers/jigsaw.py
+-rw-r--r--   0      502       20     6391 2023-06-23 22:30:50.000000 dolma-0.6.1/python/dolma/taggers/language.py
+-rw-r--r--   0      502       20     4876 2023-06-22 18:02:44.000000 dolma-0.6.1/python/dolma/taggers/length.py
+-rw-r--r--   0      502       20    10494 2023-07-09 05:40:50.000000 dolma-0.6.1/python/dolma/taggers/pii.py
+-rw-r--r--   0      502       20      744 2023-06-22 18:02:42.000000 dolma-0.6.1/python/dolma/taggers/sampling.py
+-rw-r--r--   0      502       20      232 2023-06-22 18:32:09.000000 dolma-0.6.1/res/logo.md
+-rw-r--r--   0      502       20  1813803 2023-06-22 18:39:27.000000 dolma-0.6.1/res/logo.png
+-rw-r--r--   0      502       20     9277 2023-06-21 23:41:09.000000 dolma-0.6.1/src/bloom_filter.rs
+-rw-r--r--   0      502       20    14421 2023-07-09 05:40:50.000000 dolma-0.6.1/src/deduper.rs
+-rw-r--r--   0      502       20     1124 2023-07-09 05:40:50.000000 dolma-0.6.1/src/lib.rs
+-rw-r--r--   0      502       20     7176 2023-07-09 05:40:50.000000 dolma-0.6.1/src/mixer.rs
+-rw-r--r--   0      502       20    11131 2023-07-09 05:40:50.000000 dolma-0.6.1/src/s3_util.rs
+-rw-r--r--   0      502       20    23416 2023-07-09 05:40:50.000000 dolma-0.6.1/src/shard.rs
+-rw-r--r--   0      502       20      863 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/c4-cleaned.json
+-rw-r--r--   0      502       20      564 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/dedupe-by-url.json
+-rw-r--r--   0      502       20      553 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/dedupe-paragraphs.json
+-rw-r--r--   0      502       20      815 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/email-spans.json
+-rw-r--r--   0      502       20      799 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/filter-by-spans.json
+-rw-r--r--   0      502       20      792 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/mixer.json
+-rw-r--r--   0      502       20      716 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/config/paragraph-spans.json
+-rw-r--r--   0      502       20    25985 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/documents.json.gz
+-rw-r--r--   0      502       20      702 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/duplicate-paragraphs.json.gz
+-rw-r--r--   0      502       20      489 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/expected/dedupe-by-url.json.gz
+-rw-r--r--   0      502       20      746 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/expected/dedupe-paragraphs.json.gz
+-rw-r--r--   0      502       20    26447 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/expected/email-spans.json.gz
+-rw-r--r--   0      502       20    14879 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/expected/filter-by-spans.json.gz
+-rw-r--r--   0      502       20    15748 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/expected/mixer.json.gz
+-rw-r--r--   0      502       20    26524 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/expected/remove-paragraphs.json.gz
+-rw-r--r--   0      502       20      614 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/pii-attributes.json.gz
+-rw-r--r--   0      502       20      570 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/sample-attributes.json.gz
+-rw-r--r--   0      502       20      543 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/data/toxicity-attributes.json.gz
+-rw-r--r--   0      502       20      352 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/__init__.py
+-rw-r--r--   0      502       20     3342 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_data_types.py
+-rw-r--r--   0      502       20      471 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_deduper.py
+-rw-r--r--   0      502       20      820 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_mixer.py
+-rw-r--r--   0      502       20     1395 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_omegaconf.py
+-rw-r--r--   0      502       20     2459 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_parallel.py
+-rw-r--r--   0      502       20     8972 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_paths.py
+-rw-r--r--   0      502       20     1846 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_runtime.py
+-rw-r--r--   0      502       20     9701 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_taggers.py
+-rw-r--r--   0      502       20     4043 2023-07-09 05:40:50.000000 dolma-0.6.1/tests/python/test_utils.py
+-rw-r--r--   0      502       20    57199 2023-07-09 05:40:50.000000 dolma-0.6.1/Cargo.lock
+-rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 dolma-0.6.1/PKG-INFO
```

### Comparing `dolma-0.6.0/Cargo.toml` & `dolma-0.6.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/.github/workflows/CI.yml` & `dolma-0.6.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/.gitignore` & `dolma-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/CITATION.cff` & `dolma-0.6.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/LICENSE` & `dolma-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/Makefile` & `dolma-0.6.1/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 setup:
 	@echo "${OS_MESSAGE}: installing..."
 	$(shell "${CMAKE_SETUP}")
 	$(shell "${PROTOBUF_SETUP}")
 	$(shell "${OPENSSL_SETUP}")
 	which cargo || curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
+	which maturin || pip install maturin
 
-
-release:
-	maturin build
+publish:
+	maturin publish
 
 test: setup develop setup-test test-python test-rust clean-test
 
 test-python:
 	pytest -vs tests/python
 
 test-rust:
```

### Comparing `dolma-0.6.0/pyproject.toml` & `dolma-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dolma"
-version = "0.6.0"
+version = "0.6.1"
 description = "Data filters"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "requests",
     "tqdm",
```

### Comparing `dolma-0.6.0/python/dolma/__init__.py` & `dolma-0.6.1/python/dolma/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 import warnings
 
 # warning raised by pkg_resources used in a lot of google packages
 warnings.filterwarnings("ignore", message=r".*declare_namespace\(\'.*google.*", category=DeprecationWarning)
 # base warning raised when warning above are raised
 warnings.filterwarnings("ignore", message=r".*pkg_resources is deprecated.*", category=DeprecationWarning)
 
+# must import taggers to register them
+# we import the rust extension here and wrap it in a python module
 from . import dolma as _dolma  # type: ignore   # noqa: E402
+from . import taggers  # noqa: E402
 
 
 def deduper(config: dict):
     return _dolma.deduper_entrypoint(json.dumps(config))
 
 
 def mixer(config: dict):
```

### Comparing `dolma-0.6.0/python/dolma/cli/__init__.py` & `dolma-0.6.1/python/dolma/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,20 @@
 
         if is_dataclass(typ_):
             # recursively add subparsers
             make_parser(parser, typ_, prefix=field_name)
             continue
 
         field_name = f"{prefix}.{field_name}" if prefix else field_name
-        parser.add_argument(f"--{field_name}", help=field.metadata.get("help"), default=MISSING)
+        parser.add_argument(
+            f"--{field_name}",
+            help=field.metadata.get("help"),
+            nargs=field.metadata.get("nargs", "?"),
+            default=MISSING,
+        )
 
     return parser
 
 
 def _make_nested_dict(key: str, value: Any, d: Optional[Dict[str, Any]] = None) -> Dict[str, Any]:
     d = d or {}
```

### Comparing `dolma-0.6.0/python/dolma/cli/__main__.py` & `dolma-0.6.1/python/dolma/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/cli/deduper.py` & `dolma-0.6.1/python/dolma/cli/deduper.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/cli/mixer.py` & `dolma-0.6.1/python/dolma/cli/mixer.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/cli/tagger.py` & `dolma-0.6.1/python/dolma/cli/tagger.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from argparse import ArgumentParser, Namespace
 from dataclasses import dataclass
-from typing import List, Optional, Union
+from typing import List, Optional
 
-from omegaconf import DictConfig
-from omegaconf import OmegaConf as om
+from omegaconf import MISSING
 
-from dolma.cli import BaseCli, field
+from dolma.cli import BaseCli, field, print_config
 from dolma.cli.shared import WorkDirConfig
-from dolma.core.runtime import TaggerProcessor
+from dolma.core.runtime import create_and_run_tagger
 
 
 @dataclass
 class TaggerConfig:
     documents: List[str] = field(
         default=[],
         help="One or more document paths to process; Can be either local or S3 paths. Globs are supported.",
@@ -23,22 +21,43 @@
             "If not provided, destination will be derived from the document path."
         ),
     )
     taggers: List[str] = field(
         default=[],
         help="List of taggers to run.",
     )
+    experiment: str = field(
+        default=MISSING,
+        help="Name of the experiment.",
+    )
     processes: int = field(
         default=1,
         help="Number of parallel processes to use.",
     )
+    debug: bool = field(
+        default=False,
+        help="Whether to run in debug mode.",
+    )
     work_dir: Optional[WorkDirConfig] = field(
         default=WorkDirConfig(), help="Configuration for temporary work directories."
     )
 
 
 class TaggerCli(BaseCli):
     CONFIG = TaggerConfig
 
     @classmethod
     def run(cls, parsed_config: TaggerConfig):
-        raise NotImplementedError("TaggerCli.run() is not implemented yet.")
+        metadata = parsed_config.work_dir.output if parsed_config.work_dir else None
+        documents = [str(p) for p in parsed_config.documents]
+        taggers = [str(p) for p in parsed_config.taggers]
+
+        print_config(parsed_config)
+        create_and_run_tagger(
+            documents=documents,
+            destination=parsed_config.destination,
+            metadata=metadata,
+            taggers=taggers,
+            num_processes=parsed_config.processes,
+            experiment=parsed_config.experiment,
+            debug=parsed_config.debug,
+        )
```

### Comparing `dolma-0.6.0/python/dolma/core/data_types.py` & `dolma-0.6.1/python/dolma/core/data_types.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/core/ft_dataset.py` & `dolma-0.6.1/python/dolma/core/ft_dataset.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/core/ft_tagger.py` & `dolma-0.6.1/python/dolma/core/ft_tagger.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/core/parallel.py` & `dolma-0.6.1/python/dolma/core/parallel.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,19 +36,20 @@
         self,
         source_prefix: Union[str, List[str]],
         destination_prefix: Union[str, List[str]],
         metadata_prefix: Union[str, List[str]],
         num_processes: int = 1,
         debug: bool = False,
         seed: int = 0,
-        pbar_timeout: float = 0.01,
+        pbar_timeout: float = 1e-3,
         ignore_existing: bool = False,
         include_paths: Optional[List[str]] = None,
         exclude_paths: Optional[List[str]] = None,
         files_regex_pattern: Optional[str] = None,
+        retries_on_error: int = 0,
     ):
         """Initialize the parallel processor.
 
         Args:
             source_prefix (str): The location where source files are stored. This can be a local directory or a
                 prefix to an S3 location.
             destination_prefix (str): The location where to save the transformed files. This can be a local
@@ -81,14 +82,15 @@
         self.seed = seed
         self.pbar_timeout = pbar_timeout
         self.ignore_existing = ignore_existing
 
         self.include_paths = set(include_paths) if include_paths is not None else None
         self.exclude_paths = set(exclude_paths) if exclude_paths is not None else None
         self.files_regex_pattern = re.compile(files_regex_pattern) if files_regex_pattern else None
+        self.retries_on_error = retries_on_error
 
         # checking that the increment_progressbar method is subclassed correctly
         sig = inspect.signature(self.increment_progressbar)
         if "queue" not in sig.parameters or sig.parameters["queue"].kind != inspect.Parameter.POSITIONAL_ONLY:
             raise AttributeError(
                 "increment_progressbar must have a positional-only argument named 'queue'; "
                 "Check that you have subclassed BaseParallelProcessor correctly!"
@@ -146,24 +148,24 @@
         metadata_path: str,
         queue: "Queue[Union[None, Tuple[int, ...]]]",
         serialized_kwargs: bytes,
     ):
         """A wrapper around process single that saves a metadata file if processing is successful."""
 
         kwargs = pickle.loads(serialized_kwargs)
-        tries_remaining = kwargs.get("retry_on_read_error", 0) + 1
+        retries_on_error = kwargs.get("retries_on_error", 0) + 1
         while True:
             try:
                 cls.process_single(
                     source_path=source_path, destination_path=destination_path, queue=queue, **kwargs
                 )
                 break
             except DolmaRetryableFailure as e:
-                tries_remaining -= 1
-                if tries_remaining == 0:
+                retries_on_error -= 1
+                if retries_on_error == 0:
                     raise DolmaFilterError from e
 
         with smart_open.open(metadata_path, "wt") as f:
             f.write(datetime.now().isoformat())
 
     @classmethod
     def increment_progressbar(
@@ -337,14 +339,17 @@
 
         return all_source_paths, all_destination_paths, all_metadata_paths
 
     def __call__(self, **process_single_kwargs: Any):
         """Run the processor."""
         random.seed(self.seed)
 
+        # in case the user wants to override the default kwargs for retries
+        process_single_kwargs.setdefault("retries_on_error", self.retries_on_error)
+
         all_source_paths, all_destination_paths, all_metadata_paths = self._get_all_paths()
 
         print(f"Found {len(all_source_paths):,} files to process")
 
         fn = self._debug_run_all if self.debug else self._multiprocessing_run_all
 
         fn(
```

### Comparing `dolma-0.6.0/python/dolma/core/paths.py` & `dolma-0.6.1/python/dolma/core/paths.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/core/registry.py` & `dolma-0.6.1/python/dolma/core/registry.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/core/runtime.py` & `dolma-0.6.1/python/dolma/core/runtime.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,91 @@
-import argparse
-import gzip
 import logging
 import multiprocessing
-import os
 import tempfile
 from contextlib import ExitStack
 from queue import Queue
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Union
 
 import msgspec
 import smart_open
-from numpy import source
 
 from .data_types import InputSpec, OutputSpec
 from .errors import DolmaFatalError, DolmaRetryableFailure, DolmaShardError
 from .parallel import BaseParallelProcessor
-from .paths import join_path, make_relative, split_path
+from .paths import join_path, make_relative, split_glob, split_path
 from .registry import TaggerRegistry
 from .utils import make_variable_name
 
 
+def _make_paths_from_substitution(paths: List[str], find: str, replace: str) -> List[str]:
+    """
+    Utility function to make paths using a find/replace substitution. This is useful if you want to
+    create a destination path from a source path by replacing part of the source path with something else.
+
+    For example, if you have a source path of `current_paths = ["s3://bucket/data/documents/**.json.gz"]` and
+    you want to replace `documents` with `attributes`, you can use this function to do that. by calling
+    `_make_paths_from_substitution(current_paths, "documents", "attribute")`. This will return the following
+    list `["s3://bucket/data/attributes"]`. Note how glob patterns are removed from the paths.
+    """
+    new_paths: List[str] = []
+    for curr in paths:
+        curr_pre_glob, _ = split_glob(curr)
+        curr_prot, curr_parts = split_path(curr_pre_glob)
+        find_dir_index = curr_parts.index(find)
+
+        if not curr_pre_glob.strip():
+            raise RuntimeError(f"Path '{curr}' contains a wildcard at the beginning. ")
+        elif find_dir_index < 0:
+            raise RuntimeError(f"Path '{curr}' does not contain a '{find}' component.")
+
+        dst_parts = [p if i != find_dir_index else replace for i, p in enumerate(curr_parts)]
+        new_paths.append(join_path(curr_prot, dst_parts))
+
+    return new_paths
+
+
+def _make_paths_from_prefix(paths: List[str], prefix: str) -> List[str]:
+    """
+    Utility function to make paths using a prefix. This is useful if you want to create a destination path
+    from a source path by prepending a prefix to the source path.
+
+    To create destination paths, we first find the longest common prefix among all source paths. Then, we
+    we remove the prefix from each source path and prepend the new prefix to each source path. For example,
+    if you have a source path of
+    ```
+    current_paths = [
+        "s3://bucket/data/documentsA/**.json.gz",
+        "s3://bucket/data/documentsB/**.json.gz",
+    ]
+    ```
+    and you want to replace `s3://bucket/data/` with `s3://bucket/attributes/`, you can use this function
+    to do that. by calling `_make_paths_from_prefix(current_paths, "s3://bucket/attributes/")`. This will
+    return the following list
+
+    ```
+    [
+        "s3://bucket/attributes/documentsA/",
+        "s3://bucket/attributes/documentsB/",
+    ]
+    ```
+
+    Note how glob patterns are removed from the paths.
+    """
+
+    new_paths: List[str] = []
+    prefix_prot, prefix_path = split_path(prefix)
+    _, relative_paths = make_relative(paths)
+
+    for curr_path in relative_paths:
+        base_curr_path, _ = split_glob(curr_path)
+        new_paths.append(join_path(prefix_prot, prefix_path, base_curr_path))
+
+    return new_paths
+
+
 class TaggerProcessor(BaseParallelProcessor):
     @classmethod
     def get_logger(cls) -> logging.Logger:
         return logging.getLogger(cls.__name__)
 
     @classmethod
     def increment_progressbar(  # type: ignore
@@ -62,55 +124,48 @@
         if experiment_name is None:
             raise RuntimeError("Experiment name not in kwargs, this is a bug! Please report it.")
         experiment_name = make_variable_name(experiment_name)
 
         # skip on failure
         skip_on_failure = kwargs.get("skip_on_failure", False)
 
-        # local read cache
-        local_read_cache = kwargs.get("local_read_cache", None)
-
         # interval at which to update the progress bar; will double if it gets
         # too full
         update_interval = 1
 
         # running document count; gets reset every time we update the progress
         # bar
         docs_cnt = 0
 
         # creating dedicated encoders/decoders speeds up the process
         encoder = msgspec.json.Encoder()
         decoder = msgspec.json.Decoder(InputSpec)
 
-        # this will be used to cache the file locally if needed
-        caching_path = source_path
-
         with ExitStack() as stack:
             try:
                 # open each file for reading and writing. We use open_file_for_read to handle s3 paths and
                 # download the file locally if needed, while gzip.open is used to read and write gzipped files.
                 in_stream = stack.enter_context(smart_open.open(source_path, "rt", encoding="utf-8"))
                 out_stream = stack.enter_context(smart_open.open(destination_path, "wt", encoding="utf-8"))
 
                 for raw in in_stream:
-                    # row = json.loads(raw)
                     row = decoder.decode(raw)
 
                     # running the taggers and merging them flat
                     attributes = {}
                     for tagger_name, tagger in taggers.items():
                         for key_name, key_value in tagger.tag(row).items():
                             key_name = f"{experiment_name}__{tagger_name}__{make_variable_name(key_name)}"
                             attributes[key_name] = key_value
 
                     # make output file
                     output = OutputSpec(source=row.source, id=row.id, attributes=attributes)
 
                     # write the output to the output file
-                    out_stream.write(encoder.encode(output).decode("utf-8") + "\n")  # pyright: ignore
+                    out_stream.write(encoder.encode(output).decode("utf-8") + "\n")
 
                     # increment the number of documents processed so far
                     docs_cnt += 1
 
                     if docs_cnt % update_interval == 0:
                         # update the progress bar every 1000 documents to prevent
                         # buffering
@@ -128,102 +183,83 @@
                     # Intermittent error that occurs when reading from S3
                     raise DolmaRetryableFailure(msg) from e
                 else:
                     if skip_on_failure:
                         raise DolmaShardError(msg) from e
                     else:
                         raise DolmaFatalError(msg) from e
-            finally:
-                if caching_path != source_path and os.path.exists(caching_path):
-                    os.remove(caching_path)
 
         # increment the files progress bar
         cls.increment_progressbar(queue, files=1, documents=docs_cnt)
 
-    @classmethod
-    def main(
-        cls,
-        documents: List[str],
-        destination: Union[None, List[str]] = None,
-        metadata: Union[None, List[str]] = None,
-    ):
-        if destination is None:
-            destination = []
-            for src in documents:
-                src_prot, src_parts = split_path(src)
-                wildcard_index = min([i for i, part in enumerate(src_parts) if "*" in part])
-                doc_dir_index = src_parts.index("documents")
-
-                if doc_dir_index < 0:
-                    raise RuntimeError(
-                        f"Document path {src} does not contain a 'documents' directory. "
-                        "Cannot infer destination path automatically. Please provide it explicitly."
-                    )
-                if doc_dir_index < wildcard_index:
-                    raise RuntimeError(
-                        f"Document path {src} contains a wildcard after the 'documents' directory. "
-                        "Cannot infer destination path automatically. Please provide it explicitly."
-                    )
-
-                dst_parts = [src_parts[i] if i != doc_dir_index else "attributes" for i in range(wildcard_index)]
-                destination.append(join_path(src_prot, dst_parts))
-
-        if metadata is None:
-            _, rel_docs = make_relative(documents)
-
-        # use a local read cache if we are in safe mode or if a local read cache is provided
-        local_read_cache = opts.local_read_cache or (tempfile.gettempdir() if opts.safe_mode else None)
-
-        with tempfile.TemporaryDirectory() as tempdir:
-            metadata_workdir = opts.reuse_existing or tempdir
-            ignore_existing = opts.reuse_existing is None
-            manually_included_paths = opts.manually_included_paths
-            if (
-                manually_included_paths
-                and len(manually_included_paths) == 1
-                and os.path.exists(manually_included_paths[0])
-            ):
-                manually_included_paths = [lp.strip() for lp in open(manually_included_paths[0])]
-            manually_excluded_paths = opts.manually_excluded_paths
-            if (
-                manually_excluded_paths
-                and len(manually_excluded_paths) == 1
-                and os.path.exists(manually_excluded_paths[0])
-            ):
-                manually_excluded_paths = [lp.strip() for lp in open(manually_excluded_paths[0])]
-
-            msg = (
-                "----- TaggerProcessor -----\n"
-                f"source:       {source_prefix}\n"
-                f"destination:  {destination_prefix}\n"
-                f"scratch:      {tempdir}\n"
-                f"taggers:      {', '.join(opts.taggers)}\n"
-                f"parallel:     {opts.parallel}\n"
-                f"debug:        {opts.debug}\n"
-                f"skip on fail: {opts.skip_on_failure}\n"
-                f"reuse prev:   {not ignore_existing}\n"
-                f"workdir:      {metadata_workdir}\n"
-                f"safe mode:    {opts.safe_mode}\n"
-                f"local cache:  {local_read_cache}\n"
-                f"file regex:   {opts.files_regex_pattern}\n"
-                "---------------------------\n"
-            )
-            print(msg)
-
-            parallel_compute = cls(
-                source_prefix=source_prefix,
-                destination_prefix=destination_prefix,
-                metadata_prefix=metadata_workdir,
-                num_processes=opts.parallel,
-                ignore_existing=ignore_existing,
-                debug=opts.debug,
-                include_paths=opts.manually_included_paths,
-                exclude_paths=opts.manually_excluded_paths,
-                files_regex_pattern=opts.files_regex_pattern,
-            )
-            parallel_compute(
-                taggers_names=opts.taggers,
-                experiment_name=opts.experiment_name,
-                skip_on_failure=opts.skip_on_failure,
-                local_read_cache=local_read_cache,
-                retry_on_read_error=opts.retry_on_read_error,
-            )
+
+def create_and_run_tagger(
+    documents: List[str],
+    experiment: str,
+    taggers: List[str],
+    destination: Union[None, str, List[str]] = None,
+    metadata: Union[None, str, List[str]] = None,
+    debug: bool = False,
+    seed: int = 0,
+    ignore_existing: bool = False,
+    skip_on_failure: bool = False,
+    retries_on_error: int = 0,
+    num_processes: int = 1,
+):
+    """This function creates a tagger and runs it on a list of documents.
+
+    Args:
+        documents (List[str]): List of documents to run the taggers on. Each element of the list is a path to
+            a file containing documents in json lines format, or a glob pattern that matches such files.
+        experiment (str): The name of the experiment. This will be used to prefix the names of the attributes,
+            as well as the name of the directory where the outputs will be saved in `destination`.
+        taggers (List[str]): List of taggers to run. Each element of the list is the name of a tagger.
+        destination (Union[None, str, List[str]], optional): The path where the outputs will be saved. If
+            `None`, the outputs will be saved in a directory parallel to the directory containing the
+            documents, with the same name as `experiment`. If a string, paths corresponding to each element
+            of `documents` will be created by determining a relative path from the directory containing the
+            documents.
+        metadata (Union[None, str, List[str]], optional): Location where to save metadata that keeps track of
+            which documents have been processed. If `None`, the metadata will be saved in a temporary directory.
+        debug (bool, optional): Whether to run in debug mode. Defaults to False.
+        seed (int, optional): The seed to use for the random number generator. Defaults to 0.
+        ignore_existing (bool, optional): Whether to ignore existing outputs and re-run the taggers.
+            Defaults to False.
+        skip_on_failure (bool, optional): Whether to skip a document if it fails to process. Defaults to False.
+        retries_on_error (int, optional): Number of times to retry processing a document if it fails.
+            Defaults to 0 (fail immediately)
+        num_processes (int, optional): Number of processes to use. Defaults to 1.
+    """
+
+    if destination is None:
+        try:
+            destination = _make_paths_from_substitution(documents, "documents", f"attributes/{experiment}")
+        except Exception as e:
+            raise RuntimeError("Could not make destination paths from documents paths") from e
+    elif isinstance(destination, str):
+        try:
+            destination = _make_paths_from_prefix(documents, join_path(destination, experiment))
+        except Exception as e:
+            raise RuntimeError(f"Could not make destination paths from prefix {destination}") from e
+
+    metadata = metadata or tempfile.mkdtemp()
+    if isinstance(metadata, str):
+        try:
+            metadata = _make_paths_from_prefix(documents, metadata)
+        except Exception as e:
+            raise RuntimeError(f"Could not make metadata paths from prefix {metadata}") from e
+
+        tagger = TaggerProcessor(
+            source_prefix=documents,
+            destination_prefix=destination,
+            metadata_prefix=metadata,
+            debug=debug,
+            seed=seed,
+            ignore_existing=ignore_existing,
+            retries_on_error=retries_on_error,
+            num_processes=num_processes,
+        )
+        tagger(
+            experiment_name=experiment,
+            taggers_names=taggers,
+            skip_on_failure=skip_on_failure,
+        )
```

### Comparing `dolma-0.6.0/python/dolma/core/taggers.py` & `dolma-0.6.1/python/dolma/core/taggers.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/core/utils.py` & `dolma-0.6.1/python/dolma/core/utils.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/core/vizualizer.py` & `dolma-0.6.1/python/dolma/core/vizualizer.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/data/naughty_words_en.txt` & `dolma-0.6.1/python/dolma/data/naughty_words_en.txt`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/taggers/c4.py` & `dolma-0.6.1/python/dolma/taggers/c4.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/taggers/code.py` & `dolma-0.6.1/python/dolma/taggers/code.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/taggers/gopher.py` & `dolma-0.6.1/python/dolma/taggers/gopher.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/taggers/jigsaw.py` & `dolma-0.6.1/python/dolma/taggers/jigsaw.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/taggers/language.py` & `dolma-0.6.1/python/dolma/taggers/language.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/taggers/length.py` & `dolma-0.6.1/python/dolma/taggers/length.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/taggers/pii.py` & `dolma-0.6.1/python/dolma/taggers/pii.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/python/dolma/taggers/sampling.py` & `dolma-0.6.1/python/dolma/taggers/sampling.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/res/logo.png` & `dolma-0.6.1/res/logo.png`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/src/bloom_filter.rs` & `dolma-0.6.1/src/bloom_filter.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/src/deduper.rs` & `dolma-0.6.1/src/deduper.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/src/lib.rs` & `dolma-0.6.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/src/mixer.rs` & `dolma-0.6.1/src/mixer.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/src/s3_util.rs` & `dolma-0.6.1/src/s3_util.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/src/shard.rs` & `dolma-0.6.1/src/shard.rs`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/config/c4-cleaned.json` & `dolma-0.6.1/tests/config/c4-cleaned.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/config/dedupe-by-url.json` & `dolma-0.6.1/tests/config/dedupe-by-url.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/config/dedupe-paragraphs.json` & `dolma-0.6.1/tests/config/dedupe-paragraphs.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/config/email-spans.json` & `dolma-0.6.1/tests/config/email-spans.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/config/filter-by-spans.json` & `dolma-0.6.1/tests/config/filter-by-spans.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/config/mixer.json` & `dolma-0.6.1/tests/config/mixer.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/config/paragraph-spans.json` & `dolma-0.6.1/tests/config/paragraph-spans.json`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/data/documents.json.gz` & `dolma-0.6.1/tests/data/documents.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/data/duplicate-paragraphs.json.gz` & `dolma-0.6.1/tests/data/duplicate-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/data/expected/dedupe-paragraphs.json.gz` & `dolma-0.6.1/tests/data/expected/dedupe-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/data/expected/email-spans.json.gz` & `dolma-0.6.1/tests/data/expected/email-spans.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/data/expected/filter-by-spans.json.gz` & `dolma-0.6.1/tests/data/expected/filter-by-spans.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/data/expected/mixer.json.gz` & `dolma-0.6.1/tests/data/expected/mixer.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/data/expected/remove-paragraphs.json.gz` & `dolma-0.6.1/tests/data/expected/remove-paragraphs.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/data/pii-attributes.json.gz` & `dolma-0.6.1/tests/data/pii-attributes.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/data/sample-attributes.json.gz` & `dolma-0.6.1/tests/data/sample-attributes.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/data/toxicity-attributes.json.gz` & `dolma-0.6.1/tests/data/toxicity-attributes.json.gz`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/python/test_data_types.py` & `dolma-0.6.1/tests/python/test_data_types.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/python/test_mixer.py` & `dolma-0.6.1/tests/python/test_mixer.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/python/test_omegaconf.py` & `dolma-0.6.1/tests/python/test_omegaconf.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/python/test_paths.py` & `dolma-0.6.1/tests/python/test_paths.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/python/test_runtime.py` & `dolma-0.6.1/tests/python/test_parallel.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/python/test_taggers.py` & `dolma-0.6.1/tests/python/test_taggers.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/tests/python/test_utils.py` & `dolma-0.6.1/tests/python/test_utils.py`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/Cargo.lock` & `dolma-0.6.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `dolma-0.6.0/PKG-INFO` & `dolma-0.6.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolma
-Version: 0.6.0
+Version: 0.6.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: requests
 Requires-Dist: tqdm
@@ -48,62 +48,103 @@
 Project-URL: Homepage, https://github.com/allenai/dolma
 
 # dolma
 
 *Data to feed OLMo's Appetite*
 
 
-<img alt="DOLMa logo. It's a watercolor of grape leaves with the word DOLMa in the top left." src="res/logo.png" width="256"></img>
+<img alt="DOLMa logo. It's a watercolor of grape leaves with the word DOLMa in the top left." src="https://github.com/allenai/dolma/blob/main/res/logo.png?raw=true" width="256"></img>
 
 Data and tools for generating and inspecting OLMo pre-training data.
 
+To get started, install dolma using pip.
 
-## Setup
-
-Install Rust
+```shell
+pip install dolma
 ```
-curl https://sh.rustup.rs -sSf | sh
+
+## Usage
+
+The dolma CLI can be access using the `dolma` command. To see the available commands, use the `--help` flag.
+
+```shell
+dolma --help
 ```
 
-Install [CMake](https://cmake.org/install/)
+At the moment, the CLI supports three commands: `tag`, `dedupe`, and `mix`.
+
+For all commands, configurations can be specified from command line, or by passing a YAML or JSON file using the `-c` flag. For example:
 
-  * On **Mac OSX** with `brew install cmake`
-  * On **Linux** with `apt-get install cmake`
+```shell
+dolma -c config.yaml dedupe --dedupe.name "test"
+```
+
+### `dolma tag`
 
+The tag command is used to run any of the built-in taggers on a set of documents. For example:
 
-Install [OpenSSL](https://www.openssl.org/)
+```shell
+dolma tag \
+    --experiment sample \
+    --documents \
+        's3://ai2-llm/pretraining-data/sources/common-crawl/test/v0/documents/**/*.json.gz' \
+        's3://ai2-llm/pretraining-data/sources/common-crawl/test/v1/documents/*.json.gz' \
+    --taggers random_number_v1 \
+    --processes 2
+```
 
-  * On **Mac OSX** with `brew install openssl re2`
-  * On **Linux** with `apt-get install openssl`
+This command will run the `random_number_v1` tagger on all documents in the specified S3 paths. The results will be written to the `s3://ai2-llm/pretraining-data/sources/common-crawl/test/v0/attributes/sample` and `s3://ai2-llm/pretraining-data/sources/common-crawl/test/v1/attributes/sample` paths.
 
-Install [Protobuf]()
+### `dolma dedupe`
 
-  * On **Mac OSX** with `brew install protobuf`
-  * On **Linux** with `apt-get install protobuf-compiler`
+The dedupe command is used to deduplicate a set of documents at the attribute level using a bloom filter.
+For example configurations, see directory `test/config`. For example:
 
-Setting up Python
+```shell
+dolma dedupe -c test/config/dedupe-paragraphs.json
 ```
-conda create -n dolma python=3.10
+
+### `dolma mix`
+
+The mix command is used to mix documents from multiple sources, optionally filtering by attributes and/or performing string replacement. For example configurations, see directory `test/config`. For example:
+
+```shell
+dolma mix -c test/config/mixer.json
 ```
 
 
-Install [Maturin](https://www.maturin.rs/)
+## Development
+
+Create a conda environment with Python >= 3.8. In this case, we use Python 3.10 and use Anaconda to create the environment.
 
+```shell
+conda create -n dolma python=3.10
 ```
-pip install maturin
-maturin develop
+
+After creating the environment, activate it and install necessary tools using the included makefile.
+
+```shell
+conda activate dolma
+make setup
 ```
 
+Finally, to begin development, install the repository in editable mode using maturin.
 
-Installing this repository
+```shell
+make develop
 ```
-cd dolma
-pip install -e .
+
+To run tests, use the following command.
+
+```shell
+make test
 ```
 
+You can choose to run just the Python or Rust tests by calling `make test-python` or `make test-rust` respectively.
+
 
 ## Citation
 
 If you use this repository, please cite it as:
 
 ```bibtex
 @software{dolma,
```

