# Comparing `tmp/pyfsdb-viewer-0.3.tar.gz` & `tmp/pyfsdb-viewer-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfsdb-viewer-0.3.tar", last modified: Thu Jun 29 21:17:58 2023, max compression
+gzip compressed data, was "pyfsdb-viewer-0.4.tar", last modified: Fri Jul 28 23:07:21 2023, max compression
```

## Comparing `pyfsdb-viewer-0.3.tar` & `pyfsdb-viewer-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-06-29 21:17:58.031031 pyfsdb-viewer-0.3/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      581 2023-06-29 21:17:58.030031 pyfsdb-viewer-0.3/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      212 2023-05-23 15:38:23.000000 pyfsdb-viewer-0.3/README.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-06-29 21:17:58.030031 pyfsdb-viewer-0.3/pyfsdb_viewer/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 15:40:34.000000 pyfsdb-viewer-0.3/pyfsdb_viewer/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      403 2023-06-21 15:38:50.000000 pyfsdb-viewer-0.3/pyfsdb_viewer/pyfsdb_viewer.css
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     8820 2023-06-21 15:38:50.000000 pyfsdb-viewer-0.3/pyfsdb_viewer/view.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-06-29 21:17:58.030031 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      581 2023-06-29 21:17:57.000000 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      322 2023-06-29 21:17:57.000000 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        1 2023-06-29 21:17:57.000000 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       52 2023-06-29 21:17:57.000000 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/entry_points.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       30 2023-06-29 21:17:57.000000 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/requires.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       14 2023-06-29 21:17:57.000000 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/top_level.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-06-29 21:17:58.031031 pyfsdb-viewer-0.3/setup.cfg
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      979 2023-06-29 21:17:38.000000 pyfsdb-viewer-0.3/setup.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-07-28 23:07:21.470454 pyfsdb-viewer-0.4/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      581 2023-07-28 23:07:21.470454 pyfsdb-viewer-0.4/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      212 2023-06-20 20:07:31.000000 pyfsdb-viewer-0.4/README.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-07-28 23:07:21.469454 pyfsdb-viewer-0.4/pyfsdb_viewer/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        0 2023-06-20 20:07:31.000000 pyfsdb-viewer-0.4/pyfsdb_viewer/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      940 2023-07-28 19:41:26.000000 pyfsdb-viewer-0.4/pyfsdb_viewer/pyfsdb_viewer.css
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)    11251 2023-07-28 20:26:15.000000 pyfsdb-viewer-0.4/pyfsdb_viewer/view.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-07-28 23:07:21.470454 pyfsdb-viewer-0.4/pyfsdb_viewer.egg-info/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      581 2023-07-28 23:07:21.000000 pyfsdb-viewer-0.4/pyfsdb_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      322 2023-07-28 23:07:21.000000 pyfsdb-viewer-0.4/pyfsdb_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        1 2023-07-28 23:07:21.000000 pyfsdb-viewer-0.4/pyfsdb_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       52 2023-07-28 23:07:21.000000 pyfsdb-viewer-0.4/pyfsdb_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       30 2023-07-28 23:07:21.000000 pyfsdb-viewer-0.4/pyfsdb_viewer.egg-info/requires.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       14 2023-07-28 23:07:21.000000 pyfsdb-viewer-0.4/pyfsdb_viewer.egg-info/top_level.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-07-28 23:07:21.470454 pyfsdb-viewer-0.4/setup.cfg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      964 2023-07-28 23:06:29.000000 pyfsdb-viewer-0.4/setup.py
```

### Comparing `pyfsdb-viewer-0.3/PKG-INFO` & `pyfsdb-viewer-0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfsdb-viewer
-Version: 0.3
+Version: 0.4
 Summary: A pyfsdb and textual based viewer
 Home-page: https://github.com/gawseed/pyfsdb-viewer
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyfsdb-viewer-0.3/pyfsdb_viewer/view.py` & `pyfsdb-viewer-0.4/pyfsdb_viewer/view.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,36 +8,60 @@
 import re
 import subprocess
 import tempfile
 from subprocess import Popen, PIPE, STDOUT
 import shlex
 
 from textual.app import App, ComposeResult
