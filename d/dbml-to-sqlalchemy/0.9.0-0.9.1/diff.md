# Comparing `tmp/dbml-to-sqlalchemy-0.9.0.tar.gz` & `tmp/dbml-to-sqlalchemy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbml-to-sqlalchemy-0.9.0.tar", last modified: Sat Jul  8 17:36:49 2023, max compression
+gzip compressed data, was "dbml-to-sqlalchemy-0.9.1.tar", last modified: Sat Jul 29 16:55:35 2023, max compression
```

## Comparing `dbml-to-sqlalchemy-0.9.0.tar` & `dbml-to-sqlalchemy-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-08 17:36:49.381875 dbml-to-sqlalchemy-0.9.0/
--rw-r--r--   0 abc        (911) abc        (911)       39 2023-06-25 16:54:03.000000 dbml-to-sqlalchemy-0.9.0/AUTHORS.txt
--rw-r--r--   0 abc        (911) abc        (911)        0 2023-07-08 17:32:27.000000 dbml-to-sqlalchemy-0.9.0/CHANGES.md
--rw-r--r--   0 abc        (911) abc        (911)      450 2023-06-25 16:54:03.000000 dbml-to-sqlalchemy-0.9.0/CLASSIFIERS.txt
--rw-r--r--   0 abc        (911) abc        (911)      175 2023-07-08 17:33:33.000000 dbml-to-sqlalchemy-0.9.0/MANIFEST.in
--rw-r--r--   0 abc        (911) abc        (911)     3400 2023-07-08 17:36:49.381875 dbml-to-sqlalchemy-0.9.0/PKG-INFO
--rw-r--r--   0 abc        (911) abc        (911)     2480 2023-07-08 16:36:37.000000 dbml-to-sqlalchemy-0.9.0/README.md
--rw-r--r--   0 abc        (911) abc        (911)       17 2023-06-25 16:55:43.000000 dbml-to-sqlalchemy-0.9.0/REQUIREMENTS.txt
-drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-08 17:36:49.377875 dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy/
--rw-r--r--   0 abc        (911) abc        (911)       30 2023-07-06 13:28:18.000000 dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy/__init__.py
--rw-r--r--   0 abc        (911) abc        (911)     8282 2023-07-08 17:35:22.000000 dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy/main.py
-drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-08 17:36:49.381875 dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy/mymodel/
--rw-r--r--   0 abc        (911) abc        (911)        0 2023-07-06 14:11:58.000000 dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy/mymodel/__init__.py
-drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-08 17:36:49.381875 dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy.egg-info/
--rw-r--r--   0 abc        (911) abc        (911)     3400 2023-07-08 17:36:49.000000 dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 abc        (911) abc        (911)      433 2023-07-08 17:36:49.000000 dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 abc        (911) abc        (911)        1 2023-07-08 17:36:49.000000 dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 abc        (911) abc        (911)        1 2023-07-08 17:36:49.000000 dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy.egg-info/not-zip-safe
--rw-r--r--   0 abc        (911) abc        (911)       18 2023-07-08 17:36:49.000000 dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 abc        (911) abc        (911)       19 2023-07-08 17:36:49.000000 dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 abc        (911) abc        (911)       38 2023-07-08 17:36:49.381875 dbml-to-sqlalchemy-0.9.0/setup.cfg
--rw-r--r--   0 abc        (911) abc        (911)     1381 2023-07-08 17:32:50.000000 dbml-to-sqlalchemy-0.9.0/setup.py
+drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-29 16:55:35.069022 dbml-to-sqlalchemy-0.9.1/
+-rw-r--r--   0 abc        (911) abc        (911)       39 2023-06-25 16:54:03.000000 dbml-to-sqlalchemy-0.9.1/AUTHORS.txt
+-rw-r--r--   0 abc        (911) abc        (911)      104 2023-07-08 17:52:01.000000 dbml-to-sqlalchemy-0.9.1/CHANGES.md
+-rw-r--r--   0 abc        (911) abc        (911)      450 2023-06-25 16:54:03.000000 dbml-to-sqlalchemy-0.9.1/CLASSIFIERS.txt
+-rw-r--r--   0 abc        (911) abc        (911)      175 2023-07-08 17:33:33.000000 dbml-to-sqlalchemy-0.9.1/MANIFEST.in
+-rw-r--r--   0 abc        (911) abc        (911)     4288 2023-07-29 16:55:35.069022 dbml-to-sqlalchemy-0.9.1/PKG-INFO
+-rw-r--r--   0 abc        (911) abc        (911)     3224 2023-07-09 15:20:47.000000 dbml-to-sqlalchemy-0.9.1/README.md
+-rw-r--r--   0 abc        (911) abc        (911)       17 2023-06-25 16:55:43.000000 dbml-to-sqlalchemy-0.9.1/REQUIREMENTS.txt
+drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-29 16:55:35.069022 dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy/
+-rw-r--r--   0 abc        (911) abc        (911)       30 2023-07-06 13:28:18.000000 dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy/__init__.py
+-rw-r--r--   0 abc        (911) abc        (911)     8735 2023-07-28 16:43:09.000000 dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy/main.py
+drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-29 16:55:35.069022 dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy/mymodel/
+-rw-r--r--   0 abc        (911) abc        (911)        0 2023-07-06 14:11:58.000000 dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy/mymodel/__init__.py
+drwxr-xr-x   0 abc        (911) abc        (911)        0 2023-07-29 16:55:35.069022 dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy.egg-info/
+-rw-r--r--   0 abc        (911) abc        (911)     4288 2023-07-29 16:55:35.000000 dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 abc        (911) abc        (911)      433 2023-07-29 16:55:35.000000 dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 abc        (911) abc        (911)        1 2023-07-29 16:55:35.000000 dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 abc        (911) abc        (911)        1 2023-07-29 16:55:35.000000 dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy.egg-info/not-zip-safe
+-rw-r--r--   0 abc        (911) abc        (911)       18 2023-07-29 16:55:35.000000 dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 abc        (911) abc        (911)       19 2023-07-29 16:55:35.000000 dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 abc        (911) abc        (911)       38 2023-07-29 16:55:35.069022 dbml-to-sqlalchemy-0.9.1/setup.cfg
+-rw-r--r--   0 abc        (911) abc        (911)     1432 2023-07-29 16:55:19.000000 dbml-to-sqlalchemy-0.9.1/setup.py
```

### Comparing `dbml-to-sqlalchemy-0.9.0/PKG-INFO` & `dbml-to-sqlalchemy-0.9.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,108 +1,95 @@
-Metadata-Version: 2.1
-Name: dbml-to-sqlalchemy
-Version: 0.9.0
-Summary: dbml-to-sqlalchemy extension for sqlachemy: upload dbml model in orm sqlalchemy
-Home-page: https://github.com/fraoustin/dbml-to-sqlalchemy.git
-Author: Frédéric Aoustin
-Author-email: fraoustin@gmail.com
-License: UNKNOWN
-Platform: any
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Environment :: Web Environment
-License-File: AUTHORS.txt
-
 # dbml-to-sqlalchemy
 
 generate Model Class SqlAlchemy from database model dbml
 
 
 ## Installation
 
 
