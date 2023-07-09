# Comparing `tmp/apache-airflow-providers-amazon-8.3.0rc2.tar.gz` & `tmp/apache-airflow-providers-amazon-8.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-amazon-8.3.0rc2.tar", last modified: Thu Jul  6 04:50:02 2023, max compression
+gzip compressed data, was "apache-airflow-providers-amazon-8.3.0rc3.tar", last modified: Sun Jul  9 15:12:46 2023, max compression
```

## Comparing `apache-airflow-providers-amazon-8.3.0rc2.tar` & `apache-airflow-providers-amazon-8.3.0rc3.tar`

### file list

```diff
@@ -1,194 +1,195 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.937776 apache-airflow-providers-amazon-8.3.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.3.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1219 2023-07-06 04:50:00.000000 apache-airflow-providers-amazon-8.3.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.3.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8022 2023-07-06 04:50:02.938344 apache-airflow-providers-amazon-8.3.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6037 2023-07-06 04:50:00.000000 apache-airflow-providers-amazon-8.3.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.387575 apache-airflow-providers-amazon-8.3.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.388790 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.436769 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-07-05 18:42:40.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.443080 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.558533 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/appflow.py
--rw-r--r--   0 root         (0) root         (0)    12334 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/athena.py
--rw-r--r--   0 root         (0) root         (0)    46780 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    21319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.json
--rw-r--r--   0 root         (0) root         (0)    10541 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-r--r--   0 root         (0) root         (0)     4263 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/chime.py
--rw-r--r--   0 root         (0) root         (0)     3378 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    14079 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/datasync.py
--rw-r--r--   0 root         (0) root         (0)     7907 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/dms.py
--rw-r--r--   0 root         (0) root         (0)     2670 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     7928 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/ec2.py
--rw-r--r--   0 root         (0) root         (0)     3703 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/ecr.py
--rw-r--r--   0 root         (0) root         (0)     6610 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/ecs.py
--rw-r--r--   0 root         (0) root         (0)    23958 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/eks.py
--rw-r--r--   0 root         (0) root         (0)    12119 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-r--r--   0 root         (0) root         (0)    20429 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 root         (0) root         (0)     3452 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/glacier.py
--rw-r--r--   0 root         (0) root         (0)    16313 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/glue.py
--rw-r--r--   0 root         (0) root         (0)     7616 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-r--r--   0 root         (0) root         (0)     7872 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-r--r--   0 root         (0) root         (0)     8095 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     5883 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/logs.py
--rw-r--r--   0 root         (0) root         (0)     7094 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    15479 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/rds.py
--rw-r--r--   0 root         (0) root         (0)    13169 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7722 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     7160 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    58295 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/s3.py
--rw-r--r--   0 root         (0) root         (0)    56365 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2667 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     4146 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/ses.py
--rw-r--r--   0 root         (0) root         (0)     3463 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/sns.py
--rw-r--r--   0 root         (0) root         (0)     3121 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/ssm.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/step_function.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.575392 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/base_aws.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/batch.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/emr.py
--rw-r--r--   0 root         (0) root         (0)     1229 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/glue.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.584082 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-r--r--   0 root         (0) root         (0)     9600 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.590015 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/notifications/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/notifications/chime.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.663433 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19662 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0 root         (0) root         (0)    20439 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    18421 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0 root         (0) root         (0)    10720 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0 root         (0) root         (0)     9591 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0 root         (0) root         (0)    33364 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0 root         (0) root         (0)    43249 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/eks.py
--rw-r--r--   0 root         (0) root         (0)    65005 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0 root         (0) root         (0)     9663 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0 root         (0) root         (0)     4349 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     7749 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3968 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    35167 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0 root         (0) root         (0)    32273 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5547 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)    30235 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0 root         (0) root         (0)    58086 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0 root         (0) root         (0)     4583 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.672024 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15625 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     8495 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.742908 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0 root         (0) root         (0)     9059 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 root         (0) root         (0)     4150 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)     3984 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     3721 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0 root         (0) root         (0)     7063 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9772 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0 root         (0) root         (0)    22898 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 root         (0) root         (0)     4115 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0 root         (0) root         (0)     3319 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0 root         (0) root         (0)     3719 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3027 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3626 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0 root         (0) root         (0)     6434 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)    15073 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0 root         (0) root         (0)    12794 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     9543 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0 root         (0) root         (0)     3333 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.802948 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7019 2023-07-04 06:09:02.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0 root         (0) root         (0)     7747 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6368 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8544 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4702 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4173 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     5981 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0 root         (0) root         (0)     8287 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0 root         (0) root         (0)     4634 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     3643 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8865 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.840130 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3154 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/athena.py
--rw-r--r--   0 root         (0) root         (0)     9670 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/batch.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/ec2.py
--rw-r--r--   0 root         (0) root         (0)     8212 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9760 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/eks.py
--rw-r--r--   0 root         (0) root         (0)    14727 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/emr.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/glue.py
--rw-r--r--   0 root         (0) root         (0)     3090 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3874 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/rds.py
--rw-r--r--   0 root         (0) root         (0)    14450 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     9085 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/s3.py
--rw-r--r--   0 root         (0) root         (0)     4626 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/sagemaker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.871843 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     2265 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20649 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/emailer.py
--rw-r--r--   0 root         (0) root         (0)      973 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/rds.py
--rw-r--r--   0 root         (0) root         (0)     1897 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/redshift.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     4491 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/task_log_fetcher.py
--rw-r--r--   0 root         (0) root         (0)     3509 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/waiter.py
--rw-r--r--   0 root         (0) root         (0)     5890 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/waiter_with_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.911293 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/appflow.json
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-24 10:23:43.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/athena.json
--rw-r--r--   0 root         (0) root         (0)     1853 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/base_waiter.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/batch.json
--rw-r--r--   0 root         (0) root         (0)      895 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/dynamodb.json
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/ecs.json
--rw-r--r--   0 root         (0) root         (0)      659 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/eks.json
--rw-r--r--   0 root         (0) root         (0)      851 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/emr-containers.json
--rw-r--r--   0 root         (0) root         (0)     4893 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/emr-serverless.json
--rw-r--r--   0 root         (0) root         (0)     4242 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/emr.json
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/glue.json
--rw-r--r--   0 root         (0) root         (0)     1742 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/redshift.json
--rw-r--r--   0 root         (0) root         (0)     3625 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/sagemaker.json
--rw-r--r--   0 root         (0) root         (0)    40167 2023-07-06 04:50:00.000000 apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:02.934721 apache-airflow-providers-amazon-8.3.0rc2/apache_airflow_providers_amazon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8022 2023-07-06 04:50:02.000000 apache-airflow-providers-amazon-8.3.0rc2/apache_airflow_providers_amazon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8457 2023-07-06 04:50:02.000000 apache-airflow-providers-amazon-8.3.0rc2/apache_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:02.000000 apache-airflow-providers-amazon-8.3.0rc2/apache_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-06 04:50:02.000000 apache-airflow-providers-amazon-8.3.0rc2/apache_airflow_providers_amazon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:02.000000 apache-airflow-providers-amazon-8.3.0rc2/apache_airflow_providers_amazon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      949 2023-07-06 04:50:02.000000 apache-airflow-providers-amazon-8.3.0rc2/apache_airflow_providers_amazon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:02.000000 apache-airflow-providers-amazon-8.3.0rc2/apache_airflow_providers_amazon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.3.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2243 2023-07-06 04:50:02.940269 apache-airflow-providers-amazon-8.3.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2502 2023-07-06 04:50:00.000000 apache-airflow-providers-amazon-8.3.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:46.127008 apache-airflow-providers-amazon-8.3.0rc3/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.3.0rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-07-09 15:12:43.000000 apache-airflow-providers-amazon-8.3.0rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.3.0rc3/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8022 2023-07-09 15:12:46.127702 apache-airflow-providers-amazon-8.3.0rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-07-09 15:12:43.000000 apache-airflow-providers-amazon-8.3.0rc3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:45.498020 apache-airflow-providers-amazon-8.3.0rc3/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:45.499212 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:45.561348 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-07-09 14:42:13.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:45.571248 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:45.716518 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 root         (0) root         (0)    12358 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 root         (0) root         (0)    46780 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    21319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/batch_waiters.json
+-rw-r--r--   0 root         (0) root         (0)    10541 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     4263 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/chime.py
+-rw-r--r--   0 root         (0) root         (0)     3378 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    14079 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 root         (0) root         (0)     7907 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     7928 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 root         (0) root         (0)     6610 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    23958 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 root         (0) root         (0)    12119 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 root         (0) root         (0)    20429 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 root         (0) root         (0)    16313 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 root         (0) root         (0)     7616 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 root         (0) root         (0)     7931 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     8095 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    15479 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 root         (0) root         (0)    13169 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     7160 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    58255 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 root         (0) root         (0)    56365 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:45.735118 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:45.744119 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9600 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:45.750165 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/notifications/chime.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:45.828427 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19662 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 root         (0) root         (0)    20436 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    18421 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 root         (0) root         (0)    10720 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 root         (0) root         (0)     9591 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 root         (0) root         (0)    33315 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    43203 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 root         (0) root         (0)    65010 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     9663 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     7749 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    35538 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 root         (0) root         (0)    32304 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)    30235 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 root         (0) root         (0)    58086 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     4583 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:45.837641 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15625 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8495 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:45.905137 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 root         (0) root         (0)     9160 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)     3984 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     3721 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9772 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 root         (0) root         (0)    22909 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3719 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3626 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    15066 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 root         (0) root         (0)    12794 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     9543 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:45.970323 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7019 2023-07-04 06:09:02.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6368 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8544 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4702 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4173 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     5981 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     8287 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4634 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     3643 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8865 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:46.012905 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/athena.py
+-rw-r--r--   0 root         (0) root         (0)     5403 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/base.py
+-rw-r--r--   0 root         (0) root         (0)    10706 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     8898 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     8445 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/eks.py
+-rw-r--r--   0 root         (0) root         (0)    11320 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/emr.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/glue.py
+-rw-r--r--   0 root         (0) root         (0)     2622 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/rds.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     9085 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/s3.py
+-rw-r--r--   0 root         (0) root         (0)     4626 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/sagemaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:46.047743 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20649 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 root         (0) root         (0)      973 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     4491 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/task_log_fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     3509 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/waiter.py
+-rw-r--r--   0 root         (0) root         (0)     5890 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/waiter_with_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:46.096438 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/appflow.json
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-24 10:23:43.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/athena.json
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/base_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/batch.json
+-rw-r--r--   0 root         (0) root         (0)      895 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/dynamodb.json
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/ecs.json
+-rw-r--r--   0 root         (0) root         (0)      659 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/eks.json
+-rw-r--r--   0 root         (0) root         (0)      851 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/emr-containers.json
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/emr-serverless.json
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/emr.json
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/glue.json
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/redshift.json
+-rw-r--r--   0 root         (0) root         (0)     3625 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/sagemaker.json
+-rw-r--r--   0 root         (0) root         (0)    40337 2023-07-09 15:12:43.000000 apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:12:46.124333 apache-airflow-providers-amazon-8.3.0rc3/apache_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8022 2023-07-09 15:12:45.000000 apache-airflow-providers-amazon-8.3.0rc3/apache_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8503 2023-07-09 15:12:45.000000 apache-airflow-providers-amazon-8.3.0rc3/apache_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 15:12:45.000000 apache-airflow-providers-amazon-8.3.0rc3/apache_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-09 15:12:45.000000 apache-airflow-providers-amazon-8.3.0rc3/apache_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 15:12:45.000000 apache-airflow-providers-amazon-8.3.0rc3/apache_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      949 2023-07-09 15:12:45.000000 apache-airflow-providers-amazon-8.3.0rc3/apache_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-09 15:12:45.000000 apache-airflow-providers-amazon-8.3.0rc3/apache_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.3.0rc3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-07-09 15:12:46.129851 apache-airflow-providers-amazon-8.3.0rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-07-09 15:12:43.000000 apache-airflow-providers-amazon-8.3.0rc3/setup.py
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/LICENSE` & `apache-airflow-providers-amazon-8.3.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/MANIFEST.in` & `apache-airflow-providers-amazon-8.3.0rc3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/PKG-INFO` & `apache-airflow-providers-amazon-8.3.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.3.0rc2
+Version: 8.3.0rc3
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/
@@ -80,15 +80,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.3.0rc2``
+Release: ``8.3.0rc3``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/README.rst` & `apache-airflow-providers-amazon-8.3.0rc3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.3.0rc2``
+Release: ``8.3.0rc3``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/exceptions.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/appflow.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/athena.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         :param max_polling_attempts: Number of times to poll for query state before function exits
         :param sleep_time: Time (in seconds) to wait between two consecutive query status checks.
         :return: One of the final states
         """
         try:
             wait(
                 waiter=self.get_waiter("query_complete"),
-                waiter_delay=sleep_time or self.sleep_time,
+                waiter_delay=self.sleep_time if sleep_time is None else sleep_time,
                 waiter_max_attempts=max_polling_attempts or 120,
                 args={"QueryExecutionId": query_execution_id},
                 failure_message=f"Error while waiting for query {query_execution_id} to complete",
                 status_message=f"Query execution id: {query_execution_id}, "
                 f"Query is still in non-terminal state",
                 status_args=["QueryExecution.Status.State"],
             )
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/base_aws.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/batch_client.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/batch_waiters.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/chime.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/chime.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/datasync.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/dms.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/dynamodb.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/ec2.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/ecr.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/ecs.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/eks.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/emr.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/glacier.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/glue.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,17 @@
 
         :param crawler_kwargs: Keyword args that define the configurations used for the crawler
         :return: True if crawler was updated and false otherwise
         """
         crawler_name = crawler_kwargs["Name"]
         current_crawler = self.get_crawler(crawler_name)
 