-from textual.widgets import Button, DataTable, Static, Header, Label, Footer, TextLog, Input
-from textual.containers import Container, ScrollableContainer, Horizontal
+from textual.widgets import (
+    Button,
+    DataTable,
+    Static,
+    Header,
+    Label,
+    Footer,
+    TextLog,
+    Input,
+)
+from textual.containers import Container, ScrollableContainer, Horizontal, Vertical
+from textual.binding import Binding
 import pyfsdb
 
 
 def parse_args():
     "Parse the command line arguments."
-    parser = ArgumentParser(formatter_class=ArgumentDefaultsHelpFormatter,
-                            description=__doc__,
-                            epilog="Exmaple Usage: pdbview FILE.fsdb")
-
-    parser.add_argument("--log-level", "--ll", default="info",
-                        help="Define the logging verbosity level (debug, info, warning, error, fotal, critical).")
+    parser = ArgumentParser(
+        formatter_class=ArgumentDefaultsHelpFormatter,
+        description=__doc__,
+        epilog="Exmaple Usage: pdbview FILE.fsdb",
+    )
+
+    parser.add_argument(
+        "--log-level",
+        "--ll",
+        default="info",
+        help="Define the logging verbosity level (debug, info, warning, error, fotal, critical).",
+    )
+
+    parser.add_argument(
+        "-n",
+        "--max-rows",
+        default=1024,
+        type=int,
+        help="Maximum number of rows to load at start",
+    )
 
     parser.add_argument("input_file", help="The file to view")
 
     args = parser.parse_args()
     log_level = args.log_level.upper()
-    logging.basicConfig(level=log_level,
-                        format="%(levelname)-10s:\t%(message)s")
+    logging.basicConfig(level=log_level, format="%(levelname)-10s:\t%(message)s")
     return args
 
+
 def run_command_with_arguments(parent_obj, command_name, prompt):
     class RunCommandWithArguments(Input):
         def __init__(self, base_parent, command_name, *args, **kwargs):
             super().__init__(*args, **kwargs)
             self.base_parent = base_parent
             self.command_name = command_name
             self.removeme = self
@@ -50,98 +74,183 @@
     prompter = RunCommandWithArguments(parent_obj, command_name)
     prompter.removeme = parent_obj.mount_cmd_input_and_focus(prompter, prompt)
 
 
 class FsdbView(App):
     "FSDB File Viewer"
 
-    CSS_PATH="pyfsdb_viewer.css"
-    BINDINGS=[("q", "exit", "Quit"),
-              ("h", "show_history", "command History"),
-              ("a", "add_column", "Add column"),
-              ("d", "remove_column", "Delete column"),
-              ("f", "filter", "Filter"),
-              ("e", "eval", "Eval"),
-              ("p", "pipe", "add command"),
-              ("s", "save", "Save"),
-              ("u", "undo", "Undo")]
+    CSS_PATH = "pyfsdb_viewer.css"
+    BINDINGS = [
+        ("q", "exit", "Quit"),
+        ("h", "show_history", "command History"),
+        ("a", "add_column", "Add column"),
+        ("d", "remove_column", "Delete column"),
+        ("f", "filter", "Filter"),
+        ("e", "eval", "Eval"),
+        ("|", "pipe", "add command"),
+        ("l", "load_more_data", "Load more"),
+        Binding("escape", "cancel", "Cancel", show="false"),
+        Binding("z", "show_debug_log", "Debug", show="false"),
+        ("s", "save", "Save"),
+        ("u", "undo", "Undo"),
+    ]
 
     def __init__(self, input_file, *args, **kwargs):
         self.input_file = open(input_file, "r")
         self.input_files = [input_file]
         self.added_comments = False