-::
-
     pip install dbml-to-sqlalchemy
         
 Or
 
-::
-
     git clone https://github.com/fraoustin/dbml-to-sqlalchemy.git
     cd dbml-to-sqlalchemy
     python setup.py install
 
 You can load test by
 
-::
-
     flake8 --ignore E501,E226,E128,F401
     python -m unittest discover -s tests
 
 
 ## Usage
 
 for sqlalchemy only 
 
-::
-
     import os
     from re import sub
     import sqlalchemy as db
+    from sqlalchemy.orm import Session
     from pydbml import PyDBML
 
     from dbml_to_sqlalchemy import createModel
-
+    from dbml_to_sqlalchemy import mymodel
 
     database_file = "sqlite://"
-    engine = db.create_engine(database_file, echo=True)
+    engine = db.create_engine(database_file, echo=False)
     conn = engine.connect()
     metadata = db.MetaData()
 
 
     try:
         from sqlalchemy.orm import DeclarativeBase
 
         class Base(DeclarativeBase):
             metadata = metadata
     except Exception:
         # for sqlalchemy 1.4
         from sqlalchemy.orm import declarative_base
         Base = declarative_base()
 
-
     source = """
     Table user {
-    id integer [primary key]
-    username varchar
-    role varchar
-    created_at timestamp
+        id integer [pk, increment, note:'key of user']
+        name string [default: 'me', note:'only name']
+        Note: 'Stores user data'
+    }
+
+    Table post {
+        id integer [pk, increment]
+        user_id integer [ref: > user.id]
     }
     """
 
     parsed = PyDBML(source)
 
