# Comparing `tmp/xcsf-1.2.8.tar.gz` & `tmp/xcsf-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsf-1.2.8.tar", last modified: Sun Jul  9 14:41:09 2023, max compression
+gzip compressed data, was "xcsf-1.2.9.tar", last modified: Sun Jul  9 17:49:46 2023, max compression
```

## Comparing `xcsf-1.2.8.tar` & `xcsf-1.2.9.tar`

### file list

```diff
@@ -1,691 +1,698 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.581202 xcsf-1.2.8/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7267 2023-07-09 14:14:55.000000 xcsf-1.2.8/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    35149 2023-05-01 09:22:08.000000 xcsf-1.2.8/LICENSE.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      162 2023-05-01 09:22:08.000000 xcsf-1.2.8/MANIFEST.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4708 2023-07-09 14:41:09.581202 xcsf-1.2.8/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3264 2023-05-05 14:22:38.000000 xcsf-1.2.8/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.505202 xcsf-1.2.8/lib/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.509202 xcsf-1.2.8/lib/cJSON/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      428 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/.editorconfig
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       37 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/.git
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      340 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/.gitattributes
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.509202 xcsf-1.2.8/lib/cJSON/.github/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2386 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/.github/CONTRIBUTING.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.509202 xcsf-1.2.8/lib/cJSON/.github/workflows/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3307 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/.github/workflows/CI.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      158 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      602 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/.travis.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    24245 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/CHANGELOG.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9922 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3343 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/CONTRIBUTORS.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1084 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4650 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/Makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    27272 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/README.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2284 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/appveyor.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    77769 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/cJSON.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15829 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/cJSON.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    40691 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/cJSON_Utils.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3938 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/cJSON_Utils.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.509202 xcsf-1.2.8/lib/cJSON/fuzzing/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1169 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/CMakeLists.txt
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      153 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/afl-prepare-linux.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4192 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/afl.c
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      192 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/afl.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1695 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/cjson_read_fuzzer.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      992 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/fuzz_main.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.513202 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      585 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test1
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       81 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test10
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      151 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test11
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      244 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test2
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test3
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test3.bu
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test3.uf
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test3.uu
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3465 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test4
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      875 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test5
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      487 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test6
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      401 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test7
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      249 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test8
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       52 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test9
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      914 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/json.dict
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      529 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/fuzzing/ossfuzz.sh
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.513202 xcsf-1.2.8/lib/cJSON/library_config/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      802 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/library_config/cJSONConfig.cmake.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      379 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/library_config/cJSONConfigVersion.cmake.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      304 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/library_config/libcjson.pc.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      351 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/library_config/libcjson_utils.pc.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      728 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/library_config/uninstall.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7711 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/test.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.517202 xcsf-1.2.8/lib/cJSON/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4530 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12775 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/cjson_add.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4166 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/common.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8588 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/compare_tests.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.521202 xcsf-1.2.8/lib/cJSON/tests/inputs/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      583 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test1
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      474 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test1.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       79 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test10
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       78 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test10.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      149 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test11
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      147 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test11.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      242 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test2
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      268 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test2.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test3
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      505 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test3.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3464 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test4
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3285 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test4.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      873 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test5
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      900 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test5.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      484 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test6
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      399 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test7
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      347 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test7.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      247 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test8
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      228 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test8.expected
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       50 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test9
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       34 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/inputs/test9.expected
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.521202 xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      183 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/.editorconfig
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       34 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       25 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/.npmignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2306 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/README.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2659 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/cjson-utils-tests.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      393 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/package.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4031 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/spec_tests.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    17205 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/tests.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6776 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/json_patch_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5456 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/minify_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    26201 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/misc_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3386 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/misc_utils_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7766 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/old_utils_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5068 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/parse_array.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7999 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/parse_examples.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3434 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/parse_hex4.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3902 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/parse_number.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5568 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/parse_object.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4679 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/parse_string.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3302 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/parse_value.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4168 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/parse_with_opts.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3818 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/print_array.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4447 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/print_number.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4223 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/print_object.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2822 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/print_string.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3189 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/print_value.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6854 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/readme_examples.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.525202 xcsf-1.2.8/lib/cJSON/tests/unity/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      573 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/.gitattributes
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      212 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      852 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/.travis.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7806 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.525202 xcsf-1.2.8/lib/cJSON/tests/unity/auto/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3462 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/auto/colour_prompt.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1178 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/auto/colour_reporter.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1273 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/auto/generate_config.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11086 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/auto/generate_module.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18170 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/auto/generate_test_runner.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6995 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/auto/parse_output.rb
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)     7698 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/auto/stylize_as_junit.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      766 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/auto/test_file_filter.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      201 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/auto/type_sanitizer.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5173 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/auto/unity_test_summary.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4143 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/auto/unity_test_summary.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5939 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/auto/unity_to_junit.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.525202 xcsf-1.2.8/lib/cJSON/tests/unity/docs/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8092 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/docs/ThrowTheSwitchCodingStandard.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   144467 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/docs/UnityAssertionsCheatSheetSuitableforPrintingandPossiblyFraming.pdf
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    28588 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/docs/UnityAssertionsReference.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18107 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/docs/UnityConfigurationGuide.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8249 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/docs/UnityGettingStartedGuide.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9332 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/docs/UnityHelperScriptsGuide.md
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1123 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/docs/license.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.525202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2237 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      139 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/readme.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      862 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      335 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode2.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2393 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      567 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode2.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/test/test_runners/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1178 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode2_Runner.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1998 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode_Runner.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1768 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      175 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/readme.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      847 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      331 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode2.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2453 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      664 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode2.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/test/test_runners/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      271 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode2_Runner.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode_Runner.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      221 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/test/test_runners/all_tests.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/helper/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      405 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/helper/UnityHelper.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      483 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/helper/UnityHelper.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      884 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/rakefile.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8367 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/rakefile_helper.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      696 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/readme.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      847 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      331 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode2.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      852 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/target_gcc_32.yml
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2357 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      565 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12322 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/examples/unity_config.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.505202 xcsf-1.2.8/lib/cJSON/tests/unity/extras/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/extras/eclipse/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1138 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/eclipse/error_parsers.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1109 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/rakefile.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6621 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/rakefile_helper.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      515 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/readme.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.529202 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10386 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3348 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1518 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_internals.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1892 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_malloc_overrides.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.533202 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2314 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/Makefile
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.533202 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/main/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      653 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/main/AllTests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      722 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/template_fixture_tests.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14403 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_Test.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2593 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_TestRunner.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1206 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      628 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.533202 xcsf-1.2.8/lib/cJSON/tests/unity/release/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        5 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/release/build.info
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        7 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/release/version.info
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.533202 xcsf-1.2.8/lib/cJSON/tests/unity/src/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    49464 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/src/unity.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    66485 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/src/unity.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    69552 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/src/unity_internals.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.533202 xcsf-1.2.8/lib/cJSON/tests/unity/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1386 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/.rubocop.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2665 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/Makefile
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.533202 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_cmd.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1271 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_def.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1242 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_head1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      333 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_head1.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1649 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_cmd.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1493 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_def.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1489 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      267 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1831 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1705 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1591 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_param.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1831 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1705 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1798 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_yaml.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1532 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_new1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1483 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_new2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1405 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_param.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1532 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_run1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1483 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_run2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1576 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_yaml.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3094 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/rakefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8988 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/rakefile_helper.rb
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.533202 xcsf-1.2.8/lib/cJSON/tests/unity/test/spec/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4386 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/spec/generate_module_existing_file_spec.rb
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.533202 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1552 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/clang_file.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1552 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/clang_strict.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      917 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/gcc_32.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      942 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/gcc_64.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      856 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/gcc_auto_limits.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1139 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/gcc_auto_stdint.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      854 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/gcc_manual_math.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2960 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/hitech_picc18.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2060 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_arm_v4.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1886 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_arm_v5.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1886 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_arm_v5_3.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2274 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_armcortex_LM3S9B92_v5_4.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1898 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_cortexm3_v5.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2244 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_msp430.yml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2052 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_sh2a_v6.yml
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.533202 xcsf-1.2.8/lib/cJSON/tests/unity/test/testdata/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      221 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/testdata/CException.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/testdata/Defs.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      452 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/testdata/cmock.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      291 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/testdata/mockMock.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5137 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/testdata/testRunnerGenerator.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1356 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorSmall.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5844 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorWithMocks.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.537202 xcsf-1.2.8/lib/cJSON/tests/unity/test/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    47428 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/tests/test_generate_test_runner.rb
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3442 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/tests/testparameterized.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   123592 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity/test/tests/testunity.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      121 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/tests/unity_setup.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/cJSON/valgrind.supp
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.541202 xcsf-1.2.8/lib/dSFMT/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       37 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/.git
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       30 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/.gitattributes
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       23 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/.gitignore
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2505 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/CHANGE-LOG.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1159 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/FILES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1697 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/LICENSE.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6429 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/Makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1022 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/Makefile.me
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2040 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/README.jp.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/README.txt
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      368 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/check.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3482 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-common.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2437 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-params.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1466 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-params11213.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1458 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-params1279.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1474 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-params132049.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1468 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-params19937.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1476 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-params216091.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1458 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-params2203.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1460 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-params4253.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1468 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-params44497.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1452 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-params521.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1466 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-params86243.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9492 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-ref.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   170957 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-src-2.0.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   196085 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-src-2.0.zip
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   286679 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-src-2.1.1.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   319806 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-src-2.1.1.zip
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   251845 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-src-2.1.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   280951 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT-src-2.1.zip
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41871 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT.11213.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41869 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT.1279.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41873 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT.132049.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT.19937.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41874 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT.216091.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41869 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT.2203.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41870 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT.4253.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT.44497.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41868 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT.521.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT.86243.out.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    19933 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22620 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/dSFMT.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      332 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/debug.log
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    76640 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/doxygen.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    56023 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/doxygen.cfg.bak
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.545202 xcsf-1.2.8/lib/dSFMT/html/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2202 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/annotated.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      705 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/bc_s.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2825 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/classes.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      126 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/closed.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    56903 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/d_s_f_m_t_8c.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   121388 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/d_s_f_m_t_8h.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    66996 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/d_s_f_m_t_8h_source.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16142 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/doxygen.css
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3942 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/doxygen.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2628 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/files.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2576 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/functions.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2468 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/functions_vars.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11998 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/globals.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3184 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/globals_defs.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9926 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/globals_func.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2320 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/globals_type.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2536 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/globals_vars.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11775 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/howto-compile.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9777 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/index.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    86410 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/jquery.js
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1797 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/mainpage_8txt.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      159 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/nav_f.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       97 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/nav_h.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      118 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/open.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5685 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/struct_d_s_f_m_t___t.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      140 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/tab_a.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      178 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/tab_b.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      192 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/tab_h.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      189 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/tab_s.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1095 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/tabs.css
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5509 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/html/union_w128___t.html
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.565202 xcsf-1.2.8/lib/dSFMT/jump/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       35 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/CHANGE-LOG.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1438 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/FILES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1697 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/LICENSE.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3738 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/Makefile
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1564 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/Makefile.me
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   387016 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/calc-characteristic
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   324452 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/calc-characteristic-mpi
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4265 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/calc-characteristic-mpi.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7578 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/calc-characteristic-old.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8670 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/calc-characteristic.cpp
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   320872 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/calc-jump
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1758 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/calc-jump.cpp
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)      216 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/check-jump.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2242 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/dSFMT-calc-jump.hpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4493 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/dSFMT-jump.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      596 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/dSFMT-jump.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7761 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/dSFMText.hpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    76359 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/debug.fix.11213.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)  1078648 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/debug.txt
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   316464 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/degree
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1281 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/degree.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    39223 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/degree.xlsx
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    76620 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/doxygen.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    56003 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/doxygen.cfg.bak
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22586 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/fac.fix.11213.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   264292 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/fac.fix.132049.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4473 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/fac.fix.2203.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   266939 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/fac.lcm.132049.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   436638 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/fac.lcm.216091.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4503 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/fac.lcm.2203.txt
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   366344 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/factorization
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1591 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/factorization.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2880 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/fix.11213.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    33093 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/fix.132049.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5064 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/fix.19937.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      615 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/fix.2203.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11200 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/fix.44497.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21652 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/fix.86243.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.569202 xcsf-1.2.8/lib/dSFMT/jump/html/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2110 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/annotated.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      705 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/bc_s.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      147 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/bdwn.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2512 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/classes.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      126 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/closed.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4946 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8427 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp_source.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10812 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/d_s_f_m_t-jump_8c.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16142 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/doxygen.css
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3942 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/doxygen.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2354 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/files.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2343 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/functions.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2235 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/functions_vars.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2779 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/globals.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2527 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/globals_func.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2174 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/globals_vars.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5241 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/index.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    86410 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/jquery.js
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1880 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/mainpage_8txt.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7747 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/namespacedsfmt.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2503 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/namespacemembers.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2382 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/namespacemembers_func.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2123 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/namespaces.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      159 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/nav_f.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       97 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/nav_h.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      118 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/open.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3734 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/struct_f_i_x___t.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      140 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/tab_a.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      178 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/tab_b.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      192 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/tab_h.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      189 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/tab_s.png
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1095 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/html/tabs.css
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      839 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/lcm.1279.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   455421 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/lcm.132049.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   479378 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/lcm.216091.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   124744 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/lcm.216091.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2520 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/lcm.4253.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      358 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/lcm.521.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18059 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/lcm.86243.tar.gz
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1535 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/mainpage.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      100 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/memo.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      528 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/params.csv
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2883 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/poly.11213.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      385 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/poly.1279.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    33388 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/poly.132049.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5089 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/poly.19937.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    54080 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/poly.216091.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      598 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/poly.2203.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1114 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/poly.4253.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11284 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/poly.44497.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      176 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/poly.521.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21836 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/poly.86243.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8246 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/readme-jp.html
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6265 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/readme.html
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)    26496 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/sample1
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1908 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/sample1.c
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)    18344 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/sample2
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2806 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/sample2.c
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/test-jump-M11213
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/test-jump-M1279
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   363792 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/test-jump-M132049
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/test-jump-M19937
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   376080 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/test-jump-M216091
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   343264 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/test-jump-M2203
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   343264 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/test-jump-M4253
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   351456 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/test-jump-M44497
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   339168 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/test-jump-M521
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)   355600 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/test-jump-M86243
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6612 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/jump/test-jump.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3986 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/mainpage.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      557 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/sample1.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1642 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/sample2.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/sample3.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/sample4.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    19611 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/dSFMT/test.c
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.569202 xcsf-1.2.8/lib/doctest/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6159 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.505202 xcsf-1.2.8/lib/doctest/examples/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.569202 xcsf-1.2.8/lib/doctest/examples/all_features/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7948 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/examples/all_features/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.569202 xcsf-1.2.8/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5086 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.569202 xcsf-1.2.8/lib/doctest/examples/exe_with_static_libs/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1556 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6731 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.569202 xcsf-1.2.8/lib/doctest/examples/executable_dll_and_plugin/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1184 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.505202 xcsf-1.2.8/lib/doctest/examples/installed_doctest_cmake/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.569202 xcsf-1.2.8/lib/doctest/examples/installed_doctest_cmake/dll/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      444 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/examples/installed_doctest_cmake/dll/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.569202 xcsf-1.2.8/lib/doctest/examples/installed_doctest_cmake/executable/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      284 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/examples/installed_doctest_cmake/executable/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.569202 xcsf-1.2.8/lib/doctest/examples/mpi/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      276 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/examples/mpi/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.505202 xcsf-1.2.8/lib/doctest/scripts/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.573202 xcsf-1.2.8/lib/doctest/scripts/cmake/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      979 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/scripts/cmake/assemble_single_header.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8954 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/scripts/cmake/common.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7762 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/scripts/cmake/doctest.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3688 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/scripts/cmake/doctestAddTests.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2952 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/scripts/cmake/exec_test.cmake
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.573202 xcsf-1.2.8/lib/doctest/scripts/how_stuff_works/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      201 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/scripts/how_stuff_works/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.573202 xcsf-1.2.8/lib/doctest/scripts/playground/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      364 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/doctest/scripts/playground/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.573202 xcsf-1.2.8/lib/pybind11/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10999 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.505202 xcsf-1.2.8/lib/pybind11/include/
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.573202 xcsf-1.2.8/lib/pybind11/include/pybind11/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23979 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7069 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    65705 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8458 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      120 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/common.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2096 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/complex.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.573202 xcsf-1.2.8/lib/pybind11/include/pybind11/detail/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    28337 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    49082 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5491 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    17981 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    24008 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    42266 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1625 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/detail/typeid.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    31971 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11735 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4731 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4695 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6923 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/gil.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8862 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    79251 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9051 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2181 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/options.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)   126295 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    90338 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/pytypes.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.573202 xcsf-1.2.8/lib/pybind11/include/pybind11/stl/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4185 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14556 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    27013 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/include/pybind11/stl_bind.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.573202 xcsf-1.2.8/lib/pybind11/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    20608 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tests/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.573202 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2639 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.573202 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/installed_embed/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1171 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.573202 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/installed_function/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1293 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.577202 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/installed_target/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1685 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.577202 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1353 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.577202 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1163 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.577202 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1368 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.577202 xcsf-1.2.8/lib/pybind11/tests/test_embed/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1798 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tests/test_embed/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.577202 xcsf-1.2.8/lib/pybind11/tools/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2350 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3105 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10890 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/FindPythonLibsNew.cmake
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)     1423 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/check-style.sh
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      952 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1031 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/libsize.py
--rwxrwxr-x   0 unknown   (1000) unknown   (1000)     1282 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/make_changelog.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13487 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/pybind11Common.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6930 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8804 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/pybind11NewTools.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7711 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       94 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/pyproject.toml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1851 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/setup_global.py.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1057 2023-05-01 09:22:11.000000 xcsf-1.2.8/lib/pybind11/tools/setup_main.py.in
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-07-09 14:41:09.581202 xcsf-1.2.8/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4550 2023-07-09 14:14:38.000000 xcsf-1.2.8/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.577202 xcsf-1.2.8/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1386 2023-05-01 09:22:08.000000 xcsf-1.2.8/test/CMakeLists.txt
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.581202 xcsf-1.2.8/xcsf/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4521 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/CMakeLists.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       20 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10726 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/__init__.pyi
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8230 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/act_integer.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2787 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/act_integer.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9843 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/act_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2914 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/act_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5610 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/action.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9383 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/action.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7633 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/blas.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1579 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/blas.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    19312 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cl.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3024 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cl.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21808 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/clset.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2292 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/clset.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6348 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/clset_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1636 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/clset_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8819 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_dgp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2878 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_dgp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5977 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_dummy.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2643 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_dummy.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13386 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_ellipsoid.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3046 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_ellipsoid.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8983 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_gp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2803 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_gp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11827 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3331 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15096 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_rectangle.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3097 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_rectangle.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13578 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_ternary.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3221 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/cond_ternary.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    13833 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/condition.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12061 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/condition.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2291 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/config.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      914 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/config.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23498 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/dgp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3447 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/dgp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16108 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/ea.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3096 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/ea.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1675 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/env.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3350 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/env.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7316 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/env_csv.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1679 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/env_csv.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7587 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/env_maze.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2018 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/env_maze.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4060 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/env_mux.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1720 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/env_mux.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    18130 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/gp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3137 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/gp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4443 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/image.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1149 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/image.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6930 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/loss.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2531 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/loss.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2202 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/main.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14550 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3083 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6333 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_activations.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4420 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_activations.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    17673 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    12532 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22350 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_args.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3010 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_args.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8550 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_avgpool.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2595 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_avgpool.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15031 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_connected.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2669 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_connected.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21064 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_convolutional.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2869 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_convolutional.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8227 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_dropout.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2578 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_dropout.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    25430 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_lstm.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2479 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_lstm.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11181 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_maxpool.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2587 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_maxpool.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8094 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_noise.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2533 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_noise.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    16764 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_recurrent.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2663 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_recurrent.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7627 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_softmax.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2577 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_softmax.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9233 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_upsample.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2620 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/neural_layer_upsample.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5411 2023-05-01 09:36:46.000000 xcsf-1.2.8/xcsf/pa.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1168 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/pa.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    25930 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/param.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3375 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/param.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1486 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/perf.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      944 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/perf.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6703 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/pred_constant.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2542 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/pred_constant.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14958 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/pred_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3441 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/pred_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11945 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/pred_nlms.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2918 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/pred_nlms.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11788 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/pred_rls.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3074 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/pred_rls.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10334 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/prediction.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10375 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/prediction.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    52149 2023-07-09 14:13:14.000000 xcsf-1.2.8/xcsf/pybind_wrapper.cpp
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7380 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/rule_dgp.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4871 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/rule_dgp.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7916 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/rule_neural.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5047 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/rule_neural.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3796 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/sam.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1216 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/sam.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.581202 xcsf-1.2.8/xcsf/utils/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/utils/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4045 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/utils/types.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5758 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/utils/viz.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3180 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/utils.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3501 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/utils.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8386 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/xcs_rl.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1571 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/xcs_rl.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7283 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/xcs_supervised.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1410 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/xcs_supervised.h
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6272 2023-05-01 09:22:08.000000 xcsf-1.2.8/xcsf/xcsf.c
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6725 2023-07-09 14:15:08.000000 xcsf-1.2.8/xcsf/xcsf.h
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 14:41:09.581202 xcsf-1.2.8/xcsf.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4708 2023-07-09 14:41:09.000000 xcsf-1.2.8/xcsf.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21360 2023-07-09 14:41:09.000000 xcsf-1.2.8/xcsf.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-09 14:41:09.000000 xcsf-1.2.8/xcsf.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-05-01 09:53:28.000000 xcsf-1.2.8/xcsf.egg-info/not-zip-safe
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       15 2023-07-09 14:41:09.000000 xcsf-1.2.8/xcsf.egg-info/top_level.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.020662 xcsf-1.2.9/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7267 2023-07-09 17:44:19.000000 xcsf-1.2.9/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    35149 2023-05-01 09:22:08.000000 xcsf-1.2.9/LICENSE.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      162 2023-05-01 09:22:08.000000 xcsf-1.2.9/MANIFEST.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4708 2023-07-09 17:49:46.020662 xcsf-1.2.9/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3264 2023-05-05 14:22:38.000000 xcsf-1.2.9/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      428 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/.editorconfig
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       37 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/.git
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      340 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/.gitattributes
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/.github/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2386 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/.github/CONTRIBUTING.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/.github/workflows/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3308 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/.github/workflows/CI.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      599 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/.github/workflows/ci-fuzz.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      171 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      602 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/.travis.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    24882 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/CHANGELOG.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10330 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3903 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/CONTRIBUTORS.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1084 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4650 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/Makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    27632 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/README.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2284 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/appveyor.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    77959 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/cJSON.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16193 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/cJSON.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    40729 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/cJSON_Utils.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3938 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/cJSON_Utils.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/fuzzing/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1169 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/CMakeLists.txt
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      153 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/afl-prepare-linux.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4192 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/afl.c
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      192 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/afl.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1695 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/cjson_read_fuzzer.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      992 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/fuzz_main.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      585 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test1
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       81 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test10
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      151 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test11
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      244 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test2
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3.bu
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3.uf
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3.uu
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3465 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test4
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      875 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test5
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      487 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test6
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      401 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test7
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      249 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test8
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       52 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test9
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      914 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/json.dict
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      529 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/fuzzing/ossfuzz.sh
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/library_config/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      802 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/library_config/cJSONConfig.cmake.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      379 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/library_config/cJSONConfigVersion.cmake.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      304 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/library_config/libcjson.pc.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      351 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/library_config/libcjson_utils.pc.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      728 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/library_config/uninstall.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7711 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/test.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/cJSON/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4530 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12775 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/cjson_add.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4166 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8588 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/compare_tests.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/inputs/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      583 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test1
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      474 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test1.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       79 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test10
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       78 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test10.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      149 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test11
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      147 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test11.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      242 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test2
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      268 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test2.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      603 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test3
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      505 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test3.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3464 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test4
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3285 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test4.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      873 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test5
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      900 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test5.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      484 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test6
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      399 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test7
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      347 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test7.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      247 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test8
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      228 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test8.expected
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       50 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test9
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       34 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/inputs/test9.expected
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      183 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/.editorconfig
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       34 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       25 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/.npmignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2306 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/README.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2659 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/cjson-utils-tests.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      393 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/package.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4031 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/spec_tests.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    17205 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/tests.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6776 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/json_patch_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5456 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/minify_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28328 2023-07-09 17:32:14.000000 xcsf-1.2.9/lib/cJSON/tests/misc_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3386 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/misc_utils_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7766 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/old_utils_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5068 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_array.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7999 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_examples.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3434 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_hex4.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3902 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_number.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5568 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_object.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4679 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_string.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3302 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_value.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4168 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/parse_with_opts.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3818 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/print_array.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4447 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/print_number.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4223 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/print_object.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2822 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/print_string.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3189 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/print_value.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6854 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/readme_examples.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      573 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/.gitattributes
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      212 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      852 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/.travis.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7806 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/auto/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3462 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/colour_prompt.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1178 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/colour_reporter.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1273 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/generate_config.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11086 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/generate_module.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18170 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/generate_test_runner.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6995 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/parse_output.rb
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)     7698 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/stylize_as_junit.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      766 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/test_file_filter.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      201 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/type_sanitizer.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5173 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/unity_test_summary.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4143 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/unity_test_summary.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5939 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/auto/unity_to_junit.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/docs/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8092 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/ThrowTheSwitchCodingStandard.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   144467 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityAssertionsCheatSheetSuitableforPrintingandPossiblyFraming.pdf
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28588 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityAssertionsReference.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18107 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityConfigurationGuide.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8249 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityGettingStartedGuide.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9332 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityHelperScriptsGuide.md
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1123 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/docs/license.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2237 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      139 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/readme.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      862 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      335 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode2.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2393 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      567 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode2.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/test_runners/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1178 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode2_Runner.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1998 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode_Runner.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1768 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      175 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/readme.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      847 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      331 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode2.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2453 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      664 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode2.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/test_runners/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      271 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode2_Runner.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode_Runner.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      221 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/test_runners/all_tests.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/helper/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      405 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/helper/UnityHelper.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      483 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/helper/UnityHelper.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      884 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/rakefile.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8367 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/rakefile_helper.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      696 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/readme.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      847 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      331 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       69 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode2.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      852 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/target_gcc_32.yml
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2357 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      565 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12322 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/examples/unity_config.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.988664 xcsf-1.2.9/lib/cJSON/tests/unity/extras/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/extras/eclipse/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1138 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/eclipse/error_parsers.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1109 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/rakefile.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6621 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/rakefile_helper.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      515 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/readme.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10386 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3348 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1518 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_internals.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1892 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_malloc_overrides.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2314 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/Makefile
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/main/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      653 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/main/AllTests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      722 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/template_fixture_tests.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14403 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_Test.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2593 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_TestRunner.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1206 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      628 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/release/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        5 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/release/build.info
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        7 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/release/version.info
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/src/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    49464 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/src/unity.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    66485 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/src/unity.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    69552 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/src/unity_internals.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.996663 xcsf-1.2.9/lib/cJSON/tests/unity/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1386 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/.rubocop.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2665 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/Makefile
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.000663 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_cmd.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1271 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_def.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1242 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_head1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      333 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_head1.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1649 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_cmd.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1493 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_def.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1489 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      267 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1831 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1705 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1591 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_param.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1831 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1705 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1798 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_yaml.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1532 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_new1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1483 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_new2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1405 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_param.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1532 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_run1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1483 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_run2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1576 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_yaml.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3094 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/rakefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8988 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/rakefile_helper.rb
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.000663 xcsf-1.2.9/lib/cJSON/tests/unity/test/spec/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4386 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/spec/generate_module_existing_file_spec.rb
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.000663 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1552 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/clang_file.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1552 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/clang_strict.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      917 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_32.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      942 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_64.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      856 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_auto_limits.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1139 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_auto_stdint.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      854 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_manual_math.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2960 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/hitech_picc18.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2060 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_arm_v4.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1886 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_arm_v5.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1886 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_arm_v5_3.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2274 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_armcortex_LM3S9B92_v5_4.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1898 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_cortexm3_v5.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2244 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_msp430.yml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2052 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_sh2a_v6.yml
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.000663 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      221 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/CException.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       96 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/Defs.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      452 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/cmock.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      291 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/mockMock.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5137 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/testRunnerGenerator.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1356 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorSmall.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5844 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorWithMocks.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.000663 xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    47428 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/test_generate_test_runner.rb
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3442 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/testparameterized.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   123592 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/testunity.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      121 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/tests/unity_setup.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/cJSON/valgrind.supp
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.004663 xcsf-1.2.9/lib/dSFMT/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       37 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/.git
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       30 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/.gitattributes
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       23 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/.gitignore
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2505 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/CHANGE-LOG.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1159 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/FILES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1697 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/LICENSE.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6429 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/Makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1022 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/Makefile.me
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2040 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/README.jp.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/README.txt
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      368 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/check.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3482 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2437 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1466 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params11213.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1458 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params1279.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1474 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params132049.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1468 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params19937.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1476 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params216091.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1458 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params2203.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1460 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params4253.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1468 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params44497.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1452 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params521.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1466 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-params86243.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9492 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-ref.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   170957 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.0.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   196085 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.0.zip
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   286679 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.1.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   319806 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.1.zip
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   251845 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   280951 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.zip
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41871 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.11213.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41869 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.1279.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41873 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.132049.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.19937.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41874 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.216091.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41869 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.2203.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41870 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.4253.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.44497.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41868 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.521.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    41872 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.86243.out.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19933 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22620 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/dSFMT.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      332 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/debug.log
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    76640 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/doxygen.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    56023 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/doxygen.cfg.bak
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.004663 xcsf-1.2.9/lib/dSFMT/html/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2202 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/annotated.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      705 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/bc_s.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2825 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/classes.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      126 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/closed.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    56903 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/d_s_f_m_t_8c.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   121388 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/d_s_f_m_t_8h.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    66996 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/d_s_f_m_t_8h_source.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16142 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/doxygen.css
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3942 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/doxygen.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2628 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/files.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2576 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/functions.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2468 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/functions_vars.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11998 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/globals.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3184 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/globals_defs.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9926 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/globals_func.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2320 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/globals_type.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2536 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/globals_vars.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11775 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/howto-compile.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9777 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/index.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    86410 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/jquery.js
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1797 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/mainpage_8txt.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      159 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/nav_f.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       97 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/nav_h.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      118 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/open.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5685 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/struct_d_s_f_m_t___t.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      140 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/tab_a.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      178 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/tab_b.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      192 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/tab_h.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      189 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/tab_s.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1095 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/tabs.css
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5509 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/html/union_w128___t.html
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/dSFMT/jump/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       35 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/CHANGE-LOG.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1438 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/FILES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1697 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/LICENSE.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3738 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/Makefile
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1564 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/Makefile.me
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   387016 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   324452 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic-mpi
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4265 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic-mpi.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7578 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic-old.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8670 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic.cpp
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   320872 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-jump
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1758 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/calc-jump.cpp
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)      216 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/check-jump.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2242 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/dSFMT-calc-jump.hpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4493 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/dSFMT-jump.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      596 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/dSFMT-jump.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7761 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/dSFMText.hpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    76359 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/debug.fix.11213.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)  1078648 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/debug.txt
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   316464 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/degree
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1281 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/degree.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    39223 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/degree.xlsx
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    76620 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/doxygen.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    56003 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/doxygen.cfg.bak
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22586 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fac.fix.11213.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   264292 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fac.fix.132049.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4473 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fac.fix.2203.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   266939 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fac.lcm.132049.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   436638 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fac.lcm.216091.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4503 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fac.lcm.2203.txt
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   366344 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/factorization
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1591 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/factorization.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2880 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fix.11213.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    33093 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fix.132049.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5064 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fix.19937.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      615 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fix.2203.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11200 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fix.44497.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21652 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/fix.86243.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/dSFMT/jump/html/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2110 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/annotated.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      705 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/bc_s.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      147 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/bdwn.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2512 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/classes.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      126 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/closed.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4946 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8427 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp_source.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10812 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/d_s_f_m_t-jump_8c.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16142 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/doxygen.css
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3942 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/doxygen.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2354 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/files.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2343 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/functions.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2235 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/functions_vars.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2779 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/globals.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2527 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/globals_func.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2174 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/globals_vars.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5241 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/index.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    86410 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/jquery.js
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1880 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/mainpage_8txt.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7747 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/namespacedsfmt.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2503 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/namespacemembers.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2382 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/namespacemembers_func.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2123 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/namespaces.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      159 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/nav_f.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       97 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/nav_h.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      118 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/open.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3734 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/struct_f_i_x___t.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      140 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/tab_a.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      178 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/tab_b.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      192 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/tab_h.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      189 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/tab_s.png
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1095 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/html/tabs.css
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      839 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.1279.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   455421 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.132049.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   479378 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.216091.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   124744 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.216091.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2520 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.4253.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      358 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.521.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18059 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/lcm.86243.tar.gz
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1535 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/mainpage.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      100 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/memo.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      528 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/params.csv
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2883 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.11213.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      385 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.1279.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    33388 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.132049.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5089 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.19937.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    54080 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.216091.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      598 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.2203.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1114 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.4253.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11284 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.44497.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      176 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.521.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21836 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/poly.86243.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8246 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/readme-jp.html
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6265 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/readme.html
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)    26496 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/sample1
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1908 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/sample1.c
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)    18344 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/sample2
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2806 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/sample2.c
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M11213
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M1279
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   363792 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M132049
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   347360 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M19937
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   376080 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M216091
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   343264 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M2203
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   343264 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M4253
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   351456 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M44497
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   339168 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M521
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)   355600 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump-M86243
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6612 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/jump/test-jump.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3986 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/mainpage.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      557 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/sample1.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1642 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/sample2.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/sample3.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      700 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/sample4.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19611 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/dSFMT/test.c
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6491 2023-07-09 17:33:47.000000 xcsf-1.2.9/lib/doctest/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/doctest/examples/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/all_features/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7948 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/all_features/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5086 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/exe_with_static_libs/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1556 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6731 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/executable_dll_and_plugin/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1184 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/doctest/examples/installed_doctest_cmake/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/installed_doctest_cmake/dll/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      444 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/installed_doctest_cmake/dll/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/installed_doctest_cmake/executable/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      284 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/examples/installed_doctest_cmake/executable/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/examples/mpi/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      311 2023-07-09 17:33:47.000000 xcsf-1.2.9/lib/doctest/examples/mpi/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/doctest/scripts/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/scripts/cmake/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      979 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/scripts/cmake/assemble_single_header.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8999 2023-07-09 17:33:47.000000 xcsf-1.2.9/lib/doctest/scripts/cmake/common.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7762 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/scripts/cmake/doctest.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3688 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/scripts/cmake/doctestAddTests.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2952 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/scripts/cmake/exec_test.cmake
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/scripts/how_stuff_works/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      201 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/scripts/how_stuff_works/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/doctest/scripts/playground/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      364 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/doctest/scripts/playground/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.012663 xcsf-1.2.9/lib/pybind11/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11983 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:45.992663 xcsf-1.2.9/lib/pybind11/include/
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/include/pybind11/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23959 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7069 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    65660 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8458 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      120 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2096 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/complex.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28518 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    52930 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5491 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    17869 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    26305 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    42613 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1625 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/detail/typeid.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/include/pybind11/eigen/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    31450 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/eigen/matrix.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18140 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/eigen/tensor.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      316 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13471 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4731 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5002 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8262 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/gil.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8862 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    79416 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9103 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2734 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)   126420 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    94641 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/pytypes.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/include/pybind11/stl/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4185 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    15337 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    29747 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/include/pybind11/stl_bind.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21675 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tests/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2639 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_embed/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1171 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_function/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1293 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_target/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1685 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1353 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1163 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1368 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tests/test_embed/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1798 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tests/test_embed/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/lib/pybind11/tools/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2350 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3105 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11190 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      817 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/JoinPaths.cmake
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)     1423 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/check-style.sh
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      952 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1040 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1031 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/libsize.py
+-rwxrwxr-x   0 unknown   (1000) unknown   (1000)     1311 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/make_changelog.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      196 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/pybind11.pc.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14033 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/pybind11Common.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6930 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8960 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8361 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       94 2023-05-01 09:22:11.000000 xcsf-1.2.9/lib/pybind11/tools/pyproject.toml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2104 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/setup_global.py.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1234 2023-07-09 17:26:50.000000 xcsf-1.2.9/lib/pybind11/tools/setup_main.py.in
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-07-09 17:49:46.020662 xcsf-1.2.9/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4736 2023-07-09 17:44:13.000000 xcsf-1.2.9/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.016663 xcsf-1.2.9/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1386 2023-05-01 09:22:08.000000 xcsf-1.2.9/test/CMakeLists.txt
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.020662 xcsf-1.2.9/xcsf/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4521 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/CMakeLists.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       20 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10726 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/__init__.pyi
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8230 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/act_integer.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2787 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/act_integer.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9843 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/act_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2914 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/act_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5610 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/action.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9383 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/action.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7633 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/blas.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1579 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/blas.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    19312 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cl.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3024 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cl.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21808 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/clset.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2292 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/clset.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6348 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/clset_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1636 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/clset_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8819 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_dgp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2878 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_dgp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5977 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_dummy.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2643 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_dummy.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13386 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_ellipsoid.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3046 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_ellipsoid.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8983 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_gp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2803 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_gp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11827 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3331 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    15096 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_rectangle.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3097 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_rectangle.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13578 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_ternary.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3221 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/cond_ternary.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    13833 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/condition.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12061 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/condition.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2291 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/config.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      914 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/config.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23543 2023-07-09 16:06:08.000000 xcsf-1.2.9/xcsf/dgp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3447 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/dgp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16108 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/ea.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3096 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/ea.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1675 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3350 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7316 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env_csv.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1679 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env_csv.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7587 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env_maze.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2018 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env_maze.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4060 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env_mux.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1720 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/env_mux.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    18174 2023-07-09 16:06:08.000000 xcsf-1.2.9/xcsf/gp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3137 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/gp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4443 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/image.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1149 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/image.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6930 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/loss.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2531 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/loss.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2202 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/main.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14550 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3083 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6333 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_activations.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4420 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_activations.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    17673 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12532 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22350 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_args.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3010 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_args.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8550 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_avgpool.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2595 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_avgpool.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    15031 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_connected.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2669 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_connected.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21064 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_convolutional.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2869 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_convolutional.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8227 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_dropout.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2578 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_dropout.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    25430 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_lstm.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2479 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_lstm.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11181 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_maxpool.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2587 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_maxpool.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8094 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_noise.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2533 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_noise.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    16764 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_recurrent.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2663 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_recurrent.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7627 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_softmax.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2577 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_softmax.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9233 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_upsample.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2620 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/neural_layer_upsample.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5411 2023-05-01 09:36:46.000000 xcsf-1.2.9/xcsf/pa.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1168 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pa.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    25930 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/param.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3375 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/param.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1486 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/perf.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      944 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/perf.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6703 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_constant.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2542 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_constant.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    14958 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3441 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11945 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_nlms.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2918 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_nlms.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11788 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_rls.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3074 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/pred_rls.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10334 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/prediction.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10375 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/prediction.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    52149 2023-07-09 14:13:14.000000 xcsf-1.2.9/xcsf/pybind_wrapper.cpp
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7380 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/rule_dgp.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4871 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/rule_dgp.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7916 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/rule_neural.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5047 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/rule_neural.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3796 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/sam.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1216 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/sam.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.020662 xcsf-1.2.9/xcsf/utils/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/utils/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4045 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/utils/types.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     5758 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/utils/viz.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3180 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/utils.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3501 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/utils.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8386 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/xcs_rl.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1571 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/xcs_rl.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7283 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/xcs_supervised.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1410 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/xcs_supervised.h
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6272 2023-05-01 09:22:08.000000 xcsf-1.2.9/xcsf/xcsf.c
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6725 2023-07-09 17:44:06.000000 xcsf-1.2.9/xcsf/xcsf.h
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-09 17:49:46.020662 xcsf-1.2.9/xcsf.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4708 2023-07-09 17:49:45.000000 xcsf-1.2.9/xcsf.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    21616 2023-07-09 17:49:45.000000 xcsf-1.2.9/xcsf.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-09 17:49:45.000000 xcsf-1.2.9/xcsf.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-09 17:49:45.000000 xcsf-1.2.9/xcsf.egg-info/not-zip-safe
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       15 2023-07-09 17:49:45.000000 xcsf-1.2.9/xcsf.egg-info/top_level.txt
```

### Comparing `xcsf-1.2.8/CMakeLists.txt` & `xcsf-1.2.9/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 cmake_minimum_required(VERSION 3.12)
 
 project(XCSF CXX C)
 set(PROJECT_VENDOR "Richard Preen")
 set(PROJECT_CONTACT "rpreen@gmail.com")
 set(PROJECT_URL "https://github.com/rpreen/xcsf")
 set(PROJECT_DESCRIPTION "XCSF: Learning Classifier System")