+        self.current_input = None
+        self.callback = None
+        self.ok_callback = None
+        self.debug_log = []
+
+        self.max_rows = None
+        if "max_rows" in kwargs:
+            self.max_rows = kwargs["max_rows"]
+            del kwargs["max_rows"]
+
         super().__init__(*args, **kwargs)
 
+    def error(self, err_string):
+        "displays an error message (will be a dialog box)"
+        lab = Label(err_string)
+        self.mount_cmd_input_and_focus(
+            lab,
+            prompt="error: ",
+            buttons=["Close"],
+            callback=self.button_cancel,
+        )
+        # error(err_string)
+
     def debug(self, obj):
+        self.debug_log.append(str(obj))
         with open("/tmp/debug.txt", "w") as d:
             d.write(str(obj) + "\n")
 
     def compose(self) -> ComposeResult:
         self.header = Header()
-        
+
         self.ourtitle = Label(self.input_file.name, id="ourtitle")
 
         self.data_table = DataTable(fixed_rows=1, id="fsdbtable")
 
         self.footer = Footer()
 
-        self.container = Container(self.header, self.ourtitle,
-                                   self.data_table, self.footer, id="mainpanel")
+        self.container = Container(
+            self.header, self.ourtitle, self.data_table, self.footer, id="mainpanel"
+        )
         yield self.container
 
     def reload_data(self):
         self.data_table.clear(columns=True)
         self.load_data()
 
     def load_data(self) -> None:
         self.fsh = pyfsdb.Fsdb(file_handle=self.input_file)
         self.data_table.add_columns(*self.fsh.column_names)
-        self.rows = self.fsh.get_all()
-        self.data_table.add_rows(self.rows)
+        self.rows = []
+        self.action_load_more_data()
         self.ourtitle.update(self.input_file.name)
 
+    def action_load_more_data(self) -> None:
+        more_rows = []
+        for n, row in enumerate(self.fsh):
+            more_rows.append(row)
+            if self.max_rows and n == self.max_rows:
+                break
+        self.data_table.add_rows(more_rows)
+        self.rows.extend(more_rows)
+
     def on_mount(self) -> None:
         self.load_data()
         self.data_table.focus()
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
-        self.exit(event.button.id)
+        if self.callback:
+            self.debug(event)
+            self.callback(event)
+            self.callback = None
+            if self.current_input:
+                self.current_input.remove()
+            self.current_input = None
+        else:
+            self.error("unknown button -- internal error")
 
     def action_exit(self):
         self.exit()
 
+    def button_cancel(self, cancel_button):
+        self.debug(cancel_button.control.label)
+        self.action_cancel()
+
+    def button_ok_or_cancel(self, ok_button):
+        self.debug("button here: {ok_button.control.label}")
+        if str(ok_button.control.label).lower() == "ok":
+            self.debug("button here2: {ok_button.control.label}")
+            self.ok_callback(ok_button)
+
+    def action_cancel(self):
+        if self.current_input:
+            self.current_input.remove()
+            self.current_input = None
+        else:
+            self.action_exit()
+
     def action_undo(self):
-        self.debug(self.input_files)
         self.input_files.pop()
-        self.debug(self.input_files[-1])
         self.input_file = open(self.input_files[-1], "r")
         self.data_table.clear(columns=True)
         self.reload_data()
 
     def action_remove_row(self):
-        row_id, _ = self.data_table.coordinate_to_cell_key(self.data_table.cursor_coordinate)
+        row_id, _ = self.data_table.coordinate_to_cell_key(
+            self.data_table.cursor_coordinate
+        )
 
         self.data_table.remove_row(row_id)
 
-    def mount_cmd_input_and_focus(self, widget, prompt="argument: ", show_history=True):
+    def mount_cmd_input_and_focus(
+        self,
+        widget,
+        prompt="argument: ",
+        buttons=[],
+        callback=None,
+        ok_callback=None,
+        class_name="entry_dialog",
+    ):
         "binds a standard input box and mounts after history"
+        debug(widget)
 
         self.label = Label(prompt, classes="entry_label")
 
