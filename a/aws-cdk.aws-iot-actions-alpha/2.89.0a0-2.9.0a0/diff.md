# Comparing `tmp/aws-cdk.aws-iot-actions-alpha-2.89.0a0.tar.gz` & `tmp/aws-cdk.aws-iot-actions-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src2022765760/src/packages/@aws-cdk/aws-iot-actions-alpha/dist/python/aws-cdk.aws-iot-actions-alpha-2.89.0a0.", last modified: Fri Jul 28 22:06:01 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-iot-actions/dist/python/aws-cdk.aws-iot-actions-alpha-2.9.0", last modified: Wed Jan 26 11:22:21 2022, max compression
```

## Comparing `aws-cdk.aws-iot-actions-alpha-2.89.0a0.tar` & `aws-cdk.aws-iot-actions-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-07-28 22:05:56.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 22:05:56.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1382 2023-07-28 22:05:56.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12008 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11013 2023-07-28 22:05:56.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-28 22:05:56.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2103 2023-07-28 22:05:56.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk/aws_iot_actions_alpha/
--rw-r--r--   0 root         (0) root         (0)   115264 2023-07-28 22:05:56.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk/aws_iot_actions_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-28 22:05:56.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80814 2023-07-28 22:05:55.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/aws-iot-actions-alpha@2.89.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:05:56.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk/aws_iot_actions_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12008 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      279 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-28 22:06:01.000000 aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:18.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:18.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1382 2022-01-26 11:22:18.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8235 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7273 2022-01-26 11:22:18.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:18.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1907 2022-01-26 11:22:18.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk/aws_iot_actions_alpha/
+-rw-r--r--   0 root         (0) root         (0)    54651 2022-01-26 11:22:18.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk/aws_iot_actions_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      495 2022-01-26 11:22:18.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51843 2022-01-26 11:22:18.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/aws-iot-actions-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:18.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk/aws_iot_actions_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8235 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      570 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:21.000000 aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-iot-actions-alpha-2.89.0a0/LICENSE` & `aws-cdk.aws-iot-actions-alpha-2.9.0a0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2018-2023 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+   Copyright 2018-2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `aws-cdk.aws-iot-actions-alpha-2.89.0a0/NOTICE` & `aws-cdk.aws-iot-actions-alpha-2.9.0a0/NOTICE`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 AWS Cloud Development Kit (AWS CDK)
-Copyright 2018-2023 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+Copyright 2018-2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
 -------------------------------------------------------------------------------
 
 The AWS CDK includes the following third-party software/licensing:
 
 ** case - https://www.npmjs.com/package/case
 Copyright (c) 2013 Nathan Bubna
```

### Comparing `aws-cdk.aws-iot-actions-alpha-2.89.0a0/PKG-INFO` & `aws-cdk.aws-iot-actions-alpha-2.9.0a0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-iot-actions-alpha
-Version: 2.89.0a0
+Version: 2.9.0a0
 Summary: Receipt rule actions for AWS IoT
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: Framework :: AWS CDK
-Classifier: Framework :: AWS CDK :: 2
-Requires-Python: ~=3.7
+Classifier: Framework :: AWS CDK :: 1
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Actions for AWS IoT Rule
 
 <!--BEGIN STABILITY BANNER-->---
@@ -43,43 +43,22 @@
 
 This library contains integration classes to send data to any number of
 supported AWS Services. Instances of these classes should be passed to
 `TopicRule` defined in `@aws-cdk/aws-iot`.
 
 Currently supported are:
 
-* Republish a message to another MQTT topic
 * Invoke a Lambda function
 * Put objects to a S3 bucket
 * Put logs to CloudWatch Logs
 * Capture CloudWatch metrics
 * Change state for a CloudWatch alarm
 * Put records to Kinesis Data stream
 * Put records to Kinesis Data Firehose stream
 * Send messages to SQS queues
