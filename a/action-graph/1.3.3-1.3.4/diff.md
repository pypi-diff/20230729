# Comparing `tmp/action-graph-1.3.3.tar.gz` & `tmp/action-graph-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "action-graph-1.3.3.tar", last modified: Wed Jun 28 14:35:26 2023, max compression
+gzip compressed data, was "action-graph-1.3.4.tar", last modified: Sat Jul 29 16:45:59 2023, max compression
```

## Comparing `action-graph-1.3.3.tar` & `action-graph-1.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.3.3/LICENSE
--rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.3.3/README.md
--rw-r--r--   0        0        0      684 2023-06-28 14:35:08.272045 action-graph-1.3.3/action_graph/__init__.py
--rw-r--r--   0        0        0     3595 2023-06-28 00:55:07.217794 action-graph-1.3.3/action_graph/action.py
--rw-r--r--   0        0        0    11552 2023-06-28 01:01:53.944495 action-graph-1.3.3/action_graph/agent.py
--rw-r--r--   0        0        0     4664 2023-06-25 03:02:12.179040 action-graph-1.3.3/action_graph/planner.py
--rw-r--r--   0        0        0      832 2023-06-28 14:35:13.504003 action-graph-1.3.3/pyproject.toml
--rwxr-xr-x   0        0        0     1103 2023-06-16 14:34:49.765956 action-graph-1.3.3/tests/01-redundant_precon_test.py
--rwxr-xr-x   0        0        0     1039 2023-06-23 21:15:35.619807 action-graph-1.3.3/tests/02-multi_feasible_test.py
--rwxr-xr-x   0        0        0     1284 2023-06-16 14:37:32.454361 action-graph-1.3.3/tests/03-references_test.py
--rwxr-xr-x   0        0        0      909 2023-06-23 20:50:11.922048 action-graph-1.3.3/tests/04-loop_test.py
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.3.4/LICENSE
+-rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.3.4/README.md
+-rw-r--r--   0        0        0      684 2023-07-29 16:40:34.654333 action-graph-1.3.4/action_graph/__init__.py
+-rw-r--r--   0        0        0     3612 2023-07-29 16:12:29.398338 action-graph-1.3.4/action_graph/action.py
+-rw-r--r--   0        0        0    10209 2023-07-29 16:17:30.317255 action-graph-1.3.4/action_graph/agent.py
+-rw-r--r--   0        0        0     4664 2023-06-25 03:02:12.179040 action-graph-1.3.4/action_graph/planner.py
+-rw-r--r--   0        0        0      832 2023-07-29 16:40:45.857938 action-graph-1.3.4/pyproject.toml
+-rwxr-xr-x   0        0        0     1103 2023-06-16 14:34:49.765956 action-graph-1.3.4/tests/01-redundant_precon_test.py
+-rwxr-xr-x   0        0        0     1039 2023-06-23 21:15:35.619807 action-graph-1.3.4/tests/02-multi_feasible_test.py
+-rwxr-xr-x   0        0        0     1284 2023-06-16 14:37:32.454361 action-graph-1.3.4/tests/03-references_test.py
+-rwxr-xr-x   0        0        0      909 2023-06-23 20:50:11.922048 action-graph-1.3.4/tests/04-loop_test.py
+-rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.3.4/PKG-INFO
```

### Comparing `action-graph-1.3.3/LICENSE` & `action-graph-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.3/README.md` & `action-graph-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.3/action_graph/__init__.py` & `action-graph-1.3.4/action_graph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 
 from action_graph.action import Action, ActionStatus, State
 from action_graph.agent import Agent
 
 name = 'action_graph'