-        tags_updated = self.update_tags(crawler_name, crawler_kwargs.pop("Tags", {}))
+        tags_updated = (
+            self.update_tags(crawler_name, crawler_kwargs.pop("Tags")) if "Tags" in crawler_kwargs else False
+        )
 
         update_config = {
             key: value
             for key, value in crawler_kwargs.items()
             if current_crawler.get(key, None) != crawler_kwargs.get(key)
         }
         if update_config:
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/kinesis.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/lambda_function.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/logs.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/quicksight.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/rds.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/redshift_data.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/redshift_sql.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -642,16 +642,15 @@
         min_objects: int = 1,
         previous_objects: set[str] | None = None,
         inactivity_seconds: int = 0,
         allow_delete: bool = True,
         last_activity_time: datetime | None = None,
     ) -> dict[str, Any]:
         """
-        Checks whether new objects have been uploaded and the inactivity_period
-        has passed and updates the state of the sensor accordingly.
+        Check if new objects have been uploaded and the period has passed; update sensor state accordingly.
 
         :param client: aiobotocore client
         :param bucket_name: the name of the bucket
         :param prefix: a key prefix
         :param inactivity_period:  the total seconds of inactivity to designate
             keys unchanged. Note, this mechanism is not real time and
             this operator may not return until a poke_interval after this period
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/sagemaker.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/ses.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/sns.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/sqs.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/ssm.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/step_function.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/hooks/sts.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/base_aws.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/batch.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/emr.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/glue.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/links/logs.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/links/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/log/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/log/s3_task_handler.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/notifications/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/notifications/chime.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/notifications/chime.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/appflow.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/athena.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/batch.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     BatchJobDefinitionLink,
     BatchJobDetailsLink,
     BatchJobQueueLink,
 )
 from airflow.providers.amazon.aws.links.logs import CloudWatchEventsLink
 from airflow.providers.amazon.aws.triggers.batch import (
     BatchCreateComputeEnvironmentTrigger,
-    BatchOperatorTrigger,
+    BatchJobTrigger,
 )
 from airflow.providers.amazon.aws.utils import trim_none_values
 from airflow.providers.amazon.aws.utils.task_log_fetcher import AwsTaskLogFetcher
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -217,20 +217,20 @@
         :raises: AirflowException
         """
         self.submit_job(context)
 
         if self.deferrable:
             self.defer(
                 timeout=self.execution_timeout,
-                trigger=BatchOperatorTrigger(
+                trigger=BatchJobTrigger(
                     job_id=self.job_id,
-                    max_retries=self.max_retries or 10,
+                    waiter_max_attempts=self.max_retries or 10,
                     aws_conn_id=self.aws_conn_id,
                     region_name=self.region_name,
-                    poll_interval=self.poll_interval,
+                    waiter_delay=self.poll_interval,
                 ),
                 method_name="execute_complete",
             )
 
         if self.wait_for_completion:
             self.monitor_job(context)
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/cloud_formation.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/datasync.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/dms.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/ec2.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/ecs.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,19 @@
 from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator, XCom
 from airflow.providers.amazon.aws.exceptions import EcsOperatorError, EcsTaskFailToStart
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.providers.amazon.aws.hooks.ecs import EcsClusterStates, EcsHook, should_retry_eni
 from airflow.providers.amazon.aws.hooks.logs import AwsLogsHook
-from airflow.providers.amazon.aws.triggers.ecs import ClusterWaiterTrigger, TaskDoneTrigger
+from airflow.providers.amazon.aws.triggers.ecs import (
+    ClusterActiveTrigger,
+    ClusterInactiveTrigger,
+    TaskDoneTrigger,
+)
 from airflow.providers.amazon.aws.utils.task_log_fetcher import AwsTaskLogFetcher
 from airflow.utils.helpers import prune_dict
 from airflow.utils.session import provide_session
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -135,21 +139,20 @@
 
         if cluster_state == EcsClusterStates.ACTIVE:
             # In some circumstances the ECS Cluster is created immediately,
             # and there is no reason to wait for completion.
             self.log.info("Cluster %r in state: %r.", self.cluster_name, cluster_state)
         elif self.deferrable:
             self.defer(
-                trigger=ClusterWaiterTrigger(
-                    waiter_name="cluster_active",
+                trigger=ClusterActiveTrigger(
                     cluster_arn=cluster_details["clusterArn"],
                     waiter_delay=self.waiter_delay,
                     waiter_max_attempts=self.waiter_max_attempts,
                     aws_conn_id=self.aws_conn_id,
-                    region=self.region,
+                    region_name=self.region,
                 ),
                 method_name="_complete_exec_with_cluster_desc",
                 # timeout is set to ensure that if a trigger dies, the timeout does not restart
                 # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
                 timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay + 60),
             )
         elif self.wait_for_completion:
@@ -213,21 +216,20 @@
 
         if cluster_state == EcsClusterStates.INACTIVE:
             # if the cluster doesn't have capacity providers that are associated with it,
             # the deletion is instantaneous, and we don't need to wait for it.
             self.log.info("Cluster %r in state: %r.", self.cluster_name, cluster_state)
         elif self.deferrable:
             self.defer(
-                trigger=ClusterWaiterTrigger(
-                    waiter_name="cluster_inactive",
+                trigger=ClusterInactiveTrigger(
                     cluster_arn=cluster_details["clusterArn"],
                     waiter_delay=self.waiter_delay,
                     waiter_max_attempts=self.waiter_max_attempts,
                     aws_conn_id=self.aws_conn_id,
-                    region=self.region,
+                    region_name=self.region,
                 ),
                 method_name="_complete_exec_with_cluster_desc",
                 # timeout is set to ensure that if a trigger dies, the timeout does not restart
                 # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
                 timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay + 60),
             )
         elif self.wait_for_completion:
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/eks.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/eks.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 
 from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.eks import EksHook
 from airflow.providers.amazon.aws.triggers.eks import (
     EksCreateFargateProfileTrigger,
+    EksCreateNodegroupTrigger,
     EksDeleteFargateProfileTrigger,
-    EksNodegroupTrigger,
+    EksDeleteNodegroupTrigger,
 )
 from airflow.providers.amazon.aws.utils.waiter_with_logging import wait
 from airflow.providers.cncf.kubernetes.utils.pod_manager import OnFinishAction
 
 try:
     from airflow.providers.cncf.kubernetes.operators.pod import KubernetesPodOperator
 except ImportError:
@@ -409,20 +410,19 @@
             nodegroup_role_arn=self.nodegroup_role_arn,
             create_nodegroup_kwargs=self.create_nodegroup_kwargs,
             subnets=self.nodegroup_subnets,
         )
 
         if self.deferrable:
             self.defer(
-                trigger=EksNodegroupTrigger(
-                    waiter_name="nodegroup_active",
+                trigger=EksCreateNodegroupTrigger(
                     cluster_name=self.cluster_name,
                     nodegroup_name=self.nodegroup_name,
                     aws_conn_id=self.aws_conn_id,
-                    region=self.region,
+                    region_name=self.region,
                     waiter_delay=self.waiter_delay,
                     waiter_max_attempts=self.waiter_max_attempts,
                 ),
                 method_name="execute_complete",
                 # timeout is set to ensure that if a trigger dies, the timeout does not restart
                 # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
                 timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay + 60),
@@ -707,20 +707,19 @@
             aws_conn_id=self.aws_conn_id,
             region_name=self.region,
         )
 
         eks_hook.delete_nodegroup(clusterName=self.cluster_name, nodegroupName=self.nodegroup_name)
         if self.deferrable:
             self.defer(
-                trigger=EksNodegroupTrigger(
-                    waiter_name="nodegroup_deleted",
+                trigger=EksDeleteNodegroupTrigger(
                     cluster_name=self.cluster_name,
                     nodegroup_name=self.nodegroup_name,
                     aws_conn_id=self.aws_conn_id,
-                    region=self.region,
+                    region_name=self.region,
                     waiter_delay=self.waiter_delay,
                     waiter_max_attempts=self.waiter_max_attempts,
                 ),
                 method_name="execute_complete",
                 # timeout is set to ensure that if a trigger dies, the timeout does not restart
                 # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
                 timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay + 60),
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/emr.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/emr.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,15 +573,15 @@
             )
             self.defer(
                 timeout=timeout,
                 trigger=EmrContainerTrigger(
                     virtual_cluster_id=self.virtual_cluster_id,
                     job_id=self.job_id,
                     aws_conn_id=self.aws_conn_id,
-                    poll_interval=self.poll_interval,
+                    waiter_delay=self.poll_interval,
                 ),
                 method_name="execute_complete",
             )
         if self.wait_for_completion:
             query_status = self.hook.poll_query_status(
                 self.job_id,
                 max_polling_attempts=self.max_polling_attempts,
@@ -939,16 +939,16 @@
         else:
             self.log.info("Terminating JobFlow with id %s", self.job_flow_id)
 
         if self.deferrable:
             self.defer(
                 trigger=EmrTerminateJobFlowTrigger(
                     job_flow_id=self.job_flow_id,
-                    poll_interval=self.waiter_delay,
-                    max_attempts=self.waiter_max_attempts,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
                     aws_conn_id=self.aws_conn_id,
                 ),
                 method_name="execute_complete",
                 # timeout is set to ensure that if a trigger dies, the timeout does not restart
                 # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
                 timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay + 60),
             )
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/glacier.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/glue.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/glue_crawler.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
         self.log.info("Triggering AWS Glue Crawler")
         self.hook.start_crawler(crawler_name)
         if self.deferrable:
             self.defer(
                 trigger=GlueCrawlerCompleteTrigger(
                     crawler_name=crawler_name,
-                    poll_interval=self.poll_interval,
+                    waiter_delay=self.poll_interval,
                     aws_conn_id=self.aws_conn_id,
                 ),
                 method_name="execute_complete",
             )
         elif self.wait_for_completion:
             self.log.info("Waiting for AWS Glue Crawler")
             self.hook.wait_for_crawler_completion(crawler_name=crawler_name, poll_interval=self.poll_interval)
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/lambda_function.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/quicksight.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/rds.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/rds.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,26 +39,36 @@
 
 class RdsBaseOperator(BaseOperator):
     """Base operator that implements common functions for all operators."""
 
     ui_color = "#eeaa88"
     ui_fgcolor = "#ffffff"
 