-* Publish messages on SNS topics
-* Write messages into columns of DynamoDB
-* Put messages IoT Events input
-* Send messages to HTTPS endpoints
-
-## Republish a message to another MQTT topic
-
-The code snippet below creates an AWS IoT Rule that republish a message to
-another MQTT topic when it is triggered.
-
-```python
-iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, timestamp() as timestamp, temperature FROM 'device/+/data'"),
-    actions=[
-        actions.IotRepublishMqttAction("${topic()}/republish",
-            quality_of_service=actions.MqttQualityOfService.AT_LEAST_ONCE
-        )
-    ]
-)
-```
 
 ## Invoke a Lambda function
 
 The code snippet below creates an AWS IoT Rule that invoke a Lambda function
 when it is triggered.
 
 ```python
@@ -96,15 +75,15 @@
     sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, timestamp() as timestamp, temperature FROM 'device/+/data'"),
     actions=[actions.LambdaFunctionAction(func)]
 )
 ```
 
 ## Put objects to a S3 bucket
 
-The code snippet below creates an AWS IoT Rule that puts objects to a S3 bucket
+The code snippet below creates an AWS IoT Rule that put objects to a S3 bucket
 when it is triggered.
 
 ```python
 bucket = s3.Bucket(self, "MyBucket")
 
 iot.TopicRule(self, "TopicRule",
     sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id FROM 'device/+/data'"),
@@ -147,15 +126,15 @@
         )
     ]
 )
 ```
 
 ## Put logs to CloudWatch Logs
 
-The code snippet below creates an AWS IoT Rule that puts logs to CloudWatch Logs
+The code snippet below creates an AWS IoT Rule that put logs to CloudWatch Logs
 when it is triggered.
 
 ```python
 import aws_cdk.aws_logs as logs
 
 
 log_group = logs.LogGroup(self, "MyLogGroup")
@@ -182,32 +161,14 @@
             metric_value="${value}",
             metric_timestamp="${timestamp}"
         )
     ]
 )
 ```
 
-## Start Step Functions State Machine
-
-The code snippet below creates an AWS IoT Rule that starts a Step Functions State Machine
-when it is triggered.
-
-```python
-state_machine = stepfunctions.StateMachine(self, "SM",
-    definition_body=stepfunctions.DefinitionBody.from_chainable(stepfunctions.Wait(self, "Hello", time=stepfunctions.WaitTime.duration(Duration.seconds(10))))
-)
-
-iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
-    actions=[
-        actions.StepFunctionsStateMachineAction(state_machine)
-    ]
-)
-```
-
 ## Change the state of an Amazon CloudWatch alarm
 
 The code snippet below creates an AWS IoT Rule that changes the state of an Amazon CloudWatch alarm when it is triggered:
 
 ```python
 import aws_cdk.aws_cloudwatch as cloudwatch
 
@@ -233,15 +194,15 @@
         )
     ]
 )
 ```
 
 ## Put records to Kinesis Data stream
 
-The code snippet below creates an AWS IoT Rule that puts records to Kinesis Data
+The code snippet below creates an AWS IoT Rule that put records to Kinesis Data
 stream when it is triggered.
 
 ```python
 import aws_cdk.aws_kinesis as kinesis
 
 
 stream = kinesis.Stream(self, "MyStream")
@@ -254,15 +215,15 @@
         )
     ]
 )
 ```
 
 ## Put records to Kinesis Data Firehose stream
 
-The code snippet below creates an AWS IoT Rule that puts records to Put records
+The code snippet below creates an AWS IoT Rule that put records to Put records
 to Kinesis Data Firehose stream when it is triggered.
 
 ```python
 import aws_cdk.aws_kinesisfirehose_alpha as firehose
 import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
 
 
@@ -299,91 +260,8 @@
         actions.SqsQueueAction(queue,
             use_base64=True
         )
     ]
 )
 ```
 