+
     User = createModel(parsed.tables[0], Base)
-    print(User.__name__)
+    Post = createModel(parsed.tables[1], Base)
+
+    print(User.__doc__)
+    print(Post.__doc__)
 
     metadata.create_all(engine)
 
+    with Session(engine) as session:
+        user = User(id=1)
+        session.add_all([user, ])
+        session.commit()
+        post = Post(id=1, user_id=1)
+        session.add_all([post, ])
+        session.commit()
+        mypost = session.scalars(db.select(Post)).all()[0]
+        print(mypost.user.name)
+
 
-for flask-sqlalchemy
 
-::
+for flask-sqlalchemy
 
     import os
     import logging
     from flask import Flask
     from flask_sqlalchemy import SQLAlchemy
     from pydbml import PyDBML
     from dbml_to_sqlalchemy import createModel, mymodel
@@ -145,9 +132,8 @@
             db.session.add_all([me, ])
             db.session.commit()
         app.logger.setLevel(logging.DEBUG)
         app.run(host='0.0.0.0', port=5000, debug=True)
 
 ## TODO
 
-
-
+manage view from https://github.com/jklukas/sqlalchemy-views (https://stackoverflow.com/questions/9766940/how-to-create-an-sql-view-with-sqlalchemy)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy/main.py` & `dbml-to-sqlalchemy-0.9.1/dbml_to_sqlalchemy/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,66 +77,66 @@
         return '(%s)' % ', '.join(doc)
     return ''
 
 
 def createModel(table, *cls, module=mymodel):
     if len(table.note.text) == 0:
         table.note.text = '%s Table' % toCamelCase(table.name)
-    cols = {col.name: Column(toColumnCase(col.name), getType(col.type)(*getTypeParams(col.type)[0], **getTypeParams(col.type)[1]), primary_key=col.pk, autoincrement=col.autoinc, nullable=not (col.not_null), default=col.default, server_default=getServerDefault(col.default), unique=col.unique) for col in table.columns}
+    cols = {col.name: Column(toColumnCase(col.name), getType(col.type)(*getTypeParams(col.type)[0], **getTypeParams(col.type)[1]), primary_key=col.pk, autoincrement=col.autoinc, nullable=not (col.not_null), default=col.default, server_default=getServerDefault(col.default), unique=col.unique, comment=col.note) for col in table.columns}
     tableArgs = []
     for index in [index for index in table.indexes if index.pk is True]:
         tableArgs.append(PrimaryKeyConstraint(*[cols[col.name] for col in index.subjects]))
     for index in [index for index in table.indexes if index.unique is True]:
         subargs = {}
         if index.name is not None:
             subargs = {'name': index.name}
         tableArgs.append(UniqueConstraint(*[cols[col.name] for col in index.subjects], **subargs))
     SomeClass = type(toCamelCase(table.name), cls, {
         "__tablename__": toTableCase(table.name),
         "__table_args__": tuple(tableArgs),
-        "__doc__": "%s\n\n%s" % (table.note, '\n'.join([":param %s %s: %s %s" % (col.name, col.type, col.note, spec_doc(col)) for col in table.columns])),
+        "__doc__": "%s\n\n%s" % (table.note, '\n'.join([":param %s: %s %s\n:type %s: %s" % (col.name, col.note, spec_doc(col), col.name, col.type) for col in table.columns])),
         **cols
     })
     setattr(module, toCamelCase(table.name), SomeClass)
     for ref in [ref for ref in table.database.refs if (ref.table1 == table or ref.table2 == table) and getattr(module, toCamelCase(ref.col2[0].table.name), None) is not None and getattr(module, toCamelCase(ref.col1[0].table.name), None) is not None]:
         class1 = getattr(module, toCamelCase(ref.table1.name))
         class2 = getattr(module, toCamelCase(ref.table2.name))
         if ref.type in ('<'):
             class2.__table_args__ = class2.__table_args__ + (ForeignKeyConstraint([getattr(class2, col.name) for col in ref.col2], [getattr(class1, col.name) for col in ref.col1], name=ref.name), )
         if ref.type in ('>', '-'):
             class1.__table_args__ = class1.__table_args__ + (ForeignKeyConstraint([getattr(class1, col.name) for col in ref.col1], [getattr(class2, col.name) for col in ref.col2], name=ref.name), )
         if ref.type == '<':
             setattr(class1, "%ss" % class2.__name__.lower(), relationship(class2.__name__, back_populates=class1.__name__.lower()))
