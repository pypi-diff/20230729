# Comparing `tmp/aws-cdk.aws-scheduler-alpha-2.88.0a0.tar.gz` & `tmp/aws-cdk.aws-scheduler-alpha-2.89.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src3082485108/src/packages/@aws-cdk/aws-scheduler-alpha/dist/python/aws-cdk.aws-scheduler-alpha-2.88.0a0.tar", last modified: Thu Jul 20 12:41:11 2023, max compression
+gzip compressed data, was "/codebuild/output/src2022765760/src/packages/@aws-cdk/aws-scheduler-alpha/dist/python/aws-cdk.aws-scheduler-alpha-2.89.0a0.tar", last modified: Fri Jul 28 22:05:11 2023, max compression
```

## Comparing `aws-cdk.aws-scheduler-alpha-2.88.0a0.tar` & `aws-cdk.aws-scheduler-alpha-2.89.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-07-20 12:41:06.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 12:41:06.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-20 12:41:06.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9490 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8483 2023-07-20 12:41:06.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-20 12:41:06.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1886 2023-07-20 12:41:06.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk/aws_scheduler_alpha/
--rw-r--r--   0 root         (0) root         (0)    31152 2023-07-20 12:41:06.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk/aws_scheduler_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-20 12:41:06.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36750 2023-07-20 12:41:06.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.88.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 12:41:06.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk/aws_scheduler_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9490 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 12:41:11.000000 aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-07-28 22:05:04.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 22:05:04.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-28 22:05:04.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10576 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9569 2023-07-28 22:05:04.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-28 22:05:04.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-07-28 22:05:04.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk/aws_scheduler_alpha/
+-rw-r--r--   0 root         (0) root         (0)   143150 2023-07-28 22:05:04.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk/aws_scheduler_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 22:05:04.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49013 2023-07-28 22:05:04.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.89.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:05:04.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk/aws_scheduler_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10576 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      551 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-28 22:05:11.000000 aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.88.0a0/LICENSE` & `aws-cdk.aws-scheduler-alpha-2.89.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-scheduler-alpha-2.88.0a0/PKG-INFO` & `aws-cdk.aws-scheduler-alpha-2.89.0a0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: aws-cdk.aws-scheduler-alpha
-Version: 2.88.0a0
-Summary: The CDK Construct Library for Amazon Scheduler
-Home-page: https://github.com/aws/aws-cdk
-Author: Amazon Web Services
-License: Apache-2.0
-Project-URL: Source, https://github.com/aws/aws-cdk.git
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved
-Classifier: Framework :: AWS CDK
-Classifier: Framework :: AWS CDK :: 2
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
 # Amazon EventBridge Scheduler Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
 
 
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
@@ -64,14 +37,15 @@
 ## Defining a schedule
 
 TODO: Schedule is not yet fully implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 Only an L2 class is created that wraps the L1 class and handles the following properties:
 
 * schedule
+* schedule group
 * target (only LambdaInvoke is supported for now)
 * flexibleTimeWindow will be set to `{ mode: 'OFF' }`
 
 ### Schedule Expressions
 
 You can choose from three schedule types when configuring your schedule: rate-based, cron-based, and one-time schedules.
 
