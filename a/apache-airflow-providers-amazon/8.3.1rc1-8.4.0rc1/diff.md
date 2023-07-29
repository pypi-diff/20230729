# Comparing `tmp/apache-airflow-providers-amazon-8.3.1rc1.tar.gz` & `tmp/apache-airflow-providers-amazon-8.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-amazon-8.3.1rc1.tar", last modified: Wed Jul 12 19:13:17 2023, max compression
+gzip compressed data, was "apache-airflow-providers-amazon-8.4.0rc1.tar", last modified: Sat Jul 29 12:07:48 2023, max compression
```

## Comparing `apache-airflow-providers-amazon-8.3.1rc1.tar` & `apache-airflow-providers-amazon-8.4.0rc1.tar`

### file list

```diff
@@ -1,195 +1,199 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.707884 apache-airflow-providers-amazon-8.3.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.3.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1219 2023-07-12 19:13:15.000000 apache-airflow-providers-amazon-8.3.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.3.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8022 2023-07-12 19:13:17.708447 apache-airflow-providers-amazon-8.3.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6037 2023-07-12 19:13:15.000000 apache-airflow-providers-amazon-8.3.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.125784 apache-airflow-providers-amazon-8.3.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.126911 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.182164 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-07-12 19:08:31.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.188540 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.325764 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/appflow.py
--rw-r--r--   0 root         (0) root         (0)    12358 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/athena.py
--rw-r--r--   0 root         (0) root         (0)    46780 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    21319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
--rw-r--r--   0 root         (0) root         (0)    10541 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-r--r--   0 root         (0) root         (0)     4263 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/chime.py
--rw-r--r--   0 root         (0) root         (0)     3378 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    14079 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/datasync.py
--rw-r--r--   0 root         (0) root         (0)     7907 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/dms.py
--rw-r--r--   0 root         (0) root         (0)     2670 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     7928 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ec2.py
--rw-r--r--   0 root         (0) root         (0)     3703 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ecr.py
--rw-r--r--   0 root         (0) root         (0)     6610 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ecs.py
--rw-r--r--   0 root         (0) root         (0)    23958 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/eks.py
--rw-r--r--   0 root         (0) root         (0)    12119 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-r--r--   0 root         (0) root         (0)    20429 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 root         (0) root         (0)     3452 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glacier.py
--rw-r--r--   0 root         (0) root         (0)    16313 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glue.py
--rw-r--r--   0 root         (0) root         (0)     7616 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-r--r--   0 root         (0) root         (0)     7931 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-r--r--   0 root         (0) root         (0)     8095 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     5883 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/logs.py
--rw-r--r--   0 root         (0) root         (0)     7094 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    15479 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/rds.py
--rw-r--r--   0 root         (0) root         (0)    13169 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7722 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     7160 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    58255 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/s3.py
--rw-r--r--   0 root         (0) root         (0)    56365 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2667 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     4146 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ses.py
--rw-r--r--   0 root         (0) root         (0)     3463 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sns.py
--rw-r--r--   0 root         (0) root         (0)     3121 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ssm.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/step_function.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.342697 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/base_aws.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/batch.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/emr.py
--rw-r--r--   0 root         (0) root         (0)     1229 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/glue.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.351106 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-r--r--   0 root         (0) root         (0)     9600 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.356727 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/notifications/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/notifications/chime.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.428699 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19662 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0 root         (0) root         (0)    20436 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    18421 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0 root         (0) root         (0)    10720 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0 root         (0) root         (0)     9591 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0 root         (0) root         (0)    33315 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0 root         (0) root         (0)    43203 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/eks.py
--rw-r--r--   0 root         (0) root         (0)    65010 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0 root         (0) root         (0)     9663 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     7749 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3968 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    35538 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0 root         (0) root         (0)    32304 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5547 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)    30235 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0 root         (0) root         (0)    58086 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0 root         (0) root         (0)     4583 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.437271 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15625 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     8495 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.503549 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0 root         (0) root         (0)     9160 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 root         (0) root         (0)     4150 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)     3984 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     3721 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0 root         (0) root         (0)     7063 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9772 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0 root         (0) root         (0)    22909 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 root         (0) root         (0)     4115 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0 root         (0) root         (0)     3319 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0 root         (0) root         (0)     3719 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3027 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3626 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0 root         (0) root         (0)     6434 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)    15066 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0 root         (0) root         (0)    12794 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     9543 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0 root         (0) root         (0)     3333 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.562416 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7019 2023-07-04 06:09:02.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0 root         (0) root         (0)     7755 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6368 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8544 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4702 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4173 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     5981 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0 root         (0) root         (0)     8531 2023-07-12 12:42:21.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0 root         (0) root         (0)     4634 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     3643 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8865 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.602264 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2427 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/athena.py
--rw-r--r--   0 root         (0) root         (0)     5403 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/base.py
--rw-r--r--   0 root         (0) root         (0)    10706 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/batch.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/ec2.py
--rw-r--r--   0 root         (0) root         (0)     8898 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/ecs.py
--rw-r--r--   0 root         (0) root         (0)     8445 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/eks.py
--rw-r--r--   0 root         (0) root         (0)    11320 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/emr.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/glue.py
--rw-r--r--   0 root         (0) root         (0)     2622 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3880 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/rds.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     9085 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/s3.py
--rw-r--r--   0 root         (0) root         (0)     4626 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/sagemaker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.643330 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     2265 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20649 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/emailer.py
--rw-r--r--   0 root         (0) root         (0)      973 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/rds.py
--rw-r--r--   0 root         (0) root         (0)     1897 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/redshift.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     4491 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py
--rw-r--r--   0 root         (0) root         (0)     3509 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/waiter.py
--rw-r--r--   0 root         (0) root         (0)     5890 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.682364 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/appflow.json
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-24 10:23:43.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/athena.json
--rw-r--r--   0 root         (0) root         (0)     1853 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/batch.json
--rw-r--r--   0 root         (0) root         (0)      895 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/dynamodb.json
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/ecs.json
--rw-r--r--   0 root         (0) root         (0)      659 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/eks.json
--rw-r--r--   0 root         (0) root         (0)      851 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/emr-containers.json
--rw-r--r--   0 root         (0) root         (0)     4893 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json
--rw-r--r--   0 root         (0) root         (0)     4242 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/emr.json
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/glue.json
--rw-r--r--   0 root         (0) root         (0)     1742 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/redshift.json
--rw-r--r--   0 root         (0) root         (0)     3625 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/sagemaker.json
--rw-r--r--   0 root         (0) root         (0)    40358 2023-07-12 19:13:15.000000 apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:17.705666 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8022 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8503 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      949 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:17.000000 apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.3.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2243 2023-07-12 19:13:17.710325 apache-airflow-providers-amazon-8.3.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2502 2023-07-12 19:13:15.000000 apache-airflow-providers-amazon-8.3.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.319975 apache-airflow-providers-amazon-8.4.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.4.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-07-29 12:07:45.000000 apache-airflow-providers-amazon-8.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.4.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8040 2023-07-29 12:07:48.320623 apache-airflow-providers-amazon-8.4.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6055 2023-07-29 12:07:45.000000 apache-airflow-providers-amazon-8.4.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.708955 apache-airflow-providers-amazon-8.4.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.710281 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.769495 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.776381 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.916933 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 root         (0) root         (0)    12358 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 root         (0) root         (0)    47454 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    21319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
+-rw-r--r--   0 root         (0) root         (0)    10541 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     4263 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/chime.py
+-rw-r--r--   0 root         (0) root         (0)     3378 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    14079 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 root         (0) root         (0)     7907 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     7928 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 root         (0) root         (0)     6610 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    23958 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 root         (0) root         (0)    12119 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 root         (0) root         (0)    20679 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/eventbridge.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 root         (0) root         (0)    16313 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 root         (0) root         (0)     7616 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 root         (0) root         (0)     7931 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     8095 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    15479 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 root         (0) root         (0)    13169 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     8342 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     7160 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    58255 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 root         (0) root         (0)    56469 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.936293 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.944820 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9600 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.950487 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/notifications/chime.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.029836 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19662 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 root         (0) root         (0)    20436 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    18421 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 root         (0) root         (0)    10720 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 root         (0) root         (0)     9591 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 root         (0) root         (0)    33315 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    50133 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 root         (0) root         (0)    74988 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/eventbridge.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     9663 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     7749 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    38326 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 root         (0) root         (0)    32304 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)    30235 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 root         (0) root         (0)    61246 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     6411 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.038514 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15625 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8495 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.106360 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 root         (0) root         (0)     9160 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)     3984 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     3721 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9772 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 root         (0) root         (0)    22909 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3719 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3626 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    15066 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 root         (0) root         (0)    12794 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     9543 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.171760 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7019 2023-07-04 06:09:02.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6368 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8544 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4702 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4173 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     5981 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     8550 2023-07-16 17:25:26.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4634 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     3643 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8865 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.217435 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/athena.py
+-rw-r--r--   0 root         (0) root         (0)     5403 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/base.py
+-rw-r--r--   0 root         (0) root         (0)    10713 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     9049 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    16050 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/eks.py
+-rw-r--r--   0 root         (0) root         (0)    19426 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/emr.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/glue.py
+-rw-r--r--   0 root         (0) root         (0)     2622 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)    10046 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/rds.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     9085 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/s3.py
+-rw-r--r--   0 root         (0) root         (0)     7906 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.249327 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     2968 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20649 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     4491 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     3509 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/waiter.py
+-rw-r--r--   0 root         (0) root         (0)     5890 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.293269 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/appflow.json
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-24 10:23:43.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/athena.json
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/batch.json
+-rw-r--r--   0 root         (0) root         (0)      895 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/ecs.json
+-rw-r--r--   0 root         (0) root         (0)      659 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/eks.json
+-rw-r--r--   0 root         (0) root         (0)      851 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/emr-containers.json
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/emr.json
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/glue.json
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/redshift.json
+-rw-r--r--   0 root         (0) root         (0)     5254 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/stepfunctions.json
+-rw-r--r--   0 root         (0) root         (0)    41325 2023-07-29 12:07:45.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.317181 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8040 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8718 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-amazon-8.4.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-07-29 12:07:48.322543 apache-airflow-providers-amazon-8.4.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-07-29 12:07:45.000000 apache-airflow-providers-amazon-8.4.0rc1/setup.py
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/LICENSE` & `apache-airflow-providers-amazon-8.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/MANIFEST.in` & `apache-airflow-providers-amazon-8.4.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/PKG-INFO` & `apache-airflow-providers-amazon-8.4.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.3.1rc1
+Version: 8.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -80,60 +80,60 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.3.1rc1``
+Release: ``8.4.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-amazon``
 
 The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
-=======================================  ==================
+=======================================  =====================
 PIP package                              Version required
-=======================================  ==================
+=======================================  =====================
 ``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``apache-airflow-providers-http``
 ``boto3``                                ``>=1.24.0``
 ``asgiref``
 ``watchtower``                           ``~=2.0.1``
 ``jsonpath_ng``                          ``>=1.5.3``
 ``redshift_connector``                   ``>=2.0.888``
 ``sqlalchemy_redshift``                  ``>=0.8.6``
 ``mypy-boto3-rds``                       ``>=1.24.0``
 ``mypy-boto3-redshift-data``             ``>=1.24.0``
-``mypy-boto3-appflow``                   ``>=1.24.0``
+``mypy-boto3-appflow``                   ``>=1.24.0,<1.28.12``
 ``asgiref``
 ``mypy-boto3-s3``                        ``>=1.24.0``
-=======================================  ==================
+=======================================  =====================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
 