-set(PROJECT_VERSION "1.2.8")
+set(PROJECT_VERSION "1.2.9")
 
 set(CMAKE_C_STANDARD 11)
 set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_C_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_VERBOSE_MAKEFILE OFF)
```

### Comparing `xcsf-1.2.8/LICENSE.md` & `xcsf-1.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/PKG-INFO` & `xcsf-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsf
-Version: 1.2.8
+Version: 1.2.9
 Summary: XCSF learning classifier system: rule-based evolutionary machine learning
 Home-page: https://github.com/rpreen/xcsf
 Maintainer: Richard Preen
 Maintainer-email: rpreen@gmail.com
 License: GPL-3.0
 Keywords: divide and conquer,evolutionary algorithm,genetic programming,learning classifier system,least squares,machine learning,neural networks,neuroevolution,reinforcement learning,rule-based,supervised learning,stochastic gradient descent,XCS,XCSF
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xcsf-1.2.8/README.md` & `xcsf-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/.github/CONTRIBUTING.md` & `xcsf-1.2.9/lib/cJSON/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/.github/workflows/CI.yml` & `xcsf-1.2.9/lib/cJSON/.github/workflows/CI.yml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
           - GCC
           - CLANG
     steps:
     - uses: actions/checkout@v2
     - name: install build dependencies
       run: |
         sudo apt-get update
-        sudo apt-get install clang-8 valgrind
+        sudo apt-get install clang-14 valgrind
     - name: build and test
       shell: bash
       run: |
           if [ "${{ matrix.mem_check }}" == "ENABLE_VALGRIND" ]; then
             EVENT_CMAKE_OPTIONS="-DENABLE_CJSON_UTILS=ON -DENABLE_VALGRIND=ON -DENABLE_SAFE_STACK=ON -DENABLE_SANITIZERS=OFF"
           elif [ "${{ matrix.mem_check }}" == "ENABLE_SANITIZERS" ]; then
             EVENT_CMAKE_OPTIONS="-DENABLE_CJSON_UTILS=ON -DENABLE_VALGRIND=OFF -DENABLE_SAFE_STACK=OFF -DENABLE_SANITIZERS=ON"