-## Publish messages on an SNS topic
-
-The code snippet below creates and AWS IoT Rule that publishes messages to an SNS topic when it is triggered:
-
-```python
-import aws_cdk.aws_sns as sns
-
-
-topic = sns.Topic(self, "MyTopic")
-
-topic_rule = iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, year, month, day FROM 'device/+/data'"),
-    actions=[
-        actions.SnsTopicAction(topic,
-            message_format=actions.SnsActionMessageFormat.JSON
-        )
-    ]
-)
-```
-
-## Write attributes of a message to DynamoDB
-
-The code snippet below creates an AWS IoT rule that writes all or part of an
-MQTT message to DynamoDB using the DynamoDBv2 action.
-
-```python
-import aws_cdk.aws_dynamodb as dynamodb
-
-# table: dynamodb.Table
-
-
-topic_rule = iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
-    actions=[
-        actions.DynamoDBv2PutItemAction(table)
-    ]
-)
-```
-
-## Put messages IoT Events input
-
-The code snippet below creates an AWS IoT Rule that puts messages
-to an IoT Events input when it is triggered:
-
-```python
-import aws_cdk.aws_iotevents_alpha as iotevents
-import aws_cdk.aws_iam as iam
-
-# role: iam.IRole
-
-
-input = iotevents.Input(self, "MyInput",
-    attribute_json_paths=["payload.temperature", "payload.transactionId"]
-)
-topic_rule = iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
-    actions=[
-        actions.IotEventsPutMessageAction(input,
-            batch_mode=True,  # optional property, default is 'false'
-            message_id="${payload.transactionId}",  # optional property, default is a new UUID
-            role=role
-        )
-    ]
-)
-```
-
-## Send Messages to HTTPS Endpoints
 
-The code snippet below creates an AWS IoT Rule that sends messages
-to an HTTPS endpoint when it is triggered:
-
-```python
-topic_rule = iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, year, month, day FROM 'device/+/data'")
-)
-
-topic_rule.add_action(
-    actions.HttpsAction("https://example.com/endpoint",
-        confirmation_url="https://example.com",
-        headers=[actions.HttpActionHeader(key="key0", value="value0"), actions.HttpActionHeader(key="key1", value="value1")
-        ],
-        auth=actions.HttpActionSigV4Auth(service_name="serviceName", signing_region="us-east-1")
-    ))
-```
```

### Comparing `aws-cdk.aws-iot-actions-alpha-2.89.0a0/README.md` & `aws-cdk.aws-iot-actions-alpha-2.9.0a0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -16,43 +16,22 @@
 
 This library contains integration classes to send data to any number of
 supported AWS Services. Instances of these classes should be passed to
 `TopicRule` defined in `@aws-cdk/aws-iot`.
 
 Currently supported are:
 
-* Republish a message to another MQTT topic
 * Invoke a Lambda function
 * Put objects to a S3 bucket
 * Put logs to CloudWatch Logs
 * Capture CloudWatch metrics
 * Change state for a CloudWatch alarm
 * Put records to Kinesis Data stream
 * Put records to Kinesis Data Firehose stream
 * Send messages to SQS queues
-* Publish messages on SNS topics
-* Write messages into columns of DynamoDB
-* Put messages IoT Events input
-* Send messages to HTTPS endpoints
-
-## Republish a message to another MQTT topic
-
-The code snippet below creates an AWS IoT Rule that republish a message to
-another MQTT topic when it is triggered.
-
-```python
-iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, timestamp() as timestamp, temperature FROM 'device/+/data'"),
-    actions=[
-        actions.IotRepublishMqttAction("${topic()}/republish",
-            quality_of_service=actions.MqttQualityOfService.AT_LEAST_ONCE
-        )
-    ]
-)
-```
 
 ## Invoke a Lambda function
 
 The code snippet below creates an AWS IoT Rule that invoke a Lambda function
 when it is triggered.
 
 ```python
@@ -69,15 +48,15 @@
     sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, timestamp() as timestamp, temperature FROM 'device/+/data'"),
     actions=[actions.LambdaFunctionAction(func)]
 )
 ```
 
 ## Put objects to a S3 bucket
 