@@ -158,8 +158,8 @@
 `apache-airflow-providers-microsoft-azure <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure>`_  ``microsoft.azure``
 `apache-airflow-providers-mongo <https://airflow.apache.org/docs/apache-airflow-providers-mongo>`_                      ``mongo``
 `apache-airflow-providers-salesforce <https://airflow.apache.org/docs/apache-airflow-providers-salesforce>`_            ``salesforce``
 `apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                          ``ssh``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/README.rst` & `apache-airflow-providers-amazon-8.4.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,60 +32,60 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.3.1rc1``
+Release: ``8.4.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-amazon``
 
 The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
-=======================================  ==================
+=======================================  =====================
 PIP package                              Version required
-=======================================  ==================
+=======================================  =====================
 ``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``apache-airflow-providers-http``
 ``boto3``                                ``>=1.24.0``
 ``asgiref``
 ``watchtower``                           ``~=2.0.1``
 ``jsonpath_ng``                          ``>=1.5.3``
 ``redshift_connector``                   ``>=2.0.888``
 ``sqlalchemy_redshift``                  ``>=0.8.6``
 ``mypy-boto3-rds``                       ``>=1.24.0``
 ``mypy-boto3-redshift-data``             ``>=1.24.0``
-``mypy-boto3-appflow``                   ``>=1.24.0``
+``mypy-boto3-appflow``                   ``>=1.24.0,<1.28.12``
 ``asgiref``
 ``mypy-boto3-s3``                        ``>=1.24.0``
-=======================================  ==================
+=======================================  =====================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
 
@@ -110,8 +110,8 @@
 `apache-airflow-providers-microsoft-azure <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure>`_  ``microsoft.azure``
 `apache-airflow-providers-mongo <https://airflow.apache.org/docs/apache-airflow-providers-mongo>`_                      ``mongo``
 `apache-airflow-providers-salesforce <https://airflow.apache.org/docs/apache-airflow-providers-salesforce>`_            ``salesforce``
 `apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                          ``ssh``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/__init__.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "8.3.1"
+__version__ = "8.4.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-amazon:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/__init__.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/exceptions.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/__init__.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/appflow.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/athena.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/base_aws.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,30 +193,43 @@
 
     def _create_basic_session(self, session_kwargs: dict[str, Any]) -> boto3.session.Session:
         return boto3.session.Session(**session_kwargs)
 
     def _create_session_with_assume_role(
         self, session_kwargs: dict[str, Any], deferrable: bool = False
     ) -> boto3.session.Session:
-
         if self.conn.assume_role_method == "assume_role_with_web_identity":
             # Deferred credentials have no initial credentials
             credential_fetcher = self._get_web_identity_credential_fetcher()
-            credentials = botocore.credentials.DeferredRefreshableCredentials(
-                method="assume-role-with-web-identity",
-                refresh_using=credential_fetcher.fetch_credentials,
-                time_fetcher=lambda: datetime.datetime.now(tz=tzlocal()),
-            )
+
+            params = {
+                "method": "assume-role-with-web-identity",
+                "refresh_using": credential_fetcher.fetch_credentials,
+                "time_fetcher": lambda: datetime.datetime.now(tz=tzlocal()),
+            }
+
+            if deferrable:
+                from aiobotocore.credentials import AioDeferredRefreshableCredentials
+
+                credentials = AioDeferredRefreshableCredentials(**params)
+            else:
+                credentials = botocore.credentials.DeferredRefreshableCredentials(**params)
         else:
             # Refreshable credentials do have initial credentials
-            credentials = botocore.credentials.RefreshableCredentials.create_from_metadata(
-                metadata=self._refresh_credentials(),
-                refresh_using=self._refresh_credentials,
-                method="sts-assume-role",
-            )
+            params = {
+                "metadata": self._refresh_credentials(),
+                "refresh_using": self._refresh_credentials,
+                "method": "sts-assume-role",
+            }
+            if deferrable:
+                from aiobotocore.credentials import AioRefreshableCredentials
+
+                credentials = AioRefreshableCredentials.create_from_metadata(**params)
+            else:
+                credentials = botocore.credentials.RefreshableCredentials.create_from_metadata(**params)
 
         if deferrable:
             from aiobotocore.session import get_session as async_get_session
 
             session = async_get_session()
         else:
             session = botocore.session.get_session()
@@ -792,15 +805,19 @@
         """Test the AWS connection by call AWS STS (Security Token Service) GetCallerIdentity API.
 
         .. seealso::
             https://docs.aws.amazon.com/STS/latest/APIReference/API_GetCallerIdentity.html
         """
         try:
             session = self.get_session()
-            conn_info = session.client("sts").get_caller_identity()
+            test_endpoint_url = self.conn_config.extra_config.get("test_endpoint_url")
+            conn_info = session.client(
+                "sts",
+                endpoint_url=test_endpoint_url,
+            ).get_caller_identity()
             metadata = conn_info.pop("ResponseMetadata", {})
             if metadata.get("HTTPStatusCode") != 200:
                 try:
                     return False, json.dumps(metadata)
                 except TypeError:
                     return False, str(metadata)
             conn_info["credentials_method"] = session.get_credentials().method
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/batch_client.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/chime.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/chime.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/datasync.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/dms.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/dynamodb.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ec2.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ecr.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ecs.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/eks.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/emr.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,17 +252,22 @@
     APPLICATION_FAILURE_STATES = {"STOPPED", "TERMINATED"}
     APPLICATION_SUCCESS_STATES = {"CREATED", "STARTED"}
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         kwargs["client_type"] = "emr-serverless"
         super().__init__(*args, **kwargs)
 
-    def cancel_running_jobs(self, application_id: str, waiter_config: dict = {}):
+    def cancel_running_jobs(
+        self, application_id: str, waiter_config: dict | None = None, wait_for_completion: bool = True
+    ) -> int:
         """
-        List all jobs in an intermediate state, cancel them, then wait for those jobs to reach terminal state.
+        Cancel jobs in an intermediate state, and return the number of cancelled jobs.
+
+        If wait_for_completion is True, then the method will wait until all jobs are
+        cancelled before returning.
 
         Note: if new jobs are triggered while this operation is ongoing,
         it's going to time out and return an error.
         """
         paginator = self.conn.get_paginator("list_job_runs")
         results_per_response = 50
         iterator = paginator.paginate(
@@ -280,21 +285,24 @@
                 self.log.info(
                     "Cancelling %s pending job(s) for the application %s so that it can be stopped",
                     len(job_ids),
                     application_id,
                 )
                 for job_id in job_ids:
                     self.conn.cancel_job_run(applicationId=application_id, jobRunId=job_id)
-        if count > 0:
-            self.log.info("now waiting for the %s cancelled job(s) to terminate", count)
-            self.get_waiter("no_job_running").wait(
-                applicationId=application_id,
-                states=list(self.JOB_INTERMEDIATE_STATES.union({"CANCELLING"})),
-                WaiterConfig=waiter_config,
-            )
+        if wait_for_completion:
+            if count > 0:
+                self.log.info("now waiting for the %s cancelled job(s) to terminate", count)
+                self.get_waiter("no_job_running").wait(
+                    applicationId=application_id,
+                    states=list(self.JOB_INTERMEDIATE_STATES.union({"CANCELLING"})),
+                    WaiterConfig=waiter_config or {},
+                )
+
+        return count
 
 
 class EmrContainerHook(AwsBaseHook):
     """
     Interact with Amazon EMR Containers (Amazon EMR on EKS).
 
     Provide thick wrapper around :py:class:`boto3.client("emr-containers") <EMRContainers.Client>`.
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glacier.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glue.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/kinesis.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/lambda_function.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/logs.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/quicksight.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/rds.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/redshift_data.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,49 +56,57 @@
         db_user: str | None = None,
         parameters: Iterable | None = None,
         secret_arn: str | None = None,
         statement_name: str | None = None,
         with_event: bool = False,
         wait_for_completion: bool = True,
         poll_interval: int = 10,
+        workgroup_name: str | None = None,
     ) -> str:
         """
         Execute a statement against Amazon Redshift.
 
         :param database: the name of the database
         :param sql: the SQL statement or list of  SQL statement to run
         :param cluster_identifier: unique identifier of a cluster
         :param db_user: the database username
         :param parameters: the parameters for the SQL statement
         :param secret_arn: the name or ARN of the secret that enables db access
         :param statement_name: the name of the SQL statement
         :param with_event: indicates whether to send an event to EventBridge
         :param wait_for_completion: indicates whether to wait for a result, if True wait, if False don't wait
         :param poll_interval: how often in seconds to check the query status
+        :param workgroup_name: name of the Redshift Serverless workgroup. Mutually exclusive with
+            `cluster_identifier`. Specify this parameter to query Redshift Serverless. More info
+            https://docs.aws.amazon.com/redshift/latest/mgmt/working-with-serverless.html
 
         :returns statement_id: str, the UUID of the statement
         """
         kwargs: dict[str, Any] = {
             "ClusterIdentifier": cluster_identifier,
             "Database": database,
             "DbUser": db_user,
             "Parameters": parameters,
             "WithEvent": with_event,
             "SecretArn": secret_arn,
             "StatementName": statement_name,
+            "WorkgroupName": workgroup_name,
         }
         if isinstance(sql, list):
             kwargs["Sqls"] = sql
             resp = self.conn.batch_execute_statement(**trim_none_values(kwargs))
         else:
             kwargs["Sql"] = sql
             resp = self.conn.execute_statement(**trim_none_values(kwargs))
 
         statement_id = resp["Id"]
 
+        if bool(cluster_identifier) is bool(workgroup_name):
+            raise ValueError("Either 'cluster_identifier' or 'workgroup_name' must be specified.")
+
         if wait_for_completion:
             self.wait_for_results(statement_id, poll_interval=poll_interval)
 
         return statement_id
 
     def wait_for_results(self, statement_id, poll_interval):
         while True:
@@ -123,14 +131,15 @@
 
     def get_table_primary_key(
         self,
         table: str,
         database: str,
         schema: str | None = "public",
         cluster_identifier: str | None = None,
+        workgroup_name: str | None = None,
         db_user: str | None = None,
         secret_arn: str | None = None,
         statement_name: str | None = None,
         with_event: bool = False,
         wait_for_completion: bool = True,
         poll_interval: int = 10,
     ) -> list[str] | None:
@@ -164,14 +173,15 @@
             and kcu.table_schema = {schema}
             and kcu.table_name = {table}
         """
         stmt_id = self.execute_query(
             sql=sql,
             database=database,
             cluster_identifier=cluster_identifier,
+            workgroup_name=workgroup_name,
             db_user=db_user,
             secret_arn=secret_arn,
             statement_name=statement_name,
             with_event=with_event,
             wait_for_completion=wait_for_completion,
             poll_interval=poll_interval,
         )
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sagemaker.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,23 @@
 
 import collections
 import os
 import re
 import tarfile
 import tempfile
 import time
+import warnings
 from collections import Counter
 from datetime import datetime
 from functools import partial
 from typing import Any, Callable, Generator, cast
 
 from botocore.exceptions import ClientError
 
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.providers.amazon.aws.hooks.logs import AwsLogsHook
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.amazon.aws.utils.tags import format_tags
 from airflow.utils import timezone
 
 
@@ -1057,34 +1058,39 @@
 
     def start_pipeline(
         self,
         pipeline_name: str,
         display_name: str = "airflow-triggered-execution",
         pipeline_params: dict | None = None,
         wait_for_completion: bool = False,
-        check_interval: int = 30,
+        check_interval: int | None = None,
         verbose: bool = True,
     ) -> str:
         """Start a new execution for a SageMaker pipeline.
 
         .. seealso::
             - :external+boto3:py:meth:`SageMaker.Client.start_pipeline_execution`
 
         :param pipeline_name: Name of the pipeline to start (this is _not_ the ARN).
         :param display_name: The name this pipeline execution will have in the UI. Doesn't need to be unique.
         :param pipeline_params: Optional parameters for the pipeline.
             All parameters supplied need to already be present in the pipeline definition.
-        :param wait_for_completion: Will only return once the pipeline is complete if true.
-        :param check_interval: How long to wait between checks for pipeline status when waiting for
-            completion.
-        :param verbose: Whether to print steps details when waiting for completion.
-            Defaults to true, consider turning off for pipelines that have thousands of steps.
 
         :return: the ARN of the pipeline execution launched.
         """
+        if wait_for_completion or check_interval is not None:
+            warnings.warn(
+                "parameter `wait_for_completion` and `check_interval` are deprecated, "
+                "remove them and call check_status yourself if you want to wait for completion",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+        if check_interval is None:
+            check_interval = 30
+
         formatted_params = format_tags(pipeline_params, key_label="Name")
 
         try:
             res = self.conn.start_pipeline_execution(
                 PipelineName=pipeline_name,
                 PipelineExecutionDisplayName=display_name,
                 PipelineParameters=formatted_params,
@@ -1104,39 +1110,43 @@
             )
         return arn
 
     def stop_pipeline(
         self,
         pipeline_exec_arn: str,
         wait_for_completion: bool = False,
-        check_interval: int = 10,
+        check_interval: int | None = None,
         verbose: bool = True,
         fail_if_not_running: bool = False,
     ) -> str:
         """Stop SageMaker pipeline execution.
 
         .. seealso::
             - :external+boto3:py:meth:`SageMaker.Client.stop_pipeline_execution`
 
         :param pipeline_exec_arn: Amazon Resource Name (ARN) of the pipeline execution.
             It's the ARN of the pipeline itself followed by "/execution/" and an id.
-        :param wait_for_completion: Whether to wait for the pipeline to reach a final state.
-            (i.e. either 'Stopped' or 'Failed')
-        :param check_interval: How long to wait between checks for pipeline status when waiting for
-            completion.
-        :param verbose: Whether to print steps details when waiting for completion.
-            Defaults to true, consider turning off for pipelines that have thousands of steps.
         :param fail_if_not_running: This method will raise an exception if the pipeline we're trying to stop
             is not in an "Executing" state when the call is sent (which would mean that the pipeline is
             already either stopping or stopped).
             Note that setting this to True will raise an error if the pipeline finished successfully before it
             was stopped.
         :return: Status of the pipeline execution after the operation.
             One of 'Executing'|'Stopping'|'Stopped'|'Failed'|'Succeeded'.
         """
+        if wait_for_completion or check_interval is not None:
+            warnings.warn(
+                "parameter `wait_for_completion` and `check_interval` are deprecated, "
+                "remove them and call check_status yourself if you want to wait for completion",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+        if check_interval is None:
+            check_interval = 10
+
         retries = 2  # i.e. 3 calls max, 1 initial + 2 retries
         while True:
             try:
                 self.conn.stop_pipeline_execution(PipelineExecutionArn=pipeline_exec_arn)
                 break
             except ClientError as ce:
                 # this can happen if the pipeline was transitioning between steps at that moment
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ses.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sns.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sqs.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/ssm.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/step_function.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/hooks/sts.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/__init__.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/base_aws.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/batch.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/emr.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/glue.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/links/logs.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/__init__.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/log/s3_task_handler.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/notifications/__init__.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/notifications/chime.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/notifications/chime.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,13 +49,13 @@
         self.message = message
 
     @cached_property
     def hook(self):
         """To reduce overhead cache the hook for the notifier."""
         return ChimeWebhookHook(chime_conn_id=self.chime_conn_id)
 
-    def notify(self, context: Context) -> None:
+    def notify(self, context: Context) -> None:  # type: ignore[override]
         """Send a message to a Chime Chat Room."""
         self.hook.send_message(message=self.message)
 
 
 send_chime_notification = ChimeNotifier
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/__init__.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/appflow.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/athena.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/batch.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/cloud_formation.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/datasync.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/dms.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/ec2.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/ecs.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/eks.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/eks.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 """This module contains Amazon EKS operators."""
 from __future__ import annotations
 
 import logging
 import warnings
 from ast import literal_eval
 from datetime import timedelta
-from typing import TYPE_CHECKING, List, Sequence, cast
+from typing import TYPE_CHECKING, Any, List, Sequence, cast
 
 from botocore.exceptions import ClientError, WaiterError
 
 from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.eks import EksHook
 from airflow.providers.amazon.aws.triggers.eks import (
+    EksCreateClusterTrigger,
     EksCreateFargateProfileTrigger,
     EksCreateNodegroupTrigger,
+    EksDeleteClusterTrigger,
     EksDeleteFargateProfileTrigger,
     EksDeleteNodegroupTrigger,
 )
 from airflow.providers.amazon.aws.utils.waiter_with_logging import wait
 from airflow.providers.cncf.kubernetes.utils.pod_manager import OnFinishAction
 
 try:
@@ -183,14 +185,17 @@
     :param fargate_pod_execution_role_arn: *REQUIRED* The Amazon Resource Name (ARN) of the pod execution
          role to use for pods that match the selectors in the AWS Fargate profile. (templated)
     :param fargate_selectors: The selectors to match for pods to use this AWS Fargate profile. (templated)
     :param create_fargate_profile_kwargs: Optional parameters to pass to the CreateFargateProfile API
          (templated)
     :param waiter_delay: Time (in seconds) to wait between two consecutive calls to check cluster state
     :param waiter_max_attempts: The maximum number of attempts to check cluster state
+    :param deferrable: If True, the operator will wait asynchronously for the job to complete.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False)
 
     """
 
     template_fields: Sequence[str] = (
         "cluster_name",
         "cluster_role_arn",
         "resources_vpc_config",
@@ -221,35 +226,37 @@
         fargate_profile_name: str = DEFAULT_FARGATE_PROFILE_NAME,
         fargate_pod_execution_role_arn: str | None = None,
         fargate_selectors: list | None = None,
         create_fargate_profile_kwargs: dict | None = None,
         wait_for_completion: bool = False,
         aws_conn_id: str = DEFAULT_CONN_ID,
         region: str | None = None,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         waiter_delay: int = 30,
         waiter_max_attempts: int = 40,
         **kwargs,
     ) -> None:
         self.compute = compute
         self.cluster_name = cluster_name
         self.cluster_role_arn = cluster_role_arn
         self.resources_vpc_config = resources_vpc_config
         self.create_cluster_kwargs = create_cluster_kwargs or {}
         self.nodegroup_role_arn = nodegroup_role_arn
         self.fargate_pod_execution_role_arn = fargate_pod_execution_role_arn
         self.create_fargate_profile_kwargs = create_fargate_profile_kwargs or {}
-        self.wait_for_completion = wait_for_completion
+        self.wait_for_completion = False if deferrable else wait_for_completion
         self.waiter_delay = waiter_delay
         self.waiter_max_attempts = waiter_max_attempts
         self.aws_conn_id = aws_conn_id
         self.region = region
         self.nodegroup_name = nodegroup_name
         self.create_nodegroup_kwargs = create_nodegroup_kwargs or {}
         self.fargate_selectors = fargate_selectors or [{"namespace": DEFAULT_NAMESPACE_NAME}]
         self.fargate_profile_name = fargate_profile_name
+        self.deferrable = deferrable
         super().__init__(
             **kwargs,
         )
 
     def execute(self, context: Context):
         if self.compute:
             if self.compute not in SUPPORTED_COMPUTE_VALUES:
@@ -270,20 +277,33 @@
             roleArn=self.cluster_role_arn,
             resourcesVpcConfig=self.resources_vpc_config,
             **self.create_cluster_kwargs,
         )
 
         # Short circuit early if we don't need to wait to attach compute
         # and the caller hasn't requested to wait for the cluster either.
-        if not self.compute and not self.wait_for_completion:
+        if not any([self.compute, self.wait_for_completion, self.deferrable]):
             return None
 
-        self.log.info("Waiting for EKS Cluster to provision.  This will take some time.")
+        self.log.info("Waiting for EKS Cluster to provision. This will take some time.")
         client = self.eks_hook.conn
 
+        if self.deferrable:
+            self.defer(
+                trigger=EksCreateClusterTrigger(
+                    cluster_name=self.cluster_name,
+                    aws_conn_id=self.aws_conn_id,
+                    region_name=self.region,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                ),
+                method_name="deferrable_create_cluster_next",
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+            )
+
         try:
             client.get_waiter("cluster_active").wait(
                 name=self.cluster_name,
                 WaiterConfig={"Delay": self.waiter_delay, "MaxAttempts": self.waiter_max_attempts},
             )
         except (ClientError, WaiterError) as e:
             self.log.error("Cluster failed to start and will be torn down.\n %s", e)
@@ -307,14 +327,97 @@
             fargate_profile_name=self.fargate_profile_name,
             fargate_pod_execution_role_arn=self.fargate_pod_execution_role_arn,
             fargate_selectors=self.fargate_selectors,
             create_fargate_profile_kwargs=self.create_fargate_profile_kwargs,
             subnets=cast(List[str], self.resources_vpc_config.get("subnetIds")),
         )
 
+    def deferrable_create_cluster_next(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        if event is None:
+            self.log.error("Trigger error: event is None")
+            raise AirflowException("Trigger error: event is None")
+        elif event["status"] == "failed":
+            self.log.error("Cluster failed to start and will be torn down.")
+            self.eks_hook.delete_cluster(name=self.cluster_name)
+            self.defer(
+                trigger=EksDeleteClusterTrigger(
+                    cluster_name=self.cluster_name,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                    region_name=self.region,
+                    force_delete_compute=False,
+                ),
+                method_name="execute_failed",
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+            )
+        elif event["status"] == "success":
+            self.log.info("Cluster is ready to provision compute.")
+            _create_compute(
+                compute=self.compute,
+                cluster_name=self.cluster_name,
+                aws_conn_id=self.aws_conn_id,
+                region=self.region,
+                wait_for_completion=self.wait_for_completion,
+                waiter_delay=self.waiter_delay,
+                waiter_max_attempts=self.waiter_max_attempts,
+                nodegroup_name=self.nodegroup_name,
+                nodegroup_role_arn=self.nodegroup_role_arn,
+                create_nodegroup_kwargs=self.create_nodegroup_kwargs,
+                fargate_profile_name=self.fargate_profile_name,
+                fargate_pod_execution_role_arn=self.fargate_pod_execution_role_arn,
+                fargate_selectors=self.fargate_selectors,
+                create_fargate_profile_kwargs=self.create_fargate_profile_kwargs,
+                subnets=cast(List[str], self.resources_vpc_config.get("subnetIds")),
+            )
+            if self.compute == "fargate":
+                self.defer(
+                    trigger=EksCreateFargateProfileTrigger(
+                        cluster_name=self.cluster_name,
+                        fargate_profile_name=self.fargate_profile_name,
+                        waiter_delay=self.waiter_delay,
+                        waiter_max_attempts=self.waiter_max_attempts,
+                        aws_conn_id=self.aws_conn_id,
+                        region=self.region,
+                    ),
+                    method_name="execute_complete",
+                    timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+                )
+            else:
+                self.defer(
+                    trigger=EksCreateNodegroupTrigger(
+                        nodegroup_name=self.nodegroup_name,
+                        cluster_name=self.cluster_name,
+                        aws_conn_id=self.aws_conn_id,
+                        region_name=self.region,
+                        waiter_delay=self.waiter_delay,
+                        waiter_max_attempts=self.waiter_max_attempts,
+                    ),
+                    method_name="execute_complete",
+                    timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+                )
+
+    def execute_failed(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        if event is None:
+            self.log.info("Trigger error: event is None")
+            raise AirflowException("Trigger error: event is None")
+        elif event["status"] == "delteted":
+            self.log.info("Cluster deleted")
+            raise event["exception"]
+
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        resource = "fargate profile" if self.compute == "fargate" else self.compute
+        if event is None:
+            self.log.info("Trigger error: event is None")
+            raise AirflowException("Trigger error: event is None")
+        elif event["status"] != "success":
+            raise AirflowException(f"Error creating {resource}: {event}")
+
+        self.log.info("%s created successfully", resource)
+
 
 class EksCreateNodegroupOperator(BaseOperator):
     """
     Creates an Amazon EKS managed node group for an existing Amazon EKS Cluster.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
@@ -560,14 +663,19 @@
     :param aws_conn_id: The Airflow connection used for AWS credentials. (templated)
          If this is None or empty then the default boto3 behaviour is used. If
          running Airflow in a distributed manner and aws_conn_id is None or
          empty, then the default boto3 configuration would be used (and must be
          maintained on each worker node).
     :param region: Which AWS region the connection should use. (templated)
         If this is None or empty then the default boto3 behaviour is used.
+    :param waiter_delay: Time (in seconds) to wait between two consecutive calls to check cluster state
+    :param waiter_max_attempts: The maximum number of attempts to check cluster state
+    :param deferrable: If True, the operator will wait asynchronously for the cluster to be deleted.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False)
 
     """
 
     template_fields: Sequence[str] = (
         "cluster_name",
         "force_delete_compute",
         "wait_for_completion",
@@ -578,30 +686,48 @@
     def __init__(
         self,
         cluster_name: str,
         force_delete_compute: bool = False,
         wait_for_completion: bool = False,
         aws_conn_id: str = DEFAULT_CONN_ID,
         region: str | None = None,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 40,
         **kwargs,
     ) -> None:
         self.cluster_name = cluster_name
         self.force_delete_compute = force_delete_compute
-        self.wait_for_completion = wait_for_completion
+        self.wait_for_completion = False if deferrable else wait_for_completion
         self.aws_conn_id = aws_conn_id
         self.region = region
+        self.deferrable = deferrable
+        self.waiter_delay = waiter_delay
+        self.waiter_max_attempts = waiter_max_attempts
         super().__init__(**kwargs)
 
     def execute(self, context: Context):
         eks_hook = EksHook(
             aws_conn_id=self.aws_conn_id,
             region_name=self.region,
         )
-
-        if self.force_delete_compute:
+        if self.deferrable:
+            self.defer(
+                trigger=EksDeleteClusterTrigger(
+                    cluster_name=self.cluster_name,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                    region_name=self.region,
+                    force_delete_compute=self.force_delete_compute,
+                ),
+                method_name="execute_complete",
+                timeout=timedelta(seconds=self.waiter_delay * self.waiter_max_attempts),
+            )
+        elif self.force_delete_compute:
             self.delete_any_nodegroups(eks_hook)
             self.delete_any_fargate_profiles(eks_hook)
 
         eks_hook.delete_cluster(name=self.cluster_name)
 
         if self.wait_for_completion:
             self.log.info("Waiting for cluster to delete.  This will take some time.")
@@ -641,14 +767,21 @@
                 # so each must be deleted sequentially
                 eks_hook.delete_fargate_profile(clusterName=self.cluster_name, fargateProfileName=profile)
                 eks_hook.conn.get_waiter("fargate_profile_deleted").wait(
                     clusterName=self.cluster_name, fargateProfileName=profile
                 )
         self.log.info(SUCCESS_MSG.format(compute=FARGATE_FULL_NAME))
 
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        if event is None:
+            self.log.error("Trigger error. Event is None")
+            raise AirflowException("Trigger error. Event is None")
+        elif event["status"] == "success":
+            self.log.info("Cluster deleted successfully.")
+
 
 class EksDeleteNodegroupOperator(BaseOperator):
     """
     Deletes an Amazon EKS managed node group from an Amazon EKS Cluster.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/emr.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/emr.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,20 @@
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.emr import EmrContainerHook, EmrHook, EmrServerlessHook
 from airflow.providers.amazon.aws.links.emr import EmrClusterLink, EmrLogsLink, get_log_uri
 from airflow.providers.amazon.aws.triggers.emr import (
     EmrAddStepsTrigger,
     EmrContainerTrigger,
     EmrCreateJobFlowTrigger,
+    EmrServerlessCancelJobsTrigger,
+    EmrServerlessCreateApplicationTrigger,
+    EmrServerlessDeleteApplicationTrigger,
+    EmrServerlessStartApplicationTrigger,
+    EmrServerlessStartJobTrigger,
+    EmrServerlessStopApplicationTrigger,
     EmrTerminateJobFlowTrigger,
 )
 from airflow.providers.amazon.aws.utils.waiter import waiter
 from airflow.providers.amazon.aws.utils.waiter_with_logging import wait
 from airflow.utils.helpers import exactly_one, prune_dict
 from airflow.utils.types import NOTSET, ArgNotSet
 
@@ -968,41 +974,45 @@
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:EmrServerlessCreateApplicationOperator`
 
     :param release_label: The EMR release version associated with the application.
     :param job_type: The type of application you want to start, such as Spark or Hive.
     :param wait_for_completion: If true, wait for the Application to start before returning. Default to True.