@@ -112,15 +86,39 @@
     target,
     description: 'This is a one-time schedule in New York timezone',
 });
 ```
 
 ### Grouping Schedules
 
-TODO: Group is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+Your AWS account comes with a default scheduler group. You can access default group in CDK with:
+
+```text
+const defaultGroup = Group.fromDefaultGroup(this, "DefaultGroup");
+```
+
+If not specified a schedule is added to the default group. However, you can also add the schedule to a custom scheduling group managed by you:
+
+```text
+const group = new Group(this, "Group", {
+    groupName: "MyGroup",
+});
+
+const target = new targets.LambdaInvoke(props.func, {
+    input: ScheduleTargetInput.fromObject({
+        "payload": "useful",
+    }),
+});
+
+new Schedule(this, 'Schedule', {
+    scheduleExpression: ScheduleExpression.rate(Duration.minutes(10)),
+    target,
+    group,
+});
+```
 
 ## Scheduler Targets
 
 TODO: Scheduler Targets Module is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 Only LambdaInvoke target is added for now.
 
@@ -178,8 +176,32 @@
 
 ### Metrics for all schedules
 
 TODO: Not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 ### Metrics for a Group
 
-TODO: Not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+To view metrics for a specific group you can use methods on class `Group`:
+
+```python
+group = Group(self, "Group",
+    group_name="MyGroup"
+)
+
+cloudwatch.Alarm(self, "MyGroupErrorAlarm",
+    metric=group.metric_target_errors(),
+    evaluation_periods=1,
+    threshold=0
+)
+
+# Or use default group
+default_group = Group.from_default_group(self, "DefaultGroup")
+cloudwatch.Alarm(self, "DefaultGroupErrorAlarm",
+    metric=default_group.metric_target_errors(),
+    evaluation_periods=1,
+    threshold=0
+)
+```
+
+See full list of metrics and their description at
+[Monitoring Using CloudWatch Metrics](https://docs.aws.amazon.com/scheduler/latest/UserGuide/monitoring-cloudwatch.html)
+in the *AWS Event Bridge Scheduler User Guide*.
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.88.0a0/README.md` & `aws-cdk.aws-scheduler-alpha-2.89.0a0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: aws-cdk.aws-scheduler-alpha
+Version: 2.89.0a0
+Summary: The CDK Construct Library for Amazon Scheduler
+Home-page: https://github.com/aws/aws-cdk
+Author: Amazon Web Services
+License: Apache-2.0
+Project-URL: Source, https://github.com/aws/aws-cdk.git
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved
+Classifier: Framework :: AWS CDK
+Classifier: Framework :: AWS CDK :: 2
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
 # Amazon EventBridge Scheduler Construct Library
 
 <!--BEGIN STABILITY BANNER-->---
 
 
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
@@ -37,14 +64,15 @@
 ## Defining a schedule
 
 TODO: Schedule is not yet fully implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 Only an L2 class is created that wraps the L1 class and handles the following properties:
 
 * schedule
+* schedule group
 * target (only LambdaInvoke is supported for now)
 * flexibleTimeWindow will be set to `{ mode: 'OFF' }`
 
 ### Schedule Expressions
 
 You can choose from three schedule types when configuring your schedule: rate-based, cron-based, and one-time schedules.
 
@@ -85,15 +113,39 @@
     target,
     description: 'This is a one-time schedule in New York timezone',
 });
 ```
 
 ### Grouping Schedules
 
-TODO: Group is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+Your AWS account comes with a default scheduler group. You can access default group in CDK with:
+
+```text
+const defaultGroup = Group.fromDefaultGroup(this, "DefaultGroup");
+```
+
+If not specified a schedule is added to the default group. However, you can also add the schedule to a custom scheduling group managed by you:
+
+```text
+const group = new Group(this, "Group", {
+    groupName: "MyGroup",
+});
+
+const target = new targets.LambdaInvoke(props.func, {
+    input: ScheduleTargetInput.fromObject({
+        "payload": "useful",
+    }),
+});
+
+new Schedule(this, 'Schedule', {
+    scheduleExpression: ScheduleExpression.rate(Duration.minutes(10)),
+    target,
+    group,
+});
+```
 
 ## Scheduler Targets
 
 TODO: Scheduler Targets Module is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 Only LambdaInvoke target is added for now.
 
@@ -151,8 +203,32 @@
 
 ### Metrics for all schedules
 
 TODO: Not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 ### Metrics for a Group
 