```

### Comparing `xcsf-1.2.8/lib/cJSON/.travis.yml` & `xcsf-1.2.9/lib/cJSON/.travis.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/CHANGELOG.md` & `xcsf-1.2.9/lib/cJSON/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+1.7.16 (Jul 5, 2023)
+======
+Features:
+------
+* Add an option for ENABLE_CJSON_VERSION_SO in CMakeLists.txt, see #534
+* Add cmake_policy to CMakeLists.txt, see #163
+* Add cJSON_SetBoolValue, see #639
+* Add meson documentation, see #761
+
+Fixes:
+------
+* Fix memory leak in merge_patch, see #611
+* Fix conflicting target names 'uninstall', see #617
+* Bump cmake version to 3.0 and use new version syntax, see #587
+* Print int without decimal places, see #630
+* Fix 'cjson_utils-static' target not exist, see #625
+* Add allocate check for replace_item_in_object, see #675
+* Fix a null pointer crash in cJSON_ReplaceItemViaPointer, see #726
+
 1.7.15 (Aug 25, 2021)
 ======
 Fixes:
 ------
 * Fix potential core dumped for strrchr, see [#546](https://github.com/DaveGamble/cJSON/pull/546)
 * Fix null pointer crash in cJSON_CreateXxArray, see [#538](https://github.com/DaveGamble/cJSON/pull/538)
 * Fix several null pointer problems on allocation failure, see [#526](https://github.com/DaveGamble/cJSON/pull/526)
```

### Comparing `xcsf-1.2.8/lib/cJSON/CMakeLists.txt` & `xcsf-1.2.9/lib/cJSON/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 set(CMAKE_LEGACY_CYGWIN_WIN32 0)
-cmake_minimum_required(VERSION 2.8.5)
+cmake_minimum_required(VERSION 3.0)
 
-project(cJSON C)
+project(cJSON
+    VERSION 1.7.16
+    LANGUAGES C)
+
+cmake_policy(SET CMP0054 NEW)  # set CMP0054 policy
 
 include(GNUInstallDirs)
 
-set(PROJECT_VERSION_MAJOR 1)
-set(PROJECT_VERSION_MINOR 7)
-set(PROJECT_VERSION_PATCH 15)
 set(CJSON_VERSION_SO 1)
 set(CJSON_UTILS_VERSION_SO 1)
-set(PROJECT_VERSION "${PROJECT_VERSION_MAJOR}.${PROJECT_VERSION_MINOR}.${PROJECT_VERSION_PATCH}")
-
 
 set(custom_compiler_flags)
 
 include(CheckCCompilerFlag)
 option(ENABLE_CUSTOM_COMPILER_FLAGS "Enables custom compiler flags" ON)
 if (ENABLE_CUSTOM_COMPILER_FLAGS)
     if (("${CMAKE_C_COMPILER_ID}" STREQUAL "Clang") OR ("${CMAKE_C_COMPILER_ID}" STREQUAL "GNU"))
@@ -118,14 +117,15 @@
 
 file(GLOB HEADERS cJSON.h)
 set(SOURCES cJSON.c)
 
 option(BUILD_SHARED_AND_STATIC_LIBS "Build both shared and static libraries" Off)
 option(CJSON_OVERRIDE_BUILD_SHARED_LIBS "Override BUILD_SHARED_LIBS with CJSON_BUILD_SHARED_LIBS" OFF)
 option(CJSON_BUILD_SHARED_LIBS "Overrides BUILD_SHARED_LIBS if CJSON_OVERRIDE_BUILD_SHARED_LIBS is enabled" ON)
+option(ENABLE_CJSON_VERSION_SO "Enables cJSON so version" ON)
 
 if ((CJSON_OVERRIDE_BUILD_SHARED_LIBS AND CJSON_BUILD_SHARED_LIBS) OR ((NOT CJSON_OVERRIDE_BUILD_SHARED_LIBS) AND BUILD_SHARED_LIBS))
     set(CJSON_LIBRARY_TYPE SHARED)
 else()
     set(CJSON_LIBRARY_TYPE STATIC)
 endif()
 
@@ -152,25 +152,31 @@
     EXPORT "${CJSON_LIB}"
     ARCHIVE DESTINATION "${CMAKE_INSTALL_FULL_LIBDIR}"
     LIBRARY DESTINATION "${CMAKE_INSTALL_FULL_LIBDIR}"
     RUNTIME DESTINATION "${CMAKE_INSTALL_FULL_BINDIR}"
     INCLUDES DESTINATION "${CMAKE_INSTALL_FULL_INCLUDEDIR}"
 )
 if (BUILD_SHARED_AND_STATIC_LIBS)
-    install(TARGETS "${CJSON_LIB}-static" DESTINATION "${CMAKE_INSTALL_FULL_LIBDIR}")
+    install(TARGETS "${CJSON_LIB}-static"
+    EXPORT "${CJSON_LIB}" 
+    ARCHIVE DESTINATION "${CMAKE_INSTALL_FULL_LIBDIR}"
+    INCLUDES DESTINATION "${CMAKE_INSTALL_FULL_INCLUDEDIR}"
+)
 endif()
 if(ENABLE_TARGET_EXPORT)
     # export library information for CMake projects
     install(EXPORT "${CJSON_LIB}" DESTINATION "${CMAKE_INSTALL_FULL_LIBDIR}/cmake/cJSON")
 endif()
 
-set_target_properties("${CJSON_LIB}"
-    PROPERTIES
-        SOVERSION "${CJSON_VERSION_SO}"
-        VERSION "${PROJECT_VERSION}")
+if(ENABLE_CJSON_VERSION_SO)
+    set_target_properties("${CJSON_LIB}"
+        PROPERTIES
+            SOVERSION "${CJSON_VERSION_SO}"
+            VERSION "${PROJECT_VERSION}")
+endif()
 
 #cJSON_Utils
 option(ENABLE_CJSON_UTILS "Enable building the cJSON_Utils library." OFF)
 if(ENABLE_CJSON_UTILS)
     set(CJSON_UTILS_LIB cjson_utils)
 
     file(GLOB HEADERS_UTILS cJSON_Utils.h)
@@ -195,27 +201,33 @@
         EXPORT "${CJSON_UTILS_LIB}"
         ARCHIVE DESTINATION "${CMAKE_INSTALL_FULL_LIBDIR}"
         LIBRARY DESTINATION "${CMAKE_INSTALL_FULL_LIBDIR}"
         RUNTIME DESTINATION "${CMAKE_INSTALL_FULL_BINDIR}"
         INCLUDES DESTINATION "${CMAKE_INSTALL_FULL_INCLUDEDIR}"
     )
     if (BUILD_SHARED_AND_STATIC_LIBS)
-        install(TARGETS "${CJSON_UTILS_LIB}-static" DESTINATION "${CMAKE_INSTALL_FULL_LIBDIR}")
+        install(TARGETS "${CJSON_UTILS_LIB}-static" 
+        EXPORT "${CJSON_UTILS_LIB}" 
+        ARCHIVE DESTINATION "${CMAKE_INSTALL_FULL_LIBDIR}"
+        INCLUDES DESTINATION "${CMAKE_INSTALL_FULL_INCLUDEDIR}"
+        )
     endif()
     install(FILES cJSON_Utils.h DESTINATION "${CMAKE_INSTALL_FULL_INCLUDEDIR}/cjson")
     install (FILES "${CMAKE_CURRENT_BINARY_DIR}/libcjson_utils.pc" DESTINATION "${CMAKE_INSTALL_FULL_LIBDIR}/pkgconfig")
     if(ENABLE_TARGET_EXPORT)
       # export library information for CMake projects
       install(EXPORT "${CJSON_UTILS_LIB}" DESTINATION "${CMAKE_INSTALL_FULL_LIBDIR}/cmake/cJSON")
     endif()
 
-    set_target_properties("${CJSON_UTILS_LIB}"
-        PROPERTIES
-            SOVERSION "${CJSON_UTILS_VERSION_SO}"
-            VERSION "${PROJECT_VERSION}")
+    if(ENABLE_CJSON_VERSION_SO)
+        set_target_properties("${CJSON_UTILS_LIB}"
+            PROPERTIES
+                SOVERSION "${CJSON_UTILS_VERSION_SO}"
+                VERSION "${PROJECT_VERSION}")
+    endif()
 endif()
 
 # create the other package config files
 configure_file(
     "${CMAKE_CURRENT_SOURCE_DIR}/library_config/cJSONConfig.cmake.in"
     ${PROJECT_BINARY_DIR}/cJSONConfig.cmake @ONLY)
 configure_file(
@@ -251,15 +263,19 @@
     #"check" target that automatically builds everything and runs the tests
     add_custom_target(check
         COMMAND ${CMAKE_CTEST_COMMAND} --output-on-failure
         DEPENDS ${TEST_CJSON})
 endif()
 
 #Create the uninstall target
-add_custom_target(uninstall "${CMAKE_COMMAND}" -P "${PROJECT_SOURCE_DIR}/library_config/uninstall.cmake")
+option(ENABLE_CJSON_UNINSTALL "Enable creating uninstall target" ON)
+if(ENABLE_CJSON_UNINSTALL)
+  add_custom_target(uninstall "${CMAKE_COMMAND}" -P
+    "${PROJECT_SOURCE_DIR}/library_config/uninstall.cmake")
+endif()
 
 # Enable the use of locales
 option(ENABLE_LOCALES "Enable the use of locales" ON)
 if(ENABLE_LOCALES)
 	add_definitions(-DENABLE_LOCALES)
 endif()
```

### Comparing `xcsf-1.2.8/lib/cJSON/CONTRIBUTORS.md` & `xcsf-1.2.9/lib/cJSON/CONTRIBUTORS.md`

 * *Files 17% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 
 Current Maintainer: 
 - [Max Bruckner](https://github.com/FSMaxB) 
 - [Alan Wang](https://github.com/Alanscut)
 
 Contributors:  
 * [Ajay Bhargav](https://github.com/ajaybhargav)
+* [AlexanderVasiljev](https://github.com/AlexanderVasiljev)
 * [Alper Akcan](https://github.com/alperakcan)
 * [Andrew Tang](https://github.com/singku)
+* [Andy](https://github.com/mlh0101)
 * [Anton Sergeev](https://github.com/anton-sergeev)
 * [Benbuck Nason](https://github.com/bnason-nf)
 * [Bernt Johan Damslora](https://github.com/bjda)
 * [Bob Kocisko](https://github.com/bobkocisko)
 * [Christian Schulze](https://github.com/ChristianSch)
 * [Casperinous](https://github.com/Casperinous)
 * [ChenYuan](https://github.com/zjuchenyuan)
@@ -25,28 +27,33 @@
 * [Donough Liu](https://github.com/ldm0)
 * [Erez Oxman](https://github.com/erez-o)
 * Eswar Yaganti
 * [Evan Todd](https://github.com/etodd)
 * [Fabrice Fontaine](https://github.com/ffontaine)
 * Ian Mobley
 * Irwan Djadjadi
+* [hopper-vul](https://github.com/hopper-vul)
 * [HuKeping](https://github.com/HuKeping)
 * [IvanVoid](https://github.com/npi3pak)
 * [Jakub Wilk](https://github.com/jwilk)
 * [Jiri Zouhar](https://github.com/loigu)
 * [Jonathan Fether](https://github.com/jfether)
+* [Joshua Arulsamy](https://github.com/jarulsamy)
 * [Julian Ste](https://github.com/julian-st)
 * [Julián Vásquez](https://github.com/juvasquezg)
+* [Junbo Zheng](https://github.com/Junbo-Zheng)
 * [Kevin Branigan](https://github.com/kbranigan)
 * [Kevin Sapper](https://github.com/sappo)
 * [Kyle Chisholm](https://github.com/ChisholmKyle)
 * [Linus Wallgren](https://github.com/ecksun)
+* [MaxBrandtner](https://github.com/MaxBrandtner)
 * [Mateusz Szafoni](https://github.com/raiden00pl)
 * Mike Pontillo
 * [miaoerduo](https://github.com/miaoerduo)
+* [mohawk2](https://github.com/mohawk2)
 * [Mike Jerris](https://github.com/mjerris)
 * [Mike Robinson](https://github.com/mhrobinson)
 * [Moorthy](https://github.com/moorthy-bs)
 * [myd7349](https://github.com/myd7349)
 * [NancyLi1013](https://github.com/NancyLi1013)
 * Paulo Antonio Alvarez
 * [Paweł Malowany](https://github.com/PawelMalowany)
@@ -57,23 +64,28 @@
 * [raiden00pl](https://github.com/raiden00pl)
 * [Robin Mallinson](https://github.com/rmallins)
 * [Rod Vagg](https://github.com/rvagg)
 * [Roland Meertens](https://github.com/rmeertens)
 * [Romain Porte](https://github.com/MicroJoe)
 * [SANJEEV BA](https://github.com/basanjeev)
 * [Sang-Heon Jeon](https://github.com/lntuition)
+* [Sayan Bandyopadhyay](https://github.com/saynb)
 * [Simon Sobisch](https://github.com/GitMensch)
 * [Simon Ricaldone](https://github.com/simon-p-r)
+* [Stoian Ivanov](https://github.com/sdrsdr)
+* [SuperH-0630](https://github.com/SuperH-0630)
 * [Square789](https://github.com/Square789)
 * [Stephan Gatzka](https://github.com/gatzka)
+* [Tony Langhammer](https://github.com/BigBrainAFK)
 * [Vemake](https://github.com/vemakereporter)
 * [Wei Tan](https://github.com/tan-wei)
 * [Weston Schmidt](https://github.com/schmidtw)
 * [xiaomianhehe](https://github.com/xiaomianhehe)
 * [yangfl](https://github.com/yangfl)
 * [yuta-oxo](https://github.com/yuta-oxo)
 * [Zach Hindes](https://github.com/zhindes)
 * [Zhao Zhixu](https://github.com/zhaozhixu)
+* [10km](https://github.com/10km)
 
 And probably more people on [SourceForge](https://sourceforge.net/p/cjson/bugs/search/?q=status%3Aclosed-rejected+or+status%3Aclosed-out-of-date+or+status%3Awont-fix+or+status%3Aclosed-fixed+or+status%3Aclosed&page=0)
 
 Also thanks to all the people who reported bugs and suggested new features.
```

### Comparing `xcsf-1.2.8/lib/cJSON/LICENSE` & `xcsf-1.2.9/lib/cJSON/LICENSE`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/Makefile` & `xcsf-1.2.9/lib/cJSON/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 UTILS_LIBNAME = libcjson_utils
 CJSON_TEST = cJSON_test
 
 CJSON_TEST_SRC = cJSON.c test.c
 
 LDLIBS = -lm
 
-LIBVERSION = 1.7.15
+LIBVERSION = 1.7.16
 CJSON_SOVERSION = 1
 UTILS_SOVERSION = 1
 
 CJSON_SO_LDFLAG=-Wl,-soname=$(CJSON_LIBNAME).so.$(CJSON_SOVERSION)
 UTILS_SO_LDFLAG=-Wl,-soname=$(UTILS_LIBNAME).so.$(UTILS_SOVERSION)
 
 PREFIX ?= /usr/local
```

### Comparing `xcsf-1.2.8/lib/cJSON/README.md` & `xcsf-1.2.9/lib/cJSON/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 * [License](#license)
 * [Usage](#usage)
   * [Welcome to cJSON](#welcome-to-cjson)
   * [Building](#building)
     * [Copying the source](#copying-the-source)
     * [CMake](#cmake)
     * [Makefile](#makefile)
+    * [Meson](#meson)
     * [Vcpkg](#Vcpkg)
   * [Including cJSON](#including-cjson)
   * [Data Structure](#data-structure)
   * [Working with the data structure](#working-with-the-data-structure)
     * [Basic types](#basic-types)
     * [Arrays](#arrays)
     * [Objects](#objects)
@@ -114,14 +115,15 @@
 * `-DENABLE_SANITIZERS=On`: Compile cJSON with [AddressSanitizer](https://github.com/google/sanitizers/wiki/AddressSanitizer) and [UndefinedBehaviorSanitizer](https://clang.llvm.org/docs/UndefinedBehaviorSanitizer.html) enabled (if possible). (off by default)
 * `-DENABLE_SAFE_STACK`: Enable the [SafeStack](https://clang.llvm.org/docs/SafeStack.html) instrumentation pass. Currently only works with the Clang compiler. (off by default)
 * `-DBUILD_SHARED_LIBS=On`: Build the shared libraries. (on by default)
 * `-DBUILD_SHARED_AND_STATIC_LIBS=On`: Build both shared and static libraries. (off by default)
 * `-DCMAKE_INSTALL_PREFIX=/usr`: Set a prefix for the installation.
 * `-DENABLE_LOCALES=On`: Enable the usage of localeconv method. ( on by default )
 * `-DCJSON_OVERRIDE_BUILD_SHARED_LIBS=On`: Enable overriding the value of `BUILD_SHARED_LIBS` with `-DCJSON_BUILD_SHARED_LIBS`.
+* `-DENABLE_CJSON_VERSION_SO`: Enable cJSON so version. ( on by default )
 
 If you are packaging cJSON for a distribution of Linux, you would probably take these steps for example:
 ```
 mkdir build
 cd build
 cmake .. -DENABLE_CJSON_UTILS=On -DENABLE_CJSON_TEST=Off -DCMAKE_INSTALL_PREFIX=/usr
 make
@@ -140,14 +142,31 @@
 
 ```
 make all
 ```
 
 If you want, you can install the compiled library to your system using `make install`. By default it will install the headers in `/usr/local/include/cjson` and the libraries in `/usr/local/lib`. But you can change this behavior by setting the `PREFIX` and `DESTDIR` variables: `make PREFIX=/usr DESTDIR=temp install`. And uninstall them with: `make PREFIX=/usr DESTDIR=temp uninstall`.
 
+#### Meson
+
+To make cjson work in a project using meson, the libcjson dependency has to be included:
+
+```meson
+project('c-json-example', 'c')
+
+cjson = dependency('libcjson')
+
+example = executable(
+    'example',
+    'example.c',
+    dependencies: [cjson],
+)
+```
+
+
 #### Vcpkg
 
 You can download and install cJSON using the [vcpkg](https://github.com/Microsoft/vcpkg) dependency manager:
 ```
 git clone https://github.com/Microsoft/vcpkg.git
 cd vcpkg
 ./bootstrap-vcpkg.sh
@@ -402,15 +421,15 @@
 
 end:
     cJSON_Delete(monitor);
     return string;
 }
 ```
 
-Alternatively we can use the `cJSON_Add...ToObject` helper functions to make our lifes a little easier:
+Alternatively we can use the `cJSON_Add...ToObject` helper functions to make our lives a little easier:
 
 ```c
 //NOTE: Returns a heap allocated string, you are required to free it after use.
 char *create_monitor_with_helpers(void)
 {
     const unsigned int resolution_numbers[3][2] = {
         {1280, 720},
```

### Comparing `xcsf-1.2.8/lib/cJSON/appveyor.yml` & `xcsf-1.2.9/lib/cJSON/appveyor.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/cJSON.c` & `xcsf-1.2.9/lib/cJSON/cJSON.c`

 * *Files 1% similar despite different names*

```diff
@@ -92,36 +92,36 @@
 static error global_error = { NULL, 0 };
 
 CJSON_PUBLIC(const char *) cJSON_GetErrorPtr(void)
 {
     return (const char*) (global_error.json + global_error.position);
 }
 
-CJSON_PUBLIC(char *) cJSON_GetStringValue(const cJSON * const item) 
+CJSON_PUBLIC(char *) cJSON_GetStringValue(const cJSON * const item)
 {
-    if (!cJSON_IsString(item)) 
+    if (!cJSON_IsString(item))
     {
         return NULL;
     }
 
     return item->valuestring;
 }
 
-CJSON_PUBLIC(double) cJSON_GetNumberValue(const cJSON * const item) 
+CJSON_PUBLIC(double) cJSON_GetNumberValue(const cJSON * const item)
 {
-    if (!cJSON_IsNumber(item)) 
+    if (!cJSON_IsNumber(item))
     {
         return (double) NAN;
     }
 
     return item->valuedouble;
 }
 
 /* This is a safeguard to prevent copy-pasters from using incompatible C and header files */
-#if (CJSON_VERSION_MAJOR != 1) || (CJSON_VERSION_MINOR != 7) || (CJSON_VERSION_PATCH != 15)
+#if (CJSON_VERSION_MAJOR != 1) || (CJSON_VERSION_MINOR != 7) || (CJSON_VERSION_PATCH != 16)
     #error cJSON.h and cJSON.c have different versions. Make sure that both have the same.
 #endif
 
 CJSON_PUBLIC(const char*) cJSON_Version(void)
 {
     static char version[15];
     sprintf(version, "%i.%i.%i", CJSON_VERSION_MAJOR, CJSON_VERSION_MINOR, CJSON_VERSION_PATCH);
@@ -507,15 +507,15 @@
         {
             p->hooks.deallocate(p->buffer);
             p->length = 0;
             p->buffer = NULL;
 
             return NULL;
         }
-        
+
         memcpy(newbuffer, p->buffer, p->offset + 1);
         p->hooks.deallocate(p->buffer);
     }
     p->length = newsize;
     p->buffer = newbuffer;
 
     return newbuffer + p->offset;
@@ -558,14 +558,18 @@
     }
 
     /* This checks for NaN and Infinity */
     if (isnan(d) || isinf(d))
     {
         length = sprintf((char*)number_buffer, "null");
     }
+	else if(d == (double)item->valueint)
+	{
+		length = sprintf((char*)number_buffer, "%d", item->valueint);
+	}
     else
     {
         /* Try 15 decimal places of precision to avoid nonsignificant nonzero digits */
         length = sprintf((char*)number_buffer, "%1.15g", d);
 
         /* Check whether the original double can be recovered */
         if ((sscanf((char*)number_buffer, "%lg", &test) != 1) || !compare_double((double)test, d))
@@ -1099,15 +1103,15 @@
 
     if (value == NULL || 0 == buffer_length)
     {
         goto fail;
     }
 
     buffer.content = (const unsigned char*)value;
-    buffer.length = buffer_length; 
+    buffer.length = buffer_length;
     buffer.offset = 0;
     buffer.hooks = global_hooks;
 
     item = cJSON_New_Item(&global_hooks);
     if (item == NULL) /* memory fail */
     {
         goto fail;
@@ -2283,15 +2287,15 @@
         newitem->prev->next = newitem;
     }
     return true;
 }
 
 CJSON_PUBLIC(cJSON_bool) cJSON_ReplaceItemViaPointer(cJSON * const parent, cJSON * const item, cJSON * replacement)
 {
-    if ((parent == NULL) || (replacement == NULL) || (item == NULL))
+    if ((parent == NULL) || (parent->child == NULL) || (replacement == NULL) || (item == NULL))
     {
         return false;
     }
 
     if (replacement == item)
     {
         return true;
@@ -2353,14 +2357,19 @@
 
     /* replace the name in the replacement */
     if (!(replacement->type & cJSON_StringIsConst) && (replacement->string != NULL))
     {
         cJSON_free(replacement->string);
     }
     replacement->string = (char*)cJSON_strdup((const unsigned char*)string, &global_hooks);
+    if (replacement->string == NULL)
+    {
+        return false;
+    }
+
     replacement->type &= ~cJSON_StringIsConst;
 
     return cJSON_ReplaceItemViaPointer(object, get_object_item(object, string, case_sensitive), replacement);
 }
 
 CJSON_PUBLIC(cJSON_bool) cJSON_ReplaceItemInObject(cJSON *object, const char *string, cJSON *newitem)
 {
@@ -2685,15 +2694,15 @@
         }
         p = n;
     }
 
     if (a && a->child) {
         a->child->prev = n;
     }
-    
+
     return a;
 }
 
 /* Duplication */
 CJSON_PUBLIC(cJSON *) cJSON_Duplicate(const cJSON *item, cJSON_bool recurse)
 {
     cJSON *newitem = NULL;
```

### Comparing `xcsf-1.2.8/lib/cJSON/cJSON.h` & `xcsf-1.2.9/lib/cJSON/cJSON.h`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 #define CJSON_PUBLIC(type) type
 #endif
 #endif
 
 /* project version */
 #define CJSON_VERSION_MAJOR 1
 #define CJSON_VERSION_MINOR 7
-#define CJSON_VERSION_PATCH 15
+#define CJSON_VERSION_PATCH 16
 
 #include <stddef.h>
 
 /* cJSON Types: */
 #define cJSON_Invalid (0)
 #define cJSON_False  (1 << 0)
 #define cJSON_True   (1 << 1)
@@ -275,14 +275,21 @@
 #define cJSON_SetIntValue(object, number) ((object) ? (object)->valueint = (object)->valuedouble = (number) : (number))
 /* helper for the cJSON_SetNumberValue macro */
 CJSON_PUBLIC(double) cJSON_SetNumberHelper(cJSON *object, double number);
 #define cJSON_SetNumberValue(object, number) ((object != NULL) ? cJSON_SetNumberHelper(object, (double)number) : (number))
 /* Change the valuestring of a cJSON_String object, only takes effect when type of object is cJSON_String */
 CJSON_PUBLIC(char*) cJSON_SetValuestring(cJSON *object, const char *valuestring);
 
+/* If the object is not a boolean type this does nothing and returns cJSON_Invalid else it returns the new type*/
+#define cJSON_SetBoolValue(object, boolValue) ( \
+    (object != NULL && ((object)->type & (cJSON_False|cJSON_True))) ? \
+    (object)->type=((object)->type &(~(cJSON_False|cJSON_True)))|((boolValue)?cJSON_True:cJSON_False) : \
+    cJSON_Invalid\
+)
+
 /* Macro for iterating over an array or object */
 #define cJSON_ArrayForEach(element, array) for(element = (array != NULL) ? (array)->child : NULL; element != NULL; element = element->next)
 
 /* malloc/free objects using the malloc/free functions that have been set with cJSON_InitHooks */
 CJSON_PUBLIC(void *) cJSON_malloc(size_t size);
 CJSON_PUBLIC(void) cJSON_free(void *object);
```

### Comparing `xcsf-1.2.8/lib/cJSON/cJSON_Utils.c` & `xcsf-1.2.9/lib/cJSON/cJSON_Utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -1363,14 +1363,15 @@
             {
                 replace_me = cJSON_DetachItemFromObject(target, patch_child->string);
             }
 
             replacement = merge_patch(replace_me, patch_child, case_sensitive);
             if (replacement == NULL)
             {
+                cJSON_Delete(target);
                 return NULL;
             }
 
             cJSON_AddItemToObject(target, patch_child->string, replacement);
         }
         patch_child = patch_child->next;
     }
```

### Comparing `xcsf-1.2.8/lib/cJSON/cJSON_Utils.h` & `xcsf-1.2.9/lib/cJSON/cJSON_Utils.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/CMakeLists.txt` & `xcsf-1.2.9/lib/cJSON/fuzzing/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/afl.c` & `xcsf-1.2.9/lib/cJSON/fuzzing/afl.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/cjson_read_fuzzer.c` & `xcsf-1.2.9/lib/cJSON/fuzzing/cjson_read_fuzzer.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/fuzz_main.c` & `xcsf-1.2.9/lib/cJSON/fuzzing/fuzz_main.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test1` & `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test1`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test3` & `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test3.bu` & `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3.bu`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test3.uf` & `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3.uf`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test3.uu` & `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test3.uu`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test4` & `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test4`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/inputs/test5` & `xcsf-1.2.9/lib/cJSON/fuzzing/inputs/test5`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/json.dict` & `xcsf-1.2.9/lib/cJSON/fuzzing/json.dict`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/fuzzing/ossfuzz.sh` & `xcsf-1.2.9/lib/cJSON/fuzzing/ossfuzz.sh`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/library_config/cJSONConfig.cmake.in` & `xcsf-1.2.9/lib/cJSON/library_config/cJSONConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/library_config/uninstall.cmake` & `xcsf-1.2.9/lib/cJSON/library_config/uninstall.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/test.c` & `xcsf-1.2.9/lib/cJSON/test.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/CMakeLists.txt` & `xcsf-1.2.9/lib/cJSON/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/cjson_add.c` & `xcsf-1.2.9/lib/cJSON/tests/cjson_add.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/common.h` & `xcsf-1.2.9/lib/cJSON/tests/common.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/compare_tests.c` & `xcsf-1.2.9/lib/cJSON/tests/compare_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/inputs/test1` & `xcsf-1.2.9/lib/cJSON/tests/inputs/test1`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/inputs/test3` & `xcsf-1.2.9/lib/cJSON/tests/inputs/test3`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/inputs/test4` & `xcsf-1.2.9/lib/cJSON/tests/inputs/test4`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/inputs/test4.expected` & `xcsf-1.2.9/lib/cJSON/tests/inputs/test4.expected`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/inputs/test5` & `xcsf-1.2.9/lib/cJSON/tests/inputs/test5`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/inputs/test5.expected` & `xcsf-1.2.9/lib/cJSON/tests/inputs/test5.expected`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/README.md` & `xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/README.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/cjson-utils-tests.json` & `xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/cjson-utils-tests.json`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/spec_tests.json` & `xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/spec_tests.json`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/json-patch-tests/tests.json` & `xcsf-1.2.9/lib/cJSON/tests/json-patch-tests/tests.json`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/json_patch_tests.c` & `xcsf-1.2.9/lib/cJSON/tests/json_patch_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/minify_tests.c` & `xcsf-1.2.9/lib/cJSON/tests/minify_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/misc_tests.c` & `xcsf-1.2.9/lib/cJSON/tests/misc_tests.c`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 #include <stdlib.h>
 #include <string.h>
 
 #include "unity/examples/unity_config.h"
 #include "unity/src/unity.h"
 #include "common.h"
 
-
 static void cjson_array_foreach_should_loop_over_arrays(void)
 {
     cJSON array[1];
     cJSON elements[10];
     cJSON *element_pointer = NULL;
     size_t i = 0;
 
@@ -73,15 +72,14 @@
 
     found = cJSON_GetObjectItem(NULL, "test");
     TEST_ASSERT_NULL_MESSAGE(found, "Failed to fail on NULL pointer.");
 
     found = cJSON_GetObjectItem(item, NULL);
     TEST_ASSERT_NULL_MESSAGE(found, "Failed to fail on NULL string.");
 
-
     found = cJSON_GetObjectItem(item, "one");
     TEST_ASSERT_NOT_NULL_MESSAGE(found, "Failed to find first item.");
     TEST_ASSERT_EQUAL_DOUBLE(found->valuedouble, 1);
 
     found = cJSON_GetObjectItem(item, "tWo");
     TEST_ASSERT_NOT_NULL_MESSAGE(found, "Failed to find first item.");
     TEST_ASSERT_EQUAL_DOUBLE(found->valuedouble, 2);
@@ -123,26 +121,28 @@
 
     found = cJSON_GetObjectItemCaseSensitive(item, "One");
     TEST_ASSERT_NULL_MESSAGE(found, "Should not find something that isn't there.");
 
     cJSON_Delete(item);
 }
 
-static void cjson_get_object_item_should_not_crash_with_array(void) {
+static void cjson_get_object_item_should_not_crash_with_array(void)
+{
     cJSON *array = NULL;
     cJSON *found = NULL;
     array = cJSON_Parse("[1]");
 
     found = cJSON_GetObjectItem(array, "name");
     TEST_ASSERT_NULL(found);
 
     cJSON_Delete(array);
 }
 
-static void cjson_get_object_item_case_sensitive_should_not_crash_with_array(void) {
+static void cjson_get_object_item_case_sensitive_should_not_crash_with_array(void)
+{
     cJSON *array = NULL;
     cJSON *found = NULL;
     array = cJSON_Parse("[1]");
 
     found = cJSON_GetObjectItemCaseSensitive(array, "name");
     TEST_ASSERT_NULL(found);
 
@@ -298,15 +298,14 @@
     array = cJSON_CreateArray();
     TEST_ASSERT_NOT_NULL(array);
 
     cJSON_AddItemToArray(array, beginning);
     cJSON_AddItemToArray(array, middle);
     cJSON_AddItemToArray(array, end);
 
-
     memset(replacements, '\0', sizeof(replacements));
 
     /* replace beginning */
     TEST_ASSERT_TRUE(cJSON_ReplaceItemViaPointer(array, beginning, &(replacements[0])));
     TEST_ASSERT_TRUE(replacements[0].prev == end);
     TEST_ASSERT_TRUE(replacements[0].next == middle);
     TEST_ASSERT_TRUE(middle->prev == &(replacements[0]));
@@ -325,25 +324,25 @@
     TEST_ASSERT_TRUE(replacements[1].next == &(replacements[2]));
 
     cJSON_free(array);
 }
 
 static void cjson_replace_item_in_object_should_preserve_name(void)
 {
-    cJSON root[1] = {{ NULL, NULL, NULL, 0, NULL, 0, 0, NULL }};
+    cJSON root[1] = {{NULL, NULL, NULL, 0, NULL, 0, 0, NULL}};
     cJSON *child = NULL;
     cJSON *replacement = NULL;
     cJSON_bool flag = false;
 
     child = cJSON_CreateNumber(1);
     TEST_ASSERT_NOT_NULL(child);
     replacement = cJSON_CreateNumber(2);
     TEST_ASSERT_NOT_NULL(replacement);
 
-    flag  = cJSON_AddItemToObject(root, "child", child);
+    flag = cJSON_AddItemToObject(root, "child", child);
     TEST_ASSERT_TRUE_MESSAGE(flag, "add item to object failed");
     cJSON_ReplaceItemInObject(root, "child", replacement);
 
     TEST_ASSERT_TRUE(root->child == replacement);
     TEST_ASSERT_EQUAL_STRING("child", replacement->string);
 
     cJSON_Delete(replacement);
@@ -431,46 +430,46 @@
     cJSON_Minify(NULL);
     /* skipped because it is only used via a macro that checks for NULL */
     /* cJSON_SetNumberHelper(NULL, 0); */
 
     cJSON_Delete(item);
 }
 
-static void * CJSON_CDECL failing_realloc(void *pointer, size_t size)
+static void *CJSON_CDECL failing_realloc(void *pointer, size_t size)
 {
     (void)size;
     (void)pointer;
     return NULL;
 }
 
 static void ensure_should_fail_on_failed_realloc(void)
 {
     printbuffer buffer = {NULL, 10, 0, 0, false, false, {&malloc, &free, &failing_realloc}};
-    buffer.buffer = (unsigned char*)malloc(100);
+    buffer.buffer = (unsigned char *)malloc(100);
     TEST_ASSERT_NOT_NULL(buffer.buffer);
 
     TEST_ASSERT_NULL_MESSAGE(ensure(&buffer, 200), "Ensure didn't fail with failing realloc.");
 }
 
 static void skip_utf8_bom_should_skip_bom(void)
 {
     const unsigned char string[] = "\xEF\xBB\xBF{}";
-    parse_buffer buffer = { 0, 0, 0, 0, { 0, 0, 0 } };
+    parse_buffer buffer = {0, 0, 0, 0, {0, 0, 0}};
     buffer.content = string;
     buffer.length = sizeof(string);
     buffer.hooks = global_hooks;
 
     TEST_ASSERT_TRUE(skip_utf8_bom(&buffer) == &buffer);
     TEST_ASSERT_EQUAL_UINT(3U, (unsigned int)buffer.offset);
 }
 
 static void skip_utf8_bom_should_not_skip_bom_if_not_at_beginning(void)
 {
     const unsigned char string[] = " \xEF\xBB\xBF{}";
-    parse_buffer buffer = { 0, 0, 0, 0, { 0, 0, 0 } };
+    parse_buffer buffer = {0, 0, 0, 0, {0, 0, 0}};
     buffer.content = string;
     buffer.length = sizeof(string);
     buffer.hooks = global_hooks;
     buffer.offset = 1;
 
     TEST_ASSERT_NULL(skip_utf8_bom(&buffer));
 }
@@ -492,30 +491,32 @@
 {
     cJSON *string = cJSON_CreateString("test");
     cJSON *number = cJSON_CreateNumber(1);
 
     TEST_ASSERT_EQUAL_DOUBLE(cJSON_GetNumberValue(number), number->valuedouble);
     TEST_ASSERT_DOUBLE_IS_NAN(cJSON_GetNumberValue(string));
     TEST_ASSERT_DOUBLE_IS_NAN(cJSON_GetNumberValue(NULL));
-    
+
     cJSON_Delete(number);
     cJSON_Delete(string);
 }
 
-static void cjson_create_string_reference_should_create_a_string_reference(void) {
+static void cjson_create_string_reference_should_create_a_string_reference(void)
+{
     const char *string = "I am a string!";
 
     cJSON *string_reference = cJSON_CreateStringReference(string);
     TEST_ASSERT_TRUE(string_reference->valuestring == string);
     TEST_ASSERT_EQUAL_INT(cJSON_IsReference | cJSON_String, string_reference->type);
 
     cJSON_Delete(string_reference);
 }
 
-static void cjson_create_object_reference_should_create_an_object_reference(void) {
+static void cjson_create_object_reference_should_create_an_object_reference(void)
+{
     cJSON *number_reference = NULL;
     cJSON *number_object = cJSON_CreateObject();
     cJSON *number = cJSON_CreateNumber(42);
     const char key[] = "number";
 
     TEST_ASSERT_TRUE(cJSON_IsNumber(number));
     TEST_ASSERT_TRUE(cJSON_IsObject(number_object));
@@ -525,15 +526,16 @@
     TEST_ASSERT_TRUE(number_reference->child == number);
     TEST_ASSERT_EQUAL_INT(cJSON_Object | cJSON_IsReference, number_reference->type);
 
     cJSON_Delete(number_object);
     cJSON_Delete(number_reference);
 }
 
-static void cjson_create_array_reference_should_create_an_array_reference(void) {
+static void cjson_create_array_reference_should_create_an_array_reference(void)
+{
     cJSON *number_reference = NULL;
     cJSON *number_array = cJSON_CreateArray();
     cJSON *number = cJSON_CreateNumber(42);
 
     TEST_ASSERT_TRUE(cJSON_IsNumber(number));
     TEST_ASSERT_TRUE(cJSON_IsArray(number_array));
     cJSON_AddItemToArray(number_array, number);
@@ -562,15 +564,15 @@
     cJSON_Delete(array);
 }
 
 static void cjson_add_item_to_object_should_not_use_after_free_when_string_is_aliased(void)
 {
     cJSON *object = cJSON_CreateObject();
     cJSON *number = cJSON_CreateNumber(42);
-    char *name = (char*)cJSON_strdup((const unsigned char*)"number", &global_hooks);
+    char *name = (char *)cJSON_strdup((const unsigned char *)"number", &global_hooks);
 
     TEST_ASSERT_NOT_NULL(object);
     TEST_ASSERT_NOT_NULL(number);
     TEST_ASSERT_NOT_NULL(name);
 
     number->string = name;
 
@@ -622,15 +624,15 @@
     const char *reference_valuestring = "reference item should be freed by yourself";
     const char *short_valuestring = "shorter valuestring";
     const char *long_valuestring = "new valuestring which much longer than previous should be changed safely";
     cJSON *item1 = cJSON_CreateString(stringvalue);
     cJSON *item2 = cJSON_CreateStringReference(reference_valuestring);
     char *ptr1 = NULL;
     char *return_value = NULL;
-    
+
     cJSON_AddItemToObject(root, "one", item1);
     cJSON_AddItemToObject(root, "two", item2);
 
     ptr1 = item1->valuestring;
     return_value = cJSON_SetValuestring(cJSON_GetObjectItem(root, "one"), short_valuestring);
     TEST_ASSERT_NOT_NULL(return_value);
     TEST_ASSERT_EQUAL_PTR_MESSAGE(ptr1, return_value, "new valuestring shorter than old should not reallocate memory");
@@ -646,14 +648,72 @@
     return_value = cJSON_SetValuestring(cJSON_GetObjectItem(root, "two"), long_valuestring);
     TEST_ASSERT_NULL_MESSAGE(return_value, "valuestring of reference object should not be changed");
     TEST_ASSERT_EQUAL_STRING(reference_valuestring, cJSON_GetObjectItem(root, "two")->valuestring);
 
     cJSON_Delete(root);
 }
 
+static void cjson_set_bool_value_must_not_break_objects(void)
+{
+    cJSON *bobj, *sobj, *oobj, *refobj = NULL;
+
+    TEST_ASSERT_TRUE((cJSON_SetBoolValue(refobj, 1) == cJSON_Invalid));
+
+    bobj = cJSON_CreateFalse();
+    TEST_ASSERT_TRUE(cJSON_IsFalse(bobj));
+    TEST_ASSERT_TRUE((cJSON_SetBoolValue(bobj, 1) == cJSON_True));
+    TEST_ASSERT_TRUE(cJSON_IsTrue(bobj));
+    cJSON_SetBoolValue(bobj, 1);
+    TEST_ASSERT_TRUE(cJSON_IsTrue(bobj));
+    TEST_ASSERT_TRUE((cJSON_SetBoolValue(bobj, 0) == cJSON_False));
+    TEST_ASSERT_TRUE(cJSON_IsFalse(bobj));
+    cJSON_SetBoolValue(bobj, 0);
+    TEST_ASSERT_TRUE(cJSON_IsFalse(bobj));
+
+    sobj = cJSON_CreateString("test");
+    TEST_ASSERT_TRUE(cJSON_IsString(sobj));
+    cJSON_SetBoolValue(sobj, 1);
+    TEST_ASSERT_TRUE(cJSON_IsString(sobj));
+    cJSON_SetBoolValue(sobj, 0);
+    TEST_ASSERT_TRUE(cJSON_IsString(sobj));
+
+    oobj = cJSON_CreateObject();
+    TEST_ASSERT_TRUE(cJSON_IsObject(oobj));
+    cJSON_SetBoolValue(oobj, 1);
+    TEST_ASSERT_TRUE(cJSON_IsObject(oobj));
+    cJSON_SetBoolValue(oobj, 0);
+    TEST_ASSERT_TRUE(cJSON_IsObject(oobj));
+
+    refobj = cJSON_CreateStringReference("conststring");
+    TEST_ASSERT_TRUE(cJSON_IsString(refobj));
+    TEST_ASSERT_TRUE(refobj->type & cJSON_IsReference);
+    cJSON_SetBoolValue(refobj, 1);
+    TEST_ASSERT_TRUE(cJSON_IsString(refobj));
+    TEST_ASSERT_TRUE(refobj->type & cJSON_IsReference);
+    cJSON_SetBoolValue(refobj, 0);
+    TEST_ASSERT_TRUE(cJSON_IsString(refobj));
+    TEST_ASSERT_TRUE(refobj->type & cJSON_IsReference);
+    cJSON_Delete(refobj);
+
+    refobj = cJSON_CreateObjectReference(oobj);
+    TEST_ASSERT_TRUE(cJSON_IsObject(refobj));
+    TEST_ASSERT_TRUE(refobj->type & cJSON_IsReference);
+    cJSON_SetBoolValue(refobj, 1);
+    TEST_ASSERT_TRUE(cJSON_IsObject(refobj));
+    TEST_ASSERT_TRUE(refobj->type & cJSON_IsReference);
+    cJSON_SetBoolValue(refobj, 0);
+    TEST_ASSERT_TRUE(cJSON_IsObject(refobj));
+    TEST_ASSERT_TRUE(refobj->type & cJSON_IsReference);
+    cJSON_Delete(refobj);
+
+    cJSON_Delete(oobj);
+    cJSON_Delete(bobj);
+    cJSON_Delete(sobj);
+}
+
 int CJSON_CDECL main(void)
 {
     UNITY_BEGIN();
 
     RUN_TEST(cjson_array_foreach_should_loop_over_arrays);
     RUN_TEST(cjson_array_foreach_should_not_dereference_null_pointer);
     RUN_TEST(cjson_get_object_item_should_get_object_items);
@@ -675,10 +735,11 @@
     RUN_TEST(cjson_create_string_reference_should_create_a_string_reference);
     RUN_TEST(cjson_create_object_reference_should_create_an_object_reference);
     RUN_TEST(cjson_create_array_reference_should_create_an_array_reference);
     RUN_TEST(cjson_add_item_to_object_or_array_should_not_add_itself);
     RUN_TEST(cjson_add_item_to_object_should_not_use_after_free_when_string_is_aliased);
     RUN_TEST(cjson_delete_item_from_array_should_not_broken_list_structure);
     RUN_TEST(cjson_set_valuestring_to_object_should_not_leak_memory);
+    RUN_TEST(cjson_set_bool_value_must_not_break_objects);
 
     return UNITY_END();
 }
```

### Comparing `xcsf-1.2.8/lib/cJSON/tests/misc_utils_tests.c` & `xcsf-1.2.9/lib/cJSON/tests/misc_utils_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/old_utils_tests.c` & `xcsf-1.2.9/lib/cJSON/tests/old_utils_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/parse_array.c` & `xcsf-1.2.9/lib/cJSON/tests/parse_array.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/parse_examples.c` & `xcsf-1.2.9/lib/cJSON/tests/parse_examples.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/parse_hex4.c` & `xcsf-1.2.9/lib/cJSON/tests/parse_hex4.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/parse_number.c` & `xcsf-1.2.9/lib/cJSON/tests/parse_number.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/parse_object.c` & `xcsf-1.2.9/lib/cJSON/tests/parse_object.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/parse_string.c` & `xcsf-1.2.9/lib/cJSON/tests/parse_string.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/parse_value.c` & `xcsf-1.2.9/lib/cJSON/tests/parse_value.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/parse_with_opts.c` & `xcsf-1.2.9/lib/cJSON/tests/parse_with_opts.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/print_array.c` & `xcsf-1.2.9/lib/cJSON/tests/print_array.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/print_number.c` & `xcsf-1.2.9/lib/cJSON/tests/print_number.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/print_object.c` & `xcsf-1.2.9/lib/cJSON/tests/print_object.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/print_string.c` & `xcsf-1.2.9/lib/cJSON/tests/print_string.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/print_value.c` & `xcsf-1.2.9/lib/cJSON/tests/print_value.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/readme_examples.c` & `xcsf-1.2.9/lib/cJSON/tests/readme_examples.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/.gitattributes` & `xcsf-1.2.9/lib/cJSON/tests/unity/.gitattributes`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/.travis.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/.travis.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/README.md` & `xcsf-1.2.9/lib/cJSON/tests/unity/README.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/auto/colour_prompt.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/auto/colour_prompt.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/auto/colour_reporter.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/auto/colour_reporter.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/auto/generate_config.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/auto/generate_config.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/auto/generate_module.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/auto/generate_module.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/auto/generate_test_runner.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/auto/generate_test_runner.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/auto/parse_output.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/auto/parse_output.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/auto/stylize_as_junit.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/auto/stylize_as_junit.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/auto/test_file_filter.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/auto/test_file_filter.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/auto/unity_test_summary.py` & `xcsf-1.2.9/lib/cJSON/tests/unity/auto/unity_test_summary.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/auto/unity_test_summary.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/auto/unity_test_summary.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/auto/unity_to_junit.py` & `xcsf-1.2.9/lib/cJSON/tests/unity/auto/unity_to_junit.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/docs/ThrowTheSwitchCodingStandard.md` & `xcsf-1.2.9/lib/cJSON/tests/unity/docs/ThrowTheSwitchCodingStandard.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/docs/UnityAssertionsCheatSheetSuitableforPrintingandPossiblyFraming.pdf` & `xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityAssertionsCheatSheetSuitableforPrintingandPossiblyFraming.pdf`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/docs/UnityAssertionsReference.md` & `xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityAssertionsReference.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/docs/UnityConfigurationGuide.md` & `xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityConfigurationGuide.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/docs/UnityGettingStartedGuide.md` & `xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityGettingStartedGuide.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/docs/UnityHelperScriptsGuide.md` & `xcsf-1.2.9/lib/cJSON/tests/unity/docs/UnityHelperScriptsGuide.md`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/docs/license.txt` & `xcsf-1.2.9/lib/cJSON/tests/unity/docs/license.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/makefile` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/src/ProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode2.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/TestProductionCode2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode2_Runner.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode2_Runner.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode_Runner.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_1/test/test_runners/TestProductionCode_Runner.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/makefile` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/src/ProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode2.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/TestProductionCode2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode_Runner.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_2/test/test_runners/TestProductionCode_Runner.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/rakefile.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/rakefile.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/rakefile_helper.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/rakefile_helper.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/readme.txt` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/readme.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/src/ProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/target_gcc_32.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/target_gcc_32.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode2.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/example_3/test/TestProductionCode2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/examples/unity_config.h` & `xcsf-1.2.9/lib/cJSON/tests/unity/examples/unity_config.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/eclipse/error_parsers.txt` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/eclipse/error_parsers.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/rakefile.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/rakefile.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/rakefile_helper.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/rakefile_helper.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/readme.txt` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/readme.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.h` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_internals.h` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_internals.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_malloc_overrides.h` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/src/unity_fixture_malloc_overrides.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/Makefile` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/main/AllTests.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/main/AllTests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/template_fixture_tests.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/template_fixture_tests.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_Test.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_Test.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_TestRunner.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_fixture_TestRunner.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.h` & `xcsf-1.2.9/lib/cJSON/tests/unity/extras/fixture/test/unity_output_Spy.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/src/unity.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/src/unity.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/src/unity.h` & `xcsf-1.2.9/lib/cJSON/tests/unity/src/unity.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/src/unity_internals.h` & `xcsf-1.2.9/lib/cJSON/tests/unity/src/unity_internals.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/.rubocop.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/.rubocop.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/Makefile` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_cmd.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_cmd.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_def.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_def.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_head1.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_head1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_cmd.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_cmd.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_def.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_def.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_head1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new1.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new2.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_new2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_param.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_param.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run1.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run2.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_run2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_mock_yaml.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_mock_yaml.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_new1.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_new1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_new2.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_new2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_param.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_param.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_run1.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_run1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_run2.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_run2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/expectdata/testsample_yaml.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/expectdata/testsample_yaml.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/rakefile` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/rakefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/rakefile_helper.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/rakefile_helper.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/spec/generate_module_existing_file_spec.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/spec/generate_module_existing_file_spec.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/clang_file.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/clang_file.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/clang_strict.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/clang_strict.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/gcc_32.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_32.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/gcc_64.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_64.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/gcc_auto_limits.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_auto_limits.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/gcc_auto_stdint.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_auto_stdint.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/gcc_manual_math.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/gcc_manual_math.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/hitech_picc18.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/hitech_picc18.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_arm_v4.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_arm_v4.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_arm_v5.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_arm_v5.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_arm_v5_3.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_arm_v5_3.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_armcortex_LM3S9B92_v5_4.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_armcortex_LM3S9B92_v5_4.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_cortexm3_v5.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_cortexm3_v5.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_msp430.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_msp430.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/targets/iar_sh2a_v6.yml` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/targets/iar_sh2a_v6.yml`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/testdata/testRunnerGenerator.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/testRunnerGenerator.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorSmall.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorSmall.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorWithMocks.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/testdata/testRunnerGeneratorWithMocks.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/tests/test_generate_test_runner.rb` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/test_generate_test_runner.rb`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/tests/testparameterized.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/testparameterized.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/cJSON/tests/unity/test/tests/testunity.c` & `xcsf-1.2.9/lib/cJSON/tests/unity/test/tests/testunity.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/CHANGE-LOG.txt` & `xcsf-1.2.9/lib/dSFMT/CHANGE-LOG.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/FILES.txt` & `xcsf-1.2.9/lib/dSFMT/FILES.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/LICENSE.txt` & `xcsf-1.2.9/lib/dSFMT/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/Makefile` & `xcsf-1.2.9/lib/dSFMT/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/Makefile.me` & `xcsf-1.2.9/lib/dSFMT/Makefile.me`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/README.jp.txt` & `xcsf-1.2.9/lib/dSFMT/README.jp.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/README.txt` & `xcsf-1.2.9/lib/dSFMT/README.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-common.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT-common.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-params.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT-params.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-params11213.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT-params11213.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-params1279.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT-params1279.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-params132049.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT-params132049.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-params19937.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT-params19937.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-params216091.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT-params216091.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-params2203.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT-params2203.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-params4253.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT-params4253.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-params44497.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT-params44497.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-params521.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT-params521.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-params86243.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT-params86243.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-ref.c` & `xcsf-1.2.9/lib/dSFMT/dSFMT-ref.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-src-2.0.tar.gz` & `xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-src-2.0.zip` & `xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.0.zip`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-src-2.1.1.tar.gz` & `xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-src-2.1.1.zip` & `xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.1.zip`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-src-2.1.tar.gz` & `xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT-src-2.1.zip` & `xcsf-1.2.9/lib/dSFMT/dSFMT-src-2.1.zip`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT.11213.out.txt` & `xcsf-1.2.9/lib/dSFMT/dSFMT.11213.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT.1279.out.txt` & `xcsf-1.2.9/lib/dSFMT/dSFMT.1279.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT.132049.out.txt` & `xcsf-1.2.9/lib/dSFMT/dSFMT.132049.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT.19937.out.txt` & `xcsf-1.2.9/lib/dSFMT/dSFMT.19937.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT.216091.out.txt` & `xcsf-1.2.9/lib/dSFMT/dSFMT.216091.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT.2203.out.txt` & `xcsf-1.2.9/lib/dSFMT/dSFMT.2203.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT.4253.out.txt` & `xcsf-1.2.9/lib/dSFMT/dSFMT.4253.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT.44497.out.txt` & `xcsf-1.2.9/lib/dSFMT/dSFMT.44497.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT.521.out.txt` & `xcsf-1.2.9/lib/dSFMT/dSFMT.521.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT.86243.out.txt` & `xcsf-1.2.9/lib/dSFMT/dSFMT.86243.out.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT.c` & `xcsf-1.2.9/lib/dSFMT/dSFMT.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/dSFMT.h` & `xcsf-1.2.9/lib/dSFMT/dSFMT.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/doxygen.cfg` & `xcsf-1.2.9/lib/dSFMT/doxygen.cfg`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/doxygen.cfg.bak` & `xcsf-1.2.9/lib/dSFMT/doxygen.cfg.bak`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/annotated.html` & `xcsf-1.2.9/lib/dSFMT/html/annotated.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/bc_s.png` & `xcsf-1.2.9/lib/dSFMT/html/bc_s.png`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/classes.html` & `xcsf-1.2.9/lib/dSFMT/html/classes.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/d_s_f_m_t_8c.html` & `xcsf-1.2.9/lib/dSFMT/html/d_s_f_m_t_8c.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/d_s_f_m_t_8h.html` & `xcsf-1.2.9/lib/dSFMT/html/d_s_f_m_t_8h.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/d_s_f_m_t_8h_source.html` & `xcsf-1.2.9/lib/dSFMT/html/d_s_f_m_t_8h_source.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/doxygen.css` & `xcsf-1.2.9/lib/dSFMT/html/doxygen.css`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/doxygen.png` & `xcsf-1.2.9/lib/dSFMT/html/doxygen.png`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/files.html` & `xcsf-1.2.9/lib/dSFMT/html/files.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/functions.html` & `xcsf-1.2.9/lib/dSFMT/html/functions.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/functions_vars.html` & `xcsf-1.2.9/lib/dSFMT/html/functions_vars.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/globals.html` & `xcsf-1.2.9/lib/dSFMT/html/globals.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/globals_defs.html` & `xcsf-1.2.9/lib/dSFMT/html/globals_defs.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/globals_func.html` & `xcsf-1.2.9/lib/dSFMT/html/globals_func.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/globals_type.html` & `xcsf-1.2.9/lib/dSFMT/html/globals_type.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/globals_vars.html` & `xcsf-1.2.9/lib/dSFMT/html/globals_vars.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/howto-compile.html` & `xcsf-1.2.9/lib/dSFMT/html/howto-compile.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/index.html` & `xcsf-1.2.9/lib/dSFMT/html/index.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/jquery.js` & `xcsf-1.2.9/lib/dSFMT/html/jquery.js`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/mainpage_8txt.html` & `xcsf-1.2.9/lib/dSFMT/html/mainpage_8txt.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/struct_d_s_f_m_t___t.html` & `xcsf-1.2.9/lib/dSFMT/html/struct_d_s_f_m_t___t.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/tabs.css` & `xcsf-1.2.9/lib/dSFMT/html/tabs.css`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/html/union_w128___t.html` & `xcsf-1.2.9/lib/dSFMT/html/union_w128___t.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/FILES.txt` & `xcsf-1.2.9/lib/dSFMT/jump/FILES.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/LICENSE.txt` & `xcsf-1.2.9/lib/dSFMT/jump/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/Makefile` & `xcsf-1.2.9/lib/dSFMT/jump/Makefile`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/Makefile.me` & `xcsf-1.2.9/lib/dSFMT/jump/Makefile.me`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/calc-characteristic` & `xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/calc-characteristic-mpi` & `xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic-mpi`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/calc-characteristic-mpi.cpp` & `xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic-mpi.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/calc-characteristic-old.cpp` & `xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic-old.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/calc-characteristic.cpp` & `xcsf-1.2.9/lib/dSFMT/jump/calc-characteristic.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/calc-jump` & `xcsf-1.2.9/lib/dSFMT/jump/calc-jump`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/calc-jump.cpp` & `xcsf-1.2.9/lib/dSFMT/jump/calc-jump.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/dSFMT-calc-jump.hpp` & `xcsf-1.2.9/lib/dSFMT/jump/dSFMT-calc-jump.hpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/dSFMT-jump.c` & `xcsf-1.2.9/lib/dSFMT/jump/dSFMT-jump.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/dSFMT-jump.h` & `xcsf-1.2.9/lib/dSFMT/jump/dSFMT-jump.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/dSFMText.hpp` & `xcsf-1.2.9/lib/dSFMT/jump/dSFMText.hpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/debug.fix.11213.txt` & `xcsf-1.2.9/lib/dSFMT/jump/debug.fix.11213.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/debug.txt` & `xcsf-1.2.9/lib/dSFMT/jump/debug.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/degree` & `xcsf-1.2.9/lib/dSFMT/jump/degree`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/degree.cpp` & `xcsf-1.2.9/lib/dSFMT/jump/degree.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/degree.xlsx` & `xcsf-1.2.9/lib/dSFMT/jump/degree.xlsx`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/doxygen.cfg` & `xcsf-1.2.9/lib/dSFMT/jump/doxygen.cfg`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/doxygen.cfg.bak` & `xcsf-1.2.9/lib/dSFMT/jump/doxygen.cfg.bak`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/fac.fix.11213.txt` & `xcsf-1.2.9/lib/dSFMT/jump/fac.fix.11213.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/fac.fix.132049.txt` & `xcsf-1.2.9/lib/dSFMT/jump/fac.fix.132049.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/fac.fix.2203.txt` & `xcsf-1.2.9/lib/dSFMT/jump/fac.fix.2203.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/fac.lcm.132049.txt` & `xcsf-1.2.9/lib/dSFMT/jump/fac.lcm.132049.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/fac.lcm.216091.txt` & `xcsf-1.2.9/lib/dSFMT/jump/fac.lcm.216091.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/fac.lcm.2203.txt` & `xcsf-1.2.9/lib/dSFMT/jump/fac.lcm.2203.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/factorization` & `xcsf-1.2.9/lib/dSFMT/jump/factorization`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/factorization.cpp` & `xcsf-1.2.9/lib/dSFMT/jump/factorization.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/fix.11213.txt` & `xcsf-1.2.9/lib/dSFMT/jump/fix.11213.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/fix.132049.txt` & `xcsf-1.2.9/lib/dSFMT/jump/fix.132049.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/fix.19937.txt` & `xcsf-1.2.9/lib/dSFMT/jump/fix.19937.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/fix.2203.txt` & `xcsf-1.2.9/lib/dSFMT/jump/fix.2203.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/fix.44497.txt` & `xcsf-1.2.9/lib/dSFMT/jump/fix.44497.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/fix.86243.txt` & `xcsf-1.2.9/lib/dSFMT/jump/fix.86243.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/annotated.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/annotated.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/bc_s.png` & `xcsf-1.2.9/lib/dSFMT/jump/html/bc_s.png`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/classes.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/classes.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp_source.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/d_s_f_m_t-calc-jump_8hpp_source.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/d_s_f_m_t-jump_8c.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/d_s_f_m_t-jump_8c.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/doxygen.css` & `xcsf-1.2.9/lib/dSFMT/jump/html/doxygen.css`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/doxygen.png` & `xcsf-1.2.9/lib/dSFMT/jump/html/doxygen.png`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/files.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/files.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/functions.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/functions.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/functions_vars.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/functions_vars.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/globals.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/globals.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/globals_func.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/globals_func.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/globals_vars.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/globals_vars.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/index.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/index.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/jquery.js` & `xcsf-1.2.9/lib/dSFMT/jump/html/jquery.js`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/mainpage_8txt.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/mainpage_8txt.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/namespacedsfmt.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/namespacedsfmt.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/namespacemembers.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/namespacemembers.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/namespacemembers_func.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/namespacemembers_func.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/namespaces.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/namespaces.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/struct_f_i_x___t.html` & `xcsf-1.2.9/lib/dSFMT/jump/html/struct_f_i_x___t.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/html/tabs.css` & `xcsf-1.2.9/lib/dSFMT/jump/html/tabs.css`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/lcm.1279.txt` & `xcsf-1.2.9/lib/dSFMT/jump/lcm.1279.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/lcm.132049.tar.gz` & `xcsf-1.2.9/lib/dSFMT/jump/lcm.132049.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/lcm.216091.tar.gz` & `xcsf-1.2.9/lib/dSFMT/jump/lcm.216091.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/lcm.216091.txt` & `xcsf-1.2.9/lib/dSFMT/jump/lcm.216091.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/lcm.4253.txt` & `xcsf-1.2.9/lib/dSFMT/jump/lcm.4253.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/lcm.86243.tar.gz` & `xcsf-1.2.9/lib/dSFMT/jump/lcm.86243.tar.gz`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/mainpage.txt` & `xcsf-1.2.9/lib/dSFMT/jump/mainpage.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/params.csv` & `xcsf-1.2.9/lib/dSFMT/jump/params.csv`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/poly.11213.txt` & `xcsf-1.2.9/lib/dSFMT/jump/poly.11213.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/poly.132049.txt` & `xcsf-1.2.9/lib/dSFMT/jump/poly.132049.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/poly.19937.txt` & `xcsf-1.2.9/lib/dSFMT/jump/poly.19937.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/poly.216091.txt` & `xcsf-1.2.9/lib/dSFMT/jump/poly.216091.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/poly.2203.txt` & `xcsf-1.2.9/lib/dSFMT/jump/poly.2203.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/poly.4253.txt` & `xcsf-1.2.9/lib/dSFMT/jump/poly.4253.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/poly.44497.txt` & `xcsf-1.2.9/lib/dSFMT/jump/poly.44497.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/poly.86243.txt` & `xcsf-1.2.9/lib/dSFMT/jump/poly.86243.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/readme-jp.html` & `xcsf-1.2.9/lib/dSFMT/jump/readme-jp.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/readme.html` & `xcsf-1.2.9/lib/dSFMT/jump/readme.html`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/sample1` & `xcsf-1.2.9/lib/dSFMT/jump/sample1`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/sample1.c` & `xcsf-1.2.9/lib/dSFMT/jump/sample1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/sample2` & `xcsf-1.2.9/lib/dSFMT/jump/sample2`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/sample2.c` & `xcsf-1.2.9/lib/dSFMT/jump/sample2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/test-jump-M11213` & `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M11213`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/test-jump-M1279` & `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M1279`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/test-jump-M132049` & `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M132049`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/test-jump-M19937` & `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M19937`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/test-jump-M216091` & `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M216091`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/test-jump-M2203` & `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M2203`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/test-jump-M4253` & `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M4253`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/test-jump-M44497` & `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M44497`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/test-jump-M521` & `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M521`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/test-jump-M86243` & `xcsf-1.2.9/lib/dSFMT/jump/test-jump-M86243`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/jump/test-jump.cpp` & `xcsf-1.2.9/lib/dSFMT/jump/test-jump.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/mainpage.txt` & `xcsf-1.2.9/lib/dSFMT/mainpage.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/sample1.c` & `xcsf-1.2.9/lib/dSFMT/sample1.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/sample2.c` & `xcsf-1.2.9/lib/dSFMT/sample2.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/sample3.c` & `xcsf-1.2.9/lib/dSFMT/sample3.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/sample4.c` & `xcsf-1.2.9/lib/dSFMT/sample4.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/dSFMT/test.c` & `xcsf-1.2.9/lib/dSFMT/test.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/doctest/CMakeLists.txt` & `xcsf-1.2.9/lib/doctest/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,22 @@
         COMMENT "assembling the single header")
 
     add_custom_target(assemble_single_header ALL DEPENDS ${CMAKE_CURRENT_SOURCE_DIR}/doctest/doctest.h)
 else()
     target_include_directories(${PROJECT_NAME} INTERFACE $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/>)
 endif()
 
+if(CMAKE_BUILD_TYPE STREQUAL "Debug")
+	if (CMAKE_CXX_COMPILER_ID STREQUAL "Clang")
+		if (NOT WIN32)
+			set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -gdwarf-4 ")
+		endif()
+	endif()
+endif()
+
 # hack to support building on XCode 6 and 7 - propagate the definition to everything
 if(DEFINED DOCTEST_THREAD_LOCAL)
     target_compile_definitions(${PROJECT_NAME} INTERFACE
         DOCTEST_THREAD_LOCAL=${DOCTEST_THREAD_LOCAL})
 endif()
 
 if(DOCTEST_USE_STD_HEADERS)
@@ -132,14 +140,19 @@
         INCLUDES DESTINATION "${include_install_dir}"
     )
 
     install(
         FILES "doctest/doctest.h"
         DESTINATION "${include_install_dir}/doctest"
     )
+    install(
+        DIRECTORY "doctest/extensions"
+        DESTINATION "${include_install_dir}/doctest"
+        FILES_MATCHING PATTERN "*.h"
+    )
 
     install(
         FILES "${project_config}" "${version_config}"
         DESTINATION "${config_install_dir}"
     )
 
     install(
```

### Comparing `xcsf-1.2.8/lib/doctest/examples/all_features/CMakeLists.txt` & `xcsf-1.2.9/lib/doctest/examples/all_features/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt` & `xcsf-1.2.9/lib/doctest/examples/combining_the_same_tests_built_differently_in_multiple_shared_objects/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt` & `xcsf-1.2.9/lib/doctest/examples/exe_with_static_libs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake` & `xcsf-1.2.9/lib/doctest/examples/exe_with_static_libs/doctest_force_link_static_lib_in_target.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt` & `xcsf-1.2.9/lib/doctest/examples/executable_dll_and_plugin/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/doctest/scripts/cmake/assemble_single_header.cmake` & `xcsf-1.2.9/lib/doctest/scripts/cmake/assemble_single_header.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/doctest/scripts/cmake/common.cmake` & `xcsf-1.2.9/lib/doctest/scripts/cmake/common.cmake`

 * *Files 0% similar despite different names*

```diff
@@ -191,14 +191,15 @@
     add_compiler_flags(/permissive-)   # force standard conformance - this is the better flag than /Za
     add_compiler_flags(/WX)
     add_compiler_flags(/Wall) # turns on warnings from levels 1 through 4 which are off by default - https://msdn.microsoft.com/en-us/library/23k5d385.aspx
 
     add_compiler_flags(
         /wd4514 # unreferenced inline function has been removed
         /wd4571 # SEH related
+        /wd5264 # const variable is not used
         /wd4710 # function not inlined
         /wd4711 # function 'x' selected for automatic inline expansion
 
         /wd4616 # invalid compiler warnings - https://msdn.microsoft.com/en-us/library/t7ab6xtd.aspx
         /wd4619 # invalid compiler warnings - https://msdn.microsoft.com/en-us/library/tacee08d.aspx
 
         #/wd4820 # padding in structs
```

### Comparing `xcsf-1.2.8/lib/doctest/scripts/cmake/doctest.cmake` & `xcsf-1.2.9/lib/doctest/scripts/cmake/doctest.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/doctest/scripts/cmake/doctestAddTests.cmake` & `xcsf-1.2.9/lib/doctest/scripts/cmake/doctestAddTests.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/doctest/scripts/cmake/exec_test.cmake` & `xcsf-1.2.9/lib/doctest/scripts/cmake/exec_test.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/CMakeLists.txt` & `xcsf-1.2.9/lib/pybind11/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -87,18 +87,24 @@
   set(pybind11_system SYSTEM)
 endif()
 
 # Options
 option(PYBIND11_INSTALL "Install pybind11 header files?" ${PYBIND11_MASTER_PROJECT})
 option(PYBIND11_TEST "Build pybind11 test suite?" ${PYBIND11_MASTER_PROJECT})
 option(PYBIND11_NOPYTHON "Disable search for Python" OFF)
+option(PYBIND11_SIMPLE_GIL_MANAGEMENT
+       "Use simpler GIL management logic that does not support disassociation" OFF)
 set(PYBIND11_INTERNALS_VERSION
     ""
     CACHE STRING "Override the ABI version, may be used to enable the unstable ABI.")
 
+if(PYBIND11_SIMPLE_GIL_MANAGEMENT)
+  add_compile_definitions(PYBIND11_SIMPLE_GIL_MANAGEMENT)
+endif()
+
 cmake_dependent_option(
   USE_PYTHON_INCLUDE_DIR
   "Install pybind11 headers in Python include directory instead of default installation prefix"
   OFF "PYBIND11_INSTALL" OFF)
 
 cmake_dependent_option(PYBIND11_FINDPYTHON "Force new FindPython" OFF
                        "NOT CMAKE_VERSION VERSION_LESS 3.12" OFF)
@@ -116,14 +122,16 @@
     include/pybind11/buffer_info.h
     include/pybind11/cast.h
     include/pybind11/chrono.h
     include/pybind11/common.h
     include/pybind11/complex.h
     include/pybind11/options.h
     include/pybind11/eigen.h
+    include/pybind11/eigen/matrix.h
+    include/pybind11/eigen/tensor.h
     include/pybind11/embed.h
     include/pybind11/eval.h
     include/pybind11/gil.h
     include/pybind11/iostream.h
     include/pybind11/functional.h
     include/pybind11/numpy.h
     include/pybind11/operators.h
@@ -194,14 +202,17 @@
   endif()
 else()
   # It is invalid to install a target twice, too.
   set(PYBIND11_INSTALL OFF)
 endif()
 
 include("${CMAKE_CURRENT_SOURCE_DIR}/tools/pybind11Common.cmake")
+# https://github.com/jtojnar/cmake-snips/#concatenating-paths-when-building-pkg-config-files
+# TODO: cmake 3.20 adds the cmake_path() function, which obsoletes this snippet
+include("${CMAKE_CURRENT_SOURCE_DIR}/tools/JoinPaths.cmake")
 
 # Relative directory setting
 if(USE_PYTHON_INCLUDE_DIR AND DEFINED Python_INCLUDE_DIRS)
   file(RELATIVE_PATH CMAKE_INSTALL_INCLUDEDIR ${CMAKE_INSTALL_PREFIX} ${Python_INCLUDE_DIRS})
 elseif(USE_PYTHON_INCLUDE_DIR AND DEFINED PYTHON_INCLUDE_DIR)
   file(RELATIVE_PATH CMAKE_INSTALL_INCLUDEDIR ${CMAKE_INSTALL_PREFIX} ${PYTHON_INCLUDE_DIRS})
 endif()
@@ -258,14 +269,24 @@
   install(TARGETS pybind11_headers EXPORT "${PYBIND11_EXPORT_NAME}")
 
   install(
     EXPORT "${PYBIND11_EXPORT_NAME}"
     NAMESPACE "pybind11::"
     DESTINATION ${PYBIND11_CMAKECONFIG_INSTALL_DIR})
 
+  # pkg-config support
+  if(NOT prefix_for_pc_file)
+    set(prefix_for_pc_file "${CMAKE_INSTALL_PREFIX}")
+  endif()
+  join_paths(includedir_for_pc_file "\${prefix}" "${CMAKE_INSTALL_INCLUDEDIR}")
+  configure_file("${CMAKE_CURRENT_SOURCE_DIR}/tools/pybind11.pc.in"
+                 "${CMAKE_CURRENT_BINARY_DIR}/pybind11.pc" @ONLY)
+  install(FILES "${CMAKE_CURRENT_BINARY_DIR}/pybind11.pc"
+          DESTINATION "${CMAKE_INSTALL_DATAROOTDIR}/pkgconfig/")
+
   # Uninstall target
   if(PYBIND11_MASTER_PROJECT)
     configure_file("${CMAKE_CURRENT_SOURCE_DIR}/tools/cmake_uninstall.cmake.in"
                    "${CMAKE_CURRENT_BINARY_DIR}/cmake_uninstall.cmake" IMMEDIATE @ONLY)
 
     add_custom_target(uninstall COMMAND ${CMAKE_COMMAND} -P
                                         ${CMAKE_CURRENT_BINARY_DIR}/cmake_uninstall.cmake)
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/attr.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/attr.h`

 * *Files 1% similar despite different names*

```diff
@@ -395,15 +395,15 @@
     static void init(const doc &n, function_record *r) { r->doc = const_cast<char *>(n.value); }
 };
 
 /// Process an attribute specifying the function's docstring (provided as a C-style string)
 template <>
 struct process_attribute<const char *> : process_attribute_default<const char *> {
     static void init(const char *d, function_record *r) { r->doc = const_cast<char *>(d); }
-    static void init(const char *d, type_record *r) { r->doc = const_cast<char *>(d); }
+    static void init(const char *d, type_record *r) { r->doc = d; }
 };
 template <>
 struct process_attribute<char *> : process_attribute<const char *> {};
 
 /// Process an attribute indicating the function's return value policy
 template <>
 struct process_attribute<return_value_policy> : process_attribute_default<return_value_policy> {
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/buffer_info.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/cast.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/cast.h`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 #include <string>
 #include <tuple>
 #include <type_traits>
 #include <utility>
 #include <vector>
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
+
+PYBIND11_WARNING_DISABLE_MSVC(4127)
+
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <typename type, typename SFINAE = void>
 class type_caster : public type_caster_base<type> {};
 template <typename type>
 using make_caster = type_caster<intrinsic_t<type>>;
 
@@ -84,15 +87,16 @@
     type value;                                                                                   \
                                                                                                   \
 public:                                                                                           \
     static constexpr auto name = py_name;                                                         \
     template <typename T_,                                                                        \
               ::pybind11::detail::enable_if_t<                                                    \
                   std::is_same<type, ::pybind11::detail::remove_cv_t<T_>>::value,                 \
-                  int> = 0>                                                                       \
+                  int>                                                                            \
+              = 0>                                                                                \
     static ::pybind11::handle cast(                                                               \
         T_ *src, ::pybind11::return_value_policy policy, ::pybind11::handle parent) {             \
         if (!src)                                                                                 \
             return ::pybind11::none().release();                                                  \
         if (policy == ::pybind11::return_value_policy::take_ownership) {                          \
             auto h = cast(std::move(*src), policy, parent);                                       \
             delete src;                                                                           \
@@ -244,15 +248,15 @@
     bool load(handle src, bool) {
         if (src && src.is_none()) {
             return true;
         }
         return false;
     }
     static handle cast(T, return_value_policy /* policy */, handle /* parent */) {
-        return none().inc_ref();
+        return none().release();
     }
     PYBIND11_TYPE_CASTER(T, const_name("None"));
 };
 
 template <>
 class type_caster<void_type> : public void_caster<void_type> {};
 
@@ -287,15 +291,15 @@
         return false;
     }
 
     static handle cast(const void *ptr, return_value_policy /* policy */, handle /* parent */) {
         if (ptr) {
             return capsule(ptr).release();
         }
-        return none().inc_ref();
+        return none().release();
     }
 
     template <typename T>
     using cast_op_type = void *&;
     explicit operator void *&() { return value; }
     static constexpr auto name = const_name("capsule");
 
@@ -385,15 +389,15 @@
         }
         if (!PyUnicode_Check(load_src.ptr())) {
             return load_raw(load_src);
         }
 
         // For UTF-8 we avoid the need for a temporary `bytes` object by using
         // `PyUnicode_AsUTF8AndSize`.
-        if (PYBIND11_SILENCE_MSVC_C4127(UTF_N == 8)) {
+        if (UTF_N == 8) {
             Py_ssize_t size = -1;
             const auto *buffer
                 = reinterpret_cast<const CharT *>(PyUnicode_AsUTF8AndSize(load_src.ptr(), &size));
             if (!buffer) {
                 PyErr_Clear();
                 return false;
             }
@@ -412,15 +416,15 @@
             return false;
         }
 
         const auto *buffer
             = reinterpret_cast<const CharT *>(PYBIND11_BYTES_AS_STRING(utfNbytes.ptr()));
         size_t length = (size_t) PYBIND11_BYTES_SIZE(utfNbytes.ptr()) / sizeof(CharT);
         // Skip BOM for UTF-16/32
-        if (PYBIND11_SILENCE_MSVC_C4127(UTF_N > 8)) {
+        if (UTF_N > 8) {
             buffer++;
             length--;
         }
         value = StringType(buffer, length);
 
         // If we're loading a string_view we need to keep the encoded Python object alive:
         if (IsView) {
@@ -533,15 +537,15 @@
             return true;
         }
         return str_caster.load(src, convert);
     }
 
     static handle cast(const CharT *src, return_value_policy policy, handle parent) {
         if (src == nullptr) {
-            return pybind11::none().inc_ref();
+            return pybind11::none().release();
         }
         return StringCaster::cast(StringType(src), policy, parent);
     }
 
     static handle cast(CharT src, return_value_policy policy, handle parent) {
         if (std::is_same<char, CharT>::value) {
             handle s = PyUnicode_DecodeLatin1((const char *) &src, 1, nullptr);
@@ -568,15 +572,15 @@
         }
 
         // If we're in UTF-8 mode, we have two possible failures: one for a unicode character that
         // is too high, and one for multiple unicode characters (caught later), so we need to
         // figure out how long the first encoded character is in bytes to distinguish between these
         // two errors.  We also allow want to allow unicode characters U+0080 through U+00FF, as
         // those can fit into a single char value.
-        if (PYBIND11_SILENCE_MSVC_C4127(StringCaster::UTF_N == 8) && str_len > 1 && str_len <= 4) {
+        if (StringCaster::UTF_N == 8 && str_len > 1 && str_len <= 4) {
             auto v0 = static_cast<unsigned char>(value[0]);
             // low bits only: 0-127
             // 0b110xxxxx - start of 2-byte sequence
             // 0b1110xxxx - start of 3-byte sequence
             // 0b11110xxx - start of 4-byte sequence
             size_t char0_bytes = (v0 & 0x80) == 0      ? 1
                                  : (v0 & 0xE0) == 0xC0 ? 2
@@ -594,15 +598,15 @@
                 throw value_error("Character code point not in range(0x100)");
             }
         }
 
         // UTF-16 is much easier: we can only have a surrogate pair for values above U+FFFF, thus a
         // surrogate pair with total length 2 instantly indicates a range error (but not a "your
         // string was too long" error).
-        else if (PYBIND11_SILENCE_MSVC_C4127(StringCaster::UTF_N == 16) && str_len == 2) {
+        else if (StringCaster::UTF_N == 16 && str_len == 2) {
             one_char = static_cast<CharT>(value[0]);
             if (one_char >= 0xD800 && one_char < 0xE000) {
                 throw value_error("Character code point not in range(0x10000)");
             }
         }
 
         if (str_len != 1) {
@@ -1175,19 +1179,17 @@
 // static_assert, even though if it's in dead code, so we provide a "trampoline" to pybind11::cast
 // that only does anything in cases where pybind11::cast is valid.
 template <typename T>
 enable_if_t<cast_is_temporary_value_reference<T>::value, T> cast_safe(object &&) {
     pybind11_fail("Internal error: cast_safe fallback invoked");
 }
 template <typename T>
-enable_if_t<std::is_same<void, intrinsic_t<T>>::value, void> cast_safe(object &&) {}
+enable_if_t<std::is_void<T>::value, void> cast_safe(object &&) {}
 template <typename T>
-enable_if_t<detail::none_of<cast_is_temporary_value_reference<T>,
-                            std::is_same<void, intrinsic_t<T>>>::value,
-            T>
+enable_if_t<detail::none_of<cast_is_temporary_value_reference<T>, std::is_void<T>>::value, T>
 cast_safe(object &&o) {
     return pybind11::cast<T>(std::move(o));
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 // The overloads could coexist, i.e. the #if is not strictly speaking needed,
@@ -1541,15 +1543,15 @@
         if (!a.value) {
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES)
             throw cast_error_unable_to_convert_call_arg();
 #else
             throw cast_error_unable_to_convert_call_arg(a.name, a.type);
 #endif
         }
-        m_kwargs[a.name] = a.value;
+        m_kwargs[a.name] = std::move(a.value);
     }
 
     void process(list & /*args_list*/, detail::kwargs_proxy kp) {
         if (!kp) {
             return;
         }
         for (auto k : reinterpret_borrow<dict>(kp)) {
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/chrono.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/complex.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/detail/class.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/class.h`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,17 @@
 
 /// `pybind11_static_property.__set__()`: Just like the above `__get__()`.
 extern "C" inline int pybind11_static_set(PyObject *self, PyObject *obj, PyObject *value) {
     PyObject *cls = PyType_Check(obj) ? obj : (PyObject *) Py_TYPE(obj);
     return PyProperty_Type.tp_descr_set(self, cls, value);
 }
 
+// Forward declaration to use in `make_static_property_type()`
+inline void enable_dynamic_attributes(PyHeapTypeObject *heap_type);
+
 /** A `static_property` is the same as a `property` but the `__get__()` and `__set__()`
     methods are modified to always use the object type instead of a concrete instance.
     Return value: New reference. */
 inline PyTypeObject *make_static_property_type() {
     constexpr auto *name = "pybind11_static_property";
     auto name_obj = reinterpret_steal<object>(PYBIND11_FROM_STRING(name));
 
@@ -83,14 +86,21 @@
     type->tp_descr_get = pybind11_static_get;
     type->tp_descr_set = pybind11_static_set;
 
     if (PyType_Ready(type) < 0) {
         pybind11_fail("make_static_property_type(): failure in PyType_Ready()!");
     }
 
+#    if PY_VERSION_HEX >= 0x030C0000
+    // PRE 3.12 FEATURE FREEZE. PLEASE REVIEW AFTER FREEZE.
+    // Since Python-3.12 property-derived types are required to
+    // have dynamic attributes (to set `__doc__`)
+    enable_dynamic_attributes(heap_type);
+#    endif
+
     setattr((PyObject *) type, "__module__", str("pybind11_builtins"));
     PYBIND11_SET_OLDPY_QUALNAME(type, name_obj);
 
     return type;
 }
 
 #else // PYPY
@@ -431,17 +441,25 @@
         clear_patients(self);
     }
 }
 
 /// Instance destructor function for all pybind11 types. It calls `type_info.dealloc`
 /// to destroy the C++ object itself, while the rest is Python bookkeeping.
 extern "C" inline void pybind11_object_dealloc(PyObject *self) {
+    auto *type = Py_TYPE(self);
+
+    // If this is a GC tracked object, untrack it first
+    // Note that the track call is implicitly done by the
+    // default tp_alloc, which we never override.
+    if (PyType_HasFeature(type, Py_TPFLAGS_HAVE_GC) != 0) {
+        PyObject_GC_UnTrack(self);
+    }
+
     clear_instance(self);
 
-    auto *type = Py_TYPE(self);
     type->tp_free(self);
 
 #if PY_VERSION_HEX < 0x03080000
     // `type->tp_dealloc != pybind11_object_dealloc` means that we're being called
     // as part of a derived type's dealloc, in which case we're not allowed to decref
     // the type here. For cross-module compatibility, we shouldn't compare directly
     // with `pybind11_object_dealloc`, but with the common one stashed in internals.
@@ -498,39 +516,14 @@
     setattr((PyObject *) type, "__module__", str("pybind11_builtins"));
     PYBIND11_SET_OLDPY_QUALNAME(type, name_obj);
 
     assert(!PyType_HasFeature(type, Py_TPFLAGS_HAVE_GC));
     return (PyObject *) heap_type;
 }
 
-/// dynamic_attr: Support for `d = instance.__dict__`.
-extern "C" inline PyObject *pybind11_get_dict(PyObject *self, void *) {
-    PyObject *&dict = *_PyObject_GetDictPtr(self);
-    if (!dict) {
-        dict = PyDict_New();
-    }
-    Py_XINCREF(dict);
-    return dict;
-}
-
-/// dynamic_attr: Support for `instance.__dict__ = dict()`.
-extern "C" inline int pybind11_set_dict(PyObject *self, PyObject *new_dict, void *) {
-    if (!PyDict_Check(new_dict)) {
-        PyErr_Format(PyExc_TypeError,
-                     "__dict__ must be set to a dictionary, not a '%.200s'",
-                     get_fully_qualified_tp_name(Py_TYPE(new_dict)).c_str());
-        return -1;
-    }
-    PyObject *&dict = *_PyObject_GetDictPtr(self);
-    Py_INCREF(new_dict);
-    Py_CLEAR(dict);
-    dict = new_dict;
-    return 0;
-}
-
 /// dynamic_attr: Allow the garbage collector to traverse the internal instance `__dict__`.
 extern "C" inline int pybind11_traverse(PyObject *self, visitproc visit, void *arg) {
     PyObject *&dict = *_PyObject_GetDictPtr(self);
     Py_VISIT(dict);
 // https://docs.python.org/3/c-api/typeobj.html#c.PyTypeObject.tp_traverse
 #if PY_VERSION_HEX >= 0x03090000
     Py_VISIT(Py_TYPE(self));
@@ -554,17 +547,25 @@
     type->tp_basicsize += (ssize_t) sizeof(PyObject *); // and allocate enough space for it
 #else
     type->tp_flags |= Py_TPFLAGS_MANAGED_DICT;
 #endif
     type->tp_traverse = pybind11_traverse;
     type->tp_clear = pybind11_clear;
 
-    static PyGetSetDef getset[] = {
-        {const_cast<char *>("__dict__"), pybind11_get_dict, pybind11_set_dict, nullptr, nullptr},
-        {nullptr, nullptr, nullptr, nullptr, nullptr}};
+    static PyGetSetDef getset[] = {{
+#if PY_VERSION_HEX < 0x03070000
+                                       const_cast<char *>("__dict__"),
+#else
+                                       "__dict__",
+#endif
+                                       PyObject_GenericGetDict,
+                                       PyObject_GenericSetDict,
+                                       nullptr,
+                                       nullptr},
+                                   {nullptr, nullptr, nullptr, nullptr, nullptr}};
     type->tp_getset = getset;
 }
 
 /// buffer_protocol: Fill in the view as specified by flags.
 extern "C" inline int pybind11_getbuffer(PyObject *obj, Py_buffer *view, int flags) {
     // Look for a `get_buffer` implementation in this type's info or any bases (following MRO).
     type_info *tinfo = nullptr;
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/detail/common.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/common.h`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,83 @@
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #define PYBIND11_VERSION_MAJOR 2
 #define PYBIND11_VERSION_MINOR 10
-#define PYBIND11_VERSION_PATCH 0
+#define PYBIND11_VERSION_PATCH 4
 
 // Similar to Python's convention: https://docs.python.org/3/c-api/apiabiversion.html
 // Additional convention: 0xD = dev
-#define PYBIND11_VERSION_HEX 0x020A0000
+#define PYBIND11_VERSION_HEX 0x020A0400
 
-#define PYBIND11_NAMESPACE_BEGIN(name) namespace name {
-#define PYBIND11_NAMESPACE_END(name) }
+// Define some generic pybind11 helper macros for warning management.
+//
+// Note that compiler-specific push/pop pairs are baked into the
+// PYBIND11_NAMESPACE_BEGIN/PYBIND11_NAMESPACE_END pair of macros. Therefore manual
+// PYBIND11_WARNING_PUSH/PYBIND11_WARNING_POP are usually only needed in `#include` sections.
+//
+// If you find you need to suppress a warning, please try to make the suppression as local as
+// possible using these macros. Please also be sure to push/pop with the pybind11 macros. Please
+// only use compiler specifics if you need to check specific versions, e.g. Apple Clang vs. vanilla
+// Clang.
+#if defined(_MSC_VER)
+#    define PYBIND11_COMPILER_MSVC
+#    define PYBIND11_PRAGMA(...) __pragma(__VA_ARGS__)
+#    define PYBIND11_WARNING_PUSH PYBIND11_PRAGMA(warning(push))
+#    define PYBIND11_WARNING_POP PYBIND11_PRAGMA(warning(pop))
+#elif defined(__INTEL_COMPILER)
+#    define PYBIND11_COMPILER_INTEL
+#    define PYBIND11_PRAGMA(...) _Pragma(#__VA_ARGS__)
+#    define PYBIND11_WARNING_PUSH PYBIND11_PRAGMA(warning push)
+#    define PYBIND11_WARNING_POP PYBIND11_PRAGMA(warning pop)
+#elif defined(__clang__)
+#    define PYBIND11_COMPILER_CLANG
+#    define PYBIND11_PRAGMA(...) _Pragma(#__VA_ARGS__)
+#    define PYBIND11_WARNING_PUSH PYBIND11_PRAGMA(clang diagnostic push)
+#    define PYBIND11_WARNING_POP PYBIND11_PRAGMA(clang diagnostic push)
+#elif defined(__GNUC__)
+#    define PYBIND11_COMPILER_GCC
+#    define PYBIND11_PRAGMA(...) _Pragma(#__VA_ARGS__)
+#    define PYBIND11_WARNING_PUSH PYBIND11_PRAGMA(GCC diagnostic push)
+#    define PYBIND11_WARNING_POP PYBIND11_PRAGMA(GCC diagnostic pop)
+#endif
+
+#ifdef PYBIND11_COMPILER_MSVC
+#    define PYBIND11_WARNING_DISABLE_MSVC(name) PYBIND11_PRAGMA(warning(disable : name))
+#else
+#    define PYBIND11_WARNING_DISABLE_MSVC(name)
+#endif
+
+#ifdef PYBIND11_COMPILER_CLANG
+#    define PYBIND11_WARNING_DISABLE_CLANG(name) PYBIND11_PRAGMA(clang diagnostic ignored name)
+#else
+#    define PYBIND11_WARNING_DISABLE_CLANG(name)
+#endif
+
+#ifdef PYBIND11_COMPILER_GCC
+#    define PYBIND11_WARNING_DISABLE_GCC(name) PYBIND11_PRAGMA(GCC diagnostic ignored name)
+#else
+#    define PYBIND11_WARNING_DISABLE_GCC(name)
+#endif
+
+#ifdef PYBIND11_COMPILER_INTEL
+#    define PYBIND11_WARNING_DISABLE_INTEL(name) PYBIND11_PRAGMA(warning disable name)
+#else
+#    define PYBIND11_WARNING_DISABLE_INTEL(name)
+#endif
+
+#define PYBIND11_NAMESPACE_BEGIN(name)                                                            \
+    namespace name {                                                                              \
+    PYBIND11_WARNING_PUSH
+
+#define PYBIND11_NAMESPACE_END(name)                                                              \
+    PYBIND11_WARNING_POP                                                                          \
+    }
 
 // Robust support for some features and loading modules compiled against different pybind versions
 // requires forcing hidden visibility on pybind code, so we enforce this by setting the attribute
 // on the main `pybind11` namespace.
 #if !defined(PYBIND11_NAMESPACE)
 #    ifdef __GNUG__
 #        define PYBIND11_NAMESPACE pybind11 __attribute__((visibility("hidden")))
@@ -92,21 +153,18 @@
 #        define PYBIND11_EXPORT __declspec(dllexport)
 #    else
 #        define PYBIND11_EXPORT __attribute__((visibility("default")))
 #    endif
 #endif
 
 #if !defined(PYBIND11_EXPORT_EXCEPTION)
-#    ifdef __MINGW32__
-// workaround for:
-// error: 'dllexport' implies default visibility, but xxx has already been declared with a
-// different visibility
-#        define PYBIND11_EXPORT_EXCEPTION
-#    else
+#    if defined(__apple_build_version__)
 #        define PYBIND11_EXPORT_EXCEPTION PYBIND11_EXPORT
+#    else
+#        define PYBIND11_EXPORT_EXCEPTION
 #    endif
 #endif
 
 // For CUDA, GCC7, GCC8:
 // PYBIND11_NOINLINE_FORCED is incompatible with `-Wattributes -Werror`.
 // When defining PYBIND11_NOINLINE_FORCED, it is best to also use `-Wno-attributes`.
 // However, the measured shared-library size saving when using noinline are only
@@ -150,17 +208,17 @@
    properly in Visual Studio since 2015. */
 #if defined(_MSC_VER)
 #    define HAVE_SNPRINTF 1
 #endif
 
 /// Include Python header, disable linking to pythonX_d.lib on Windows in debug mode
 #if defined(_MSC_VER)
-#    pragma warning(push)
+PYBIND11_WARNING_PUSH
+PYBIND11_WARNING_DISABLE_MSVC(4505)
 // C4505: 'PySlice_GetIndicesEx': unreferenced local function has been removed (PyPy only)
-#    pragma warning(disable : 4505)
 #    if defined(_DEBUG) && !defined(Py_DEBUG)
 // Workaround for a VS 2022 issue.
 // NOTE: This workaround knowingly violates the Python.h include order requirement:
 // https://docs.python.org/3/c-api/intro.html#include-files
 // See https://github.com/pybind/pybind11/pull/3497 for full context.
 #        include <yvals.h>
 #        if _MSVC_STL_VERSION >= 143
@@ -201,19 +259,16 @@
 #            define PYBIND11_HAS_STRING_VIEW
 #        endif
 #    elif defined(_MSC_VER)
 #        define PYBIND11_HAS_STRING_VIEW
 #    endif
 #endif
 
-#if defined(__cpp_lib_char8_t) && __cpp_lib_char8_t >= 201811L
-#    define PYBIND11_HAS_U8STRING
-#endif
-
 #include <Python.h>
+// Reminder: WITH_THREAD is always defined if PY_VERSION_HEX >= 0x03070000
 #if PY_VERSION_HEX < 0x03060000
 #    error "PYTHON < 3.6 IS UNSUPPORTED. pybind11 v2.9 was the last to support Python 2 and 3.5."
 #endif
 #include <frameobject.h>
 #include <pythread.h>
 
 /* Python #defines overrides on all sorts of core functions, which
@@ -229,20 +284,24 @@
 #    undef toupper
 #endif
 
 #if defined(copysign)
 #    undef copysign
 #endif
 
+#if defined(PYPY_VERSION) && !defined(PYBIND11_SIMPLE_GIL_MANAGEMENT)
+#    define PYBIND11_SIMPLE_GIL_MANAGEMENT
+#endif
+
 #if defined(_MSC_VER)
 #    if defined(PYBIND11_DEBUG_MARKER)
 #        define _DEBUG
 #        undef PYBIND11_DEBUG_MARKER
 #    endif
-#    pragma warning(pop)
+PYBIND11_WARNING_POP
 #endif
 
 #include <cstddef>
 #include <cstring>
 #include <exception>
 #include <forward_list>
 #include <memory>
@@ -255,14 +314,29 @@
 #include <vector>
 #if defined(__has_include)
 #    if __has_include(<version>)
 #        include <version>
 #    endif
 #endif
 
+// Must be after including <version> or one of the other headers specified by the standard
+#if defined(__cpp_lib_char8_t) && __cpp_lib_char8_t >= 201811L
+#    define PYBIND11_HAS_U8STRING
+#endif
+
+// See description of PR #4246:
+#if !defined(NDEBUG) && !defined(PY_ASSERT_GIL_HELD_INCREF_DECREF)                                \
+    && !(defined(PYPY_VERSION)                                                                    \
+         && defined(_MSC_VER)) /* PyPy Windows: pytest hangs indefinitely at the end of the       \
+                                  process (see PR #4268) */                                       \
+    && !defined(PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF)
+// The following define will be enabled by default in the 2.11 release
+// define PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
+#endif
+
 // #define PYBIND11_STR_LEGACY_PERMISSIVE
 // If DEFINED, pybind11::str can hold PyUnicodeObject or PyBytesObject
 //             (probably surprising and never documented, but this was the
 //             legacy behavior until and including v2.6.x). As a side-effect,
 //             pybind11::isinstance<str>() is true for both pybind11::str and
 //             pybind11::bytes.
 // If UNDEFINED, pybind11::str can only hold PyUnicodeObject, and
@@ -359,15 +433,15 @@
         }                                                                                         \
         PYBIND11_CATCH_INIT_EXCEPTIONS                                                            \
     }                                                                                             \
     PyObject *pybind11_init()
 
 /** \rst
     This macro creates the entry point that will be invoked when the Python interpreter
-    imports an extension module. The module name is given as the fist argument and it
+    imports an extension module. The module name is given as the first argument and it
     should not be in quotes. The second macro argument defines a variable of type
     `py::module_` which can be used to initialize the module.
 
     The entry point is marked as "maybe unused" to aid dead-code detection analysis:
     since the entry point is typically only looked up at runtime and not referenced
     during translation, it would otherwise appear as unused ("dead") code.
 
@@ -894,30 +968,21 @@
 using expand_side_effects = bool[];
 #    define PYBIND11_EXPAND_SIDE_EFFECTS(PATTERN)                                                 \
         (void) pybind11::detail::expand_side_effects { ((PATTERN), void(), false)..., false }
 #endif
 
 PYBIND11_NAMESPACE_END(detail)
 
-#if defined(_MSC_VER)
-#    pragma warning(push)
-#    pragma warning(disable : 4275)
-//     warning C4275: An exported class was derived from a class that wasn't exported.
-//     Can be ignored when derived from a STL class.
-#endif
 /// C++ bindings of builtin Python exceptions
 class PYBIND11_EXPORT_EXCEPTION builtin_exception : public std::runtime_error {
 public:
     using std::runtime_error::runtime_error;
     /// Set the error using the Python C API
     virtual void set_error() const = 0;
 };
-#if defined(_MSC_VER)
-#    pragma warning(pop)
-#endif
 
 #define PYBIND11_RUNTIME_EXCEPTION(name, type)                                                    \
     class PYBIND11_EXPORT_EXCEPTION name : public builtin_exception {                             \
     public:                                                                                       \
         using builtin_exception::builtin_exception;                                               \
         name() : name("") {}                                                                      \
         void set_error() const override { PyErr_SetString(type, what()); }                        \
@@ -1029,20 +1094,15 @@
 // overload_cast requires variable templates: C++14
 #if defined(PYBIND11_CPP14)
 #    define PYBIND11_OVERLOAD_CAST 1
 /// Syntax sugar for resolving overloaded function pointers:
 ///  - regular: static_cast<Return (Class::*)(Arg0, Arg1, Arg2)>(&Class::func)
 ///  - sweet:   overload_cast<Arg0, Arg1, Arg2>(&Class::func)
 template <typename... Args>
-#    if (defined(_MSC_VER) && _MSC_VER < 1920) /* MSVC 2017 */                                    \
-        || (defined(__clang__) && __clang_major__ == 5)
-static constexpr detail::overload_cast_impl<Args...> overload_cast = {};
-#    else
-static constexpr detail::overload_cast_impl<Args...> overload_cast;
-#    endif
+static constexpr detail::overload_cast_impl<Args...> overload_cast{};
 #endif
 
 /// Const member function selector for overload_cast
 ///  - regular: static_cast<Return (Class::*)(Arg) const>(&Class::func)
 ///  - sweet:   overload_cast<Arg>(&Class::func, const_)
 static constexpr auto const_ = std::true_type{};
 
@@ -1143,23 +1203,30 @@
 #if defined(__GNUG__) && !defined(__clang__) && !defined(__INTEL_COMPILER)
 #    define PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(...)                       \
         detail::silence_unused_warnings(__VA_ARGS__)
 #else
 #    define PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(...)
 #endif
 
-#if defined(_MSC_VER) // All versions (as of July 2021).
-
-// warning C4127: Conditional expression is constant
-constexpr inline bool silence_msvc_c4127(bool cond) { return cond; }
-
-#    define PYBIND11_SILENCE_MSVC_C4127(...) ::pybind11::detail::silence_msvc_c4127(__VA_ARGS__)
-
-#else
-#    define PYBIND11_SILENCE_MSVC_C4127(...) __VA_ARGS__
+#if defined(__clang__)                                                                            \
+    && (defined(__apple_build_version__) /* AppleClang 13.0.0.13000029 was the only data point    \
+                                            available. */                                         \
+        || (__clang_major__ >= 7                                                                  \
+            && __clang_major__ <= 12) /* Clang 3, 5, 13, 14, 15 do not generate the warning. */   \
+    )
+#    define PYBIND11_DETECTED_CLANG_WITH_MISLEADING_CALL_STD_MOVE_EXPLICITLY_WARNING
+// Example:
+// tests/test_kwargs_and_defaults.cpp:46:68: error: local variable 'args' will be copied despite
+// being returned by name [-Werror,-Wreturn-std-move]
+//     m.def("args_function", [](py::args args) -> py::tuple { return args; });
+//                                                                    ^~~~
+// test_kwargs_and_defaults.cpp:46:68: note: call 'std::move' explicitly to avoid copying
+//     m.def("args_function", [](py::args args) -> py::tuple { return args; });
+//                                                                    ^~~~
+//                                                                    std::move(args)
 #endif
 
 // Pybind offers detailed error messages by default for all builts that are debug (through the
 // negation of ndebug). This can also be manually enabled by users, for any builds, through
 // defining PYBIND11_DETAILED_ERROR_MESSAGES.
 #if !defined(PYBIND11_DETAILED_ERROR_MESSAGES) && !defined(NDEBUG)
 #    define PYBIND11_DETAILED_ERROR_MESSAGES
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/detail/descr.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/detail/init.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/init.h`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 */
 
 #pragma once
 
 #include "class.h"
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
+
+PYBIND11_WARNING_DISABLE_MSVC(4127)
+
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <>
 class type_caster<value_and_holder> {
 public:
     bool load(handle h, bool) {
         value = reinterpret_cast<value_and_holder *>(h.ptr());
@@ -111,15 +114,15 @@
 // If we don't need an alias (because this class doesn't have one, or because the final type is
 // inherited on the Python side) we can simply take over ownership.  Otherwise we need to try to
 // construct an Alias from the returned base instance.
 template <typename Class>
 void construct(value_and_holder &v_h, Cpp<Class> *ptr, bool need_alias) {
     PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
     no_nullptr(ptr);
-    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias && !is_alias<Class>(ptr)) {
+    if (Class::has_alias && need_alias && !is_alias<Class>(ptr)) {
         // We're going to try to construct an alias by moving the cpp type.  Whether or not
         // that succeeds, we still need to destroy the original cpp pointer (either the
         // moved away leftover, if the alias construction works, or the value itself if we
         // throw an error), but we can't just call `delete ptr`: it might have a special
         // deleter, or might be shared_from_this.  So we construct a holder around it as if
         // it was a normal instance, then steal the holder away into a local variable; thus
         // the holder and destruction happens when we leave the C++ scope, and the holder
@@ -152,15 +155,15 @@
 // constructors).
 template <typename Class>
 void construct(value_and_holder &v_h, Holder<Class> holder, bool need_alias) {
     PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
     auto *ptr = holder_helper<Holder<Class>>::get(holder);
     no_nullptr(ptr);
     // If we need an alias, check that the held pointer is actually an alias instance
-    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias && !is_alias<Class>(ptr)) {
+    if (Class::has_alias && need_alias && !is_alias<Class>(ptr)) {
         throw type_error("pybind11::init(): construction failed: returned holder-wrapped instance "
                          "is not an alias instance");
     }
 
     v_h.value_ptr() = ptr;
     v_h.type->init_instance(v_h.inst, &holder);
 }
@@ -170,15 +173,15 @@
 // the alias from the base when needed (i.e. because of Python-side inheritance).  When we don't
 // need it, we simply move-construct the cpp value into a new instance.
 template <typename Class>
 void construct(value_and_holder &v_h, Cpp<Class> &&result, bool need_alias) {
     PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
     static_assert(std::is_move_constructible<Cpp<Class>>::value,
                   "pybind11::init() return-by-value factory function requires a movable class");
-    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias) {
+    if (Class::has_alias && need_alias) {
         construct_alias_from_cpp<Class>(is_alias_constructible<Class>{}, v_h, std::move(result));
     } else {
         v_h.value_ptr() = new Cpp<Class>(std::move(result));
     }
 }
 
 // return-by-value version 2: returning a value of the alias type itself.  We move-construct an
@@ -202,18 +205,19 @@
             [](value_and_holder &v_h, Args... args) {
                 v_h.value_ptr() = construct_or_initialize<Cpp<Class>>(std::forward<Args>(args)...);
             },
             is_new_style_constructor(),
             extra...);
     }
 
-    template <typename Class,
-              typename... Extra,
-              enable_if_t<Class::has_alias && std::is_constructible<Cpp<Class>, Args...>::value,
-                          int> = 0>
+    template <
+        typename Class,
+        typename... Extra,
+        enable_if_t<Class::has_alias && std::is_constructible<Cpp<Class>, Args...>::value, int>
+        = 0>
     static void execute(Class &cl, const Extra &...extra) {
         cl.def(
             "__init__",
             [](value_and_holder &v_h, Args... args) {
                 if (Py_TYPE(v_h.inst) == v_h.type->type) {
                     v_h.value_ptr()
                         = construct_or_initialize<Cpp<Class>>(std::forward<Args>(args)...);
@@ -222,18 +226,19 @@
                         = construct_or_initialize<Alias<Class>>(std::forward<Args>(args)...);
                 }
             },
             is_new_style_constructor(),
             extra...);
     }
 
-    template <typename Class,
-              typename... Extra,
-              enable_if_t<Class::has_alias && !std::is_constructible<Cpp<Class>, Args...>::value,
-                          int> = 0>
+    template <
+        typename Class,
+        typename... Extra,
+        enable_if_t<Class::has_alias && !std::is_constructible<Cpp<Class>, Args...>::value, int>
+        = 0>
     static void execute(Class &cl, const Extra &...extra) {
         cl.def(
             "__init__",
             [](value_and_holder &v_h, Args... args) {
                 v_h.value_ptr()
                     = construct_or_initialize<Alias<Class>>(std::forward<Args>(args)...);
             },
@@ -241,18 +246,19 @@
             extra...);
     }
 };
 
 // Implementing class for py::init_alias<...>()
 template <typename... Args>
 struct alias_constructor {
-    template <typename Class,
-              typename... Extra,
-              enable_if_t<Class::has_alias && std::is_constructible<Alias<Class>, Args...>::value,
-                          int> = 0>
+    template <
+        typename Class,
+        typename... Extra,
+        enable_if_t<Class::has_alias && std::is_constructible<Alias<Class>, Args...>::value, int>
+        = 0>
     static void execute(Class &cl, const Extra &...extra) {
         cl.def(
             "__init__",
             [](value_and_holder &v_h, Args... args) {
                 v_h.value_ptr()
                     = construct_or_initialize<Alias<Class>>(std::forward<Args>(args)...);
             },
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/detail/internals.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/internals.h`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
+#include "common.h"
+
+#if defined(WITH_THREAD) && defined(PYBIND11_SIMPLE_GIL_MANAGEMENT)
+#    include "../gil.h"
+#endif
+
 #include "../pytypes.h"
 
 #include <exception>
 
 /// Tracks the `internals` and `type_info` ABI version independent of the main library version.
 ///
 /// Some portions of the code use an ABI that is conditional depending on this
@@ -33,27 +39,29 @@
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 using ExceptionTranslator = void (*)(std::exception_ptr);
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
+constexpr const char *internals_function_record_capsule_name = "pybind11_function_record_capsule";
+
 // Forward declarations
 inline PyTypeObject *make_static_property_type();
 inline PyTypeObject *make_default_metaclass();
 inline PyObject *make_object_base_type(PyTypeObject *metaclass);
 
 // The old Python Thread Local Storage (TLS) API is deprecated in Python 3.7 in favor of the new
 // Thread Specific Storage (TSS) API.
 #if PY_VERSION_HEX >= 0x03070000
 // Avoid unnecessary allocation of `Py_tss_t`, since we cannot use
 // `Py_LIMITED_API` anyway.
 #    if PYBIND11_INTERNALS_VERSION > 4
 #        define PYBIND11_TLS_KEY_REF Py_tss_t &
-#        ifdef __GNUC__
+#        if defined(__GNUC__) && !defined(__INTEL_COMPILER)
 // Clang on macOS warns due to `Py_tss_NEEDS_INIT` not specifying an initializer
 // for every field.
 #            define PYBIND11_TLS_KEY_INIT(var)                                                    \
                 _Pragma("GCC diagnostic push")                                         /**/       \
                     _Pragma("GCC diagnostic ignored \"-Wmissing-field-initializers\"") /**/       \
                     Py_tss_t var                                                                  \
                     = Py_tss_NEEDS_INIT;                                                          \
@@ -165,19 +173,31 @@
 #endif
     std::forward_list<std::string> static_strings; // Stores the std::strings backing
                                                    // detail::c_str()
     PyTypeObject *static_property_type;
     PyTypeObject *default_metaclass;
     PyObject *instance_base;
 #if defined(WITH_THREAD)
+    // Unused if PYBIND11_SIMPLE_GIL_MANAGEMENT is defined:
     PYBIND11_TLS_KEY_INIT(tstate)
 #    if PYBIND11_INTERNALS_VERSION > 4
     PYBIND11_TLS_KEY_INIT(loader_life_support_tls_key)
 #    endif // PYBIND11_INTERNALS_VERSION > 4
+    // Unused if PYBIND11_SIMPLE_GIL_MANAGEMENT is defined:
     PyInterpreterState *istate = nullptr;
+
+#    if PYBIND11_INTERNALS_VERSION > 4
+    // Note that we have to use a std::string to allocate memory to ensure a unique address
+    // We want unique addresses since we use pointer equality to compare function records
+    std::string function_record_capsule_name = internals_function_record_capsule_name;
+#    endif
+
+    internals() = default;
+    internals(const internals &other) = delete;
+    internals &operator=(const internals &other) = delete;
     ~internals() {
 #    if PYBIND11_INTERNALS_VERSION > 4
         PYBIND11_TLS_FREE(loader_life_support_tls_key);
 #    endif // PYBIND11_INTERNALS_VERSION > 4
 
         // This destructor is called *after* Py_Finalize() in finalize_interpreter().
         // That *SHOULD BE* fine. The following details what happens when PyThread_tss_free is
@@ -404,21 +424,29 @@
 /// Return a reference to the current `internals` data
 PYBIND11_NOINLINE internals &get_internals() {
     auto **&internals_pp = get_internals_pp();
     if (internals_pp && *internals_pp) {
         return **internals_pp;
     }
 
+#if defined(WITH_THREAD)
+#    if defined(PYBIND11_SIMPLE_GIL_MANAGEMENT)
+    gil_scoped_acquire gil;
+#    else
     // Ensure that the GIL is held since we will need to make Python calls.
     // Cannot use py::gil_scoped_acquire here since that constructor calls get_internals.
     struct gil_scoped_acquire_local {
         gil_scoped_acquire_local() : state(PyGILState_Ensure()) {}
+        gil_scoped_acquire_local(const gil_scoped_acquire_local &) = delete;
+        gil_scoped_acquire_local &operator=(const gil_scoped_acquire_local &) = delete;
         ~gil_scoped_acquire_local() { PyGILState_Release(state); }
         const PyGILState_STATE state;
     } gil;
+#    endif
+#endif
     error_scope err_scope;
 
     PYBIND11_STR_TYPE id(PYBIND11_INTERNALS_ID);
     auto builtins = handle(PyEval_GetBuiltins());
     if (builtins.contains(id) && isinstance<capsule>(builtins[id])) {
         internals_pp = static_cast<internals **>(capsule(builtins[id]));
 
@@ -436,17 +464,14 @@
         if (!internals_pp) {
             internals_pp = new internals *();
         }
         auto *&internals_ptr = *internals_pp;
         internals_ptr = new internals();
 #if defined(WITH_THREAD)
 
-#    if PY_VERSION_HEX < 0x03090000
-        PyEval_InitThreads();
-#    endif
         PyThreadState *tstate = PyThreadState_Get();
         if (!PYBIND11_TLS_KEY_CREATE(internals_ptr->tstate)) {
             pybind11_fail("get_internals: could not successfully initialize the tstate TSS key!");
         }
         PYBIND11_TLS_REPLACE_VALUE(internals_ptr->tstate, tstate);
 
 #    if PYBIND11_INTERNALS_VERSION > 4
@@ -508,29 +533,53 @@
             = static_cast<shared_loader_life_support_data *>(ptr)->loader_life_support_tls_key;
     }
 #endif //  defined(WITH_THREAD) && PYBIND11_INTERNALS_VERSION == 4
 };
 
 /// Works like `get_internals`, but for things which are locally registered.
 inline local_internals &get_local_internals() {
-    static local_internals locals;
-    return locals;
+    // Current static can be created in the interpreter finalization routine. If the later will be
+    // destroyed in another static variable destructor, creation of this static there will cause
+    // static deinitialization fiasco. In order to avoid it we avoid destruction of the
+    // local_internals static. One can read more about the problem and current solution here:
+    // https://google.github.io/styleguide/cppguide.html#Static_and_Global_Variables
+    static auto *locals = new local_internals();
+    return *locals;
 }
 
 /// Constructs a std::string with the given arguments, stores it in `internals`, and returns its
 /// `c_str()`.  Such strings objects have a long storage duration -- the internal strings are only
 /// cleared when the program exits or after interpreter shutdown (when embedding), and so are
 /// suitable for c-style strings needed by Python internals (such as PyTypeObject's tp_name).
 template <typename... Args>
 const char *c_str(Args &&...args) {
     auto &strings = get_internals().static_strings;
     strings.emplace_front(std::forward<Args>(args)...);
     return strings.front().c_str();
 }
 
+inline const char *get_function_record_capsule_name() {
+#if PYBIND11_INTERNALS_VERSION > 4
+    return get_internals().function_record_capsule_name.c_str();
+#else
+    return nullptr;
+#endif
+}
+
+// Determine whether or not the following capsule contains a pybind11 function record.
+// Note that we use `internals` to make sure that only ABI compatible records are touched.
+//
+// This check is currently used in two places:
+// - An important optimization in functional.h to avoid overhead in C++ -> Python -> C++
+// - The sibling feature of cpp_function to allow overloads
+inline bool is_function_record_capsule(const capsule &cap) {
+    // Pointer equality as we rely on internals() to ensure unique pointers
+    return cap.name() == get_function_record_capsule_name();
+}
+
 PYBIND11_NAMESPACE_END(detail)
 
 /// Returns a named pointer that is shared among all extension modules (using the same
 /// pybind11 version) running in the current interpreter. Names starting with underscores
 /// are reserved for internal usage. Returns `nullptr` if no matching entry was found.
 PYBIND11_NOINLINE void *get_shared_data(const std::string &name) {
     auto &internals = detail::get_internals();
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/detail/type_caster_base.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files 1% similar despite different names*

```diff
@@ -1002,9 +1002,18 @@
         };
     }
 
     static Constructor make_copy_constructor(...) { return nullptr; }
     static Constructor make_move_constructor(...) { return nullptr; }
 };
 
+PYBIND11_NOINLINE std::string type_info_description(const std::type_info &ti) {
+    if (auto *type_data = get_type_info(ti)) {
+        handle th((PyObject *) type_data->type);
+        return th.attr("__module__").cast<std::string>() + '.'
+               + th.attr("__qualname__").cast<std::string>();
+    }
+    return clean_type_id(ti.name());
+}
+
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/detail/typeid.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/eigen.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/eigen/matrix.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,47 @@
 /*
-    pybind11/eigen.h: Transparent conversion for dense and sparse Eigen matrices
+    pybind11/eigen/matrix.h: Transparent conversion for dense and sparse Eigen matrices
 
     Copyright (c) 2016 Wenzel Jakob <wenzel.jakob@epfl.ch>
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
+#include "../numpy.h"
+
 /* HINT: To suppress warnings originating from the Eigen headers, use -isystem.
    See also:
        https://stackoverflow.com/questions/2579576/i-dir-vs-isystem-dir
        https://stackoverflow.com/questions/1741816/isystem-for-ms-visual-studio-c-compiler
 */
-
-#include "numpy.h"
-
-// The C4127 suppression was introduced for Eigen 3.4.0. In theory we could
-// make it version specific, or even remove it later, but considering that
-// 1. C4127 is generally far more distracting than useful for modern template code, and
-// 2. we definitely want to ignore any MSVC warnings originating from Eigen code,
-//    it is probably best to keep this around indefinitely.
-#if defined(_MSC_VER)
-#    pragma warning(push)
-#    pragma warning(disable : 4127) // C4127: conditional expression is constant
-#    pragma warning(disable : 5054) // https://github.com/pybind/pybind11/pull/3741
+PYBIND11_WARNING_PUSH
+PYBIND11_WARNING_DISABLE_MSVC(5054) // https://github.com/pybind/pybind11/pull/3741
 //       C5054: operator '&': deprecated between enumerations of different types
+#if defined(__MINGW32__)
+PYBIND11_WARNING_DISABLE_GCC("-Wmaybe-uninitialized")
 #endif
 
 #include <Eigen/Core>
 #include <Eigen/SparseCore>
 
-#if defined(_MSC_VER)
-#    pragma warning(pop)
-#endif
+PYBIND11_WARNING_POP
 
 // Eigen prior to 3.2.7 doesn't have proper move constructors--but worse, some classes get implicit
 // move constructors that break things.  We could detect this an explicitly copy, but an extra copy
 // of matrices seems highly undesirable.
 static_assert(EIGEN_VERSION_AT_LEAST(3, 2, 7),
-              "Eigen support in pybind11 requires Eigen >= 3.2.7");
+              "Eigen matrix support in pybind11 requires Eigen >= 3.2.7");
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
+PYBIND11_WARNING_DISABLE_MSVC(4127)
+
 // Provide a convenience alias for easier pass-by-ref usage with fully dynamic strides:
 using EigenDStride = Eigen::Stride<Eigen::Dynamic, Eigen::Dynamic>;
 template <typename MatrixType>
 using EigenDRef = Eigen::Ref<MatrixType, 0, EigenDStride>;
 template <typename MatrixType>
 using EigenDMap = Eigen::Map<MatrixType, 0, EigenDStride>;
 
@@ -181,29 +175,28 @@
         }
 
         if (dims == 2) { // Matrix type: require exact match (or dynamic)
 
             EigenIndex np_rows = a.shape(0), np_cols = a.shape(1),
                        np_rstride = a.strides(0) / static_cast<ssize_t>(sizeof(Scalar)),
                        np_cstride = a.strides(1) / static_cast<ssize_t>(sizeof(Scalar));
-            if ((PYBIND11_SILENCE_MSVC_C4127(fixed_rows) && np_rows != rows)
-                || (PYBIND11_SILENCE_MSVC_C4127(fixed_cols) && np_cols != cols)) {
+            if ((fixed_rows && np_rows != rows) || (fixed_cols && np_cols != cols)) {
                 return false;
             }
 
             return {np_rows, np_cols, np_rstride, np_cstride};
         }
 
         // Otherwise we're storing an n-vector.  Only one of the strides will be used, but
         // whichever is used, we want the (single) numpy stride value.
         const EigenIndex n = a.shape(0),
                          stride = a.strides(0) / static_cast<ssize_t>(sizeof(Scalar));
 
         if (vector) { // Eigen type is a compile-time vector
-            if (PYBIND11_SILENCE_MSVC_C4127(fixed) && size != n) {
+            if (fixed && size != n) {
                 return false; // Vector size mismatch
             }
             return {rows == 1 ? 1 : n, cols == 1 ? 1 : n, stride};
         }
         if (fixed) {
             // The type has a fixed size, but is not a vector: abort
             return false;
@@ -212,15 +205,15 @@
             // Since this isn't a vector, cols must be != 1.  We allow this only if it exactly
             // equals the number of elements (rows is Dynamic, and so 1 row is allowed).
             if (cols != n) {
                 return false;
             }
             return {1, n, stride};
         } // Otherwise it's either fully dynamic, or column dynamic; both become a column vector
-        if (PYBIND11_SILENCE_MSVC_C4127(fixed_rows) && rows != n) {
+        if (fixed_rows && rows != n) {
             return false;
         }
         return {n, 1, stride};
     }
 
     static constexpr bool show_writeable
         = is_eigen_dense_map<Type>::value && is_eigen_mutable_map<Type>::value;
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/embed.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/embed.h`

 * *Files 12% similar despite different names*

```diff
@@ -82,46 +82,34 @@
 };
 
 inline wchar_t *widen_chars(const char *safe_arg) {
     wchar_t *widened_arg = Py_DecodeLocale(safe_arg, nullptr);
     return widened_arg;
 }
 
-PYBIND11_NAMESPACE_END(detail)
-
-/** \rst
-    Initialize the Python interpreter. No other pybind11 or CPython API functions can be
-    called before this is done; with the exception of `PYBIND11_EMBEDDED_MODULE`. The
-    optional `init_signal_handlers` parameter can be used to skip the registration of
-    signal handlers (see the `Python documentation`_ for details). Calling this function
-    again after the interpreter has already been initialized is a fatal error.
-
-    If initializing the Python interpreter fails, then the program is terminated.  (This
-    is controlled by the CPython runtime and is an exception to pybind11's normal behavior
-    of throwing exceptions on errors.)
-
-    The remaining optional parameters, `argc`, `argv`, and `add_program_dir_to_path` are
-    used to populate ``sys.argv`` and ``sys.path``.
-    See the |PySys_SetArgvEx documentation|_ for details.
-
-    .. _Python documentation: https://docs.python.org/3/c-api/init.html#c.Py_InitializeEx
-    .. |PySys_SetArgvEx documentation| replace:: ``PySys_SetArgvEx`` documentation
-    .. _PySys_SetArgvEx documentation: https://docs.python.org/3/c-api/init.html#c.PySys_SetArgvEx
- \endrst */
-inline void initialize_interpreter(bool init_signal_handlers = true,
-                                   int argc = 0,
-                                   const char *const *argv = nullptr,
-                                   bool add_program_dir_to_path = true) {
+inline void precheck_interpreter() {
     if (Py_IsInitialized() != 0) {
         pybind11_fail("The interpreter is already running");
     }
+}
 
-#if PY_VERSION_HEX < 0x030B0000
+#if !defined(PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX)
+#    define PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX (0x03080000)
+#endif
 
+#if PY_VERSION_HEX < PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX
+inline void initialize_interpreter_pre_pyconfig(bool init_signal_handlers,
+                                                int argc,
+                                                const char *const *argv,
+                                                bool add_program_dir_to_path) {
+    detail::precheck_interpreter();
     Py_InitializeEx(init_signal_handlers ? 1 : 0);
+#    if defined(WITH_THREAD) && PY_VERSION_HEX < 0x03070000
+    PyEval_InitThreads();
+#    endif
 
     // Before it was special-cased in python 3.8, passing an empty or null argv
     // caused a segfault, so we have to reimplement the special case ourselves.
     bool special_case = (argv == nullptr || argc <= 0);
 
     const char *const empty_argv[]{"\0"};
     const char *const *safe_argv = special_case ? empty_argv : argv;
@@ -143,39 +131,82 @@
         }
         widened_argv[ii] = widened_argv_entries.back().get();
     }
 
     auto *pysys_argv = widened_argv.get();
 
     PySys_SetArgvEx(argc, pysys_argv, static_cast<int>(add_program_dir_to_path));
-#else
-    PyConfig config;
-    PyConfig_InitIsolatedConfig(&config);
-    config.install_signal_handlers = init_signal_handlers ? 1 : 0;
+}
+#endif
 
-    PyStatus status = PyConfig_SetBytesArgv(&config, argc, const_cast<char *const *>(argv));
-    if (PyStatus_Exception(status)) {
+PYBIND11_NAMESPACE_END(detail)
+
+#if PY_VERSION_HEX >= PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX
+inline void initialize_interpreter(PyConfig *config,
+                                   int argc = 0,
+                                   const char *const *argv = nullptr,
+                                   bool add_program_dir_to_path = true) {
+    detail::precheck_interpreter();
+    PyStatus status = PyConfig_SetBytesArgv(config, argc, const_cast<char *const *>(argv));
+    if (PyStatus_Exception(status) != 0) {
         // A failure here indicates a character-encoding failure or the python
         // interpreter out of memory. Give up.
-        PyConfig_Clear(&config);
-        throw std::runtime_error(PyStatus_IsError(status) ? status.err_msg
-                                                          : "Failed to prepare CPython");
-    }
-    status = Py_InitializeFromConfig(&config);
-    PyConfig_Clear(&config);
-    if (PyStatus_Exception(status)) {
-        throw std::runtime_error(PyStatus_IsError(status) ? status.err_msg
-                                                          : "Failed to init CPython");
+        PyConfig_Clear(config);
+        throw std::runtime_error(PyStatus_IsError(status) != 0 ? status.err_msg
+                                                               : "Failed to prepare CPython");
+    }
+    status = Py_InitializeFromConfig(config);
+    if (PyStatus_Exception(status) != 0) {
+        PyConfig_Clear(config);
+        throw std::runtime_error(PyStatus_IsError(status) != 0 ? status.err_msg
+                                                               : "Failed to init CPython");
     }
     if (add_program_dir_to_path) {
         PyRun_SimpleString("import sys, os.path; "
                            "sys.path.insert(0, "
                            "os.path.abspath(os.path.dirname(sys.argv[0])) "
                            "if sys.argv and os.path.exists(sys.argv[0]) else '')");
     }
+    PyConfig_Clear(config);
+}
+#endif
+
+/** \rst
+    Initialize the Python interpreter. No other pybind11 or CPython API functions can be
+    called before this is done; with the exception of `PYBIND11_EMBEDDED_MODULE`. The
+    optional `init_signal_handlers` parameter can be used to skip the registration of
+    signal handlers (see the `Python documentation`_ for details). Calling this function
+    again after the interpreter has already been initialized is a fatal error.
+
+    If initializing the Python interpreter fails, then the program is terminated.  (This
+    is controlled by the CPython runtime and is an exception to pybind11's normal behavior
+    of throwing exceptions on errors.)
+
+    The remaining optional parameters, `argc`, `argv`, and `add_program_dir_to_path` are
+    used to populate ``sys.argv`` and ``sys.path``.
+    See the |PySys_SetArgvEx documentation|_ for details.
+
+    .. _Python documentation: https://docs.python.org/3/c-api/init.html#c.Py_InitializeEx
+    .. |PySys_SetArgvEx documentation| replace:: ``PySys_SetArgvEx`` documentation
+    .. _PySys_SetArgvEx documentation: https://docs.python.org/3/c-api/init.html#c.PySys_SetArgvEx
+ \endrst */
+inline void initialize_interpreter(bool init_signal_handlers = true,
+                                   int argc = 0,
+                                   const char *const *argv = nullptr,
+                                   bool add_program_dir_to_path = true) {
+#if PY_VERSION_HEX < PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX
+    detail::initialize_interpreter_pre_pyconfig(
+        init_signal_handlers, argc, argv, add_program_dir_to_path);
+#else
+    PyConfig config;
+    PyConfig_InitIsolatedConfig(&config);
+    config.isolated = 0;
+    config.use_environment = 1;
+    config.install_signal_handlers = init_signal_handlers ? 1 : 0;
+    initialize_interpreter(&config, argc, argv, add_program_dir_to_path);
 #endif
 }
 
 /** \rst
     Shut down the Python interpreter. No pybind11 or CPython API functions can be called
     after this. In addition, pybind11 objects must not outlive the interpreter:
 
@@ -255,14 +286,23 @@
     explicit scoped_interpreter(bool init_signal_handlers = true,
                                 int argc = 0,
                                 const char *const *argv = nullptr,
                                 bool add_program_dir_to_path = true) {
         initialize_interpreter(init_signal_handlers, argc, argv, add_program_dir_to_path);
     }
 
+#if PY_VERSION_HEX >= PYBIND11_PYCONFIG_SUPPORT_PY_VERSION_HEX
+    explicit scoped_interpreter(PyConfig *config,
+                                int argc = 0,
+                                const char *const *argv = nullptr,
+                                bool add_program_dir_to_path = true) {
+        initialize_interpreter(config, argc, argv, add_program_dir_to_path);
+    }
+#endif
+
     scoped_interpreter(const scoped_interpreter &) = delete;
     scoped_interpreter(scoped_interpreter &&other) noexcept { other.is_valid = false; }
     scoped_interpreter &operator=(const scoped_interpreter &) = delete;
     scoped_interpreter &operator=(scoped_interpreter &&) = delete;
 
     ~scoped_interpreter() {
         if (is_valid) {
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/eval.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/functional.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/functional.h`

 * *Files 5% similar despite different names*

```diff
@@ -44,17 +44,24 @@
            a full C++ -> Python -> C++ roundtrip, which can be prohibitive.
            Here, we try to at least detect the case where the function is
            stateless (i.e. function pointer or lambda function without
            captured variables), in which case the roundtrip can be avoided.
          */
         if (auto cfunc = func.cpp_function()) {
             auto *cfunc_self = PyCFunction_GET_SELF(cfunc.ptr());
-            if (isinstance<capsule>(cfunc_self)) {
+            if (cfunc_self == nullptr) {
+                PyErr_Clear();
+            } else if (isinstance<capsule>(cfunc_self)) {
                 auto c = reinterpret_borrow<capsule>(cfunc_self);
-                auto *rec = (function_record *) c;
+
+                function_record *rec = nullptr;
+                // Check that we can safely reinterpret the capsule into a function_record
+                if (detail::is_function_record_capsule(c)) {
+                    rec = c.get_pointer<function_record>();
+                }
 
                 while (rec != nullptr) {
                     if (rec->is_stateless
                         && same_type(typeid(function_type),
                                      *reinterpret_cast<const std::type_info *>(rec->data[1]))) {
                         struct capture {
                             function_type f;
@@ -106,15 +113,15 @@
         value = func_wrapper(func_handle(std::move(func)));
         return true;
     }
 
     template <typename Func>
     static handle cast(Func &&f_, return_value_policy policy, handle /* parent */) {
         if (!f_) {
-            return none().inc_ref();
+            return none().release();
         }
 
         auto result = f_.template target<function_type>();
         if (result) {
             return cpp_function(*result, policy).release();
         }
         return cpp_function(std::forward<Func>(f_), policy).release();
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/gil.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/gil.h`

 * *Files 18% similar despite different names*

```diff
@@ -6,26 +6,31 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "detail/common.h"
-#include "detail/internals.h"
+
+#if defined(WITH_THREAD) && !defined(PYBIND11_SIMPLE_GIL_MANAGEMENT)
+#    include "detail/internals.h"
+#endif
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 // forward declarations
 PyThreadState *get_thread_state_unchecked();
 
 PYBIND11_NAMESPACE_END(detail)
 
-#if defined(WITH_THREAD) && !defined(PYPY_VERSION)
+#if defined(WITH_THREAD)
+
+#    if !defined(PYBIND11_SIMPLE_GIL_MANAGEMENT)
 
 /* The functions below essentially reproduce the PyGILState_* API using a RAII
  * pattern, but there are a few important differences:
  *
  * 1. When acquiring the GIL from an non-main thread during the finalization
  *    phase, the GILState API blindly terminates the calling thread, which
  *    is often not what is wanted. This API does not do this.
@@ -58,50 +63,53 @@
                below. Note we don't save this state with internals.tstate, since we don't
                create it we would fail to clear it (its reference count should be > 0). */
             tstate = PyGILState_GetThisThreadState();
         }
 
         if (!tstate) {
             tstate = PyThreadState_New(internals.istate);
-#    if defined(PYBIND11_DETAILED_ERROR_MESSAGES)
+#        if defined(PYBIND11_DETAILED_ERROR_MESSAGES)
             if (!tstate) {
                 pybind11_fail("scoped_acquire: could not create thread state!");
             }
-#    endif
+#        endif
             tstate->gilstate_counter = 0;
             PYBIND11_TLS_REPLACE_VALUE(internals.tstate, tstate);
         } else {
             release = detail::get_thread_state_unchecked() != tstate;
         }
 
         if (release) {
             PyEval_AcquireThread(tstate);
         }
 
         inc_ref();
     }
 
+    gil_scoped_acquire(const gil_scoped_acquire &) = delete;
+    gil_scoped_acquire &operator=(const gil_scoped_acquire &) = delete;
+
     void inc_ref() { ++tstate->gilstate_counter; }
 
     PYBIND11_NOINLINE void dec_ref() {
         --tstate->gilstate_counter;
-#    if defined(PYBIND11_DETAILED_ERROR_MESSAGES)
+#        if defined(PYBIND11_DETAILED_ERROR_MESSAGES)
         if (detail::get_thread_state_unchecked() != tstate) {
             pybind11_fail("scoped_acquire::dec_ref(): thread state must be current!");
         }
         if (tstate->gilstate_counter < 0) {
             pybind11_fail("scoped_acquire::dec_ref(): reference count underflow!");
         }
-#    endif
+#        endif
         if (tstate->gilstate_counter == 0) {
-#    if defined(PYBIND11_DETAILED_ERROR_MESSAGES)
+#        if defined(PYBIND11_DETAILED_ERROR_MESSAGES)
             if (!release) {
                 pybind11_fail("scoped_acquire::dec_ref(): internal error!");
             }
-#    endif
+#        endif
             PyThreadState_Clear(tstate);
             if (active) {
                 PyThreadState_DeleteCurrent();
             }
             PYBIND11_TLS_DELETE_VALUE(detail::get_internals().tstate);
             release = false;
         }
@@ -140,14 +148,17 @@
             // Python >= 3.7 can remove this, it's an int before 3.7
             // NOLINTNEXTLINE(readability-qualified-auto)
             auto key = internals.tstate;
             PYBIND11_TLS_DELETE_VALUE(key);
         }
     }
 
+    gil_scoped_release(const gil_scoped_release &) = delete;
+    gil_scoped_release &operator=(const gil_scoped_release &) = delete;
+
     /// This method will disable the PyThreadState_DeleteCurrent call and the
     /// GIL won't be acquired. This method should be used if the interpreter
     /// could be shutting down when this is called, as thread deletion is not
     /// allowed during shutdown. Check _Py_IsFinalizing() on Python 3.7+, and
     /// protect subsequent code.
     PYBIND11_NOINLINE void disarm() { active = false; }
 
@@ -168,35 +179,61 @@
     }
 
 private:
     PyThreadState *tstate;
     bool disassoc;
     bool active = true;
 };
-#elif defined(PYPY_VERSION)
+
+#    else // PYBIND11_SIMPLE_GIL_MANAGEMENT
+
 class gil_scoped_acquire {
     PyGILState_STATE state;
 
 public:
-    gil_scoped_acquire() { state = PyGILState_Ensure(); }
+    gil_scoped_acquire() : state{PyGILState_Ensure()} {}
+    gil_scoped_acquire(const gil_scoped_acquire &) = delete;
+    gil_scoped_acquire &operator=(const gil_scoped_acquire &) = delete;
     ~gil_scoped_acquire() { PyGILState_Release(state); }
     void disarm() {}
 };
 
 class gil_scoped_release {
     PyThreadState *state;
 
 public:
-    gil_scoped_release() { state = PyEval_SaveThread(); }
+    gil_scoped_release() : state{PyEval_SaveThread()} {}
+    gil_scoped_release(const gil_scoped_release &) = delete;
+    gil_scoped_release &operator=(const gil_scoped_release &) = delete;
     ~gil_scoped_release() { PyEval_RestoreThread(state); }
     void disarm() {}
 };
-#else
+
+#    endif // PYBIND11_SIMPLE_GIL_MANAGEMENT
+
+#else // WITH_THREAD
+
 class gil_scoped_acquire {
+public:
+    gil_scoped_acquire() {
+        // Trick to suppress `unused variable` error messages (at call sites).
+        (void) (this != (this + 1));
+    }
+    gil_scoped_acquire(const gil_scoped_acquire &) = delete;
+    gil_scoped_acquire &operator=(const gil_scoped_acquire &) = delete;
     void disarm() {}
 };
+
 class gil_scoped_release {
+public:
+    gil_scoped_release() {
+        // Trick to suppress `unused variable` error messages (at call sites).
+        (void) (this != (this + 1));
+    }
+    gil_scoped_release(const gil_scoped_release &) = delete;
+    gil_scoped_release &operator=(const gil_scoped_release &) = delete;
     void disarm() {}
 };
-#endif
+
+#endif // WITH_THREAD
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/iostream.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/numpy.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/numpy.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,16 @@
    upon the library user. */
 static_assert(sizeof(::pybind11::ssize_t) == sizeof(Py_intptr_t), "ssize_t != Py_intptr_t");
 static_assert(std::is_signed<Py_intptr_t>::value, "Py_intptr_t must be signed");
 // We now can reinterpret_cast between py::ssize_t and Py_intptr_t (MSVC + PyPy cares)
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
+PYBIND11_WARNING_DISABLE_MSVC(4127)
+
 class array; // Forward declaration
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <>
 struct handle_type_name<array> {
     static constexpr auto name = const_name("numpy.ndarray");
@@ -533,15 +535,15 @@
 struct type_caster<unchecked_mutable_reference<T, Dim>>
     : type_caster<unchecked_reference<T, Dim>> {};
 
 PYBIND11_NAMESPACE_END(detail)
 
 class dtype : public object {
 public:
-    PYBIND11_OBJECT_DEFAULT(dtype, object, detail::npy_api::get().PyArrayDescr_Check_);
+    PYBIND11_OBJECT_DEFAULT(dtype, object, detail::npy_api::get().PyArrayDescr_Check_)
 
     explicit dtype(const buffer_info &info) {
         dtype descr(_dtype_from_pep3118()(pybind11::str(info.format)));
         // If info.itemsize == 0, use the value calculated from the format string
         m_ptr = descr.strip_padding(info.itemsize != 0 ? info.itemsize : descr.itemsize())
                     .release()
                     .ptr();
@@ -871,15 +873,15 @@
      * Returns a proxy object that provides access to the array's data without bounds or
      * dimensionality checking.  Will throw if the array is missing the `writeable` flag.  Use with
      * care: the array must not be destroyed or reshaped for the duration of the returned object,
      * and the caller must take care not to access invalid dimensions or dimension indices.
      */
     template <typename T, ssize_t Dims = -1>
     detail::unchecked_mutable_reference<T, Dims> mutable_unchecked() & {
-        if (PYBIND11_SILENCE_MSVC_C4127(Dims >= 0) && ndim() != Dims) {
+        if (Dims >= 0 && ndim() != Dims) {
             throw std::domain_error("array has incorrect number of dimensions: "
                                     + std::to_string(ndim()) + "; expected "
                                     + std::to_string(Dims));
         }
         return detail::unchecked_mutable_reference<T, Dims>(
             mutable_data(), shape(), strides(), ndim());
     }
@@ -889,15 +891,15 @@
      * dimensionality checking.  Unlike `mutable_unchecked()`, this does not require that the
      * underlying array have the `writable` flag.  Use with care: the array must not be destroyed
      * or reshaped for the duration of the returned object, and the caller must take care not to
      * access invalid dimensions or dimension indices.
      */
     template <typename T, ssize_t Dims = -1>
     detail::unchecked_reference<T, Dims> unchecked() const & {
-        if (PYBIND11_SILENCE_MSVC_C4127(Dims >= 0) && ndim() != Dims) {
+        if (Dims >= 0 && ndim() != Dims) {
             throw std::domain_error("array has incorrect number of dimensions: "
                                     + std::to_string(ndim()) + "; expected "
                                     + std::to_string(Dims));
         }
         return detail::unchecked_reference<T, Dims>(data(), shape(), strides(), ndim());
     }
 
@@ -1115,18 +1117,18 @@
     template <ssize_t Dims = -1>
     detail::unchecked_mutable_reference<T, Dims> mutable_unchecked() & {
         return array::mutable_unchecked<T, Dims>();
     }
 
     /**
      * Returns a proxy object that provides const access to the array's data without bounds or
-     * dimensionality checking.  Unlike `unchecked()`, this does not require that the underlying
-     * array have the `writable` flag.  Use with care: the array must not be destroyed or reshaped
-     * for the duration of the returned object, and the caller must take care not to access invalid
-     * dimensions or dimension indices.
+     * dimensionality checking.  Unlike `mutable_unchecked()`, this does not require that the
+     * underlying array have the `writable` flag.  Use with care: the array must not be destroyed
+     * or reshaped for the duration of the returned object, and the caller must take care not to
+     * access invalid dimensions or dimension indices.
      */
     template <ssize_t Dims = -1>
     detail::unchecked_reference<T, Dims> unchecked() const & {
         return array::unchecked<T, Dims>();
     }
 
     /// Ensure that the argument is a NumPy array of the correct dtype (and if not, try to convert
@@ -1397,15 +1399,15 @@
     }
     if (itemsize > offset) {
         oss << (itemsize - offset) << 'x';
     }
     oss << '}';
     auto format_str = oss.str();
 
-    // Sanity check: verify that NumPy properly parses our buffer format string
+    // Smoke test: verify that NumPy properly parses our buffer format string
     auto &api = npy_api::get();
     auto arr = array(buffer_info(nullptr, itemsize, format_str, 1));
     if (!api.PyArray_EquivTypes_(dtype_ptr, arr.dtype().ptr())) {
         pybind11_fail("NumPy: invalid buffer descriptor!");
     }
 
     auto tindex = std::type_index(tinfo);
@@ -1465,15 +1467,15 @@
             Name, offsetof(T, Field), sizeof(decltype(std::declval<T>().Field)),                  \
                 ::pybind11::format_descriptor<decltype(std::declval<T>().Field)>::format(),       \
                 ::pybind11::detail::npy_format_descriptor<                                        \
                     decltype(std::declval<T>().Field)>::dtype()                                   \
         }
 
 // Extract name, offset and format descriptor for a struct field
-#    define PYBIND11_FIELD_DESCRIPTOR(T, Field) PYBIND11_FIELD_DESCRIPTOR_EX(T, Field, #    Field)
+#    define PYBIND11_FIELD_DESCRIPTOR(T, Field) PYBIND11_FIELD_DESCRIPTOR_EX(T, Field, #Field)
 
 // The main idea of this macro is borrowed from https://github.com/swansontec/map-macro
 // (C) William Swanson, Paul Fultz
 #    define PYBIND11_EVAL0(...) __VA_ARGS__
 #    define PYBIND11_EVAL1(...) PYBIND11_EVAL0(PYBIND11_EVAL0(PYBIND11_EVAL0(__VA_ARGS__)))
 #    define PYBIND11_EVAL2(...) PYBIND11_EVAL1(PYBIND11_EVAL1(PYBIND11_EVAL1(__VA_ARGS__)))
 #    define PYBIND11_EVAL3(...) PYBIND11_EVAL2(PYBIND11_EVAL2(PYBIND11_EVAL2(__VA_ARGS__)))
@@ -1862,27 +1864,33 @@
             PYBIND11_EXPAND_SIDE_EFFECTS(params[VIndex] = buffers[BIndex].ptr);
             return cast(
                 returned_array::call(f, *reinterpret_cast<param_n_t<Index> *>(params[Index])...));
         }
 
         auto result = returned_array::create(trivial, shape);
 
+        PYBIND11_WARNING_PUSH
+#ifdef PYBIND11_DETECTED_CLANG_WITH_MISLEADING_CALL_STD_MOVE_EXPLICITLY_WARNING
+        PYBIND11_WARNING_DISABLE_CLANG("-Wreturn-std-move")
+#endif
+
         if (size == 0) {
-            return std::move(result);
+            return result;
         }
 
         /* Call the function */
         auto *mutable_data = returned_array::mutable_data(result);
         if (trivial == broadcast_trivial::non_trivial) {
             apply_broadcast(buffers, params, mutable_data, size, shape, i_seq, vi_seq, bi_seq);
         } else {
             apply_trivial(buffers, params, mutable_data, size, i_seq, vi_seq, bi_seq);
         }
 
-        return std::move(result);
+        return result;
+        PYBIND11_WARNING_POP
     }
 
     template <size_t... Index, size_t... VIndex, size_t... BIndex>
     void apply_trivial(std::array<buffer_info, NVectorized> &buffers,
                        std::array<void *, N> &params,
                        Return *out,
                        size_t size,
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/operators.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/operators.h`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 /// base template of operator implementations
 template <op_id, op_type, typename B, typename L, typename R>
 struct op_impl {};
 
 /// Operator implementation generator
 template <op_id id, op_type ot, typename L, typename R>
 struct op_ {
+    static constexpr bool op_enable_if_hook = true;
     template <typename Class, typename... Extra>
     void execute(Class &cl, const Extra &...extra) const {
         using Base = typename Class::type;
         using L_type = conditional_t<std::is_same<L, self_t>::value, Base, L>;
         using R_type = conditional_t<std::is_same<R, self_t>::value, Base, R>;
         using op = op_impl<id, ot, Base, L_type, R_type>;
         cl.def(op::name(), &op::execute, is_operator(), extra...);
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/options.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/options.h`

 * *Files 25% similar despite different names*

```diff
@@ -43,30 +43,46 @@
     }
 
     options &enable_function_signatures() & {
         global_state().show_function_signatures = true;
         return *this;
     }
 
+    options &disable_enum_members_docstring() & {
+        global_state().show_enum_members_docstring = false;
+        return *this;
+    }
+
+    options &enable_enum_members_docstring() & {
+        global_state().show_enum_members_docstring = true;
+        return *this;
+    }
+
     // Getter methods (return the global state):
 
     static bool show_user_defined_docstrings() {
         return global_state().show_user_defined_docstrings;
     }
 
     static bool show_function_signatures() { return global_state().show_function_signatures; }
 
+    static bool show_enum_members_docstring() {
+        return global_state().show_enum_members_docstring;
+    }
+
     // This type is not meant to be allocated on the heap.
     void *operator new(size_t) = delete;
 
 private:
     struct state {
         bool show_user_defined_docstrings = true; //< Include user-supplied texts in docstrings.
         bool show_function_signatures = true;     //< Include auto-generated function signatures
                                                   //  in docstrings.
+        bool show_enum_members_docstring = true;  //< Include auto-generated member list in enum
+                                                  //  docstrings.
     };
 
     static state &global_state() {
         static state instance;
         return instance;
     }
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/pybind11.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/pybind11.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,27 +31,28 @@
 #    define PYBIND11_STD_LAUNDER
 #    define PYBIND11_HAS_STD_LAUNDER 0
 #endif
 #if defined(__GNUG__) && !defined(__clang__)
 #    include <cxxabi.h>
 #endif
 
+PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
+
 /* https://stackoverflow.com/questions/46798456/handling-gccs-noexcept-type-warning
    This warning is about ABI compatibility, not code health.
    It is only actually needed in a couple places, but apparently GCC 7 "generates this warning if
    and only if the first template instantiation ... involves noexcept" [stackoverflow], therefore
    it could get triggered from seemingly random places, depending on user code.
    No other GCC version generates this warning.
  */
 #if defined(__GNUC__) && __GNUC__ == 7
-#    pragma GCC diagnostic push
-#    pragma GCC diagnostic ignored "-Wnoexcept-type"
+PYBIND11_WARNING_DISABLE_GCC("-Wnoexcept-type")
 #endif
 
-PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
+PYBIND11_WARNING_DISABLE_MSVC(4127)
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 // Apply all the extensions translators from a list
 // Return true if one of the translators completed without raising an exception
 // itself. Return of false indicates that if there are other translators
 // available, they should be tried.
@@ -173,42 +174,40 @@
         /* Store the function including any extra state it might have (e.g. a lambda capture
          * object) */
         // The unique_ptr makes sure nothing is leaked in case of an exception.
         auto unique_rec = make_function_record();
         auto *rec = unique_rec.get();
 
         /* Store the capture object directly in the function record if there is enough space */
-        if (PYBIND11_SILENCE_MSVC_C4127(sizeof(capture) <= sizeof(rec->data))) {
+        if (sizeof(capture) <= sizeof(rec->data)) {
             /* Without these pragmas, GCC warns that there might not be
                enough space to use the placement new operator. However, the
                'if' statement above ensures that this is the case. */
-#if defined(__GNUG__) && __GNUC__ >= 6 && !defined(__clang__) && !defined(__INTEL_COMPILER)
-#    pragma GCC diagnostic push
-#    pragma GCC diagnostic ignored "-Wplacement-new"
+            PYBIND11_WARNING_PUSH
+
+#if defined(__GNUG__) && __GNUC__ >= 6
+            PYBIND11_WARNING_DISABLE_GCC("-Wplacement-new")
 #endif
+
             new ((capture *) &rec->data) capture{std::forward<Func>(f)};
-#if defined(__GNUG__) && __GNUC__ >= 6 && !defined(__clang__) && !defined(__INTEL_COMPILER)
-#    pragma GCC diagnostic pop
-#endif
-#if defined(__GNUG__) && !PYBIND11_HAS_STD_LAUNDER && !defined(__INTEL_COMPILER)
-#    pragma GCC diagnostic push
-#    pragma GCC diagnostic ignored "-Wstrict-aliasing"
+
+#if !PYBIND11_HAS_STD_LAUNDER
+            PYBIND11_WARNING_DISABLE_GCC("-Wstrict-aliasing")
 #endif
+
             // UB without std::launder, but without breaking ABI and/or
             // a significant refactoring it's "impossible" to solve.
             if (!std::is_trivially_destructible<capture>::value) {
                 rec->free_data = [](function_record *r) {
                     auto data = PYBIND11_STD_LAUNDER((capture *) &r->data);
                     (void) data;
                     data->~capture();
                 };
             }
-#if defined(__GNUG__) && !PYBIND11_HAS_STD_LAUNDER && !defined(__INTEL_COMPILER)
-#    pragma GCC diagnostic pop
-#endif
+            PYBIND11_WARNING_POP
         } else {
             rec->data[0] = new capture{std::forward<Func>(f)};
             rec->free_data = [](function_record *r) { delete ((capture *) r->data[0]); };
         }
 
         /* Type casters for the function arguments and return value */
         using cast_in = argument_loader<Args...>;
@@ -464,21 +463,28 @@
             rec->sibling = PYBIND11_INSTANCE_METHOD_GET_FUNCTION(rec->sibling.ptr());
         }
 
         detail::function_record *chain = nullptr, *chain_start = rec;
         if (rec->sibling) {
             if (PyCFunction_Check(rec->sibling.ptr())) {
                 auto *self = PyCFunction_GET_SELF(rec->sibling.ptr());
-                capsule rec_capsule = isinstance<capsule>(self) ? reinterpret_borrow<capsule>(self)
-                                                                : capsule(self);
-                chain = (detail::function_record *) rec_capsule;
-                /* Never append a method to an overload chain of a parent class;
-                   instead, hide the parent's overloads in this case */
-                if (!chain->scope.is(rec->scope)) {
+                if (!isinstance<capsule>(self)) {
                     chain = nullptr;
+                } else {
+                    auto rec_capsule = reinterpret_borrow<capsule>(self);
+                    if (detail::is_function_record_capsule(rec_capsule)) {
+                        chain = rec_capsule.get_pointer<detail::function_record>();
+                        /* Never append a method to an overload chain of a parent class;
+                           instead, hide the parent's overloads in this case */
+                        if (!chain->scope.is(rec->scope)) {
+                            chain = nullptr;
+                        }
+                    } else {
+                        chain = nullptr;
+                    }
                 }
             }
             // Don't trigger for things like the default __init__, which are wrapper_descriptors
             // that we are intentionally replacing
             else if (!rec->sibling.is_none() && rec->name[0] != '_') {
                 pybind11_fail("Cannot overload existing non-function object \""
                               + std::string(rec->name) + "\" with a function of the same name");
@@ -492,14 +498,15 @@
             rec->def->ml_name = rec->name;
             rec->def->ml_meth
                 = reinterpret_cast<PyCFunction>(reinterpret_cast<void (*)()>(dispatcher));
             rec->def->ml_flags = METH_VARARGS | METH_KEYWORDS;
 
             capsule rec_capsule(unique_rec.release(),
                                 [](void *ptr) { destruct((detail::function_record *) ptr); });
+            rec_capsule.set_name(detail::get_function_record_capsule_name());
             guarded_strdup.release();
 
             object scope_module;
             if (rec->scope) {
                 if (hasattr(rec->scope, "__module__")) {
                     scope_module = rec->scope.attr("__module__");
                 } else if (hasattr(rec->scope, "__name__")) {
@@ -657,18 +664,21 @@
             rec = next;
         }
     }
 
     /// Main dispatch logic for calls to functions bound using pybind11
     static PyObject *dispatcher(PyObject *self, PyObject *args_in, PyObject *kwargs_in) {
         using namespace detail;
+        assert(isinstance<capsule>(self));
 
         /* Iterator over the list of potentially admissible overloads */
-        const function_record *overloads = (function_record *) PyCapsule_GetPointer(self, nullptr),
+        const function_record *overloads = reinterpret_cast<function_record *>(
+                                  PyCapsule_GetPointer(self, get_function_record_capsule_name())),
                               *it = overloads;
+        assert(overloads != nullptr);
 
         /* Need to know how many arguments + keyword arguments there are to pick the right
            overload */
         const auto n_args_in = (size_t) PyTuple_GET_SIZE(args_in);
 
         handle parent = n_args_in > 0 ? PyTuple_GET_ITEM(args_in, 0) : nullptr,
                result = PYBIND11_TRY_NEXT_OVERLOAD;
@@ -1412,17 +1422,17 @@
     void_t<decltype(static_cast<void (*)(void *, size_t)>(T::operator delete))>> : std::true_type {
 };
 /// Call class-specific delete if it exists or global otherwise. Can also be an overload set.
 template <typename T, enable_if_t<has_operator_delete<T>::value, int> = 0>
 void call_operator_delete(T *p, size_t, size_t) {
     T::operator delete(p);
 }
-template <
-    typename T,
-    enable_if_t<!has_operator_delete<T>::value && has_operator_delete_size<T>::value, int> = 0>
+template <typename T,
+          enable_if_t<!has_operator_delete<T>::value && has_operator_delete_size<T>::value, int>
+          = 0>
 void call_operator_delete(T *p, size_t s, size_t) {
     T::operator delete(p, s);
 }
 
 inline void call_operator_delete(void *p, size_t s, size_t a) {
     (void) s;
     (void) a;
@@ -1574,22 +1584,22 @@
                         sibling(getattr(*this, name_, none())),
                         extra...);
         auto cf_name = cf.name();
         attr(std::move(cf_name)) = staticmethod(std::move(cf));
         return *this;
     }
 
-    template <detail::op_id id, detail::op_type ot, typename L, typename R, typename... Extra>
-    class_ &def(const detail::op_<id, ot, L, R> &op, const Extra &...extra) {
+    template <typename T, typename... Extra, detail::enable_if_t<T::op_enable_if_hook, int> = 0>
+    class_ &def(const T &op, const Extra &...extra) {
         op.execute(*this, extra...);
         return *this;
     }
 
-    template <detail::op_id id, detail::op_type ot, typename L, typename R, typename... Extra>
-    class_ &def_cast(const detail::op_<id, ot, L, R> &op, const Extra &...extra) {
+    template <typename T, typename... Extra, detail::enable_if_t<T::op_enable_if_hook, int> = 0>
+    class_ &def_cast(const T &op, const Extra &...extra) {
         op.execute_cast(*this, extra...);
         return *this;
     }
 
     template <typename... Args, typename... Extra>
     class_ &def(const detail::initimpl::constructor<Args...> &init, const Extra &...extra) {
         PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(init);
@@ -1826,16 +1836,15 @@
     static void init_holder(detail::instance *inst,
                             detail::value_and_holder &v_h,
                             const holder_type *holder_ptr,
                             const void * /* dummy -- not enable_shared_from_this<T>) */) {
         if (holder_ptr) {
             init_holder_from_existing(v_h, holder_ptr, std::is_copy_constructible<holder_type>());
             v_h.set_holder_constructed();
-        } else if (PYBIND11_SILENCE_MSVC_C4127(detail::always_construct_holder<holder_type>::value)
-                   || inst->owned) {
+        } else if (detail::always_construct_holder<holder_type>::value || inst->owned) {
             new (std::addressof(v_h.holder<holder_type>())) holder_type(v_h.value_ptr<type>());
             v_h.set_holder_constructed();
         }
     }
 
     /// Performs instance initialization including constructing a holder and registering the known
     /// instance.  Should be called as soon as the `type` value_ptr is set for an instance.  Takes
@@ -1867,17 +1876,30 @@
                 v_h.value_ptr<type>(), v_h.type->type_size, v_h.type->type_align);
         }
         v_h.value_ptr() = nullptr;
     }
 
     static detail::function_record *get_function_record(handle h) {
         h = detail::get_function(h);
-        return h ? (detail::function_record *) reinterpret_borrow<capsule>(
-                   PyCFunction_GET_SELF(h.ptr()))
-                 : nullptr;
+        if (!h) {
+            return nullptr;
+        }
+
+        handle func_self = PyCFunction_GET_SELF(h.ptr());
+        if (!func_self) {
+            throw error_already_set();
+        }
+        if (!isinstance<capsule>(func_self)) {
+            return nullptr;
+        }
+        auto cap = reinterpret_borrow<capsule>(func_self);
+        if (!detail::is_function_record_capsule(cap)) {
+            return nullptr;
+        }
+        return cap.get_pointer<detail::function_record>();
     }
 };
 
 /// Binds an existing constructor taking arguments Args...
 template <typename... Args>
 detail::initimpl::constructor<Args...> init() {
     return {};
@@ -1946,37 +1968,43 @@
             [](handle arg) -> str {
                 object type_name = type::handle_of(arg).attr("__name__");
                 return pybind11::str("{}.{}").format(std::move(type_name), enum_name(arg));
             },
             name("name"),
             is_method(m_base));
 
-        m_base.attr("__doc__") = static_property(
-            cpp_function(
-                [](handle arg) -> std::string {
-                    std::string docstring;
-                    dict entries = arg.attr("__entries");
-                    if (((PyTypeObject *) arg.ptr())->tp_doc) {
-                        docstring += std::string(((PyTypeObject *) arg.ptr())->tp_doc) + "\n\n";
-                    }
-                    docstring += "Members:";
-                    for (auto kv : entries) {
-                        auto key = std::string(pybind11::str(kv.first));
-                        auto comment = kv.second[int_(1)];
-                        docstring += "\n\n  " + key;
-                        if (!comment.is_none()) {
-                            docstring += " : " + (std::string) pybind11::str(comment);
+        if (options::show_enum_members_docstring()) {
+            m_base.attr("__doc__") = static_property(
+                cpp_function(
+                    [](handle arg) -> std::string {
+                        std::string docstring;
+                        dict entries = arg.attr("__entries");
+                        if (((PyTypeObject *) arg.ptr())->tp_doc) {
+                            docstring += std::string(
+                                reinterpret_cast<PyTypeObject *>(arg.ptr())->tp_doc);
+                            docstring += "\n\n";
                         }
-                    }
-                    return docstring;
-                },
-                name("__doc__")),
-            none(),
-            none(),
-            "");
+                        docstring += "Members:";
+                        for (auto kv : entries) {
+                            auto key = std::string(pybind11::str(kv.first));
+                            auto comment = kv.second[int_(1)];
+                            docstring += "\n\n  ";
+                            docstring += key;
+                            if (!comment.is_none()) {
+                                docstring += " : ";
+                                docstring += pybind11::str(comment).cast<std::string>();
+                            }
+                        }
+                        return docstring;
+                    },
+                    name("__doc__")),
+                none(),
+                none(),
+                "");
+        }
 
         m_base.attr("__members__") = static_property(cpp_function(
                                                          [](handle arg) -> dict {
                                                              dict entries = arg.attr("__entries"),
                                                                   m;
                                                              for (auto kv : entries) {
                                                                  m[kv.first] = kv.second[int_(0)];
@@ -2069,15 +2097,15 @@
         str name(name_);
         if (entries.contains(name)) {
             std::string type_name = (std::string) str(m_base.attr("__name__"));
             throw value_error(std::move(type_name) + ": element \"" + std::string(name_)
                               + "\" already exists!");
         }
 
-        entries[name] = std::make_pair(value, doc);
+        entries[name] = pybind11::make_tuple(value, doc);
         m_base.attr(std::move(name)) = std::move(value);
     }
 
     PYBIND11_NOINLINE void export_values() {
         dict entries = m_base.attr("__entries");
         for (auto kv : entries) {
             m_parent.attr(kv.first) = kv.second[int_(0)];
@@ -2329,15 +2357,15 @@
 
 template <typename Access,
           return_value_policy Policy,
           typename Iterator,
           typename Sentinel,
           typename ValueType,
           typename... Extra>
-iterator make_iterator_impl(Iterator &&first, Sentinel &&last, Extra &&...extra) {
+iterator make_iterator_impl(Iterator first, Sentinel last, Extra &&...extra) {
     using state = detail::iterator_state<Access, Policy, Iterator, Sentinel, ValueType, Extra...>;
     // TODO: state captures only the types of Extra, not the values
 
     if (!detail::get_type_info(typeid(state), false)) {
         class_<state>(handle(), "iterator", pybind11::module_local())
             .def("__iter__", [](state &s) -> state & { return s; })
             .def(
@@ -2355,70 +2383,64 @@
                     return Access()(s.it);
                     // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
                 },
                 std::forward<Extra>(extra)...,
                 Policy);
     }
 
-    return cast(state{std::forward<Iterator>(first), std::forward<Sentinel>(last), true});
+    return cast(state{first, last, true});
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 /// Makes a python iterator from a first and past-the-end C++ InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
           typename ValueType = typename detail::iterator_access<Iterator>::result_type,
           typename... Extra>
-iterator make_iterator(Iterator &&first, Sentinel &&last, Extra &&...extra) {
+iterator make_iterator(Iterator first, Sentinel last, Extra &&...extra) {
     return detail::make_iterator_impl<detail::iterator_access<Iterator>,
                                       Policy,
                                       Iterator,
                                       Sentinel,
                                       ValueType,
-                                      Extra...>(std::forward<Iterator>(first),
-                                                std::forward<Sentinel>(last),
-                                                std::forward<Extra>(extra)...);
+                                      Extra...>(first, last, std::forward<Extra>(extra)...);
 }
 
 /// Makes a python iterator over the keys (`.first`) of a iterator over pairs from a
 /// first and past-the-end InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
           typename KeyType = typename detail::iterator_key_access<Iterator>::result_type,
           typename... Extra>
-iterator make_key_iterator(Iterator &&first, Sentinel &&last, Extra &&...extra) {
+iterator make_key_iterator(Iterator first, Sentinel last, Extra &&...extra) {
     return detail::make_iterator_impl<detail::iterator_key_access<Iterator>,
                                       Policy,
                                       Iterator,
                                       Sentinel,
                                       KeyType,
-                                      Extra...>(std::forward<Iterator>(first),
-                                                std::forward<Sentinel>(last),
-                                                std::forward<Extra>(extra)...);
+                                      Extra...>(first, last, std::forward<Extra>(extra)...);
 }
 
 /// Makes a python iterator over the values (`.second`) of a iterator over pairs from a
 /// first and past-the-end InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
           typename ValueType = typename detail::iterator_value_access<Iterator>::result_type,
           typename... Extra>
-iterator make_value_iterator(Iterator &&first, Sentinel &&last, Extra &&...extra) {
+iterator make_value_iterator(Iterator first, Sentinel last, Extra &&...extra) {
     return detail::make_iterator_impl<detail::iterator_value_access<Iterator>,
                                       Policy,
                                       Iterator,
                                       Sentinel,
                                       ValueType,
-                                      Extra...>(std::forward<Iterator>(first),
-                                                std::forward<Sentinel>(last),
-                                                std::forward<Extra>(extra)...);
+                                      Extra...>(first, last, std::forward<Extra>(extra)...);
 }
 
 /// Makes an iterator over values of an stl container or other container supporting
 /// `std::begin()`/`std::end()`
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Type,
           typename... Extra>
@@ -2854,11 +2876,7 @@
         PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), name, fn, __VA_ARGS__);
 #define PYBIND11_OVERLOAD(ret_type, cname, fn, ...)                                               \
     PYBIND11_OVERRIDE(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), fn, __VA_ARGS__)
 #define PYBIND11_OVERLOAD_PURE(ret_type, cname, fn, ...)                                          \
     PYBIND11_OVERRIDE_PURE(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), fn, __VA_ARGS__);
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
-
-#if defined(__GNUC__) && __GNUC__ == 7
-#    pragma GCC diagnostic pop // -Wnoexcept-type
-#endif
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/pytypes.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/pytypes.h`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 #ifdef PYBIND11_HAS_STRING_VIEW
 #    include <string_view>
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
+PYBIND11_WARNING_DISABLE_MSVC(4127)
+
 /* A few forward declarations */
 class handle;
 class object;
 class str;
 class iterator;
 class type;
 struct arg;
@@ -151,31 +153,31 @@
     bool operator<=(object_api const &other) const { return rich_compare(other, Py_LE); }
     bool operator>(object_api const &other) const { return rich_compare(other, Py_GT); }
     bool operator>=(object_api const &other) const { return rich_compare(other, Py_GE); }
 
     object operator-() const;
     object operator~() const;
     object operator+(object_api const &other) const;
-    object operator+=(object_api const &other) const;
+    object operator+=(object_api const &other);
     object operator-(object_api const &other) const;
-    object operator-=(object_api const &other) const;
+    object operator-=(object_api const &other);
     object operator*(object_api const &other) const;
-    object operator*=(object_api const &other) const;
+    object operator*=(object_api const &other);
     object operator/(object_api const &other) const;
-    object operator/=(object_api const &other) const;
+    object operator/=(object_api const &other);
     object operator|(object_api const &other) const;
-    object operator|=(object_api const &other) const;
+    object operator|=(object_api const &other);
     object operator&(object_api const &other) const;
-    object operator&=(object_api const &other) const;
+    object operator&=(object_api const &other);
     object operator^(object_api const &other) const;
-    object operator^=(object_api const &other) const;
+    object operator^=(object_api const &other);
     object operator<<(object_api const &other) const;
-    object operator<<=(object_api const &other) const;
+    object operator<<=(object_api const &other);
     object operator>>(object_api const &other) const;
-    object operator>>=(object_api const &other) const;
+    object operator>>=(object_api const &other);
 
     PYBIND11_DEPRECATED("Use py::str(obj) instead")
     pybind11::str str() const;
 
     /// Get or set the object's docstring, i.e. ``obj.__doc__``.
     str_attr_accessor doc() const;
 
@@ -226,15 +228,16 @@
 
     /// Enable implicit conversion through ``T::operator PyObject *()``.
     template <
         typename T,
         detail::enable_if_t<detail::all_of<detail::none_of<std::is_base_of<handle, T>,
                                                            detail::is_pyobj_ptr_or_nullptr_t<T>>,
                                            std::is_convertible<T, PyObject *>>::value,
-                            int> = 0>
+                            int>
+        = 0>
     // NOLINTNEXTLINE(google-explicit-constructor)
     handle(T &obj) : m_ptr(obj) {}
 
     /// Return the underlying ``PyObject *`` pointer
     PyObject *ptr() const { return m_ptr; }
     PyObject *&ptr() { return m_ptr; }
 
@@ -243,24 +246,34 @@
         preferable to use the `object` class which derives from `handle` and calls
         this function automatically. Returns a reference to itself.
     \endrst */
     const handle &inc_ref() const & {
 #ifdef PYBIND11_HANDLE_REF_DEBUG
         inc_ref_counter(1);
 #endif
+#ifdef PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
+        if (m_ptr != nullptr && !PyGILState_Check()) {
+            throw_gilstate_error("pybind11::handle::inc_ref()");
+        }
+#endif
         Py_XINCREF(m_ptr);
         return *this;
     }
 
     /** \rst
         Manually decrease the reference count of the Python object. Usually, it is
         preferable to use the `object` class which derives from `handle` and calls
         this function automatically. Returns a reference to itself.
     \endrst */
     const handle &dec_ref() const & {
+#ifdef PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
+        if (m_ptr != nullptr && !PyGILState_Check()) {
+            throw_gilstate_error("pybind11::handle::dec_ref()");
+        }
+#endif
         Py_XDECREF(m_ptr);
         return *this;
     }
 
     /** \rst
         Attempt to cast the Python object into the given C++ type. A `cast_error`
         will be throw upon failure.
@@ -279,16 +292,36 @@
     bool operator!=(const handle &h) const { return m_ptr != h.m_ptr; }
     PYBIND11_DEPRECATED("Use handle::operator bool() instead")
     bool check() const { return m_ptr != nullptr; }
 
 protected:
     PyObject *m_ptr = nullptr;
 
-#ifdef PYBIND11_HANDLE_REF_DEBUG
 private:
+#ifdef PYBIND11_ASSERT_GIL_HELD_INCREF_DECREF
+    void throw_gilstate_error(const std::string &function_name) const {
+        fprintf(
+            stderr,
+            "%s is being called while the GIL is either not held or invalid. Please see "
+            "https://pybind11.readthedocs.io/en/stable/advanced/"
+            "misc.html#common-sources-of-global-interpreter-lock-errors for debugging advice.\n",
+            function_name.c_str());
+        fflush(stderr);
+        if (Py_TYPE(m_ptr)->tp_name != nullptr) {
+            fprintf(stderr,
+                    "The failing %s call was triggered on a %s object.\n",
+                    function_name.c_str(),
+                    Py_TYPE(m_ptr)->tp_name);
+            fflush(stderr);
+        }
+        throw std::runtime_error(function_name + " PyGILState_Check() failure.");
+    }
+#endif
+
+#ifdef PYBIND11_HANDLE_REF_DEBUG
     static std::size_t inc_ref_counter(std::size_t add) {
         thread_local std::size_t counter = 0;
         counter += add;
         return counter;
     }
 
 public:
@@ -330,33 +363,50 @@
     handle release() {
         PyObject *tmp = m_ptr;
         m_ptr = nullptr;
         return handle(tmp);
     }
 
     object &operator=(const object &other) {
-        other.inc_ref();
-        // Use temporary variable to ensure `*this` remains valid while
-        // `Py_XDECREF` executes, in case `*this` is accessible from Python.
-        handle temp(m_ptr);
-        m_ptr = other.m_ptr;
-        temp.dec_ref();
+        // Skip inc_ref and dec_ref if both objects are the same
+        if (!this->is(other)) {
+            other.inc_ref();
+            // Use temporary variable to ensure `*this` remains valid while
+            // `Py_XDECREF` executes, in case `*this` is accessible from Python.
+            handle temp(m_ptr);
+            m_ptr = other.m_ptr;
+            temp.dec_ref();
+        }
         return *this;
     }
 
     object &operator=(object &&other) noexcept {
         if (this != &other) {
             handle temp(m_ptr);
             m_ptr = other.m_ptr;
             other.m_ptr = nullptr;
             temp.dec_ref();
         }
         return *this;
     }
 
+#define PYBIND11_INPLACE_OP(iop)                                                                  \
+    object iop(object_api const &other) { return operator=(handle::iop(other)); }
+
+    PYBIND11_INPLACE_OP(operator+=)
+    PYBIND11_INPLACE_OP(operator-=)
+    PYBIND11_INPLACE_OP(operator*=)
+    PYBIND11_INPLACE_OP(operator/=)
+    PYBIND11_INPLACE_OP(operator|=)
+    PYBIND11_INPLACE_OP(operator&=)
+    PYBIND11_INPLACE_OP(operator^=)
+    PYBIND11_INPLACE_OP(operator<<=)
+    PYBIND11_INPLACE_OP(operator>>=)
+#undef PYBIND11_INPLACE_OP
+
     // Calling cast() on an object lvalue just copies (via handle::cast)
     template <typename T>
     T cast() const &;
     // Calling on an object rvalue does a move, if needed and/or possible
     template <typename T>
     T cast() &&;
 
@@ -409,15 +459,15 @@
     return {h, object::stolen_t{}};
 }
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 // Equivalent to obj.__class__.__name__ (or obj.__name__ if obj is a class).
 inline const char *obj_class_name(PyObject *obj) {
-    if (Py_TYPE(obj) == &PyType_Type) {
+    if (PyType_Check(obj)) {
         return reinterpret_cast<PyTypeObject *>(obj)->tp_name;
     }
     return Py_TYPE(obj)->tp_name;
 }
 
 std::string error_string();
 
@@ -447,45 +497,70 @@
         PyErr_NormalizeException(&m_type.ptr(), &m_value.ptr(), &m_trace.ptr());
         if (m_type.ptr() == nullptr) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " failed to normalize the "
                             "active exception.");
         }
         const char *exc_type_name_norm = detail::obj_class_name(m_type.ptr());
-        if (exc_type_name_orig == nullptr) {
+        if (exc_type_name_norm == nullptr) {
             pybind11_fail("Internal error: " + std::string(called)
                           + " failed to obtain the name "
                             "of the normalized active exception type.");
         }
+#if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x07030a00
+        // This behavior runs the risk of masking errors in the error handling, but avoids a
+        // conflict with PyPy, which relies on the normalization here to change OSError to
+        // FileNotFoundError (https://github.com/pybind/pybind11/issues/4075).
+        m_lazy_error_string = exc_type_name_norm;
+#else
         if (exc_type_name_norm != m_lazy_error_string) {
             std::string msg = std::string(called)
                               + ": MISMATCH of original and normalized "
                                 "active exception types: ";
             msg += "ORIGINAL ";
             msg += m_lazy_error_string;
             msg += " REPLACED BY ";
             msg += exc_type_name_norm;
             msg += ": " + format_value_and_trace();
             pybind11_fail(msg);
         }
+#endif
     }
 
     error_fetch_and_normalize(const error_fetch_and_normalize &) = delete;
     error_fetch_and_normalize(error_fetch_and_normalize &&) = delete;
 
     std::string format_value_and_trace() const {
         std::string result;
         std::string message_error_string;
         if (m_value) {
             auto value_str = reinterpret_steal<object>(PyObject_Str(m_value.ptr()));
+            constexpr const char *message_unavailable_exc
+                = "<MESSAGE UNAVAILABLE DUE TO ANOTHER EXCEPTION>";
             if (!value_str) {
                 message_error_string = detail::error_string();
-                result = "<MESSAGE UNAVAILABLE DUE TO ANOTHER EXCEPTION>";
+                result = message_unavailable_exc;
             } else {
-                result = value_str.cast<std::string>();
+                // Not using `value_str.cast<std::string>()`, to not potentially throw a secondary
+                // error_already_set that will then result in process termination (#4288).
+                auto value_bytes = reinterpret_steal<object>(
+                    PyUnicode_AsEncodedString(value_str.ptr(), "utf-8", "backslashreplace"));
+                if (!value_bytes) {
+                    message_error_string = detail::error_string();
+                    result = message_unavailable_exc;
+                } else {
+                    char *buffer = nullptr;
+                    Py_ssize_t length = 0;
+                    if (PyBytes_AsStringAndSize(value_bytes.ptr(), &buffer, &length) == -1) {
+                        message_error_string = detail::error_string();
+                        result = message_unavailable_exc;
+                    } else {
+                        result = std::string(buffer, static_cast<std::size_t>(length));
+                    }
+                }
             }
         } else {
             result = "<MESSAGE UNAVAILABLE>";
         }
         if (result.empty()) {
             result = "<EMPTY MESSAGE>";
         }
@@ -577,20 +652,14 @@
 
 inline std::string error_string() {
     return error_fetch_and_normalize("pybind11::detail::error_string").error_string();
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
-#if defined(_MSC_VER)
-#    pragma warning(push)
-#    pragma warning(disable : 4275 4251)
-//     warning C4275: An exported class was derived from a class that wasn't exported.
-//     Can be ignored when derived from a STL class.
-#endif
 /// Fetch and hold an error which was already set in Python.  An instance of this is typically
 /// thrown to propagate python-side errors back through C++ which can either be caught manually or
 /// else falls back to the function dispatcher (which then raises the captured error back to
 /// python).
 class PYBIND11_EXPORT_EXCEPTION error_already_set : public std::exception {
 public:
     /// Fetches the current Python exception (using PyErr_Fetch()), which will clear the
@@ -642,17 +711,14 @@
 private:
     std::shared_ptr<detail::error_fetch_and_normalize> m_fetched_error;
 
     /// WARNING: This custom deleter needs to acquire the Python GIL. This can lead to
     ///          crashes (undefined behavior) if the Python interpreter is finalizing.
     static void m_fetched_error_deleter(detail::error_fetch_and_normalize *raw_ptr);
 };
-#if defined(_MSC_VER)
-#    pragma warning(pop)
-#endif
 
 /// Replaces the current Python error indicator with the chosen error, performing a
 /// 'raise from' to indicate that the chosen error was caused by the original error.
 inline void raise_from(PyObject *type, const char *message) {
     // Based on _PyErr_FormatVFromCause:
     // https://github.com/python/cpython/blob/467ab194fc6189d9f7310c89937c51abeac56839/Python/errors.c#L405
     // See https://github.com/pybind/pybind11/pull/2112 for details.
@@ -847,18 +913,16 @@
 }
 // The following casting version is implemented in cast.h:
 template <typename T, enable_if_t<!is_pyobject<T>::value, int> = 0>
 object object_or_cast(T &&o);
 // Match a PyObject*, which we want to convert directly to handle via its converting constructor
 inline handle object_or_cast(PyObject *ptr) { return ptr; }
 
-#if defined(_MSC_VER) && _MSC_VER < 1920
-#    pragma warning(push)
-#    pragma warning(disable : 4522) // warning C4522: multiple assignment operators specified
-#endif
+PYBIND11_WARNING_PUSH
+PYBIND11_WARNING_DISABLE_MSVC(4522) // warning C4522: multiple assignment operators specified
 template <typename Policy>
 class accessor : public object_api<accessor<Policy>> {
     using key_type = typename Policy::key_type;
 
 public:
     accessor(handle obj, key_type key) : obj(obj), key(std::move(key)) {}
     accessor(const accessor &) = default;
@@ -914,17 +978,15 @@
     }
 
 private:
     handle obj;
     key_type key;
     mutable object cache;
 };
-#if defined(_MSC_VER) && _MSC_VER < 1920
-#    pragma warning(pop)
-#endif
+PYBIND11_WARNING_POP
 
 PYBIND11_NAMESPACE_BEGIN(accessor_policies)
 struct obj_attr {
     using key_type = object;
     static object get(handle obj, handle key) { return getattr(obj, key); }
     static void set(handle obj, handle key, handle val) { setattr(obj, key, val); }
 };
@@ -1262,15 +1324,15 @@
     Name(object &&o) : Parent(check_(o) ? o.release().ptr() : ConvertFun(o.ptr()), stolen_t{}) {  \
         if (!m_ptr)                                                                               \
             throw ::pybind11::error_already_set();                                                \
     }
 
 #define PYBIND11_OBJECT_CVT_DEFAULT(Name, Parent, CheckFun, ConvertFun)                           \
     PYBIND11_OBJECT_CVT(Name, Parent, CheckFun, ConvertFun)                                       \
-    Name() : Parent() {}
+    Name() = default;
 
 #define PYBIND11_OBJECT_CHECK_FAILED(Name, o_ptr)                                                 \
     ::pybind11::type_error("Object of type '"                                                     \
                            + ::pybind11::detail::get_fully_qualified_tp_name(Py_TYPE(o_ptr))      \
                            + "' is not an instance of '" #Name "'")
 
 #define PYBIND11_OBJECT(Name, Parent, CheckFun)                                                   \
@@ -1285,15 +1347,15 @@
     Name(object &&o) : Parent(std::move(o)) {                                                     \
         if (m_ptr && !check_(m_ptr))                                                              \
             throw PYBIND11_OBJECT_CHECK_FAILED(Name, m_ptr);                                      \
     }
 
 #define PYBIND11_OBJECT_DEFAULT(Name, Parent, CheckFun)                                           \
     PYBIND11_OBJECT(Name, Parent, CheckFun)                                                       \
-    Name() : Parent() {}
+    Name() = default;
 
 /// \addtogroup pytypes
 /// @{
 
 /** \rst
     Wraps a Python iterator so that it can also be used as a C++ input iterator
 
@@ -1354,15 +1416,15 @@
 
     friend bool operator==(const iterator &a, const iterator &b) { return a->ptr() == b->ptr(); }
     friend bool operator!=(const iterator &a, const iterator &b) { return a->ptr() != b->ptr(); }
 
 private:
     void advance() {
         value = reinterpret_steal<object>(PyIter_Next(m_ptr));
-        if (PyErr_Occurred()) {
+        if (value.ptr() == nullptr && PyErr_Occurred()) {
             throw error_already_set();
         }
     }
 
 private:
     object value = {};
 };
@@ -1404,23 +1466,29 @@
 public:
     PYBIND11_OBJECT_CVT(str, object, PYBIND11_STR_CHECK_FUN, raw_str)
 
     template <typename SzType, detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
     str(const char *c, const SzType &n)
         : object(PyUnicode_FromStringAndSize(c, ssize_t_cast(n)), stolen_t{}) {
         if (!m_ptr) {
+            if (PyErr_Occurred()) {
+                throw error_already_set();
+            }
             pybind11_fail("Could not allocate string object!");
         }
     }
 
     // 'explicit' is explicitly omitted from the following constructors to allow implicit
     // conversion to py::str from C++ string-like objects
     // NOLINTNEXTLINE(google-explicit-constructor)
     str(const char *c = "") : object(PyUnicode_FromString(c), stolen_t{}) {
         if (!m_ptr) {
+            if (PyErr_Occurred()) {
+                throw error_already_set();
+            }
             pybind11_fail("Could not allocate string object!");
         }
     }
 
     // NOLINTNEXTLINE(google-explicit-constructor)
     str(const std::string &s) : str(s.data(), s.size()) {}
 
@@ -1570,14 +1638,17 @@
     char *buffer = nullptr;
     ssize_t length = 0;
     if (PyBytes_AsStringAndSize(b.ptr(), &buffer, &length) != 0) {
         throw error_already_set();
     }
     auto obj = reinterpret_steal<object>(PyUnicode_FromStringAndSize(buffer, length));
     if (!obj) {
+        if (PyErr_Occurred()) {
+            throw error_already_set();
+        }
         pybind11_fail("Could not allocate string object!");
     }
     m_ptr = obj.release().ptr();
 }
 
 /// \addtogroup pytypes
 /// @{
@@ -1647,15 +1718,15 @@
 PYBIND11_NAMESPACE_BEGIN(detail)
 // Converts a value to the given unsigned type.  If an error occurs, you get back (Unsigned) -1;
 // otherwise you get back the unsigned long or unsigned long long value cast to (Unsigned).
 // (The distinction is critically important when casting a returned -1 error value to some other
 // unsigned type: (A)-1 != (B)-1 when A and B are unsigned types of different sizes).
 template <typename Unsigned>
 Unsigned as_unsigned(PyObject *o) {
-    if (PYBIND11_SILENCE_MSVC_C4127(sizeof(Unsigned) <= sizeof(unsigned long))) {
+    if (sizeof(Unsigned) <= sizeof(unsigned long)) {
         unsigned long v = PyLong_AsUnsignedLong(o);
         return v == (unsigned long) -1 && PyErr_Occurred() ? (Unsigned) -1 : (Unsigned) v;
     }
     unsigned long long v = PyLong_AsUnsignedLongLong(o);
     return v == (unsigned long long) -1 && PyErr_Occurred() ? (Unsigned) -1 : (Unsigned) v;
 }
 PYBIND11_NAMESPACE_END(detail)
@@ -1664,15 +1735,15 @@
 public:
     PYBIND11_OBJECT_CVT(int_, object, PYBIND11_LONG_CHECK, PyNumber_Long)
     int_() : object(PyLong_FromLong(0), stolen_t{}) {}
     // Allow implicit conversion from C++ integral types:
     template <typename T, detail::enable_if_t<std::is_integral<T>::value, int> = 0>
     // NOLINTNEXTLINE(google-explicit-constructor)
     int_(T value) {
-        if (PYBIND11_SILENCE_MSVC_C4127(sizeof(T) <= sizeof(long))) {
+        if (sizeof(T) <= sizeof(long)) {
             if (std::is_signed<T>::value) {
                 m_ptr = PyLong_FromLong((long) value);
             } else {
                 m_ptr = PyLong_FromUnsignedLong((unsigned long) value);
             }
         } else {
             if (std::is_signed<T>::value) {
@@ -1781,49 +1852,49 @@
     PYBIND11_OBJECT_DEFAULT(capsule, object, PyCapsule_CheckExact)
     PYBIND11_DEPRECATED("Use reinterpret_borrow<capsule>() or reinterpret_steal<capsule>()")
     capsule(PyObject *ptr, bool is_borrowed)
         : object(is_borrowed ? object(ptr, borrowed_t{}) : object(ptr, stolen_t{})) {}
 
     explicit capsule(const void *value,
                      const char *name = nullptr,
-                     void (*destructor)(PyObject *) = nullptr)
+                     PyCapsule_Destructor destructor = nullptr)
         : object(PyCapsule_New(const_cast<void *>(value), name, destructor), stolen_t{}) {
         if (!m_ptr) {
             throw error_already_set();
         }
     }
 
-    PYBIND11_DEPRECATED("Please pass a destructor that takes a void pointer as input")
-    capsule(const void *value, void (*destruct)(PyObject *))
-        : object(PyCapsule_New(const_cast<void *>(value), nullptr, destruct), stolen_t{}) {
+    PYBIND11_DEPRECATED("Please use the ctor with value, name, destructor args")
+    capsule(const void *value, PyCapsule_Destructor destructor)
+        : object(PyCapsule_New(const_cast<void *>(value), nullptr, destructor), stolen_t{}) {
         if (!m_ptr) {
             throw error_already_set();
         }
     }
 
     capsule(const void *value, void (*destructor)(void *)) {
         m_ptr = PyCapsule_New(const_cast<void *>(value), nullptr, [](PyObject *o) {
             // guard if destructor called while err indicator is set
             error_scope error_guard;
             auto destructor = reinterpret_cast<void (*)(void *)>(PyCapsule_GetContext(o));
-            if (destructor == nullptr) {
-                if (PyErr_Occurred()) {
-                    throw error_already_set();
-                }
-                pybind11_fail("Unable to get capsule context");
+            if (destructor == nullptr && PyErr_Occurred()) {
+                throw error_already_set();
             }
             const char *name = get_name_in_error_scope(o);
             void *ptr = PyCapsule_GetPointer(o, name);
             if (ptr == nullptr) {
                 throw error_already_set();
             }
-            destructor(ptr);
+
+            if (destructor != nullptr) {
+                destructor(ptr);
+            }
         });
 
-        if (!m_ptr || PyCapsule_SetContext(m_ptr, (void *) destructor) != 0) {
+        if (!m_ptr || PyCapsule_SetContext(m_ptr, reinterpret_cast<void *>(destructor)) != 0) {
             throw error_already_set();
         }
     }
 
     explicit capsule(void (*destructor)()) {
         m_ptr = PyCapsule_New(reinterpret_cast<void *>(destructor), nullptr, [](PyObject *o) {
             const char *name = get_name_in_error_scope(o);
@@ -1939,15 +2010,19 @@
     size_t size() const { return (size_t) PyDict_Size(m_ptr); }
     bool empty() const { return size() == 0; }
     detail::dict_iterator begin() const { return {*this, 0}; }
     detail::dict_iterator end() const { return {}; }
     void clear() /* py-non-const */ { PyDict_Clear(ptr()); }
     template <typename T>
     bool contains(T &&key) const {
-        return PyDict_Contains(m_ptr, detail::object_or_cast(std::forward<T>(key)).ptr()) == 1;
+        auto result = PyDict_Contains(m_ptr, detail::object_or_cast(std::forward<T>(key)).ptr());
+        if (result == -1) {
+            throw error_already_set();
+        }
+        return result == 1;
     }
 
 private:
     /// Call the `dict` Python type -- always returns a new reference
     static PyObject *raw_dict(PyObject *op) {
         if (PyDict_Check(op)) {
             return handle(op).inc_ref().ptr();
@@ -1994,22 +2069,28 @@
     detail::item_accessor operator[](T &&o) const {
         return object::operator[](std::forward<T>(o));
     }
     detail::list_iterator begin() const { return {*this, 0}; }
     detail::list_iterator end() const { return {*this, PyList_GET_SIZE(m_ptr)}; }
     template <typename T>
     void append(T &&val) /* py-non-const */ {
-        PyList_Append(m_ptr, detail::object_or_cast(std::forward<T>(val)).ptr());
+        if (PyList_Append(m_ptr, detail::object_or_cast(std::forward<T>(val)).ptr()) != 0) {
+            throw error_already_set();
+        }
     }
     template <typename IdxType,
               typename ValType,
               detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
     void insert(const IdxType &index, ValType &&val) /* py-non-const */ {
-        PyList_Insert(
-            m_ptr, ssize_t_cast(index), detail::object_or_cast(std::forward<ValType>(val)).ptr());
+        if (PyList_Insert(m_ptr,
+                          ssize_t_cast(index),
+                          detail::object_or_cast(std::forward<ValType>(val)).ptr())
+            != 0) {
+            throw error_already_set();
+        }
     }
 };
 
 class args : public tuple {
     PYBIND11_OBJECT_DEFAULT(args, tuple, PyTuple_Check)
 };
 class kwargs : public dict {
@@ -2019,15 +2100,19 @@
 class anyset : public object {
 public:
     PYBIND11_OBJECT(anyset, object, PyAnySet_Check)
     size_t size() const { return static_cast<size_t>(PySet_Size(m_ptr)); }
     bool empty() const { return size() == 0; }
     template <typename T>
     bool contains(T &&val) const {
-        return PySet_Contains(m_ptr, detail::object_or_cast(std::forward<T>(val)).ptr()) == 1;
+        auto result = PySet_Contains(m_ptr, detail::object_or_cast(std::forward<T>(val)).ptr());
+        if (result == -1) {
+            throw error_already_set();
+        }
+        return result == 1;
     }
 };
 
 class set : public anyset {
 public:
     PYBIND11_OBJECT_CVT(set, anyset, PySet_Check, PySet_New)
     set() : anyset(PySet_New(nullptr), stolen_t{}) {
@@ -2360,33 +2445,43 @@
     object object_api<D>::op(object_api const &other) const {                                     \
         object result = reinterpret_steal<object>(fn(derived().ptr(), other.derived().ptr()));    \
         if (!result.ptr())                                                                        \
             throw error_already_set();                                                            \
         return result;                                                                            \
     }
 
+#define PYBIND11_MATH_OPERATOR_BINARY_INPLACE(iop, fn)                                            \
+    template <typename D>                                                                         \
+    object object_api<D>::iop(object_api const &other) {                                          \
+        object result = reinterpret_steal<object>(fn(derived().ptr(), other.derived().ptr()));    \
+        if (!result.ptr())                                                                        \
+            throw error_already_set();                                                            \
+        return result;                                                                            \
+    }
+
 PYBIND11_MATH_OPERATOR_UNARY(operator~, PyNumber_Invert)
 PYBIND11_MATH_OPERATOR_UNARY(operator-, PyNumber_Negative)
 PYBIND11_MATH_OPERATOR_BINARY(operator+, PyNumber_Add)
-PYBIND11_MATH_OPERATOR_BINARY(operator+=, PyNumber_InPlaceAdd)
+PYBIND11_MATH_OPERATOR_BINARY_INPLACE(operator+=, PyNumber_InPlaceAdd)
 PYBIND11_MATH_OPERATOR_BINARY(operator-, PyNumber_Subtract)
-PYBIND11_MATH_OPERATOR_BINARY(operator-=, PyNumber_InPlaceSubtract)
+PYBIND11_MATH_OPERATOR_BINARY_INPLACE(operator-=, PyNumber_InPlaceSubtract)
 PYBIND11_MATH_OPERATOR_BINARY(operator*, PyNumber_Multiply)
-PYBIND11_MATH_OPERATOR_BINARY(operator*=, PyNumber_InPlaceMultiply)
+PYBIND11_MATH_OPERATOR_BINARY_INPLACE(operator*=, PyNumber_InPlaceMultiply)
 PYBIND11_MATH_OPERATOR_BINARY(operator/, PyNumber_TrueDivide)
-PYBIND11_MATH_OPERATOR_BINARY(operator/=, PyNumber_InPlaceTrueDivide)
+PYBIND11_MATH_OPERATOR_BINARY_INPLACE(operator/=, PyNumber_InPlaceTrueDivide)
 PYBIND11_MATH_OPERATOR_BINARY(operator|, PyNumber_Or)
-PYBIND11_MATH_OPERATOR_BINARY(operator|=, PyNumber_InPlaceOr)
+PYBIND11_MATH_OPERATOR_BINARY_INPLACE(operator|=, PyNumber_InPlaceOr)
 PYBIND11_MATH_OPERATOR_BINARY(operator&, PyNumber_And)
-PYBIND11_MATH_OPERATOR_BINARY(operator&=, PyNumber_InPlaceAnd)
+PYBIND11_MATH_OPERATOR_BINARY_INPLACE(operator&=, PyNumber_InPlaceAnd)
 PYBIND11_MATH_OPERATOR_BINARY(operator^, PyNumber_Xor)
-PYBIND11_MATH_OPERATOR_BINARY(operator^=, PyNumber_InPlaceXor)
+PYBIND11_MATH_OPERATOR_BINARY_INPLACE(operator^=, PyNumber_InPlaceXor)
 PYBIND11_MATH_OPERATOR_BINARY(operator<<, PyNumber_Lshift)
-PYBIND11_MATH_OPERATOR_BINARY(operator<<=, PyNumber_InPlaceLshift)
+PYBIND11_MATH_OPERATOR_BINARY_INPLACE(operator<<=, PyNumber_InPlaceLshift)
 PYBIND11_MATH_OPERATOR_BINARY(operator>>, PyNumber_Rshift)
-PYBIND11_MATH_OPERATOR_BINARY(operator>>=, PyNumber_InPlaceRshift)
+PYBIND11_MATH_OPERATOR_BINARY_INPLACE(operator>>=, PyNumber_InPlaceRshift)
 
 #undef PYBIND11_MATH_OPERATOR_UNARY
 #undef PYBIND11_MATH_OPERATOR_BINARY
+#undef PYBIND11_MATH_OPERATOR_BINARY_INPLACE
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/stl/filesystem.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/stl.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/stl.h`

 * *Files 6% similar despite different names*

```diff
@@ -41,29 +41,43 @@
 using forwarded_type = conditional_t<std::is_lvalue_reference<T>::value,
                                      remove_reference_t<U> &,
                                      remove_reference_t<U> &&>;
 
 /// Forwards a value U as rvalue or lvalue according to whether T is rvalue or lvalue; typically
 /// used for forwarding a container's elements.
 template <typename T, typename U>
-forwarded_type<T, U> forward_like(U &&u) {
+constexpr forwarded_type<T, U> forward_like(U &&u) {
     return std::forward<detail::forwarded_type<T, U>>(std::forward<U>(u));
 }
 
+// Checks if a container has a STL style reserve method.
+// This will only return true for a `reserve()` with a `void` return.
+template <typename C>
+using has_reserve_method = std::is_same<decltype(std::declval<C>().reserve(0)), void>;
+
 template <typename Type, typename Key>
 struct set_caster {
     using type = Type;
     using key_conv = make_caster<Key>;
 
+private:
+    template <typename T = Type, enable_if_t<has_reserve_method<T>::value, int> = 0>
+    void reserve_maybe(const anyset &s, Type *) {
+        value.reserve(s.size());
+    }
+    void reserve_maybe(const anyset &, void *) {}
+
+public:
     bool load(handle src, bool convert) {
         if (!isinstance<anyset>(src)) {
             return false;
         }
         auto s = reinterpret_borrow<anyset>(src);
         value.clear();
+        reserve_maybe(s, &value);
         for (auto entry : s) {
             key_conv conv;
             if (!conv.load(entry, convert)) {
                 return false;
             }
             value.insert(cast_op<Key &&>(std::move(conv)));
         }
@@ -74,15 +88,15 @@
     static handle cast(T &&src, return_value_policy policy, handle parent) {
         if (!std::is_lvalue_reference<T>::value) {
             policy = return_value_policy_override<Key>::policy(policy);
         }
         pybind11::set s;
         for (auto &&value : src) {
             auto value_ = reinterpret_steal<object>(
-                key_conv::cast(forward_like<T>(value), policy, parent));
+                key_conv::cast(detail::forward_like<T>(value), policy, parent));
             if (!value_ || !s.add(std::move(value_))) {
                 return handle();
             }
         }
         return s.release();
     }
 
@@ -90,20 +104,29 @@
 };
 
 template <typename Type, typename Key, typename Value>
 struct map_caster {
     using key_conv = make_caster<Key>;
     using value_conv = make_caster<Value>;
 
+private:
+    template <typename T = Type, enable_if_t<has_reserve_method<T>::value, int> = 0>
+    void reserve_maybe(const dict &d, Type *) {
+        value.reserve(d.size());
+    }
+    void reserve_maybe(const dict &, void *) {}
+
+public:
     bool load(handle src, bool convert) {
         if (!isinstance<dict>(src)) {
             return false;
         }
         auto d = reinterpret_borrow<dict>(src);
         value.clear();
+        reserve_maybe(d, &value);
         for (auto it : d) {
             key_conv kconv;
             value_conv vconv;
             if (!kconv.load(it.first.ptr(), convert) || !vconv.load(it.second.ptr(), convert)) {
                 return false;
             }
             value.emplace(cast_op<Key &&>(std::move(kconv)), cast_op<Value &&>(std::move(vconv)));
@@ -118,17 +141,17 @@
         return_value_policy policy_value = policy;
         if (!std::is_lvalue_reference<T>::value) {
             policy_key = return_value_policy_override<Key>::policy(policy_key);
             policy_value = return_value_policy_override<Value>::policy(policy_value);
         }
         for (auto &&kv : src) {
             auto key = reinterpret_steal<object>(
-                key_conv::cast(forward_like<T>(kv.first), policy_key, parent));
+                key_conv::cast(detail::forward_like<T>(kv.first), policy_key, parent));
             auto value = reinterpret_steal<object>(
-                value_conv::cast(forward_like<T>(kv.second), policy_value, parent));
+                value_conv::cast(detail::forward_like<T>(kv.second), policy_value, parent));
             if (!key || !value) {
                 return handle();
             }
             d[std::move(key)] = std::move(value);
         }
         return d.release();
     }
@@ -156,17 +179,15 @@
             }
             value.push_back(cast_op<Value &&>(std::move(conv)));
         }
         return true;
     }
 
 private:
-    template <
-        typename T = Type,
-        enable_if_t<std::is_same<decltype(std::declval<T>().reserve(0)), void>::value, int> = 0>
+    template <typename T = Type, enable_if_t<has_reserve_method<T>::value, int> = 0>
     void reserve_maybe(const sequence &s, Type *) {
         value.reserve(s.size());
     }
     void reserve_maybe(const sequence &, void *) {}
 
 public:
     template <typename T>
@@ -174,15 +195,15 @@
         if (!std::is_lvalue_reference<T>::value) {
             policy = return_value_policy_override<Value>::policy(policy);
         }
         list l(src.size());
         ssize_t index = 0;
         for (auto &&value : src) {
             auto value_ = reinterpret_steal<object>(
-                value_conv::cast(forward_like<T>(value), policy, parent));
+                value_conv::cast(detail::forward_like<T>(value), policy, parent));
             if (!value_) {
                 return handle();
             }
             PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
@@ -238,15 +259,15 @@
 
     template <typename T>
     static handle cast(T &&src, return_value_policy policy, handle parent) {
         list l(src.size());
         ssize_t index = 0;
         for (auto &&value : src) {
             auto value_ = reinterpret_steal<object>(
-                value_conv::cast(forward_like<T>(value), policy, parent));
+                value_conv::cast(detail::forward_like<T>(value), policy, parent));
             if (!value_) {
                 return handle();
             }
             PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
@@ -286,15 +307,15 @@
 template <typename Type, typename Value = typename Type::value_type>
 struct optional_caster {
     using value_conv = make_caster<Value>;
 
     template <typename T>
     static handle cast(T &&src, return_value_policy policy, handle parent) {
         if (!src) {
-            return none().inc_ref();
+            return none().release();
         }
         if (!std::is_lvalue_reference<T>::value) {
             policy = return_value_policy_override<Value>::policy(policy);
         }
         return value_conv::cast(*std::forward<T>(src), policy, parent);
     }
```

### Comparing `xcsf-1.2.8/lib/pybind11/include/pybind11/stl_bind.h` & `xcsf-1.2.9/lib/pybind11/include/pybind11/stl_bind.h`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,21 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "detail/common.h"
+#include "detail/type_caster_base.h"
+#include "cast.h"
 #include "operators.h"
 
 #include <algorithm>
 #include <sstream>
+#include <type_traits>
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 /* SFINAE helper class used by 'is_comparable */
 template <typename T>
 struct container_traits {
@@ -632,57 +635,138 @@
             }
             s << '}';
             return s.str();
         },
         "Return the canonical string representation of this map.");
 }
 
-template <typename Map>
+template <typename KeyType>
 struct keys_view {
-    Map &map;
+    virtual size_t len() = 0;
+    virtual iterator iter() = 0;
+    virtual bool contains(const KeyType &k) = 0;
+    virtual bool contains(const object &k) = 0;
+    virtual ~keys_view() = default;
 };
 
-template <typename Map>
+template <typename MappedType>
 struct values_view {
-    Map &map;
+    virtual size_t len() = 0;
+    virtual iterator iter() = 0;
+    virtual ~values_view() = default;
 };
 
-template <typename Map>
+template <typename KeyType, typename MappedType>
 struct items_view {
+    virtual size_t len() = 0;
+    virtual iterator iter() = 0;
+    virtual ~items_view() = default;
+};
+
+template <typename Map, typename KeysView>
+struct KeysViewImpl : public KeysView {
+    explicit KeysViewImpl(Map &map) : map(map) {}
+    size_t len() override { return map.size(); }
+    iterator iter() override { return make_key_iterator(map.begin(), map.end()); }
+    bool contains(const typename Map::key_type &k) override { return map.find(k) != map.end(); }
+    bool contains(const object &) override { return false; }
+    Map &map;
+};
+
+template <typename Map, typename ValuesView>
+struct ValuesViewImpl : public ValuesView {
+    explicit ValuesViewImpl(Map &map) : map(map) {}
+    size_t len() override { return map.size(); }
+    iterator iter() override { return make_value_iterator(map.begin(), map.end()); }
+    Map &map;
+};
+
+template <typename Map, typename ItemsView>
+struct ItemsViewImpl : public ItemsView {
+    explicit ItemsViewImpl(Map &map) : map(map) {}
+    size_t len() override { return map.size(); }
+    iterator iter() override { return make_iterator(map.begin(), map.end()); }
     Map &map;
 };
 
 PYBIND11_NAMESPACE_END(detail)
 
 template <typename Map, typename holder_type = std::unique_ptr<Map>, typename... Args>
 class_<Map, holder_type> bind_map(handle scope, const std::string &name, Args &&...args) {
     using KeyType = typename Map::key_type;
     using MappedType = typename Map::mapped_type;
-    using KeysView = detail::keys_view<Map>;
-    using ValuesView = detail::values_view<Map>;
-    using ItemsView = detail::items_view<Map>;
+    using StrippedKeyType = detail::remove_cvref_t<KeyType>;
+    using StrippedMappedType = detail::remove_cvref_t<MappedType>;
+    using KeysView = detail::keys_view<StrippedKeyType>;
+    using ValuesView = detail::values_view<StrippedMappedType>;
+    using ItemsView = detail::items_view<StrippedKeyType, StrippedMappedType>;
     using Class_ = class_<Map, holder_type>;
 
     // If either type is a non-module-local bound type then make the map binding non-local as well;
     // otherwise (e.g. both types are either module-local or converting) the map will be
     // module-local.
     auto *tinfo = detail::get_type_info(typeid(MappedType));
     bool local = !tinfo || tinfo->module_local;
     if (local) {
         tinfo = detail::get_type_info(typeid(KeyType));
         local = !tinfo || tinfo->module_local;
     }
 
     Class_ cl(scope, name.c_str(), pybind11::module_local(local), std::forward<Args>(args)...);
-    class_<KeysView> keys_view(
-        scope, ("KeysView[" + name + "]").c_str(), pybind11::module_local(local));
-    class_<ValuesView> values_view(
-        scope, ("ValuesView[" + name + "]").c_str(), pybind11::module_local(local));
-    class_<ItemsView> items_view(
-        scope, ("ItemsView[" + name + "]").c_str(), pybind11::module_local(local));
+    static constexpr auto key_type_descr = detail::make_caster<KeyType>::name;
+    static constexpr auto mapped_type_descr = detail::make_caster<MappedType>::name;
+    std::string key_type_name(key_type_descr.text), mapped_type_name(mapped_type_descr.text);
+
+    // If key type isn't properly wrapped, fall back to C++ names
+    if (key_type_name == "%") {
+        key_type_name = detail::type_info_description(typeid(KeyType));
+    }
+    // Similarly for value type:
+    if (mapped_type_name == "%") {
+        mapped_type_name = detail::type_info_description(typeid(MappedType));
+    }
+
+    // Wrap KeysView[KeyType] if it wasn't already wrapped
+    if (!detail::get_type_info(typeid(KeysView))) {
+        class_<KeysView> keys_view(
+            scope, ("KeysView[" + key_type_name + "]").c_str(), pybind11::module_local(local));
+        keys_view.def("__len__", &KeysView::len);
+        keys_view.def("__iter__",
+                      &KeysView::iter,
+                      keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
+        );
+        keys_view.def("__contains__",
+                      static_cast<bool (KeysView::*)(const KeyType &)>(&KeysView::contains));
+        // Fallback for when the object is not of the key type
+        keys_view.def("__contains__",
+                      static_cast<bool (KeysView::*)(const object &)>(&KeysView::contains));
+    }
+    // Similarly for ValuesView:
+    if (!detail::get_type_info(typeid(ValuesView))) {
+        class_<ValuesView> values_view(scope,
+                                       ("ValuesView[" + mapped_type_name + "]").c_str(),
+                                       pybind11::module_local(local));
+        values_view.def("__len__", &ValuesView::len);
+        values_view.def("__iter__",
+                        &ValuesView::iter,
+                        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
+        );
+    }
+    // Similarly for ItemsView:
+    if (!detail::get_type_info(typeid(ItemsView))) {
+        class_<ItemsView> items_view(
+            scope,
+            ("ItemsView[" + key_type_name + ", ").append(mapped_type_name + "]").c_str(),
+            pybind11::module_local(local));
+        items_view.def("__len__", &ItemsView::len);
+        items_view.def("__iter__",
+                       &ItemsView::iter,
+                       keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
+        );
+    }
 
     cl.def(init<>());
 
     // Register stream insertion operator (if possible)
     detail::map_if_insertion_operator<Map, Class_>(cl, name);
 
     cl.def(
@@ -694,27 +778,33 @@
         "__iter__",
         [](Map &m) { return make_key_iterator(m.begin(), m.end()); },
         keep_alive<0, 1>() /* Essential: keep map alive while iterator exists */
     );
 
     cl.def(
         "keys",
-        [](Map &m) { return KeysView{m}; },
+        [](Map &m) {
+            return std::unique_ptr<KeysView>(new detail::KeysViewImpl<Map, KeysView>(m));
+        },
         keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def(
         "values",
-        [](Map &m) { return ValuesView{m}; },
+        [](Map &m) {
+            return std::unique_ptr<ValuesView>(new detail::ValuesViewImpl<Map, ValuesView>(m));
+        },
         keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def(
         "items",
-        [](Map &m) { return ItemsView{m}; },
+        [](Map &m) {
+            return std::unique_ptr<ItemsView>(new detail::ItemsViewImpl<Map, ItemsView>(m));
+        },
         keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def(
         "__getitem__",
         [](Map &m, const KeyType &k) -> MappedType & {
             auto it = m.find(k);
@@ -745,41 +835,11 @@
             throw key_error();
         }
         m.erase(it);
     });
 
     cl.def("__len__", &Map::size);
 
-    keys_view.def("__len__", [](KeysView &view) { return view.map.size(); });
-    keys_view.def(
-        "__iter__",
-        [](KeysView &view) { return make_key_iterator(view.map.begin(), view.map.end()); },
-        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
-    );
-    keys_view.def("__contains__", [](KeysView &view, const KeyType &k) -> bool {
-        auto it = view.map.find(k);
-        if (it == view.map.end()) {
-            return false;
-        }
-        return true;
-    });
-    // Fallback for when the object is not of the key type
-    keys_view.def("__contains__", [](KeysView &, const object &) -> bool { return false; });
-
-    values_view.def("__len__", [](ValuesView &view) { return view.map.size(); });
-    values_view.def(
-        "__iter__",
-        [](ValuesView &view) { return make_value_iterator(view.map.begin(), view.map.end()); },
-        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
-    );
-
-    items_view.def("__len__", [](ItemsView &view) { return view.map.size(); });
-    items_view.def(
-        "__iter__",
-        [](ItemsView &view) { return make_iterator(view.map.begin(), view.map.end()); },
-        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
-    );
-
     return cl;
 }
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `xcsf-1.2.8/lib/pybind11/tests/CMakeLists.txt` & `xcsf-1.2.9/lib/pybind11/tests/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -124,15 +124,16 @@
     test_class
     test_const_name
     test_constants_and_functions
     test_copy_move
     test_custom_type_casters
     test_custom_type_setup
     test_docstring_options
-    test_eigen
+    test_eigen_matrix
+    test_eigen_tensor
     test_enum
     test_eval
     test_exceptions
     test_factory_constructors
     test_gil_scoped
     test_iostream
     test_kwargs_and_defaults
@@ -164,15 +165,15 @@
   # Instead of doing a direct override here, we iterate over the overrides without extension and
   # match them against entries from the PYBIND11_TEST_FILES, anything that not matches goes into the filter list.
   string(REGEX REPLACE "\\.[^.;]*;" ";" TEST_OVERRIDE_NO_EXT "${PYBIND11_TEST_OVERRIDE};")
   string(REGEX REPLACE "\\.[^.;]*;" ";" TEST_FILES_NO_EXT "${PYBIND11_TEST_FILES};")
   # This allows the override to be done with extensions, preserving backwards compatibility.
   foreach(test_name ${TEST_FILES_NO_EXT})
     if(NOT ${test_name} IN_LIST TEST_OVERRIDE_NO_EXT
-    )# If not in the whitelist, add to be filtered out.
+    )# If not in the allowlist, add to be filtered out.
       list(APPEND PYBIND11_TEST_FILTER ${test_name})
     endif()
   endforeach()
 endif()
 
 # You can also filter tests:
 if(PYBIND11_TEST_FILTER)
@@ -229,15 +230,18 @@
 
 list(GET PYBIND11_EIGEN_VERSION_AND_HASH 0 PYBIND11_EIGEN_VERSION_STRING)
 list(GET PYBIND11_EIGEN_VERSION_AND_HASH 1 PYBIND11_EIGEN_VERSION_HASH)
 
 # Check if Eigen is available; if not, remove from PYBIND11_TEST_FILES (but
 # keep it in PYBIND11_PYTEST_FILES, so that we get the "eigen is not installed"
 # skip message).
-list(FIND PYBIND11_TEST_FILES test_eigen.cpp PYBIND11_TEST_FILES_EIGEN_I)
+list(FIND PYBIND11_TEST_FILES test_eigen_matrix.cpp PYBIND11_TEST_FILES_EIGEN_I)
+if(PYBIND11_TEST_FILES_EIGEN_I EQUAL -1)
+  list(FIND PYBIND11_TEST_FILES test_eigen_tensor.cpp PYBIND11_TEST_FILES_EIGEN_I)
+endif()
 if(PYBIND11_TEST_FILES_EIGEN_I GREATER -1)
   # Try loading via newer Eigen's Eigen3Config first (bypassing tools/FindEigen3.cmake).
   # Eigen 3.3.1+ exports a cmake 3.0+ target for handling dependency requirements, but also
   # produces a fatal error if loaded from a pre-3.0 cmake.
   if(DOWNLOAD_EIGEN)
     if(CMAKE_VERSION VERSION_LESS 3.11)
       message(FATAL_ERROR "CMake 3.11+ required when using DOWNLOAD_EIGEN")
@@ -284,21 +288,42 @@
     # Eigen 3.3.1+ cmake sets EIGEN3_VERSION_STRING (and hard codes the version when installed
     # rather than looking it up in the cmake script); older versions, and the
     # tools/FindEigen3.cmake, set EIGEN3_VERSION instead.
     if(NOT EIGEN3_VERSION AND EIGEN3_VERSION_STRING)
       set(EIGEN3_VERSION ${EIGEN3_VERSION_STRING})
     endif()
     message(STATUS "Building tests with Eigen v${EIGEN3_VERSION}")
+
+    if(NOT (CMAKE_CXX_COMPILER_ID STREQUAL "GNU" AND CMAKE_CXX_COMPILER_VERSION VERSION_LESS 5.0))
+      tests_extra_targets("test_eigen_tensor.py" "eigen_tensor_avoid_stl_array")
+    endif()
+
   else()
-    list(REMOVE_AT PYBIND11_TEST_FILES ${PYBIND11_TEST_FILES_EIGEN_I})
+    list(FIND PYBIND11_TEST_FILES test_eigen_matrix.cpp PYBIND11_TEST_FILES_EIGEN_I)
+    if(PYBIND11_TEST_FILES_EIGEN_I GREATER -1)
+      list(REMOVE_AT PYBIND11_TEST_FILES ${PYBIND11_TEST_FILES_EIGEN_I})
+    endif()
+
+    list(FIND PYBIND11_TEST_FILES test_eigen_tensor.cpp PYBIND11_TEST_FILES_EIGEN_I)
+    if(PYBIND11_TEST_FILES_EIGEN_I GREATER -1)
+      list(REMOVE_AT PYBIND11_TEST_FILES ${PYBIND11_TEST_FILES_EIGEN_I})
+    endif()
     message(
       STATUS "Building tests WITHOUT Eigen, use -DDOWNLOAD_EIGEN=ON on CMake 3.11+ to download")
   endif()
 endif()
 
+# Some code doesn't support gcc 4
+if(CMAKE_CXX_COMPILER_ID STREQUAL "GNU" AND CMAKE_CXX_COMPILER_VERSION VERSION_LESS 5.0)
+  list(FIND PYBIND11_TEST_FILES test_eigen_tensor.cpp PYBIND11_TEST_FILES_EIGEN_I)
+  if(PYBIND11_TEST_FILES_EIGEN_I GREATER -1)
+    list(REMOVE_AT PYBIND11_TEST_FILES ${PYBIND11_TEST_FILES_EIGEN_I})
+  endif()
+endif()
+
 # Optional dependency for some tests (boost::variant is only supported with version >= 1.56)
 find_package(Boost 1.56)
 
 if(Boost_FOUND)
   if(NOT TARGET Boost::headers)
     add_library(Boost::headers IMPORTED INTERFACE)
     if(TARGET Boost::boost)
```

### Comparing `xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/CMakeLists.txt` & `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `xcsf-1.2.9/lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tests/test_embed/CMakeLists.txt` & `xcsf-1.2.9/lib/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tools/FindCatch.cmake` & `xcsf-1.2.9/lib/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tools/FindEigen3.cmake` & `xcsf-1.2.9/lib/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tools/FindPythonLibsNew.cmake` & `xcsf-1.2.9/lib/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files 7% similar despite different names*

```diff
@@ -147,17 +147,21 @@
     message(FATAL_ERROR "Python config failure:\n${_PYTHON_ERROR_VALUE}")
   endif()
   set(PYTHONLIBS_FOUND FALSE)
   set(PythonLibsNew_FOUND FALSE)
   return()
 endif()
 
+option(
+  PYBIND11_PYTHONLIBS_OVERWRITE
+  "Overwrite cached values read from Python library (classic search). Turn off if cross-compiling and manually setting these values."
+  ON)
 # Can manually set values when cross-compiling
 macro(_PYBIND11_GET_IF_UNDEF lst index name)
-  if(NOT DEFINED "${name}")
+  if(PYBIND11_PYTHONLIBS_OVERWRITE OR NOT DEFINED "${name}")
     list(GET "${lst}" "${index}" "${name}")
   endif()
 endmacro()
 
 # Convert the process output into a list
 if(WIN32)
   string(REGEX REPLACE "\\\\" "/" _PYTHON_VALUES ${_PYTHON_VALUES})
@@ -200,15 +204,17 @@
 set(PYTHON_VERSION "${PYTHON_VERSION_MAJOR}.${PYTHON_VERSION_MINOR}.${PYTHON_VERSION_PATCH}")
 
 # Make sure all directory separators are '/'
 string(REGEX REPLACE "\\\\" "/" PYTHON_PREFIX "${PYTHON_PREFIX}")
 string(REGEX REPLACE "\\\\" "/" PYTHON_INCLUDE_DIR "${PYTHON_INCLUDE_DIR}")
 string(REGEX REPLACE "\\\\" "/" PYTHON_SITE_PACKAGES "${PYTHON_SITE_PACKAGES}")
 
-if(CMAKE_HOST_WIN32)
+if(DEFINED PYTHON_LIBRARY)
+  # Don't write to PYTHON_LIBRARY if it's already set
+elseif(CMAKE_HOST_WIN32)
   set(PYTHON_LIBRARY "${PYTHON_PREFIX}/libs/python${PYTHON_LIBRARY_SUFFIX}.lib")
 
   # when run in a venv, PYTHON_PREFIX points to it. But the libraries remain in the
   # original python installation. They may be found relative to PYTHON_INCLUDE_DIR.
   if(NOT EXISTS "${PYTHON_LIBRARY}")
     get_filename_component(_PYTHON_ROOT ${PYTHON_INCLUDE_DIR} DIRECTORY)
     set(PYTHON_LIBRARY "${_PYTHON_ROOT}/libs/python${PYTHON_LIBRARY_SUFFIX}.lib")
@@ -266,15 +272,15 @@
 set(PYTHON_INCLUDE_DIRS "${PYTHON_INCLUDE_DIR}")
 set(PYTHON_LIBRARIES "${PYTHON_LIBRARY}")
 if(NOT PYTHON_DEBUG_LIBRARY)
   set(PYTHON_DEBUG_LIBRARY "")
 endif()
 set(PYTHON_DEBUG_LIBRARIES "${PYTHON_DEBUG_LIBRARY}")
 
-find_package_message(PYTHON "Found PythonLibs: ${PYTHON_LIBRARY}"
+find_package_message(PYTHON "Found PythonLibs: ${PYTHON_LIBRARIES}"
                      "${PYTHON_EXECUTABLE}${PYTHON_VERSION_STRING}")
 
 set(PYTHONLIBS_FOUND TRUE)
 set(PythonLibsNew_FOUND TRUE)
 
 if(NOT PYTHON_MODULE_PREFIX)
   set(PYTHON_MODULE_PREFIX "")
```

### Comparing `xcsf-1.2.8/lib/pybind11/tools/check-style.sh` & `xcsf-1.2.9/lib/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tools/cmake_uninstall.cmake.in` & `xcsf-1.2.9/lib/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tools/libsize.py` & `xcsf-1.2.9/lib/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tools/make_changelog.py` & `xcsf-1.2.9/lib/pybind11/tools/make_changelog.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,30 +27,29 @@
 issues_pages = ghapi.page.paged(
     api.issues.list_for_repo, labels="needs changelog", state="closed"
 )
 issues = (issue for page in issues_pages for issue in page)
 missing = []
 
 for issue in issues:
-    changelog = ENTRY.findall(issue.body)
-    if changelog:
+    changelog = ENTRY.findall(issue.body or "")
+    if not changelog or not changelog[0]:
+        missing.append(issue)
+    else:
         (msg,) = changelog
         if not msg.startswith("* "):
             msg = "* " + msg
         if not msg.endswith("."):
             msg += "."
 
         msg += f"\n  `#{issue.number} <{issue.html_url}>`_"
 
         print(Syntax(msg, "rst", theme="ansi_light", word_wrap=True))
         print()
 
-    else:
-        missing.append(issue)
-
 if missing:
     print()
     print("[blue]" + "-" * 30)
     print()
 
     for issue in missing:
         print(f"[red bold]Missing:[/red bold][red] {issue.title}")
```

### Comparing `xcsf-1.2.8/lib/pybind11/tools/pybind11Common.cmake` & `xcsf-1.2.9/lib/pybind11/tools/pybind11Common.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -307,14 +307,24 @@
     endif()
 
     if(NOT HAS_FLTO_THIN AND NOT NO_FLTO_ARCH)
       _pybind11_return_if_cxx_and_linker_flags_work(
         HAS_FLTO "-flto${cxx_append}" "-flto${linker_append}" PYBIND11_LTO_CXX_FLAGS
         PYBIND11_LTO_LINKER_FLAGS)
     endif()
+  elseif(CMAKE_CXX_COMPILER_ID MATCHES "IntelLLVM")
+    # IntelLLVM equivalent to LTO is called IPO; also IntelLLVM is WIN32/UNIX
+    # WARNING/HELP WANTED: This block of code is currently not covered by pybind11 GitHub Actions!
+    if(WIN32)
+      _pybind11_return_if_cxx_and_linker_flags_work(
+        HAS_INTEL_IPO "-Qipo" "-Qipo" PYBIND11_LTO_CXX_FLAGS PYBIND11_LTO_LINKER_FLAGS)
+    else()
+      _pybind11_return_if_cxx_and_linker_flags_work(
+        HAS_INTEL_IPO "-ipo" "-ipo" PYBIND11_LTO_CXX_FLAGS PYBIND11_LTO_LINKER_FLAGS)
+    endif()
   elseif(CMAKE_CXX_COMPILER_ID MATCHES "Intel")
     # Intel equivalent to LTO is called IPO
     _pybind11_return_if_cxx_and_linker_flags_work(HAS_INTEL_IPO "-ipo" "-ipo"
                                                   PYBIND11_LTO_CXX_FLAGS PYBIND11_LTO_LINKER_FLAGS)
   elseif(MSVC)
     # cmake only interprets libraries as linker flags when they start with a - (otherwise it
     # converts /LTCG to \LTCG as if it was a Windows path).  Luckily MSVC supports passing flags
```

### Comparing `xcsf-1.2.8/lib/pybind11/tools/pybind11Config.cmake.in` & `xcsf-1.2.9/lib/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/lib/pybind11/tools/pybind11NewTools.cmake` & `xcsf-1.2.9/lib/pybind11/tools/pybind11NewTools.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 
 if(CMAKE_VERSION VERSION_LESS 3.12)
   message(FATAL_ERROR "You cannot use the new FindPython module with CMake < 3.12")
 endif()
 
-include_guard(GLOBAL)
+include_guard(DIRECTORY)
 
 get_property(
   is_config
   TARGET pybind11::headers
   PROPERTY IMPORTED)
 
 if(pybind11_FIND_QUIETLY)
@@ -229,15 +229,17 @@
     if(ARG_THIN_LTO)
       target_link_libraries(${target_name} PRIVATE pybind11::thin_lto)
     else()
       target_link_libraries(${target_name} PRIVATE pybind11::lto)
     endif()
   endif()
 
-  if(NOT MSVC AND NOT ${CMAKE_BUILD_TYPE} MATCHES Debug|RelWithDebInfo)
+  # Use case-insensitive comparison to match the result of $<CONFIG:cfgs>
+  string(TOUPPER "${CMAKE_BUILD_TYPE}" uppercase_CMAKE_BUILD_TYPE)
+  if(NOT MSVC AND NOT "${uppercase_CMAKE_BUILD_TYPE}" MATCHES DEBUG|RELWITHDEBINFO)
     # Strip unnecessary sections of the binary on Linux/macOS
     pybind11_strip(${target_name})
   endif()
 
   if(MSVC)
     target_link_libraries(${target_name} PRIVATE pybind11::windows_extras)
   endif()
```

### Comparing `xcsf-1.2.8/lib/pybind11/tools/pybind11Tools.cmake` & `xcsf-1.2.9/lib/pybind11/tools/pybind11Tools.cmake`

 * *Files 4% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 if(PYTHON_IS_DEBUG)
   set_property(
     TARGET pybind11::pybind11
     APPEND
     PROPERTY INTERFACE_COMPILE_DEFINITIONS Py_DEBUG)
 endif()
 
+# The <3.11 code here does not support release/debug builds at the same time, like on vcpkg
 if(CMAKE_VERSION VERSION_LESS 3.11)
   set_property(
     TARGET pybind11::module
     APPEND
     PROPERTY
       INTERFACE_LINK_LIBRARIES
       pybind11::python_link_helper
@@ -126,24 +127,27 @@
   )
 
   set_property(
     TARGET pybind11::embed
     APPEND
     PROPERTY INTERFACE_LINK_LIBRARIES pybind11::pybind11 $<BUILD_INTERFACE:${PYTHON_LIBRARIES}>)
 else()
+  # The IMPORTED INTERFACE library here is to ensure that "debug" and "release" get processed outside
+  # of a generator expression - https://gitlab.kitware.com/cmake/cmake/-/issues/18424, as they are
+  # target_link_library keywords rather than real libraries.
+  add_library(pybind11::_ClassicPythonLibraries IMPORTED INTERFACE)
+  target_link_libraries(pybind11::_ClassicPythonLibraries INTERFACE ${PYTHON_LIBRARIES})
   target_link_libraries(
     pybind11::module
     INTERFACE
       pybind11::python_link_helper
-      "$<$<OR:$<PLATFORM_ID:Windows>,$<PLATFORM_ID:Cygwin>>:$<BUILD_INTERFACE:${PYTHON_LIBRARIES}>>"
-  )
+      "$<$<OR:$<PLATFORM_ID:Windows>,$<PLATFORM_ID:Cygwin>>:pybind11::_ClassicPythonLibraries>")
 
   target_link_libraries(pybind11::embed INTERFACE pybind11::pybind11
-                                                  $<BUILD_INTERFACE:${PYTHON_LIBRARIES}>)
-
+                                                  pybind11::_ClassicPythonLibraries)
 endif()
 
 function(pybind11_extension name)
   # The prefix and extension are provided by FindPythonLibsNew.cmake
   set_target_properties(${name} PROPERTIES PREFIX "${PYTHON_MODULE_PREFIX}"
                                            SUFFIX "${PYTHON_MODULE_EXTENSION}")
 endfunction()
@@ -204,15 +208,17 @@
     if(ARG_THIN_LTO)
       target_link_libraries(${target_name} PRIVATE pybind11::thin_lto)
     else()
       target_link_libraries(${target_name} PRIVATE pybind11::lto)
     endif()
   endif()
 
-  if(NOT MSVC AND NOT ${CMAKE_BUILD_TYPE} MATCHES Debug|RelWithDebInfo)
+  # Use case-insensitive comparison to match the result of $<CONFIG:cfgs>
+  string(TOUPPER "${CMAKE_BUILD_TYPE}" uppercase_CMAKE_BUILD_TYPE)
+  if(NOT MSVC AND NOT "${uppercase_CMAKE_BUILD_TYPE}" MATCHES DEBUG|RELWITHDEBINFO)
     pybind11_strip(${target_name})
   endif()
 
   if(MSVC)
     target_link_libraries(${target_name} PRIVATE pybind11::windows_extras)
   endif()
```

### Comparing `xcsf-1.2.8/lib/pybind11/tools/setup_global.py.in` & `xcsf-1.2.9/lib/pybind11/tools/setup_global.py.in`

 * *Files 19% similar despite different names*

```diff
@@ -23,17 +23,19 @@
             self.mkpath(dst)
             (out, _) = self.copy_file(header, dst)
             self.outfiles.append(out)
 
 
 main_headers = glob.glob("pybind11/include/pybind11/*.h")
 detail_headers = glob.glob("pybind11/include/pybind11/detail/*.h")
+eigen_headers = glob.glob("pybind11/include/pybind11/eigen/*.h")
 stl_headers = glob.glob("pybind11/include/pybind11/stl/*.h")
 cmake_files = glob.glob("pybind11/share/cmake/pybind11/*.cmake")
-headers = main_headers + detail_headers + stl_headers
+pkgconfig_files = glob.glob("pybind11/share/pkgconfig/*.pc")
+headers = main_headers + detail_headers + stl_headers + eigen_headers
 
 cmdclass = {"install_headers": InstallHeadersNested}
 $extra_cmd
 
 # This will _not_ affect installing from wheels,
 # only building wheels or installing from SDist.
 # Primarily intended on Windows, where this is sometimes
@@ -47,13 +49,15 @@
 setup(
     name="pybind11_global",
     version="$version",
     packages=[],
     headers=headers,
     data_files=[
         (base + "share/cmake/pybind11", cmake_files),
+        (base + "share/pkgconfig", pkgconfig_files),
         (base + "include/pybind11", main_headers),
         (base + "include/pybind11/detail", detail_headers),
+        (base + "include/pybind11/eigen", eigen_headers),
         (base + "include/pybind11/stl", stl_headers),
     ],
     cmdclass=cmdclass,
 )
```

### Comparing `xcsf-1.2.8/lib/pybind11/tools/setup_main.py.in` & `xcsf-1.2.9/lib/pybind11/tools/setup_main.py.in`

 * *Files 26% similar despite different names*

```diff
@@ -11,23 +11,27 @@
     name="pybind11",
     version="$version",
     download_url='https://github.com/pybind/pybind11/tarball/v$version',
     packages=[
         "pybind11",
         "pybind11.include.pybind11",
         "pybind11.include.pybind11.detail",
+        "pybind11.include.pybind11.eigen",
         "pybind11.include.pybind11.stl",
         "pybind11.share.cmake.pybind11",
+        "pybind11.share.pkgconfig",
     ],
     package_data={
         "pybind11": ["py.typed"],
         "pybind11.include.pybind11": ["*.h"],
         "pybind11.include.pybind11.detail": ["*.h"],
+        "pybind11.include.pybind11.eigen": ["*.h"],
         "pybind11.include.pybind11.stl": ["*.h"],
         "pybind11.share.cmake.pybind11": ["*.cmake"],
+        "pybind11.share.pkgconfig": ["*.pc"],
     },
     extras_require={
         "global": ["pybind11_global==$version"]
         },
     entry_points={
         "console_scripts": [
              "pybind11-config = pybind11.__main__:main",
```

### Comparing `xcsf-1.2.8/setup.py` & `xcsf-1.2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,17 @@
             "-DENABLE_DOXYGEN=OFF",
             "-DNATIVE_OPT=OFF",
         ]
         build_args = [
             "--config",
             "Release",
         ]
+        if platform.system() == "Darwin":  # set to force CI to use GCC
+            cmake_args[2] = "-DCMAKE_C_COMPILER=gcc-11"
+            cmake_args[3] = "-DCMAKE_CXX_COMPILER=g++-11"
         if platform.system() == "Windows":
             cmake_args += ["-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_RELEASE=" + extdir]
             cmake_args += ["-GMinGW Makefiles"]
         else:
             cmake_args += ["-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=" + extdir]
             build_args += ["-j4"]
         subprocess.check_call(
@@ -76,15 +79,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="xcsf",
-    version="1.2.8",
+    version="1.2.9",
     license="GPL-3.0",
     maintainer="Richard Preen",
     maintainer_email="rpreen@gmail.com",
     description="XCSF learning classifier system: rule-based evolutionary machine learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rpreen/xcsf",
```

### Comparing `xcsf-1.2.8/test/CMakeLists.txt` & `xcsf-1.2.9/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/CMakeLists.txt` & `xcsf-1.2.9/xcsf/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/__init__.pyi` & `xcsf-1.2.9/xcsf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/act_integer.c` & `xcsf-1.2.9/xcsf/act_integer.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/act_integer.h` & `xcsf-1.2.9/xcsf/act_integer.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/act_neural.c` & `xcsf-1.2.9/xcsf/act_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/act_neural.h` & `xcsf-1.2.9/xcsf/act_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/action.c` & `xcsf-1.2.9/xcsf/action.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/action.h` & `xcsf-1.2.9/xcsf/action.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/blas.c` & `xcsf-1.2.9/xcsf/blas.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/blas.h` & `xcsf-1.2.9/xcsf/blas.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cl.c` & `xcsf-1.2.9/xcsf/cl.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cl.h` & `xcsf-1.2.9/xcsf/cl.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/clset.c` & `xcsf-1.2.9/xcsf/clset.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/clset.h` & `xcsf-1.2.9/xcsf/clset.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/clset_neural.c` & `xcsf-1.2.9/xcsf/clset_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/clset_neural.h` & `xcsf-1.2.9/xcsf/clset_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_dgp.c` & `xcsf-1.2.9/xcsf/cond_dgp.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_dgp.h` & `xcsf-1.2.9/xcsf/cond_dgp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_dummy.c` & `xcsf-1.2.9/xcsf/cond_dummy.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_dummy.h` & `xcsf-1.2.9/xcsf/cond_dummy.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_ellipsoid.c` & `xcsf-1.2.9/xcsf/cond_ellipsoid.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_ellipsoid.h` & `xcsf-1.2.9/xcsf/cond_ellipsoid.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_gp.c` & `xcsf-1.2.9/xcsf/cond_gp.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_gp.h` & `xcsf-1.2.9/xcsf/cond_gp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_neural.c` & `xcsf-1.2.9/xcsf/cond_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_neural.h` & `xcsf-1.2.9/xcsf/cond_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_rectangle.c` & `xcsf-1.2.9/xcsf/cond_rectangle.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_rectangle.h` & `xcsf-1.2.9/xcsf/cond_rectangle.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_ternary.c` & `xcsf-1.2.9/xcsf/cond_ternary.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/cond_ternary.h` & `xcsf-1.2.9/xcsf/cond_ternary.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/condition.c` & `xcsf-1.2.9/xcsf/condition.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/condition.h` & `xcsf-1.2.9/xcsf/condition.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/config.c` & `xcsf-1.2.9/xcsf/config.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/config.h` & `xcsf-1.2.9/xcsf/config.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/dgp.c` & `xcsf-1.2.9/xcsf/dgp.c`

 * *Files 0% similar despite different names*

```diff
@@ -601,14 +601,15 @@
     }
     dgp->state = malloc(sizeof(double) * dgp->n);
     dgp->initial_state = malloc(sizeof(double) * dgp->n);
     dgp->tmp_state = malloc(sizeof(double) * dgp->n);
     dgp->tmp_input = malloc(sizeof(double) * dgp->max_k);
     dgp->function = malloc(sizeof(int) * dgp->n);
     dgp->connectivity = malloc(sizeof(int) * dgp->klen);
+    dgp->mu = malloc(sizeof(double) * N_MU);
     s += fread(dgp->state, sizeof(double), dgp->n, fp);
     s += fread(dgp->initial_state, sizeof(double), dgp->n, fp);
     s += fread(dgp->function, sizeof(int), dgp->n, fp);
     s += fread(dgp->connectivity, sizeof(int), dgp->klen, fp);
     s += fread(dgp->mu, sizeof(double), N_MU, fp);
     return s;
 }
```

### Comparing `xcsf-1.2.8/xcsf/dgp.h` & `xcsf-1.2.9/xcsf/dgp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/ea.c` & `xcsf-1.2.9/xcsf/ea.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/ea.h` & `xcsf-1.2.9/xcsf/ea.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/env.c` & `xcsf-1.2.9/xcsf/env.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/env.h` & `xcsf-1.2.9/xcsf/env.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/env_csv.c` & `xcsf-1.2.9/xcsf/env_csv.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/env_csv.h` & `xcsf-1.2.9/xcsf/env_csv.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/env_maze.c` & `xcsf-1.2.9/xcsf/env_maze.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/env_maze.h` & `xcsf-1.2.9/xcsf/env_maze.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/env_mux.c` & `xcsf-1.2.9/xcsf/env_mux.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/env_mux.h` & `xcsf-1.2.9/xcsf/env_mux.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/gp.c` & `xcsf-1.2.9/xcsf/gp.c`

 * *Files 0% similar despite different names*

```diff
@@ -404,14 +404,15 @@
     s += fread(&gp->len, sizeof(int), 1, fp);
     if (gp->len < 1) {
         printf("tree_load(): read error\n");
         gp->len = 1;
         exit(EXIT_FAILURE);
     }
     gp->tree = malloc(sizeof(int) * gp->len);
+    gp->mu = malloc(sizeof(double) * N_MU);
     s += fread(gp->tree, sizeof(int), gp->len, fp);
     s += fread(gp->mu, sizeof(double), N_MU, fp);
     return s;
 }
 
 /**
  * @brief Sets tree GP parameters to default values.
```

### Comparing `xcsf-1.2.8/xcsf/gp.h` & `xcsf-1.2.9/xcsf/gp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/image.c` & `xcsf-1.2.9/xcsf/image.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/image.h` & `xcsf-1.2.9/xcsf/image.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/loss.c` & `xcsf-1.2.9/xcsf/loss.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/loss.h` & `xcsf-1.2.9/xcsf/loss.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/main.c` & `xcsf-1.2.9/xcsf/main.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural.c` & `xcsf-1.2.9/xcsf/neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural.h` & `xcsf-1.2.9/xcsf/neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_activations.c` & `xcsf-1.2.9/xcsf/neural_activations.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_activations.h` & `xcsf-1.2.9/xcsf/neural_activations.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer.c` & `xcsf-1.2.9/xcsf/neural_layer.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer.h` & `xcsf-1.2.9/xcsf/neural_layer.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_args.c` & `xcsf-1.2.9/xcsf/neural_layer_args.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_args.h` & `xcsf-1.2.9/xcsf/neural_layer_args.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_avgpool.c` & `xcsf-1.2.9/xcsf/neural_layer_avgpool.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_avgpool.h` & `xcsf-1.2.9/xcsf/neural_layer_avgpool.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_connected.c` & `xcsf-1.2.9/xcsf/neural_layer_connected.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_connected.h` & `xcsf-1.2.9/xcsf/neural_layer_connected.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_convolutional.c` & `xcsf-1.2.9/xcsf/neural_layer_convolutional.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_convolutional.h` & `xcsf-1.2.9/xcsf/neural_layer_convolutional.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_dropout.c` & `xcsf-1.2.9/xcsf/neural_layer_dropout.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_dropout.h` & `xcsf-1.2.9/xcsf/neural_layer_dropout.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_lstm.c` & `xcsf-1.2.9/xcsf/neural_layer_lstm.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_lstm.h` & `xcsf-1.2.9/xcsf/neural_layer_lstm.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_maxpool.c` & `xcsf-1.2.9/xcsf/neural_layer_maxpool.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_maxpool.h` & `xcsf-1.2.9/xcsf/neural_layer_maxpool.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_noise.c` & `xcsf-1.2.9/xcsf/neural_layer_noise.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_noise.h` & `xcsf-1.2.9/xcsf/neural_layer_noise.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_recurrent.c` & `xcsf-1.2.9/xcsf/neural_layer_recurrent.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_recurrent.h` & `xcsf-1.2.9/xcsf/neural_layer_recurrent.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_softmax.c` & `xcsf-1.2.9/xcsf/neural_layer_softmax.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_softmax.h` & `xcsf-1.2.9/xcsf/neural_layer_softmax.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_upsample.c` & `xcsf-1.2.9/xcsf/neural_layer_upsample.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/neural_layer_upsample.h` & `xcsf-1.2.9/xcsf/neural_layer_upsample.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/pa.c` & `xcsf-1.2.9/xcsf/pa.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/pa.h` & `xcsf-1.2.9/xcsf/pa.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/param.c` & `xcsf-1.2.9/xcsf/param.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/param.h` & `xcsf-1.2.9/xcsf/param.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/perf.c` & `xcsf-1.2.9/xcsf/perf.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/perf.h` & `xcsf-1.2.9/xcsf/perf.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/pred_constant.c` & `xcsf-1.2.9/xcsf/pred_constant.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/pred_constant.h` & `xcsf-1.2.9/xcsf/pred_constant.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/pred_neural.c` & `xcsf-1.2.9/xcsf/pred_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/pred_neural.h` & `xcsf-1.2.9/xcsf/pred_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/pred_nlms.c` & `xcsf-1.2.9/xcsf/pred_nlms.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/pred_nlms.h` & `xcsf-1.2.9/xcsf/pred_nlms.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/pred_rls.c` & `xcsf-1.2.9/xcsf/pred_rls.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/pred_rls.h` & `xcsf-1.2.9/xcsf/pred_rls.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/prediction.c` & `xcsf-1.2.9/xcsf/prediction.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/prediction.h` & `xcsf-1.2.9/xcsf/prediction.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/pybind_wrapper.cpp` & `xcsf-1.2.9/xcsf/pybind_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/rule_dgp.c` & `xcsf-1.2.9/xcsf/rule_dgp.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/rule_dgp.h` & `xcsf-1.2.9/xcsf/rule_dgp.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/rule_neural.c` & `xcsf-1.2.9/xcsf/rule_neural.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/rule_neural.h` & `xcsf-1.2.9/xcsf/rule_neural.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/sam.c` & `xcsf-1.2.9/xcsf/sam.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/sam.h` & `xcsf-1.2.9/xcsf/sam.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/utils/types.py` & `xcsf-1.2.9/xcsf/utils/types.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/utils/viz.py` & `xcsf-1.2.9/xcsf/utils/viz.py`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/utils.c` & `xcsf-1.2.9/xcsf/utils.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/utils.h` & `xcsf-1.2.9/xcsf/utils.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/xcs_rl.c` & `xcsf-1.2.9/xcsf/xcs_rl.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/xcs_rl.h` & `xcsf-1.2.9/xcsf/xcs_rl.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/xcs_supervised.c` & `xcsf-1.2.9/xcsf/xcs_supervised.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/xcs_supervised.h` & `xcsf-1.2.9/xcsf/xcs_supervised.h`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/xcsf.c` & `xcsf-1.2.9/xcsf/xcsf.c`

 * *Files identical despite different names*

### Comparing `xcsf-1.2.8/xcsf/xcsf.h` & `xcsf-1.2.9/xcsf/xcsf.h`

 * *Files identical despite different names*

```diff
@@ -33,15 +33,15 @@
 #include <stdint.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 
 static const int VERSION_MAJOR = 1; //!< XCSF major version number
 static const int VERSION_MINOR = 2; //!< XCSF minor version number
-static const int VERSION_BUILD = 8; //!< XCSF build version number
+static const int VERSION_BUILD = 9; //!< XCSF build version number
 
 /**
  * @brief Classifier data structure.
  */
 struct Cl {
     struct CondVtbl const *cond_vptr; //!< Functions acting on conditions
     struct PredVtbl const *pred_vptr; //!< Functions acting on predictions
```

### Comparing `xcsf-1.2.8/xcsf.egg-info/PKG-INFO` & `xcsf-1.2.9/xcsf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsf
-Version: 1.2.8
+Version: 1.2.9
 Summary: XCSF learning classifier system: rule-based evolutionary machine learning
 Home-page: https://github.com/rpreen/xcsf
 Maintainer: Richard Preen
 Maintainer-email: rpreen@gmail.com
 License: GPL-3.0
 Keywords: divide and conquer,evolutionary algorithm,genetic programming,learning classifier system,least squares,machine learning,neural networks,neuroevolution,reinforcement learning,rule-based,supervised learning,stochastic gradient descent,XCS,XCSF
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xcsf-1.2.8/xcsf.egg-info/SOURCES.txt` & `xcsf-1.2.9/xcsf.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 lib/cJSON/cJSON.h
 lib/cJSON/cJSON_Utils.c
 lib/cJSON/cJSON_Utils.h
 lib/cJSON/test.c
 lib/cJSON/valgrind.supp
 lib/cJSON/.github/CONTRIBUTING.md
 lib/cJSON/.github/workflows/CI.yml
+lib/cJSON/.github/workflows/ci-fuzz.yml
 lib/cJSON/fuzzing/.gitignore
 lib/cJSON/fuzzing/CMakeLists.txt
 lib/cJSON/fuzzing/afl-prepare-linux.sh
 lib/cJSON/fuzzing/afl.c
 lib/cJSON/fuzzing/afl.sh
 lib/cJSON/fuzzing/cjson_read_fuzzer.c
 lib/cJSON/fuzzing/fuzz_main.c
@@ -459,31 +460,36 @@
 lib/pybind11/include/pybind11/detail/class.h
 lib/pybind11/include/pybind11/detail/common.h
 lib/pybind11/include/pybind11/detail/descr.h
 lib/pybind11/include/pybind11/detail/init.h
 lib/pybind11/include/pybind11/detail/internals.h
 lib/pybind11/include/pybind11/detail/type_caster_base.h
 lib/pybind11/include/pybind11/detail/typeid.h
+lib/pybind11/include/pybind11/eigen/matrix.h
+lib/pybind11/include/pybind11/eigen/tensor.h
 lib/pybind11/include/pybind11/stl/filesystem.h
 lib/pybind11/tests/CMakeLists.txt
 lib/pybind11/tests/test_cmake_build/CMakeLists.txt
 lib/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
 lib/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
 lib/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
 lib/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
 lib/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
 lib/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
 lib/pybind11/tests/test_embed/CMakeLists.txt
 lib/pybind11/tools/FindCatch.cmake
 lib/pybind11/tools/FindEigen3.cmake
 lib/pybind11/tools/FindPythonLibsNew.cmake
+lib/pybind11/tools/JoinPaths.cmake
 lib/pybind11/tools/check-style.sh
 lib/pybind11/tools/cmake_uninstall.cmake.in
+lib/pybind11/tools/codespell_ignore_lines_from_errors.py
 lib/pybind11/tools/libsize.py
 lib/pybind11/tools/make_changelog.py
+lib/pybind11/tools/pybind11.pc.in
 lib/pybind11/tools/pybind11Common.cmake
 lib/pybind11/tools/pybind11Config.cmake.in
 lib/pybind11/tools/pybind11NewTools.cmake
 lib/pybind11/tools/pybind11Tools.cmake
 lib/pybind11/tools/pyproject.toml
 lib/pybind11/tools/setup_global.py.in
 lib/pybind11/tools/setup_main.py.in
```