-__version__ = '1.3.3'
+__version__ = '1.3.4'
 __all__ = [
     'State',
     'Action',
     'ActionStatus',
     'ActionFailedException',
     'ActionAbortedException',
     'ActionTimedOutException',
```

### Comparing `action-graph-1.3.3/action_graph/action.py` & `action-graph-1.3.4/action_graph/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 class ActionStatus(Enum):
     FAILURE = auto()
     SUCCESS = auto()
     RUNNING = auto()
     ABORTED = auto()
     NEUTRAL = auto()
+    REVOKED = auto()
 
 
 class Action():
 
     effects: State = {}
     preconditions: State = {}
 
@@ -55,15 +56,15 @@
 
     def on_failure(self, outcome: State = None):
         pass
 
     def on_aborted(self, outcome: State = None):
         pass
 
-    def on_preempted(self, outcome: State = None):
+    def on_revoked(self, outcome: State = None):
         pass
 
     def on_neutral(self, outcome: State = None):
         pass
 
     def on_exit(self, outcome: State = None):
         pass
@@ -131,9 +132,9 @@
     pass
 
 
 class ActionTimedOutException(Exception):
     pass
 
 
-class ActionPreemptedException(Exception):
+class ActionRevokedException(Exception):
     pass
```

### Comparing `action-graph-1.3.3/action_graph/agent.py` & `action-graph-1.3.4/action_graph/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 import logging
 from time import sleep, time
 from typing import Iterable, List
 
 from action_graph.action import (Action, ActionStatus, State,
                                  ActionTimedOutException, ActionAbortedException, 
-                                 ActionFailedException, ActionPreemptedException)
+                                 ActionFailedException, ActionRevokedException)
 from action_graph.planner import Planner, PlanningFailedException
 
 
 class Agent:
     """Autonomous agent to monitor system state, keep track of feasible actions, generate plans and achive desired goals"""
 
     __planner: Planner = Planner([])
     __abort: bool = False
-    __preempted: bool = False
+    __revoked: bool = False
 
     def __init__(self, agent_name=None) -> None:
         if not agent_name:
             agent_name = self.__class__.__name__
         self.name = agent_name
         #
         self.state: State = {}
@@ -47,28 +47,28 @@
     def abort(self):
         """
         Abort execution.
         """
 
         self.__abort = True
 
-    def preempt(self):
+    def revoke(self):
         """
-        Preempt execution.
+        Revoke goals.
         """
 
-        self.__preempted = True
+        self.__revoked = True
 
     def reset(self):
         """
-        Resets the abort/preempt status back to False in the event abort was triggered.
+        Resets the abort/revoke status back to False in the event abort was triggered.
         """
 
         self.__abort = False