-The code snippet below creates an AWS IoT Rule that puts objects to a S3 bucket
+The code snippet below creates an AWS IoT Rule that put objects to a S3 bucket
 when it is triggered.
 
 ```python
 bucket = s3.Bucket(self, "MyBucket")
 
 iot.TopicRule(self, "TopicRule",
     sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id FROM 'device/+/data'"),
@@ -120,15 +99,15 @@
         )
     ]
 )
 ```
 
 ## Put logs to CloudWatch Logs
 
-The code snippet below creates an AWS IoT Rule that puts logs to CloudWatch Logs
+The code snippet below creates an AWS IoT Rule that put logs to CloudWatch Logs
 when it is triggered.
 
 ```python
 import aws_cdk.aws_logs as logs
 
 
 log_group = logs.LogGroup(self, "MyLogGroup")
@@ -155,32 +134,14 @@
             metric_value="${value}",
             metric_timestamp="${timestamp}"
         )
     ]
 )
 ```
 
-## Start Step Functions State Machine
-
-The code snippet below creates an AWS IoT Rule that starts a Step Functions State Machine
-when it is triggered.
-
-```python
-state_machine = stepfunctions.StateMachine(self, "SM",
-    definition_body=stepfunctions.DefinitionBody.from_chainable(stepfunctions.Wait(self, "Hello", time=stepfunctions.WaitTime.duration(Duration.seconds(10))))
-)
-
-iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
-    actions=[
-        actions.StepFunctionsStateMachineAction(state_machine)
-    ]
-)
-```
-
 ## Change the state of an Amazon CloudWatch alarm
 
 The code snippet below creates an AWS IoT Rule that changes the state of an Amazon CloudWatch alarm when it is triggered:
 
 ```python
 import aws_cdk.aws_cloudwatch as cloudwatch
 
@@ -206,15 +167,15 @@
         )
     ]
 )
 ```
 
 ## Put records to Kinesis Data stream
 
-The code snippet below creates an AWS IoT Rule that puts records to Kinesis Data
+The code snippet below creates an AWS IoT Rule that put records to Kinesis Data
 stream when it is triggered.
 
 ```python
 import aws_cdk.aws_kinesis as kinesis
 
 
 stream = kinesis.Stream(self, "MyStream")
@@ -227,15 +188,15 @@
         )
     ]
 )
 ```
 
 ## Put records to Kinesis Data Firehose stream
 
-The code snippet below creates an AWS IoT Rule that puts records to Put records
+The code snippet below creates an AWS IoT Rule that put records to Put records
 to Kinesis Data Firehose stream when it is triggered.
 
 ```python
 import aws_cdk.aws_kinesisfirehose_alpha as firehose
 import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
 
 
@@ -271,92 +232,7 @@
     actions=[
         actions.SqsQueueAction(queue,
             use_base64=True
         )
     ]
 )
 ```