-    def __init__(self, *args, aws_conn_id: str = "aws_conn_id", hook_params: dict | None = None, **kwargs):
+    def __init__(
+        self,
+        *args,
+        aws_conn_id: str = "aws_conn_id",
+        region_name: str | None = None,
+        hook_params: dict | None = None,
+        **kwargs,
+    ):
         if hook_params is not None:
             warnings.warn(
                 "The parameter hook_params is deprecated and will be removed. "
-                "If you were using it, please get in touch either on airflow slack, "
-                "or by opening a github issue on the project. "
+                "Note that it is also incompatible with deferrable mode. "
+                "You can use the region_name parameter to specify the region. "
+                "If you were using hook_params for other purposes, please get in touch either on "
+                "airflow slack, or by opening a github issue on the project. "
                 "You can mention https://github.com/apache/airflow/pull/32352",
                 AirflowProviderDeprecationWarning,
                 stacklevel=3,  # 2 is in the operator's init, 3 is in the user code creating the operator
             )
-        self.hook_params = hook_params or {}
-        self.hook = RdsHook(aws_conn_id=aws_conn_id, **self.hook_params)
+        hook_params = hook_params or {}
+        self.region_name = region_name or hook_params.pop("region_name", None)
+        self.hook = RdsHook(aws_conn_id=aws_conn_id, region_name=self.region_name, **(hook_params))
         super().__init__(*args, **kwargs)
 
         self._await_interval = 60  # seconds
 
     def execute(self, context: Context) -> str:
         """Different implementations for snapshots, tasks and events."""
         raise NotImplementedError
@@ -584,15 +594,15 @@
         if self.deferrable:
             self.defer(
                 trigger=RdsDbInstanceTrigger(
                     db_instance_identifier=self.db_instance_identifier,
                     waiter_delay=self.waiter_delay,
                     waiter_max_attempts=self.waiter_max_attempts,
                     aws_conn_id=self.aws_conn_id,
-                    hook_params=self.hook_params,
+                    region_name=self.region_name,
                     waiter_name="db_instance_available",
                     # ignoring type because create_db_instance is a dict
                     response=create_db_instance,  # type: ignore[arg-type]
                 ),
                 method_name="execute_complete",
                 timeout=timedelta(seconds=self.waiter_delay * self.waiter_max_attempts),
             )
@@ -670,15 +680,15 @@
         if self.deferrable:
             self.defer(
                 trigger=RdsDbInstanceTrigger(
                     db_instance_identifier=self.db_instance_identifier,
                     waiter_delay=self.waiter_delay,
                     waiter_max_attempts=self.waiter_max_attempts,
                     aws_conn_id=self.aws_conn_id,
-                    hook_params=self.hook_params,
+                    region_name=self.region_name,
                     waiter_name="db_instance_deleted",
                     # ignoring type because delete_db_instance is a dict
                     response=delete_db_instance,  # type: ignore[arg-type]
                 ),
                 method_name="execute_complete",
                 timeout=timedelta(seconds=self.waiter_delay * self.waiter_max_attempts),
             )
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,16 +263,16 @@
             self.master_user_password,
             params,
         )
         if self.deferrable:
             self.defer(
                 trigger=RedshiftCreateClusterTrigger(
                     cluster_identifier=self.cluster_identifier,
-                    poll_interval=self.poll_interval,
-                    max_attempt=self.max_attempt,
+                    waiter_delay=self.poll_interval,
+                    waiter_max_attempts=self.max_attempt,
                     aws_conn_id=self.aws_conn_id,
                 ),
                 method_name="execute_complete",
             )
         if self.wait_for_completion:
             redshift_hook.get_conn().get_waiter("cluster_available").wait(
                 ClusterIdentifier=self.cluster_identifier,
@@ -357,16 +357,16 @@
             retention_period=self.retention_period,
             tags=self.tags,
         )
         if self.deferrable:
             self.defer(
                 trigger=RedshiftCreateClusterSnapshotTrigger(
                     cluster_identifier=self.cluster_identifier,
-                    poll_interval=self.poll_interval,
-                    max_attempts=self.max_attempt,
+                    waiter_delay=self.poll_interval,
+                    waiter_max_attempts=self.max_attempt,
                     aws_conn_id=self.aws_conn_id,
                 ),
                 method_name="execute_complete",
                 # timeout is set to ensure that if a trigger dies, the timeout does not restart
                 # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
                 timeout=timedelta(seconds=self.max_attempt * self.poll_interval + 60),
             )
@@ -506,16 +506,16 @@
                     time.sleep(self._attempt_interval)
                 else:
                     raise error
         if self.deferrable:
             self.defer(
                 trigger=RedshiftResumeClusterTrigger(
                     cluster_identifier=self.cluster_identifier,
-                    poll_interval=self.poll_interval,
-                    max_attempts=self.max_attempts,
+                    waiter_delay=self.poll_interval,
+                    waiter_max_attempts=self.max_attempts,
                     aws_conn_id=self.aws_conn_id,
                 ),
                 method_name="execute_complete",
                 # timeout is set to ensure that if a trigger dies, the timeout does not restart
                 # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
                 timeout=timedelta(seconds=self.max_attempts * self.poll_interval + 60),
             )
@@ -594,16 +594,16 @@
                     time.sleep(self._attempt_interval)
                 else:
                     raise error
         if self.deferrable:
             self.defer(
                 trigger=RedshiftPauseClusterTrigger(
                     cluster_identifier=self.cluster_identifier,
-                    poll_interval=self.poll_interval,
-                    max_attempts=self.max_attempts,
+                    waiter_delay=self.poll_interval,
+                    waiter_max_attempts=self.max_attempts,
                     aws_conn_id=self.aws_conn_id,
                 ),
                 method_name="execute_complete",
                 # timeout is set to ensure that if a trigger dies, the timeout does not restart
                 # 60 seconds is added to allow the trigger to exit gracefully (i.e. yield TriggerEvent)
                 timeout=timedelta(seconds=self.max_attempts * self.poll_interval + 60),
             )