-            class1.__doc__ = class1.__doc__ + "\n:param %ss List(%s):" % (class2.__name__.lower(), class2.__name__)
+            class1.__doc__ = class1.__doc__ + "\n:param %ss:\n:type %ss: relationship(%s)" % (class2.__name__.lower(), class2.__name__.lower(), class2.__name__)
             setattr(class2, class1.__name__.lower(), relationship(class1.__name__, back_populates="%ss" % class2.__name__.lower()))
-            class2.__doc__ = class2.__doc__ + "\n:param %s %s:" % (class1.__name__.lower(), class1.__name__)
+            class2.__doc__ = class2.__doc__ + "\n:param %s :\n:type %s: %s" % (class1.__name__.lower(), class1.__name__.lower(), class1.__name__)
         elif ref.type == '>':
             setattr(class1, class2.__name__.lower(), relationship(class2.__name__, back_populates="%ss" % class1.__name__.lower()))
-            class1.__doc__ = class1.__doc__ + "\n:param %s %s:" % (class2.__name__.lower(), class2.__name__)
+            class1.__doc__ = class1.__doc__ + "\n:param %s:\n:type %s: %s" % (class2.__name__.lower(), class2.__name__.lower(), class2.__name__)
             setattr(class2, "%ss" % class1.__name__.lower(), relationship(class1.__name__, back_populates=class2.__name__.lower()))
-            class2.__doc__ = class2.__doc__ + "\n:param %ss List(%s):" % (class1.__name__.lower(), class1.__name__)
+            class2.__doc__ = class2.__doc__ + "\n:param %ss:\n:type %ss: relationship(%s):" % (class1.__name__.lower(), class1.__name__.lower(), class1.__name__)
         elif ref.type == '-':
             setattr(class1, class2.__name__.lower(), relationship(class2.__name__, uselist=False, back_populates=class1.__name__.lower()))
             setattr(class2, class1.__name__.lower(), relationship(class1.__name__, uselist=False, back_populates=class2.__name__.lower()))
         if ref.type == '<>':
             newt_name = "%s_%s" % (ref.table1.name, ref.table2.name)
             newt_col1 = "\n".join(["%s_%s %s" % (col.table.name, col.name, col.type) for col in ref.col1])
             newt_col2 = "\n".join(["%s_%s %s" % (col.table.name, col.name, col.type) for col in ref.col2])
             newt_pk = "%s, %s" % ("\n".join(["%s_%s" % (col.table.name, col.name) for col in ref.col1]), "\n".join(["%s_%s" % (col.table.name, col.name) for col in ref.col2]))
             new_table = "Table %s\n{\n%s\n%s\nindexes {\n(%s) [pk]\n}\n}" % (newt_name, newt_col1, newt_col2, newt_pk)
             newt = createModel(PyDBML(new_table).tables[0], *cls, module=module)
             newt.__table_args__ = newt.__table_args__ + (ForeignKeyConstraint([getattr(newt, "%s_%s" % (col.table.name, col.name)) for col in ref.col1], [getattr(class1, col.name) for col in ref.col1]), )
             newt.__table_args__ = newt.__table_args__ + (ForeignKeyConstraint([getattr(newt, "%s_%s" % (col.table.name, col.name)) for col in ref.col2], [getattr(class2, col.name) for col in ref.col2]), )
             setattr(class1, "%ss" % newt.__name__.lower(), relationship(newt.__name__, back_populates=class1.__name__.lower()))