-
-## Publish messages on an SNS topic
-
-The code snippet below creates and AWS IoT Rule that publishes messages to an SNS topic when it is triggered:
-
-```python
-import aws_cdk.aws_sns as sns
-
-
-topic = sns.Topic(self, "MyTopic")
-
-topic_rule = iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, year, month, day FROM 'device/+/data'"),
-    actions=[
-        actions.SnsTopicAction(topic,
-            message_format=actions.SnsActionMessageFormat.JSON
-        )
-    ]
-)
-```
-
-## Write attributes of a message to DynamoDB
-
-The code snippet below creates an AWS IoT rule that writes all or part of an
-MQTT message to DynamoDB using the DynamoDBv2 action.
-
-```python
-import aws_cdk.aws_dynamodb as dynamodb
-
-# table: dynamodb.Table
-
-
-topic_rule = iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
-    actions=[
-        actions.DynamoDBv2PutItemAction(table)
-    ]
-)
-```
-
-## Put messages IoT Events input
-
-The code snippet below creates an AWS IoT Rule that puts messages
-to an IoT Events input when it is triggered:
-
-```python
-import aws_cdk.aws_iotevents_alpha as iotevents
-import aws_cdk.aws_iam as iam
-
-# role: iam.IRole
-
-
-input = iotevents.Input(self, "MyInput",
-    attribute_json_paths=["payload.temperature", "payload.transactionId"]
-)
-topic_rule = iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
-    actions=[
-        actions.IotEventsPutMessageAction(input,
-            batch_mode=True,  # optional property, default is 'false'
-            message_id="${payload.transactionId}",  # optional property, default is a new UUID
-            role=role
-        )
-    ]
-)
-```
-
-## Send Messages to HTTPS Endpoints
-
-The code snippet below creates an AWS IoT Rule that sends messages
-to an HTTPS endpoint when it is triggered:
-
-```python
-topic_rule = iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, year, month, day FROM 'device/+/data'")
-)
-
-topic_rule.add_action(
-    actions.HttpsAction("https://example.com/endpoint",
-        confirmation_url="https://example.com",
-        headers=[actions.HttpActionHeader(key="key0", value="value0"), actions.HttpActionHeader(key="key1", value="value1")
-        ],
-        auth=actions.HttpActionSigV4Auth(service_name="serviceName", signing_region="us-east-1")
-    ))
-```
```

### Comparing `aws-cdk.aws-iot-actions-alpha-2.89.0a0/setup.py` & `aws-cdk.aws-iot-actions-alpha-2.9.0a0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-iot-actions-alpha",
-    "version": "2.89.0.a0",
+    "version": "2.9.0.a0",
     "description": "Receipt rule actions for AWS IoT",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,47 +22,43 @@
     },
     "packages": [
         "aws_cdk.aws_iot_actions_alpha",
         "aws_cdk.aws_iot_actions_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_iot_actions_alpha._jsii": [
-            "aws-iot-actions-alpha@2.89.0-alpha.0.jsii.tgz"
+            "aws-iot-actions-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_iot_actions_alpha": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk-lib==2.89.0",
-        "aws-cdk.aws-iot-alpha==2.89.0.a0",
-        "aws-cdk.aws-iotevents-alpha==2.89.0.a0",
-        "aws-cdk.aws-kinesisfirehose-alpha==2.89.0.a0",
-        "aws-cdk.aws-kinesisfirehose-destinations-alpha==2.89.0.a0",
+        "aws-cdk-lib>=2.9.0, <3.0.0",
+        "aws-cdk.aws-iot-alpha==2.9.0.a0",
+        "aws-cdk.aws-kinesisfirehose-alpha==2.9.0.a0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.85.0, <2.0.0",
-        "publication>=0.0.3",
-        "typeguard~=2.13.3"
+        "jsii>=1.52.1, <2.0.0",
+        "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved",
         "Framework :: AWS CDK",
-        "Framework :: AWS CDK :: 2"
+        "Framework :: AWS CDK :: 1"
     ],
     "scripts": []
 }
 """
 )
 
 with open("README.md", encoding="utf8") as fp:
```

### Comparing `aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-iot-actions-alpha
-Version: 2.89.0a0
+Version: 2.9.0a0
 Summary: Receipt rule actions for AWS IoT
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: Framework :: AWS CDK
-Classifier: Framework :: AWS CDK :: 2
-Requires-Python: ~=3.7
+Classifier: Framework :: AWS CDK :: 1
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Actions for AWS IoT Rule
 
 <!--BEGIN STABILITY BANNER-->---
@@ -43,43 +43,22 @@
 
 This library contains integration classes to send data to any number of
 supported AWS Services. Instances of these classes should be passed to
 `TopicRule` defined in `@aws-cdk/aws-iot`.
 
 Currently supported are:
 
-* Republish a message to another MQTT topic
 * Invoke a Lambda function
 * Put objects to a S3 bucket
 * Put logs to CloudWatch Logs
 * Capture CloudWatch metrics
 * Change state for a CloudWatch alarm
 * Put records to Kinesis Data stream
 * Put records to Kinesis Data Firehose stream
 * Send messages to SQS queues
-* Publish messages on SNS topics
-* Write messages into columns of DynamoDB
-* Put messages IoT Events input
-* Send messages to HTTPS endpoints
-
-## Republish a message to another MQTT topic
-
-The code snippet below creates an AWS IoT Rule that republish a message to
-another MQTT topic when it is triggered.
-
-```python
-iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, timestamp() as timestamp, temperature FROM 'device/+/data'"),
-    actions=[
-        actions.IotRepublishMqttAction("${topic()}/republish",
-            quality_of_service=actions.MqttQualityOfService.AT_LEAST_ONCE
-        )
-    ]
-)
-```
 
 ## Invoke a Lambda function
 
 The code snippet below creates an AWS IoT Rule that invoke a Lambda function
 when it is triggered.
 
 ```python
@@ -96,15 +75,15 @@
     sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, timestamp() as timestamp, temperature FROM 'device/+/data'"),
     actions=[actions.LambdaFunctionAction(func)]
 )
 ```
 
 ## Put objects to a S3 bucket
 
-The code snippet below creates an AWS IoT Rule that puts objects to a S3 bucket
+The code snippet below creates an AWS IoT Rule that put objects to a S3 bucket
 when it is triggered.
 
 ```python
 bucket = s3.Bucket(self, "MyBucket")
 
 iot.TopicRule(self, "TopicRule",
     sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id FROM 'device/+/data'"),
@@ -147,15 +126,15 @@
         )
     ]
 )
 ```
 
 ## Put logs to CloudWatch Logs
 
-The code snippet below creates an AWS IoT Rule that puts logs to CloudWatch Logs
+The code snippet below creates an AWS IoT Rule that put logs to CloudWatch Logs
 when it is triggered.
 
 ```python
 import aws_cdk.aws_logs as logs
 
 
 log_group = logs.LogGroup(self, "MyLogGroup")
@@ -182,32 +161,14 @@
             metric_value="${value}",
             metric_timestamp="${timestamp}"
         )
     ]
 )
 ```
 
-## Start Step Functions State Machine
-
-The code snippet below creates an AWS IoT Rule that starts a Step Functions State Machine
-when it is triggered.
-
-```python
-state_machine = stepfunctions.StateMachine(self, "SM",
-    definition_body=stepfunctions.DefinitionBody.from_chainable(stepfunctions.Wait(self, "Hello", time=stepfunctions.WaitTime.duration(Duration.seconds(10))))
-)
-
-iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
-    actions=[
-        actions.StepFunctionsStateMachineAction(state_machine)
-    ]
-)
-```
-
 ## Change the state of an Amazon CloudWatch alarm
 
 The code snippet below creates an AWS IoT Rule that changes the state of an Amazon CloudWatch alarm when it is triggered:
 
 ```python
 import aws_cdk.aws_cloudwatch as cloudwatch
 
@@ -233,15 +194,15 @@
         )
     ]
 )
 ```
 
 ## Put records to Kinesis Data stream
 
-The code snippet below creates an AWS IoT Rule that puts records to Kinesis Data
+The code snippet below creates an AWS IoT Rule that put records to Kinesis Data
 stream when it is triggered.
 
 ```python
 import aws_cdk.aws_kinesis as kinesis
 
 
 stream = kinesis.Stream(self, "MyStream")
@@ -254,15 +215,15 @@
         )
     ]
 )
 ```
 
 ## Put records to Kinesis Data Firehose stream
 
-The code snippet below creates an AWS IoT Rule that puts records to Put records
+The code snippet below creates an AWS IoT Rule that put records to Put records
 to Kinesis Data Firehose stream when it is triggered.
 
 ```python
 import aws_cdk.aws_kinesisfirehose_alpha as firehose
 import aws_cdk.aws_kinesisfirehose_destinations_alpha as destinations
 
 
@@ -299,91 +260,8 @@
         actions.SqsQueueAction(queue,
             use_base64=True
         )
     ]
 )
 ```
 
-## Publish messages on an SNS topic
-
-The code snippet below creates and AWS IoT Rule that publishes messages to an SNS topic when it is triggered:
-
-```python
-import aws_cdk.aws_sns as sns
-
-
-topic = sns.Topic(self, "MyTopic")
-
-topic_rule = iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, year, month, day FROM 'device/+/data'"),
-    actions=[
-        actions.SnsTopicAction(topic,
-            message_format=actions.SnsActionMessageFormat.JSON
-        )
-    ]
-)
-```
-
-## Write attributes of a message to DynamoDB
-
-The code snippet below creates an AWS IoT rule that writes all or part of an
-MQTT message to DynamoDB using the DynamoDBv2 action.
-
-```python
-import aws_cdk.aws_dynamodb as dynamodb
-
-# table: dynamodb.Table
-
-
-topic_rule = iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
-    actions=[
-        actions.DynamoDBv2PutItemAction(table)
-    ]
-)
-```
-
-## Put messages IoT Events input
-
-The code snippet below creates an AWS IoT Rule that puts messages
-to an IoT Events input when it is triggered:
-
-```python
-import aws_cdk.aws_iotevents_alpha as iotevents
-import aws_cdk.aws_iam as iam
-
-# role: iam.IRole
-
-
-input = iotevents.Input(self, "MyInput",
-    attribute_json_paths=["payload.temperature", "payload.transactionId"]
-)
-topic_rule = iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT * FROM 'device/+/data'"),
-    actions=[
-        actions.IotEventsPutMessageAction(input,
-            batch_mode=True,  # optional property, default is 'false'
-            message_id="${payload.transactionId}",  # optional property, default is a new UUID
-            role=role
-        )
-    ]
-)
-```
-
-## Send Messages to HTTPS Endpoints
 
-The code snippet below creates an AWS IoT Rule that sends messages
-to an HTTPS endpoint when it is triggered:
-
-```python
-topic_rule = iot.TopicRule(self, "TopicRule",
-    sql=iot.IotSql.from_string_as_ver20160323("SELECT topic(2) as device_id, year, month, day FROM 'device/+/data'")
-)
-
-topic_rule.add_action(
-    actions.HttpsAction("https://example.com/endpoint",
-        confirmation_url="https://example.com",
-        headers=[actions.HttpActionHeader(key="key0", value="value0"), actions.HttpActionHeader(key="key1", value="value1")
-        ],
-        auth=actions.HttpActionSigV4Auth(service_name="serviceName", signing_region="us-east-1")
-    ))
-```
```

### Comparing `aws-cdk.aws-iot-actions-alpha-2.89.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-iot-actions-alpha-2.9.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_iot_actions_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_iot_actions_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_iot_actions_alpha.egg-info/requires.txt
 src/aws_cdk.aws_iot_actions_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_iot_actions_alpha/__init__.py
 src/aws_cdk/aws_iot_actions_alpha/py.typed
 src/aws_cdk/aws_iot_actions_alpha/_jsii/__init__.py
-src/aws_cdk/aws_iot_actions_alpha/_jsii/aws-iot-actions-alpha@2.89.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_iot_actions_alpha/_jsii/aws-iot-actions-alpha@2.9.0-alpha.0.jsii.tgz
```