-        If set to False, ``waiter_countdown`` and ``waiter_check_interval_seconds`` will only be applied when
+        If set to False, ``waiter_max_attempts`` and ``waiter_delay`` will only be applied when
         waiting for the application to be in the ``CREATED`` state.
     :param client_request_token: The client idempotency token of the application to create.
       Its value must be unique for each request.
     :param config: Optional dictionary for arbitrary parameters to the boto API create_application call.
     :param aws_conn_id: AWS connection to use
     :param waiter_countdown: (deprecated) Total amount of time, in seconds, the operator will wait for
         the application to start. Defaults to 25 minutes.
     :param waiter_check_interval_seconds: (deprecated) Number of seconds between polling the state
         of the application. Defaults to 60 seconds.
     :waiter_max_attempts: Number of times the waiter should poll the application to check the state.
         If not set, the waiter will use its default value.
     :param waiter_delay: Number of seconds between polling the state of the application.
+    :param deferrable: If True, the operator will wait asynchronously for application to be created.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False, but can be overridden in config file by setting default_deferrable to True)
     """
 
     def __init__(
         self,
         release_label: str,
         job_type: str,
         client_request_token: str = "",
         config: dict | None = None,
         wait_for_completion: bool = True,
         aws_conn_id: str = "aws_default",
         waiter_countdown: int | ArgNotSet = NOTSET,
         waiter_check_interval_seconds: int | ArgNotSet = NOTSET,
         waiter_max_attempts: int | ArgNotSet = NOTSET,
         waiter_delay: int | ArgNotSet = NOTSET,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         if waiter_check_interval_seconds is NOTSET:
             waiter_delay = 60 if waiter_delay is NOTSET else waiter_delay
         else:
             waiter_delay = waiter_check_interval_seconds if waiter_delay is NOTSET else waiter_delay
             warnings.warn(
@@ -1026,14 +1036,15 @@
         self.release_label = release_label
         self.job_type = job_type
         self.wait_for_completion = wait_for_completion
         self.kwargs = kwargs
         self.config = config or {}
         self.waiter_max_attempts = int(waiter_max_attempts)  # type: ignore[arg-type]
         self.waiter_delay = int(waiter_delay)  # type: ignore[arg-type]
+        self.deferrable = deferrable
         super().__init__(**kwargs)
 
         self.client_request_token = client_request_token or str(uuid4())
 
     @cached_property
     def hook(self) -> EmrServerlessHook:
         """Create and return an EmrServerlessHook."""
@@ -1048,16 +1059,27 @@
         )
         application_id = response["applicationId"]
 
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"Application Creation failed: {response}")
 
         self.log.info("EMR serverless application created: %s", application_id)
-        waiter = self.hook.get_waiter("serverless_app_created")
+        if self.deferrable:
+            self.defer(
+                trigger=EmrServerlessCreateApplicationTrigger(
+                    application_id=application_id,
+                    aws_conn_id=self.aws_conn_id,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                ),
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+                method_name="start_application_deferred",
+            )
 
+        waiter = self.hook.get_waiter("serverless_app_created")
         wait(
             waiter=waiter,
             waiter_delay=self.waiter_delay,
             waiter_max_attempts=self.waiter_max_attempts,
             args={"applicationId": application_id},
             failure_message="Serverless Application creation failed",
             status_message="Serverless Application status is",
@@ -1075,14 +1097,40 @@
                 args={"applicationId": application_id},
                 failure_message="Serverless Application failed to start",
                 status_message="Serverless Application status is",
                 status_args=["application.state", "application.stateDetails"],
             )
         return application_id
 
+    def start_application_deferred(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        if event is None:
+            self.log.error("Trigger error: event is None")
+            raise AirflowException("Trigger error: event is None")
+        elif event["status"] != "success":
+            raise AirflowException(f"Application {event['application_id']} failed to create")
+        self.log.info("Starting application %s", event["application_id"])
+        self.hook.conn.start_application(applicationId=event["application_id"])
+        self.defer(
+            trigger=EmrServerlessStartApplicationTrigger(
+                application_id=event["application_id"],
+                aws_conn_id=self.aws_conn_id,
+                waiter_delay=self.waiter_delay,
+                waiter_max_attempts=self.waiter_max_attempts,
+            ),
+            timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+            method_name="execute_complete",
+        )
+
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        if event is None or event["status"] != "success":
+            raise AirflowException(f"Trigger error: Application failed to start, event is {event}")
+
+        self.log.info("Application %s started", event["application_id"])
+        return event["application_id"]
+
 
 class EmrServerlessStartJobOperator(BaseOperator):
     """
     Operator to start EMR Serverless job.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
@@ -1103,14 +1151,17 @@
     :param waiter_countdown: (deprecated) Total amount of time, in seconds, the operator will wait for
         the job finish. Defaults to 25 minutes.
     :param waiter_check_interval_seconds: (deprecated) Number of seconds between polling the state of the job.
         Defaults to 60 seconds.
     :waiter_max_attempts: Number of times the waiter should poll the application to check the state.
         If not set, the waiter will use its default value.
     :param waiter_delay: Number of seconds between polling the state of the job run.