-        self.__preempted = False
+        self.__revoked = False
 
     def is_goal_met(self, goal: State) -> bool:
         """
         Compares the desired goal state against the system state to check if it is already met.
 
         :param goal:State: Desired goal state
         :return:bool: True if goal state and current system state is same; False otherwise
@@ -122,56 +122,14 @@
 
             except Exception as _ex:
                 logging.error(f"{_ex}")
                 raise
 
         logging.info(f"EXECUTION SUCCEDED!")
 
-    def achieve_goal(self, goal: State, verbose: bool = False):
-        """
-        Creates a plan to satisfy the goal state; executes it action-by-action; re-evaluates the plan at each step;
-
-        :param goal:State: Desired goal state
-        :param verbose:bool: Print plan to console at each step, if True
-        """
-
-        blacklisted_actions: List[str] = []
-
-        # state might have changed since the last step was executed
-        while not self.is_goal_met(goal):
-
-            try:
-                # (re)generate the plan
-                plan: List[Action] = self.__planner.generate_plan(goal, self.state, blacklisted_actions)
-                if verbose:
-                    self.print_plan_to_console(plan)
-                # execute one plan step at a time
-                first_action = plan[0]
-                self.execute_action(first_action)
-
-                # if the latest executed action has the same effect as any of the blacklisted actions,
-                # then it is prudent(?) to remove such a blacklisted action
-                ba: List[Action] = [a for a in self.__actions if str(a) in blacklisted_actions]
-                for action in ba:
-                    if set(first_action.effects.keys()) <= set(action.effects.keys()):
-                        blacklisted_actions.remove(str(action))
-
-            except ActionFailedException as ex_fail:
-                logging.error(f"{ex_fail} / ATTEMPTING ALTERNATIVE PLAN")
-                __action_name = str(first_action)
-                if __action_name not in blacklisted_actions:
-                    blacklisted_actions.append(__action_name)
-                continue
-
-            except Exception as _ex:
-                logging.error(f"{_ex}")
-                raise
-
-        logging.info(f"EXECUTION SUCCEDED!")
-
     def plan_and_execute(self, goal: State, verbose: bool = False) -> Iterable:
         """
         Creates a plan to satisfy the goal state; executes it action-by-action; re-evaluates the plan at each step;
 
         :param goal:State: Desired goal state
         :param verbose:bool: if True, prints formatted plan to console at each step
         """
@@ -203,17 +161,17 @@
 
             except ActionFailedException as ex_fail:
                 logging.error(f"{ex_fail} / ATTEMPTING ALTERNATIVE PLAN")
                 if str(first_action) not in blacklisted_actions:
                     blacklisted_actions.append(str(first_action))
                 continue
 
-            except ActionPreemptedException as _ex_preempted:
-                # logging.info(f"{ex_preempted}")
-                self.__preempted = False  # reset preempted status
+            except ActionRevokedException as _ex_revoked:
+                logging.info(f"{_ex_revoked} / STOPPING.")
+                self.__revoked = False  # reset revoked status
                 break
 
             except Exception as _ex:
                 logging.error(f"{_ex}")
                 raise
 
         logging.info(f"EXECUTION SUCCEDED!")
@@ -228,19 +186,19 @@
     def execute_action(self, action: Action):
         # Check for abort status
         if self.__abort:
             # logging.error(f'ACTION: {action} : EXECUTION ABORTED BEFORE START !!')
             action.on_aborted(action.effects)
             raise ActionAbortedException(f'ACTION: {action} FAILED. ABORTED STATE IS ACTIVE!!')
 
-        # Check for preempt status
-        if self.__preempted:
-            # logging.error(f'ACTION: {action} : EXECUTION PREEMPTED BEFORE START !!')
-            action.on_preempted(action.effects)
-            raise ActionPreemptedException(f'EXECUTION PREEMPTED WHILE AT ACTION: {action}')
+        # Check for revoked status
+        if self.__revoked:
+            # logging.error(f'ACTION: {action} : EXECUTION REVOKED BEFORE START !!')
+            action.on_revoked(action.effects)
+            raise ActionRevokedException(f'ACTION/GOALS REVOKED WHILE AT ACTION: {action}')
 
         # Check runtime precondition
         if not action.check_runtime_precondition(action.effects):
             raise ActionFailedException(f'ACTION: {action} RUNTIME PRECONDITION CHECK FAILED!!.')
 
         # Execute the plan step
         action._execute(action.effects)
@@ -252,17 +210,22 @@
             return
 
         # monitor the status; wait until execution is complete
         time0 = time()
         while action.is_running():
             if self.__abort:
                 # if an abort was signalled
-                logging.critical(f'ACTION: {action} : EXECUTION ABORTED!!')
+                # logging.critical(f'ACTION: {action} : EXECUTION ABORTED!!')
                 action.status = ActionStatus.ABORTED
                 break
+            if self.__revoked:
+                # if an revoke was signalled
+                # logging.critical(f'ACTION: {action} : GOALS REVOKED. STOPPING!!')
+                action.status = ActionStatus.REVOKED
+                break
             if time()-time0 > action.timeout:
                 # Action timeout exceeded
                 raise ActionTimedOutException(f'ACTION: {action} : TIMED OUT!!')
             if not action.status == ActionStatus.RUNNING:
                 # thread is alive but the status has changed
                 break  # so move on
             sleep(0.05)  # throttle loop
@@ -296,9 +259,15 @@
 
         # Execution aborted
         if action.status == ActionStatus.ABORTED:
             action.on_aborted(action.effects)
             # Stop execution as action aborted
             raise ActionAbortedException(f'ACTION: {action} ABORTED!')
 
+        # Goals revoked
+        if action.status == ActionStatus.REVOKED:
+            action.on_revoked(action.effects)
+            # Stop execution as goals revoked
+            raise ActionRevokedException(f'ACTION: {action} REVOKED!')
+
         # Any clean up needed after execution e.g. updating system states
         action.on_exit(action.effects)
```

### Comparing `action-graph-1.3.3/action_graph/planner.py` & `action-graph-1.3.4/action_graph/planner.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.3/pyproject.toml` & `action-graph-1.3.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 authors = [
     { name = "Bharath Achyutha Rao", email = "bharath.rao@hotmail.com" },
 ]
 name = "action_graph"
-version = "1.3.3"
+version = "1.3.4"
 description = "Autonomous agent for task/action planning and execution"
 readme = "README.md"
 requires-python = ">=3.7,<4.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `action-graph-1.3.3/tests/01-redundant_precon_test.py` & `action-graph-1.3.4/tests/01-redundant_precon_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.3/tests/02-multi_feasible_test.py` & `action-graph-1.3.4/tests/02-multi_feasible_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.3/tests/03-references_test.py` & `action-graph-1.3.4/tests/03-references_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.3/tests/04-loop_test.py` & `action-graph-1.3.4/tests/04-loop_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.3/PKG-INFO` & `action-graph-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action_graph
-Version: 1.3.3
+Version: 1.3.4
 Summary: Autonomous agent for task/action planning and execution
 Author-email: Bharath Achyutha Rao <bharath.rao@hotmail.com>
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Bug Tracker, https://github.com/bharathra/action_graph/issues
```