-TODO: Not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+To view metrics for a specific group you can use methods on class `Group`:
+
+```python
+group = Group(self, "Group",
+    group_name="MyGroup"
+)
+
+cloudwatch.Alarm(self, "MyGroupErrorAlarm",
+    metric=group.metric_target_errors(),
+    evaluation_periods=1,
+    threshold=0
+)
+
+# Or use default group
+default_group = Group.from_default_group(self, "DefaultGroup")
+cloudwatch.Alarm(self, "DefaultGroupErrorAlarm",
+    metric=default_group.metric_target_errors(),
+    evaluation_periods=1,
+    threshold=0
+)
+```
+
+See full list of metrics and their description at
+[Monitoring Using CloudWatch Metrics](https://docs.aws.amazon.com/scheduler/latest/UserGuide/monitoring-cloudwatch.html)
+in the *AWS Event Bridge Scheduler User Guide*.
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.88.0a0/setup.py` & `aws-cdk.aws-scheduler-alpha-2.89.0a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-scheduler-alpha",
-    "version": "2.88.0.a0",
+    "version": "2.89.0.a0",
     "description": "The CDK Construct Library for Amazon Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.aws_scheduler_alpha",
         "aws_cdk.aws_scheduler_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_scheduler_alpha._jsii": [
-            "aws-scheduler-alpha@2.88.0-alpha.0.jsii.tgz"
+            "aws-scheduler-alpha@2.89.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_scheduler_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.88.0",
+        "aws-cdk-lib==2.89.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-scheduler-alpha
-Version: 2.88.0a0
+Version: 2.89.0a0
 Summary: The CDK Construct Library for Amazon Scheduler
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -64,14 +64,15 @@
 ## Defining a schedule
 
 TODO: Schedule is not yet fully implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 Only an L2 class is created that wraps the L1 class and handles the following properties:
 
 * schedule
+* schedule group
 * target (only LambdaInvoke is supported for now)
 * flexibleTimeWindow will be set to `{ mode: 'OFF' }`
 
 ### Schedule Expressions
 
 You can choose from three schedule types when configuring your schedule: rate-based, cron-based, and one-time schedules.
 
@@ -112,15 +113,39 @@
     target,
     description: 'This is a one-time schedule in New York timezone',
 });
 ```
 
 ### Grouping Schedules
 
-TODO: Group is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+Your AWS account comes with a default scheduler group. You can access default group in CDK with:
+
+```text
+const defaultGroup = Group.fromDefaultGroup(this, "DefaultGroup");
+```
+
+If not specified a schedule is added to the default group. However, you can also add the schedule to a custom scheduling group managed by you:
+
+```text
+const group = new Group(this, "Group", {
+    groupName: "MyGroup",
+});
+
+const target = new targets.LambdaInvoke(props.func, {
+    input: ScheduleTargetInput.fromObject({
+        "payload": "useful",
+    }),
+});
+
+new Schedule(this, 'Schedule', {
+    scheduleExpression: ScheduleExpression.rate(Duration.minutes(10)),
+    target,
+    group,
+});
+```
 
 ## Scheduler Targets
 
 TODO: Scheduler Targets Module is not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 Only LambdaInvoke target is added for now.
 
@@ -178,8 +203,32 @@
 
 ### Metrics for all schedules
 
 TODO: Not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
 
 ### Metrics for a Group
 
-TODO: Not yet implemented. See section in [L2 Event Bridge Scheduler RFC](https://github.com/aws/aws-cdk-rfcs/blob/master/text/0474-event-bridge-scheduler-l2.md)
+To view metrics for a specific group you can use methods on class `Group`:
+
+```python
+group = Group(self, "Group",
+    group_name="MyGroup"
+)
+
+cloudwatch.Alarm(self, "MyGroupErrorAlarm",
+    metric=group.metric_target_errors(),
+    evaluation_periods=1,
+    threshold=0
+)
+
+# Or use default group
+default_group = Group.from_default_group(self, "DefaultGroup")
+cloudwatch.Alarm(self, "DefaultGroupErrorAlarm",
+    metric=default_group.metric_target_errors(),
+    evaluation_periods=1,
+    threshold=0
+)
+```
+
+See full list of metrics and their description at
+[Monitoring Using CloudWatch Metrics](https://docs.aws.amazon.com/scheduler/latest/UserGuide/monitoring-cloudwatch.html)
+in the *AWS Event Bridge Scheduler User Guide*.
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.88.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-scheduler-alpha-2.89.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_scheduler_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_scheduler_alpha.egg-info/requires.txt
 src/aws_cdk.aws_scheduler_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_scheduler_alpha/__init__.py
 src/aws_cdk/aws_scheduler_alpha/py.typed
 src/aws_cdk/aws_scheduler_alpha/_jsii/__init__.py
-src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.88.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.89.0-alpha.0.jsii.tgz
```