+    :param deferrable: If True, the operator will wait asynchronously for the crawl to complete.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False, but can be overridden in config file by setting default_deferrable to True)
     """
 
     template_fields: Sequence[str] = (
         "application_id",
         "config",
         "execution_role_arn",
         "job_driver",
@@ -1133,14 +1184,15 @@
         wait_for_completion: bool = True,
         aws_conn_id: str = "aws_default",
         name: str | None = None,
         waiter_countdown: int | ArgNotSet = NOTSET,
         waiter_check_interval_seconds: int | ArgNotSet = NOTSET,
         waiter_max_attempts: int | ArgNotSet = NOTSET,
         waiter_delay: int | ArgNotSet = NOTSET,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         if waiter_check_interval_seconds is NOTSET:
             waiter_delay = 60 if waiter_delay is NOTSET else waiter_delay
         else:
             waiter_delay = waiter_check_interval_seconds if waiter_delay is NOTSET else waiter_delay
             warnings.warn(
@@ -1167,41 +1219,53 @@
         self.configuration_overrides = configuration_overrides
         self.wait_for_completion = wait_for_completion
         self.config = config or {}
         self.name = name or self.config.pop("name", f"emr_serverless_job_airflow_{uuid4()}")
         self.waiter_max_attempts = int(waiter_max_attempts)  # type: ignore[arg-type]
         self.waiter_delay = int(waiter_delay)  # type: ignore[arg-type]
         self.job_id: str | None = None
+        self.deferrable = deferrable
         super().__init__(**kwargs)
 
         self.client_request_token = client_request_token or str(uuid4())
 
     @cached_property
     def hook(self) -> EmrServerlessHook:
         """Create and return an EmrServerlessHook."""
         return EmrServerlessHook(aws_conn_id=self.aws_conn_id)
 
-    def execute(self, context: Context) -> str | None:
-        self.log.info("Starting job on Application: %s", self.application_id)
+    def execute(self, context: Context, event: dict[str, Any] | None = None) -> str | None:
 
         app_state = self.hook.conn.get_application(applicationId=self.application_id)["application"]["state"]
         if app_state not in EmrServerlessHook.APPLICATION_SUCCESS_STATES:
+            self.log.info("Application state is %s", app_state)
+            self.log.info("Starting application %s", self.application_id)
             self.hook.conn.start_application(applicationId=self.application_id)
             waiter = self.hook.get_waiter("serverless_app_started")
-
+            if self.deferrable:
+                self.defer(
+                    trigger=EmrServerlessStartApplicationTrigger(
+                        application_id=self.application_id,
+                        waiter_delay=self.waiter_delay,
+                        waiter_max_attempts=self.waiter_max_attempts,
+                        aws_conn_id=self.aws_conn_id,
+                    ),
+                    method_name="execute",
+                    timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+                )
             wait(
                 waiter=waiter,
                 waiter_max_attempts=self.waiter_max_attempts,
                 waiter_delay=self.waiter_delay,
                 args={"applicationId": self.application_id},
                 failure_message="Serverless Application failed to start",
                 status_message="Serverless Application status is",
                 status_args=["application.state", "application.stateDetails"],
             )
-
+        self.log.info("Starting job on Application: %s", self.application_id)
         response = self.hook.conn.start_job_run(
             clientToken=self.client_request_token,
             applicationId=self.application_id,
             executionRoleArn=self.execution_role_arn,
             jobDriver=self.job_driver,
             configurationOverrides=self.configuration_overrides,
             name=self.name,
@@ -1209,30 +1273,54 @@
         )
 
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"EMR serverless job failed to start: {response}")
 
         self.job_id = response["jobRunId"]
         self.log.info("EMR serverless job started: %s", self.job_id)
+        if self.deferrable:
+            self.defer(
+                trigger=EmrServerlessStartJobTrigger(
+                    application_id=self.application_id,
+                    job_id=self.job_id,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                ),
+                method_name="execute_complete",
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+            )
         if self.wait_for_completion:
             waiter = self.hook.get_waiter("serverless_job_completed")
             wait(
                 waiter=waiter,
                 waiter_max_attempts=self.waiter_max_attempts,
                 waiter_delay=self.waiter_delay,
                 args={"applicationId": self.application_id, "jobRunId": self.job_id},
                 failure_message="Serverless Job failed",
                 status_message="Serverless Job status is",
                 status_args=["jobRun.state", "jobRun.stateDetails"],
             )
 
         return self.job_id
 
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        if event is None:
+            self.log.error("Trigger error: event is None")
+            raise AirflowException("Trigger error: event is None")
+        elif event["status"] == "success":
+            self.log.info("Serverless job completed")
+            return event["job_id"]
+
     def on_kill(self) -> None:
-        """Cancel the submitted job run."""
+        """
+        Cancel the submitted job run.
+
+        Note: this method will not run in deferrable mode.
+        """
         if self.job_id:
             self.log.info("Stopping job run with jobId - %s", self.job_id)
             response = self.hook.conn.cancel_job_run(applicationId=self.application_id, jobRunId=self.job_id)
             http_status_code = (
                 response.get("ResponseMetadata", {}).get("HTTPStatusCode") if response else None
             )
             if http_status_code is None or http_status_code != 200:
@@ -1266,36 +1354,44 @@
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:EmrServerlessStopApplicationOperator`
 
     :param application_id: ID of the EMR Serverless application to stop.
     :param wait_for_completion: If true, wait for the Application to stop before returning. Default to True
     :param aws_conn_id: AWS connection to use
-    :param waiter_countdown: Total amount of time, in seconds, the operator will wait for
+    :param waiter_countdown: (deprecated) Total amount of time, in seconds, the operator will wait for
         the application be stopped. Defaults to 5 minutes.
-    :param waiter_check_interval_seconds: Number of seconds between polling the state of the application.
-        Defaults to 30 seconds.
+    :param waiter_check_interval_seconds: (deprecated) Number of seconds between polling the state of the
+        application. Defaults to 60 seconds.
     :param force_stop: If set to True, any job for that app that is not in a terminal state will be cancelled.
         Otherwise, trying to stop an app with running jobs will return an error.
         If you want to wait for the jobs to finish gracefully, use
         :class:`airflow.providers.amazon.aws.sensors.emr.EmrServerlessJobSensor`
+    :waiter_max_attempts: Number of times the waiter should poll the application to check the state.
+        Default is 25.
+    :param waiter_delay: Number of seconds between polling the state of the application.
+        Default is 60 seconds.
+    :param deferrable: If True, the operator will wait asynchronously for the application to stop.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False, but can be overridden in config file by setting default_deferrable to True)
     """
 
     template_fields: Sequence[str] = ("application_id",)
 
     def __init__(
         self,
         application_id: str,
         wait_for_completion: bool = True,
         aws_conn_id: str = "aws_default",
         waiter_countdown: int | ArgNotSet = NOTSET,
         waiter_check_interval_seconds: int | ArgNotSet = NOTSET,
         waiter_max_attempts: int | ArgNotSet = NOTSET,
         waiter_delay: int | ArgNotSet = NOTSET,
         force_stop: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         if waiter_check_interval_seconds is NOTSET:
             waiter_delay = 60 if waiter_delay is NOTSET else waiter_delay
         else:
             waiter_delay = waiter_check_interval_seconds if waiter_delay is NOTSET else waiter_delay
             warnings.warn(
@@ -1313,69 +1409,131 @@
             warnings.warn(
                 "The parameter waiter_countdown has been deprecated to standardize "
                 "naming conventions.  Please use waiter_max_attempts instead.  In the "
                 "future this will default to None and defer to the waiter's default value."
             )
         self.aws_conn_id = aws_conn_id
         self.application_id = application_id
-        self.wait_for_completion = wait_for_completion
+        self.wait_for_completion = False if deferrable else wait_for_completion
         self.waiter_max_attempts = int(waiter_max_attempts)  # type: ignore[arg-type]
         self.waiter_delay = int(waiter_delay)  # type: ignore[arg-type]
         self.force_stop = force_stop
+        self.deferrable = deferrable
         super().__init__(**kwargs)
 
     @cached_property
     def hook(self) -> EmrServerlessHook:
         """Create and return an EmrServerlessHook."""
         return EmrServerlessHook(aws_conn_id=self.aws_conn_id)
 
     def execute(self, context: Context) -> None:
         self.log.info("Stopping application: %s", self.application_id)
 
         if self.force_stop:
-            self.hook.cancel_running_jobs(
-                self.application_id,
-                waiter_config={
-                    "Delay": self.waiter_delay,
-                    "MaxAttempts": self.waiter_max_attempts,
-                },
-            )
+            count = self.hook.cancel_running_jobs(
+                application_id=self.application_id,
+                wait_for_completion=False,
+            )
+            if count > 0:
+                self.log.info("now waiting for the %s cancelled job(s) to terminate", count)
+                if self.deferrable:
+                    self.defer(
+                        trigger=EmrServerlessCancelJobsTrigger(
+                            application_id=self.application_id,
+                            aws_conn_id=self.aws_conn_id,
+                            waiter_delay=self.waiter_delay,
+                            waiter_max_attempts=self.waiter_max_attempts,
+                        ),
+                        timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+                        method_name="stop_application",
+                    )
+                self.hook.get_waiter("no_job_running").wait(
+                    applicationId=self.application_id,
+                    states=list(self.hook.JOB_INTERMEDIATE_STATES.union({"CANCELLING"})),
+                    WaiterConfig={
+                        "Delay": self.waiter_delay,
+                        "MaxAttempts": self.waiter_max_attempts,
+                    },
+                )
+            else:
+                self.log.info("no running jobs found with application ID %s", self.application_id)
 
         self.hook.conn.stop_application(applicationId=self.application_id)
-
+        if self.deferrable:
+            self.defer(
+                trigger=EmrServerlessStopApplicationTrigger(
+                    application_id=self.application_id,
+                    aws_conn_id=self.aws_conn_id,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                ),
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+                method_name="execute_complete",
+            )
         if self.wait_for_completion:
             waiter = self.hook.get_waiter("serverless_app_stopped")
             wait(
                 waiter=waiter,
                 waiter_max_attempts=self.waiter_max_attempts,
                 waiter_delay=self.waiter_delay,
                 args={"applicationId": self.application_id},
                 failure_message="Error stopping application",
                 status_message="Serverless Application status is",
                 status_args=["application.state", "application.stateDetails"],
             )
             self.log.info("EMR serverless application %s stopped successfully", self.application_id)
 
+    def stop_application(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        if event is None:
+            self.log.error("Trigger error: event is None")
+            raise AirflowException("Trigger error: event is None")
+        elif event["status"] == "success":
+            self.hook.conn.stop_application(applicationId=self.application_id)
+            self.defer(
+                trigger=EmrServerlessStopApplicationTrigger(
+                    application_id=self.application_id,
+                    aws_conn_id=self.aws_conn_id,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                ),
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+                method_name="execute_complete",
+            )
+
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        if event is None:
+            self.log.error("Trigger error: event is None")
+            raise AirflowException("Trigger error: event is None")
+        elif event["status"] == "success":
+            self.log.info("EMR serverless application %s stopped successfully", self.application_id)
+
 
 class EmrServerlessDeleteApplicationOperator(EmrServerlessStopApplicationOperator):
     """
     Operator to delete EMR Serverless application.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:EmrServerlessDeleteApplicationOperator`
 
     :param application_id: ID of the EMR Serverless application to delete.
     :param wait_for_completion: If true, wait for the Application to be deleted before returning.
         Defaults to True. Note that this operator will always wait for the application to be STOPPED first.
     :param aws_conn_id: AWS connection to use
-    :param waiter_countdown: Total amount of time, in seconds, the operator will wait for each step of first,
-        the application to be stopped, and then deleted. Defaults to 25 minutes.
-    :param waiter_check_interval_seconds: Number of seconds between polling the state of the application.
+    :param waiter_countdown: (deprecated) Total amount of time, in seconds, the operator will wait for each
+        step of first,the application to be stopped, and then deleted. Defaults to 25 minutes.
+    :param waiter_check_interval_seconds: (deprecated) Number of seconds between polling the state
+        of the application. Defaults to 60 seconds.
+    :waiter_max_attempts: Number of times the waiter should poll the application to check the state.
+        Defaults to 25.
+    :param waiter_delay: Number of seconds between polling the state of the application.
         Defaults to 60 seconds.
+    :param deferrable: If True, the operator will wait asynchronously for application to be deleted.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False, but can be overridden in config file by setting default_deferrable to True)
     :param force_stop: If set to True, any job for that app that is not in a terminal state will be cancelled.
         Otherwise, trying to delete an app with running jobs will return an error.
         If you want to wait for the jobs to finish gracefully, use
         :class:`airflow.providers.amazon.aws.sensors.emr.EmrServerlessJobSensor`
     """
 
     template_fields: Sequence[str] = ("application_id",)
@@ -1386,14 +1544,15 @@
         wait_for_completion: bool = True,
         aws_conn_id: str = "aws_default",
         waiter_countdown: int | ArgNotSet = NOTSET,
         waiter_check_interval_seconds: int | ArgNotSet = NOTSET,
         waiter_max_attempts: int | ArgNotSet = NOTSET,
         waiter_delay: int | ArgNotSet = NOTSET,
         force_stop: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         if waiter_check_interval_seconds is NOTSET:
             waiter_delay = 60 if waiter_delay is NOTSET else waiter_delay
         else:
             waiter_delay = waiter_check_interval_seconds if waiter_delay is NOTSET else waiter_delay
             warnings.warn(
@@ -1421,32 +1580,53 @@
             wait_for_completion=True,
             aws_conn_id=aws_conn_id,
             waiter_delay=waiter_delay,
             waiter_max_attempts=waiter_max_attempts,
             force_stop=force_stop,
             **kwargs,
         )
+        self.deferrable = deferrable
+        self.wait_for_delete_completion = False if deferrable else wait_for_completion
 
     def execute(self, context: Context) -> None:
         # super stops the app (or makes sure it's already stopped)
         super().execute(context)
 
         self.log.info("Now deleting application: %s", self.application_id)
         response = self.hook.conn.delete_application(applicationId=self.application_id)
 
         if response["ResponseMetadata"]["HTTPStatusCode"] != 200:
             raise AirflowException(f"Application deletion failed: {response}")
 
-        if self.wait_for_delete_completion:
+        if self.deferrable:
+            self.defer(
+                trigger=EmrServerlessDeleteApplicationTrigger(
+                    application_id=self.application_id,
+                    aws_conn_id=self.aws_conn_id,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                ),
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+                method_name="execute_complete",
+            )
+
+        elif self.wait_for_delete_completion:
             waiter = self.hook.get_waiter("serverless_app_terminated")
 
             wait(
                 waiter=waiter,
                 waiter_max_attempts=self.waiter_max_attempts,
                 waiter_delay=self.waiter_delay,
                 args={"applicationId": self.application_id},
                 failure_message="Error terminating application",
                 status_message="Serverless Application status is",
                 status_args=["application.state", "application.stateDetails"],
             )
 
         self.log.info("EMR serverless application deleted")
+
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        if event is None:
+            self.log.error("Trigger error: event is None")
+            raise AirflowException("Trigger error: event is None")
+        elif event["status"] == "success":
+            self.log.info("EMR serverless application %s deleted successfully", self.application_id)
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/glacier.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/glue.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/glue_crawler.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/lambda_function.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/quicksight.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/rds.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/rds.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import json
 import warnings
 from datetime import timedelta
-from typing import TYPE_CHECKING, Sequence
+from typing import TYPE_CHECKING, Any, Sequence
 
+from astroid.decorators import cachedproperty
 from mypy_boto3_rds.type_defs import TagTypeDef
 
 from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.rds import RdsHook
-from airflow.providers.amazon.aws.triggers.rds import RdsDbInstanceTrigger
+from airflow.providers.amazon.aws.triggers.rds import (
+    RdsDbAvailableTrigger,
+    RdsDbDeletedTrigger,
+    RdsDbStoppedTrigger,
+)
 from airflow.providers.amazon.aws.utils.rds import RdsDbType
 from airflow.providers.amazon.aws.utils.tags import format_tags
 from airflow.providers.amazon.aws.utils.waiter_with_logging import wait
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -58,21 +63,25 @@
                 "You can use the region_name parameter to specify the region. "
                 "If you were using hook_params for other purposes, please get in touch either on "
                 "airflow slack, or by opening a github issue on the project. "
                 "You can mention https://github.com/apache/airflow/pull/32352",
                 AirflowProviderDeprecationWarning,
                 stacklevel=3,  # 2 is in the operator's init, 3 is in the user code creating the operator
             )
-        hook_params = hook_params or {}
-        self.region_name = region_name or hook_params.pop("region_name", None)
-        self.hook = RdsHook(aws_conn_id=aws_conn_id, region_name=self.region_name, **(hook_params))
+        self.hook_params = hook_params or {}
+        self.aws_conn_id = aws_conn_id
+        self.region_name = region_name or self.hook_params.pop("region_name", None)
         super().__init__(*args, **kwargs)
 
         self._await_interval = 60  # seconds
 
+    @cachedproperty
+    def hook(self) -> RdsHook:
+        return RdsHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name, **self.hook_params)
+
     def execute(self, context: Context) -> str:
         """Different implementations for snapshots, tasks and events."""
         raise NotImplementedError
 
     def on_kill(self) -> None:
         """Different implementations for snapshots, tasks and events."""
         raise NotImplementedError
@@ -102,18 +111,17 @@
         self,
         *,
         db_type: str,
         db_identifier: str,
         db_snapshot_identifier: str,
         tags: Sequence[TagTypeDef] | dict | None = None,
         wait_for_completion: bool = True,
-        aws_conn_id: str = "aws_default",
         **kwargs,
     ):
-        super().__init__(aws_conn_id=aws_conn_id, **kwargs)
+        super().__init__(**kwargs)
         self.db_type = RdsDbType(db_type)
         self.db_identifier = db_identifier
         self.db_snapshot_identifier = db_snapshot_identifier
         self.tags = tags
         self.wait_for_completion = wait_for_completion
 
     def execute(self, context: Context) -> str:
@@ -190,18 +198,17 @@
         tags: Sequence[TagTypeDef] | dict | None = None,
         copy_tags: bool = False,
         pre_signed_url: str = "",
         option_group_name: str = "",
         target_custom_availability_zone: str = "",
         source_region: str = "",
         wait_for_completion: bool = True,
-        aws_conn_id: str = "aws_default",
         **kwargs,
     ):
-        super().__init__(aws_conn_id=aws_conn_id, **kwargs)
+        super().__init__(**kwargs)
 
         self.db_type = RdsDbType(db_type)
         self.source_db_snapshot_identifier = source_db_snapshot_identifier
         self.target_db_snapshot_identifier = target_db_snapshot_identifier
         self.kms_key_id = kms_key_id
         self.tags = tags
         self.copy_tags = copy_tags
@@ -270,18 +277,17 @@
 
     def __init__(
         self,
         *,
         db_type: str,
         db_snapshot_identifier: str,
         wait_for_completion: bool = True,
-        aws_conn_id: str = "aws_default",
         **kwargs,
     ):
-        super().__init__(aws_conn_id=aws_conn_id, **kwargs)
+        super().__init__(**kwargs)
 
         self.db_type = RdsDbType(db_type)
         self.db_snapshot_identifier = db_snapshot_identifier
         self.wait_for_completion = wait_for_completion
 
     def execute(self, context: Context) -> str:
         self.log.info("Starting to delete snapshot '%s'", self.db_snapshot_identifier)
@@ -341,18 +347,17 @@
         source_arn: str,
         s3_bucket_name: str,
         iam_role_arn: str,
         kms_key_id: str,
         s3_prefix: str = "",
         export_only: list[str] | None = None,
         wait_for_completion: bool = True,
-        aws_conn_id: str = "aws_default",
         **kwargs,
     ):
-        super().__init__(aws_conn_id=aws_conn_id, **kwargs)
+        super().__init__(**kwargs)
 
         self.export_task_identifier = export_task_identifier
         self.source_arn = source_arn
         self.s3_bucket_name = s3_bucket_name
         self.iam_role_arn = iam_role_arn
         self.kms_key_id = kms_key_id
         self.s3_prefix = s3_prefix
@@ -393,18 +398,17 @@
 
     def __init__(
         self,
         *,
         export_task_identifier: str,
         wait_for_completion: bool = True,
         check_interval: int = 30,
-        aws_conn_id: str = "aws_default",
         **kwargs,
     ):