@@ -686,16 +686,16 @@
                 else:
                     raise
         if self.deferrable:
             self.defer(
                 timeout=timedelta(seconds=self.max_attempts * self.poll_interval + 60),
                 trigger=RedshiftDeleteClusterTrigger(
                     cluster_identifier=self.cluster_identifier,
-                    poll_interval=self.poll_interval,
-                    max_attempts=self.max_attempts,
+                    waiter_delay=self.poll_interval,
+                    waiter_max_attempts=self.max_attempts,
                     aws_conn_id=self.aws_conn_id,
                 ),
                 method_name="execute_complete",
             )
         elif self.wait_for_completion:
             waiter = self.redshift_hook.get_conn().get_waiter("cluster_deleted")
             waiter.wait(
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/redshift_data.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/sagemaker.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/sns.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/sqs.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/operators/step_function.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/secrets/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/secrets/systems_manager.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/athena.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/batch.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from typing import TYPE_CHECKING, Any, Sequence
 
 from deprecated import deprecated
 
 from airflow.configuration import conf
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.batch_client import BatchClientHook
-from airflow.providers.amazon.aws.triggers.batch import BatchSensorTrigger
+from airflow.providers.amazon.aws.triggers.batch import BatchJobTrigger
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class BatchSensor(BaseSensorOperator):
@@ -94,32 +94,34 @@
             timeout = (
                 timedelta(seconds=self.max_retries * self.poke_interval + 60)
                 if self.max_retries
                 else self.execution_timeout
             )
             self.defer(
                 timeout=timeout,
-                trigger=BatchSensorTrigger(
+                trigger=BatchJobTrigger(
                     job_id=self.job_id,
                     aws_conn_id=self.aws_conn_id,
                     region_name=self.region_name,
-                    poke_interval=self.poke_interval,
+                    waiter_delay=int(self.poke_interval),
+                    waiter_max_attempts=self.max_retries,
                 ),
                 method_name="execute_complete",
             )
 
     def execute_complete(self, context: Context, event: dict[str, Any]) -> None:
         """
         Callback for when the trigger fires - returns immediately.
 
         Relies on trigger to throw an exception, otherwise it assumes execution was successful.
         """
-        if "status" in event and event["status"] == "failure":
-            raise AirflowException(event["message"])
-        self.log.info(event["message"])
+        if event["status"] != "success":
+            raise AirflowException(f"Error while running job: {event}")
+        job_id = event["job_id"]
+        self.log.info("Batch Job %s complete", job_id)
 
     @deprecated(reason="use `hook` property instead.")
     def get_hook(self) -> BatchClientHook:
         """Create and return a BatchClientHook."""
         return self.hook
 
     @cached_property
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/dms.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/dynamodb.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/ec2.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/ecs.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/eks.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/emr.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
             )
             self.defer(
                 timeout=timeout,
                 trigger=EmrContainerTrigger(
                     virtual_cluster_id=self.virtual_cluster_id,
                     job_id=self.job_id,
                     aws_conn_id=self.aws_conn_id,
-                    poll_interval=self.poll_interval,
+                    waiter_delay=self.poll_interval,
                 ),
                 method_name="execute_complete",
             )
 
     def execute_complete(self, context, event=None):
         if event["status"] != "success":
             raise AirflowException(f"Error while running job: {event}")
@@ -497,17 +497,17 @@
         if not self.deferrable:
             super().execute(context=context)
         elif not self.poke(context):
             self.defer(
                 timeout=timedelta(seconds=self.poke_interval * self.max_attempts),
                 trigger=EmrTerminateJobFlowTrigger(
                     job_flow_id=self.job_flow_id,
-                    max_attempts=self.max_attempts,
+                    waiter_max_attempts=self.max_attempts,
                     aws_conn_id=self.aws_conn_id,
-                    poll_interval=int(self.poke_interval),
+                    waiter_delay=int(self.poke_interval),
                 ),
                 method_name="execute_complete",
             )
 
     def execute_complete(self, context, event=None):
         if event["status"] != "success":
             raise AirflowException(f"Error while running job: {event}")
@@ -624,17 +624,17 @@
             super().execute(context=context)
         elif not self.poke(context):
             self.defer(
                 timeout=timedelta(seconds=self.max_attempts * self.poke_interval),
                 trigger=EmrStepSensorTrigger(
                     job_flow_id=self.job_flow_id,
                     step_id=self.step_id,
+                    waiter_delay=int(self.poke_interval),
+                    waiter_max_attempts=self.max_attempts,
                     aws_conn_id=self.aws_conn_id,
-                    max_attempts=self.max_attempts,
-                    poke_interval=int(self.poke_interval),
                 ),
                 method_name="execute_complete",
             )
 
     def execute_complete(self, context, event=None):
         if event["status"] != "success":
             raise AirflowException(f"Error while running job: {event}")
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/glacier.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/glue.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/lambda_function.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/quicksight.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/rds.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,13 +352,13 @@
                     ),
                     method_name="execute_complete",
                 )
 
     def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> None:
         """
         Callback for when the trigger fires - returns immediately.
-        Relies on trigger to throw an exception, otherwise it assumes execution was
-        successful.
+
+        Relies on trigger to throw an exception, otherwise it assumes execution was successful.
         """
         if event and event["status"] == "error":
             raise AirflowException(event["message"])
         return None
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/sagemaker.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/sqs.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/sensors/step_function.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/base.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,16 @@
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/transfer:DynamoDBToS3Operator`
 
     :param dynamodb_table_name: Dynamodb table to replicate data from
     :param s3_bucket_name: S3 bucket to replicate data to
     :param file_size: Flush file to s3 if file size >= file_size
-    :param dynamodb_scan_kwargs: kwargs pass to <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan>
+    :param dynamodb_scan_kwargs: kwargs pass to
+        <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan>
     :param s3_key_prefix: Prefix of s3 object key
     :param process_func: How we transform a dynamodb item to bytes. By default, we dump the json
     :param export_time: Time in the past from which to export table data, counted in seconds from the start of
      the Unix epoch. The table export will be a snapshot of the table's state at this point in time.
     :param export_format: The format for the exported data. Valid values for ExportFormat are DYNAMODB_JSON
      or ION.
     """
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sql.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/athena.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/athena.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,65 +12,47 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-from typing import Any
-
 from airflow.providers.amazon.aws.hooks.athena import AthenaHook
-from airflow.providers.amazon.aws.utils.waiter_with_logging import async_wait
-from airflow.triggers.base import BaseTrigger, TriggerEvent
+from airflow.providers.amazon.aws.hooks.base_aws import AwsGenericHook
+from airflow.providers.amazon.aws.triggers.base import AwsBaseWaiterTrigger
 
 
-class AthenaTrigger(BaseTrigger):
+class AthenaTrigger(AwsBaseWaiterTrigger):
     """
     Trigger for RedshiftCreateClusterOperator.
 
     The trigger will asynchronously poll the boto3 API and wait for the
     Redshift cluster to be in the `available` state.
 
     :param query_execution_id:  ID of the Athena query execution to watch
-    :param poll_interval: The amount of time in seconds to wait between attempts.
-    :param max_attempt: The maximum number of attempts to be made.
+    :param waiter_delay: The amount of time in seconds to wait between attempts.
+    :param waiter_max_attempts: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
     """
 
     def __init__(
         self,
         query_execution_id: str,
-        poll_interval: int,
-        max_attempt: int,
+        waiter_delay: int,
+        waiter_max_attempts: int,
         aws_conn_id: str,
     ):
-        self.query_execution_id = query_execution_id
-        self.poll_interval = poll_interval
-        self.max_attempt = max_attempt
-        self.aws_conn_id = aws_conn_id
-
-    def serialize(self) -> tuple[str, dict[str, Any]]:
-        return (
-            self.__class__.__module__ + "." + self.__class__.__qualname__,
-            {
-                "query_execution_id": str(self.query_execution_id),
-                "poll_interval": str(self.poll_interval),
-                "max_attempt": str(self.max_attempt),
-                "aws_conn_id": str(self.aws_conn_id),
-            },
+        super().__init__(
+            serialized_fields={"query_execution_id": query_execution_id},
+            waiter_name="query_complete",
+            waiter_args={"QueryExecutionId": query_execution_id},
+            failure_message=f"Error while waiting for query {query_execution_id} to complete",
+            status_message=f"Query execution id: {query_execution_id}",
+            status_queries=["QueryExecution.Status"],
+            return_value=query_execution_id,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
         )
 
-    async def run(self):
-        hook = AthenaHook(self.aws_conn_id)
-        async with hook.async_conn as client:
-            waiter = hook.get_waiter("query_complete", deferrable=True, client=client)
-            await async_wait(
-                waiter=waiter,
-                waiter_delay=self.poll_interval,
-                waiter_max_attempts=self.max_attempt,
-                args={"QueryExecutionId": self.query_execution_id},
-                failure_message=f"Error while waiting for query {self.query_execution_id} to complete",
-                status_message=f"Query execution id: {self.query_execution_id}, "
-                "Query is still in non-terminal state",
-                status_args=["QueryExecution.Status.State"],
-            )
-        yield TriggerEvent({"status": "success", "value": self.query_execution_id})
+    def hook(self) -> AwsGenericHook:
+        return AthenaHook(self.aws_conn_id)
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/batch.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/batch.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,20 +17,23 @@
 from __future__ import annotations
 
 import asyncio
 from functools import cached_property
 from typing import Any
 
 from botocore.exceptions import WaiterError
+from deprecated import deprecated
 
+from airflow.providers.amazon.aws.hooks.base_aws import AwsGenericHook
 from airflow.providers.amazon.aws.hooks.batch_client import BatchClientHook
-from airflow.providers.amazon.aws.utils.waiter_with_logging import async_wait
+from airflow.providers.amazon.aws.triggers.base import AwsBaseWaiterTrigger
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
+@deprecated(reason="use BatchJobTrigger instead")
 class BatchOperatorTrigger(BaseTrigger):
     """
     Asynchronously poll the boto3 API and wait for the Batch job to be in the `SUCCEEDED` state.
 
     :param job_id:  A unique identifier for the cluster.
     :param max_retries: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
@@ -102,14 +105,15 @@
 
         if attempt >= self.max_retries:
             yield TriggerEvent({"status": "failure", "message": "Job Failed - max attempts reached."})
         else:
             yield TriggerEvent({"status": "success", "job_id": self.job_id})
 
 
+@deprecated(reason="use BatchJobTrigger instead")
 class BatchSensorTrigger(BaseTrigger):
     """
     Checks for the status of a submitted job_id to AWS Batch until it reaches a failure or a success state.
 
     BatchSensorTrigger is fired as deferred class with params to poll the job state in Triggerer.
 
     :param job_id: the job ID, to poll for job completion or not
@@ -185,60 +189,82 @@
                     "status": "success",
                     "job_id": self.job_id,
                     "message": f"Job {self.job_id} Succeeded",
                 }
             )
 
 
-class BatchCreateComputeEnvironmentTrigger(BaseTrigger):
+class BatchJobTrigger(AwsBaseWaiterTrigger):
+    """
+    Checks for the status of a submitted job_id to AWS Batch until it reaches a failure or a success state.
+
+    :param job_id: the job ID, to poll for job completion or not
+    :param region_name: AWS region name to use
+        Override the region_name in connection (if provided)
+    :param aws_conn_id: connection id of AWS credentials / region name. If None,
+        credential boto3 strategy will be used
+    :param waiter_delay: polling period in seconds to check for the status of the job
+    :param waiter_max_attempts: The maximum number of attempts to be made.
+    """
+
+    def __init__(
+        self,
+        job_id: str | None,
+        region_name: str | None,
+        aws_conn_id: str | None = "aws_default",
+        waiter_delay: int = 5,
+        waiter_max_attempts: int = 720,
+    ):
+        super().__init__(
+            serialized_fields={"job_id": job_id},
+            waiter_name="batch_job_complete",
+            waiter_args={"jobs": [job_id]},
+            failure_message=f"Failure while running batch job {job_id}",
+            status_message=f"Batch job {job_id} not ready yet",
+            status_queries=["jobs[].status", "computeEnvironments[].statusReason"],
+            return_key="job_id",
+            return_value=job_id,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
+            region_name=region_name,
+        )
+
+    def hook(self) -> AwsGenericHook:
+        return BatchClientHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
+
+
+class BatchCreateComputeEnvironmentTrigger(AwsBaseWaiterTrigger):
     """
     Asynchronously poll the boto3 API and wait for the compute environment to be ready.
 
-    :param job_id:  A unique identifier for the cluster.
-    :param max_retries: The maximum number of attempts to be made.
+    :param compute_env_arn: The ARN of the compute env.
+    :param waiter_max_attempts: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
     :param region_name: region name to use in AWS Hook
-    :param poll_interval: The amount of time in seconds to wait between attempts.
+    :param waiter_delay: The amount of time in seconds to wait between attempts.
     """
 
     def __init__(
         self,
-        compute_env_arn: str | None = None,
-        poll_interval: int = 30,
-        max_retries: int = 10,
+        compute_env_arn: str,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 10,
         aws_conn_id: str | None = "aws_default",
         region_name: str | None = None,
     ):
-        super().__init__()
-        self.compute_env_arn = compute_env_arn
-        self.max_retries = max_retries
-        self.aws_conn_id = aws_conn_id
-        self.region_name = region_name
-        self.poll_interval = poll_interval
-
-    def serialize(self) -> tuple[str, dict[str, Any]]:
-        """Serializes BatchOperatorTrigger arguments and classpath."""
-        return (
-            self.__class__.__module__ + "." + self.__class__.__qualname__,
-            {
-                "compute_env_arn": self.compute_env_arn,
-                "max_retries": self.max_retries,
-                "aws_conn_id": self.aws_conn_id,
-                "region_name": self.region_name,
-                "poll_interval": self.poll_interval,
-            },
+        super().__init__(
+            serialized_fields={"compute_env_arn": compute_env_arn},
+            waiter_name="compute_env_ready",
+            waiter_args={"computeEnvironments": [compute_env_arn]},
+            failure_message="Failure while creating Compute Environment",
+            status_message="Compute Environment not ready yet",
+            status_queries=["computeEnvironments[].status", "computeEnvironments[].statusReason"],
+            return_value=compute_env_arn,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
+            region_name=region_name,
         )
 
-    async def run(self):
-        hook = BatchClientHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
-        async with hook.async_conn as client:
-            waiter = hook.get_waiter("compute_env_ready", deferrable=True, client=client)
-            await async_wait(
-                waiter=waiter,
-                waiter_delay=self.poll_interval,
-                waiter_max_attempts=self.max_retries,
-                args={"computeEnvironments": [self.compute_env_arn]},
-                failure_message="Failure while creating Compute Environment",
-                status_message="Compute Environment not ready yet",
-                status_args=["computeEnvironments[].status", "computeEnvironments[].statusReason"],
-            )
-            yield TriggerEvent({"status": "success", "value": self.compute_env_arn})
+    def hook(self) -> AwsGenericHook:
+        return BatchClientHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/ec2.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/ecs.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/ecs.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,76 +18,97 @@
 from __future__ import annotations
 
 import asyncio
 from typing import Any, AsyncIterator
 
 from botocore.exceptions import ClientError, WaiterError
 
+from airflow.providers.amazon.aws.hooks.base_aws import AwsGenericHook
 from airflow.providers.amazon.aws.hooks.ecs import EcsHook
 from airflow.providers.amazon.aws.hooks.logs import AwsLogsHook
+from airflow.providers.amazon.aws.triggers.base import AwsBaseWaiterTrigger
 from airflow.providers.amazon.aws.utils.task_log_fetcher import AwsTaskLogFetcher
-from airflow.providers.amazon.aws.utils.waiter_with_logging import async_wait
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
-class ClusterWaiterTrigger(BaseTrigger):
+class ClusterActiveTrigger(AwsBaseWaiterTrigger):
     """
-    Polls the status of a cluster using a given waiter. Can be used to poll for an active or inactive cluster.
+    Polls the status of a cluster until it's active.
 
-    :param waiter_name: Name of the waiter to use, for instance 'cluster_active' or 'cluster_inactive'
     :param cluster_arn: ARN of the cluster to watch.
     :param waiter_delay: The amount of time in seconds to wait between attempts.
     :param waiter_max_attempts: The number of times to ping for status.
         Will fail after that many unsuccessful attempts.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
-    :param region: The AWS region where the cluster is located.
+    :param region_name: The AWS region where the cluster is located.
     """
 
     def __init__(
         self,
-        waiter_name: str,
         cluster_arn: str,
-        waiter_delay: int | None,
-        waiter_max_attempts: int | None,
+        waiter_delay: int,
+        waiter_max_attempts: int,
         aws_conn_id: str | None,
-        region: str | None,
+        region_name: str | None,
     ):
-        self.cluster_arn = cluster_arn
-        self.waiter_name = waiter_name
-        self.waiter_delay = waiter_delay if waiter_delay is not None else 15  # written like this to allow 0
-        self.attempts = waiter_max_attempts or 999999999
-        self.aws_conn_id = aws_conn_id
-        self.region = region
-
-    def serialize(self) -> tuple[str, dict[str, Any]]:
-        return (
-            self.__class__.__module__ + "." + self.__class__.__qualname__,
-            {
-                "waiter_name": self.waiter_name,
-                "cluster_arn": self.cluster_arn,
-                "waiter_delay": self.waiter_delay,
-                "waiter_max_attempts": self.attempts,
-                "aws_conn_id": self.aws_conn_id,
-                "region": self.region,
-            },
+        super().__init__(
+            serialized_fields={"cluster_arn": cluster_arn},
+            waiter_name="cluster_active",
+            waiter_args={"clusters": [cluster_arn]},
+            failure_message="Failure while waiting for cluster to be available",
+            status_message="Cluster is not ready yet",
+            status_queries=["clusters[].status", "failures"],
+            return_key="arn",
+            return_value=cluster_arn,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
+            region_name=region_name,
         )
 
-    async def run(self) -> AsyncIterator[TriggerEvent]:
-        async with EcsHook(aws_conn_id=self.aws_conn_id, region_name=self.region).async_conn as client:
-            waiter = client.get_waiter(self.waiter_name)
-            await async_wait(
-                waiter,
-                self.waiter_delay,
-                self.attempts,
-                {"clusters": [self.cluster_arn]},
-                "error when checking cluster status",
-                "Status of cluster",
-                ["clusters[].status"],
-            )
-            yield TriggerEvent({"status": "success", "arn": self.cluster_arn})
+    def hook(self) -> AwsGenericHook:
+        return EcsHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
+
+
+class ClusterInactiveTrigger(AwsBaseWaiterTrigger):
+    """
+    Polls the status of a cluster until it's inactive.
+
+    :param cluster_arn: ARN of the cluster to watch.
+    :param waiter_delay: The amount of time in seconds to wait between attempts.
+    :param waiter_max_attempts: The number of times to ping for status.
+        Will fail after that many unsuccessful attempts.
+    :param aws_conn_id: The Airflow connection used for AWS credentials.
+    :param region_name: The AWS region where the cluster is located.
+    """
+
+    def __init__(
+        self,
+        cluster_arn: str,
+        waiter_delay: int,
+        waiter_max_attempts: int,
+        aws_conn_id: str | None,
+        region_name: str | None,
+    ):
+        super().__init__(
+            serialized_fields={"cluster_arn": cluster_arn},
+            waiter_name="cluster_inactive",
+            waiter_args={"clusters": [cluster_arn]},
+            failure_message="Failure while waiting for cluster to be deactivated",
+            status_message="Cluster deactivation is not done yet",
+            status_queries=["clusters[].status", "failures"],
+            return_value=cluster_arn,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
+            region_name=region_name,
+        )
+
+    def hook(self) -> AwsGenericHook:
+        return EcsHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
 
 
 class TaskDoneTrigger(BaseTrigger):
     """
     Waits for an ECS task to be done, while eventually polling logs.
 
     :param cluster: short name or full ARN of the cluster where the task is running.
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/eks.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/eks.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,26 +12,23 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-import asyncio
-from typing import Any
+import warnings
 
-from botocore.exceptions import WaiterError
-
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowProviderDeprecationWarning
+from airflow.providers.amazon.aws.hooks.base_aws import AwsGenericHook
 from airflow.providers.amazon.aws.hooks.eks import EksHook
-from airflow.providers.amazon.aws.utils.waiter_with_logging import async_wait
-from airflow.triggers.base import BaseTrigger, TriggerEvent
+from airflow.providers.amazon.aws.triggers.base import AwsBaseWaiterTrigger
 
 
-class EksCreateFargateProfileTrigger(BaseTrigger):
+class EksCreateFargateProfileTrigger(AwsBaseWaiterTrigger):
     """
     Asynchronously wait for the fargate profile to be created.
 
     :param cluster_name: The name of the EKS cluster
     :param fargate_profile_name: The name of the fargate profile
     :param waiter_delay: The amount of time in seconds to wait between attempts.
     :param waiter_max_attempts: The maximum number of attempts to be made.
@@ -42,65 +39,43 @@
         self,
         cluster_name: str,
         fargate_profile_name: str,
         waiter_delay: int,
         waiter_max_attempts: int,
         aws_conn_id: str,
         region: str | None = None,
+        region_name: str | None = None,
     ):
-        self.cluster_name = cluster_name
-        self.fargate_profile_name = fargate_profile_name
-        self.waiter_delay = waiter_delay
-        self.waiter_max_attempts = waiter_max_attempts
-        self.aws_conn_id = aws_conn_id
-        self.region = region
-
-    def serialize(self) -> tuple[str, dict[str, Any]]:
-        return (
-            self.__class__.__module__ + "." + self.__class__.__qualname__,
-            {
-                "cluster_name": self.cluster_name,
-                "fargate_profile_name": self.fargate_profile_name,
-                "waiter_delay": str(self.waiter_delay),
-                "waiter_max_attempts": str(self.waiter_max_attempts),
-                "aws_conn_id": self.aws_conn_id,
-                "region": self.region,
-            },
+        if region is not None:
+            warnings.warn(
+                "please use region_name param instead of region",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+            region_name = region
+
+        super().__init__(
+            serialized_fields={"cluster_name": cluster_name, "fargate_profile_name": fargate_profile_name},
+            waiter_name="fargate_profile_active",
+            waiter_args={"clusterName": cluster_name, "fargateProfileName": fargate_profile_name},
+            failure_message="Failure while creating Fargate profile",
+            status_message="Fargate profile not created yet",
+            status_queries=["fargateProfile.status"],
+            return_value=None,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
+            region_name=region_name,
         )
 
-    async def run(self):
-        self.hook = EksHook(aws_conn_id=self.aws_conn_id, region_name=self.region)
-        async with self.hook.async_conn as client:
-            attempt = 0
-            waiter = client.get_waiter("fargate_profile_active")
-            while attempt < int(self.waiter_max_attempts):
-                attempt += 1
-                try:
-                    await waiter.wait(
-                        clusterName=self.cluster_name,
-                        fargateProfileName=self.fargate_profile_name,
-                        WaiterConfig={"Delay": int(self.waiter_delay), "MaxAttempts": 1},
-                    )
-                    break
-                except WaiterError as error:
-                    if "terminal failure" in str(error):
-                        raise AirflowException(f"Create Fargate Profile failed: {error}")
-                    self.log.info(
-                        "Status of fargate profile is %s", error.last_response["fargateProfile"]["status"]
-                    )
-                    await asyncio.sleep(int(self.waiter_delay))
-        if attempt >= int(self.waiter_max_attempts):
-            raise AirflowException(
-                f"Create Fargate Profile failed - max attempts reached: {self.waiter_max_attempts}"
-            )
-        else:
-            yield TriggerEvent({"status": "success", "message": "Fargate Profile Created"})
+    def hook(self) -> AwsGenericHook:
+        return EksHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
 
 
-class EksDeleteFargateProfileTrigger(BaseTrigger):
+class EksDeleteFargateProfileTrigger(AwsBaseWaiterTrigger):
     """
     Asynchronously wait for the fargate profile to be deleted.
 
     :param cluster_name: The name of the EKS cluster
     :param fargate_profile_name: The name of the fargate profile
     :param waiter_delay: The amount of time in seconds to wait between attempts.
     :param waiter_max_attempts: The maximum number of attempts to be made.
@@ -111,67 +86,45 @@
         self,
         cluster_name: str,
         fargate_profile_name: str,
         waiter_delay: int,
         waiter_max_attempts: int,
         aws_conn_id: str,
         region: str | None = None,
+        region_name: str | None = None,
     ):
-        self.cluster_name = cluster_name
-        self.fargate_profile_name = fargate_profile_name
-        self.waiter_delay = waiter_delay
-        self.waiter_max_attempts = waiter_max_attempts
-        self.aws_conn_id = aws_conn_id
-        self.region = region
-
-    def serialize(self) -> tuple[str, dict[str, Any]]:
-        return (
-            self.__class__.__module__ + "." + self.__class__.__qualname__,
-            {
-                "cluster_name": self.cluster_name,
-                "fargate_profile_name": self.fargate_profile_name,
-                "waiter_delay": str(self.waiter_delay),
-                "waiter_max_attempts": str(self.waiter_max_attempts),
-                "aws_conn_id": self.aws_conn_id,
-                "region": self.region,
-            },
+        if region is not None:
+            warnings.warn(
+                "please use region_name param instead of region",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+            region_name = region
+
+        super().__init__(
+            serialized_fields={"cluster_name": cluster_name, "fargate_profile_name": fargate_profile_name},
+            waiter_name="fargate_profile_deleted",
+            waiter_args={"clusterName": cluster_name, "fargateProfileName": fargate_profile_name},
+            failure_message="Failure while deleting Fargate profile",
+            status_message="Fargate profile not deleted yet",
+            status_queries=["fargateProfile.status"],
+            return_value=None,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
+            region_name=region_name,
         )
 
-    async def run(self):
-        self.hook = EksHook(aws_conn_id=self.aws_conn_id, region_name=self.region)
-        async with self.hook.async_conn as client:
-            attempt = 0
-            waiter = client.get_waiter("fargate_profile_deleted")
-            while attempt < int(self.waiter_max_attempts):
-                attempt += 1
-                try:
-                    await waiter.wait(
-                        clusterName=self.cluster_name,
-                        fargateProfileName=self.fargate_profile_name,
-                        WaiterConfig={"Delay": int(self.waiter_delay), "MaxAttempts": 1},
-                    )
-                    break
-                except WaiterError as error:
-                    if "terminal failure" in str(error):
-                        raise AirflowException(f"Delete Fargate Profile failed: {error}")
-                    self.log.info(
-                        "Status of fargate profile is %s", error.last_response["fargateProfile"]["status"]
-                    )
-                    await asyncio.sleep(int(self.waiter_delay))
-        if attempt >= int(self.waiter_max_attempts):
-            raise AirflowException(
-                f"Delete Fargate Profile failed - max attempts reached: {self.waiter_max_attempts}"
-            )
-        else:
-            yield TriggerEvent({"status": "success", "message": "Fargate Profile Deleted"})
+    def hook(self) -> AwsGenericHook:
+        return EksHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
 
 
-class EksNodegroupTrigger(BaseTrigger):
+class EksCreateNodegroupTrigger(AwsBaseWaiterTrigger):
     """
-    Trigger for EksCreateNodegroupOperator and EksDeleteNodegroupOperator.
+    Trigger for EksCreateNodegroupOperator.
 
     The trigger will asynchronously poll the boto3 API and wait for the
     nodegroup to be in the state specified by the waiter.
 
     :param waiter_name: Name of the waiter to use, for instance 'nodegroup_active' or 'nodegroup_deleted'
     :param cluster_name: The name of the EKS cluster associated with the node group.
     :param nodegroup_name: The name of the nodegroup to check.
@@ -180,58 +133,74 @@
     :param aws_conn_id: The Airflow connection used for AWS credentials.
     :param region: Which AWS region the connection should use. (templated)
         If this is None or empty then the default boto3 behaviour is used.
     """
 
     def __init__(
         self,
-        waiter_name: str,
         cluster_name: str,
         nodegroup_name: str,
         waiter_delay: int,
         waiter_max_attempts: int,
         aws_conn_id: str,
-        region: str | None,
+        region_name: str | None,
     ):
-        self.waiter_name = waiter_name
-        self.cluster_name = cluster_name
-        self.nodegroup_name = nodegroup_name
-        self.aws_conn_id = aws_conn_id
-        self.waiter_delay = waiter_delay
-        self.waiter_max_attempts = waiter_max_attempts
-        self.region = region
-
-    def serialize(self) -> tuple[str, dict[str, Any]]:
-        return (
-            self.__class__.__module__ + "." + self.__class__.__qualname__,
-            {
-                "waiter_name": self.waiter_name,
-                "cluster_name": self.cluster_name,
-                "nodegroup_name": self.nodegroup_name,
-                "waiter_delay": str(self.waiter_delay),
-                "waiter_max_attempts": str(self.waiter_max_attempts),
-                "aws_conn_id": self.aws_conn_id,
-                "region": self.region,
-            },
+        super().__init__(
+            serialized_fields={"cluster_name": cluster_name, "nodegroup_name": nodegroup_name},
+            waiter_name="nodegroup_active",
+            waiter_args={"clusterName": cluster_name, "nodegroupName": nodegroup_name},
+            failure_message="Error creating nodegroup",
+            status_message="Nodegroup status is",
+            status_queries=["nodegroup.status", "nodegroup.health.issues"],
+            return_value=None,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
+            region_name=region_name,
         )
 
-    async def run(self):
-        self.hook = EksHook(aws_conn_id=self.aws_conn_id, region_name=self.region)
-        async with self.hook.async_conn as client:
-            waiter = client.get_waiter(self.waiter_name)
-            await async_wait(
-                waiter=waiter,
-                waiter_max_attempts=int(self.waiter_max_attempts),
-                waiter_delay=int(self.waiter_delay),
-                args={"clusterName": self.cluster_name, "nodegroupName": self.nodegroup_name},
-                failure_message="Error checking nodegroup",
-                status_message="Nodegroup status is",
-                status_args=["nodegroup.status"],
-            )
+    def hook(self) -> AwsGenericHook:
+        return EksHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
+
 
-        yield TriggerEvent(
-            {
-                "status": "success",
-                "cluster_name": self.cluster_name,
-                "nodegroup_name": self.nodegroup_name,
-            }
+class EksDeleteNodegroupTrigger(AwsBaseWaiterTrigger):
+    """
+    Trigger for EksDeleteNodegroupOperator.
+
+    The trigger will asynchronously poll the boto3 API and wait for the
+    nodegroup to be in the state specified by the waiter.
+
+    :param waiter_name: Name of the waiter to use, for instance 'nodegroup_active' or 'nodegroup_deleted'
+    :param cluster_name: The name of the EKS cluster associated with the node group.
+    :param nodegroup_name: The name of the nodegroup to check.
+    :param waiter_delay: The amount of time in seconds to wait between attempts.
+    :param waiter_max_attempts: The maximum number of attempts to be made.
+    :param aws_conn_id: The Airflow connection used for AWS credentials.
+    :param region: Which AWS region the connection should use. (templated)
+        If this is None or empty then the default boto3 behaviour is used.
+    """
+
+    def __init__(
+        self,
+        cluster_name: str,
+        nodegroup_name: str,
+        waiter_delay: int,
+        waiter_max_attempts: int,
+        aws_conn_id: str,
+        region_name: str | None,
+    ):
+        super().__init__(
+            serialized_fields={"cluster_name": cluster_name, "nodegroup_name": nodegroup_name},
+            waiter_name="nodegroup_deleted",
+            waiter_args={"clusterName": cluster_name, "nodegroupName": nodegroup_name},
+            failure_message="Error deleting nodegroup",
+            status_message="Nodegroup status is",
+            status_queries=["nodegroup.status", "nodegroup.health.issues"],
+            return_value=None,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
+            region_name=region_name,
         )
+
+    def hook(self) -> AwsGenericHook:
+        return EksHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/emr.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/emr.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import asyncio
-from functools import cached_property
-from typing import Any, AsyncIterator
+import warnings
+from typing import Any
 
 from botocore.exceptions import WaiterError
 
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowProviderDeprecationWarning
+from airflow.providers.amazon.aws.hooks.base_aws import AwsGenericHook
 from airflow.providers.amazon.aws.hooks.emr import EmrContainerHook, EmrHook
-from airflow.providers.amazon.aws.utils.waiter_with_logging import async_wait
+from airflow.providers.amazon.aws.triggers.base import AwsBaseWaiterTrigger
 from airflow.triggers.base import BaseTrigger, TriggerEvent
-from airflow.utils.helpers import prune_dict
 
 
 class EmrAddStepsTrigger(BaseTrigger):
     """
     Asynchronously poll the boto3 API and wait for the steps to finish executing.
 
     :param job_flow_id: The id of the job flow.
@@ -98,278 +98,188 @@
                         await asyncio.sleep(int(self.poll_interval))
         if attempt >= int(self.max_attempts):
             yield TriggerEvent({"status": "failure", "message": "Steps failed: max attempts reached"})
         else:
             yield TriggerEvent({"status": "success", "message": "Steps completed", "step_ids": self.step_ids})
 
 
-class EmrCreateJobFlowTrigger(BaseTrigger):
+class EmrCreateJobFlowTrigger(AwsBaseWaiterTrigger):
     """
     Asynchronously poll the boto3 API and wait for the JobFlow to finish executing.
 
     :param job_flow_id: The id of the job flow to wait for.
-    :param poll_interval: The amount of time in seconds to wait between attempts.
-    :param max_attempts: The maximum number of attempts to be made.
+    :param waiter_delay: The amount of time in seconds to wait between attempts.
+    :param waiter_max_attempts: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
     """
 
     def __init__(
         self,
         job_flow_id: str,
-        poll_interval: int,
-        max_attempts: int,
-        aws_conn_id: str,
+        poll_interval: int | None = None,  # deprecated
+        max_attempts: int | None = None,  # deprecated
+        aws_conn_id: str | None = None,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 60,
     ):
-        self.job_flow_id = job_flow_id
-        self.poll_interval = poll_interval
-        self.max_attempts = max_attempts
-        self.aws_conn_id = aws_conn_id
-
-    def serialize(self) -> tuple[str, dict[str, Any]]:
-        return (
-            self.__class__.__module__ + "." + self.__class__.__qualname__,
-            {
-                "job_flow_id": self.job_flow_id,
-                "poll_interval": str(self.poll_interval),
-                "max_attempts": str(self.max_attempts),
-                "aws_conn_id": self.aws_conn_id,
-            },
+        if poll_interval is not None or max_attempts is not None:
+            warnings.warn(
+                "please use waiter_delay instead of poll_interval "
+                "and waiter_max_attempts instead of max_attempts",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+            waiter_delay = poll_interval or waiter_delay
+            waiter_max_attempts = max_attempts or waiter_max_attempts
+        super().__init__(
+            serialized_fields={"job_flow_id": job_flow_id},
+            waiter_name="job_flow_waiting",
+            waiter_args={"ClusterId": job_flow_id},
+            failure_message="JobFlow creation failed",
+            status_message="JobFlow creation in progress",
+            status_queries=[
+                "Cluster.Status.State",
+                "Cluster.Status.StateChangeReason",
+                "Cluster.Status.ErrorDetails",
+            ],
+            return_key="job_flow_id",
+            return_value=job_flow_id,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
         )
 
-    async def run(self):
-        self.hook = EmrHook(aws_conn_id=self.aws_conn_id)
-        async with self.hook.async_conn as client:
-            attempt = 0
-            waiter = self.hook.get_waiter("job_flow_waiting", deferrable=True, client=client)
-            while attempt < int(self.max_attempts):
-                attempt = attempt + 1
-                try:
-                    await waiter.wait(
-                        ClusterId=self.job_flow_id,
-                        WaiterConfig=prune_dict(
-                            {
-                                "Delay": self.poll_interval,
-                                "MaxAttempts": 1,
-                            }
-                        ),
-                    )
-                    break
-                except WaiterError as error:
-                    if "terminal failure" in str(error):
-                        raise AirflowException(f"JobFlow creation failed: {error}")
-                    self.log.info(
-                        "Status of jobflow is %s - %s",
-                        error.last_response["Cluster"]["Status"]["State"],
-                        error.last_response["Cluster"]["Status"]["StateChangeReason"],
-                    )
-                    await asyncio.sleep(int(self.poll_interval))
-        if attempt >= int(self.max_attempts):
-            raise AirflowException(f"JobFlow creation failed - max attempts reached: {self.max_attempts}")
-        else:
-            yield TriggerEvent(
-                {
-                    "status": "success",
-                    "message": "JobFlow completed successfully",
-                    "job_flow_id": self.job_flow_id,
-                }
-            )
+    def hook(self) -> AwsGenericHook:
+        return EmrHook(aws_conn_id=self.aws_conn_id)
 
 
-class EmrTerminateJobFlowTrigger(BaseTrigger):
+class EmrTerminateJobFlowTrigger(AwsBaseWaiterTrigger):
     """
     Asynchronously poll the boto3 API and wait for the JobFlow to finish terminating.
 
     :param job_flow_id: ID of the EMR Job Flow to terminate
-    :param poll_interval: The amount of time in seconds to wait between attempts.
-    :param max_attempts: The maximum number of attempts to be made.
+    :param waiter_delay: The amount of time in seconds to wait between attempts.
+    :param waiter_max_attempts: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
     """
 
     def __init__(
         self,
         job_flow_id: str,
-        poll_interval: int,
-        max_attempts: int,
-        aws_conn_id: str,
+        poll_interval: int | None = None,  # deprecated
+        max_attempts: int | None = None,  # deprecated
+        aws_conn_id: str | None = None,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 60,
     ):
-        self.job_flow_id = job_flow_id
-        self.poll_interval = poll_interval
-        self.max_attempts = max_attempts
-        self.aws_conn_id = aws_conn_id
-
-    def serialize(self) -> tuple[str, dict[str, Any]]:
-        return (
-            self.__class__.__module__ + "." + self.__class__.__qualname__,
-            {
-                "job_flow_id": self.job_flow_id,
-                "poll_interval": str(self.poll_interval),
-                "max_attempts": str(self.max_attempts),
-                "aws_conn_id": self.aws_conn_id,
-            },
+        if poll_interval is not None or max_attempts is not None:
+            warnings.warn(
+                "please use waiter_delay instead of poll_interval "
+                "and waiter_max_attempts instead of max_attempts",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+            waiter_delay = poll_interval or waiter_delay
+            waiter_max_attempts = max_attempts or waiter_max_attempts
+        super().__init__(
+            serialized_fields={"job_flow_id": job_flow_id},
+            waiter_name="job_flow_terminated",
+            waiter_args={"ClusterId": job_flow_id},
+            failure_message="JobFlow termination failed",
+            status_message="JobFlow termination in progress",
+            status_queries=[
+                "Cluster.Status.State",
+                "Cluster.Status.StateChangeReason",
+                "Cluster.Status.ErrorDetails",
+            ],
+            return_value=None,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
         )
 
-    async def run(self):
-        self.hook = EmrHook(aws_conn_id=self.aws_conn_id)
-        async with self.hook.async_conn as client:
-            attempt = 0
-            waiter = self.hook.get_waiter("job_flow_terminated", deferrable=True, client=client)
-            while attempt < int(self.max_attempts):
-                attempt = attempt + 1
-                try:
-                    await waiter.wait(
-                        ClusterId=self.job_flow_id,
-                        WaiterConfig=prune_dict(
-                            {
-                                "Delay": self.poll_interval,
-                                "MaxAttempts": 1,
-                            }
-                        ),
-                    )
-                    break
-                except WaiterError as error:
-                    if "terminal failure" in str(error):
-                        raise AirflowException(f"JobFlow termination failed: {error}")
-                    self.log.info(
-                        "Status of jobflow is %s - %s",
-                        error.last_response["Cluster"]["Status"]["State"],
-                        error.last_response["Cluster"]["Status"]["StateChangeReason"],
-                    )
-                    await asyncio.sleep(int(self.poll_interval))
-        if attempt >= int(self.max_attempts):
-            raise AirflowException(f"JobFlow termination failed - max attempts reached: {self.max_attempts}")
-        else:
-            yield TriggerEvent(
-                {
-                    "status": "success",
-                    "message": "JobFlow terminated successfully",
-                }
-            )
+    def hook(self) -> AwsGenericHook:
+        return EmrHook(aws_conn_id=self.aws_conn_id)
 
 
-class EmrContainerTrigger(BaseTrigger):
+class EmrContainerTrigger(AwsBaseWaiterTrigger):
     """
     Poll for the status of EMR container until reaches terminal state.
 
     :param virtual_cluster_id: Reference Emr cluster id
     :param job_id:  job_id to check the state
     :param aws_conn_id: Reference to AWS connection id
-    :param poll_interval: polling period in seconds to check for the status
+    :param waiter_delay: polling period in seconds to check for the status
     """
 
     def __init__(
         self,
         virtual_cluster_id: str,
         job_id: str,
         aws_conn_id: str = "aws_default",
-        poll_interval: int = 30,
-        **kwargs: Any,
+        poll_interval: int | None = None,  # deprecated
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 600,
     ):
-        self.virtual_cluster_id = virtual_cluster_id
-        self.job_id = job_id
-        self.aws_conn_id = aws_conn_id
-        self.poll_interval = poll_interval
-        super().__init__(**kwargs)
-
-    @cached_property
-    def hook(self) -> EmrContainerHook:
-        return EmrContainerHook(self.aws_conn_id, virtual_cluster_id=self.virtual_cluster_id)
-
-    def serialize(self) -> tuple[str, dict[str, Any]]:
-        """Serializes EmrContainerTrigger arguments and classpath."""
-        return (
-            "airflow.providers.amazon.aws.triggers.emr.EmrContainerTrigger",
-            {
-                "virtual_cluster_id": self.virtual_cluster_id,
-                "job_id": self.job_id,
-                "aws_conn_id": self.aws_conn_id,
-                "poll_interval": self.poll_interval,
-            },
+        if poll_interval is not None:
+            warnings.warn(
+                "please use waiter_delay instead of poll_interval.",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+            waiter_delay = poll_interval or waiter_delay
+        super().__init__(
+            serialized_fields={"virtual_cluster_id": virtual_cluster_id, "job_id": job_id},
+            waiter_name="container_job_complete",
+            waiter_args={"id": job_id, "virtualClusterId": virtual_cluster_id},
+            failure_message="Job failed",
+            status_message="Job in progress",
+            status_queries=["jobRun.state", "jobRun.failureReason"],
+            return_key="job_id",
+            return_value=job_id,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
         )
 
-    async def run(self) -> AsyncIterator[TriggerEvent]:
-        async with self.hook.async_conn as client:
-            waiter = self.hook.get_waiter("container_job_complete", deferrable=True, client=client)
-            attempt = 0
-            while True:
-                attempt = attempt + 1
-                try:
-                    await waiter.wait(
-                        id=self.job_id,
-                        virtualClusterId=self.virtual_cluster_id,
-                        WaiterConfig={
-                            "Delay": self.poll_interval,
-                            "MaxAttempts": 1,
-                        },
-                    )
-                    break
-                except WaiterError as error:
-                    if "terminal failure" in str(error):
-                        yield TriggerEvent({"status": "failure", "message": f"Job Failed: {error}"})
-                        break
-                    self.log.info(
-                        "Job status is %s. Retrying attempt %s",
-                        error.last_response["jobRun"]["state"],
-                        attempt,
-                    )
-                    await asyncio.sleep(int(self.poll_interval))
-
-            yield TriggerEvent({"status": "success", "job_id": self.job_id})
+    def hook(self) -> AwsGenericHook:
+        return EmrContainerHook(self.aws_conn_id)
 
 
-class EmrStepSensorTrigger(BaseTrigger):
+class EmrStepSensorTrigger(AwsBaseWaiterTrigger):
     """
     Poll for the status of EMR container until reaches terminal state.
 
     :param job_flow_id: job_flow_id which contains the step check the state of
     :param step_id:  step to check the state of
+    :param waiter_delay: polling period in seconds to check for the status
+    :param waiter_max_attempts: The maximum number of attempts to be made
     :param aws_conn_id: Reference to AWS connection id
-    :param max_attempts: The maximum number of attempts to be made
-    :param poke_interval: polling period in seconds to check for the status
     """
 
     def __init__(
         self,
         job_flow_id: str,
         step_id: str,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 60,
         aws_conn_id: str = "aws_default",
-        max_attempts: int = 60,
-        poke_interval: int = 30,
-        **kwargs: Any,
     ):
-        self.job_flow_id = job_flow_id
-        self.step_id = step_id
-        self.aws_conn_id = aws_conn_id
-        self.max_attempts = max_attempts
-        self.poke_interval = poke_interval
-        super().__init__(**kwargs)
-
-    @cached_property
-    def hook(self) -> EmrHook:
-        return EmrHook(self.aws_conn_id)
-
-    def serialize(self) -> tuple[str, dict[str, Any]]:
-        return (
-            "airflow.providers.amazon.aws.triggers.emr.EmrStepSensorTrigger",
-            {
-                "job_flow_id": self.job_flow_id,
-                "step_id": self.step_id,
-                "aws_conn_id": self.aws_conn_id,
-                "max_attempts": self.max_attempts,
-                "poke_interval": self.poke_interval,
-            },
+        super().__init__(
+            serialized_fields={"job_flow_id": job_flow_id, "step_id": step_id},
+            waiter_name="step_wait_for_terminal",
+            waiter_args={"ClusterId": job_flow_id, "StepId": step_id},
+            failure_message=f"Error while waiting for step {step_id} to complete",
+            status_message=f"Step id: {step_id}, Step is still in non-terminal state",
+            status_queries=[
+                "Step.Status.State",
+                "Step.Status.FailureDetails",
+                "Step.Status.StateChangeReason",
+            ],
+            return_value=None,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
         )
 
-    async def run(self) -> AsyncIterator[TriggerEvent]:
-
-        async with self.hook.async_conn as client:
-            waiter = client.get_waiter("step_wait_for_terminal", deferrable=True, client=client)
-            await async_wait(
-                waiter=waiter,
-                waiter_delay=self.poke_interval,
-                waiter_max_attempts=self.max_attempts,
-                args={"ClusterId": self.job_flow_id, "StepId": self.step_id},
-                failure_message=f"Error while waiting for step {self.step_id} to complete",
-                status_message=f"Step id: {self.step_id}, Step is still in non-terminal state",
-                status_args=["Step.Status.State"],
-            )
-
-        yield TriggerEvent({"status": "success"})
+    def hook(self) -> AwsGenericHook:
+        return EmrHook(self.aws_conn_id)
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/glue.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/rds.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/rds.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,42 +43,42 @@
     def __init__(
         self,
         waiter_name: str,
         db_instance_identifier: str,
         waiter_delay: int,
         waiter_max_attempts: int,
         aws_conn_id: str,
-        hook_params: dict[str, Any],
+        region_name: str | None,
         response: dict[str, Any],
     ):
         self.db_instance_identifier = db_instance_identifier
         self.waiter_delay = waiter_delay
         self.waiter_max_attempts = waiter_max_attempts
         self.aws_conn_id = aws_conn_id
-        self.hook_params = hook_params
+        self.region_name = region_name
         self.waiter_name = waiter_name
         self.response = response
 
     def serialize(self) -> tuple[str, dict[str, Any]]:
         return (
             # dynamically generate the fully qualified name of the class
             self.__class__.__module__ + "." + self.__class__.__qualname__,
             {
                 "db_instance_identifier": self.db_instance_identifier,
                 "waiter_delay": str(self.waiter_delay),
                 "waiter_max_attempts": str(self.waiter_max_attempts),
                 "aws_conn_id": self.aws_conn_id,
-                "hook_params": self.hook_params,
+                "region_name": self.region_name,
                 "waiter_name": self.waiter_name,
                 "response": self.response,
             },
         )
 
     async def run(self):
-        self.hook = RdsHook(aws_conn_id=self.aws_conn_id, **self.hook_params)
+        self.hook = RdsHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
         async with self.hook.async_conn as client:
             waiter = client.get_waiter(self.waiter_name)
             await async_wait(
                 waiter=waiter,
                 waiter_delay=int(self.waiter_delay),
                 waiter_max_attempts=int(self.waiter_max_attempts),
                 args={"DBInstanceIdentifier": self.db_instance_identifier},
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/s3.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/triggers/sagemaker.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/triggers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/eks_get_token.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/emailer.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/rds.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/redshift.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/sagemaker.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/tags.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/tags.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/task_log_fetcher.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/task_log_fetcher.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/waiter.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/utils/waiter_with_logging.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/utils/waiter_with_logging.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/__init__.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/appflow.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/appflow.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/athena.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/athena.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/base_waiter.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/batch.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/batch.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/dynamodb.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/dynamodb.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/ecs.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/ecs.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/eks.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/eks.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/emr-containers.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/emr-containers.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/emr-serverless.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/emr-serverless.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/emr.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/emr.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/glue.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/glue.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/redshift.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/redshift.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/aws/waiters/sagemaker.json` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/aws/waiters/sagemaker.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/airflow/providers/amazon/get_provider_info.py` & `apache-airflow-providers-amazon-8.3.0rc3/airflow/providers/amazon/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -641,14 +641,18 @@
             {
                 "integration-name": "Amazon Appflow",
                 "python-modules": ["airflow.providers.amazon.aws.hooks.appflow"],
             },
         ],
         "triggers": [
             {
+                "integration-name": "Amazon Web Services",
+                "python-modules": ["airflow.providers.amazon.aws.triggers.base"],
+            },
+            {
                 "integration-name": "Amazon Athena",
                 "python-modules": ["airflow.providers.amazon.aws.triggers.athena"],
             },
             {
                 "integration-name": "AWS Batch",
                 "python-modules": ["airflow.providers.amazon.aws.triggers.batch"],
             },
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/apache_airflow_providers_amazon.egg-info/PKG-INFO` & `apache-airflow-providers-amazon-8.3.0rc3/apache_airflow_providers_amazon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.3.0rc2
+Version: 8.3.0rc3
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.0/
@@ -80,15 +80,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.3.0rc2``
+Release: ``8.3.0rc3``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/apache_airflow_providers_amazon.egg-info/SOURCES.txt` & `apache-airflow-providers-amazon-8.3.0rc3/apache_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 airflow/providers/amazon/aws/transfers/s3_to_sftp.py
 airflow/providers/amazon/aws/transfers/s3_to_sql.py
 airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
 airflow/providers/amazon/aws/transfers/sftp_to_s3.py
 airflow/providers/amazon/aws/transfers/sql_to_s3.py
 airflow/providers/amazon/aws/triggers/__init__.py
 airflow/providers/amazon/aws/triggers/athena.py
+airflow/providers/amazon/aws/triggers/base.py
 airflow/providers/amazon/aws/triggers/batch.py
 airflow/providers/amazon/aws/triggers/ec2.py
 airflow/providers/amazon/aws/triggers/ecs.py
 airflow/providers/amazon/aws/triggers/eks.py
 airflow/providers/amazon/aws/triggers/emr.py
 airflow/providers/amazon/aws/triggers/glue.py
 airflow/providers/amazon/aws/triggers/glue_crawler.py
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/apache_airflow_providers_amazon.egg-info/requires.txt` & `apache-airflow-providers-amazon-8.3.0rc3/apache_airflow_providers_amazon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/pyproject.toml` & `apache-airflow-providers-amazon-8.3.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/setup.cfg` & `apache-airflow-providers-amazon-8.3.0rc3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -66,10 +66,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.amazon.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.amazon
 
 [egg_info]
-tag_build = rc2
+tag_build = rc3
 tag_date = 0
```

### Comparing `apache-airflow-providers-amazon-8.3.0rc2/setup.py` & `apache-airflow-providers-amazon-8.3.0rc3/setup.py`

 * *Files identical despite different names*