-            class1.__doc__ = class1.__doc__ + "\n:param %ss List(%s):" % (newt.__name__.lower(), newt.__name__)
+            class1.__doc__ = class1.__doc__ + "\n:param %ss:\n:type %ss: relationship(%s)" % (newt.__name__.lower(), newt.__name__.lower(), newt.__name__)
             setattr(newt, class1.__name__.lower(), relationship(class1.__name__, back_populates="%ss" % newt.__name__.lower()))
-            newt.__doc__ = newt.__doc__ + "\n:param %s %s:" % (class1.__name__.lower(), class1.__name__)
+            newt.__doc__ = newt.__doc__ + "\n:param %s:\n:type %s: %s" % (class1.__name__.lower(), class1.__name__.lower(), class1.__name__)
             setattr(class2, "%ss" % newt.__name__.lower(), relationship(newt.__name__, back_populates=class2.__name__.lower()))
-            class2.__doc__ = class2.__doc__ + "\n:param %ss List(%s):" % (newt.__name__.lower(), newt.__name__)
+            class2.__doc__ = class2.__doc__ + "\n:param %ss:\n:type %ss: relationship(%s):" % (newt.__name__.lower(), newt.__name__.lower(), newt.__name__)
             setattr(newt, class2.__name__.lower(), relationship(class2.__name__, back_populates="%ss" % newt.__name__.lower()))
-            newt.__doc__ = newt.__doc__ + "\n:param %s %s:" % (class2.__name__.lower(), class2.__name__)
+            newt.__doc__ = newt.__doc__ + "\n:param %s:\n:type %s: %s:" % (class2.__name__.lower(), class2.__name__.lower(), class2.__name__)
             setattr(class1, "%ss" % class2.__name__.lower(), spec_many("%ss" % newt.__name__.lower(), class2.__name__.lower()))
-            class1.__doc__ = class1.__doc__ + "\n:param %ss List(%s):" % (class2.__name__.lower(), class2.__name__)
+            class1.__doc__ = class1.__doc__ + "\n:param %ss:\n:type %ss: relationship(%s)" % (class2.__name__.lower(), class2.__name__.lower(), class2.__name__)
             setattr(class2, "%ss" % class1.__name__.lower(), spec_many("%ss" % newt.__name__.lower(), class1.__name__.lower()))
-            class2.__doc__ = class2.__doc__ + "\n:param %ss List(%s):" % (class1.__name__.lower(), class1.__name__)
+            class2.__doc__ = class2.__doc__ + "\n:param %ss:\n:type %ss: relationship(%s)" % (class1.__name__.lower(), class1.__name__.lower(), class1.__name__)
             setattr(module, newt.__name__, newt)
     return getattr(module, toCamelCase(table.name))
```

### Comparing `dbml-to-sqlalchemy-0.9.0/dbml_to_sqlalchemy.egg-info/PKG-INFO` & `dbml-to-sqlalchemy-0.9.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbml-to-sqlalchemy
-Version: 0.9.0
+Version: 0.9.1
 Summary: dbml-to-sqlalchemy extension for sqlachemy: upload dbml model in orm sqlalchemy
 Home-page: https://github.com/fraoustin/dbml-to-sqlalchemy.git
 Author: Frédéric Aoustin
 Author-email: fraoustin@gmail.com
 License: UNKNOWN
 Platform: any
 Classifier: Programming Language :: Python
@@ -14,95 +14,105 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
+Description-Content-Type: text/markdown
 License-File: AUTHORS.txt
 
 # dbml-to-sqlalchemy
 
 generate Model Class SqlAlchemy from database model dbml
 
 
 ## Installation
 
 