-        super().__init__(aws_conn_id=aws_conn_id, **kwargs)
+        super().__init__(**kwargs)
 
         self.export_task_identifier = export_task_identifier
         self.wait_for_completion = wait_for_completion
         self.check_interval = check_interval
 
     def execute(self, context: Context) -> str:
         self.log.info("Canceling export task %s", self.export_task_identifier)
@@ -457,18 +461,17 @@
         sns_topic_arn: str,
         source_type: str = "",
         event_categories: Sequence[str] | None = None,
         source_ids: Sequence[str] | None = None,
         enabled: bool = True,
         tags: Sequence[TagTypeDef] | dict | None = None,
         wait_for_completion: bool = True,
-        aws_conn_id: str = "aws_default",
         **kwargs,
     ):
-        super().__init__(aws_conn_id=aws_conn_id, **kwargs)
+        super().__init__(**kwargs)
 
         self.subscription_name = subscription_name
         self.sns_topic_arn = sns_topic_arn
         self.source_type = source_type
         self.event_categories = event_categories or []
         self.source_ids = source_ids or []
         self.enabled = enabled
@@ -507,18 +510,17 @@
 
     template_fields = ("subscription_name",)
 
     def __init__(
         self,
         *,
         subscription_name: str,
-        aws_conn_id: str = "aws_default",
         **kwargs,
     ):
