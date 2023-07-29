# Comparing `tmp/yunxiao-0.3.4.tar.gz` & `tmp/yunxiao-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.3.4.tar", last modified: Tue Jul  4 05:07:43 2023, max compression
+gzip compressed data, was "yunxiao-0.3.5.tar", last modified: Sat Jul 29 04:54:01 2023, max compression
```

## Comparing `yunxiao-0.3.4.tar` & `yunxiao-0.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 05:07:43.488906 yunxiao-0.3.4/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     6351 2023-07-04 05:07:43.488404 yunxiao-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.3.4/README.md
--rw-rw-rw-   0        0        0     1488 2023-07-04 05:07:29.000000 yunxiao-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 05:07:43.488906 yunxiao-0.3.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 05:07:43.478374 yunxiao-0.3.4/test/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.3.4/test/test.py
-drwxrwxrwx   0        0        0        0 2023-07-04 05:07:43.481397 yunxiao-0.3.4/yunxiao/
--rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.3.4/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    40893 2023-07-04 05:04:56.000000 yunxiao-0.3.4/yunxiao/v2.py
--rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.3.4/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-07-04 05:07:43.487403 yunxiao-0.3.4/yunxiao.egg-info/
--rw-rw-rw-   0        0        0     6351 2023-07-04 05:07:43.000000 yunxiao-0.3.4/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-07-04 05:07:43.000000 yunxiao-0.3.4/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 05:07:43.000000 yunxiao-0.3.4/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 05:07:43.000000 yunxiao-0.3.4/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-04 05:07:43.000000 yunxiao-0.3.4/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 04:54:01.125195 yunxiao-0.3.5/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0     6351 2023-07-29 04:54:01.125195 yunxiao-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.3.5/README.md
+-rw-rw-rw-   0        0        0     1523 2023-07-29 04:53:43.000000 yunxiao-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 04:54:01.125195 yunxiao-0.3.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 04:54:01.111648 yunxiao-0.3.5/test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.3.5/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:54:01.115651 yunxiao-0.3.5/yunxiao/
+-rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.3.5/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    41302 2023-07-28 19:53:52.000000 yunxiao-0.3.5/yunxiao/v2.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.3.5/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:54:01.123191 yunxiao-0.3.5/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0     6351 2023-07-29 04:54:01.000000 yunxiao-0.3.5/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-07-29 04:54:01.000000 yunxiao-0.3.5/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 04:54:01.000000 yunxiao-0.3.5/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 04:54:01.000000 yunxiao-0.3.5/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 04:54:01.000000 yunxiao-0.3.5/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.3.4/LICENSE` & `yunxiao-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.4/PKG-INFO` & `yunxiao-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.3.4
+Version: 0.3.5
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.3.4/README.md` & `yunxiao-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.4/pyproject.toml` & `yunxiao-0.3.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.3.4"
+version = "0.3.5"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
@@ -22,14 +22,15 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.3.5" = "更新可用参数。"
 "0.3.4" = "修复BUG:拉取意向失败。"
 "0.3.3" = "修复BUG：班级查询根据名称检索失效。"
 "0.3.2" = "更新参数，修复BUG，新增意向管理API"
 "0.3.1" = "修复整合"
 "0.2.9" = "删除其他，只使用V2"
 "0.2.6" = "V2 中更多使用分片读取。"
 "0.2.5" = "修复 V2 中的 API端点错误。新增 loop 装饰器便于分片提取大量数据。"
```

### Comparing `yunxiao-0.3.4/yunxiao/v2.py` & `yunxiao-0.3.5/yunxiao/v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,37 +296,42 @@
                 "page": {"pageNum": page, "pageSize": size}
             }
         )
 
     # 查询学生
     @loop("")
     def students_query(self, page, size, curriculumids: tuple = (), classids: tuple = (), name: str = "",
-                       status: tuple = (1, 7), class_student_status: int = 0):
+                       status: tuple = (1, 7), class_student_status: int = 0,
+                       start_create_time: str = "", end_create_time: str = ""):
         """
         查询学生
         :param size: 分页查询，每页数量
         :param page: 分页查询，初始页码，应设为 0
         :param curriculumids: 课程筛选
         :param classids: 班级筛选
         :param name: 姓名查询关键字
         :param status: 学员状态。 **0** 未收费 **1** 在读 **6** 曾就读 **7** 停课 **99** 无效学员
         :param class_student_status: **0** 不筛选 **1** 未入班 **2** 已入班
+        :param start_create_time: 起始创建时间
+        :param end_create_time: 截止创建时间
         :return:
         """
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-crm/student/list",
             json={
                 "_t_": UsedTime.stamp,
                 "name": name,
                 "campusIds": self.campus,
                 "status": list(status),
                 "curriculumIds": list(curriculumids),
                 "classIds": list(classids),
                 "classStudentStatus": class_student_status,
+                "startCreateTime": start_create_time,
+                "endCreateTime": end_create_time,
                 "orgTag": 1,
                 "page": {"pageNum": page, "pageSize": size}
             }
         )
 
     # 学生数据费用报表。
     @loop("cardCourseTradedList")
@@ -379,34 +384,36 @@
                 "studentName": studentName
             }
         )
 
     # 查询学生课程卡
     @loop("")
     def students_query_cards(self, page: int, size: int, display_history: bool = True,
-                             remain_amount_min: str = "", remain_amount_max: str = ""):
+                             remain_amount_min: str = "", remain_amount_max: str = "", student_name: str = ""):
         """
         列出所有课程卡
         :param size: 分页查询，每页数量
         :param page: 分页查询，起始页码，应设为 0
         :param display_history: 是否显示曾就读学生
         :param remain_amount_max: 限制查询剩余次数-最大
         :param remain_amount_min: 限制查询剩余次数-最小
+        :param student_name: 查询学员名
         :return:
         """
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/studentCourseCard/report",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": page, "pageSize": size},
                 "campusIds": self.campus,
                 "displayHistory": display_history,
                 "remainAmountMin": remain_amount_min,
-                "remainAmountMax": remain_amount_max
+                "remainAmountMax": remain_amount_max,
+                "studentName": student_name
             }
         )
 
     # 查询学生基本信息
     def student_query_info(self, studentid: int, companyid: int = None):
         """
         查询学生基本信息
@@ -603,15 +610,15 @@
                 "displayCompletedClass": displayCompletedClass,
                 "page": {"pageNum": page, "pageSize": size}
             }
         )
 
     # 查询班级
     @loop("")
-    def classes_query(self, page, size, teacherids: tuple = (), classname: str = "", classStatus: int = 0):
+    def classes_query(self, page, size, teacherids: tuple = (), classname: str = "", classStatus: int = ""):
         """
         查询班级
         :param size: 分页查询，每页数量
         :param page: 分页查询，起始页码，应设为 0
         :param classname: 班级名称
         :param classStatus: 班级状态。 **0** 未结班 **1** 已结班
         :param teacherids: 老师ID
```

### Comparing `yunxiao-0.3.4/yunxiao/yunxiao.py` & `yunxiao-0.3.5/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.4/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.3.5/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.3.4
+Version: 0.3.5
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

