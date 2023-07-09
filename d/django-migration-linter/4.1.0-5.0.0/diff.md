# Comparing `tmp/django-migration-linter-4.1.0.tar.gz` & `tmp/django-migration-linter-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-migration-linter-4.1.0.tar", last modified: Sun Apr 24 16:03:28 2022, max compression
+gzip compressed data, was "django-migration-linter-5.0.0.tar", last modified: Sun Jul  9 12:49:41 2023, max compression
```

## Comparing `django-migration-linter-4.1.0.tar` & `django-migration-linter-5.0.0.tar`

### file list

```diff
@@ -1,190 +1,44 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/
--rw-rw-r--   0 david     (1000) david     (1000)    10035 2022-04-24 16:00:31.000000 django-migration-linter-4.1.0/CHANGELOG.md
--rw-r--r--   0 david     (1000) david     (1000)    10173 2019-01-19 11:56:14.000000 django-migration-linter-4.1.0/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)      145 2021-06-12 11:40:31.000000 django-migration-linter-4.1.0/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     6605 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     4815 2022-01-28 18:11:14.000000 django-migration-linter-4.1.0/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.930713 django-migration-linter-4.1.0/django_migration_linter/
--rw-r--r--   0 david     (1000) david     (1000)       74 2020-01-19 16:33:23.000000 django-migration-linter-4.1.0/django_migration_linter/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      735 2020-01-19 16:33:23.000000 django-migration-linter-4.1.0/django_migration_linter/cache.py
--rw-rw-r--   0 david     (1000) david     (1000)      277 2022-04-24 16:00:46.000000 django-migration-linter-4.1.0/django_migration_linter/constants.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.930713 django-migration-linter-4.1.0/django_migration_linter/management/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/django_migration_linter/management/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.930713 django-migration-linter-4.1.0/django_migration_linter/management/commands/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/django_migration_linter/management/commands/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     7761 2022-04-24 15:53:18.000000 django-migration-linter-4.1.0/django_migration_linter/management/commands/lintmigrations.py
--rw-rw-r--   0 david     (1000) david     (1000)     4132 2022-03-16 16:54:06.000000 django-migration-linter-4.1.0/django_migration_linter/management/commands/makemigrations.py
--rw-rw-r--   0 david     (1000) david     (1000)     1726 2022-03-16 16:54:06.000000 django-migration-linter-4.1.0/django_migration_linter/management/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)    25131 2022-03-16 16:54:06.000000 django-migration-linter-4.1.0/django_migration_linter/migration_linter.py
--rw-r--r--   0 david     (1000) david     (1000)      658 2020-01-19 16:33:23.000000 django-migration-linter-4.1.0/django_migration_linter/operations.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.930713 django-migration-linter-4.1.0/django_migration_linter/sql_analyser/
--rw-rw-r--   0 david     (1000) david     (1000)      263 2022-01-30 14:20:23.000000 django-migration-linter-4.1.0/django_migration_linter/sql_analyser/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1605 2022-01-30 14:20:23.000000 django-migration-linter-4.1.0/django_migration_linter/sql_analyser/analyser.py
--rw-rw-r--   0 david     (1000) david     (1000)     5551 2022-01-28 20:28:05.000000 django-migration-linter-4.1.0/django_migration_linter/sql_analyser/base.py
--rw-rw-r--   0 david     (1000) david     (1000)      747 2021-08-14 13:01:27.000000 django-migration-linter-4.1.0/django_migration_linter/sql_analyser/mysql.py
--rw-rw-r--   0 david     (1000) david     (1000)     1419 2022-01-28 18:11:14.000000 django-migration-linter-4.1.0/django_migration_linter/sql_analyser/postgresql.py
--rw-rw-r--   0 david     (1000) david     (1000)     1665 2022-01-28 20:28:05.000000 django-migration-linter-4.1.0/django_migration_linter/sql_analyser/sqlite.py
--rw-r--r--   0 david     (1000) david     (1000)      689 2020-01-19 16:33:23.000000 django-migration-linter-4.1.0/django_migration_linter/sql_analyser/utils.py
--rw-r--r--   0 david     (1000) david     (1000)     1491 2020-01-19 16:33:23.000000 django-migration-linter-4.1.0/django_migration_linter/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.930713 django-migration-linter-4.1.0/django_migration_linter.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)     6605 2022-04-24 16:03:28.000000 django-migration-linter-4.1.0/django_migration_linter.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     7740 2022-04-24 16:03:28.000000 django-migration-linter-4.1.0/django_migration_linter.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2022-04-24 16:03:28.000000 django-migration-linter-4.1.0/django_migration_linter.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)      156 2022-04-24 16:03:28.000000 django-migration-linter-4.1.0/django_migration_linter.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       24 2022-04-24 16:03:28.000000 django-migration-linter-4.1.0/django_migration_linter.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.930713 django-migration-linter-4.1.0/docs/
--rw-rw-r--   0 david     (1000) david     (1000)    12310 2022-03-12 11:57:16.000000 django-migration-linter-4.1.0/docs/incompatibilities.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.930713 django-migration-linter-4.1.0/docs/internals/
--rw-r--r--   0 david     (1000) david     (1000)      594 2020-01-19 16:33:23.000000 django-migration-linter-4.1.0/docs/internals/cache.md
--rw-rw-r--   0 david     (1000) david     (1000)      258 2022-01-28 18:11:14.000000 django-migration-linter-4.1.0/docs/internals/publishing.md
--rw-r--r--   0 david     (1000) david     (1000)      809 2021-02-04 18:07:32.000000 django-migration-linter-4.1.0/docs/internals/testing.md
--rw-rw-r--   0 david     (1000) david     (1000)     1511 2022-03-16 16:54:06.000000 django-migration-linter-4.1.0/docs/makemigrations.md
--rw-rw-r--   0 david     (1000) david     (1000)     7830 2022-03-16 16:54:06.000000 django-migration-linter-4.1.0/docs/usage.md
--rw-r--r--   0 david     (1000) david     (1000)      228 2022-04-24 16:03:28.942714 django-migration-linter-4.1.0/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     2097 2022-01-28 20:28:05.000000 django-migration-linter-4.1.0/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.930713 django-migration-linter-4.1.0/tests/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-01-19 11:56:14.000000 django-migration-linter-4.1.0/tests/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      763 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/fixtures.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.930713 django-migration-linter-4.1.0/tests/functional/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-01-19 11:56:14.000000 django-migration-linter-4.1.0/tests/functional/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     9699 2022-01-28 18:11:14.000000 django-migration-linter-4.1.0/tests/functional/test_cache.py
--rw-rw-r--   0 david     (1000) david     (1000)    11464 2022-03-16 16:54:06.000000 django-migration-linter-4.1.0/tests/functional/test_data_migrations.py
--rw-rw-r--   0 david     (1000) david     (1000)     1340 2022-03-12 11:57:16.000000 django-migration-linter-4.1.0/tests/functional/test_lintmigrations_command.py
--rw-rw-r--   0 david     (1000) david     (1000)     8296 2022-01-28 18:11:14.000000 django-migration-linter-4.1.0/tests/functional/test_makemigrations_command.py
--rw-rw-r--   0 david     (1000) david     (1000)     4386 2021-06-12 11:40:31.000000 django-migration-linter-4.1.0/tests/functional/test_migration_linter.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.930713 django-migration-linter-4.1.0/tests/test_project/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_add_manytomany_field/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-10-21 20:27:47.000000 django-migration-linter-4.1.0/tests/test_project/app_add_manytomany_field/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_add_manytomany_field/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      984 2019-10-21 20:27:47.000000 django-migration-linter-4.1.0/tests/test_project/app_add_manytomany_field/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      397 2019-10-21 20:27:47.000000 django-migration-linter-4.1.0/tests/test_project/app_add_manytomany_field/migrations/0002_b_many_to_many.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-10-21 20:27:47.000000 django-migration-linter-4.1.0/tests/test_project/app_add_manytomany_field/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      133 2019-10-21 20:27:47.000000 django-migration-linter-4.1.0/tests/test_project/app_add_manytomany_field/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      657 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column/migrations/0001_create_table.py
--rw-r--r--   0 david     (1000) david     (1000)      420 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column/migrations/0002_add_new_not_null_field.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      159 2020-06-12 08:25:31.000000 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column_followed_by_default/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column_followed_by_default/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column_followed_by_default/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      709 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column_followed_by_default/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      563 2021-02-04 18:07:32.000000 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column_followed_by_default/migrations/0002_a_not_null_field.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column_followed_by_default/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      217 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_add_not_null_column_followed_by_default/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_alter_column/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_alter_column/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_alter_column/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      718 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_alter_column/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      439 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_alter_column/migrations/0002_auto_20190414_1456.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_alter_column/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      174 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_alter_column/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_alter_column_drop_not_null/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-07-29 19:05:31.000000 django-migration-linter-4.1.0/tests/test_project/app_alter_column_drop_not_null/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_alter_column_drop_not_null/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      662 2019-07-29 19:05:31.000000 django-migration-linter-4.1.0/tests/test_project/app_alter_column_drop_not_null/migrations/0001_create_table.py
--rw-r--r--   0 david     (1000) david     (1000)      364 2019-07-29 19:05:31.000000 django-migration-linter-4.1.0/tests/test_project/app_alter_column_drop_not_null/migrations/0002_drop_not_null.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-07-29 19:05:31.000000 django-migration-linter-4.1.0/tests/test_project/app_alter_column_drop_not_null/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      106 2019-07-29 19:05:31.000000 django-migration-linter-4.1.0/tests/test_project/app_alter_column_drop_not_null/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_correct/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_correct/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_correct/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      657 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_correct/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      338 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_correct/migrations/0002_foo.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_correct/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      154 2020-06-20 20:02:00.000000 django-migration-linter-4.1.0/tests/test_project/app_correct/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_create_table_with_not_null_column/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_create_table_with_not_null_column/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_create_table_with_not_null_column/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      720 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_create_table_with_not_null_column/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_create_table_with_not_null_column/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      176 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_create_table_with_not_null_column/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_data_migrations/
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_data_migrations/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_data_migrations/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      649 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_data_migrations/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      290 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_data_migrations/migrations/0002_missing_reverse.py
--rw-r--r--   0 david     (1000) david     (1000)      375 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_data_migrations/migrations/0003_incorrect_arguments.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_data_migrations/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)       96 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_data_migrations/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_drop_column/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_drop_column/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_drop_column/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      773 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_drop_column/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      322 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_drop_column/migrations/0002_remove_a_field_b.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_drop_column/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      155 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_drop_column/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.934713 django-migration-linter-4.1.0/tests/test_project/app_drop_table/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-07-29 21:16:32.000000 django-migration-linter-4.1.0/tests/test_project/app_drop_table/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_drop_table/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      711 2019-07-29 21:16:32.000000 django-migration-linter-4.1.0/tests/test_project/app_drop_table/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      234 2019-07-29 21:16:32.000000 django-migration-linter-4.1.0/tests/test_project/app_drop_table/migrations/0002_delete_a.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-07-29 21:16:32.000000 django-migration-linter-4.1.0/tests/test_project/app_drop_table/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      157 2021-02-04 18:07:32.000000 django-migration-linter-4.1.0/tests/test_project/app_drop_table/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_ignore_migration/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_ignore_migration/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_ignore_migration/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      648 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_ignore_migration/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      486 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_ignore_migration/migrations/0002_ignore_migration.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_ignore_migration/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      147 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_ignore_migration/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_django_default/
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_django_default/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_django_default/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      661 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_django_default/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      412 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_django_default/migrations/0002_make_not_null_with_django_default.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_django_default/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      125 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_django_default/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_lib_default/
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_lib_default/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_lib_default/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      661 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_lib_default/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      532 2021-02-04 18:07:32.000000 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_lib_default/migrations/0002_make_not_null_with_lib_default.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_lib_default/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      126 2020-06-20 17:05:25.000000 django-migration-linter-4.1.0/tests/test_project/app_make_not_null_with_lib_default/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_rename_column/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_rename_column/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_rename_column/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      709 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_rename_column/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      360 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_rename_column/migrations/0002_auto_20190414_1502.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_rename_column/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      155 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_rename_column/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_rename_table/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_rename_table/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_rename_table/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      709 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_rename_table/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      319 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_rename_table/migrations/0002_auto_20190414_1500.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_rename_table/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      153 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/app_rename_table/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_unique_together/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-07-30 08:47:39.000000 django-migration-linter-4.1.0/tests/test_project/app_unique_together/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/app_unique_together/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      711 2019-07-30 08:47:39.000000 django-migration-linter-4.1.0/tests/test_project/app_unique_together/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)      327 2019-07-30 08:47:39.000000 django-migration-linter-4.1.0/tests/test_project/app_unique_together/migrations/0002_auto_20190729_2122.py
--rw-r--r--   0 david     (1000) david     (1000)      278 2019-07-30 08:47:39.000000 django-migration-linter-4.1.0/tests/test_project/app_unique_together/migrations/0003_auto_20190729_2122.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-07-30 08:47:39.000000 django-migration-linter-4.1.0/tests/test_project/app_unique_together/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      220 2019-07-30 08:47:39.000000 django-migration-linter-4.1.0/tests/test_project/app_unique_together/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/makemigrations_backward_incompatible_migration_missing/
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-07-03 17:13:04.000000 django-migration-linter-4.1.0/tests/test_project/makemigrations_backward_incompatible_migration_missing/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/makemigrations_backward_incompatible_migration_missing/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      638 2020-07-03 17:13:04.000000 django-migration-linter-4.1.0/tests/test_project/makemigrations_backward_incompatible_migration_missing/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-07-03 17:13:04.000000 django-migration-linter-4.1.0/tests/test_project/makemigrations_backward_incompatible_migration_missing/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      162 2020-07-03 17:13:04.000000 django-migration-linter-4.1.0/tests/test_project/makemigrations_backward_incompatible_migration_missing/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/makemigrations_correct_migration_missing/
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-07-03 17:13:04.000000 django-migration-linter-4.1.0/tests/test_project/makemigrations_correct_migration_missing/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/test_project/makemigrations_correct_migration_missing/migrations/
--rw-r--r--   0 david     (1000) david     (1000)      638 2020-07-03 17:13:04.000000 django-migration-linter-4.1.0/tests/test_project/makemigrations_correct_migration_missing/migrations/0001_initial.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-07-03 17:13:04.000000 django-migration-linter-4.1.0/tests/test_project/makemigrations_correct_migration_missing/migrations/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      144 2020-07-03 17:13:04.000000 django-migration-linter-4.1.0/tests/test_project/makemigrations_correct_migration_missing/models.py
--rw-rw-r--   0 david     (1000) david     (1000)     4471 2022-01-28 18:15:57.000000 django-migration-linter-4.1.0/tests/test_project/settings.py
--rw-rw-r--   0 david     (1000) david     (1000)      747 2022-01-28 20:28:05.000000 django-migration-linter-4.1.0/tests/test_project/urls.py
--rw-r--r--   0 david     (1000) david     (1000)      401 2019-05-12 13:38:36.000000 django-migration-linter-4.1.0/tests/test_project/wsgi.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-04-24 16:03:28.938713 django-migration-linter-4.1.0/tests/unit/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-01-19 11:56:14.000000 django-migration-linter-4.1.0/tests/unit/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     6392 2021-02-04 18:07:32.000000 django-migration-linter-4.1.0/tests/unit/test_linter.py
--rw-rw-r--   0 david     (1000) david     (1000)    15640 2022-01-30 14:20:23.000000 django-migration-linter-4.1.0/tests/unit/test_sql_analyser.py
--rw-r--r--   0 david     (1000) david     (1000)     1595 2021-02-04 18:07:32.000000 django-migration-linter-4.1.0/tests/unit/test_utils.py
--rw-rw-r--   0 david     (1000) david     (1000)      739 2022-01-28 20:28:05.000000 django-migration-linter-4.1.0/tox.ini
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-09 12:49:41.770737 django-migration-linter-5.0.0/
+-rw-r--r--   0 david      (501) staff       (20)    11362 2023-07-09 12:43:25.000000 django-migration-linter-5.0.0/CHANGELOG.md
+-rw-r--r--   0 david      (501) staff       (20)    10173 2022-07-09 13:06:11.000000 django-migration-linter-5.0.0/LICENSE
+-rw-r--r--   0 david      (501) staff       (20)      116 2022-12-17 10:58:07.000000 django-migration-linter-5.0.0/MANIFEST.in
+-rw-r--r--   0 david      (501) staff       (20)     5969 2023-07-09 12:49:41.770823 django-migration-linter-5.0.0/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     4963 2022-10-03 13:49:14.000000 django-migration-linter-5.0.0/README.md
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-09 12:49:41.767814 django-migration-linter-5.0.0/django_migration_linter/
+-rw-r--r--   0 david      (501) staff       (20)      110 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/django_migration_linter/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)      801 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/django_migration_linter/cache.py
+-rw-r--r--   0 david      (501) staff       (20)      313 2023-07-09 12:43:43.000000 django-migration-linter-5.0.0/django_migration_linter/constants.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-09 12:49:41.768674 django-migration-linter-5.0.0/django_migration_linter/management/
+-rw-r--r--   0 david      (501) staff       (20)        0 2022-07-09 13:06:11.000000 django-migration-linter-5.0.0/django_migration_linter/management/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-09 12:49:41.769065 django-migration-linter-5.0.0/django_migration_linter/management/commands/
+-rw-r--r--   0 david      (501) staff       (20)        0 2022-07-09 13:06:11.000000 django-migration-linter-5.0.0/django_migration_linter/management/commands/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     8005 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/django_migration_linter/management/commands/lintmigrations.py
+-rw-r--r--   0 david      (501) staff       (20)     4307 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/django_migration_linter/management/commands/makemigrations.py
+-rw-r--r--   0 david      (501) staff       (20)     1906 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/django_migration_linter/management/utils.py
+-rw-r--r--   0 david      (501) staff       (20)    26637 2023-07-09 12:27:14.000000 django-migration-linter-5.0.0/django_migration_linter/migration_linter.py
+-rw-r--r--   0 david      (501) staff       (20)      714 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/django_migration_linter/operations.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-09 12:49:41.769863 django-migration-linter-5.0.0/django_migration_linter/sql_analyser/
+-rw-r--r--   0 david      (501) staff       (20)      299 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/django_migration_linter/sql_analyser/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     2226 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/django_migration_linter/sql_analyser/analyser.py
+-rw-r--r--   0 david      (501) staff       (20)     7368 2023-07-09 12:27:14.000000 django-migration-linter-5.0.0/django_migration_linter/sql_analyser/base.py
+-rw-r--r--   0 david      (501) staff       (20)     1011 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/django_migration_linter/sql_analyser/mysql.py
+-rw-r--r--   0 david      (501) staff       (20)     3415 2023-07-09 12:42:44.000000 django-migration-linter-5.0.0/django_migration_linter/sql_analyser/postgresql.py
+-rw-r--r--   0 david      (501) staff       (20)     1949 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/django_migration_linter/sql_analyser/sqlite.py
+-rw-r--r--   0 david      (501) staff       (20)     1661 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/django_migration_linter/utils.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-09 12:49:41.768442 django-migration-linter-5.0.0/django_migration_linter.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)     5969 2023-07-09 12:49:41.000000 django-migration-linter-5.0.0/django_migration_linter.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     1224 2023-07-09 12:49:41.000000 django-migration-linter-5.0.0/django_migration_linter.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-07-09 12:49:41.000000 django-migration-linter-5.0.0/django_migration_linter.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)      142 2023-07-09 12:49:41.000000 django-migration-linter-5.0.0/django_migration_linter.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       24 2023-07-09 12:49:41.000000 django-migration-linter-5.0.0/django_migration_linter.egg-info/top_level.txt
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-09 12:49:41.770246 django-migration-linter-5.0.0/docs/
+-rw-r--r--   0 david      (501) staff       (20)    12484 2023-07-09 12:42:44.000000 django-migration-linter-5.0.0/docs/incompatibilities.md
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-09 12:49:41.770617 django-migration-linter-5.0.0/docs/internals/
+-rw-r--r--   0 david      (501) staff       (20)      594 2022-07-09 13:06:11.000000 django-migration-linter-5.0.0/docs/internals/cache.md
+-rw-r--r--   0 david      (501) staff       (20)      330 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/docs/internals/publishing.md
+-rw-r--r--   0 david      (501) staff       (20)      810 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/docs/internals/testing.md
+-rw-r--r--   0 david      (501) staff       (20)     1511 2022-07-09 13:06:11.000000 django-migration-linter-5.0.0/docs/makemigrations.md
+-rw-r--r--   0 david      (501) staff       (20)     7939 2022-12-26 15:26:33.000000 django-migration-linter-5.0.0/docs/usage.md
+-rw-r--r--   0 david      (501) staff       (20)      298 2023-07-09 12:49:41.771090 django-migration-linter-5.0.0/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)     2202 2023-07-09 12:27:14.000000 django-migration-linter-5.0.0/setup.py
+-rw-r--r--   0 david      (501) staff       (20)      791 2023-07-09 12:27:14.000000 django-migration-linter-5.0.0/tox.ini
```

### Comparing `django-migration-linter-4.1.0/CHANGELOG.md` & `django-migration-linter-5.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+## 5.0.0
+
+- **Breaking change**: stop silently ignoring when the internal `sqlmigrate` call fails and the linter cannot analyse the migration.
+Instead, the linter crashes and lets the `sqlmigrate` error raise, in order to avoid letting a problematic migration pass.
+One common reason for such an error is the SQL generation which requires the database to be actually migrated in order to fetch actual constraint names from it.
+The crash is a sign to double-check the migration. But if you are certain the migration is safe, you can ignore it (issue #209)
+
+Features:
+
+- Fixed `RunPython` model import check when using a `through` object like `MyModel.many_to_many.through.objects.filter(...)` (issue #218)
+- Mark the `IgnoreMigration` operation as `elidable=True`
+- Handle `functools.partial` functions in RunPython data migrations
+- Add a new check, `CREATE_INDEX_EXCLUSIVE` to detect index creation while an exclusive lock is held
+
+Bug:
+
+- Don't detect not nullable field on partial index creation (issue #250)
+
+Miscellaneous:
+
+- Add support for Python 3.11
+- Add support for Django 4.1
+- Add support for Django 4.2
+- Drop support for Django 2.2
+- Internally rename "migration tests" to "migration checks"
+- Add dataclasses internally instead of custom dicts
+- Use pre-commit hooks for linting
+- Add `mypy` and `ruff` usages
+
 ## 4.1.0
 
 - Allow configuring logging for `makemigrations` command and unify behaviour with `lintmigrations` (issue #207)
 - Adapt `--warnings-as-errors` option to allow selecting some migration tests only (issue #201)
 - Add `sql_analyser` option to `makemigrations` in order to specify the SQL analyser to use (issue #208)
 - Make `project_root_path` and `verbosity` configurable from other setting source (issue #203)
```

### Comparing `django-migration-linter-4.1.0/LICENSE` & `django-migration-linter-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-migration-linter-4.1.0/PKG-INFO` & `django-migration-linter-5.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,133 +1,144 @@
 Metadata-Version: 2.1
 Name: django-migration-linter
-Version: 4.1.0
+Version: 5.0.0
 Summary: Detect backward incompatible migrations for your django project
 Home-page: https://github.com/3YOURMIND/django-migration-linter
 Author: 3YOURMIND GmbH
 Author-email: david.wobrock@gmail.com
 License: Apache License 2.0
-Description: # Django migration linter
-        
-        Detect backward incompatible migrations for your Django project.
-        It will save you time by making sure migrations will not break with a older codebase.
-        
-        [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2F3YOURMIND%2Fdjango-migration-linter%2Fbadge%3Fref%3Dmain&style=flat)](https://actions-badge.atrox.dev/3YOURMIND/django-migration-linter/goto?ref=main)
-        [![codecov](https://codecov.io/gh/3YOURMIND/django-migration-linter/branch/master/graph/badge.svg?token=pgNNXGbCf7)](https://codecov.io/gh/3YOURMIND/django-migration-linter)
-        [![PyPI](https://img.shields.io/pypi/v/django-migration-linter.svg)](https://pypi.python.org/pypi/django-migration-linter/)
-        [![PR_Welcome](https://img.shields.io/badge/PR-welcome-green.svg)](https://github.com/3YOURMIND/django-migration-linter/pulls)
-        [![3YD_Hiring](https://img.shields.io/badge/3YOURMIND-Hiring-brightgreen.svg)](https://www.3yourmind.com/career)
-        [![GitHub_Stars](https://img.shields.io/github/stars/3YOURMIND/django-migration-linter.svg?style=social&label=Stars)](https://github.com/3YOURMIND/django-migration-linter/stargazers)
-        
-        ## Quick installation
-        
-        ```
-        pip install django-migration-linter
-        ```
-        
-        And add the migration linter your ``INSTALLED_APPS``:
-        ```
-            INSTALLED_APPS = [
-                ...,
-                "django_migration_linter",
-                ...,
-            ]
-        ```
-        
-        ## Usage example
-        
-        ```
-        $ python manage.py lintmigrations
-        
-        (app_add_not_null_column, 0001_create_table)... OK
-        (app_add_not_null_column, 0002_add_new_not_null_field)... ERR
-                NOT NULL constraint on columns
-        (app_drop_table, 0001_initial)... OK
-        (app_drop_table, 0002_delete_a)... ERR
-                DROPPING table
-        (app_ignore_migration, 0001_initial)... OK
-        (app_ignore_migration, 0002_ignore_migration)... IGNORE
-        (app_rename_table, 0001_initial)... OK
-        (app_rename_table, 0002_auto_20190414_1500)... ERR
-                RENAMING tables
-        
-        *** Summary ***
-        Valid migrations: 4/8
-        Erroneous migrations: 3/8
-        Migrations with warnings: 0/8
-        Ignored migrations: 1/8
-        ```
-        
-        The linter analysed all migrations from the Django project.
-        It found 3 migrations that are doing backward incompatible operations and 1 that is explicitly ignored.
-        The list of incompatibilities that the linter analyses [can be found at docs/incompatibilities.md](./docs/incompatibilities.md).
-        
-        More advanced usages of the linter and options [can be found at docs/usage.md](./docs/usage.md).
-        
-        ## Integration
-        
-        One can either integrate the linter in the CI using its `lintmigrations` command, or detect incompatibilities during generation of migrations with
-        ```
-        $ python manage.py makemigrations --lint
-        
-        Migrations for 'app_correct':
-          tests/test_project/app_correct/migrations/0003_a_column.py
-            - Add field column to a
-        Linting for 'app_correct':
-        (app_correct, 0003_a_column)... ERR
-                NOT NULL constraint on columns
-        
-        The migration linter detected that this migration is not backward compatible.
-        - If you keep the migration, you will want to fix the issue or ignore the migration.
-        - By default, the newly created migration file will be deleted.
-        Do you want to keep the migration? [y/N] n
-        Deleted tests/test_project/app_correct/migrations/0003_a_column.py
-        ```
-        
-        The linter found that the newly created migration is not backward compatible and deleted the file after confirmation.
-        This behaviour can be the default of the `makemigrations` command through the `MIGRATION_LINTER_OVERRIDE_MAKEMIGRATIONS` Django setting.
-        Find out more about the [makemigrations command at docs/makemigrations.md](./docs/makemigrations.md).
-        
-        ### More information
-        
-        Please find more documentation [in the docs/ folder](./docs/).
-        
-        Some implementation details [can be found in the ./docs/internals/ folder](./docs/internals/).
-        
-        ### Blog post
-        
-        * [Keeping Django database migrations backward compatible](https://medium.com/3yourmind/keeping-django-database-migrations-backward-compatible-727820260dbb)
-        * [Django and its default values](https://medium.com/botify-labs/django-and-its-default-values-c21a13cff9f)
-        
-        ### They talk about the linter
-        
-        * [Django News](https://django-news.com/issues/6?m=web#uMmosw7)
-        * [wemake-django-template](https://wemake-django-template.readthedocs.io/en/latest/pages/template/linters.html#django-migration-linter)
-        * [Testing Django migrations on sobolevn's blog](https://sobolevn.me/2019/10/testing-django-migrations#existing-setup)
-        
-        ### Related
-        
-        * [django-test-migrations](https://github.com/wemake-services/django-test-migrations) - Test django schema and data migrations, including migrations' order and best practices.
-        
-        ### License
-        
-        *django-migration-linter* is released under the [Apache 2.0 License](./LICENSE).
-        
-        ##### Maintained by [David Wobrock](https://github.com/David-Wobrock)
-        
 Keywords: django migration lint linter database backward compatibility
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# Django migration linter
+
+Detect backward incompatible migrations for your Django project.
+It will save you time by making sure migrations will not break with a older codebase.
+
+[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2F3YOURMIND%2Fdjango-migration-linter%2Fbadge%3Fref%3Dmain&style=flat)](https://actions-badge.atrox.dev/3YOURMIND/django-migration-linter/goto?ref=main)
+[![codecov](https://codecov.io/gh/3YOURMIND/django-migration-linter/branch/master/graph/badge.svg?token=pgNNXGbCf7)](https://codecov.io/gh/3YOURMIND/django-migration-linter)
+[![PyPI](https://img.shields.io/pypi/v/django-migration-linter.svg)](https://pypi.python.org/pypi/django-migration-linter/)
+[![PR_Welcome](https://img.shields.io/badge/PR-welcome-green.svg)](https://github.com/3YOURMIND/django-migration-linter/pulls)
+[![3YD_Hiring](https://img.shields.io/badge/3YOURMIND-Hiring-brightgreen.svg)](https://www.3yourmind.com/career)
+[![GitHub_Stars](https://img.shields.io/github/stars/3YOURMIND/django-migration-linter.svg?style=social&label=Stars)](https://github.com/3YOURMIND/django-migration-linter/stargazers)
+
+## Quick installation
+
+```
+pip install django-migration-linter
+```
+
+And add the migration linter to your ``INSTALLED_APPS``:
+```
+INSTALLED_APPS = [
+    ...,
+    "django_migration_linter",
+    ...,
+]
+```
+
+Optionally, add a configuration:
+```
+MIGRATION_LINTER_OPTIONS = {
+    ...
+}
+```
+
+For details about configuration options, checkout [Usage](docs/usage.md).
+
+## Usage example
+
+```
+$ python manage.py lintmigrations
+
+(app_add_not_null_column, 0001_create_table)... OK
+(app_add_not_null_column, 0002_add_new_not_null_field)... ERR
+        NOT NULL constraint on columns
+(app_drop_table, 0001_initial)... OK
+(app_drop_table, 0002_delete_a)... ERR
+        DROPPING table
+(app_ignore_migration, 0001_initial)... OK
+(app_ignore_migration, 0002_ignore_migration)... IGNORE
+(app_rename_table, 0001_initial)... OK
+(app_rename_table, 0002_auto_20190414_1500)... ERR
+        RENAMING tables
+
+*** Summary ***
+Valid migrations: 4/8
+Erroneous migrations: 3/8
+Migrations with warnings: 0/8
+Ignored migrations: 1/8
+```
+
+The linter analysed all migrations from the Django project.
+It found 3 migrations that are doing backward incompatible operations and 1 that is explicitly ignored.
+The list of incompatibilities that the linter analyses [can be found at docs/incompatibilities.md](./docs/incompatibilities.md).
+
+More advanced usages of the linter and options [can be found at docs/usage.md](./docs/usage.md).
+
+## Integration
+
+One can either integrate the linter in the CI using its `lintmigrations` command, or detect incompatibilities during generation of migrations with
+```
+$ python manage.py makemigrations --lint
+
+Migrations for 'app_correct':
+  tests/test_project/app_correct/migrations/0003_a_column.py
+    - Add field column to a
+Linting for 'app_correct':
+(app_correct, 0003_a_column)... ERR
+        NOT NULL constraint on columns
+
+The migration linter detected that this migration is not backward compatible.
+- If you keep the migration, you will want to fix the issue or ignore the migration.
+- By default, the newly created migration file will be deleted.
+Do you want to keep the migration? [y/N] n
+Deleted tests/test_project/app_correct/migrations/0003_a_column.py
+```
+
+The linter found that the newly created migration is not backward compatible and deleted the file after confirmation.
+This behaviour can be the default of the `makemigrations` command through the `MIGRATION_LINTER_OVERRIDE_MAKEMIGRATIONS` Django setting.
+Find out more about the [makemigrations command at docs/makemigrations.md](./docs/makemigrations.md).
+
+### More information
+
+Please find more documentation [in the docs/ folder](./docs/).
+
+Some implementation details [can be found in the ./docs/internals/ folder](./docs/internals/).
+
+### Blog post
+
+* [Keeping Django database migrations backward compatible](https://medium.com/3yourmind/keeping-django-database-migrations-backward-compatible-727820260dbb)
+* [Django and its default values](https://medium.com/botify-labs/django-and-its-default-values-c21a13cff9f)
+
+### They talk about the linter
+
+* [Django News](https://django-news.com/issues/6?m=web#uMmosw7)
+* [wemake-django-template](https://wemake-django-template.readthedocs.io/en/latest/pages/template/linters.html#django-migration-linter)
+* [Testing Django migrations on sobolevn's blog](https://sobolevn.me/2019/10/testing-django-migrations#existing-setup)
+
+### Related
+
+* [django-test-migrations](https://github.com/wemake-services/django-test-migrations) - Test django schema and data migrations, including migrations' order and best practices.
+
+### License
+
+*django-migration-linter* is released under the [Apache 2.0 License](./LICENSE).
+
+##### Maintained by [David Wobrock](https://github.com/David-Wobrock)
```

### Comparing `django-migration-linter-4.1.0/README.md` & `django-migration-linter-5.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,32 @@
 
 ## Quick installation
 
 ```
 pip install django-migration-linter
 ```
 
-And add the migration linter your ``INSTALLED_APPS``:
+And add the migration linter to your ``INSTALLED_APPS``:
 ```
-    INSTALLED_APPS = [
-        ...,
-        "django_migration_linter",
-        ...,
-    ]
+INSTALLED_APPS = [
+    ...,
+    "django_migration_linter",
+    ...,
+]
 ```
 
+Optionally, add a configuration:
+```
+MIGRATION_LINTER_OPTIONS = {
+    ...
+}
+```
+
+For details about configuration options, checkout [Usage](docs/usage.md).
+
 ## Usage example
 
 ```
 $ python manage.py lintmigrations
 
 (app_add_not_null_column, 0001_create_table)... OK
 (app_add_not_null_column, 0002_add_new_not_null_field)... ERR
```

### Comparing `django-migration-linter-4.1.0/django_migration_linter/cache.py` & `django-migration-linter-5.0.0/django_migration_linter/cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+from __future__ import annotations
+
 import os
 import pickle
 
 
 class Cache(dict):
-    def __init__(self, django_folder, database, cache_path):
+    def __init__(self, django_folder: str | None, database: str, cache_path: str):
         self.filename = os.path.join(
             cache_path,
-            "{0}_{1}.pickle".format(django_folder.replace(os.sep, "_"), database),
+            "{}_{}.pickle".format(str(django_folder).replace(os.sep, "_"), database),
         )
 
         if not os.path.exists(os.path.dirname(self.filename)):
             os.makedirs(os.path.dirname(self.filename))
 
-        super(Cache, self).__init__()
+        super().__init__()
 
-    def load(self):
+    def load(self) -> None:
         try:
             with open(self.filename, "rb") as f:
                 tmp_dict = pickle.load(f)
                 self.update(tmp_dict)
-        except IOError:
+        except OSError:
             pass
 
-    def save(self):
+    def save(self) -> None:
         with open(self.filename, "wb") as f:
             pickle.dump(self, f, protocol=2)
```

### Comparing `django-migration-linter-4.1.0/django_migration_linter/management/commands/lintmigrations.py` & `django-migration-linter-5.0.0/django_migration_linter/management/commands/lintmigrations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,41 @@
+from __future__ import annotations
+
 import configparser
 import itertools
 import os
 import sys
 from importlib import import_module
+from typing import Any, Callable
 
 import toml
 from django.conf import settings
-from django.core.management.base import BaseCommand
+from django.core.management.base import BaseCommand, CommandParser
 
 from ...constants import __version__
 from ...migration_linter import MessageType, MigrationLinter
 from ..utils import (
     configure_logging,
     extract_warnings_as_errors_option,
     register_linting_configuration_options,
 )
 
 CONFIG_NAME = "django_migration_linter"
 PYPROJECT_TOML = "pyproject.toml"
 DEFAULT_CONFIG_FILES = (
-    ".{}.cfg".format(CONFIG_NAME),
+    f".{CONFIG_NAME}.cfg",
     "setup.cfg",
     "tox.ini",
 )
 
 
 class Command(BaseCommand):
     help = "Lint your migrations"
 
-    def add_arguments(self, parser):
+    def add_arguments(self, parser: CommandParser) -> None:
         parser.add_argument(
             "app_label",
             nargs="?",
             type=str,
             help="App label of an application to lint migrations.",
         )
         parser.add_argument(
@@ -180,51 +183,52 @@
             migrations_file_path=options["include_migrations_from"],
         )
         linter.print_summary()
         if linter.has_errors:
             sys.exit(1)
 
     @staticmethod
-    def read_django_settings(options):
+    def read_django_settings(options: dict[str, Any]) -> dict[str, Any]:
         django_settings_options = dict()
 
         django_migration_linter_settings = getattr(
             settings, "MIGRATION_LINTER_OPTIONS", dict()
         )
         for key in options:
             if key in django_migration_linter_settings:
                 django_settings_options[key] = django_migration_linter_settings[key]
 
         return django_settings_options
 
     @staticmethod
-    def read_config_file(options):
+    def read_config_file(options: dict[str, Any]) -> dict[str, Any]:
         config_options = dict()
 
         config_parser = configparser.ConfigParser()
         config_parser.read(DEFAULT_CONFIG_FILES, encoding="utf-8")
         for key, value in options.items():
+            config_get_fn: Callable
             if isinstance(value, bool):
                 config_get_fn = config_parser.getboolean
             else:
                 config_get_fn = config_parser.get
 
             config_value = config_get_fn(CONFIG_NAME, key, fallback=None)
             if config_value is not None:
                 config_options[key] = config_value
         return config_options
 
     @staticmethod
-    def read_toml_file(options):
+    def read_toml_file(options: dict[str, Any]) -> dict[str, Any]:
         toml_options = dict()
 
         if os.path.exists(PYPROJECT_TOML):
             pyproject_toml = toml.load(PYPROJECT_TOML)
             section = pyproject_toml.get("tool", {}).get(CONFIG_NAME, {})
             for key in options:
                 if key in section:
                     toml_options[key] = section[key]
 
         return toml_options
 
-    def get_version(self):
+    def get_version(self) -> str:
         return __version__
```

### Comparing `django-migration-linter-4.1.0/django_migration_linter/management/commands/makemigrations.py` & `django-migration-linter-5.0.0/django_migration_linter/management/commands/makemigrations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,66 @@
+from __future__ import annotations
+
 import os
 
 from django.conf import settings
+from django.core.management import CommandParser
 from django.core.management.commands.makemigrations import (
     Command as MakeMigrationsCommand,
 )
+from django.db.migrations import Migration
 from django.db.migrations.questioner import InteractiveMigrationQuestioner
 from django.db.migrations.writer import MigrationWriter
 
 from django_migration_linter import MigrationLinter
 
 from ..utils import (
     configure_logging,
     extract_warnings_as_errors_option,
     register_linting_configuration_options,
 )
 
 
-def ask_should_keep_migration():
+def ask_should_keep_migration() -> bool:
     questioner = InteractiveMigrationQuestioner()
-    msg = """\nThe migration linter detected that this migration is not backward compatible.
+    msg = """
+The migration linter detected that this migration is not backward compatible.
 - If you keep the migration, you will want to fix the issue or ignore the migration.
 - By default, the newly created migration file will be deleted.
 Do you want to keep the migration? [y/N]"""
     return questioner._boolean_input(msg, False)
 
 
 def default_should_keep_migration():
     return False
 
 
 class Command(MakeMigrationsCommand):
     help = "Creates new migration(s) for apps and lints them."
 
-    def add_arguments(self, parser):
-        super(Command, self).add_arguments(parser)
+    def add_arguments(self, parser: CommandParser) -> None:
+        super().add_arguments(parser)
         parser.add_argument(
             "--lint",
             action="store_true",
             help="Lint newly generated migrations.",
         )
         register_linting_configuration_options(parser)
 
     def handle(self, *app_labels, **options):
         self.lint = options["lint"]
         self.database = options["database"]
         self.exclude_migrations_tests = options["exclude_migration_tests"]
         self.warnings_as_errors = options["warnings_as_errors"]
         self.sql_analyser = options["sql_analyser"]
         configure_logging(options["verbosity"])
-        return super(Command, self).handle(*app_labels, **options)
+        return super().handle(*app_labels, **options)
 
-    def write_migration_files(self, changes):
-        super(Command, self).write_migration_files(changes)
+    def write_migration_files(self, changes: dict[str, list[Migration]]) -> None:
+        super().write_migration_files(changes)
 
         if (
             not getattr(settings, "MIGRATION_LINTER_OVERRIDE_MAKEMIGRATIONS", False)
             and not self.lint
         ):
             return
 
@@ -74,15 +79,15 @@
         )
 
         (
             warnings_as_errors_tests,
             all_warnings_as_errors,
         ) = extract_warnings_as_errors_option(self.warnings_as_errors)
 
-        # Lint migrations
+        # Lint migrations.
         linter = MigrationLinter(
             path=os.environ["DJANGO_SETTINGS_MODULE"],
             database=self.database,
             no_cache=True,
             exclude_migration_tests=self.exclude_migrations_tests,
             warnings_as_errors_tests=warnings_as_errors_tests,
             all_warnings_as_errors=all_warnings_as_errors,
@@ -98,15 +103,15 @@
             for migration in app_migrations:
                 linter.lint_migration(migration)
                 if linter.has_errors:
                     if not should_keep_migration():
                         self.delete_migration(migration)
                 linter.reset_counters()
 
-    def delete_migration(self, migration):
+    def delete_migration(self, migration: Migration) -> None:
         writer = MigrationWriter(migration)
         os.remove(writer.path)
 
         if self.verbosity >= 1:
             try:
                 migration_string = os.path.relpath(writer.path)
             except ValueError:
```

### Comparing `django-migration-linter-4.1.0/django_migration_linter/management/utils.py` & `django-migration-linter-5.0.0/django_migration_linter/management/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+from __future__ import annotations
+
 import logging
 
+from django.core.management import CommandParser
+
 from ..sql_analyser.analyser import ANALYSER_STRING_MAPPING
 
 
-def register_linting_configuration_options(parser):
+def register_linting_configuration_options(parser: CommandParser) -> None:
     parser.add_argument(
         "--database",
         type=str,
         nargs="?",
         help=(
             "specify the database for which to generate the SQL. Defaults to default"
         ),
@@ -33,26 +37,28 @@
         "--sql-analyser",
         nargs="?",
         choices=list(ANALYSER_STRING_MAPPING.keys()),
         help="select the SQL analyser",
     )
 
 
-def configure_logging(verbosity):
+def configure_logging(verbosity: int) -> None:
     logger = logging.getLogger("django_migration_linter")
 
     if verbosity > 1:
         logging.basicConfig(format="%(message)s", level=logging.DEBUG)
     elif verbosity == 0:
         logger.disabled = True
     else:
         logging.basicConfig(format="%(message)s")
 
 
-def extract_warnings_as_errors_option(warnings_as_errors):
+def extract_warnings_as_errors_option(
+    warnings_as_errors: list[str] | None,
+) -> tuple[list[str] | None, bool]:
     if isinstance(warnings_as_errors, list):
         warnings_as_errors_tests = warnings_as_errors
         # If the option is specified but without any test codes,
         # all warnings become errors
         all_warnings_as_errors = len(warnings_as_errors) == 0
     else:
         warnings_as_errors_tests = None
```

### Comparing `django-migration-linter-4.1.0/django_migration_linter/migration_linter.py` & `django-migration-linter-5.0.0/django_migration_linter/migration_linter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,79 @@
-from __future__ import print_function
+from __future__ import annotations
 
+import functools
 import hashlib
 import inspect
 import logging
 import os
 import re
 from enum import Enum, unique
 from subprocess import PIPE, Popen
+from typing import Callable, Iterable
 
 from django.conf import settings
 from django.core.management import call_command
 from django.db import DEFAULT_DB_ALIAS, ProgrammingError, connections
-from django.db.migrations import RunPython, RunSQL
+from django.db.migrations import Migration, RunPython, RunSQL
+from django.db.migrations.operations.base import Operation
 
 from .cache import Cache
 from .constants import (
     DEFAULT_CACHE_PATH,
     DJANGO_APPS_WITH_MIGRATIONS,
     EXPECTED_DATA_MIGRATION_ARGS,
 )
 from .operations import IgnoreMigration
 from .sql_analyser import analyse_sql_statements, get_sql_analyser_class
+from .sql_analyser.base import Issue
 from .utils import clean_bytes_to_str, get_migration_abspath, split_migration_path
 
 logger = logging.getLogger("django_migration_linter")
 
 
 @unique
 class MessageType(Enum):
     OK = "ok"
     IGNORE = "ignore"
     WARNING = "warning"
     ERROR = "error"
 
     @staticmethod
-    def values():
+    def values() -> list[str]:
         return list(map(lambda c: c.value, MessageType))
 
 
-class MigrationLinter(object):
+class MigrationLinter:
     def __init__(
         self,
-        path=None,
-        ignore_name_contains=None,
-        ignore_name=None,
-        include_name_contains=None,
-        include_name=None,
-        include_apps=None,
-        exclude_apps=None,
-        database=DEFAULT_DB_ALIAS,
-        cache_path=DEFAULT_CACHE_PATH,
-        no_cache=False,
-        only_applied_migrations=False,
-        only_unapplied_migrations=False,
-        exclude_migration_tests=None,
-        quiet=None,
-        warnings_as_errors_tests=None,
-        all_warnings_as_errors=False,
-        no_output=False,
-        analyser_string=None,
+        path: str | None = None,
+        ignore_name_contains: str | None = None,
+        ignore_name: Iterable[str] | None = None,
+        include_name_contains: str | None = None,
+        include_name: Iterable[str] | None = None,
+        include_apps: Iterable[str] | None = None,
+        exclude_apps: Iterable[str] | None = None,
+        database: str = DEFAULT_DB_ALIAS,
+        cache_path: str = DEFAULT_CACHE_PATH,
+        no_cache: bool = False,
+        only_applied_migrations: bool = False,
+        only_unapplied_migrations: bool = False,
+        exclude_migration_tests: Iterable[str] | None = None,
+        quiet: Iterable[str] | None = None,
+        warnings_as_errors_tests: Iterable[str] | None = None,
+        all_warnings_as_errors: bool = False,
+        no_output: bool = False,
+        analyser_string: str | None = None,
     ):
         # Store parameters and options
         self.django_path = path
         self.ignore_name_contains = ignore_name_contains
-        self.ignore_name = ignore_name or tuple()
+        self.ignore_name = ignore_name or []
         self.include_name_contains = include_name_contains
-        self.include_name = include_name or tuple()
+        self.include_name = include_name or []
         self.include_apps = include_apps
         self.exclude_apps = exclude_apps
         self.exclude_migration_tests = exclude_migration_tests or []
         self.database = database or DEFAULT_DB_ALIAS
         self.cache_path = cache_path or DEFAULT_CACHE_PATH
         self.no_cache = no_cache
         self.only_applied_migrations = only_applied_migrations
@@ -82,52 +86,52 @@
             settings.DATABASES[self.database]["ENGINE"],
             analyser_string=analyser_string,
         )
 
         # Initialise counters
         self.reset_counters()
 
-        # Initialise cache. Read from old, write to new to prune old entries.
+        # Initialise cache. Read from old, write to new, in order to prune old entries.
         if self.should_use_cache():
             self.old_cache = Cache(self.django_path, self.database, self.cache_path)
             self.new_cache = Cache(self.django_path, self.database, self.cache_path)
             self.old_cache.load()
 
         # Initialise migrations
         from django.db.migrations.loader import MigrationLoader
 
         self.migration_loader = MigrationLoader(
             connection=connections[self.database], load=True
         )
 
-    def reset_counters(self):
+    def reset_counters(self) -> None:
         self.nb_valid = 0
         self.nb_ignored = 0
         self.nb_warnings = 0
         self.nb_erroneous = 0
         self.nb_total = 0
 
-    def should_use_cache(self):
-        return self.django_path and not self.no_cache
+    def should_use_cache(self) -> bool:
+        return bool(self.django_path and not self.no_cache)
 
     def lint_all_migrations(
         self,
-        app_label=None,
-        migration_name=None,
-        git_commit_id=None,
-        migrations_file_path=None,
-    ):
-        # Collect migrations
+        app_label: str | None = None,
+        migration_name: str | None = None,
+        git_commit_id: str | None = None,
+        migrations_file_path: str | None = None,
+    ) -> None:
+        # Collect migrations.
         migrations_list = self.read_migrations_list(migrations_file_path)
         if git_commit_id:
             migrations = self._gather_migrations_git(git_commit_id, migrations_list)
         else:
             migrations = self._gather_all_migrations(migrations_list)
 
-        # Lint those migrations
+        # Lint those migrations.
         sorted_migrations = sorted(
             migrations, key=lambda migration: (migration.app_label, migration.name)
         )
 
         specific_target_migration = (
             self.migration_loader.get_migration_by_prefix(app_label, migration_name)
             if app_label and migration_name
@@ -143,15 +147,15 @@
                     self.lint_migration(m)
             else:
                 self.lint_migration(m)
 
         if self.should_use_cache():
             self.new_cache.save()
 
-    def lint_migration(self, migration):
+    def lint_migration(self, migration: Migration) -> None:
         app_label = migration.app_label
         migration_name = migration.name
         operations = migration.operations
         self.nb_total += 1
 
         md5hash = self.get_migration_hash(app_label, migration_name)
 
@@ -183,15 +187,15 @@
 
         if self.all_warnings_as_errors:
             errors += warnings
             warnings = []
         elif self.warnings_as_errors_tests:
             new_warnings = []
             for w in warnings:
-                if w["code"] in self.warnings_as_errors_tests:
+                if w.code in self.warnings_as_errors_tests:
                     errors.append(w)
                 else:
                     new_warnings.append(w)
             warnings = new_warnings
 
         # Fixme: have a more generic approach to handling errors/warnings/ignored/ok?
         if errors:
@@ -220,22 +224,24 @@
             self.nb_valid += 1
             value_to_cache = {"result": "OK"}
 
         if self.should_use_cache():
             self.new_cache[md5hash] = value_to_cache
 
     @staticmethod
-    def get_migration_hash(app_label, migration_name):
+    def get_migration_hash(app_label: str, migration_name: str) -> str:
         hash_md5 = hashlib.md5()
         with open(get_migration_abspath(app_label, migration_name), "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 hash_md5.update(chunk)
         return hash_md5.hexdigest()
 
-    def lint_cached_migration(self, app_label, migration_name, md5hash):
+    def lint_cached_migration(
+        self, app_label: str, migration_name: str, md5hash: str
+    ) -> None:
         cached_value = self.old_cache[md5hash]
         if cached_value["result"] == "IGNORE":
             self.print_linting_msg(
                 app_label, migration_name, "IGNORE (cached)", MessageType.IGNORE
             )
             self.nb_ignored += 1
         elif cached_value["result"] == "OK":
@@ -257,126 +263,129 @@
             if "errors" in cached_value:
                 self.print_errors(cached_value["errors"])
             if "warnings" in cached_value and cached_value["warnings"]:
                 self.print_warnings(cached_value["warnings"])
 
         self.new_cache[md5hash] = cached_value
 
-    def print_linting_msg(self, app_label, migration_name, msg, lint_result):
+    def print_linting_msg(
+        self, app_label: str, migration_name: str, msg: str, lint_result: MessageType
+    ) -> None:
         if lint_result.value in self.quiet:
             return
         if not self.no_output:
-            print("({0}, {1})... {2}".format(app_label, migration_name, msg))
+            print(f"({app_label}, {migration_name})... {msg}")
 
-    def print_errors(self, errors):
+    def print_errors(self, errors: list[Issue]) -> None:
         if MessageType.ERROR.value in self.quiet:
             return
         for err in errors:
-            error_str = "\t{0}".format(err["msg"])
-            if err.get("table"):
-                error_str += " (table: {0}".format(err["table"])
-                if err.get("column"):
-                    error_str += ", column: {0}".format(err["column"])
+            error_str = "\t{}".format(err.message)
+            if err.table:
+                error_str += " (table: {}".format(err.table)
+                if err.column:
+                    error_str += ", column: {}".format(err.column)
                 error_str += ")"
             if not self.no_output:
                 print(error_str)
 
-    def print_warnings(self, warnings):
+    def print_warnings(self, warnings: list[Issue]) -> None:
         if MessageType.WARNING.value in self.quiet:
             return
 
         for warning_details in warnings:
-            warn_str = "\t{}".format(warning_details["msg"])
+            warn_str = "\t{}".format(warning_details.message)
             if not self.no_output:
                 print(warn_str)
 
-    def print_summary(self):
+    def print_summary(self) -> None:
         if self.no_output:
             return
         print("*** Summary ***")
-        print("Valid migrations: {}/{}".format(self.nb_valid, self.nb_total))
-        print("Erroneous migrations: {}/{}".format(self.nb_erroneous, self.nb_total))
-        print("Migrations with warnings: {}/{}".format(self.nb_warnings, self.nb_total))
-        print("Ignored migrations: {}/{}".format(self.nb_ignored, self.nb_total))
+        print(f"Valid migrations: {self.nb_valid}/{self.nb_total}")
+        print(f"Erroneous migrations: {self.nb_erroneous}/{self.nb_total}")
+        print(f"Migrations with warnings: {self.nb_warnings}/{self.nb_total}")
+        print(f"Ignored migrations: {self.nb_ignored}/{self.nb_total}")
 
     @property
-    def has_errors(self):
+    def has_errors(self) -> bool:
         return self.nb_erroneous > 0
 
-    def get_sql(self, app_label, migration_name):
-        logger.info(
-            "Calling sqlmigrate command {} {}".format(app_label, migration_name)
-        )
-        dev_null = open(os.devnull, "w")
+    def get_sql(self, app_label: str, migration_name: str) -> list[str]:
+        logger.info(f"Calling sqlmigrate command {app_label} {migration_name}")
         try:
-            sql_statement = call_command(
-                "sqlmigrate",
-                app_label,
-                migration_name,
-                database=self.database,
-                stdout=dev_null,
-            )
+            with open(os.devnull, "w") as dev_null:
+                sql_statement = call_command(
+                    "sqlmigrate",
+                    app_label,
+                    migration_name,
+                    database=self.database,
+                    stdout=dev_null,
+                )
         except (ValueError, ProgrammingError):
             logger.warning(
-                (
-                    "Error while executing sqlmigrate on (%s, %s). "
-                    "Continuing execution with empty SQL."
-                ),
+                "Error while executing sqlmigrate on (%s, %s).",
                 app_label,
                 migration_name,
             )
-            sql_statement = ""
+            raise
         return sql_statement.splitlines()
 
     @staticmethod
-    def is_migration_file(filename):
+    def is_migration_file(filename: str) -> bool:
         from django.db.migrations.loader import MIGRATIONS_MODULE_NAME
 
-        return (
-            re.search(r"/{0}/.*\.py".format(MIGRATIONS_MODULE_NAME), filename)
+        return bool(
+            re.search(rf"/{MIGRATIONS_MODULE_NAME}/.*\.py", filename)
             and "__init__" not in filename
         )
 
     @classmethod
-    def read_migrations_list(cls, migrations_file_path):
+    def read_migrations_list(
+        cls, migrations_file_path: str | None
+    ) -> list[tuple[str, str]] | None:
         """
         Returning an empty list is different from returning None here.
         None: no file was specified and we should consider all migrations
         Empty list: no migration found in the file and we should consider no migration
         """
         if not migrations_file_path:
             return None
 
         migrations = []
         try:
-            with open(migrations_file_path, "r") as file:
+            with open(migrations_file_path) as file:
                 for line in file:
                     if cls.is_migration_file(line):
                         app_label, name = split_migration_path(line)
                         migrations.append((app_label, name))
-        except IOError:
+        except OSError:
             logger.exception("Migrations list path not found %s", migrations_file_path)
             raise Exception("Error while reading migrations list file")
 
         if not migrations:
             logger.info(
                 "No valid migration paths found in the migrations file %s",
                 migrations_file_path,
             )
         return migrations
 
-    def _gather_migrations_git(self, git_commit_id, migrations_list=None):
+    def _gather_migrations_git(
+        self, git_commit_id: str, migrations_list: list[tuple[str, str]] | None = None
+    ) -> Iterable[Migration]:
         migrations = []
         # Get changes since specified commit
         git_diff_command = (
-            "cd {0} && git diff --relative --name-only --diff-filter=AR {1}"
+            "cd {} && git diff --relative --name-only --diff-filter=AR {}"
         ).format(self.django_path, git_commit_id)
-        logger.info("Executing {0}".format(git_diff_command))
+        logger.info(f"Executing {git_diff_command}")
         diff_process = Popen(git_diff_command, shell=True, stdout=PIPE, stderr=PIPE)
-        for line in map(clean_bytes_to_str, diff_process.stdout.readlines()):
+        for line in map(
+            clean_bytes_to_str, diff_process.stdout.readlines()  # type: ignore
+        ):
             # Only gather lines that include added migrations
             if self.is_migration_file(line):
                 app_label, name = split_migration_path(line)
                 if migrations_list is None or (app_label, name) in migrations_list:
                     if (app_label, name) in self.migration_loader.disk_migrations:
                         migration = self.migration_loader.disk_migrations[
                             app_label, name
@@ -389,30 +398,36 @@
                             app_label,
                             name,
                         )
         diff_process.wait()
 
         if diff_process.returncode != 0:
             output = []
-            for line in map(clean_bytes_to_str, diff_process.stderr.readlines()):
+            for line in map(
+                clean_bytes_to_str, diff_process.stderr.readlines()  # type: ignore
+            ):
                 output.append(line)
             logger.error("Error while git diff command:\n{}".format("".join(output)))
             raise Exception("Error while executing git diff command")
         return migrations
 
-    def _gather_all_migrations(self, migrations_list=None):
+    def _gather_all_migrations(
+        self, migrations_list: list[tuple[str, str]] | None = None
+    ) -> Iterable[Migration]:
         for (
             (app_label, name),
             migration,
         ) in self.migration_loader.disk_migrations.items():
             if app_label not in DJANGO_APPS_WITH_MIGRATIONS:  # Prune Django apps
                 if migrations_list is None or (app_label, name) in migrations_list:
                     yield migration
 
-    def should_ignore_migration(self, app_label, migration_name, operations=()):
+    def should_ignore_migration(
+        self, app_label: str, migration_name: str, operations: Iterable[Operation] = ()
+    ) -> bool:
         return (
             (self.include_apps and app_label not in self.include_apps)
             or (self.exclude_apps and app_label in self.exclude_apps)
             or any(isinstance(o, IgnoreMigration) for o in operations)
             or (
                 self.ignore_name_contains
                 and self.ignore_name_contains in migration_name
@@ -431,15 +446,17 @@
             or (
                 self.only_unapplied_migrations
                 and (app_label, migration_name)
                 in self.migration_loader.applied_migrations
             )
         )
 
-    def analyse_data_migration(self, migration):
+    def analyse_data_migration(
+        self, migration: Migration
+    ) -> tuple[list[Issue], list[Issue], list[Issue]]:
         errors = []
         ignored = []
         warnings = []
 
         for operation in migration.operations:
             if isinstance(operation, RunPython):
                 op_errors, op_ignored, op_warnings = self.lint_runpython(operation)
@@ -453,122 +470,133 @@
             if op_ignored:
                 ignored += op_ignored
             if op_warnings:
                 warnings += op_warnings
 
         return errors, ignored, warnings
 
-    def lint_runpython(self, runpython):
-        function_name = runpython.code.__name__
+    @staticmethod
+    def discover_function(function):
+        if isinstance(function, functools.partial):
+            return function.func
+        return function
+
+    def lint_runpython(
+        self, runpython: RunPython
+    ) -> tuple[list[Issue], list[Issue], list[Issue]]:
+        function_name = self.discover_function(runpython.code).__name__
         error = []
         ignored = []
         warning = []
 
         # Detect warning on missing reverse operation
         if not runpython.reversible:
-            issue = {
-                "code": "RUNPYTHON_REVERSIBLE",
-                "msg": "'{}': RunPython data migration is not reversible".format(
+            issue = Issue(
+                code="RUNPYTHON_REVERSIBLE",
+                message="'{}': RunPython data migration is not reversible".format(
                     function_name
                 ),
-            }
-            if issue["code"] in self.exclude_migration_tests:
+            )
+            if issue.code in self.exclude_migration_tests:
                 ignored.append(issue)
             else:
                 warning.append(issue)
 
         # Detect warning for argument naming convention
         args_spec = inspect.getfullargspec(runpython.code)
         if tuple(args_spec.args) != EXPECTED_DATA_MIGRATION_ARGS:
-            issue = {
-                "code": "RUNPYTHON_ARGS_NAMING_CONVENTION",
-                "msg": (
+            issue = Issue(
+                code="RUNPYTHON_ARGS_NAMING_CONVENTION",
+                message=(
                     "'{}': By convention, "
                     "RunPython names the two arguments: apps, schema_editor"
                 ).format(function_name),
-            }
-            if issue["code"] in self.exclude_migration_tests:
+            )
+            if issue.code in self.exclude_migration_tests:
                 ignored.append(issue)
             else:
                 warning.append(issue)
 
         # Detect wrong model imports
         # Forward
         issues = self.get_runpython_model_import_issues(runpython.code)
         for issue in issues:
-            if issue["code"] in self.exclude_migration_tests:
+            if issue.code in self.exclude_migration_tests:
                 ignored.append(issue)
             else:
                 error.append(issue)
 
         # Backward
         if runpython.reversible:
             issues = self.get_runpython_model_import_issues(runpython.reverse_code)
             for issue in issues:
-                if issue and issue["code"] in self.exclude_migration_tests:
+                if issue and issue.code in self.exclude_migration_tests:
                     ignored.append(issue)
                 else:
                     error.append(issue)
 
         # Detect warning if model variable name is not the same as model class
         issues = self.get_runpython_model_variable_naming_issues(runpython.code)
         for issue in issues:
-            if issue and issue["code"] in self.exclude_migration_tests:
+            if issue and issue.code in self.exclude_migration_tests:
                 ignored.append(issue)
             else:
                 warning.append(issue)
 
         if runpython.reversible:
             issues = self.get_runpython_model_variable_naming_issues(
                 runpython.reverse_code
             )
             for issue in issues:
-                if issue and issue["code"] in self.exclude_migration_tests:
+                if issue and issue.code in self.exclude_migration_tests:
                     ignored.append(issue)
                 else:
                     warning.append(issue)
 
         return error, ignored, warning
 
     @staticmethod
-    def get_runpython_model_import_issues(code):
-        model_object_regex = re.compile(r"[^a-zA-Z]?([a-zA-Z0-9]+?)\.objects")
+    def get_runpython_model_import_issues(code: Callable) -> list[Issue]:
+        model_object_regex = re.compile(r"[^a-zA-Z0-9._]?([a-zA-Z0-9._]+?)\.objects")
 
-        function_name = code.__name__
-        source_code = inspect.getsource(code)
+        function = MigrationLinter.discover_function(code)
+        function_name = function.__name__
+        source_code = inspect.getsource(function)
 
         called_models = model_object_regex.findall(source_code)
         issues = []
         for model in called_models:
+            model = model.split(".", 1)[0]
             has_get_model_call = (
                 re.search(
-                    r"{}.*= +\w+\.get_model\(".format(model),
+                    rf"{model}.*= +\w+\.get_model\(",
                     source_code,
                 )
                 is not None
             )
             if not has_get_model_call:
                 issues.append(
-                    {
-                        "code": "RUNPYTHON_MODEL_IMPORT",
-                        "msg": (
+                    Issue(
+                        code="RUNPYTHON_MODEL_IMPORT",
+                        message=(
                             "'{}': Could not find an 'apps.get_model(\"...\", \"{}\")' "
                             "call. Importing the model directly is incorrect for "
                             "data migrations."
                         ).format(function_name, model),
-                    }
+                    )
                 )
         return issues
 
     @staticmethod
-    def get_runpython_model_variable_naming_issues(code):
+    def get_runpython_model_variable_naming_issues(code: Callable) -> list[Issue]:
         model_object_regex = re.compile(r"[^a-zA-Z]?([a-zA-Z0-9]+?)\.objects")
 
-        function_name = code.__name__
-        source_code = inspect.getsource(code)
+        function = MigrationLinter.discover_function(code)
+        function_name = function.__name__
+        source_code = inspect.getsource(function)
 
         called_models = model_object_regex.findall(source_code)
         issues = []
         for model in called_models:
             has_same_model_name = (
                 re.search(
                     r"{model}.*= +\w+?\.get_model\([^)]+?\.{model}.*?\)".format(
@@ -585,37 +613,39 @@
                     source_code,
                     re.MULTILINE | re.DOTALL,
                 )
                 is not None
             )
             if not has_same_model_name:
                 issues.append(
-                    {
-                        "code": "RUNPYTHON_MODEL_VARIABLE_NAME",
-                        "msg": (
+                    Issue(
+                        code="RUNPYTHON_MODEL_VARIABLE_NAME",
+                        message=(
                             "'{}': Model variable name {} is different from the "
                             "model class name that was found in the "
                             "apps.get_model(...) call."
                         ).format(function_name, model),
-                    }
+                    )
                 )
         return issues
 
-    def lint_runsql(self, runsql):
+    def lint_runsql(
+        self, runsql: RunSQL
+    ) -> tuple[list[Issue], list[Issue], list[Issue]]:
         error = []
         ignored = []
         warning = []
 
         # Detect warning on missing reverse operation
         if not runsql.reversible:
-            issue = {
-                "code": "RUNSQL_REVERSIBLE",
-                "msg": "RunSQL data migration is not reversible",
-            }
-            if issue["code"] in self.exclude_migration_tests:
+            issue = Issue(
+                code="RUNSQL_REVERSIBLE",
+                message="RunSQL data migration is not reversible",
+            )
+            if issue.code in self.exclude_migration_tests:
                 ignored.append(issue)
             else:
                 warning.append(issue)
 
         # Put the SQL in our SQL analyser
         if runsql.sql != RunSQL.noop:
             sql_statements = []
```

### Comparing `django-migration-linter-4.1.0/django_migration_linter/operations.py` & `django-migration-linter-5.0.0/django_migration_linter/operations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+from __future__ import annotations
+
 from django.db.migrations.operations.base import Operation
 
 
 class IgnoreMigration(Operation):
     """
     No-op migration operation that will enable the Django Migration Linter
     to detect if the entire migration should be ignored (through code).
     """
 
     reversible = True
     reduces_to_sql = False
+    elidable = True
 
     def state_forwards(self, app_label, state):
         pass
 
     def database_forwards(self, app_label, schema_editor, from_state, to_state):
         pass
```

### Comparing `django-migration-linter-4.1.0/django_migration_linter/sql_analyser/analyser.py` & `django-migration-linter-5.0.0/django_migration_linter/sql_analyser/analyser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,70 @@
+from __future__ import annotations
+
 import logging
+from typing import TYPE_CHECKING, Iterable, Type
+
+if TYPE_CHECKING:
+    from sql_analyser.base import Issue
 
 from django_migration_linter.sql_analyser import (
+    BaseAnalyser,
     MySqlAnalyser,
     PostgresqlAnalyser,
     SqliteAnalyser,
 )
 
 logger = logging.getLogger("django_migration_linter")
 
-ANALYSER_STRING_MAPPING = {
+ANALYSER_STRING_MAPPING: dict[str, Type[BaseAnalyser]] = {
     "sqlite": SqliteAnalyser,
     "mysql": MySqlAnalyser,
     "postgresql": PostgresqlAnalyser,
 }
 
 
-def get_sql_analyser_class(database_vendor, analyser_string=None):
+def get_sql_analyser_class(
+    database_vendor: str, analyser_string: str | None = None
+) -> Type[BaseAnalyser]:
     if analyser_string:
         return get_sql_analyser_from_string(analyser_string)
     return get_sql_analyser_class_from_db_vendor(database_vendor)
 
 
-def get_sql_analyser_from_string(analyser_string):
+def get_sql_analyser_from_string(analyser_string: str) -> Type[BaseAnalyser]:
     if analyser_string not in ANALYSER_STRING_MAPPING:
         raise ValueError(
-            "Unknown SQL analyser. Known values: {}".format(analyser_string.keys())
+            "Unknown SQL analyser '{}'. Known values: '{}'".format(
+                analyser_string,
+                "','".join(ANALYSER_STRING_MAPPING.keys()),
+            )
         )
     return ANALYSER_STRING_MAPPING[analyser_string]
 
 
-def get_sql_analyser_class_from_db_vendor(database_vendor):
+def get_sql_analyser_class_from_db_vendor(database_vendor: str) -> Type[BaseAnalyser]:
+    sql_analyser_class: Type[BaseAnalyser]
     if "mysql" in database_vendor:
         sql_analyser_class = MySqlAnalyser
     elif "postgre" in database_vendor:
         sql_analyser_class = PostgresqlAnalyser
     elif "sqlite" in database_vendor:
         sql_analyser_class = SqliteAnalyser
     else:
-        raise ValueError("Unsupported database vendor. Try specifying an SQL analyser.")
+        raise ValueError(
+            "Unsupported database vendor '{}'. Try specifying an SQL analyser.".format(
+                database_vendor
+            )
+        )
 
     logger.debug("Chosen SQL analyser class: %s", sql_analyser_class)
     return sql_analyser_class
 
 
 def analyse_sql_statements(
-    sql_analyser_class, sql_statements, exclude_migration_tests=None
-):
+    sql_analyser_class: Type[BaseAnalyser],
+    sql_statements: list[str],
+    exclude_migration_tests: Iterable[str] | None = None,
+) -> tuple[list[Issue], list[Issue], list[Issue]]:
     sql_analyser = sql_analyser_class(exclude_migration_tests)
     sql_analyser.analyse(sql_statements)
     return sql_analyser.errors, sql_analyser.ignored, sql_analyser.warnings
```

### Comparing `django-migration-linter-4.1.0/django_migration_linter/sql_analyser/sqlite.py` & `django-migration-linter-5.0.0/django_migration_linter/sql_analyser/sqlite.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,56 @@
+from __future__ import annotations
+
 import re
 
-from .base import BaseAnalyser
+from .base import BaseAnalyser, Check, CheckMode, CheckType
 
 
 class SqliteAnalyser(BaseAnalyser):
-    migration_tests = [
-        {
-            "code": "RENAME_TABLE",
-            "fn": lambda sql, **kw: re.search("ALTER TABLE .* RENAME TO", sql)
+    migration_checks: list[Check] = [
+        Check(
+            code="RENAME_TABLE",
+            fn=lambda sql, **kw: re.search("ALTER TABLE .* RENAME TO", sql)
             and "__old" not in sql
             and "new__" not in sql,
-            "type": "error",
-        },
-        {
-            "code": "DROP_TABLE",
+            message="RENAMING tables",
+            mode=CheckMode.ONE_LINER,
+            type=CheckType.ERROR,
+        ),
+        Check(
+            code="DROP_TABLE",
             # TODO: improve to detect that the table names overlap
-            "fn": lambda sql_statements, **kw: any(
+            fn=lambda sql_statements, **kw: any(
                 sql.startswith("DROP TABLE") for sql in sql_statements
             )
             and not any(sql.startswith("CREATE TABLE") for sql in sql_statements),
-            "msg": "DROPPING table",
-            "mode": "transaction",
-            "type": "error",
-        },
-        {
-            "code": "NOT_NULL",
-            "fn": lambda sql_statements, **kw: any(
+            message="DROPPING table",
+            mode=CheckMode.TRANSACTION,
+            type=CheckType.ERROR,
+        ),
+        Check(
+            code="NOT_NULL",
+            fn=lambda sql_statements, **kw: any(
                 re.search("NOT NULL(?! PRIMARY)(?! DEFAULT)", sql)
                 for sql in sql_statements
             )
             and any(
                 re.search("ALTER TABLE .* RENAME TO", sql)
                 and ("__old" in sql or "new__" in sql)
                 for sql in sql_statements
             ),
-            "mode": "transaction",
-            "type": "error",
-        },
+            message="NOT NULL constraint on columns",
+            mode=CheckMode.TRANSACTION,
+            type=CheckType.ERROR,
+        ),
     ]
 
     @staticmethod
-    def detect_table(sql):
+    def detect_table(sql: list[str] | str) -> str | None:
         if isinstance(sql, str):
             regex_result = re.search("TABLE [`\"'](.*?)[`\"']", sql, re.IGNORECASE)
             if regex_result:
                 return regex_result.group(1)
             regex_result = re.search("ON [`\"'](.*?)[`\"']", sql, re.IGNORECASE)
             if regex_result:
                 return regex_result.group(1)
+        return None
```

### Comparing `django-migration-linter-4.1.0/django_migration_linter/utils.py` & `django-migration-linter-5.0.0/django_migration_linter/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from __future__ import print_function
+from __future__ import annotations
 
 import os
 from importlib import import_module
 
 
-def split_path(path):
-    decomposed_path = []
+def split_path(path: str) -> list[str]:
+    decomposed_path: list[str] = []
     while 1:
         head, tail = os.path.split(path)
         if head == path:  # sentinel for absolute paths
             decomposed_path.insert(0, head)
             break
         elif tail == path:  # sentinel for relative paths
             decomposed_path.insert(0, tail)
@@ -19,31 +19,35 @@
             decomposed_path.insert(0, tail)
 
     if not decomposed_path[-1]:
         decomposed_path = decomposed_path[:-1]
     return decomposed_path
 
 
-def split_migration_path(migration_path):
+def split_migration_path(migration_path: str) -> tuple[str, str]:
     from django.db.migrations.loader import MIGRATIONS_MODULE_NAME
 
     decomposed_path = split_path(migration_path)
     for i, p in enumerate(decomposed_path):
         if p == MIGRATIONS_MODULE_NAME:
             return decomposed_path[i - 1], os.path.splitext(decomposed_path[i + 1])[0]
+    return "", ""
 
 
-def clean_bytes_to_str(byte_input):
+def clean_bytes_to_str(byte_input: bytes) -> str:
     return byte_input.decode("utf-8").strip()
 
 
-def get_migration_abspath(app_label, migration_name):
+def get_migration_abspath(app_label: str, migration_name: str) -> str:
     from django.db.migrations.loader import MigrationLoader
 
     module_name, _ = MigrationLoader.migrations_module(app_label)
-    migration_path = "{}.{}".format(module_name, migration_name)
+    migration_path = f"{module_name}.{migration_name}"
     migration_module = import_module(migration_path)
 
     migration_file = migration_module.__file__
+    if not migration_file:
+        raise ValueError("Migration file not found")
+
     if migration_file.endswith(".pyc"):
         migration_file = migration_file[:-1]
     return migration_file
```

### Comparing `django-migration-linter-4.1.0/django_migration_linter.egg-info/PKG-INFO` & `django-migration-linter-5.0.0/django_migration_linter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,133 +1,144 @@
 Metadata-Version: 2.1
 Name: django-migration-linter
-Version: 4.1.0
+Version: 5.0.0
 Summary: Detect backward incompatible migrations for your django project
 Home-page: https://github.com/3YOURMIND/django-migration-linter
 Author: 3YOURMIND GmbH
 Author-email: david.wobrock@gmail.com
 License: Apache License 2.0
-Description: # Django migration linter
-        
-        Detect backward incompatible migrations for your Django project.
-        It will save you time by making sure migrations will not break with a older codebase.
-        
-        [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2F3YOURMIND%2Fdjango-migration-linter%2Fbadge%3Fref%3Dmain&style=flat)](https://actions-badge.atrox.dev/3YOURMIND/django-migration-linter/goto?ref=main)
-        [![codecov](https://codecov.io/gh/3YOURMIND/django-migration-linter/branch/master/graph/badge.svg?token=pgNNXGbCf7)](https://codecov.io/gh/3YOURMIND/django-migration-linter)
-        [![PyPI](https://img.shields.io/pypi/v/django-migration-linter.svg)](https://pypi.python.org/pypi/django-migration-linter/)
-        [![PR_Welcome](https://img.shields.io/badge/PR-welcome-green.svg)](https://github.com/3YOURMIND/django-migration-linter/pulls)
-        [![3YD_Hiring](https://img.shields.io/badge/3YOURMIND-Hiring-brightgreen.svg)](https://www.3yourmind.com/career)
-        [![GitHub_Stars](https://img.shields.io/github/stars/3YOURMIND/django-migration-linter.svg?style=social&label=Stars)](https://github.com/3YOURMIND/django-migration-linter/stargazers)
-        
-        ## Quick installation
-        
-        ```
-        pip install django-migration-linter
-        ```
-        
-        And add the migration linter your ``INSTALLED_APPS``:
-        ```
-            INSTALLED_APPS = [
-                ...,
-                "django_migration_linter",
-                ...,
-            ]
-        ```
-        
-        ## Usage example
-        
-        ```
-        $ python manage.py lintmigrations
-        
-        (app_add_not_null_column, 0001_create_table)... OK
-        (app_add_not_null_column, 0002_add_new_not_null_field)... ERR
-                NOT NULL constraint on columns
-        (app_drop_table, 0001_initial)... OK
-        (app_drop_table, 0002_delete_a)... ERR
-                DROPPING table
-        (app_ignore_migration, 0001_initial)... OK
-        (app_ignore_migration, 0002_ignore_migration)... IGNORE
-        (app_rename_table, 0001_initial)... OK
-        (app_rename_table, 0002_auto_20190414_1500)... ERR
-                RENAMING tables
-        
-        *** Summary ***
-        Valid migrations: 4/8
-        Erroneous migrations: 3/8
-        Migrations with warnings: 0/8
-        Ignored migrations: 1/8
-        ```
-        
-        The linter analysed all migrations from the Django project.
-        It found 3 migrations that are doing backward incompatible operations and 1 that is explicitly ignored.
-        The list of incompatibilities that the linter analyses [can be found at docs/incompatibilities.md](./docs/incompatibilities.md).
-        
-        More advanced usages of the linter and options [can be found at docs/usage.md](./docs/usage.md).
-        
-        ## Integration
-        
-        One can either integrate the linter in the CI using its `lintmigrations` command, or detect incompatibilities during generation of migrations with
-        ```
-        $ python manage.py makemigrations --lint
-        
-        Migrations for 'app_correct':
-          tests/test_project/app_correct/migrations/0003_a_column.py
-            - Add field column to a
-        Linting for 'app_correct':
-        (app_correct, 0003_a_column)... ERR
-                NOT NULL constraint on columns
-        
-        The migration linter detected that this migration is not backward compatible.
-        - If you keep the migration, you will want to fix the issue or ignore the migration.
-        - By default, the newly created migration file will be deleted.
-        Do you want to keep the migration? [y/N] n
-        Deleted tests/test_project/app_correct/migrations/0003_a_column.py
-        ```
-        
-        The linter found that the newly created migration is not backward compatible and deleted the file after confirmation.
-        This behaviour can be the default of the `makemigrations` command through the `MIGRATION_LINTER_OVERRIDE_MAKEMIGRATIONS` Django setting.
-        Find out more about the [makemigrations command at docs/makemigrations.md](./docs/makemigrations.md).
-        
-        ### More information
-        
-        Please find more documentation [in the docs/ folder](./docs/).
-        
-        Some implementation details [can be found in the ./docs/internals/ folder](./docs/internals/).
-        
-        ### Blog post
-        
-        * [Keeping Django database migrations backward compatible](https://medium.com/3yourmind/keeping-django-database-migrations-backward-compatible-727820260dbb)
-        * [Django and its default values](https://medium.com/botify-labs/django-and-its-default-values-c21a13cff9f)
-        
-        ### They talk about the linter
-        
-        * [Django News](https://django-news.com/issues/6?m=web#uMmosw7)
-        * [wemake-django-template](https://wemake-django-template.readthedocs.io/en/latest/pages/template/linters.html#django-migration-linter)
-        * [Testing Django migrations on sobolevn's blog](https://sobolevn.me/2019/10/testing-django-migrations#existing-setup)
-        
-        ### Related
-        
-        * [django-test-migrations](https://github.com/wemake-services/django-test-migrations) - Test django schema and data migrations, including migrations' order and best practices.
-        
-        ### License
-        
-        *django-migration-linter* is released under the [Apache 2.0 License](./LICENSE).
-        
-        ##### Maintained by [David Wobrock](https://github.com/David-Wobrock)
-        
 Keywords: django migration lint linter database backward compatibility
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# Django migration linter
+
+Detect backward incompatible migrations for your Django project.
+It will save you time by making sure migrations will not break with a older codebase.
+
+[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2F3YOURMIND%2Fdjango-migration-linter%2Fbadge%3Fref%3Dmain&style=flat)](https://actions-badge.atrox.dev/3YOURMIND/django-migration-linter/goto?ref=main)
+[![codecov](https://codecov.io/gh/3YOURMIND/django-migration-linter/branch/master/graph/badge.svg?token=pgNNXGbCf7)](https://codecov.io/gh/3YOURMIND/django-migration-linter)
+[![PyPI](https://img.shields.io/pypi/v/django-migration-linter.svg)](https://pypi.python.org/pypi/django-migration-linter/)
+[![PR_Welcome](https://img.shields.io/badge/PR-welcome-green.svg)](https://github.com/3YOURMIND/django-migration-linter/pulls)
+[![3YD_Hiring](https://img.shields.io/badge/3YOURMIND-Hiring-brightgreen.svg)](https://www.3yourmind.com/career)
+[![GitHub_Stars](https://img.shields.io/github/stars/3YOURMIND/django-migration-linter.svg?style=social&label=Stars)](https://github.com/3YOURMIND/django-migration-linter/stargazers)
+
+## Quick installation
+
+```
+pip install django-migration-linter
+```
+
+And add the migration linter to your ``INSTALLED_APPS``:
+```
+INSTALLED_APPS = [
+    ...,
+    "django_migration_linter",
+    ...,
+]
+```
+
+Optionally, add a configuration:
+```
+MIGRATION_LINTER_OPTIONS = {
+    ...
+}
+```
+
+For details about configuration options, checkout [Usage](docs/usage.md).
+
+## Usage example
+
+```
+$ python manage.py lintmigrations
+
+(app_add_not_null_column, 0001_create_table)... OK
+(app_add_not_null_column, 0002_add_new_not_null_field)... ERR
+        NOT NULL constraint on columns
+(app_drop_table, 0001_initial)... OK
+(app_drop_table, 0002_delete_a)... ERR
+        DROPPING table
+(app_ignore_migration, 0001_initial)... OK
+(app_ignore_migration, 0002_ignore_migration)... IGNORE
+(app_rename_table, 0001_initial)... OK
+(app_rename_table, 0002_auto_20190414_1500)... ERR
+        RENAMING tables
+
+*** Summary ***
+Valid migrations: 4/8
+Erroneous migrations: 3/8
+Migrations with warnings: 0/8
+Ignored migrations: 1/8
+```
+
+The linter analysed all migrations from the Django project.
+It found 3 migrations that are doing backward incompatible operations and 1 that is explicitly ignored.
+The list of incompatibilities that the linter analyses [can be found at docs/incompatibilities.md](./docs/incompatibilities.md).
+
+More advanced usages of the linter and options [can be found at docs/usage.md](./docs/usage.md).
+
+## Integration
+
+One can either integrate the linter in the CI using its `lintmigrations` command, or detect incompatibilities during generation of migrations with
+```
+$ python manage.py makemigrations --lint
+
+Migrations for 'app_correct':
+  tests/test_project/app_correct/migrations/0003_a_column.py
+    - Add field column to a
+Linting for 'app_correct':
+(app_correct, 0003_a_column)... ERR
+        NOT NULL constraint on columns
+
+The migration linter detected that this migration is not backward compatible.
+- If you keep the migration, you will want to fix the issue or ignore the migration.
+- By default, the newly created migration file will be deleted.
+Do you want to keep the migration? [y/N] n
+Deleted tests/test_project/app_correct/migrations/0003_a_column.py
+```
+
+The linter found that the newly created migration is not backward compatible and deleted the file after confirmation.
+This behaviour can be the default of the `makemigrations` command through the `MIGRATION_LINTER_OVERRIDE_MAKEMIGRATIONS` Django setting.
+Find out more about the [makemigrations command at docs/makemigrations.md](./docs/makemigrations.md).
+
+### More information
+
+Please find more documentation [in the docs/ folder](./docs/).
+
+Some implementation details [can be found in the ./docs/internals/ folder](./docs/internals/).
+
+### Blog post
+
+* [Keeping Django database migrations backward compatible](https://medium.com/3yourmind/keeping-django-database-migrations-backward-compatible-727820260dbb)
+* [Django and its default values](https://medium.com/botify-labs/django-and-its-default-values-c21a13cff9f)
+
+### They talk about the linter
+
+* [Django News](https://django-news.com/issues/6?m=web#uMmosw7)
+* [wemake-django-template](https://wemake-django-template.readthedocs.io/en/latest/pages/template/linters.html#django-migration-linter)
+* [Testing Django migrations on sobolevn's blog](https://sobolevn.me/2019/10/testing-django-migrations#existing-setup)
+
+### Related
+
+* [django-test-migrations](https://github.com/wemake-services/django-test-migrations) - Test django schema and data migrations, including migrations' order and best practices.
+
+### License
+
+*django-migration-linter* is released under the [Apache 2.0 License](./LICENSE).
+
+##### Maintained by [David Wobrock](https://github.com/David-Wobrock)
```

### Comparing `django-migration-linter-4.1.0/docs/incompatibilities.md` & `django-migration-linter-5.0.0/docs/incompatibilities.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 | `ADD_UNIQUE`                       | Add unique constraints                                                                                               | Error        |
 | `RUNPYTHON_REVERSIBLE`             | RunPython data migration is not reversible (missing reverse code)                                                    | Warning      |
 | `RUNPYTHON_ARGS_NAMING_CONVENTION` | By convention, RunPython names two arguments: apps, schema_editor                                                    | Warning      |
 | `RUNPYTHON_MODEL_IMPORT`           | Missing apps.get_model() calls for model                                                                             | Error        |
 | `RUNPYTHON_MODEL_VARIABLE_NAME`    | The model variable name is different from the model class itself                                                     | Warning      |
 | `RUNSQL_REVERSIBLE`                | RunSQL data migration is not reversible (missing reverse SQL)                                                        | Warning      |
 | `CREATE_INDEX`                     | (Postgresql specific) Creating an index without the concurrent keyword will lock the table and may generate downtime | Warning      |
+| `CREATE_INDEX_EXCLUSIVE`           | (Postgresql specific) Creating an index in a transaction (after an `EXCLUSIVE` lock) prolongs the exclusive lock     | Warning      |
 | `DROP_INDEX`                       | (Postgresql specific) Dropping an index without the concurrent keyword will lock the table and may generate downtime | Warning      |
 | `REINDEX`                          | (Postgresql specific) Reindexing will lock the table and may generate downtime                                       | Warning      |
 
 
 ## Details about backward incompatibilities
 
 This section will go into the depth of the different check the migration linter makes.
```

### Comparing `django-migration-linter-4.1.0/docs/internals/cache.md` & `django-migration-linter-5.0.0/docs/internals/cache.md`

 * *Files identical despite different names*

### Comparing `django-migration-linter-4.1.0/docs/internals/testing.md` & `django-migration-linter-5.0.0/docs/internals/testing.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 
 To be able to fully test the linter, you will need both MySQL and PostgreSQL databases running.
 You can either tweak the ``tests/test_project/settings.py`` file to get your DB settings right, or to have databases and users corresponding to the default CI users.
 
 ## Database setup
 
 By default, the test Django project in the repository has multiple databases configured in order to make the CI tests work.
-Do not hesitate to modify [the configured test databases](../../tests/test_project/settings.py).
+Do not hesitate to modify [the configured test databases](../../tests/test_project/settings.py).
```

### Comparing `django-migration-linter-4.1.0/docs/makemigrations.md` & `django-migration-linter-5.0.0/docs/makemigrations.md`

 * *Files identical despite different names*

### Comparing `django-migration-linter-4.1.0/docs/usage.md` & `django-migration-linter-5.0.0/docs/usage.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 # Usage
 
 ## Command line usage
 
-The linter is installed as a Django app and is integrated through the Django management command system. 
+The linter is installed as a Django app and is integrated through the Django management command system.
 
 `python manage.py lintmigrations [app_label] [migration_name]`
 
 The three main usages are:
 
 * Lint your entire code base
 `python manage.py lintmigrations`
 
 * Lint one Django app
 `python manage.py lintmigrations app_label`
 
 * Lint a specific migration
 `python manage.py lintmigrations app_label migration_name`
 
-Below the detailed command line options, which can all also be defined using a config file (`setup.cfg`, `tox.ini`, `pyproject.toml`, `.django_migration_linter.cfg`):
+Below the detailed command line options, which can all also be defined using a config file:
+- `settings.py`
+- `setup.cfg`
+- `tox.ini`
+- `pyproject.toml`
+- `.django_migration_linter.cfg`
+
+If you are using a config file, replace any dashes (`-`) with an underscore (`_`).
 
 | Parameter                                             | Description                                                                                                                                                                                                     |
 |-------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `--git-commit-id GIT_COMMIT_ID`                       | If specified, only migrations since this commit will be taken into account.                                                                                                                                     |
 | `--ignore-name-contains IGNORE_NAME_CONTAINS`         | Ignore migrations containing this name.                                                                                                                                                                         |
 | `--ignore-name IGNORE_NAME [IGNORE_NAME ...]`         | Ignore migrations with exactly one of these names.                                                                                                                                                              |
 | `--include-name-contains INCLUDE_NAME_CONTAINS`       | Include migrations containing this name.                                                                                                                                                                        |
```

### Comparing `django-migration-linter-4.1.0/setup.py` & `django-migration-linter-5.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+from __future__ import annotations
+
 import ast
 import re
 from os import path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = path.abspath(path.dirname(__file__))
 
 
 def get_version():
     constants = path.join(PROJECT_DIR, "django_migration_linter", "constants.py")
     _version_re = re.compile(r"__version__\s+=\s+(?P<version>.*)")
-    with open(constants, "r") as f:
+    with open(constants) as f:
         match = _version_re.search(f.read())
         version = match.group("version") if match is not None else '"unknown"'
     return str(ast.literal_eval(version))
 
 
 with open(path.join(PROJECT_DIR, "README.md")) as f:
     long_description = f.read()
@@ -34,31 +36,33 @@
     install_requires=[
         "django>=2.2",
         "appdirs>=1.4.3",
         "toml>=0.10.2",
     ],
     extras_require={
         "test": [
-            "tox>=3.15.2",
-            "mysqlclient>=1.4.6,<2",
-            "psycopg2-binary>=2.8.5,<2.9",
+            "tox>=4.6.3",
+            "mysqlclient>=2.1.1",
+            "psycopg2>=2.9.6",
             "django_add_default_value>=0.4.0",
-            "coverage>=5.5",
+            "coverage>=7.2.7",
         ],
     },
     keywords="django migration lint linter database backward compatibility",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Web Environment",
         "Framework :: Django",
-        "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