-        super().__init__(aws_conn_id=aws_conn_id, **kwargs)
+        super().__init__(**kwargs)
 
         self.subscription_name = subscription_name
 
     def execute(self, context: Context) -> str:
         self.log.info(
             "Deleting event subscription %s",
             self.subscription_name,
@@ -541,15 +543,14 @@
 
     :param db_instance_identifier: The DB instance identifier, must start with a letter and
         contain from 1 to 63 letters, numbers, or hyphens
     :param db_instance_class: The compute and memory capacity of the DB instance, for example db.m5.large
     :param engine: The name of the database engine to be used for this instance
     :param rds_kwargs: Named arguments to pass to boto3 RDS client function ``create_db_instance``
         https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.create_db_instance
-    :param aws_conn_id: The Airflow connection used for AWS credentials.
     :param wait_for_completion:  If True, waits for creation of the DB instance to complete. (default: True)
     :param waiter_delay: Time (in seconds) to wait between two consecutive calls to check DB instance state
     :param waiter_max_attempts: The maximum number of attempts to check DB instance state
     :param deferrable: If True, the operator will wait asynchronously for the DB instance to be created.
         This implies waiting for completion. This mode requires aiobotocore module to be installed.
         (default: False)
     """
@@ -559,53 +560,51 @@
     def __init__(
         self,
         *,
         db_instance_identifier: str,
         db_instance_class: str,
         engine: str,
         rds_kwargs: dict | None = None,
-        aws_conn_id: str = "aws_default",
         wait_for_completion: bool = True,
         deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         waiter_delay: int = 30,
         waiter_max_attempts: int = 60,
         **kwargs,
     ):
-        super().__init__(aws_conn_id=aws_conn_id, **kwargs)
+        super().__init__(**kwargs)
 
         self.db_instance_identifier = db_instance_identifier
         self.db_instance_class = db_instance_class
         self.engine = engine
         self.rds_kwargs = rds_kwargs or {}
         self.wait_for_completion = False if deferrable else wait_for_completion
         self.deferrable = deferrable
         self.waiter_delay = waiter_delay
         self.waiter_max_attempts = waiter_max_attempts
-        self.aws_conn_id = aws_conn_id
 
     def execute(self, context: Context) -> str:
         self.log.info("Creating new DB instance %s", self.db_instance_identifier)
 
         create_db_instance = self.hook.conn.create_db_instance(
             DBInstanceIdentifier=self.db_instance_identifier,
             DBInstanceClass=self.db_instance_class,
             Engine=self.engine,
             **self.rds_kwargs,
         )
         if self.deferrable:
             self.defer(
-                trigger=RdsDbInstanceTrigger(
-                    db_instance_identifier=self.db_instance_identifier,
+                trigger=RdsDbAvailableTrigger(
+                    db_identifier=self.db_instance_identifier,
                     waiter_delay=self.waiter_delay,
                     waiter_max_attempts=self.waiter_max_attempts,
                     aws_conn_id=self.aws_conn_id,
                     region_name=self.region_name,
-                    waiter_name="db_instance_available",
                     # ignoring type because create_db_instance is a dict
                     response=create_db_instance,  # type: ignore[arg-type]
+                    db_type=RdsDbType.INSTANCE,
                 ),
                 method_name="execute_complete",
                 timeout=timedelta(seconds=self.waiter_delay * self.waiter_max_attempts),
             )
 
         if self.wait_for_completion:
             waiter = self.hook.conn.get_waiter("db_instance_available")
@@ -634,15 +633,14 @@
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:RdsDeleteDbInstanceOperator`
 
     :param db_instance_identifier: The DB instance identifier for the DB instance to be deleted
     :param rds_kwargs: Named arguments to pass to boto3 RDS client function ``delete_db_instance``
         https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.delete_db_instance
-    :param aws_conn_id: The Airflow connection used for AWS credentials.
     :param wait_for_completion:  If True, waits for deletion of the DB instance to complete. (default: True)
     :param waiter_delay: Time (in seconds) to wait between two consecutive calls to check DB instance state
     :param waiter_max_attempts: The maximum number of attempts to check DB instance state
     :param deferrable: If True, the operator will wait asynchronously for the DB instance to be created.
         This implies waiting for completion. This mode requires aiobotocore module to be installed.
         (default: False)
     """
@@ -650,48 +648,46 @@
     template_fields = ("db_instance_identifier", "rds_kwargs")
 
     def __init__(
         self,
         *,
         db_instance_identifier: str,
         rds_kwargs: dict | None = None,
-        aws_conn_id: str = "aws_default",
         wait_for_completion: bool = True,
         deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         waiter_delay: int = 30,
         waiter_max_attempts: int = 60,
         **kwargs,
     ):
-        super().__init__(aws_conn_id=aws_conn_id, **kwargs)
+        super().__init__(**kwargs)
         self.db_instance_identifier = db_instance_identifier
         self.rds_kwargs = rds_kwargs or {}
         self.wait_for_completion = False if deferrable else wait_for_completion
         self.deferrable = deferrable
         self.waiter_delay = waiter_delay
         self.waiter_max_attempts = waiter_max_attempts
-        self.aws_conn_id = aws_conn_id
 
     def execute(self, context: Context) -> str:
         self.log.info("Deleting DB instance %s", self.db_instance_identifier)
 
         delete_db_instance = self.hook.conn.delete_db_instance(
             DBInstanceIdentifier=self.db_instance_identifier,
             **self.rds_kwargs,
         )
         if self.deferrable:
             self.defer(
-                trigger=RdsDbInstanceTrigger(
-                    db_instance_identifier=self.db_instance_identifier,
+                trigger=RdsDbDeletedTrigger(
+                    db_identifier=self.db_instance_identifier,
                     waiter_delay=self.waiter_delay,
                     waiter_max_attempts=self.waiter_max_attempts,
                     aws_conn_id=self.aws_conn_id,
                     region_name=self.region_name,
-                    waiter_name="db_instance_deleted",
                     # ignoring type because delete_db_instance is a dict
                     response=delete_db_instance,  # type: ignore[arg-type]
+                    db_type=RdsDbType.INSTANCE,
                 ),
                 method_name="execute_complete",
                 timeout=timedelta(seconds=self.waiter_delay * self.waiter_max_attempts),
             )
 
         if self.wait_for_completion:
             waiter = self.hook.conn.get_waiter("db_instance_deleted")
@@ -719,55 +715,94 @@
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:RdsStartDbOperator`
 
     :param db_identifier: The AWS identifier of the DB to start
     :param db_type: Type of the DB - either "instance" or "cluster" (default: "instance")
-    :param aws_conn_id: The Airflow connection used for AWS credentials. (default: "aws_default")
     :param wait_for_completion:  If True, waits for DB to start. (default: True)
+    :param waiter_delay: Time (in seconds) to wait between two consecutive calls to check DB instance state
+    :param waiter_max_attempts: The maximum number of attempts to check DB instance state
+    :param deferrable: If True, the operator will wait asynchronously for the DB instance to be created.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
     """
 
     template_fields = ("db_identifier", "db_type")
 
     def __init__(
         self,
         *,
         db_identifier: str,
         db_type: RdsDbType | str = RdsDbType.INSTANCE,
-        aws_conn_id: str = "aws_default",
         wait_for_completion: bool = True,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 40,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
-        super().__init__(aws_conn_id=aws_conn_id, **kwargs)
+        super().__init__(**kwargs)
         self.db_identifier = db_identifier
         self.db_type = db_type
         self.wait_for_completion = wait_for_completion
+        self.waiter_delay = waiter_delay
+        self.waiter_max_attempts = waiter_max_attempts
+        self.deferrable = deferrable
 
     def execute(self, context: Context) -> str:
         self.db_type = RdsDbType(self.db_type)
-        start_db_response = self._start_db()
-        if self.wait_for_completion:
+        start_db_response: dict[str, Any] = self._start_db()
+        if self.deferrable:
+            self.defer(
+                trigger=RdsDbAvailableTrigger(
+                    db_identifier=self.db_identifier,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                    region_name=self.region_name,
+                    response=start_db_response,
+                    db_type=RdsDbType.INSTANCE,
+                ),
+                method_name="execute_complete",
+            )
+        elif self.wait_for_completion:
             self._wait_until_db_available()
         return json.dumps(start_db_response, default=str)
 
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> str:
+        if event is None or event["status"] != "success":
+            raise AirflowException(f"Failed to start DB: {event}")
+        else:
+            return json.dumps(event["response"], default=str)
+
     def _start_db(self):
         self.log.info("Starting DB %s '%s'", self.db_type.value, self.db_identifier)
         if self.db_type == RdsDbType.INSTANCE:
-            response = self.hook.conn.start_db_instance(DBInstanceIdentifier=self.db_identifier)
+            response = self.hook.conn.start_db_instance(
+                DBInstanceIdentifier=self.db_identifier,
+            )
         else:
             response = self.hook.conn.start_db_cluster(DBClusterIdentifier=self.db_identifier)
         return response
 
     def _wait_until_db_available(self):
         self.log.info("Waiting for DB %s to reach 'available' state", self.db_type.value)
         if self.db_type == RdsDbType.INSTANCE:
-            self.hook.wait_for_db_instance_state(self.db_identifier, target_state="available")
+            self.hook.wait_for_db_instance_state(
+                self.db_identifier,
+                target_state="available",
+                check_interval=self.waiter_delay,
+                max_attempts=self.waiter_max_attempts,
+            )
         else:
-            self.hook.wait_for_db_cluster_state(self.db_identifier, target_state="available")
+            self.hook.wait_for_db_cluster_state(
+                self.db_identifier,
+                target_state="available",
+                check_interval=self.waiter_delay,
+                max_attempts=self.waiter_max_attempts,
+            )
 
 
 class RdsStopDbOperator(RdsBaseOperator):
     """
     Stops an RDS DB instance / cluster.
 
     .. seealso::
@@ -775,43 +810,70 @@
         :ref:`howto/operator:RdsStopDbOperator`
 
     :param db_identifier: The AWS identifier of the DB to stop
     :param db_type: Type of the DB - either "instance" or "cluster" (default: "instance")
     :param db_snapshot_identifier: The instance identifier of the DB Snapshot to create before
         stopping the DB instance. The default value (None) skips snapshot creation. This
         parameter is ignored when ``db_type`` is "cluster"
-    :param aws_conn_id: The Airflow connection used for AWS credentials. (default: "aws_default")
     :param wait_for_completion:  If True, waits for DB to stop. (default: True)
+    :param waiter_delay: Time (in seconds) to wait between two consecutive calls to check DB instance state
+    :param waiter_max_attempts: The maximum number of attempts to check DB instance state
+    :param deferrable: If True, the operator will wait asynchronously for the DB instance to be created.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
     """
 
     template_fields = ("db_identifier", "db_snapshot_identifier", "db_type")
 
     def __init__(
         self,
         *,
         db_identifier: str,
         db_type: RdsDbType | str = RdsDbType.INSTANCE,
         db_snapshot_identifier: str | None = None,
-        aws_conn_id: str = "aws_default",
         wait_for_completion: bool = True,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 40,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
-        super().__init__(aws_conn_id=aws_conn_id, **kwargs)
+        super().__init__(**kwargs)
         self.db_identifier = db_identifier
         self.db_type = db_type
         self.db_snapshot_identifier = db_snapshot_identifier
         self.wait_for_completion = wait_for_completion
+        self.waiter_delay = waiter_delay
+        self.waiter_max_attempts = waiter_max_attempts
+        self.deferrable = deferrable
 
     def execute(self, context: Context) -> str:
         self.db_type = RdsDbType(self.db_type)
-        stop_db_response = self._stop_db()
-        if self.wait_for_completion:
+        stop_db_response: dict[str, Any] = self._stop_db()
+        if self.deferrable:
+            self.defer(
+                trigger=RdsDbStoppedTrigger(
+                    db_identifier=self.db_identifier,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                    region_name=self.region_name,
+                    response=stop_db_response,
+                    db_type=RdsDbType.INSTANCE,
+                ),
+                method_name="execute_complete",
+            )
+        elif self.wait_for_completion:
             self._wait_until_db_stopped()
         return json.dumps(stop_db_response, default=str)
 
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> str:
+        if event is None or event["status"] != "success":
+            raise AirflowException(f"Failed to start DB: {event}")
+        else:
+            return json.dumps(event["response"], default=str)
+
     def _stop_db(self):
         self.log.info("Stopping DB %s '%s'", self.db_type.value, self.db_identifier)
         if self.db_type == RdsDbType.INSTANCE:
             conn_params = {"DBInstanceIdentifier": self.db_identifier}
             # The db snapshot parameter is optional, but the AWS SDK raises an exception
             # if passed a null value. Only set snapshot id if value is present.
             if self.db_snapshot_identifier:
@@ -825,17 +887,27 @@
                 )
             response = self.hook.conn.stop_db_cluster(DBClusterIdentifier=self.db_identifier)
         return response
 
     def _wait_until_db_stopped(self):
         self.log.info("Waiting for DB %s to reach 'stopped' state", self.db_type.value)
         if self.db_type == RdsDbType.INSTANCE:
-            self.hook.wait_for_db_instance_state(self.db_identifier, target_state="stopped")
+            self.hook.wait_for_db_instance_state(
+                self.db_identifier,
+                target_state="stopped",
+                check_interval=self.waiter_delay,
+                max_attempts=self.waiter_max_attempts,
+            )
         else:
-            self.hook.wait_for_db_cluster_state(self.db_identifier, target_state="stopped")
+            self.hook.wait_for_db_cluster_state(
+                self.db_identifier,
+                target_state="stopped",
+                check_interval=self.waiter_delay,
+                max_attempts=self.waiter_max_attempts,
+            )
 
 
 __all__ = [
     "RdsCreateDbSnapshotOperator",
     "RdsCopyDbSnapshotOperator",
     "RdsDeleteDbSnapshotOperator",
     "RdsCreateEventSubscriptionOperator",
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/redshift_data.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,25 +47,29 @@
     :param with_event: indicates whether to send an event to EventBridge
     :param wait_for_completion: indicates whether to wait for a result, if True wait, if False don't wait
     :param poll_interval: how often in seconds to check the query status
     :param return_sql_result: if True will return the result of an SQL statement,
         if False (default) will return statement ID
     :param aws_conn_id: aws connection to use
     :param region: aws region to use
+    :param workgroup_name: name of the Redshift Serverless workgroup. Mutually exclusive with
+        `cluster_identifier`. Specify this parameter to query Redshift Serverless. More info
+        https://docs.aws.amazon.com/redshift/latest/mgmt/working-with-serverless.html
     """
 
     template_fields = (
         "cluster_identifier",
         "database",
         "sql",
         "db_user",
         "parameters",
         "statement_name",
         "aws_conn_id",
         "region",
+        "workgroup_name",
     )
     template_ext = (".sql",)
     template_fields_renderers = {"sql": "sql"}
     statement_id: str | None
 
     def __init__(
         self,
@@ -78,20 +82,22 @@
         statement_name: str | None = None,
         with_event: bool = False,
         wait_for_completion: bool = True,
         poll_interval: int = 10,
         return_sql_result: bool = False,
         aws_conn_id: str = "aws_default",
         region: str | None = None,
+        workgroup_name: str | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.database = database
         self.sql = sql
         self.cluster_identifier = cluster_identifier
+        self.workgroup_name = workgroup_name
         self.db_user = db_user
         self.parameters = parameters
         self.secret_arn = secret_arn
         self.statement_name = statement_name
         self.with_event = with_event
         self.wait_for_completion = wait_for_completion
         if poll_interval > 0:
@@ -115,14 +121,15 @@
         """Execute a statement against Amazon Redshift."""
         self.log.info("Executing statement: %s", self.sql)
 
         self.statement_id = self.hook.execute_query(
             database=self.database,
             sql=self.sql,
             cluster_identifier=self.cluster_identifier,
+            workgroup_name=self.workgroup_name,
             db_user=self.db_user,
             parameters=self.parameters,
             secret_arn=self.secret_arn,
             statement_name=self.statement_name,
             with_event=self.with_event,
             wait_for_completion=self.wait_for_completion,
             poll_interval=self.poll_interval,
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/sagemaker.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,18 @@
 from botocore.exceptions import ClientError
 
 from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.providers.amazon.aws.hooks.sagemaker import SageMakerHook
-from airflow.providers.amazon.aws.triggers.sagemaker import SageMakerTrigger
+from airflow.providers.amazon.aws.triggers.sagemaker import (
+    SageMakerPipelineTrigger,
+    SageMakerTrigger,
+)
 from airflow.providers.amazon.aws.utils import trim_none_values
 from airflow.providers.amazon.aws.utils.sagemaker import ApprovalStatus
 from airflow.providers.amazon.aws.utils.tags import format_tags
 from airflow.utils.json import AirflowJsonEncoder
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
@@ -994,16 +997,18 @@
     :param aws_conn_id: The AWS connection ID to use.
     :param pipeline_name: Name of the pipeline to start.
     :param display_name: The name this pipeline execution will have in the UI. Doesn't need to be unique.
     :param pipeline_params: Optional parameters for the pipeline.
         All parameters supplied need to already be present in the pipeline definition.
     :param wait_for_completion: If true, this operator will only complete once the pipeline is complete.
     :param check_interval: How long to wait between checks for pipeline status when waiting for completion.
+    :param waiter_max_attempts: How many times to check the status before failing.
     :param verbose: Whether to print steps details when waiting for completion.
         Defaults to true, consider turning off for pipelines that have thousands of steps.
+    :param deferrable: Run operator in the deferrable mode.
 
     :return str: Returns The ARN of the pipeline execution created in Amazon SageMaker.
     """
 
     template_fields: Sequence[str] = ("aws_conn_id", "pipeline_name", "display_name", "pipeline_params")
 
     def __init__(
@@ -1011,39 +1016,65 @@
         *,
         aws_conn_id: str = DEFAULT_CONN_ID,
         pipeline_name: str,
         display_name: str = "airflow-triggered-execution",
         pipeline_params: dict | None = None,
         wait_for_completion: bool = False,
         check_interval: int = CHECK_INTERVAL_SECOND,
+        waiter_max_attempts: int = 9999,
         verbose: bool = True,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(config={}, aws_conn_id=aws_conn_id, **kwargs)
         self.pipeline_name = pipeline_name
         self.display_name = display_name
         self.pipeline_params = pipeline_params
         self.wait_for_completion = wait_for_completion
         self.check_interval = check_interval
+        self.waiter_max_attempts = waiter_max_attempts
         self.verbose = verbose
+        self.deferrable = deferrable
 
     def execute(self, context: Context) -> str:
         arn = self.hook.start_pipeline(
             pipeline_name=self.pipeline_name,
             display_name=self.display_name,
             pipeline_params=self.pipeline_params,
-            wait_for_completion=self.wait_for_completion,
-            check_interval=self.check_interval,
-            verbose=self.verbose,
         )
         self.log.info(
             "Starting a new execution for pipeline %s, running with ARN %s", self.pipeline_name, arn
         )
+        if self.deferrable:
+            self.defer(
+                trigger=SageMakerPipelineTrigger(
+                    waiter_type=SageMakerPipelineTrigger.Type.COMPLETE,
+                    pipeline_execution_arn=arn,
+                    waiter_delay=self.check_interval,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                ),
+                method_name="execute_complete",
+            )
+        elif self.wait_for_completion:
+            self.hook.check_status(
+                arn,
+                "PipelineExecutionStatus",
+                lambda p: self.hook.describe_pipeline_exec(p, self.verbose),
+                self.check_interval,
+                non_terminal_states=self.hook.pipeline_non_terminal_states,
+                max_ingestion_time=self.waiter_max_attempts * self.check_interval,
+            )
         return arn
 
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> str:
+        if event is None or event["status"] != "success":
+            raise AirflowException(f"Failure during pipeline execution: {event}")
+        return event["value"]
+
 
 class SageMakerStopPipelineOperator(SageMakerBaseOperator):
     """
     Stops a SageMaker pipeline execution.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
@@ -1053,14 +1084,15 @@
     :param aws_conn_id: The AWS connection ID to use.
     :param pipeline_exec_arn: Amazon Resource Name of the pipeline execution to stop.
     :param wait_for_completion: If true, this operator will only complete once the pipeline is fully stopped.
     :param check_interval: How long to wait between checks for pipeline status when waiting for completion.
     :param verbose: Whether to print steps details when waiting for completion.
         Defaults to true, consider turning off for pipelines that have thousands of steps.
     :param fail_if_not_running: raises an exception if the pipeline stopped or succeeded before this was run
+    :param deferrable: Run operator in the deferrable mode.
 
     :return str: Returns the status of the pipeline execution after the operation has been done.
     """
 
     template_fields: Sequence[str] = (
         "aws_conn_id",
         "pipeline_exec_arn",
@@ -1069,40 +1101,76 @@
     def __init__(
         self,
         *,
         aws_conn_id: str = DEFAULT_CONN_ID,
         pipeline_exec_arn: str,
         wait_for_completion: bool = False,
         check_interval: int = CHECK_INTERVAL_SECOND,
+        waiter_max_attempts: int = 9999,
         verbose: bool = True,
         fail_if_not_running: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(config={}, aws_conn_id=aws_conn_id, **kwargs)
         self.pipeline_exec_arn = pipeline_exec_arn
         self.wait_for_completion = wait_for_completion
         self.check_interval = check_interval
+        self.waiter_max_attempts = waiter_max_attempts
         self.verbose = verbose
         self.fail_if_not_running = fail_if_not_running
+        self.deferrable = deferrable
 
     def execute(self, context: Context) -> str:
         status = self.hook.stop_pipeline(
             pipeline_exec_arn=self.pipeline_exec_arn,
-            wait_for_completion=self.wait_for_completion,
-            check_interval=self.check_interval,
-            verbose=self.verbose,
             fail_if_not_running=self.fail_if_not_running,
         )
         self.log.info(
             "Stop requested for pipeline execution with ARN %s. Status is now %s",
             self.pipeline_exec_arn,
             status,
         )
+
+        if status not in self.hook.pipeline_non_terminal_states:
+            # pipeline already stopped
+            return status
+
+        # else, eventually wait for completion
+        if self.deferrable:
+            self.defer(
+                trigger=SageMakerPipelineTrigger(
+                    waiter_type=SageMakerPipelineTrigger.Type.STOPPED,
+                    pipeline_execution_arn=self.pipeline_exec_arn,
+                    waiter_delay=self.check_interval,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                ),
+                method_name="execute_complete",
+            )
+        elif self.wait_for_completion:
+            status = self.hook.check_status(
+                self.pipeline_exec_arn,
+                "PipelineExecutionStatus",
+                lambda p: self.hook.describe_pipeline_exec(p, self.verbose),
+                self.check_interval,
+                non_terminal_states=self.hook.pipeline_non_terminal_states,
+                max_ingestion_time=self.waiter_max_attempts * self.check_interval,
+            )["PipelineExecutionStatus"]
+
         return status
 
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> str:
+        if event is None or event["status"] != "success":
+            raise AirflowException(f"Failure during pipeline execution: {event}")
+        else:
+            # theoretically we should do a `describe` call to know this,
+            # but if we reach this point, this is the only possible status
+            return "Stopped"
+
 
 class SageMakerRegisterModelVersionOperator(SageMakerBaseOperator):
     """
     Register a SageMaker model by creating a model version that specifies the model group to which it belongs.
 
     Will create the model group if it does not exist already.
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/sns.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/sqs.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/operators/step_function.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import json
-from typing import TYPE_CHECKING, Sequence
+from datetime import timedelta
+from typing import TYPE_CHECKING, Any, Sequence
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.step_function import StepFunctionHook
+from airflow.providers.amazon.aws.triggers.step_function import StepFunctionsExecutionCompleteTrigger
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class StepFunctionStartExecutionOperator(BaseOperator):
     """
@@ -38,49 +41,78 @@
         :ref:`howto/operator:StepFunctionStartExecutionOperator`
 
     :param state_machine_arn: ARN of the Step Function State Machine
     :param name: The name of the execution.
     :param state_machine_input: JSON data input to pass to the State Machine
     :param aws_conn_id: aws connection to uses
     :param do_xcom_push: if True, execution_arn is pushed to XCom with key execution_arn.
+    :param waiter_max_attempts: Maximum number of attempts to poll the execution.
+    :param waiter_delay: Number of seconds between polling the state of the execution.
+    :param deferrable: If True, the operator will wait asynchronously for the job to complete.
+        This implies waiting for completion. This mode requires aiobotocore module to be installed.
+        (default: False, but can be overridden in config file by setting default_deferrable to True)
     """
 
     template_fields: Sequence[str] = ("state_machine_arn", "name", "input")
     template_ext: Sequence[str] = ()
     ui_color = "#f9c915"
 
     def __init__(
         self,
         *,
         state_machine_arn: str,
         name: str | None = None,
         state_machine_input: dict | str | None = None,
         aws_conn_id: str = "aws_default",
         region_name: str | None = None,
+        waiter_max_attempts: int = 30,
+        waiter_delay: int = 60,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.state_machine_arn = state_machine_arn
         self.name = name
         self.input = state_machine_input
         self.aws_conn_id = aws_conn_id
         self.region_name = region_name
+        self.waiter_delay = waiter_delay
+        self.waiter_max_attempts = waiter_max_attempts
+        self.deferrable = deferrable
 
     def execute(self, context: Context):
         hook = StepFunctionHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
 
         execution_arn = hook.start_execution(self.state_machine_arn, self.name, self.input)
 
         if execution_arn is None:
             raise AirflowException(f"Failed to start State Machine execution for: {self.state_machine_arn}")
 
         self.log.info("Started State Machine execution for %s: %s", self.state_machine_arn, execution_arn)
-
+        if self.deferrable:
+            self.defer(
+                trigger=StepFunctionsExecutionCompleteTrigger(
+                    execution_arn=execution_arn,
+                    waiter_delay=self.waiter_delay,
+                    waiter_max_attempts=self.waiter_max_attempts,
+                    aws_conn_id=self.aws_conn_id,
+                    region_name=self.region_name,
+                ),
+                method_name="execute_complete",
+                timeout=timedelta(seconds=self.waiter_max_attempts * self.waiter_delay),
+            )
         return execution_arn
 
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        if event is None or event["status"] != "success":
+            raise AirflowException(f"Trigger error: event is {event}")
+
+        self.log.info("State Machine execution completed successfully")
+        return event["execution_arn"]
+
 
 class StepFunctionGetExecutionOutputOperator(BaseOperator):
     """
     An Operator that returns the output of an AWS Step Function State Machine execution.
 
     Additional arguments may be specified and are passed down to the underlying BaseOperator.
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/__init__.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/secrets/systems_manager.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/__init__.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/athena.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/batch.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/dms.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/dynamodb.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/ec2.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/ecs.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/eks.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/emr.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glacier.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glue.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/lambda_function.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/quicksight.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/rds.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/sagemaker.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/sqs.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/sensors/step_function.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/__init__.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/base.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
             if not keys:
                 raise AirflowException(
                     f"No primary key on {self.schema}.{self.table}. Please provide keys on 'upsert_keys'"
                 )
             where_statement = " AND ".join([f"{self.table}.{k} = {copy_destination}.{k}" for k in keys])
 
             sql = [
-                f"CREATE TABLE {copy_destination} (LIKE {destination});",
+                f"CREATE TABLE {copy_destination} (LIKE {destination} INCLUDING DEFAULTS);",
                 copy_statement,
                 "BEGIN;",
                 f"DELETE FROM {destination} USING {copy_destination} WHERE {where_statement};",
                 f"INSERT INTO {destination} SELECT * FROM {copy_destination};",
                 "COMMIT",
             ]
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/__init__.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/athena.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/base.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/batch.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     :param waiter_delay: polling period in seconds to check for the status of the job
     :param waiter_max_attempts: The maximum number of attempts to be made.
     """
 
     def __init__(
         self,
         job_id: str | None,
-        region_name: str | None,
+        region_name: str | None = None,
         aws_conn_id: str | None = "aws_default",
         waiter_delay: int = 5,
         waiter_max_attempts: int = 720,
     ):
         super().__init__(
             serialized_fields={"job_id": job_id},
             waiter_name="batch_job_complete",
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/ec2.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/ecs.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/ecs.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from __future__ import annotations
 
 import asyncio
 from typing import Any, AsyncIterator
 
 from botocore.exceptions import ClientError, WaiterError
 
+from airflow import AirflowException
 from airflow.providers.amazon.aws.hooks.base_aws import AwsGenericHook
 from airflow.providers.amazon.aws.hooks.ecs import EcsHook
 from airflow.providers.amazon.aws.hooks.logs import AwsLogsHook
 from airflow.providers.amazon.aws.triggers.base import AwsBaseWaiterTrigger
 from airflow.providers.amazon.aws.utils.task_log_fetcher import AwsTaskLogFetcher
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
@@ -44,15 +45,15 @@
 
     def __init__(
         self,
         cluster_arn: str,
         waiter_delay: int,
         waiter_max_attempts: int,
         aws_conn_id: str | None,
-        region_name: str | None,
+        region_name: str | None = None,
     ):
         super().__init__(
             serialized_fields={"cluster_arn": cluster_arn},
             waiter_name="cluster_active",
             waiter_args={"clusters": [cluster_arn]},
             failure_message="Failure while waiting for cluster to be available",
             status_message="Cluster is not ready yet",
@@ -83,15 +84,15 @@
 
     def __init__(
         self,
         cluster_arn: str,
         waiter_delay: int,
         waiter_max_attempts: int,
         aws_conn_id: str | None,
-        region_name: str | None,
+        region_name: str | None = None,
     ):
         super().__init__(
             serialized_fields={"cluster_arn": cluster_arn},
             waiter_name="cluster_inactive",
             waiter_args={"clusters": [cluster_arn]},
             failure_message="Failure while waiting for cluster to be deactivated",
             status_message="Cluster deactivation is not done yet",
@@ -166,25 +167,26 @@
             logs_token = None
             while self.waiter_max_attempts >= 1:
                 self.waiter_max_attempts = self.waiter_max_attempts - 1
                 try:
                     await waiter.wait(
                         cluster=self.cluster, tasks=[self.task_arn], WaiterConfig={"MaxAttempts": 1}
                     )
-                    break  # we reach this point only if the waiter met a success criteria
+                    # we reach this point only if the waiter met a success criteria
+                    yield TriggerEvent({"status": "success", "task_arn": self.task_arn})
+                    return
                 except WaiterError as error:
                     if "terminal failure" in str(error):
                         raise
                     self.log.info("Status of the task is %s", error.last_response["tasks"][0]["lastStatus"])
                     await asyncio.sleep(int(self.waiter_delay))
                 finally:
                     if self.log_group and self.log_stream:
                         logs_token = await self._forward_logs(logs_client, logs_token)
-
-        yield TriggerEvent({"status": "success", "task_arn": self.task_arn})
+        raise AirflowException("Waiter error: max attempts reached")
 
     async def _forward_logs(self, logs_client, next_token: str | None = None) -> str | None:
         """
         Reads logs from the cloudwatch stream and prints them to the task logs.
 
         :return: the token to pass to the next iteration to resume where we started.
         """
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/emr.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/rds.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,274 +12,234 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-import asyncio
 import warnings
 from typing import Any
 
-from botocore.exceptions import WaiterError
-
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.amazon.aws.hooks.base_aws import AwsGenericHook
-from airflow.providers.amazon.aws.hooks.emr import EmrContainerHook, EmrHook
+from airflow.providers.amazon.aws.hooks.rds import RdsHook
 from airflow.providers.amazon.aws.triggers.base import AwsBaseWaiterTrigger
+from airflow.providers.amazon.aws.utils.rds import RdsDbType
+from airflow.providers.amazon.aws.utils.waiter_with_logging import async_wait
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
-class EmrAddStepsTrigger(BaseTrigger):
+class RdsDbInstanceTrigger(BaseTrigger):
     """
-    Asynchronously poll the boto3 API and wait for the steps to finish executing.
+    Deprecated Trigger for RDS operations. Do not use.
 
-    :param job_flow_id: The id of the job flow.
-    :param step_ids: The id of the steps being waited upon.
-    :param poll_interval: The amount of time in seconds to wait between attempts.
-    :param max_attempts: The maximum number of attempts to be made.
+    :param waiter_name: Name of the waiter to use, for instance 'db_instance_available'
+        or 'db_instance_deleted'.
+    :param db_instance_identifier: The DB instance identifier for the DB instance to be polled.
+    :param waiter_delay: The amount of time in seconds to wait between attempts.
+    :param waiter_max_attempts: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
+    :param region_name: AWS region where the DB is located, if different from the default one.
+    :param response: The response from the RdsHook, to be passed back to the operator.
     """
 
     def __init__(
         self,
-        job_flow_id: str,
-        step_ids: list[str],
+        waiter_name: str,
+        db_instance_identifier: str,
+        waiter_delay: int,
+        waiter_max_attempts: int,
         aws_conn_id: str,
-        max_attempts: int | None,
-        poll_interval: int | None,
+        region_name: str | None,
+        response: dict[str, Any],
     ):
-        self.job_flow_id = job_flow_id
-        self.step_ids = step_ids
+        warnings.warn(
+            "This trigger is deprecated, please use the other RDS triggers "
+            "such as RdsDbDeletedTrigger, RdsDbStoppedTrigger or RdsDbAvailableTrigger",
+            AirflowProviderDeprecationWarning,
+            stacklevel=2,
+        )
+        self.db_instance_identifier = db_instance_identifier
+        self.waiter_delay = waiter_delay
+        self.waiter_max_attempts = waiter_max_attempts
         self.aws_conn_id = aws_conn_id
-        self.max_attempts = max_attempts
-        self.poll_interval = poll_interval
+        self.region_name = region_name
+        self.waiter_name = waiter_name
+        self.response = response
 
     def serialize(self) -> tuple[str, dict[str, Any]]:
         return (
-            "airflow.providers.amazon.aws.triggers.emr.EmrAddStepsTrigger",
+            # dynamically generate the fully qualified name of the class
+            self.__class__.__module__ + "." + self.__class__.__qualname__,
             {
-                "job_flow_id": str(self.job_flow_id),
-                "step_ids": self.step_ids,
-                "poll_interval": str(self.poll_interval),
-                "max_attempts": str(self.max_attempts),
-                "aws_conn_id": str(self.aws_conn_id),
+                "db_instance_identifier": self.db_instance_identifier,
+                "waiter_delay": str(self.waiter_delay),
+                "waiter_max_attempts": str(self.waiter_max_attempts),
+                "aws_conn_id": self.aws_conn_id,
+                "region_name": self.region_name,
+                "waiter_name": self.waiter_name,
+                "response": self.response,
             },
         )
 
     async def run(self):
-        self.hook = EmrHook(aws_conn_id=self.aws_conn_id)
+        self.hook = RdsHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
         async with self.hook.async_conn as client:
-            for step_id in self.step_ids:
-                attempt = 0
-                waiter = client.get_waiter("step_complete")
-                while attempt < int(self.max_attempts):
-                    attempt += 1
-                    try:
-                        await waiter.wait(
-                            ClusterId=self.job_flow_id,
-                            StepId=step_id,
-                            WaiterConfig={
-                                "Delay": int(self.poll_interval),
-                                "MaxAttempts": 1,
-                            },
-                        )
-                        break
-                    except WaiterError as error:
-                        if "terminal failure" in str(error):
-                            yield TriggerEvent(
-                                {"status": "failure", "message": f"Step {step_id} failed: {error}"}
-                            )
-                            break
-                        self.log.info(
-                            "Status of step is %s - %s",
-                            error.last_response["Step"]["Status"]["State"],
-                            error.last_response["Step"]["Status"]["StateChangeReason"],
-                        )
-                        await asyncio.sleep(int(self.poll_interval))
-        if attempt >= int(self.max_attempts):
-            yield TriggerEvent({"status": "failure", "message": "Steps failed: max attempts reached"})
-        else:
-            yield TriggerEvent({"status": "success", "message": "Steps completed", "step_ids": self.step_ids})
+            waiter = client.get_waiter(self.waiter_name)
+            await async_wait(
+                waiter=waiter,
+                waiter_delay=int(self.waiter_delay),
+                waiter_max_attempts=int(self.waiter_max_attempts),
+                args={"DBInstanceIdentifier": self.db_instance_identifier},
+                failure_message="Error checking DB Instance status",
+                status_message="DB instance status is",
+                status_args=["DBInstances[0].DBInstanceStatus"],
+            )
+        yield TriggerEvent({"status": "success", "response": self.response})
 
 
-class EmrCreateJobFlowTrigger(AwsBaseWaiterTrigger):
+_waiter_arg = {
+    RdsDbType.INSTANCE: "DBInstanceIdentifier",
+    RdsDbType.CLUSTER: "DBClusterIdentifier",
+}
+_status_paths = {
+    RdsDbType.INSTANCE: ["DBInstances[].DBInstanceStatus", "DBInstances[].StatusInfos"],
+    RdsDbType.CLUSTER: ["DBClusters[].Status"],
+}
+
+
+class RdsDbAvailableTrigger(AwsBaseWaiterTrigger):
     """
-    Asynchronously poll the boto3 API and wait for the JobFlow to finish executing.
+    Trigger to wait asynchronously for a DB instance or cluster to be available.
 
-    :param job_flow_id: The id of the job flow to wait for.
+    :param db_identifier: The DB identifier for the DB instance or cluster to be polled.
     :param waiter_delay: The amount of time in seconds to wait between attempts.
     :param waiter_max_attempts: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
+    :param region_name: AWS region where the DB is located, if different from the default one.
+    :param response: The response from the RdsHook, to be passed back to the operator.
+    :param db_type: The type of DB: instance or cluster.
     """
 
     def __init__(
         self,
-        job_flow_id: str,
-        poll_interval: int | None = None,  # deprecated
-        max_attempts: int | None = None,  # deprecated
-        aws_conn_id: str | None = None,
-        waiter_delay: int = 30,
-        waiter_max_attempts: int = 60,
-    ):
-        if poll_interval is not None or max_attempts is not None:
-            warnings.warn(
-                "please use waiter_delay instead of poll_interval "
-                "and waiter_max_attempts instead of max_attempts",
-                AirflowProviderDeprecationWarning,
-                stacklevel=2,
-            )
-            waiter_delay = poll_interval or waiter_delay
-            waiter_max_attempts = max_attempts or waiter_max_attempts
+        db_identifier: str,
+        waiter_delay: int,
+        waiter_max_attempts: int,
+        aws_conn_id: str,
+        response: dict[str, Any],
+        db_type: RdsDbType,
+        region_name: str | None = None,
+    ) -> None:
         super().__init__(
-            serialized_fields={"job_flow_id": job_flow_id},
-            waiter_name="job_flow_waiting",
-            waiter_args={"ClusterId": job_flow_id},
-            failure_message="JobFlow creation failed",
-            status_message="JobFlow creation in progress",
-            status_queries=[
-                "Cluster.Status.State",
-                "Cluster.Status.StateChangeReason",
-                "Cluster.Status.ErrorDetails",
-            ],
-            return_key="job_flow_id",
-            return_value=job_flow_id,
+            serialized_fields={
+                "db_identifier": db_identifier,
+                "response": response,
+                "db_type": db_type,
+            },
+            waiter_name=f"db_{db_type.value}_available",
+            waiter_args={_waiter_arg[db_type]: db_identifier},
+            failure_message="Error while waiting for DB to be available",
+            status_message="DB initialization in progress",
+            status_queries=_status_paths[db_type],
+            return_key="response",
+            return_value=response,
             waiter_delay=waiter_delay,
             waiter_max_attempts=waiter_max_attempts,
             aws_conn_id=aws_conn_id,
+            region_name=region_name,
         )
 
     def hook(self) -> AwsGenericHook:
-        return EmrHook(aws_conn_id=self.aws_conn_id)
+        return RdsHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
 
 
-class EmrTerminateJobFlowTrigger(AwsBaseWaiterTrigger):
+class RdsDbDeletedTrigger(AwsBaseWaiterTrigger):
     """
-    Asynchronously poll the boto3 API and wait for the JobFlow to finish terminating.
+    Trigger to wait asynchronously for a DB instance or cluster to be deleted.
 
-    :param job_flow_id: ID of the EMR Job Flow to terminate
+    :param db_identifier: The DB identifier for the DB instance or cluster to be polled.
     :param waiter_delay: The amount of time in seconds to wait between attempts.
     :param waiter_max_attempts: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
+    :param region_name: AWS region where the DB is located, if different from the default one.
+    :param response: The response from the RdsHook, to be passed back to the operator.
+    :param db_type: The type of DB: instance or cluster.
     """
 
     def __init__(
         self,
-        job_flow_id: str,
-        poll_interval: int | None = None,  # deprecated
-        max_attempts: int | None = None,  # deprecated
-        aws_conn_id: str | None = None,
-        waiter_delay: int = 30,
-        waiter_max_attempts: int = 60,
-    ):
-        if poll_interval is not None or max_attempts is not None:
-            warnings.warn(
-                "please use waiter_delay instead of poll_interval "
-                "and waiter_max_attempts instead of max_attempts",
-                AirflowProviderDeprecationWarning,
-                stacklevel=2,
-            )
-            waiter_delay = poll_interval or waiter_delay
-            waiter_max_attempts = max_attempts or waiter_max_attempts
-        super().__init__(
-            serialized_fields={"job_flow_id": job_flow_id},
-            waiter_name="job_flow_terminated",
-            waiter_args={"ClusterId": job_flow_id},
-            failure_message="JobFlow termination failed",
-            status_message="JobFlow termination in progress",
-            status_queries=[
-                "Cluster.Status.State",
-                "Cluster.Status.StateChangeReason",
-                "Cluster.Status.ErrorDetails",
-            ],
-            return_value=None,
-            waiter_delay=waiter_delay,
-            waiter_max_attempts=waiter_max_attempts,
-            aws_conn_id=aws_conn_id,
-        )
-
-    def hook(self) -> AwsGenericHook:
-        return EmrHook(aws_conn_id=self.aws_conn_id)
-
-
-class EmrContainerTrigger(AwsBaseWaiterTrigger):
-    """
-    Poll for the status of EMR container until reaches terminal state.
-
-    :param virtual_cluster_id: Reference Emr cluster id
-    :param job_id:  job_id to check the state
-    :param aws_conn_id: Reference to AWS connection id
-    :param waiter_delay: polling period in seconds to check for the status
-    """
-
-    def __init__(
-        self,
-        virtual_cluster_id: str,
-        job_id: str,
-        aws_conn_id: str = "aws_default",
-        poll_interval: int | None = None,  # deprecated
-        waiter_delay: int = 30,
-        waiter_max_attempts: int = 600,
-    ):
-        if poll_interval is not None:
-            warnings.warn(
-                "please use waiter_delay instead of poll_interval.",
-                AirflowProviderDeprecationWarning,
-                stacklevel=2,
-            )
-            waiter_delay = poll_interval or waiter_delay
+        db_identifier: str,
+        waiter_delay: int,
+        waiter_max_attempts: int,
+        aws_conn_id: str,
+        response: dict[str, Any],
+        db_type: RdsDbType,
+        region_name: str | None = None,
+    ) -> None:
         super().__init__(
-            serialized_fields={"virtual_cluster_id": virtual_cluster_id, "job_id": job_id},
-            waiter_name="container_job_complete",
-            waiter_args={"id": job_id, "virtualClusterId": virtual_cluster_id},
-            failure_message="Job failed",
-            status_message="Job in progress",
-            status_queries=["jobRun.state", "jobRun.failureReason"],
-            return_key="job_id",
-            return_value=job_id,
+            serialized_fields={
+                "db_identifier": db_identifier,
+                "response": response,
+                "db_type": db_type,
+            },
+            waiter_name=f"db_{db_type.value}_deleted",
+            waiter_args={_waiter_arg[db_type]: db_identifier},
+            failure_message="Error while deleting DB",
+            status_message="DB deletion in progress",
+            status_queries=_status_paths[db_type],
+            return_key="response",
+            return_value=response,
             waiter_delay=waiter_delay,
             waiter_max_attempts=waiter_max_attempts,
             aws_conn_id=aws_conn_id,
+            region_name=region_name,
         )
 
     def hook(self) -> AwsGenericHook:
-        return EmrContainerHook(self.aws_conn_id)
+        return RdsHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
 
 
-class EmrStepSensorTrigger(AwsBaseWaiterTrigger):
+class RdsDbStoppedTrigger(AwsBaseWaiterTrigger):
     """
-    Poll for the status of EMR container until reaches terminal state.
+    Trigger to wait asynchronously for a DB instance or cluster to be stopped.
 
-    :param job_flow_id: job_flow_id which contains the step check the state of
-    :param step_id:  step to check the state of
-    :param waiter_delay: polling period in seconds to check for the status
-    :param waiter_max_attempts: The maximum number of attempts to be made
-    :param aws_conn_id: Reference to AWS connection id
+    :param db_identifier: The DB identifier for the DB instance or cluster to be polled.
+    :param waiter_delay: The amount of time in seconds to wait between attempts.
+    :param waiter_max_attempts: The maximum number of attempts to be made.
+    :param aws_conn_id: The Airflow connection used for AWS credentials.
+    :param region_name: AWS region where the DB is located, if different from the default one.
+    :param response: The response from the RdsHook, to be passed back to the operator.
+    :param db_type: The type of DB: instance or cluster.
     """
 
     def __init__(
         self,
-        job_flow_id: str,
-        step_id: str,
-        waiter_delay: int = 30,
-        waiter_max_attempts: int = 60,
-        aws_conn_id: str = "aws_default",
-    ):
+        db_identifier: str,
+        waiter_delay: int,
+        waiter_max_attempts: int,
+        aws_conn_id: str,
+        response: dict[str, Any],
+        db_type: RdsDbType,
+        region_name: str | None = None,
+    ) -> None:
         super().__init__(
-            serialized_fields={"job_flow_id": job_flow_id, "step_id": step_id},
-            waiter_name="step_wait_for_terminal",
-            waiter_args={"ClusterId": job_flow_id, "StepId": step_id},
-            failure_message=f"Error while waiting for step {step_id} to complete",
-            status_message=f"Step id: {step_id}, Step is still in non-terminal state",
-            status_queries=[
-                "Step.Status.State",
-                "Step.Status.FailureDetails",
-                "Step.Status.StateChangeReason",
-            ],
-            return_value=None,
+            serialized_fields={
+                "db_identifier": db_identifier,
+                "response": response,
+                "db_type": db_type,
+            },
+            waiter_name=f"db_{db_type.value}_stopped",
+            waiter_args={_waiter_arg[db_type]: db_identifier},
+            failure_message="Error while stopping DB",
+            status_message="DB is being stopped",
+            status_queries=_status_paths[db_type],
+            return_key="response",
+            return_value=response,
             waiter_delay=waiter_delay,
             waiter_max_attempts=waiter_max_attempts,
             aws_conn_id=aws_conn_id,
+            region_name=region_name,
         )
 
     def hook(self) -> AwsGenericHook:
-        return EmrHook(self.aws_conn_id)
+        return RdsHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/glue.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/triggers/s3.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/eks_get_token.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/emailer.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/rds.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/rds.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 
 from enum import Enum
 
 
 class RdsDbType(Enum):
     """Only available types for the RDS."""
 
-    INSTANCE: str = "instance"
-    CLUSTER: str = "cluster"
+    INSTANCE = "instance"
+    CLUSTER = "cluster"
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/redshift.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/sagemaker.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/tags.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/tags.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/waiter.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/__init__.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/appflow.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/appflow.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/athena.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/athena.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/base_waiter.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/batch.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/batch.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/dynamodb.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/ecs.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/ecs.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/eks.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/eks.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/emr-containers.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/emr-containers.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/emr.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/emr.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/glue.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/glue.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/redshift.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/redshift.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/aws/waiters/sagemaker.json` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'waiters'": "{'PipelineExecutionComplete': OrderedDict([('delay', 30), ('operation', "*

 * *              "'DescribePipelineExecution'), ('maxAttempts', 60), ('description', 'Wait until "*

 * *              "pipeline execution is Succeeded'), ('acceptors', [OrderedDict([('matcher', 'path'), "*

 * *              "('argument', 'PipelineExecutionStatus'), ('expected', 'Succeeded'), ('state', "*

 * *              "'success')]), OrderedDict([('matcher', 'path'), ('argument', "*

 * *              "'PipelineExecutionStatus'), ('expected […]*

```diff
@@ -1,10 +1,56 @@
 {
     "version": 2,
     "waiters": {
+        "PipelineExecutionComplete": {
+            "acceptors": [
+                {
+                    "argument": "PipelineExecutionStatus",
+                    "expected": "Succeeded",
+                    "matcher": "path",
+                    "state": "success"
+                },
+                {
+                    "argument": "PipelineExecutionStatus",
+                    "expected": "Failed",
+                    "matcher": "path",
+                    "state": "failure"
+                },
+                {
+                    "argument": "PipelineExecutionStatus",
+                    "expected": "Stopped",
+                    "matcher": "path",
+                    "state": "failure"
+                }
+            ],
+            "delay": 30,
+            "description": "Wait until pipeline execution is Succeeded",
+            "maxAttempts": 60,
+            "operation": "DescribePipelineExecution"
+        },
+        "PipelineExecutionStopped": {
+            "acceptors": [
+                {
+                    "argument": "PipelineExecutionStatus",
+                    "expected": "Stopped",
+                    "matcher": "path",
+                    "state": "success"
+                },
+                {
+                    "argument": "PipelineExecutionStatus",
+                    "expected": "Failed",
+                    "matcher": "path",
+                    "state": "failure"
+                }
+            ],
+            "delay": 10,
+            "description": "Wait until pipeline execution is Stopped",
+            "maxAttempts": 120,
+            "operation": "DescribePipelineExecution"
+        },
         "ProcessingJobComplete": {
             "acceptors": [
                 {
                     "argument": "ProcessingJobStatus",
                     "expected": "Completed",
                     "matcher": "path",
                     "state": "success"
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/airflow/providers/amazon/get_provider_info.py` & `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-amazon",
         "name": "Amazon",
         "description": "Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).\n",
         "suspended": False,
         "versions": [
+            "8.4.0",
             "8.3.1",
             "8.3.0",
             "8.2.0",
             "8.1.0",
             "8.0.0",
             "7.4.1",
             "7.4.0",
@@ -74,15 +75,15 @@
             "asgiref",
             "watchtower~=2.0.1",
             "jsonpath_ng>=1.5.3",
             "redshift_connector>=2.0.888",
             "sqlalchemy_redshift>=0.8.6",
             "mypy-boto3-rds>=1.24.0",
             "mypy-boto3-redshift-data>=1.24.0",
-            "mypy-boto3-appflow>=1.24.0",
+            "mypy-boto3-appflow>=1.24.0,<1.28.12",
             "asgiref",
             "mypy-boto3-s3>=1.24.0",
         ],
         "integrations": [
             {
                 "integration-name": "Amazon Athena",
                 "external-doc-url": "https://aws.amazon.com/athena/",
@@ -172,14 +173,21 @@
                 "integration-name": "Amazon EMR Serverless",
                 "external-doc-url": "https://docs.aws.amazon.com/emr/latest/EMR-Serverless-UserGuide/emr-serverless.html",
                 "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/emr/emr_serverless.rst"],
                 "logo": "/integration-logos/aws/Amazon-EMR_light-bg@4x.png",
                 "tags": ["aws"],
             },
             {
+                "integration-name": "Amazon EventBridge",
+                "external-doc-url": "https://docs.aws.amazon.com/eventbridge/latest/APIReference/Welcome.html",
+                "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/eventbridge.rst"],
+                "logo": "/integration-logos/aws/Amazon-EventBridge_64.png",
+                "tags": ["aws"],
+            },
+            {
                 "integration-name": "Amazon Glacier",
                 "external-doc-url": "https://aws.amazon.com/glacier/",
                 "logo": "/integration-logos/aws/Amazon-S3-Glacier_light-bg@4x.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/s3/glacier.rst"],
                 "tags": ["aws"],
             },
             {
@@ -367,14 +375,18 @@
                 "python-modules": ["airflow.providers.amazon.aws.operators.emr"],
             },
             {
                 "integration-name": "Amazon EMR on EKS",
                 "python-modules": ["airflow.providers.amazon.aws.operators.emr"],
             },
             {
+                "integration-name": "Amazon EventBridge",
+                "python-modules": ["airflow.providers.amazon.aws.operators.eventbridge"],
+            },
+            {
                 "integration-name": "Amazon Glacier",
                 "python-modules": ["airflow.providers.amazon.aws.operators.glacier"],
             },
             {
                 "integration-name": "AWS Glue",
                 "python-modules": [
                     "airflow.providers.amazon.aws.operators.glue",
@@ -563,14 +575,18 @@
             },
             {"integration-name": "Amazon EMR", "python-modules": ["airflow.providers.amazon.aws.hooks.emr"]},
             {
                 "integration-name": "Amazon EMR on EKS",
                 "python-modules": ["airflow.providers.amazon.aws.hooks.emr"],
             },
             {
+                "integration-name": "Amazon EventBridge",
+                "python-modules": ["airflow.providers.amazon.aws.hooks.eventbridge"],
+            },
+            {
                 "integration-name": "Amazon Glacier",
                 "python-modules": ["airflow.providers.amazon.aws.hooks.glacier"],
             },
             {
                 "integration-name": "AWS Glue",
                 "python-modules": [
                     "airflow.providers.amazon.aws.hooks.glue",
@@ -692,14 +708,18 @@
                 "integration-name": "Amazon ECS",
                 "python-modules": ["airflow.providers.amazon.aws.triggers.ecs"],
             },
             {
                 "integration-name": "Amazon RDS",
                 "python-modules": ["airflow.providers.amazon.aws.triggers.rds"],
             },
+            {
+                "integration-name": "AWS Step Functions",
+                "python-modules": ["airflow.providers.amazon.aws.triggers.step_function"],
+            },
         ],
         "transfers": [
             {
                 "source-integration-name": "Amazon DynamoDB",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
                 "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/dynamodb_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.dynamodb_to_s3",
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO` & `apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.3.1rc1
+Version: 8.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -80,60 +80,60 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.3.1rc1``
+Release: ``8.4.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-amazon``
 
 The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
-=======================================  ==================
+=======================================  =====================
 PIP package                              Version required
-=======================================  ==================
+=======================================  =====================
 ``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``apache-airflow-providers-http``
 ``boto3``                                ``>=1.24.0``
 ``asgiref``
 ``watchtower``                           ``~=2.0.1``
 ``jsonpath_ng``                          ``>=1.5.3``
 ``redshift_connector``                   ``>=2.0.888``
 ``sqlalchemy_redshift``                  ``>=0.8.6``
 ``mypy-boto3-rds``                       ``>=1.24.0``
 ``mypy-boto3-redshift-data``             ``>=1.24.0``
-``mypy-boto3-appflow``                   ``>=1.24.0``
+``mypy-boto3-appflow``                   ``>=1.24.0,<1.28.12``
 ``asgiref``
 ``mypy-boto3-s3``                        ``>=1.24.0``
-=======================================  ==================
+=======================================  =====================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
 
@@ -158,8 +158,8 @@
 `apache-airflow-providers-microsoft-azure <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure>`_  ``microsoft.azure``
 `apache-airflow-providers-mongo <https://airflow.apache.org/docs/apache-airflow-providers-mongo>`_                      ``mongo``
 `apache-airflow-providers-salesforce <https://airflow.apache.org/docs/apache-airflow-providers-salesforce>`_            ``salesforce``
 `apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                          ``ssh``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt` & `apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 airflow/providers/amazon/aws/hooks/dynamodb.py
 airflow/providers/amazon/aws/hooks/ec2.py
 airflow/providers/amazon/aws/hooks/ecr.py
 airflow/providers/amazon/aws/hooks/ecs.py
 airflow/providers/amazon/aws/hooks/eks.py
 airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
 airflow/providers/amazon/aws/hooks/emr.py
+airflow/providers/amazon/aws/hooks/eventbridge.py
 airflow/providers/amazon/aws/hooks/glacier.py
 airflow/providers/amazon/aws/hooks/glue.py
 airflow/providers/amazon/aws/hooks/glue_catalog.py
 airflow/providers/amazon/aws/hooks/glue_crawler.py
 airflow/providers/amazon/aws/hooks/kinesis.py
 airflow/providers/amazon/aws/hooks/lambda_function.py
 airflow/providers/amazon/aws/hooks/logs.py
@@ -66,14 +67,15 @@
 airflow/providers/amazon/aws/operators/cloud_formation.py
 airflow/providers/amazon/aws/operators/datasync.py
 airflow/providers/amazon/aws/operators/dms.py
 airflow/providers/amazon/aws/operators/ec2.py
 airflow/providers/amazon/aws/operators/ecs.py
 airflow/providers/amazon/aws/operators/eks.py
 airflow/providers/amazon/aws/operators/emr.py
+airflow/providers/amazon/aws/operators/eventbridge.py
 airflow/providers/amazon/aws/operators/glacier.py
 airflow/providers/amazon/aws/operators/glue.py
 airflow/providers/amazon/aws/operators/glue_crawler.py
 airflow/providers/amazon/aws/operators/lambda_function.py
 airflow/providers/amazon/aws/operators/quicksight.py
 airflow/providers/amazon/aws/operators/rds.py
 airflow/providers/amazon/aws/operators/redshift_cluster.py
@@ -139,14 +141,15 @@
 airflow/providers/amazon/aws/triggers/emr.py
 airflow/providers/amazon/aws/triggers/glue.py
 airflow/providers/amazon/aws/triggers/glue_crawler.py
 airflow/providers/amazon/aws/triggers/rds.py
 airflow/providers/amazon/aws/triggers/redshift_cluster.py
 airflow/providers/amazon/aws/triggers/s3.py
 airflow/providers/amazon/aws/triggers/sagemaker.py
+airflow/providers/amazon/aws/triggers/step_function.py
 airflow/providers/amazon/aws/utils/__init__.py
 airflow/providers/amazon/aws/utils/connection_wrapper.py
 airflow/providers/amazon/aws/utils/eks_get_token.py
 airflow/providers/amazon/aws/utils/emailer.py
 airflow/providers/amazon/aws/utils/rds.py
 airflow/providers/amazon/aws/utils/redshift.py
 airflow/providers/amazon/aws/utils/sagemaker.py
@@ -164,14 +167,15 @@
 airflow/providers/amazon/aws/waiters/eks.json
 airflow/providers/amazon/aws/waiters/emr-containers.json
 airflow/providers/amazon/aws/waiters/emr-serverless.json
 airflow/providers/amazon/aws/waiters/emr.json
 airflow/providers/amazon/aws/waiters/glue.json
 airflow/providers/amazon/aws/waiters/redshift.json
 airflow/providers/amazon/aws/waiters/sagemaker.json
+airflow/providers/amazon/aws/waiters/stepfunctions.json
 apache_airflow_providers_amazon.egg-info/PKG-INFO
 apache_airflow_providers_amazon.egg-info/SOURCES.txt
 apache_airflow_providers_amazon.egg-info/dependency_links.txt
 apache_airflow_providers_amazon.egg-info/entry_points.txt
 apache_airflow_providers_amazon.egg-info/not-zip-safe
 apache_airflow_providers_amazon.egg-info/requires.txt
 apache_airflow_providers_amazon.egg-info/top_level.txt
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/apache_airflow_providers_amazon.egg-info/requires.txt` & `apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 apache-airflow-providers-common-sql>=1.3.1.dev0
 apache-airflow-providers-http
 apache-airflow>=2.4.0.dev0
 asgiref
 asgiref
 boto3>=1.24.0
 jsonpath_ng>=1.5.3
-mypy-boto3-appflow>=1.24.0
+mypy-boto3-appflow<1.28.12,>=1.24.0
 mypy-boto3-rds>=1.24.0
 mypy-boto3-redshift-data>=1.24.0
 mypy-boto3-s3>=1.24.0
 redshift_connector>=2.0.888
 sqlalchemy_redshift>=0.8.6
 watchtower~=2.0.1
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/pyproject.toml` & `apache-airflow-providers-amazon-8.4.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 extend-exclude = [
     ".eggs",
     "airflow/_vendor/*",
     "airflow/providers/google/ads/_vendor/*",
     # The files generated by stubgen aren't 100% valid syntax it turns out, and we don't ship them, so we can
     # ignore them in ruff
     "airflow/providers/common/sql/*/*.pyi",
-    "airflow/migrations/versions/*.py"
+    "airflow/migrations/versions/*.py",
+    "tests/dags/test_imports.py",
 ]
 
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
@@ -69,14 +70,16 @@
     "D212",
     "D213",
     "D214",
     "D215",
     "E731",
 ]
 
+namespace-packages = ["airflow/providers"]
+
 [tool.pytest.ini_options]
 # * Disable `flaky` plugin for pytest. This plugin conflicts with `rerunfailures` because provide same marker.
 # * Disable `nose` builtin plugin for pytest. This feature deprecated in 7.2 and will be removed in pytest>=8
 # * And we focus on use native pytest capabilities rather than adopt another frameworks.
 addopts = "-rasl --verbosity=2 -p no:flaky -p no:nose --asyncio-mode=strict"
 norecursedirs = [
     ".eggs",
@@ -95,54 +98,28 @@
     "ignore::DeprecationWarning:flask_appbuilder.widgets",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
     "ignore::DeprecationWarning:flask_sqlalchemy",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
     "ignore::DeprecationWarning:apispec.utils",
 ]
 python_files = [
-    "*.py",
+    "test_*.py",
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff.isort]
-known-first-party = ["airflow", "airflow_breeze", "docker_tests", "docs", "kubernetes_tests", "tests"]
 required-imports = ["from __future__ import annotations"]
 combine-as-imports = true
 
-# TODO: for now, https://github.com/charliermarsh/ruff/issues/1817
-known-third-party = [
-    "asana",
-    "atlassian",
-    "celery",
-    "cloudant",
-    "databricks",
-    "datadog",
-    "docker",
-    "elasticsearch",
-    "github",
-    "google",
-    "grpc",
-    "jenkins",
-    "mysql",
-    "neo4j",
-    "papermill",
-    "redis",
-    "sendgrid",
-    "snowflake",
-    "telegram",
-    "trino",
-]
-
 [tool.ruff.per-file-ignores]
 "airflow/models/__init__.py" = ["F401"]
 "airflow/models/sqla_models.py" = ["F401"]
 
-
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
 # The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
 # when __future__.annotations is used so we need to skip them from upgrading
 "airflow/serialization/pydantic/*.py" = ["I002"]
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/setup.cfg` & `apache-airflow-providers-amazon-8.4.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.3.1/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -50,15 +50,15 @@
 	apache-airflow-providers-common-sql>=1.3.1.dev0
 	apache-airflow-providers-http
 	apache-airflow>=2.4.0.dev0
 	asgiref
 	asgiref
 	boto3>=1.24.0
 	jsonpath_ng>=1.5.3
-	mypy-boto3-appflow>=1.24.0
+	mypy-boto3-appflow>=1.24.0,<1.28.12
 	mypy-boto3-rds>=1.24.0
 	mypy-boto3-redshift-data>=1.24.0
 	mypy-boto3-s3>=1.24.0
 	redshift_connector>=2.0.888
 	sqlalchemy_redshift>=0.8.6
 	watchtower~=2.0.1
```

### Comparing `apache-airflow-providers-amazon-8.3.1rc1/setup.py` & `apache-airflow-providers-amazon-8.4.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-amazon package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "8.3.1"
+version = "8.4.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-amazon setup."""
     setup(
         version=version,
         extras_require={
```