-        # show the history to date if appropriate
-        if show_history and not self.added_comments:
-            self.action_show_history()
+        container = Vertical(self.label, widget, classes=class_name)
 
-        container = Horizontal(self.label, widget, classes="entry_dialog")
+        self.callback = callback
+        self.ok_callback = ok_callback
+        if not self.callback and self.ok_callback:
+            self.callback = self.button_ok_or_cancel
+
+        # use default buttons if the ok_callback was created
+        if len(buttons) == 0 and self.ok_callback:
+            buttons = ["Ok", "Cancel"]
+
+        if len(buttons) > 0:
+            button_horiz = Horizontal(classes="entry_button_row")
+            for button in buttons:
+                button_widget = Button(button, classes="entry_button")
+                button_horiz.compose_add_child(button_widget)
+
+            container.compose_add_child(button_horiz)
 
         # show the new widget after the history
-        self.mount(container, after = self.history_log)
+        self.mount(container)
 
         # and focus the keyboard toward it
         widget.focus()
+        self.current_input = container
         return container
 
     def action_add_column(self):
         "add a new column to the data with pdbcolcreate"
 
         run_command_with_arguments(self, "dbcolcreate", "column name: ")
 
@@ -151,106 +260,106 @@
         run_command_with_arguments(self, "pdbrow", "pdbrow filter: ")
 
     def action_eval(self):
         "Evaluate rows with a pdbroweval expression"
 
         run_command_with_arguments(self, "pdbroweval", "pdbroweval expr: ")
 
+    def save_current(self, button):
+        current = self.input_file
+        path = str(self.save_info.value)
+        os.rename(self.input_files[-1], path)
+        self.input_file = path
+        self.input_files[-1] = path
+        self.ourtitle.update(path)
+
     def action_save(self):
         "saves the current contents to a new file"
-        class ActionSave(Input):
-            def __init__(self, base_parent, *args, **kwargs):
-                super().__init__(*args, **kwargs)
-                self.base_parent = base_parent
-                self.removeme = self
-
-            def action_submit(self):
-                path = self.value
-                current = self.base_parent.input_file
-                os.rename(self.base_parent.input_files[-1], str(path))
-                self.base_parent.input_file = path
-                self.base_parent.input_files[-1] = path
-                self.removeme.remove()
-
-        self.save_info = ActionSave(self)
-        # TODO: , show_history=False
-        self.save_info.removeme = self.mount_cmd_input_and_focus(self.save_info, "file name:")
+
+        if len(self.input_files) == 1:
+            self.error("Cannot rename the unmodified original file")
+            return
+
+        self.save_info = Input()
+        self.mount_cmd_input_and_focus(
+            self.save_info, "file name:", ok_callback=self.save_current
+        )
 
     def action_remove_column(self):
         "drops the current column by calling dbcol"
         columns = self.data_table.ordered_columns
         new_columns = []
         for n, column in enumerate(columns):
             if self.data_table.cursor_column != n:
                 new_columns.append(str(column.label))
 
         # TODO: allow passing of exact arguments in a list
-        self.run_pipe(['dbcol'] + new_columns)
-        self.debug(new_columns)
+        self.run_pipe(["dbcol"] + new_columns)
+
+    def run_entered_command(self, command):
+        self.run_pipe(self.command_input.value)
 
     def action_pipe(self):
         "prompt for a command to run"
 
-        class CommandInput(Input):
-            def __init__(self, base_parent, *args, **kwargs):
-                super().__init__(*args, **kwargs)
-                self.base_parent = base_parent
-                self.removeme = self
-
-            def action_submit(self):
-                command = self.value
-                self.base_parent.run_pipe(self.value)
-                self.removeme.remove()
-
-        self.command_input = CommandInput(self)
-        self.command_input.removeme = self.mount_cmd_input_and_focus(self.command_input, "command: ")
+        self.command_input = Input()
+        self.mount_cmd_input_and_focus(
+            self.command_input,
+            "command: ",
+            ok_callback=self.run_entered_command,
+        )
 
     def run_pipe(self, command_parts="dbcolcreate foo"):
         "Runs a new command on the data, and re-displays the output file"