-::
-
     pip install dbml-to-sqlalchemy
         
 Or
 
-::
-
     git clone https://github.com/fraoustin/dbml-to-sqlalchemy.git
     cd dbml-to-sqlalchemy
     python setup.py install
 
 You can load test by
 
-::
-
     flake8 --ignore E501,E226,E128,F401
     python -m unittest discover -s tests
 
 
 ## Usage
 
 for sqlalchemy only 
 
-::
-
     import os
     from re import sub
     import sqlalchemy as db
+    from sqlalchemy.orm import Session
     from pydbml import PyDBML
 
     from dbml_to_sqlalchemy import createModel
-
+    from dbml_to_sqlalchemy import mymodel
 
     database_file = "sqlite://"
-    engine = db.create_engine(database_file, echo=True)
+    engine = db.create_engine(database_file, echo=False)
     conn = engine.connect()
     metadata = db.MetaData()
 
 
     try:
         from sqlalchemy.orm import DeclarativeBase
 
         class Base(DeclarativeBase):
             metadata = metadata
     except Exception:
         # for sqlalchemy 1.4
         from sqlalchemy.orm import declarative_base
         Base = declarative_base()
 
-
     source = """
     Table user {
-    id integer [primary key]
-    username varchar
-    role varchar
-    created_at timestamp
+        id integer [pk, increment, note:'key of user']
+        name string [default: 'me', note:'only name']
+        Note: 'Stores user data'
+    }
+
+    Table post {
+        id integer [pk, increment]
+        user_id integer [ref: > user.id]
     }
     """
 
     parsed = PyDBML(source)
 
+
     User = createModel(parsed.tables[0], Base)
-    print(User.__name__)
+    Post = createModel(parsed.tables[1], Base)
+
+    print(User.__doc__)
+    print(Post.__doc__)
 
     metadata.create_all(engine)
 
+    with Session(engine) as session:
+        user = User(id=1)
+        session.add_all([user, ])
+        session.commit()
+        post = Post(id=1, user_id=1)
+        session.add_all([post, ])
+        session.commit()
+        mypost = session.scalars(db.select(Post)).all()[0]
+        print(mypost.user.name)
+
 
-for flask-sqlalchemy
 
-::
+for flask-sqlalchemy
 
     import os
     import logging
     from flask import Flask
     from flask_sqlalchemy import SQLAlchemy
     from pydbml import PyDBML
     from dbml_to_sqlalchemy import createModel, mymodel
@@ -145,9 +155,22 @@
             db.session.add_all([me, ])
             db.session.commit()
         app.logger.setLevel(logging.DEBUG)
         app.run(host='0.0.0.0', port=5000, debug=True)
 
 ## TODO
 
+manage view from https://github.com/jklukas/sqlalchemy-views (https://stackoverflow.com/questions/9766940/how-to-create-an-sql-view-with-sqlalchemy)
+
+# Feature
+
+- generate documentation
+- TODO
+
+# V. 0.9.1
+
+- add sample in README
+
+# V. 0.9.0
 
+- init repos
```

### Comparing `dbml-to-sqlalchemy-0.9.0/setup.py` & `dbml-to-sqlalchemy-0.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Setup for dbml-to-sqlalchemy
 """
 
 import os
 from setuptools import setup, find_packages
 
-__version_info__ = (0, 9, 0)
+__version_info__ = (0, 9, 1)
 VERSION = '.'.join([str(val) for val in __version_info__])
 NAME = "dbml-to-sqlalchemy"
 DESC = "dbml-to-sqlalchemy extension for sqlachemy: upload dbml model in orm sqlalchemy"
 URLPKG = "https://github.com/fraoustin/dbml-to-sqlalchemy.git"
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
@@ -35,14 +35,15 @@
     name=NAME,
     version=VERSION,
     packages=find_packages(),
     author=AUTHORS,
     author_email=AUTHORS_EMAIL,
     description=DESC,
     long_description=LONG_DESC,
+    long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=REQUIRED,
     url=URLPKG,
     classifiers=CLASSIFIED,
     entry_points={},
     zip_safe=False,
     platforms='any'
```