-        
+
         if not isinstance(command_parts, list):
             command_parts = shlex.split(command_parts)
-        p = Popen(command_parts, stdout=PIPE, stdin=PIPE, stderr=PIPE)
-        
-        # run the specified command
-        input_file = open(self.input_file.name, "r").read().encode()
-        output_data = p.communicate(input=input_file)
-        with tempfile.NamedTemporaryFile(delete=False) as tmp:
-            self.debug(tmp.name)
-            tmp.write(output_data[0])
-            self.input_files.append(tmp.name)
-            self.input_file = open(tmp.name, "r")
-        self.reload_data()
-        self.action_show_history(force=True)
+
+        try:
+            p = Popen(command_parts, stdout=PIPE, stdin=PIPE, stderr=PIPE)
+
+            # run the specified command
+            input_file = open(self.input_file.name, "r").read().encode()
+            output_data = p.communicate(input=input_file)
+            with tempfile.NamedTemporaryFile(delete=False) as tmp:
+                tmp.write(output_data[0])
+                self.input_files.append(tmp.name)
+                self.input_file = open(tmp.name, "r")
+            self.reload_data()
+        except Exception as e:
+            self.debug(f"failed with {e}")
+
+    def action_show_debug_log(self):
+        self.debug("showing debug log")
+        self.debug_log_ui = TextLog(id="debug_log")
+        for line in self.debug_log:
+            self.debug_log_ui.write(line)
+        self.mount_cmd_input_and_focus(
+            self.debug_log_ui, class_name="text_dialog", buttons=["Close"]
+        )
 
     def action_show_history(self, force=False):
-        "show's the comment history"
-        if self.added_comments:
-            self.history_log.remove()
-            self.added_comments = False
-            if not force:
-                return
-        
-        self.added_comments = True
+        "show's the command history that created the file"
 
+        self.debug("showing history")
         self.history_log = TextLog(id="history")
-        self.mount(self.history_log, after = self.data_table)
-
-        is_command = re.compile("# +\|")
-        count = 0
-        for comment in self.fsh.comments:
-            if is_command.match(comment):
-                count += 1
-                self.history_log.write(comment.strip())
 
-        # needs + 1 (maybe because of footer?)
-        self.history_log.styles.height = count + 1
+        if self.fsh.commands is None:
+            # this means pyfsdb couldn't get them
+            self.history_log.write("[HISTORY UNAVAILABLE]")
+        else:
+            for command in self.fsh.commands:
+                self.history_log.write(command)
+
+        self.mount_cmd_input_and_focus(
+            self.history_log, class_name="text_dialog", buttons=["Close"]
+        )
 
 
 def main():
     args = parse_args()
-    app = FsdbView(args.input_file)
+    app = FsdbView(args.input_file, max_rows=args.max_rows)
     app.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/PKG-INFO` & `pyfsdb-viewer-0.4/pyfsdb_viewer.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfsdb-viewer
-Version: 0.3
+Version: 0.4
 Summary: A pyfsdb and textual based viewer
 Home-page: https://github.com/gawseed/pyfsdb-viewer
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyfsdb-viewer-0.3/setup.py` & `pyfsdb-viewer-0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfsdb-viewer",
-    version="0.3",
+    version="0.4",
     author="Wes Hardaker",
     author_email="opensource@hardakers.net",
     description="A pyfsdb and textual based viewer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gawseed/pyfsdb-viewer",
     packages=setuptools.find_packages(),
@@ -26,11 +26,9 @@
     python_requires=">=3.6",
     test_suite="nose.collector",
     tests_require=["nose"],
     install_requires=[
         "pyfsdb>=2.1.5",
         "textual>=0.26.0",
     ],
-    package_data = {
-        'pyfsdb_viewer': ['pyfsdb_viewer.css']
-    }
+    package_data={"pyfsdb_viewer": ["pyfsdb_viewer.css"]},
 )
```

