# Comparing `tmp/jedi-0.8.1-final0.tar.gz` & `tmp/jedi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jedi-0.8.1-final0.tar", last modified: Tue Jul 22 23:04:24 2014, max compression
+gzip compressed data, was "dist/jedi-0.9.0.tar", last modified: Tue Apr 28 17:03:47 2015, max compression
```

## Comparing `jedi-0.8.1-final0.tar` & `jedi-0.9.0.tar`

### file list

```diff
@@ -1,247 +1,289 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/
--rw-rw-r--   0 david     (1000) david     (1000)      390 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/pytest.ini
--rwxrwxr-x   0 david     (1000) david     (1000)     7100 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/sith.py
--rw-rw-r--   0 david     (1000) david     (1000)      955 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/AUTHORS.txt
--rw-rw-r--   0 david     (1000) david     (1000)     8803 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      290 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)      566 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/tox.ini
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/docs/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/docs/_screenshots/
--rw-rw-r--   0 david     (1000) david     (1000)    22041 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/_screenshots/screenshot_pydoc.png
--rw-rw-r--   0 david     (1000) david     (1000)    17109 2013-08-18 16:18:22.000000 jedi-0.8.1-final0/docs/_screenshots/screenshot_complete.png
--rw-rw-r--   0 david     (1000) david     (1000)    40035 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/_screenshots/screenshot_function.png
--rw-rw-r--   0 david     (1000) david     (1000)     9201 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/docs/conf.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/docs/_templates/
--rw-rw-r--   0 david     (1000) david     (1000)      136 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/_templates/sidebarlogo.html
--rw-rw-r--   0 david     (1000) david     (1000)      230 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/_templates/ghbuttons.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/docs/_static/
--rw-rw-r--   0 david     (1000) david     (1000)      122 2013-08-18 16:18:22.000000 jedi-0.8.1-final0/docs/_static/logo-src.txt
--rw-rw-r--   0 david     (1000) david     (1000)    28795 2013-08-18 16:18:22.000000 jedi-0.8.1-final0/docs/_static/logo.png
--rw-rw-r--   0 david     (1000) david     (1000)       37 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/global.rst
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/docs/docs/
--rw-rw-r--   0 david     (1000) david     (1000)     2103 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/docs/docs/plugin-api.rst
--rw-rw-r--   0 david     (1000) david     (1000)     2061 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/docs/docs/usage.rst
--rw-rw-r--   0 david     (1000) david     (1000)     2559 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/docs/docs/installation.rst
--rw-rw-r--   0 david     (1000) david     (1000)     5562 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/docs/docs/features.rst
--rw-rw-r--   0 david     (1000) david     (1000)      865 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/docs/docs/testing.rst
--rw-rw-r--   0 david     (1000) david     (1000)      159 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/docs/docs/plugin-api-classes.rst
--rw-rw-r--   0 david     (1000) david     (1000)       77 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/docs/docs/settings.rst
--rw-rw-r--   0 david     (1000) david     (1000)     5661 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/docs/docs/development.rst
--rw-rw-r--   0 david     (1000) david     (1000)      749 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/docs/index.rst
--rw-rw-r--   0 david     (1000) david     (1000)     5556 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/Makefile
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/docs/_themes/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/docs/_themes/flask/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/docs/_themes/flask/static/
--rw-rw-r--   0 david     (1000) david     (1000)     6411 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/_themes/flask/static/flasky.css_t
--rw-rw-r--   0 david     (1000) david     (1000)      976 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/_themes/flask/static/small_flask.css
--rw-rw-r--   0 david     (1000) david     (1000)      971 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/_themes/flask/layout.html
--rw-rw-r--   0 david     (1000) david     (1000)     1789 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/_themes/flask/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)      162 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/_themes/flask/theme.conf
--rw-rw-r--   0 david     (1000) david     (1000)      590 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/_themes/flask/relations.html
--rw-rw-r--   0 david     (1000) david     (1000)     6672 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/docs/_themes/flask_theme_support.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/refactor/
--rw-rw-r--   0 david     (1000) david     (1000)      697 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/refactor/extract.py
--rw-rw-r--   0 david     (1000) david     (1000)      287 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/refactor/rename.py
--rw-rw-r--   0 david     (1000) david     (1000)      246 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/refactor/inline.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_api/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_api/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     5549 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_api/test_api_classes.py
--rw-rw-r--   0 david     (1000) david     (1000)     2147 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_api/test_unicode.py
--rw-rw-r--   0 david     (1000) david     (1000)     2017 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_api/test_api_classes_follow_definition.py
--rw-rw-r--   0 david     (1000) david     (1000)     7855 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_api/test_call_signatures.py
--rw-rw-r--   0 david     (1000) david     (1000)     3545 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_api/test_api.py
--rw-rw-r--   0 david     (1000) david     (1000)     3079 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_api/test_interpreter.py
--rw-rw-r--   0 david     (1000) david     (1000)     2385 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_api/test_full_name.py
--rw-rw-r--   0 david     (1000) david     (1000)     2421 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_api/test_defined_names.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_parser/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_parser/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1907 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_parser/test_get_code.py
--rw-rw-r--   0 david     (1000) david     (1000)      602 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_parser/test_token.py
--rw-rw-r--   0 david     (1000) david     (1000)     1863 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_parser/test_fast_parser.py
--rw-rw-r--   0 david     (1000) david     (1000)      244 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_parser/test_representation.py
--rw-rw-r--   0 david     (1000) david     (1000)     4220 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_parser/test_parser.py
--rw-rw-r--   0 david     (1000) david     (1000)      147 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_parser/test_user_context.py
--rw-rw-r--   0 david     (1000) david     (1000)        0 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      768 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_integration_keyword.py
--rw-rw-r--   0 david     (1000) david     (1000)     3500 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_utils.py
--rwxrwxr-x   0 david     (1000) david     (1000)    12845 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/run.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/speed/
--rw-rw-r--   0 david     (1000) david     (1000)      647 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/speed/precedence.py
--rw-rw-r--   0 david     (1000) david     (1000)     3029 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_cache.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/static_analysis/
--rw-rw-r--   0 david     (1000) david     (1000)     2102 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/static_analysis/star_arguments.py
--rw-rw-r--   0 david     (1000) david     (1000)      134 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/static_analysis/operations.py
--rw-rw-r--   0 david     (1000) david     (1000)      245 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/static_analysis/descriptors.py
--rw-rw-r--   0 david     (1000) david     (1000)     1150 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/static_analysis/arguments.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/static_analysis/import_tree/
--rw-rw-r--   0 david     (1000) david     (1000)       16 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/static_analysis/import_tree/a.py
--rw-rw-r--   0 david     (1000) david     (1000)       98 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/static_analysis/import_tree/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)        0 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/static_analysis/import_tree/b.py
--rw-rw-r--   0 david     (1000) david     (1000)     1432 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/static_analysis/try_except.py
--rw-rw-r--   0 david     (1000) david     (1000)      738 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/static_analysis/attribute_warnings.py
--rw-rw-r--   0 david     (1000) david     (1000)     2087 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/static_analysis/attribute_error.py
--rw-rw-r--   0 david     (1000) david     (1000)       94 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/static_analysis/generators.py
--rw-rw-r--   0 david     (1000) david     (1000)      378 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/static_analysis/imports.py
--rw-rw-r--   0 david     (1000) david     (1000)     1519 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_integration.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/completion/
--rw-rw-r--   0 david     (1000) david     (1000)     2662 2013-08-18 16:18:23.000000 jedi-0.8.1-final0/test/completion/descriptors.py
--rw-rw-r--   0 david     (1000) david     (1000)     6313 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/completion/functions.py
--rw-rw-r--   0 david     (1000) david     (1000)       77 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      197 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/completion/complex.py
--rw-rw-r--   0 david     (1000) david     (1000)     1905 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/completion/ordering.py
--rw-rw-r--   0 david     (1000) david     (1000)     2526 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/completion/goto.py
--rw-rw-r--   0 david     (1000) david     (1000)     1107 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/types.py
--rw-rw-r--   0 david     (1000) david     (1000)     4900 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/completion/basic.py
--rw-rw-r--   0 david     (1000) david     (1000)     6696 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/completion/classes.py
--rw-rw-r--   0 david     (1000) david     (1000)     1779 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/completion/precedence.py
--rw-rw-r--   0 david     (1000) david     (1000)       55 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/keywords.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/completion/import_tree/
--rw-rw-r--   0 david     (1000) david     (1000)       62 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/import_tree/random.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/completion/import_tree/pkg/
--rw-rw-r--   0 david     (1000) david     (1000)       29 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/import_tree/pkg/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)        8 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/import_tree/pkg/mod1.py
--rw-rw-r--   0 david     (1000) david     (1000)        7 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/completion/import_tree/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)       59 2013-08-18 16:18:23.000000 jedi-0.8.1-final0/test/completion/import_tree/recurse_class2.py
--rw-rw-r--   0 david     (1000) david     (1000)       41 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/import_tree/rename1.py
--rw-rw-r--   0 david     (1000) david     (1000)       44 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/import_tree/mod1.py
--rw-rw-r--   0 david     (1000) david     (1000)       80 2013-08-18 16:18:23.000000 jedi-0.8.1-final0/test/completion/import_tree/recurse_class1.py
--rw-rw-r--   0 david     (1000) david     (1000)       63 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/import_tree/rename2.py
--rw-rw-r--   0 david     (1000) david     (1000)       27 2013-08-18 16:18:23.000000 jedi-0.8.1-final0/test/completion/import_tree/mod2.py
--rw-rw-r--   0 david     (1000) david     (1000)     1135 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/completion/lambdas.py
--rw-rw-r--   0 david     (1000) david     (1000)     4843 2013-08-18 16:18:23.000000 jedi-0.8.1-final0/test/completion/decorators.py
--rw-rw-r--   0 david     (1000) david     (1000)      219 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/completion/named_param.py
--rw-rw-r--   0 david     (1000) david     (1000)      627 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/completion/parser.py
--rw-rw-r--   0 david     (1000) david     (1000)     2379 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/completion/docstring.py
--rw-rw-r--   0 david     (1000) david     (1000)     4695 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/completion/usages.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/completion/thirdparty/
--rw-rw-r--   0 david     (1000) david     (1000)      212 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/thirdparty/django_.py
--rw-rw-r--   0 david     (1000) david     (1000)      320 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/thirdparty/PyQt4_.py
--rw-rw-r--   0 david     (1000) david     (1000)     1474 2013-08-18 16:18:23.000000 jedi-0.8.1-final0/test/completion/thirdparty/jedi_.py
--rw-rw-r--   0 david     (1000) david     (1000)      134 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/thirdparty/psycopg2_.py
--rw-rw-r--   0 david     (1000) david     (1000)      544 2013-05-11 06:23:15.000000 jedi-0.8.1-final0/test/completion/thirdparty/pylab_.py
--rw-rw-r--   0 david     (1000) david     (1000)      975 2013-08-18 16:18:23.000000 jedi-0.8.1-final0/test/completion/definition.py
--rw-rw-r--   0 david     (1000) david     (1000)     1060 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/completion/isinstance.py
--rw-rw-r--   0 david     (1000) david     (1000)     2046 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/completion/invalid.py
--rw-rw-r--   0 david     (1000) david     (1000)      431 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/completion/sys_path.py
--rw-rw-r--   0 david     (1000) david     (1000)     1887 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/completion/generators.py
--rw-rw-r--   0 david     (1000) david     (1000)     5595 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/completion/dynamic.py
--rw-rw-r--   0 david     (1000) david     (1000)     4220 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/completion/arrays.py
--rw-rw-r--   0 david     (1000) david     (1000)     5243 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/completion/imports.py
--rw-rw-r--   0 david     (1000) david     (1000)     2085 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/completion/stdlib.py
--rw-rw-r--   0 david     (1000) david     (1000)     1866 2013-08-18 16:18:23.000000 jedi-0.8.1-final0/test/test_jedi_system.py
--rw-rw-r--   0 david     (1000) david     (1000)     2545 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_integration_import.py
--rw-rw-r--   0 david     (1000) david     (1000)     1870 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_speed.py
--rw-rw-r--   0 david     (1000) david     (1000)      209 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_debug.py
--rw-rw-r--   0 david     (1000) david     (1000)     5398 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_regression.py
--rwxrwxr-x   0 david     (1000) david     (1000)     3478 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/refactor.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/
--rw-rw-r--   0 david     (1000) david     (1000)     1684 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/test_pyc.py
--rw-rw-r--   0 david     (1000) david     (1000)     2193 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/test_namespace_package.py
--rw-rw-r--   0 david     (1000) david     (1000)        0 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1856 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_evaluate/test_buildout_detection.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns1/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns1/pkg/
--rw-rw-r--   0 david     (1000) david     (1000)      214 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns1/pkg/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns1/pkg/ns1_folder/
--rw-rw-r--   0 david     (1000) david     (1000)       20 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns1/pkg/ns1_folder/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)       18 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns1/pkg/ns1_file.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns2/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns2/pkg/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns2/pkg/ns2_folder/
--rw-rw-r--   0 david     (1000) david     (1000)       20 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns2/pkg/ns2_folder/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns2/pkg/ns2_folder/nested/
--rw-rw-r--   0 david     (1000) david     (1000)       16 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns2/pkg/ns2_folder/nested/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)       18 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/namespace_package/ns2/pkg/ns2_file.py
--rw-rw-r--   0 david     (1000) david     (1000)     1692 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_evaluate/test_compiled.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/absolute_import/
--rw-rw-r--   0 david     (1000) david     (1000)      437 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/absolute_import/unittest.py
--rw-rw-r--   0 david     (1000) david     (1000)      383 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/absolute_import/local_module.py
--rw-rw-r--   0 david     (1000) david     (1000)     2524 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/test_docstring.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/buildout_project/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/buildout_project/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/buildout_project/src/proj_name/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_evaluate/buildout_project/src/proj_name/module_name.py
--rw-rw-r--   0 david     (1000) david     (1000)        0 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_evaluate/buildout_project/buildout.cfg
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/buildout_project/bin/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_evaluate/buildout_project/bin/empty_file
--rw-rw-r--   0 david     (1000) david     (1000)      227 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_evaluate/buildout_project/bin/app
--rw-rw-r--   0 david     (1000) david     (1000)      664 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_evaluate/test_extension.py
--rw-rw-r--   0 david     (1000) david     (1000)     1207 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/test_absolute_import.py
--rw-rw-r--   0 david     (1000) david     (1000)      610 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/test_evaluate/test_representation.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/not_in_sys_path/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/not_in_sys_path/not_in_sys_path_package/
--rw-rw-r--   0 david     (1000) david     (1000)       18 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/not_in_sys_path/not_in_sys_path_package/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)       25 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/not_in_sys_path/not_in_sys_path_package/module.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/test/test_evaluate/not_in_sys_path/pkg/
--rw-rw-r--   0 david     (1000) david     (1000)      163 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/not_in_sys_path/pkg/module.py
--rw-rw-r--   0 david     (1000) david     (1000)       10 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/not_in_sys_path/not_in_sys_path.py
--rw-rw-r--   0 david     (1000) david     (1000)      723 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/test_imports.py
--rw-rw-r--   0 david     (1000) david     (1000)     2282 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/test/test_evaluate/test_precedence.py
--rw-rw-r--   0 david     (1000) david     (1000)     1029 2013-08-18 16:18:23.000000 jedi-0.8.1-final0/test/helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)     5125 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/test/conftest.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/jedi/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/jedi/evaluate/
--rw-rw-r--   0 david     (1000) david     (1000)     5675 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/recursion.py
--rw-rw-r--   0 david     (1000) david     (1000)    15914 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     9987 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/precedence.py
--rw-rw-r--   0 david     (1000) david     (1000)    21646 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/representation.py
--rw-rw-r--   0 david     (1000) david     (1000)     7855 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/analysis.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/jedi/evaluate/compiled/
--rw-rw-r--   0 david     (1000) david     (1000)    13463 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/compiled/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/jedi/evaluate/compiled/fake/
--rw-rw-r--   0 david     (1000) david     (1000)       77 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/jedi/evaluate/compiled/fake/datetime.pym
--rw-rw-r--   0 david     (1000) david     (1000)     4913 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/compiled/fake/builtins.pym
--rw-rw-r--   0 david     (1000) david     (1000)      201 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/jedi/evaluate/compiled/fake/_weakref.pym
--rw-rw-r--   0 david     (1000) david     (1000)     3019 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/compiled/fake/_sre.pym
--rw-rw-r--   0 david     (1000) david     (1000)      489 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/jedi/evaluate/compiled/fake/_sqlite3.pym
--rw-rw-r--   0 david     (1000) david     (1000)      342 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/compiled/fake/_functools.pym
--rw-rw-r--   0 david     (1000) david     (1000)       58 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/jedi/evaluate/compiled/fake/posix.pym
--rw-rw-r--   0 david     (1000) david     (1000)       81 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/jedi/evaluate/compiled/fake/io.pym
--rw-rw-r--   0 david     (1000) david     (1000)     3742 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/jedi/evaluate/compiled/fake.py
--rw-rw-r--   0 david     (1000) david     (1000)     7446 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)     4492 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/jedi/evaluate/docstrings.py
--rw-rw-r--   0 david     (1000) david     (1000)     6864 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/sys_path.py
--rw-rw-r--   0 david     (1000) david     (1000)    22191 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/finder.py
--rw-rw-r--   0 david     (1000) david     (1000)    15137 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/param.py
--rw-rw-r--   0 david     (1000) david     (1000)     5747 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/dynamic.py
--rw-rw-r--   0 david     (1000) david     (1000)    22487 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/imports.py
--rw-rw-r--   0 david     (1000) david     (1000)    18885 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/iterable.py
--rw-rw-r--   0 david     (1000) david     (1000)     4097 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/evaluate/stdlib.py
--rw-rw-r--   0 david     (1000) david     (1000)     1898 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/jedi/evaluate/cache.py
--rw-rw-r--   0 david     (1000) david     (1000)     1511 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1322 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/__main__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/jedi/parser/
--rw-rw-r--   0 david     (1000) david     (1000)    26029 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/parser/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    16500 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/parser/fast.py
--rw-rw-r--   0 david     (1000) david     (1000)    53858 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/parser/representation.py
--rw-rw-r--   0 david     (1000) david     (1000)     9158 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/parser/user_context.py
--rw-rw-r--   0 david     (1000) david     (1000)    10438 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/parser/tokenize.py
--rw-rw-r--   0 david     (1000) david     (1000)     4083 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/jedi/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)     7043 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/refactoring.py
--rw-rw-r--   0 david     (1000) david     (1000)     5332 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/_compatibility.py
--rw-rw-r--   0 david     (1000) david     (1000)     5047 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/common.py
--rw-rw-r--   0 david     (1000) david     (1000)     6243 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/settings.py
--rw-rw-r--   0 david     (1000) david     (1000)     2432 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/jedi/debug.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/jedi/api/
--rw-rw-r--   0 david     (1000) david     (1000)    29148 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/api/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    25964 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/api/classes.py
--rw-rw-r--   0 david     (1000) david     (1000)     2354 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/jedi/api/keywords.py
--rw-rw-r--   0 david     (1000) david     (1000)     4091 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/api/usages.py
--rw-rw-r--   0 david     (1000) david     (1000)      832 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/api/replstartup.py
--rw-rw-r--   0 david     (1000) david     (1000)     1407 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/api/helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)     3616 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/api/interpreter.py
--rw-rw-r--   0 david     (1000) david     (1000)    10729 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/jedi/cache.py
--rw-rw-r--   0 david     (1000) david     (1000)       59 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)      421 2013-05-11 06:23:14.000000 jedi-0.8.1-final0/.coveragerc
--rw-rw-r--   0 david     (1000) david     (1000)     1521 2014-05-04 22:34:52.000000 jedi-0.8.1-final0/conftest.py
--rwxrwxr-x   0 david     (1000) david     (1000)     1732 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/setup.py
--rw-rw-r--   0 david     (1000) david     (1000)     5088 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/README.rst
--rw-rw-r--   0 david     (1000) david     (1000)     1122 2014-07-22 23:03:50.000000 jedi-0.8.1-final0/CHANGELOG.rst
--rw-rw-r--   0 david     (1000) david     (1000)     1111 2013-08-18 16:18:22.000000 jedi-0.8.1-final0/LICENSE.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/jedi.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     8803 2014-07-22 23:04:22.000000 jedi-0.8.1-final0/jedi.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)        1 2014-07-22 23:04:22.000000 jedi-0.8.1-final0/jedi.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        5 2014-07-22 23:04:22.000000 jedi-0.8.1-final0/jedi.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)     6218 2014-07-22 23:04:24.000000 jedi-0.8.1-final0/jedi.egg-info/SOURCES.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/
+-rw-rw-r--   0 david     (1000) david     (1000)      454 2015-04-28 17:03:23.000000 jedi-0.9.0/pytest.ini
+-rwxrwxr-x   0 david     (1000) david     (1000)     7100 2014-05-04 22:34:52.000000 jedi-0.9.0/sith.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1244 2015-04-28 17:03:23.000000 jedi-0.9.0/AUTHORS.txt
+-rw-rw-r--   0 david     (1000) david     (1000)    11151 2015-04-28 17:03:47.000000 jedi-0.9.0/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      323 2015-04-28 17:03:23.000000 jedi-0.9.0/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)      737 2015-04-28 17:03:23.000000 jedi-0.9.0/tox.ini
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/docs/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/docs/_screenshots/
+-rw-rw-r--   0 david     (1000) david     (1000)    22041 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/_screenshots/screenshot_pydoc.png
+-rw-rw-r--   0 david     (1000) david     (1000)    17109 2013-08-18 16:18:22.000000 jedi-0.9.0/docs/_screenshots/screenshot_complete.png
+-rw-rw-r--   0 david     (1000) david     (1000)    40035 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/_screenshots/screenshot_function.png
+-rw-rw-r--   0 david     (1000) david     (1000)     9201 2014-05-04 22:34:52.000000 jedi-0.9.0/docs/conf.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/docs/_templates/
+-rw-rw-r--   0 david     (1000) david     (1000)      136 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/_templates/sidebarlogo.html
+-rw-rw-r--   0 david     (1000) david     (1000)      230 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/_templates/ghbuttons.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/docs/_static/
+-rw-rw-r--   0 david     (1000) david     (1000)      122 2013-08-18 16:18:22.000000 jedi-0.9.0/docs/_static/logo-src.txt
+-rw-rw-r--   0 david     (1000) david     (1000)    28795 2013-08-18 16:18:22.000000 jedi-0.9.0/docs/_static/logo.png
+-rw-rw-r--   0 david     (1000) david     (1000)       37 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/global.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/docs/docs/
+-rw-rw-r--   0 david     (1000) david     (1000)     2103 2014-05-04 22:34:52.000000 jedi-0.9.0/docs/docs/plugin-api.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     2061 2014-07-22 23:03:50.000000 jedi-0.9.0/docs/docs/usage.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     2618 2015-04-28 17:03:23.000000 jedi-0.9.0/docs/docs/installation.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     7232 2015-04-28 17:03:23.000000 jedi-0.9.0/docs/docs/features.rst
+-rw-rw-r--   0 david     (1000) david     (1000)      865 2014-05-04 22:34:52.000000 jedi-0.9.0/docs/docs/testing.rst
+-rw-rw-r--   0 david     (1000) david     (1000)      159 2014-05-04 22:34:52.000000 jedi-0.9.0/docs/docs/plugin-api-classes.rst
+-rw-rw-r--   0 david     (1000) david     (1000)       77 2014-05-04 22:34:52.000000 jedi-0.9.0/docs/docs/settings.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     5661 2014-05-04 22:34:52.000000 jedi-0.9.0/docs/docs/development.rst
+-rw-rw-r--   0 david     (1000) david     (1000)      781 2015-04-28 17:03:23.000000 jedi-0.9.0/docs/index.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     5556 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/Makefile
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/docs/_themes/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/docs/_themes/flask/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/docs/_themes/flask/static/
+-rw-rw-r--   0 david     (1000) david     (1000)     6411 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/_themes/flask/static/flasky.css_t
+-rw-rw-r--   0 david     (1000) david     (1000)      976 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/_themes/flask/static/small_flask.css
+-rw-rw-r--   0 david     (1000) david     (1000)      971 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/_themes/flask/layout.html
+-rw-rw-r--   0 david     (1000) david     (1000)     1789 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/_themes/flask/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)      162 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/_themes/flask/theme.conf
+-rw-rw-r--   0 david     (1000) david     (1000)      590 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/_themes/flask/relations.html
+-rw-rw-r--   0 david     (1000) david     (1000)     6672 2013-05-11 06:23:14.000000 jedi-0.9.0/docs/_themes/flask_theme_support.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/refactor/
+-rw-rw-r--   0 david     (1000) david     (1000)      697 2013-05-11 06:23:15.000000 jedi-0.9.0/test/refactor/extract.py
+-rw-rw-r--   0 david     (1000) david     (1000)      287 2013-05-11 06:23:15.000000 jedi-0.9.0/test/refactor/rename.py
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2013-05-11 06:23:15.000000 jedi-0.9.0/test/refactor/inline.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_api/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_api/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10309 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_api/test_classes.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2147 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_api/test_unicode.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2032 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_api/test_api_classes_follow_definition.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9832 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_api/test_call_signatures.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4042 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_api/test_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3378 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_api/test_interpreter.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2537 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_api/test_full_name.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2448 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_api/test_defined_names.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_parser/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_parser/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2429 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_parser/test_get_code.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9100 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_parser/test_fast_parser.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6633 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_parser/test_parser.py
+-rw-rw-r--   0 david     (1000) david     (1000)      147 2014-07-22 23:03:50.000000 jedi-0.9.0/test/test_parser/test_user_context.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5167 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_parser/test_tokenize.py
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2013-05-11 06:23:15.000000 jedi-0.9.0/test/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      411 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_new_parser.py
+-rw-rw-r--   0 david     (1000) david     (1000)      762 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_integration_keyword.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3553 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_utils.py
+-rwxrwxr-x   0 david     (1000) david     (1000)    13069 2015-04-28 17:03:23.000000 jedi-0.9.0/test/run.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/speed/
+-rw-rw-r--   0 david     (1000) david     (1000)      647 2014-05-04 22:34:52.000000 jedi-0.9.0/test/speed/precedence.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3178 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_cache.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/static_analysis/
+-rw-rw-r--   0 david     (1000) david     (1000)     2237 2015-04-28 17:03:23.000000 jedi-0.9.0/test/static_analysis/star_arguments.py
+-rw-rw-r--   0 david     (1000) david     (1000)      134 2014-07-22 23:03:50.000000 jedi-0.9.0/test/static_analysis/operations.py
+-rw-rw-r--   0 david     (1000) david     (1000)      245 2014-07-22 23:03:50.000000 jedi-0.9.0/test/static_analysis/descriptors.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1150 2015-04-28 17:03:23.000000 jedi-0.9.0/test/static_analysis/arguments.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/static_analysis/import_tree/
+-rw-rw-r--   0 david     (1000) david     (1000)       16 2014-07-22 23:03:50.000000 jedi-0.9.0/test/static_analysis/import_tree/a.py
+-rw-rw-r--   0 david     (1000) david     (1000)       98 2014-07-22 23:03:50.000000 jedi-0.9.0/test/static_analysis/import_tree/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2014-07-22 23:03:50.000000 jedi-0.9.0/test/static_analysis/import_tree/b.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1432 2014-07-22 23:03:50.000000 jedi-0.9.0/test/static_analysis/try_except.py
+-rw-rw-r--   0 david     (1000) david     (1000)      738 2014-07-22 23:03:50.000000 jedi-0.9.0/test/static_analysis/attribute_warnings.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2269 2015-04-28 17:03:23.000000 jedi-0.9.0/test/static_analysis/attribute_error.py
+-rw-rw-r--   0 david     (1000) david     (1000)       94 2015-04-28 17:03:23.000000 jedi-0.9.0/test/static_analysis/generators.py
+-rw-rw-r--   0 david     (1000) david     (1000)      378 2015-04-28 17:03:23.000000 jedi-0.9.0/test/static_analysis/imports.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1519 2014-07-22 23:03:50.000000 jedi-0.9.0/test/test_integration.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/completion/
+-rw-rw-r--   0 david     (1000) david     (1000)     3399 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/descriptors.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6298 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/functions.py
+-rw-rw-r--   0 david     (1000) david     (1000)       77 2013-05-11 06:23:15.000000 jedi-0.9.0/test/completion/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      197 2014-05-04 22:34:52.000000 jedi-0.9.0/test/completion/complex.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2079 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/ordering.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2851 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/goto.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1191 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/types.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3436 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/basic.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7277 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/classes.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1842 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/precedence.py
+-rw-rw-r--   0 david     (1000) david     (1000)       55 2013-05-11 06:23:15.000000 jedi-0.9.0/test/completion/keywords.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/completion/import_tree/
+-rw-rw-r--   0 david     (1000) david     (1000)       62 2013-05-11 06:23:15.000000 jedi-0.9.0/test/completion/import_tree/random.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/completion/import_tree/pkg/
+-rw-rw-r--   0 david     (1000) david     (1000)       29 2013-05-11 06:23:15.000000 jedi-0.9.0/test/completion/import_tree/pkg/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2013-05-11 06:23:15.000000 jedi-0.9.0/test/completion/import_tree/pkg/mod1.py
+-rw-rw-r--   0 david     (1000) david     (1000)       80 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/import_tree/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)       59 2013-08-18 16:18:23.000000 jedi-0.9.0/test/completion/import_tree/recurse_class2.py
+-rw-rw-r--   0 david     (1000) david     (1000)       41 2013-05-11 06:23:15.000000 jedi-0.9.0/test/completion/import_tree/rename1.py
+-rw-rw-r--   0 david     (1000) david     (1000)      193 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/import_tree/invisible_pkg.py
+-rw-rw-r--   0 david     (1000) david     (1000)       61 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/import_tree/mod1.py
+-rw-rw-r--   0 david     (1000) david     (1000)       80 2013-08-18 16:18:23.000000 jedi-0.9.0/test/completion/import_tree/recurse_class1.py
+-rw-rw-r--   0 david     (1000) david     (1000)       63 2013-05-11 06:23:15.000000 jedi-0.9.0/test/completion/import_tree/rename2.py
+-rw-rw-r--   0 david     (1000) david     (1000)       27 2013-08-18 16:18:23.000000 jedi-0.9.0/test/completion/import_tree/mod2.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1752 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/lambdas.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4993 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/decorators.py
+-rw-rw-r--   0 david     (1000) david     (1000)      219 2014-05-04 22:34:52.000000 jedi-0.9.0/test/completion/named_param.py
+-rw-rw-r--   0 david     (1000) david     (1000)      627 2014-07-22 23:03:50.000000 jedi-0.9.0/test/completion/parser.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2934 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/flow_analysis.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2634 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/docstring.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1754 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/on_import.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5057 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/usages.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1844 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/comprehensions.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/completion/thirdparty/
+-rw-rw-r--   0 david     (1000) david     (1000)      212 2013-05-11 06:23:15.000000 jedi-0.9.0/test/completion/thirdparty/django_.py
+-rw-rw-r--   0 david     (1000) david     (1000)      320 2013-05-11 06:23:15.000000 jedi-0.9.0/test/completion/thirdparty/PyQt4_.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1474 2013-08-18 16:18:23.000000 jedi-0.9.0/test/completion/thirdparty/jedi_.py
+-rw-rw-r--   0 david     (1000) david     (1000)      134 2013-05-11 06:23:15.000000 jedi-0.9.0/test/completion/thirdparty/psycopg2_.py
+-rw-rw-r--   0 david     (1000) david     (1000)      544 2013-05-11 06:23:15.000000 jedi-0.9.0/test/completion/thirdparty/pylab_.py
+-rw-rw-r--   0 david     (1000) david     (1000)      975 2013-08-18 16:18:23.000000 jedi-0.9.0/test/completion/definition.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1229 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/isinstance.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2653 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/invalid.py
+-rw-rw-r--   0 david     (1000) david     (1000)      431 2014-05-04 22:34:52.000000 jedi-0.9.0/test/completion/sys_path.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4208 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/dynamic_arrays.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2196 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/generators.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4401 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/arrays.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1926 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/dynamic_params.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4703 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/imports.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2393 2015-04-28 17:03:23.000000 jedi-0.9.0/test/completion/stdlib.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1866 2013-08-18 16:18:23.000000 jedi-0.9.0/test/test_jedi_system.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1346 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_integration_stdlib.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3071 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_integration_import.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1870 2014-07-22 23:03:50.000000 jedi-0.9.0/test/test_speed.py
+-rw-rw-r--   0 david     (1000) david     (1000)      209 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_debug.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5379 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_regression.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     3478 2014-05-04 22:34:52.000000 jedi-0.9.0/test/refactor.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/
+-rw-rw-r--   0 david     (1000) david     (1000)     1684 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/test_pyc.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2316 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/test_namespace_package.py
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2751 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/test_buildout_detection.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/init_extension_module/
+-rwxrwxr-x   0 david     (1000) david     (1000)    16493 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/init_extension_module/__init__.cpython-34m.so
+-rw-rw-r--   0 david     (1000) david     (1000)      250 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/init_extension_module/setup.py
+-rw-rw-r--   0 david     (1000) david     (1000)      294 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/init_extension_module/module.c
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/namespace_package/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns1/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns1/pkg/
+-rw-rw-r--   0 david     (1000) david     (1000)      214 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns1/pkg/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns1/pkg/ns1_folder/
+-rw-rw-r--   0 david     (1000) david     (1000)       20 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns1/pkg/ns1_folder/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)       18 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns1/pkg/ns1_file.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns2/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns2/pkg/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns2/pkg/ns2_folder/
+-rw-rw-r--   0 david     (1000) david     (1000)       20 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns2/pkg/ns2_folder/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns2/pkg/ns2_folder/nested/
+-rw-rw-r--   0 david     (1000) david     (1000)       16 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns2/pkg/ns2_folder/nested/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)       18 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/namespace_package/ns2/pkg/ns2_file.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1803 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/test_compiled.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/absolute_import/
+-rw-rw-r--   0 david     (1000) david     (1000)      437 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/absolute_import/unittest.py
+-rw-rw-r--   0 david     (1000) david     (1000)      383 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/absolute_import/local_module.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4392 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/test_docstring.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/buildout_project/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/buildout_project/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/buildout_project/src/proj_name/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2014-07-22 23:03:50.000000 jedi-0.9.0/test/test_evaluate/buildout_project/src/proj_name/module_name.py
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2014-07-22 23:03:50.000000 jedi-0.9.0/test/test_evaluate/buildout_project/buildout.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/buildout_project/bin/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2014-07-22 23:03:50.000000 jedi-0.9.0/test/test_evaluate/buildout_project/bin/empty_file
+-rw-rw-r--   0 david     (1000) david     (1000)      227 2014-07-22 23:03:50.000000 jedi-0.9.0/test/test_evaluate/buildout_project/bin/app
+-rw-rw-r--   0 david     (1000) david     (1000)     1680 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/test_extension.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1269 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/test_absolute_import.py
+-rw-rw-r--   0 david     (1000) david     (1000)      964 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/test_representation.py
+-rw-rw-r--   0 david     (1000) david     (1000)      628 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/test_annotations.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/not_in_sys_path/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/not_in_sys_path/not_in_sys_path_package/
+-rw-rw-r--   0 david     (1000) david     (1000)       18 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/not_in_sys_path/not_in_sys_path_package/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)       25 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/not_in_sys_path/not_in_sys_path_package/module.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/not_in_sys_path/pkg/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/not_in_sys_path/pkg/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      221 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/not_in_sys_path/pkg/module.py
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/not_in_sys_path/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)       10 2014-05-04 22:34:52.000000 jedi-0.9.0/test/test_evaluate/not_in_sys_path/not_in_sys_path.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/flask_foo.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/flask_baz/
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/flask_baz/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/flaskext/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/flaskext/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/flaskext/moo/
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/flaskext/moo/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/flaskext/bar.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/flask/
+-rw-rw-r--   0 david     (1000) david     (1000)       21 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/flask/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/flask/ext/
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/flask-site-packages/flask/ext/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2007 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/test_imports.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/egg-link/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/egg-link/venv/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/egg-link/venv/lib/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/egg-link/venv/lib/python3.4/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/test/test_evaluate/egg-link/venv/lib/python3.4/site-packages/
+-rw-rw-r--   0 david     (1000) david     (1000)       20 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/egg-link/venv/lib/python3.4/site-packages/egg_link.egg-link
+-rw-rw-r--   0 david     (1000) david     (1000)     1106 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_evaluate/test_sys_path.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1029 2013-08-18 16:18:23.000000 jedi-0.9.0/test/helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5125 2014-07-22 23:03:50.000000 jedi-0.9.0/test/conftest.py
+-rw-rw-r--   0 david     (1000) david     (1000)      346 2015-04-28 17:03:23.000000 jedi-0.9.0/test/test_integration_analysis.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/jedi/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/jedi/evaluate/
+-rw-rw-r--   0 david     (1000) david     (1000)     5084 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/recursion.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16430 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6101 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/precedence.py
+-rw-rw-r--   0 david     (1000) david     (1000)    31708 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/representation.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10812 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/analysis.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2891 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/flow_analysis.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/jedi/evaluate/compiled/
+-rw-rw-r--   0 david     (1000) david     (1000)    16590 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/compiled/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/jedi/evaluate/compiled/fake/
+-rw-rw-r--   0 david     (1000) david     (1000)       77 2014-05-04 22:34:52.000000 jedi-0.9.0/jedi/evaluate/compiled/fake/datetime.pym
+-rw-rw-r--   0 david     (1000) david     (1000)     5013 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/compiled/fake/builtins.pym
+-rw-rw-r--   0 david     (1000) david     (1000)      201 2014-05-04 22:34:52.000000 jedi-0.9.0/jedi/evaluate/compiled/fake/_weakref.pym
+-rw-rw-r--   0 david     (1000) david     (1000)     3019 2014-07-22 23:03:50.000000 jedi-0.9.0/jedi/evaluate/compiled/fake/_sre.pym
+-rw-rw-r--   0 david     (1000) david     (1000)      489 2014-05-04 22:34:52.000000 jedi-0.9.0/jedi/evaluate/compiled/fake/_sqlite3.pym
+-rw-rw-r--   0 david     (1000) david     (1000)      325 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/compiled/fake/_functools.pym
+-rw-rw-r--   0 david     (1000) david     (1000)       58 2014-05-04 22:34:52.000000 jedi-0.9.0/jedi/evaluate/compiled/fake/posix.pym
+-rw-rw-r--   0 david     (1000) david     (1000)      113 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/compiled/fake/io.pym
+-rw-rw-r--   0 david     (1000) david     (1000)     4068 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/compiled/fake.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5517 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6754 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/docstrings.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8662 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/sys_path.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21281 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/finder.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16911 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/param.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4936 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/dynamic.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19845 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/imports.py
+-rw-rw-r--   0 david     (1000) david     (1000)    22526 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/iterable.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8241 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/stdlib.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2039 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/evaluate/cache.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1640 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1322 2014-07-22 23:03:50.000000 jedi-0.9.0/jedi/__main__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/jedi/parser/
+-rw-rw-r--   0 david     (1000) david     (1000)    16804 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/parser/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/jedi/parser/pgen2/
+-rw-rw-r--   0 david     (1000) david     (1000)    13966 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/parser/pgen2/pgen.py
+-rw-rw-r--   0 david     (1000) david     (1000)      337 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/parser/pgen2/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8124 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/parser/pgen2/parse.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4691 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/parser/pgen2/grammar.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21590 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/parser/fast.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6668 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/parser/grammar2.7.txt
+-rw-rw-r--   0 david     (1000) david     (1000)    35759 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/parser/tree.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1188 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/parser/token.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12849 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/parser/user_context.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10888 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/parser/tokenize.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6236 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/parser/grammar3.4.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     4061 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7033 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/refactoring.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5661 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/_compatibility.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4935 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/common.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6134 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/settings.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2527 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/debug.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/jedi/api/
+-rw-rw-r--   0 david     (1000) david     (1000)    28950 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/api/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    23964 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/api/classes.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2047 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/api/keywords.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1791 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/api/usages.py
+-rw-rw-r--   0 david     (1000) david     (1000)      832 2014-07-22 23:03:50.000000 jedi-0.9.0/jedi/api/replstartup.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2567 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/api/helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3714 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/api/interpreter.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10055 2015-04-28 17:03:23.000000 jedi-0.9.0/jedi/cache.py
+-rw-rw-r--   0 david     (1000) david     (1000)       59 2015-04-28 17:03:47.000000 jedi-0.9.0/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)      421 2013-05-11 06:23:14.000000 jedi-0.9.0/.coveragerc
+-rw-rw-r--   0 david     (1000) david     (1000)     1521 2014-05-04 22:34:52.000000 jedi-0.9.0/conftest.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     1859 2015-04-28 17:03:23.000000 jedi-0.9.0/setup.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6486 2015-04-28 17:03:23.000000 jedi-0.9.0/README.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     1629 2015-04-28 17:03:23.000000 jedi-0.9.0/CHANGELOG.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     1111 2013-08-18 16:18:22.000000 jedi-0.9.0/LICENSE.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2015-04-28 17:03:47.000000 jedi-0.9.0/jedi.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)    11151 2015-04-28 17:03:45.000000 jedi-0.9.0/jedi.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2015-04-28 17:03:45.000000 jedi-0.9.0/jedi.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        5 2015-04-28 17:03:45.000000 jedi-0.9.0/jedi.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     7446 2015-04-28 17:03:47.000000 jedi-0.9.0/jedi.egg-info/SOURCES.txt
```

### Comparing `jedi-0.8.1-final0/sith.py` & `jedi-0.9.0/sith.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/AUTHORS.txt` & `jedi-0.9.0/AUTHORS.txt`

 * *Files 20% similar despite different names*

```diff
@@ -22,9 +22,16 @@
 srusskih (@srusskih)
 Steven Silvester (@blink1073)
 Colin Duquesnoy (@ColinDuquesnoy) <colin.duquesnoy@gmail.com>
 Jorgen Schaefer (@jorgenschaefer) <contact@jorgenschaefer.de>
 Fredrik Bergroth (@fbergroth)
 Mathias Fußenegger (@mfussenegger)
 Syohei Yoshida (@syohex) <syohex@gmail.com>
+ppalucky (@ppalucky)
+immerrr (@immerrr) immerrr@gmail.com
+Albertas Agejevas (@alga)
+Savor d'Isavano (@KenetJervet) <newelevenken@163.com>
+Phillip Berndt (@phillipberndt) <phillip.berndt@gmail.com>
+Ian Lee (@IanLee1521) <IanLee1521@gmail.com>
+Farkhad Khatamov (@hatamov) <comsgn@gmail.com>
 
 Note: (@user) means a github user name.
```

### Comparing `jedi-0.8.1-final0/PKG-INFO` & `jedi-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,132 +1,166 @@
 Metadata-Version: 1.1
 Name: jedi
-Version: 0.8.1-final0
+Version: 0.9.0
 Summary: An autocompletion tool for Python that can be used for text editors.
 Home-page: https://github.com/davidhalter/jedi
 Author: David Halter
 Author-email: davidhalter88@gmail.com
 License: MIT
-Description: ###################################################
-        Jedi - an awesome autocompletion library for Python
-        ###################################################
+Description: ###################################################################
+        Jedi - an awesome autocompletion/static analysis library for Python
+        ###################################################################
         
         .. image:: https://secure.travis-ci.org/davidhalter/jedi.png?branch=master
             :target: http://travis-ci.org/davidhalter/jedi
             :alt: Travis-CI build status
         
         .. image:: https://coveralls.io/repos/davidhalter/jedi/badge.png?branch=master
             :target: https://coveralls.io/r/davidhalter/jedi
             :alt: Coverage Status
         
-        .. image:: https://pypip.in/d/jedi/badge.png
-            :target: https://crate.io/packages/jedi/
-            :alt: Number of PyPI downloads
-        
-        .. image:: https://pypip.in/v/jedi/badge.png
-            :target: https://crate.io/packages/jedi/
-            :alt: Latest PyPI version
-        
-        Jedi is an autocompletion tool for Python that can be used in IDEs/editors.
-        Jedi works. Jedi is fast. It understands all of the basic Python syntax
-        elements including many builtin functions.
         
-        Additionaly, Jedi suports two different goto functions and has support for
-        renaming as well as Pydoc support and some other IDE features.
+        *If you have specific questions, please add an issue or ask on* `stackoverflow
+        <https://stackoverflow.com>`_ *with the label* ``python-jedi``.
+        
+        
+        Jedi is a static analysis tool for Python that can be used in IDEs/editors. Its
+        historic focus is autocompletion, but does static analysis for now as well.
+        Jedi is fast and is very well tested. It understands Python on a deeper level
+        than all other static analysis frameworks for Python.
+        
+        Jedi has support for two different goto functions. It's possible to search for
+        related names and to list all names in a Python file and infer them. Jedi
+        understands docstrings and you can use Jedi autocompletion in your REPL as
+        well.
         
         Jedi uses a very simple API to connect with IDE's. There's a reference
         implementation as a `VIM-Plugin <https://github.com/davidhalter/jedi-vim>`_,
-        which uses Jedi's autocompletion.  I encourage you to use Jedi in your IDEs.
-        It's really easy. If there are any problems (also with licensing), just contact
-        me.
+        which uses Jedi's autocompletion.  We encourage you to use Jedi in your IDEs.
+        It's really easy.
         
-        Jedi can be used with the following editors:
+        Jedi can currently be used with the following editors:
         
         - Vim (jedi-vim_, YouCompleteMe_)
-        - Emacs (Jedi.el_, elpy_, anaconda-mode_)
+        - Emacs (Jedi.el_, elpy_, anaconda-mode_, ycmd_)
         - Sublime Text (SublimeJEDI_ [ST2 + ST3], anaconda_ [only ST3])
         - SynWrite_
         - TextMate_ (Not sure if it's actually working)
         - Kate_ version 4.13+ supports it natively, you have to enable it, though. [`proof
           <https://projects.kde.org/projects/kde/applications/kate/repository/show?rev=KDE%2F4.13>`_]
         
         And it powers the following projects:
         
         - wdb_ - Web Debugger
         
         
-        Here are some pictures:
+        Here are some pictures taken from jedi-vim_:
         
         .. image:: https://github.com/davidhalter/jedi/raw/master/docs/_screenshots/screenshot_complete.png
         
         Completion for almost anything (Ctrl+Space).
         
         .. image:: https://github.com/davidhalter/jedi/raw/master/docs/_screenshots/screenshot_function.png
         
         Display of function/class bodies, docstrings.
         
         .. image:: https://github.com/davidhalter/jedi/raw/master/docs/_screenshots/screenshot_pydoc.png
         
-        Pydoc support (with highlighting, Shift+k).
+        Pydoc support (Shift+k).
         
         There is also support for goto and renaming.
         
         Get the latest version from `github <https://github.com/davidhalter/jedi>`_
         (master branch should always be kind of stable/working).
         
-        Docs are available at `https://jedi.jedidjah.ch/
-        <https://jedi.jedidjah.ch/>`_. Pull requests with documentation
+        Docs are available at `https://jedi.readthedocs.org/en/latest/
+        <https://jedi.readthedocs.org/en/latest/>`_. Pull requests with documentation
         enhancements and/or fixes are awesome and most welcome. Jedi uses `semantic
         versioning <http://semver.org/>`_.
         
         
         Installation
         ============
         
             pip install jedi
         
         Note: This just installs the Jedi library, not the editor plugins. For
         information about how to make it work with your editor, refer to the
         corresponding documentation.
         
         You don't want to use ``pip``? Please refer to the `manual
-        <https://jedi.jedidjah.ch/en/latest/docs/installation.html>`_.
+        <https://jedi.readthedocs.org/en/latest/docs/installation.html>`_.
         
         
         Feature Support and Caveats
         ===========================
         
         Jedi really understands your Python code. For a comprehensive list what Jedi
-        can do, see: `Features
-        <https://jedi.jedidjah.ch/en/latest/docs/features.html>`_. A list of
+        understands, see: `Features
+        <https://jedi.readthedocs.org/en/latest/docs/features.html>`_. A list of
         caveats can be found on the same page.
         
-        You can run Jedi on cPython 2.6, 2.7, 3.2 or 3.3, but it should also
+        You can run Jedi on cPython 2.6, 2.7, 3.2, 3.3 or 3.4, but it should also
         understand/parse code older than those versions.
         
         Tips on how to use Jedi efficiently can be found `here
-        <https://jedi.jedidjah.ch/en/latest/docs/recipes.html>`_.
+        <https://jedi.readthedocs.org/en/latest/docs/recipes.html>`_.
         
+        API
+        ---
         
-        API for IDEs
-        ============
+        You can find the documentation for the `API here <https://jedi.readthedocs.org/en/latest/docs/plugin-api.html>`_.
+        
+        
+        Autocompletion / Goto / Pydoc
+        -----------------------------
+        
+        Please check the API for a good explanation. There are the following commands:
+        
+        - ``jedi.Script.goto_assignments``
+        - ``jedi.Script.completions``
+        - ``jedi.Script.usages``
+        
+        The returned objects are very powerful and really all you might need.
+        
+        
+        Autocompletion in your REPL (IPython, etc.)
+        -------------------------------------------
         
-        It's very easy to create an editor plugin that uses Jedi. See `Plugin API
-        <https://jedi.jedidjah.ch/en/latest/docs/plugin-api.html>`_ for more
-        information.
+        It's possible to have Jedi autocompletion in REPL modes - `example video <https://vimeo.com/122332037>`_.
+        This means that IPython and others are `supported
+        <https://jedi.readthedocs.org/en/latest/docs/usage.html#tab-completion-in-the-python-shell>`_.
         
-        If you have specific questions, please add an issue or ask on `stackoverflow
-        <https://stackoverflow.com>`_ with the label ``python-jedi``.
+        
+        Static Analysis / Linter
+        ------------------------
+        
+        To do all forms of static analysis, please try to use ``jedi.names``. It will
+        return a list of names that you can use to infer types and so on.
+        
+        Linting is another thing that is going to be part of Jedi. For now you can try
+        an alpha version ``python -m jedi linter``. The API might change though and
+        it's still buggy. It's Jedi's goal to be smarter than classic linter and
+        understand ``AttributeError`` and other code issues.
+        
+        
+        Refactoring
+        -----------
+        
+        Jedi would in theory support refactoring, but we have never publicized it,
+        because it's not production ready. If you're interested in helping out here,
+        let me know. With the latest parser changes, it should be very easy to actually
+        make it work.
         
         
         Development
         ===========
         
         There's a pretty good and extensive `development documentation
-        <https://jedi.jedidjah.ch/en/latest/docs/development.html>`_.
+        <https://jedi.readthedocs.org/en/latest/docs/development.html>`_.
         
         
         Testing
         =======
         
         The test suite depends on ``tox`` and ``pytest``::
         
@@ -141,81 +175,98 @@
         
             tox -e py27
         
         Tests are also run automatically on `Travis CI
         <https://travis-ci.org/davidhalter/jedi/>`_.
         
         For more detailed information visit the `testing documentation
-        <https://jedi.jedidjah.ch/en/latest/docs/testing.html>`_
+        <https://jedi.readthedocs.org/en/latest/docs/testing.html>`_
         
         
         .. _jedi-vim: https://github.com/davidhalter/jedi-vim
         .. _youcompleteme: http://valloric.github.io/YouCompleteMe/
         .. _Jedi.el: https://github.com/tkf/emacs-jedi
         .. _elpy: https://github.com/jorgenschaefer/elpy
         .. _anaconda-mode: https://github.com/proofit404/anaconda-mode
+        .. _ycmd: https://github.com/abingham/emacs-ycmd
         .. _sublimejedi: https://github.com/srusskih/SublimeJEDI
         .. _anaconda: https://github.com/DamnWidget/anaconda
         .. _SynWrite: http://uvviewsoft.com/synjedi/
         .. _wdb: https://github.com/Kozea/wdb
         .. _TextMate: https://github.com/lawrenceakka/python-jedi.tmbundle
         .. _Kate: http://kate-editor.org
         
         
         .. :changelog:
         
         Changelog
         ---------
         
-        0.8.1 (2014-07-15)
+        0.9.0 (2015-04-10)
+        ++++++++++++++++++
+        
+        - Integrated the parser of 2to3. This will make refactoring possible. It will
+          also be possible to check for error messages (like compiling an AST would give)
+          in the future.
+        - With the new parser, the evaluation also completely changed. It's now simpler
+          and more readable.
+        - Completely rewritten REPL completion.
+        - Added ``jedi.names``, a command to do static analysis. Thanks to that
+          sourcegraph guys for sponsoring this!
+        - Alpha version of the linter.
+        
+        
+        0.8.1 (2014-07-23)
         +++++++++++++++++++
         
-        * Bugfix release, the last release forgot to include files that improve
-            autocompletion for builtin libraries. Fixed.
+        - Bugfix release, the last release forgot to include files that improve
+          autocompletion for builtin libraries. Fixed.
         
         0.8.0 (2014-05-05)
         +++++++++++++++++++
         
         - Memory Consumption for compiled modules (e.g. builtins, sys) has been reduced
           drastically. Loading times are down as well (it takes basically as long as an
           import).
         - REPL completion is starting to become usable.
-        - Various small API changes. Generally this released focuses on stability and
+        - Various small API changes. Generally this release focuses on stability and
           refactoring of internal APIs.
-        - Introducing operator precedence, which makes calculating correct Array indices
-          and ``__getattr__`` strings possible.
+        - Introducing operator precedence, which makes calculating correct Array
+          indices and ``__getattr__`` strings possible.
         
         0.7.0 (2013-08-09)
         ++++++++++++++++++
         
-        - Switched from LGPL to MIT license
-        - Added an Interpreter class to the API to make autocompletion in REPL possible.
-        - Added autocompletion support for namespace packages
-        - Add sith.py, a new random testing method
+        - Switched from LGPL to MIT license.
+        - Added an Interpreter class to the API to make autocompletion in REPL
+          possible.
+        - Added autocompletion support for namespace packages.
+        - Add sith.py, a new random testing method.
         
         0.6.0 (2013-05-14)
         ++++++++++++++++++
         
-        - Much faster parser with builtin part caching
-        - A test suite, thanks @tkf
+        - Much faster parser with builtin part caching.
+        - A test suite, thanks @tkf.
         
         0.5 versions (2012)
         +++++++++++++++++++
         
-        - Initial development
+        - Initial development.
         
 Keywords: python completion refactoring vim
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
 Classifier: Topic :: Utilities
```

### Comparing `jedi-0.8.1-final0/docs/_screenshots/screenshot_pydoc.png` & `jedi-0.9.0/docs/_screenshots/screenshot_pydoc.png`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/_screenshots/screenshot_complete.png` & `jedi-0.9.0/docs/_screenshots/screenshot_complete.png`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/_screenshots/screenshot_function.png` & `jedi-0.9.0/docs/_screenshots/screenshot_function.png`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/conf.py` & `jedi-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/_static/logo.png` & `jedi-0.9.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/docs/plugin-api.rst` & `jedi-0.9.0/docs/docs/plugin-api.rst`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/docs/usage.rst` & `jedi-0.9.0/docs/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/docs/installation.rst` & `jedi-0.9.0/docs/docs/installation.rst`

 * *Files 14% similar despite different names*

```diff
@@ -26,26 +26,28 @@
 
 System-wide installation via a package manager
 ----------------------------------------------
 
 Arch Linux
 ~~~~~~~~~~
 
-You can install |jedi| directly from official AUR packages:
+You can install |jedi| directly from official Arch Linux packages:
 
-- `python-jedi <https://aur.archlinux.org/packages/python-jedi/>`__ (Python 3)
-- `python2-jedi <https://aur.archlinux.org/packages/python2-jedi/>`__ (Python 2)
+- `python-jedi <https://www.archlinux.org/packages/community/any/python-jedi/>`__
+  (Python 3)
+- `python2-jedi <https://www.archlinux.org/packages/community/any/python2-jedi/>`__
+  (Python 2)
 
 The specified Python version just refers to the *runtime environment* for
 |jedi|. Use the Python 2 version if you're running vim (or whatever editor you
 use) under Python 2. Otherwise, use the Python 3 version. But whatever version
 you choose, both are able to complete both Python 2 and 3 *code*.
 
-(There is also a packaged version of the vim plugin available: `vim-jedi at AUR
-<https://aur.archlinux.org/packages/vim-jedi/>`__.)
+(There is also a packaged version of the vim plugin available: `vim-jedi at
+Arch Linux<https://www.archlinux.org/packages/community/any/vim-jedi/>`__.)
 
 Debian
 ~~~~~~
 
 Debian packages are available in the `unstable repository
 <http://packages.debian.org/search?keywords=python%20jedi>`__.
```

### Comparing `jedi-0.8.1-final0/docs/docs/features.rst` & `jedi-0.9.0/docs/docs/features.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 .. include:: ../global.rst
 
 Features and Caveats
 ====================
 
-|jedi| supports many of the widely used Python features:
+Jedi obviously supports autocompletion. It's also possible to get it working in
+(:ref:`your REPL (IPython, etc.) <repl-completion>`).
+
+Static analysis is also possible by using the command ``jedi.names``.
+
+The Jedi Linter is currently in an alpha version and can be tested by calling
+``python -m jedi linter``.
+
+Jedi would in theory support refactoring, but we have never publicized it,
+because it's not production ready. If you're interested in helping out here,
+let me know. With the latest parser changes, it should be very easy to actually
+make it work.
 
 
 General Features
 ----------------
 
 - python 2.6+ and 3.2+ support
 - ignores syntax errors and wrong indentation
 - can deal with complex module / function / class structures
 - virtualenv support
-- can infer function arguments from sphinx and epydoc docstrings (:ref:`type
-  hinting <type-hinting>`)
+- can infer function arguments from sphinx, epydoc and basic numpydoc docstrings
+  (:ref:`type hinting <type-hinting>`)
 
 
 Supported Python Features
 -------------------------
 
+|jedi| supports many of the widely used Python features:
+
 - builtins
 - multiple returns or yields
 - tuple assignments / array indexing / dictionary indexing
 - with-statement / exception handling
 - ``*args`` / ``**kwargs``
 - decorators / lambdas / closures
 - generators / iterators
@@ -37,14 +50,15 @@
 - function annotations (py3k feature, are ignored right now, but being parsed.
   I don't know what to do with them.)
 - class decorators (py3k feature, are being ignored too, until I find a use
   case, that doesn't work with |jedi|)
 - simple/usual ``sys.path`` modifications
 - ``isinstance`` checks for if/while/assert
 - namespace packages (includes ``pkgutil`` and ``pkg_resources`` namespaces)
+- Django / Flask / Buildout support
 
 
 Unsupported Features
 --------------------
 
 Not yet implemented:
 
@@ -107,26 +121,27 @@
 .. _type-hinting:
 
 Type Hinting
 ~~~~~~~~~~~~
 
 If |jedi| cannot detect the type of a function argument correctly (due to the
 dynamic nature of Python), you can help it by hinting the type using
-Sphinx-style info field lists or Epydoc docstrings.
+one of the following docstring syntax styles:
 
 **Sphinx style**
 
 http://sphinx-doc.org/domains.html#info-field-lists
 
 ::
 
-    def myfunction(node):
+    def myfunction(node, foo):
         """Do something with a ``node``.
 
         :type node: ProgramNode
+        :param str foo: foo parameter description
 
         """
         node.| # complete here
 
 **Epydoc**
 
 http://epydoc.sourceforge.net/manual-fields.html
@@ -137,14 +152,47 @@
         """Do something with a ``node``.
 
         @type node: ProgramNode
 
         """
         node.| # complete here
 
+**Numpydoc**
+
+https://github.com/numpy/numpy/blob/master/doc/HOWTO_DOCUMENT.rst.txt
+
+In order to support the numpydoc format, you need to install the `numpydoc
+<https://pypi.python.org/pypi/numpydoc>`__ package.
+
+::
+
+    def foo(var1, var2, long_var_name='hi'):
+        r"""A one-line summary that does not use variable names or the
+        function name.
+
+        ...
+
+        Parameters
+        ----------
+        var1 : array_like
+            Array_like means all those objects -- lists, nested lists,
+            etc. -- that can be converted to an array. We can also
+            refer to variables like `var1`.
+        var2 : int
+            The type above can either refer to an actual Python type
+            (e.g. ``int``), or describe the type of the variable in more
+            detail, e.g. ``(N,) ndarray`` or ``array_like``.
+        long_variable_name : {'hi', 'ho'}, optional
+            Choices in brackets, default first when optional.
+
+        ...
+
+        """
+        var2.| # complete here
+
 A little history
 ----------------
 
 The Star Wars Jedi are awesome. My Jedi software tries to imitate a little bit
 of the precognition the Jedi have. There's even an awesome `scene
 <http://www.youtube.com/watch?v=5BDO3pyavOY>`_ of Monty Python Jedis :-).
```

### Comparing `jedi-0.8.1-final0/docs/docs/testing.rst` & `jedi-0.9.0/docs/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/docs/development.rst` & `jedi-0.9.0/docs/docs/development.rst`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/index.rst` & `jedi-0.9.0/docs/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .. include global.rst
 
-Jedi - an awesome autocompletion library for Python
-===================================================
+Jedi - an awesome autocompletion/static analysis library for Python
+===================================================================
 
 Release v\ |release|. (:doc:`Installation <docs/installation>`)
 
 .. automodule:: jedi
 
 Autocompletion can look like this (e.g. VIM plugin):
```

### Comparing `jedi-0.8.1-final0/docs/Makefile` & `jedi-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/_themes/flask/static/flasky.css_t` & `jedi-0.9.0/docs/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/_themes/flask/static/small_flask.css` & `jedi-0.9.0/docs/_themes/flask/static/small_flask.css`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/_themes/flask/layout.html` & `jedi-0.9.0/docs/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/_themes/flask/LICENSE` & `jedi-0.9.0/docs/_themes/flask/LICENSE`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/_themes/flask/relations.html` & `jedi-0.9.0/docs/_themes/flask/relations.html`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/docs/_themes/flask_theme_support.py` & `jedi-0.9.0/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/refactor/extract.py` & `jedi-0.9.0/test/refactor/extract.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/test_api/test_unicode.py` & `jedi-0.9.0/test/test_api/test_unicode.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/test_api/test_api_classes_follow_definition.py` & `jedi-0.9.0/test/test_api/test_api_classes_follow_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     itert = jedi.Script("from itertools import ").completions()
     definitions = [d for d in itert if d.name == 'chain']
     assert len(definitions) == 1
     assert [d.type for d in definitions[0].follow_definition()] == ['class']
 
     # incomplete `from * import` part
     datetime = check_follow_definition_types("from datetime import datetim")
-    assert set(datetime) == set(['class'])  # py33: builtin and pure py version
+    assert set(datetime) == set(['class', 'instance'])  # py33: builtin and pure py version
 
     # os.path check
     ospath = check_follow_definition_types("from os.path import abspat")
     assert ospath == ['function']
 
     # alias
     alias = check_follow_definition_types("import io as abcd; abcd")
@@ -50,13 +50,13 @@
     types = check_follow_definition_types("import pkg.mod1; pkg")
     assert types == ['module']
 
     types = check_follow_definition_types("import pkg.mod1; pkg.mod1")
     assert types == ['module']
 
     types = check_follow_definition_types("import pkg.mod1; pkg.mod1.a")
-    assert types == ['class']
+    assert types == ['instance']
 
 
 def test_follow_definition_land_on_import():
     types = check_follow_definition_types("import datetime; datetim")
     assert types == ['module']
```

### Comparing `jedi-0.8.1-final0/test/test_api/test_call_signatures.py` & `jedi-0.9.0/test/test_api/test_call_signatures.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,22 @@
         else:
             assert signatures[0].name == expected_name
             assert signatures[0].index == expected_index
 
     def _run_simple(self, source, name, index=0, column=None, line=1):
         self._run(source, name, index, line, column)
 
+    def test_valid_call(self):
+        self._run('str()', 'str', column=4)
+
     def test_simple(self):
         run = self._run_simple
+        s7 = "str().upper().center("
+        s8 = "str(int[zip("
+        run(s7, 'center', 0)
 
         # simple
         s1 = "sorted(a, str("
         run(s1, 'sorted', 0, 7)
         run(s1, 'sorted', 1, 9)
         run(s1, 'sorted', 1, 10)
         run(s1, 'sorted', 1, 11)
@@ -164,14 +170,56 @@
 
     def test_additional_brackets(self):
         self._run('str((', 'str', 0)
 
     def test_unterminated_strings(self):
         self._run('str(";', 'str', 0)
 
+    def test_whitespace_before_bracket(self):
+        self._run('str (', 'str', 0)
+        self._run('str (";', 'str', 0)
+        # TODO this is not actually valid Python, the newline token should be
+        # ignored.
+        self._run('str\n(', 'str', 0)
+
+    def test_brackets_in_string_literals(self):
+        self._run('str (" (', 'str', 0)
+        self._run('str (" )', 'str', 0)
+
+    def test_function_definitions_should_break(self):
+        """
+        Function definitions (and other tokens that cannot exist within call
+        signatures) should break and not be able to return a call signature.
+        """
+        assert not Script('str(\ndef x').call_signatures()
+
+    def test_flow_call(self):
+        assert not Script('if (1').call_signatures()
+
+    def test_chained_calls(self):
+        source = dedent('''
+        class B():
+          def test2(self, arg):
+            pass
+
+        class A():
+          def test1(self):
+            return B()
+
+        A().test1().test2(''')
+
+        self._run(source, 'test2', 0)
+
+    def test_return(self):
+        source = dedent('''
+        def foo():
+            return '.'.join()''')
+
+        self._run(source, 'join', 0, column=len("    return '.'.join("))
+
 
 class TestParams(TestCase):
     def params(self, source, line=None, column=None):
         signatures = Script(source, line, column).call_signatures()
         assert len(signatures) == 1
         return signatures[0].params
 
@@ -185,14 +233,26 @@
             # TODO have multiple call signatures for int (like in the docstr)
             #assert p[1].name == 'base'
 
         p = self.params('''open(something,''')
         assert p[0].name in ['file', 'name']
         assert p[1].name == 'mode'
 
+    def test_builtins(self):
+        """
+        The self keyword should be visible even for builtins, if not
+        instantiated.
+        """
+        p = self.params('str.endswith(')
+        assert p[0].name == 'self'
+        assert p[1].name == 'suffix'
+        p = self.params('str().endswith(')
+        assert p[0].name == 'suffix'
+
+
 
 def test_signature_is_definition():
     """
     Through inheritance, a call signature is a sub class of Definition.
     Check if the attributes match.
     """
     s = """class Spam(): pass\nSpam"""
@@ -200,15 +260,15 @@
     definition = Script(s + '(').goto_definitions()[0]
     signature.line == 1
     signature.column == 6
 
     # Now compare all the attributes that a CallSignature must also have.
     for attr_name in dir(definition):
         dont_scan = ['defined_names', 'line_nr', 'start_pos', 'documentation',
-                     'doc', 'parent']
+                     'doc', 'parent', 'goto_assignments']
         if attr_name.startswith('_') or attr_name in dont_scan:
             continue
         attribute = getattr(definition, attr_name)
         signature_attribute = getattr(signature, attr_name)
         if inspect.ismethod(attribute):
             assert attribute() == signature_attribute()
         else:
@@ -270,7 +330,16 @@
     assert get(kwargs_func + 'foo(a=2').index == 0
     assert get(kwargs_func + 'foo(a=2, b=2').index == 0
 
     both = 'def foo(*args, **kwargs): pass\n'
     assert get(both + 'foo(a=2').index == 1
     assert get(both + 'foo(a=2, b=2').index == 1
     assert get(both + 'foo(a, b, c').index == 0
+
+
+def test_bracket_start():
+    def bracket_start(src):
+        signatures = Script(src).call_signatures()
+        assert len(signatures) == 1
+        return signatures[0].bracket_start
+
+    assert bracket_start('str(') == (1, 3)
```

### Comparing `jedi-0.8.1-final0/test/test_api/test_api.py` & `jedi-0.9.0/test/test_api/test_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Test all things related to the ``jedi.api`` module.
 """
 
 from textwrap import dedent
 
 from jedi import api
+from jedi._compatibility import is_py3
 from pytest import raises
 
 
 def test_preload_modules():
     def check_loaded(*modules):
         # +1 for None module (currently used)
         assert len(parser_cache) == len(modules) + 1
@@ -75,15 +76,18 @@
     assert api.Script('1.e3..').completions() == []
     assert api.Script('1.e-13..').completions() == []
 
 
 def test_completion_on_hex_literals():
     assert api.Script('0x1..').completions() == []
     _check_number('0x1.', 'int')  # hexdecimal
-    _check_number('0b3.', 'int')  # binary
+    # Completing binary literals doesn't work if they are not actually binary
+    # (invalid statements).
+    assert api.Script('0b2.').completions() == []
+    _check_number('0b1.', 'int')  # binary
     _check_number('0o7.', 'int')  # octal
 
     _check_number('0x2e.', 'int')
     _check_number('0xE7.', 'int')
     _check_number('0xEa.', 'int')
     # theoretically, but people can just check for syntax errors:
     #assert api.Script('0x.').completions() == []
@@ -94,20 +98,27 @@
     _check_number('1j.', 'complex')
     _check_number('44.j.', 'complex')
     _check_number('4.0j.', 'complex')
     # No dot no completion
     assert api.Script('4j').completions() == []
 
 
-def test_goto_assignments_on_non_statement():
-    with raises(api.NotFoundError):
-        api.Script('for').goto_assignments()
+def test_goto_assignments_on_non_name():
+    assert api.Script('for').goto_assignments() == []
 
-    with raises(api.NotFoundError):
-        api.Script('assert').goto_assignments()
+    assert api.Script('assert').goto_assignments() == []
+    if is_py3:
+        assert api.Script('True').goto_assignments() == []
+    else:
+        # In Python 2.7 True is still a name.
+        assert api.Script('True').goto_assignments()[0].description == 'class bool'
+
+
+def test_goto_definitions_on_non_name():
+    assert api.Script('import x', column=0).goto_definitions() == []
 
 
 def test_goto_definition_not_multiple():
     """
     There should be only one Definition result if it leads back to the same
     origin (e.g. instance method)
     """
@@ -126,9 +137,9 @@
             else:
                 a = A(1)
             a''')
     assert len(api.Script(s).goto_definitions()) == 1
 
 
 def test_usage_description():
-    for u in api.Script('foo = ''; foo').usages():
-        assert u.description == 'foo'
+    descs = [u.description for u in api.Script("foo = ''; foo").usages()]
+    assert set(descs) == set(["foo = ''", 'foo'])
```

### Comparing `jedi-0.8.1-final0/test/test_api/test_interpreter.py` & `jedi-0.9.0/test/test_api/test_interpreter.py`

 * *Files 16% similar despite different names*

```diff
@@ -76,7 +76,17 @@
         class Foo():
             def __getitem__(self, index):
                 # possible side effects here, should therefore not call this.
                 return index
 
         foo = Foo()
         self.check_interpreter_complete('foo[0].', locals(), [])
+
+    def test_property_error(self):
+        class Foo():
+            @property
+            def bar(self):
+                raise ValueError
+
+        foo = Foo()
+        self.check_interpreter_complete('foo.bar', locals(), ['bar'])
+        self.check_interpreter_complete('foo.bar.baz', locals(), [])
```

### Comparing `jedi-0.8.1-final0/test/test_api/test_full_name.py` & `jedi-0.9.0/test/test_api/test_full_name.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,46 +11,48 @@
    ``obj.full_name`` and ``jedi.defined_names``.
 
 #. Misc single-function tests.
 """
 
 import textwrap
 
+import pytest
+
 import jedi
-from jedi.api import classes
-from jedi.evaluate import Evaluator
 from ..helpers import TestCase
 
 
 class MixinTestFullName(object):
     operation = None
 
     def check(self, source, desired):
         script = jedi.Script(textwrap.dedent(source))
         definitions = getattr(script, type(self).operation)()
-        self.assertEqual(definitions[0].full_name, desired)
+        for d in definitions:
+            self.assertEqual(d.full_name, desired)
 
     def test_os_path_join(self):
         self.check('import os; os.path.join', 'os.path.join')
 
     def test_builtin(self):
-        self.check('type', 'type')
-
-    def test_from_import(self):
-        self.check('from os import path', 'os.path')
+        self.check('TypeError', 'TypeError')
 
 
 class TestFullNameWithGotoDefinitions(MixinTestFullName, TestCase):
     operation = 'goto_definitions'
 
+    @pytest.mark.skipif('sys.version_info[0] < 3', reason='Python 2 also yields None.')
     def test_tuple_mapping(self):
         self.check("""
         import re
         any_re = re.compile('.*')
-        any_re""", 're.RegexObject')
+        any_re""", '_sre.compile.SRE_Pattern')
+
+    def test_from_import(self):
+        self.check('from os import path', 'os.path')
 
 
 class TestFullNameWithCompletions(MixinTestFullName, TestCase):
     operation = 'completions'
 
 
 class TestFullDefinedName(TestCase):
@@ -74,14 +76,16 @@
         import os
         from os import path
         from os.path import join
         from os import path as opath
         """, ['os', 'os.path', 'os.path.join', 'os.path'])
 
 
-def test_keyword_full_name_should_be_none():
-    """issue #94"""
-    # Using `from jedi.keywords import Keyword` here does NOT work
-    # in Python 3.  This is due to the import hack jedi using.
-    Keyword = classes.keywords.Keyword
-    d = classes.Definition(Evaluator(), Keyword('(', (0, 0)))
-    assert d.full_name is None
+def test_sub_module():
+    """
+    ``full_name needs to check sys.path to actually find it's real path module
+    path.
+    """
+    defs = jedi.Script('from jedi.api import classes; classes').goto_definitions()
+    assert [d.full_name for d in defs] == ['jedi.api.classes']
+    defs = jedi.Script('import jedi.api; jedi.api').goto_definitions()
+    assert [d.full_name for d in defs] == ['jedi.api']
```

### Comparing `jedi-0.8.1-final0/test/test_api/test_defined_names.py` & `jedi-0.9.0/test/test_api/test_defined_names.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 from jedi import api
 from ..helpers import TestCase
 
 
 class TestDefinedNames(TestCase):
     def assert_definition_names(self, definitions, names):
-        self.assertEqual([d.name for d in definitions], names)
+        assert [d.name for d in definitions] == names
 
     def check_defined_names(self, source, names):
-        definitions = api.defined_names(textwrap.dedent(source))
+        definitions = api.names(textwrap.dedent(source))
         self.assert_definition_names(definitions, names)
         return definitions
 
     def test_get_definitions_flat(self):
         self.check_defined_names("""
         import module
         class Class:
@@ -27,15 +27,15 @@
         data = None
         """, ['module', 'Class', 'func', 'data'])
 
     def test_dotted_assignment(self):
         self.check_defined_names("""
         x = Class()
         x.y.z = None
-        """, ['x'])
+        """, ['x', 'z'])  # TODO is this behavior what we want?
 
     def test_multiple_assignment(self):
         self.check_defined_names("""
         x = y = None
         """, ['x', 'y'])
 
     def test_multiple_imports(self):
```

### Comparing `jedi-0.8.1-final0/test/test_parser/test_get_code.py` & `jedi-0.9.0/test/test_parser/test_get_code.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import difflib
 
 import pytest
 
 from jedi._compatibility import u
-from jedi.parser import Parser
+from jedi.parser import Parser, load_grammar
 
 code_basic_features = u('''
 """A mod docstring"""
 
 def a_function(a_argument, a_default = "default"):
     """A func docstring"""
 
@@ -40,29 +40,27 @@
     pass
 
 
 @pytest.mark.skipif('True', reason='Refactor a few parser things first.')
 def test_basic_parsing():
     """Validate the parsing features"""
 
-    prs = Parser(code_basic_features)
+    prs = Parser(load_grammar(), code_basic_features)
     diff_code_assert(
         code_basic_features,
-        prs.module.get_code2()
+        prs.module.get_code()
     )
 
 
-@pytest.mark.skipif('True', reason='Not yet working.')
 def test_operators():
     src = u('5  * 3')
-    prs = Parser(src)
+    prs = Parser(load_grammar(), src)
     diff_code_assert(src, prs.module.get_code())
 
 
-@pytest.mark.skipif('True', reason='Broke get_code support for yield/return statements.')
 def test_get_code():
     """Use the same code that the parser also generates, to compare"""
     s = u('''"""a docstring"""
 class SomeClass(object, mixin):
     def __init__(self):
         self.xy = 3.0
         """statement docstr"""
@@ -80,8 +78,28 @@
 class WithDocstring:
     """class docstr"""
     pass
 def method_with_docstring():
     """class docstr"""
     pass
 ''')
-    assert Parser(s).module.get_code() == s
+    assert Parser(load_grammar(), s).module.get_code() == s
+
+
+def test_end_newlines():
+    """
+    The Python grammar explicitly needs a newline at the end. Jedi though still
+    wants to be able, to return the exact same code without the additional new
+    line the parser needs.
+    """
+    def test(source, end_pos):
+        module = Parser(load_grammar(), u(source)).module
+        assert module.get_code() == source
+        assert module.end_pos == end_pos
+
+    test('a', (1, 1))
+    test('a\n', (2, 0))
+    test('a\nb', (2, 1))
+    test('a\n#comment\n', (3, 0))
+    test('a\n#comment', (2, 8))
+    test('a#comment', (1, 9))
+    test('def a():\n pass', (2, 5))
```

### Comparing `jedi-0.8.1-final0/test/test_integration_keyword.py` & `jedi-0.9.0/test/test_integration_keyword.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 Test of keywords and ``jedi.keywords``
 """
-import jedi
-from jedi import Script, common
+from jedi._compatibility import is_py3
+from jedi import Script
 
 
 def test_goto_assignments_keyword():
     """
     Bug: goto assignments on ``in`` used to raise AttributeError::
 
       'unicode' object has no attribute 'generate_call_path'
     """
     Script('in').goto_assignments()
 
 
 def test_keyword():
     """ github jedi-vim issue #44 """
     defs = Script("print").goto_definitions()
-    assert [d.doc for d in defs]
+    if is_py3:
+        assert [d.doc for d in defs]
+    else:
+        assert defs == []
+
+    assert Script("import").goto_assignments() == []
 
-    defs = Script("import").goto_assignments()
-    assert len(defs) == 0
     completions = Script("import", 1, 1).completions()
-    assert len(completions) == 0
-    with common.ignored(jedi.NotFoundError):  # TODO shouldn't throw that.
-        defs = Script("assert").goto_definitions()
-        assert len(defs) == 1
+    assert len(completions) > 10 and 'if' in [c.name for c in completions]
+    assert Script("assert").goto_definitions() == []
```

### Comparing `jedi-0.8.1-final0/test/test_utils.py` & `jedi-0.9.0/test/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,22 +47,23 @@
 
     def test_modules(self):
         import sys
         import os
         self.namespace.sys = sys
         self.namespace.os = os
 
-        assert self.completions('os.path.join') == ['os.path.join']
-        assert self.completions('os.path.join().upper') == ['os.path.join().upper']
-
-        c = set(['os.' + d for d in dir(os) if d.startswith('ch')])
-        assert set(self.completions('os.ch')) == set(c)
-
-        del self.namespace.sys
-        del self.namespace.os
+        try:
+            assert self.completions('os.path.join') == ['os.path.join']
+            assert self.completions('os.path.join().upper') == ['os.path.join().upper']
+
+            c = set(['os.' + d for d in dir(os) if d.startswith('ch')])
+            assert set(self.completions('os.ch')) == set(c)
+        finally:
+            del self.namespace.sys
+            del self.namespace.os
 
     def test_calls(self):
         s = 'str(bytes'
         assert self.completions(s) == [s, 'str(BytesWarning']
 
     def test_import(self):
         s = 'from os.path import a'
```

### Comparing `jedi-0.8.1-final0/test/run.py` & `jedi-0.9.0/test/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -166,45 +166,48 @@
         completions = self.script().completions()
         #import cProfile; cProfile.run('script.completions()')
 
         comp_str = set([c.name for c in completions])
         return compare_cb(self, comp_str, set(literal_eval(self.correct)))
 
     def run_goto_definitions(self, compare_cb):
+        def comparison(definition):
+            suffix = '()' if definition.type == 'instance' else ''
+            return definition.desc_with_module + suffix
+
         def definition(correct, correct_start, path):
             def defs(line_nr, indent):
                 s = jedi.Script(self.source, line_nr, indent, path)
                 return set(s.goto_definitions())
 
             should_be = set()
             number = 0
-            for index in re.finditer('(?: +|$)', correct):
-                if correct == ' ':
-                    continue
-                # -1 for the comment, +3 because of the comment start `#? `
-                start = index.start()
+            for index in re.finditer('(?:[^ ]+)', correct):
+                end = index.end()
+                # +3 because of the comment start `#? `
+                end += 3
                 number += 1
                 try:
-                    should_be |= defs(self.line_nr - 1, start + correct_start)
+                    should_be |= defs(self.line_nr - 1, end + correct_start)
                 except Exception:
                     print('could not resolve %s indent %s'
-                          % (self.line_nr - 1, start))
+                          % (self.line_nr - 1, end))
                     raise
             # because the objects have different ids, `repr`, then compare.
-            should_str = set(r.desc_with_module for r in should_be)
-            if len(should_str) < number:
-                raise Exception('Solution @%s not right, '
-                   'too few test results: %s' % (self.line_nr - 1, should_str))
-            return should_str
+            should = set(comparison(r) for r in should_be)
+            if len(should) < number:
+                raise Exception('Solution @%s not right, too few test results: %s'
+                                % (self.line_nr - 1, should))
+            return should
 
         script = self.script()
-        should_str = definition(self.correct, self.start, script.path)
+        should = definition(self.correct, self.start, script.path)
         result = script.goto_definitions()
-        is_str = set(r.desc_with_module for r in result)
-        return compare_cb(self, is_str, should_str)
+        is_str = set(comparison(r) for r in result)
+        return compare_cb(self, is_str, should)
 
     def run_goto_assignments(self, compare_cb):
         result = self.script().goto_assignments()
         comp_str = str(sorted(str(r.description) for r in result))
         return compare_cb(self, comp_str, self.correct)
 
     def run_usages(self, compare_cb):
@@ -232,15 +235,15 @@
 def collect_file_tests(lines, lines_to_execute):
     makecase = lambda t: IntegrationTestCase(t, correct, line_nr, column,
                                              start, line)
     start = None
     correct = None
     test_type = None
     for line_nr, line in enumerate(lines, 1):
-        if correct:
+        if correct is not None:
             r = re.match('^(\d+)\s*(.*)$', correct)
             if r:
                 column = int(r.group(1))
                 correct = r.group(2)
                 start += r.regs[2][0]  # second group, start index
             else:
                 column = len(line) - 1  # -1 for the \n
@@ -251,30 +254,33 @@
             elif correct.startswith('['):
                 yield makecase(TEST_COMPLETIONS)
             else:
                 yield makecase(TEST_DEFINITIONS)
             correct = None
         else:
             try:
-                r = re.search(r'(?:^|(?<=\s))#([?!<])\s*([^\n]+)', line)
+                r = re.search(r'(?:^|(?<=\s))#([?!<])\s*([^\n]*)', line)
                 # test_type is ? for completion and ! for goto_assignments
                 test_type = r.group(1)
                 correct = r.group(2)
+                # Quick hack to make everything work (not quite a bloody unicorn hack though).
+                if correct == '':
+                    correct = ' '
                 start = r.start()
             except AttributeError:
                 correct = None
             else:
                 # skip the test, if this is not specified test
                 if lines_to_execute and line_nr not in lines_to_execute:
                     correct = None
 
 
 def collect_dir_tests(base_dir, test_files, check_thirdparty=False):
     for f_name in os.listdir(base_dir):
-        files_to_execute = [a for a in test_files.items() if a[0] in f_name]
+        files_to_execute = [a for a in test_files.items() if f_name.startswith(a[0])]
         lines_to_execute = reduce(lambda x, y: x + y[1], files_to_execute, [])
         if f_name.endswith(".py") and (not test_files or files_to_execute):
             skip = None
             if check_thirdparty:
                 lib = f_name.replace('_.py', '')
                 try:
                     # there is always an underline at the end.
@@ -383,14 +389,14 @@
                 import pdb
                 pdb.post_mortem()
 
         count += 1
 
     file_change(current, count, fails)
 
-    print('\nSummary: (%s fails of %s tests) in %.3fs' % (tests_fail,
-                                        len(cases), time.time() - t_start))
+    print('\nSummary: (%s fails of %s tests) in %.3fs'
+          % (tests_fail, len(cases), time.time() - t_start))
     for s in summary:
         print(s)
 
     exit_code = 1 if tests_fail else 0
     sys.exit(exit_code)
```

### Comparing `jedi-0.8.1-final0/test/speed/precedence.py` & `jedi-0.9.0/test/speed/precedence.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/test_cache.py` & `jedi-0.9.0/test/test_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,28 +58,32 @@
 
     cache2 = ParserPicklingCls()
     cache2.version = 2
     cached2 = load_stored_item(cache2, path, item)
     assert cached2 is None
 
 
+@pytest.mark.skipif('True', message='Currently the star import cache is not enabled.')
 def test_star_import_cache_duration():
     new = 0.01
     old, jedi.settings.star_import_cache_validity = \
         jedi.settings.star_import_cache_validity, new
 
-    cache._star_import_cache = {}  # first empty...
+    dct = cache._time_caches['star_import_cache_validity']
+    old_dct = dict(dct)
+    dct.clear()  # first empty...
     # path needs to be not-None (otherwise caching effects are not visible)
     jedi.Script('', 1, 0, '').completions()
     time.sleep(2 * new)
     jedi.Script('', 1, 0, '').completions()
 
     # reset values
     jedi.settings.star_import_cache_validity = old
-    assert len(cache._star_import_cache) == 1
+    assert len(dct) == 1
+    dct = old_dct
     cache._star_import_cache = {}
 
 
 def test_cache_call_signatures():
     """
     See github issue #390.
     """
```

### Comparing `jedi-0.8.1-final0/test/static_analysis/star_arguments.py` & `jedi-0.9.0/test/static_analysis/star_arguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return b
 def nested(*args):
     return simple2(1, *args)
 def nested_twice(*args1):
     return nested(*args1)
 
 nested_twice(2, 3)
-#! 12 type-error-too-few-arguments
+#! 13 type-error-too-few-arguments
 nested_twice(2)
 #! 19 type-error-too-many-arguments
 nested_twice(2, 3, 4)
 
 
 # A named argument can be located before *args.
 def star_args_with_named(*args):
@@ -43,71 +43,77 @@
 # -----------------
 
 
 def kwargs_test(**kwargs):
     return simple2(1, **kwargs)
 
 kwargs_test(c=3, b=2)
-#! 11 type-error-too-few-arguments
+#! 12 type-error-too-few-arguments
 kwargs_test(c=3)
-#! 11 type-error-too-few-arguments
+#! 12 type-error-too-few-arguments
 kwargs_test(b=2)
 #! 22 type-error-keyword-argument
 kwargs_test(b=2, c=3, d=4)
-##! 11 type-error-multiple-values
+#! 12 type-error-multiple-values
 kwargs_test(b=2, c=3, a=4)
 
 
 def kwargs_nested(**kwargs):
     return kwargs_test(b=2, **kwargs)
 
 kwargs_nested(c=3)
 #! 13 type-error-too-few-arguments
 kwargs_nested()
 #! 19 type-error-keyword-argument
 kwargs_nested(c=2, d=4)
-##! 13 type-error-multiple-values
+#! 14 type-error-multiple-values
 kwargs_nested(c=2, a=4)
-#! 13 type-error-multiple-values
-kwargs_nested(b=3, c=2)
+# TODO reenable
+##! 14 type-error-multiple-values
+#kwargs_nested(b=3, c=2)
 
 # -----------------
 # mixed *args/**kwargs
 # -----------------
 
 def simple_mixed(a, b, c):
     return b
 
-
 def mixed(*args, **kwargs):
     return simple_mixed(1, *args, **kwargs)
 
 mixed(1, 2)
 mixed(1, c=2)
 mixed(b=2, c=3)
 mixed(c=4, b='')
 
 # need separate functions, otherwise these might swallow the errors
 def mixed2(*args, **kwargs):
     return simple_mixed(1, *args, **kwargs)
 
 
-#! 6 type-error-too-few-arguments
+#! 7 type-error-too-few-arguments
 mixed2(c=2)
-#! 6 type-error-too-few-arguments
+#! 7 type-error-too-few-arguments
 mixed2(3)
 #! 13 type-error-too-many-arguments
 mixed2(3, 4, 5)
-#! 13 type-error-too-many-arguments
-mixed2(3, 4, c=5)
-#! 6 type-error-multiple-values
+# TODO reenable
+##! 13 type-error-too-many-arguments
+#mixed2(3, 4, c=5)
+#! 7 type-error-multiple-values
 mixed2(3, b=5)
 
 # -----------------
 # plain wrong arguments
 # -----------------
 
 #! 12 type-error-star-star
 simple(1, **[])
+#! 12 type-error-star-star
+simple(1, **1)
+class A(): pass
+#! 12 type-error-star-star
+simple(1, **A())
 
 #! 11 type-error-star
 simple(1, *1)
```

### Comparing `jedi-0.8.1-final0/test/static_analysis/arguments.py` & `jedi-0.9.0/test/static_analysis/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 def two_params(x, y):
     return y
 
 
 two_params(y=2, x=1)
 two_params(1, y=2)
 
-#! 10 type-error-multiple-values
+#! 11 type-error-multiple-values
 two_params(1, x=2)
 #! 17 type-error-too-many-arguments
 two_params(1, 2, y=3)
 
 # -----------------
 # default arguments
 # -----------------
```

### Comparing `jedi-0.8.1-final0/test/static_analysis/try_except.py` & `jedi-0.9.0/test/static_analysis/try_except.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/static_analysis/attribute_warnings.py` & `jedi-0.9.0/test/static_analysis/attribute_warnings.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/static_analysis/attribute_error.py` & `jedi-0.9.0/test/static_analysis/attribute_error.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,7 +107,13 @@
 
 # Star imports and the like in modules should not cause attribute errors in
 # this module.
 import import_tree
 
 import_tree.a
 import_tree.b
+
+# This is something that raised an error, because it was using a complex
+# mixture of Jedi fakes and compiled objects.
+import _sre
+#! 15 attribute-error
+_sre.compile().not_existing
```

### Comparing `jedi-0.8.1-final0/test/test_integration.py` & `jedi-0.9.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/completion/descriptors.py` & `jedi-0.9.0/test/completion/descriptors.py`

 * *Files 21% similar despite different names*

```diff
@@ -176,7 +176,44 @@
 #? int()
 E.t(1)
 
 #? str()
 e.u(1)
 #? str()
 E.u(1)
+
+# -----------------
+# Conditions
+# -----------------
+
+from functools import partial
+
+
+class Memoize():
+    def __init__(self, func):
+        self.func = func
+
+    def __get__(self, obj, objtype):
+        if obj is None:
+            return self.func
+
+        return partial(self, obj)
+
+    def __call__(self, *args, **kwargs):
+        # We don't do caching here, but that's what would normally happen.
+        return self.func(*args, **kwargs)
+
+
+class MemoizeTest():
+    def __init__(self, x):
+        self.x = x
+
+    @Memoize
+    def some_func(self):
+        return self.x
+
+
+#? int()
+MemoizeTest(10).some_func()
+# Now also call the same function over the class (see if clause above).
+#? float()
+MemoizeTest.some_func(MemoizeTest(10.0))
```

### Comparing `jedi-0.8.1-final0/test/completion/functions.py` & `jedi-0.9.0/test/completion/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #? ['array']
 arr
 
 
 def inputs(param):
     return param
 
-#? list()
+#? list
 inputs(list)
 
 def variable_middle():
     var = 3
     return var
 
 #? int()
@@ -92,19 +92,21 @@
 #? float()
 recursion("a", 1.0)
 
 def other(a):
     return recursion2(a)
 
 def recursion2(a):
-    if a:
+    if random.choice([0, 1]):
         return other(a)
     else:
-        return recursion2("")
-    return a
+        if random.choice([0, 1]):
+            return recursion2("")
+        else:
+            return a
 
 #? int() str()
 recursion2(1)
 
 # -----------------
 # ordering
 # -----------------
@@ -201,15 +203,15 @@
 exe = args_func(1, "")
 #? int()
 exe[0]
 #? str()
 exe[1]
 
 # illegal args (TypeError)
-#? 
+#?
 args_func(*1)[0]
 # iterator
 #? int()
 args_func(*iter([1]))[0]
 
 # different types
 e = args_func(*[1+"", {}])
@@ -233,15 +235,15 @@
     return arg1, args
 
 exe = args_func(1, "", list)
 #? int()
 exe[0]
 #? tuple()
 exe[1]
-#? list()
+#? list
 exe[1][1]
 
 
 # In a dynamic search, both inputs should be given.
 def simple(a):
     #? int() str()
     return a
@@ -260,14 +262,15 @@
 
 
 class Something():
     @memoize
     def x(self, a, b=1):
         return a
 
+#? int()
 Something().x(1)
 
 
 # -----------------
 # ** kwargs
 # -----------------
 def kwargs_func(**kwargs):
@@ -282,18 +285,23 @@
 #? int()
 exe['a']
 #? float()
 exe['b']
 #? int() float()
 exe['c']
 
+a = 'a'
 exe2 = kwargs_func(**{a:3,
-                      b:4.0})
+                      'b':4.0})
 #? int()
 exe2['a']
+#? float()
+exe2['b']
+#? int() float()
+exe2['c']
 
 # -----------------
 # *args / ** kwargs
 # -----------------
 
 def func_without_call(*args, **kwargs):
     #? tuple()
@@ -302,25 +310,25 @@
     kwargs
 
 def fu(a=1, b="", *args, **kwargs):
     return a, b, args, kwargs
 
 exe = fu(list, 1, "", c=set, d="")
 
-#? list()
+#? list
 exe[0]
 #? int()
 exe[1]
 #? tuple()
 exe[2]
 #? str()
 exe[2][0]
 #? dict()
 exe[3]
-#? set()
+#? set
 exe[3]['c']
 
 # -----------------
 # nested *args
 # -----------------
 def function_args(a, b, c):
     return b
@@ -346,28 +354,28 @@
 # -----------------
 def nested_kw(**kwargs1):
     return function_args(**kwargs1)
 
 def nested_kw2(**kwargs2):
     return nested_kw(**kwargs2)
 
-#? int()
+# invalid command, doesn't need to return anything
+#? 
 nested_kw(b=1, c=1.0, list)
 #? int()
 nested_kw(b=1)
-#? int()
+# invalid command, doesn't need to return anything
+#?  
 nested_kw(d=1.0, b=1, list)
 #? int()
-nested_kw(b=1)
-#? int()
 nested_kw(a=3.0, b=1)
 #? int()
 nested_kw(b=1, a=r"")
 #? []
-nested_kw('')
+nested_kw(1, '')
 #? []
 nested_kw(a='')
 
 #? int()
 nested_kw2(b=1)
 #? int()
 nested_kw2(b=1, c=1.0)
@@ -385,18 +393,20 @@
 # -----------------
 def nested_both(*args, **kwargs):
     return function_args(*args, **kwargs)
 
 def nested_both2(*args, **kwargs):
     return nested_both(*args, **kwargs)
 
-#? int()
+# invalid commands, may return whatever.
+#? list
 nested_both('', b=1, c=1.0, list)
-#? int()
+#? list
 nested_both('', c=1.0, b=1, list)
+
 #? []
 nested_both('')
 
 #? int()
 nested_both2('', b=1, c=1.0)
 #? int()
 nested_both2('', c=1.0, b=1)
@@ -427,29 +437,12 @@
 nested_def2('', b=1, c=1.0)[1]
 #? int()
 nested_def2('', c=1.0, b=1)[1]
 #? []
 nested_def2('')[1]
 
 # -----------------
-# function annotations (should be ignored at the moment)
-# -----------------
-def annot(a:3, *args:3):
-    return a, args[0]
-
-#? str()
-annot('', 1.0)[0]
-#? float()
-annot('', 1.0)[1]
-
-def annot_ret(a:3) -> 3:
-    return a
-
-#? str()
-annot_ret('')
-
-# -----------------
 # magic methods
 # -----------------
 def a(): pass
 #? ['__closure__']
 a.__closure__
```

### Comparing `jedi-0.8.1-final0/test/completion/ordering.py` & `jedi-0.9.0/test/completion/ordering.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,29 +86,45 @@
 
 # should not return a function, because `a` is a function above
 def f(b, a): return a
 #? []
 f(b=3)
 
 # -----------------
+# closure
+# -----------------
+
+def x():
+    a = 0
+
+    def x():
+        return a
+
+    a = 3.0
+    return x()
+
+#? float()
+x()
+
+# -----------------
 # class
 # -----------------
 class A(object):
     a = ""
     a = 3
     #? int()
     a
     a = list()
     def __init__(self):
         self.b = ""
 
     def before(self):
         self.b = 3
-        # TODO should this be so?
-        #? int() str() list()
+        # TODO should this be so? include entries after cursor?
+        #? int() str() list
         self.b
         self.b = list
 
         self.a = 1
         #? str() int()
         self.a
```

### Comparing `jedi-0.8.1-final0/test/completion/goto.py` & `jedi-0.9.0/test/completion/goto.py`

 * *Files 15% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 #! 10 ['x = 3']
 ClassVar.x = ''
 #! 12 ['x = 3']
 ClassVar().x = ''
 
 # Recurring use of the same var name, github #315
 def f(t=None):
-    #! 9 ['t = None']
+    #! 9 ['t=None']
     t = t or 1
 
 # -----------------
 # imports
 # -----------------
 
 #! ['module import_tree']
@@ -177,17 +177,42 @@
 ab1(ClassDef);ab2(ClassDef);ab3(ClassDef)
 
 # -----------------
 # for loops
 # -----------------
 
 for i in range(1):
-    #! ['for i in range(1):    i']
+    #! ['for i in range(1): i']
     i
 
 for key, value in [(1,2)]:
-    #! ['for key,value in [(1, 2)]:    key']
+    #! ['for key, value in [(1,2)]: key']
     key
 
 for i in []:
-    #! ['for i in []:    i']
+    #! ['for i in []: i']
     i
+
+# -----------------
+# decorator
+# -----------------
+def dec(dec_param=3):
+    pass
+
+#! 8 ['dec_param=3']
+@dec(dec_param=5)
+def y():
+    pass
+
+class ClassDec():
+    def class_func(func):
+        return func
+
+#! 14 ['def class_func']
+@ClassDec.class_func
+def x():
+    pass
+
+#! 2 ['class ClassDec']
+@ClassDec.class_func
+def z():
+    pass
```

### Comparing `jedi-0.8.1-final0/test/completion/types.py` & `jedi-0.9.0/test/completion/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,14 +43,25 @@
 arr2 = [1,2,3]
 #? ['append']
 arr2.app
 
 #? int()
 arr.count(1)
 
+x = []
+#?
+x.pop()
+x = [3]
+#? int()
+x.pop()
+x = []
+x.append(1.0)
+#? float()
+x.pop()
+
 # -----------------
 # dicts
 # -----------------
 dic = {}
 
 #? ['copy', 'clear']
 dic.c
```

### Comparing `jedi-0.8.1-final0/test/completion/classes.py` & `jedi-0.9.0/test/completion/classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,14 +188,30 @@
 
 #? ['upper']
 Base.upper
 #? ['upper']
 Base().upper
 
 # -----------------
+# dynamic inheritance
+# -----------------
+
+class Angry(object):
+    def shout(self):
+        return 'THIS IS MALARKEY!'
+
+def classgetter():
+    return Angry
+
+class Dude(classgetter()):
+    def react(self):
+        #? ['shout']
+        self.s
+
+# -----------------
 # __call__
 # -----------------
 
 class CallClass():
     def __call__(self):
         return 1
 
@@ -274,18 +290,18 @@
 # recursions
 # -----------------
 def Recursion():
     def recurse(self):
         self.a = self.a
         self.b = self.b.recurse()
 
-#? 
+#?
 Recursion().a
 
-#? 
+#?
 Recursion().b
 
 # -----------------
 # ducktyping
 # -----------------
 
 def meth(self):
@@ -319,23 +335,23 @@
 
 #? str().upper
 getattr(str(), 'upper')
 #? str.upper
 getattr(str, 'upper')
 
 # some strange getattr calls
-#? 
+#?
 getattr(str, 1)
-#? 
+#?
 getattr()
-#? 
+#?
 getattr(str)
-#? 
+#?
 getattr(getattr, 1)
-#? 
+#?
 getattr(str, [])
 
 
 class Base():
     def ret(self, b):
         return b
 
@@ -368,40 +384,51 @@
 # private vars
 # -----------------
 class PrivateVar():
     def __init__(self):
         self.__var = 1
         #? int()
         self.__var
+        #? ['__var']
+        self.__var
 #? []
 PrivateVar().__var
-#? 
+#?
 PrivateVar().__var
 
 # -----------------
 # super
 # -----------------
 class Super(object):
     a = 3
+    def return_sup(self):
+        return 1
 
 class TestSuper(Super):
-    #? 
+    #?
     super()
     def test(self):
         #? Super()
         super()
         #? ['a']
         super().a
         if 1:
             #? Super()
             super()
         def a():
-            #? 
+            #?
             super()
 
+    def return_sup(self):
+        #? int()
+        return super().return_sup()
+
+#? int()
+TestSuper().return_sup()
+
 
 # -----------------
 # if flow at class level
 # -----------------
 class TestX(object):
     def normal_method(self):
         return 1
@@ -419,13 +446,30 @@
         var
 
 # -----------------
 # mro method
 # -----------------
 
 class A(object):
-    pass
+    a = 3
 
 #? ['mro']
 A.mro
 #? []
 A().mro
+
+
+# -----------------
+# mro resolution
+# -----------------
+
+class B(A()):
+    b = 3
+
+#?
+B.a
+#?
+B().a
+#? int()
+B.b
+#? int()
+B().b
```

### Comparing `jedi-0.8.1-final0/test/completion/precedence.py` & `jedi-0.9.0/test/completion/precedence.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,27 @@
 i += 1
 i -= 3
 i += 1
 #? int()
 x[i]
 
 # -----------------
+# in
+# -----------------
+
+if 'X' in 'Y':
+    a = 3
+else:
+    a = ''
+# For now don't really check for truth values. So in should return both
+# results.
+#? str() int()
+a
+
+# -----------------
 # for flow assignments
 # -----------------
 
 class FooBar(object):
     fuu = 0.1
     raboof = 'fourtytwo'
 
@@ -105,23 +118,13 @@
     b += x
 
 #? str()
 b[1]
 
 
 # -----------------
-# syntax errors
-# -----------------
-
-# strange slice
-z = sorted([1], key = lambda x : x):
-#? int()
-z[0]
-
-
-# -----------------
 # undefined names
 # -----------------
 a = foobarbaz + 'hello'
 
 #? int() float()
 {'hello': 1, 'bar': 1.0}[a]
```

### Comparing `jedi-0.8.1-final0/test/completion/lambdas.py` & `jedi-0.9.0/test/completion/lambdas.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,23 +51,56 @@
 
 # magic method
 a = lambda: 3
 #? ['__closure__']
 a.__closure__
 
 class C():
-    def __init__(self):
+    def __init__(self, foo=1.0):
         self.a = lambda: 1
+        self.foo = foo
+
+    def ret(self):
+        return lambda: self.foo
+
+    def with_param(self):
+        return lambda x: x + self.a()
+
 #? int()
 C().a()
 
+#? str()
+C('foo').ret()()
+
+index = C().with_param()(1)
+#? float()
+['', 1, 1.0][index]
+
+
+def xy(param):
+    def ret(a, b):
+        return a + b
+
+    return lambda b: ret(param, b)
+
+#? int()
+xy(1)(2)
 
 # -----------------
 # lambda param (#379)
 # -----------------
 class Test(object):
     def __init__(self, pred=lambda a, b: a):
         self.a = 1
         #? int()
         self.a
         #? float()
         pred(1.0, 2)
+
+# -----------------
+# test_nocond in grammar (happens in list comprehensions with `if`)
+# -----------------
+# Doesn't need to do anything yet. It should just not raise an error. These
+# nocond lambdas make no sense at all.
+
+#? int()
+[a for a in [1,2] if lambda: 3][0]
```

### Comparing `jedi-0.8.1-final0/test/completion/decorators.py` & `jedi-0.9.0/test/completion/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 @dec
 def fu(a, b, c, *args, **kwargs):
     return a, b, c, args, kwargs
 
 exe = fu(list, c=set, b=3, d='')
 
-#? list()
+#? list
 exe[0]
 #? int()
 exe[1]
 #? set
 exe[2]
 #? []
 exe[3][0]
@@ -59,15 +59,15 @@
 @dec2
 @dec
 def fu2(a, b, c, *args, **kwargs):
     return a, b, c, args, kwargs
 
 exe = fu2(list, c=set, b=3, d='str')
 
-#? list()
+#? list
 exe[0]
 #? int()
 exe[1]
 #? set
 exe[2]
 #? []
 exe[3][0]
@@ -117,15 +117,15 @@
 
 
 class SelfVars():
     """Init decorator problem as an instance, #247"""
     @Decorator
     def __init__(self):
         """
-        init decorators should be ignored when looking up variables in the
+        __init__ decorators should be ignored when looking up variables in the
         class.
         """
         self.c = list
 
     @Decorator
     def shouldnt_expose_var(not_self):
         """
@@ -187,14 +187,26 @@
     return 1
 
 #? 
 f()
 #? int()
 g()
 
+
+class X():
+    @str
+    def x(self):
+        pass
+
+    def y(self):
+        #? str()
+        self.x
+        #?
+        self.x()
+
 # -----------------
 # method decorators
 # -----------------
 
 def dec(f):
     def wrapper(s):
         return f(s)
@@ -253,15 +265,15 @@
         return 1.0
 
 # -----------------
 # others
 # -----------------
 def memoize(function):
         def wrapper(*args):
-            if 1:
+            if random.choice([0, 1]):
                 pass
             else:
                 rv = function(*args)
                 return rv
         return wrapper
 
 @memoize
```

### Comparing `jedi-0.8.1-final0/test/completion/parser.py` & `jedi-0.9.0/test/completion/parser.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/completion/docstring.py` & `jedi-0.9.0/test/completion/docstring.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,114 @@
 """ Test docstrings in functions and classes, which are used to infer types """
 
 # -----------------
 # sphinx style
 # -----------------
-def f(a, b, c, d):
+def sphinxy(a, b, c, d, x):
     """ asdfasdf
     :param a: blablabla
     :type a: str
     :type b: (str, int)
-    :type c: threading.Thread
-    :type d: :class:`threading.Thread`
+    :type c: random.Random
+    :type d: :class:`random.Random`
+    :param str x: blablabla
     :rtype: dict
     """
     #? str()
     a
     #? str()
     b[0]
     #? int()
     b[1]
-    #? ['join']
-    c.join
-    #? ['join']
-    d.join
+    #? ['seed']
+    c.seed
+    #? ['seed']
+    d.seed
+    #? ['lower']
+    x.lower
 
 #? dict()
-f()
+sphinxy()
 
 # wrong declarations
-def f(a, b):
+def sphinxy2(a, b, x):
     """
     :param a: Forgot type declaration
     :type a:
     :param b: Just something
     :type b: ``
-    :rtype: 
+    :param x: Just something without type
+    :rtype:
     """
     #? 
     a
     #? 
     b
+    #?
+    x
 
 #? 
-f()
+sphinxy2()
 
 # local classes -> github #370
 class ProgramNode():
     pass
 
 def local_classes(node, node2):
     """
     :type node: ProgramNode
     ... and the class definition after this func definition:
     :type node2: ProgramNode2
     """
-    #? ProgramNode
+    #? ProgramNode()
     node
-    #? ProgramNode2
+    #? ProgramNode2()
     node2
 
 class ProgramNode2():
     pass
 
 
 def list_with_non_imports(lst):
     """
     Should be able to work with tuples and lists and still import stuff.
 
-    :type lst: (threading.Thread, [collections.defaultdict, ...])
+    :type lst: (random.Random, [collections.defaultdict, ...])
     """
-    #? ['start']
-    lst[0].start
+    #? ['seed']
+    lst[0].seed
 
     import collections as col
     # use some weird index
     #? col.defaultdict()
     lst[1][10]
 
 
+def two_dots(a):
+    """
+    :type a: json.decoder.JSONDecoder
+    """
+    #? ['raw_decode']
+    a.raw_decode
+
+
 # sphinx returns
 def return_module_object():
     """
-    :rtype: :class:`threading.Thread`
+    :rtype: :class:`random.Random`
     """
 
-#? ['join']
-return_module_object().join
+#? ['seed']
+return_module_object().seed
+
 
 # -----------------
 # epydoc style
 # -----------------
-def e(a, b):
+def epydoc(a, b):
     """ asdfasdf
     @type a: str
     @param a: blablabla
     @type b: (str, int)
     @param b: blablah
     @rtype: list
     """
@@ -102,15 +117,15 @@
     #? str()
     b[0]
 
     #? int()
     b[1]
 
 #? list()
-e()
+epydoc()
 
 
 # Returns with param type only
 def rparam(a,b):
     """
     @type a: str
     """
@@ -138,15 +153,15 @@
 # Both docstring and calculated return type
 def both():
     """
     @rtype: str
     """
     return 23
 
-#? str(), int()
+#? str() int()
 both()
 
 class Test(object):
     def __init__(self):
         self.teststr = ""
     """
     # jedi issue #210
```

### Comparing `jedi-0.8.1-final0/test/completion/usages.py` & `jedi-0.9.0/test/completion/usages.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """
 Renaming tests. This means search for usages.
 I always leave a little bit of space to add room for additions, because the
 results always contain position informations.
 """
-#< 4 (0,4), (3,0), (5,0)
+#< 4 (0,4), (3,0), (5,0), (17,0)
 def abc(): pass
 
-#< 0 (-3,4), (0,0), (2,0)
+#< 0 (-3,4), (0,0), (2,0), (14,0)
 abc.d.a.bsaasd.abc.d
 
 abc
 # unicode chars shouldn't be a problem.
 x['smörbröd'].abc
 
+# With the new parser these statements are not recognized as stateents, because
+# they are not valid Python.
 if 1:
     abc = 
 else:
     (abc) = 
-
 abc = 
-
-#< (-3,0), (0,0)
+#< (-17,4), (-14,0), (-12,0), (0,0)
 abc
 
+abc = 5
+
 
 Abc = 3
 
 #< 6 (0,6), (2,4), (5,8), (17,0)
 class Abc():
     #< (-2,6), (0,4), (3,8), (15,0)
     Abc
@@ -43,20 +45,21 @@
     def self_test(self):
         #< 12 (-2,18), (0,8)
         self.b
 
 Abc.d.Abc
 
 
-#< 4 (0,4), (4,1)
-def blub():
+#< 4 (0,4), (5,1)
+def blubi():
+    pass
 
 
-#< (-4,4), (0,1)
-@blub
+#< (-5,4), (0,1)
+@blubi
 def a(): pass
 
 
 #< 0 (0,0), (1,0)
 set_object_var = object()
 set_object_var.var = 1
 
@@ -92,16 +95,15 @@
 
 #< 20 ('rename1', 1,0), ('rename2', 4,5), (-10,24), (-7,0), (-4,17), (0,17), (3,17), ('imports', 70, 16)
 from import_tree.rename1 import abc
 
 #< (0, 32),
 from import_tree.rename1 import not_existing
 
-# shouldn't work
-#< 
+# Shouldn't raise an error or do anything weird.
 from not_existing import *
 
 # -----------------
 # classes
 # -----------------
 
 class TestMethods(object):
@@ -133,14 +135,17 @@
     def a(self):
         #< 13 (4,13), (0,13)
         self._instance_var = 3
 
     def b(self):
         #< (-4,13), (0,13)
         self._instance_var
+        # A call to self used to trigger an error, because it's also a trailer
+        # with two children.
+        self()
 
 
 class NestedClass():
     def __getattr__(self, name):
         return self
 
 # Shouldn't find a definition, because there's other `instance`.
@@ -158,15 +163,15 @@
     #< 4 (0,4),
     class_var = 1
 
     #< 8 (0,8),
     def base_method(self):
         #< 13 (0,13), (20,13)
         self.base_var = 1
-        #< 13 (0,13), (24,13), (29,13)
+        #< 13 (0,13),
         self.instance_var = 1
 
     #< 8 (0,8),
     def just_a_method(self): pass
 
 
 #< 20 (0,16), (-18,6)
@@ -187,15 +192,15 @@
 
 
         #< 13 (5,13), (0,13)
         self.instance_var = 3
 
     #< 9 (0,8), 
     def just_a_method(self):
-        #< (-5,13), (0,13), (-29,13)
+        #< (-5,13), (0,13)
         self.instance_var
 
 
 # -----------------
 # properties
 # -----------------
 class TestProperty:
@@ -257,7 +262,14 @@
 # Compiled Objects
 # -----------------
 
 import _sre
 
 #< 0 (-3,7), (0,0), ('_sre', None, None)
 _sre
+
+# -----------------
+# on syntax
+# -----------------
+
+#< 0
+import undefined
```

### Comparing `jedi-0.8.1-final0/test/completion/thirdparty/jedi_.py` & `jedi-0.9.0/test/completion/thirdparty/jedi_.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/completion/thirdparty/pylab_.py` & `jedi-0.9.0/test/completion/thirdparty/pylab_.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/completion/definition.py` & `jedi-0.9.0/test/completion/definition.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/completion/invalid.py` & `jedi-0.9.0/test/completion/invalid.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,35 +6,42 @@
 there should never be any errors.
 """
 
 # wait until keywords are out of definitions (pydoc function).
 ##? 5 
 's'()
 
-#? ['upper']
+#? []
 str()).upper
 
 # -----------------
 # funcs
 # -----------------
 def asdf(a or b): # multiple param names
     return a
 
-#? int()
+#? 
 asdf(2)
 
+asdf = ''
+
 from a import (b
 def blub():
     return 0
-def openbrace():
+def wrong_indents():
     asdf = 3
      asdf
     asdf(
     #? int()
     asdf
+def openbrace():
+    asdf = 3
+    asdf(
+    #? int()
+    asdf
     return 1
 
 #? int()
 openbrace()
 
 blub([
 #? int()
@@ -54,15 +61,15 @@
 
 #? int()
 normalfunc()
 
 # dots in param
 def f(seq1...=None):
     return seq1
-#? int()
+#?
 f(1)
 
 @
 def test_empty_decorator():
     return 1
 
 #? int()
@@ -92,22 +99,25 @@
 #? ['isinstance']
 if isi
 try:
     except TypeError:
         #? str()
         ""
 
+def break(): pass
 # wrong ternary expression
+a = ''
 a = 1 if
-#? int()
+#? str()
 a
 
+# No completions for for loops without the right syntax
 for for_local in :
     for_local
-#? ['for_local']
+#? []
 for_local
 #? 
 for_local
 
 
 # -----------------
 # list comprehensions
@@ -118,33 +128,33 @@
 a2[0]
 
 a3 = [for xyz in]
 #? 
 a3[0]
 
 a3 = [a4 for in 'b']
-#? str()
+#? 
 a3[0]
 
 a3 = [a4 for a in for x in y]
 #? 
 a3[0]
 
 a = [for a in
 def break(): pass
 
 #? 
 a[0]
 
 a = [a for a in [1,2]
 def break(): pass
-#? int()
+#?
 a[0]
 
-#? ['real']
+#? []
 int()).real
 
 # -----------------
 # keywords
 # -----------------
 
 #! []
@@ -161,18 +171,43 @@
 
 # -----------------
 # statements
 # -----------------
 
 call = ''
 invalid = .call
-#? str()
+#?
 invalid
 
 invalid = call?.call
-#? str()
+#?
 invalid
 
 # comma
 invalid = ,call
-#? str()
+#?
 invalid
+
+
+# -----------------
+# classes
+# -----------------
+
+class BrokenPartsOfClass():
+    def foo(self):
+        # This construct contains two places where Jedi with Python 3 can fail.
+        # It should just ignore those constructs and still execute `bar`.
+        pass
+        if 2:
+            try:
+                pass
+            except ValueError, e:
+                raise TypeError, e
+        else:
+            pass
+
+    def bar(self):
+        self.x = 3
+        return ''
+
+#? str()
+BrokenPartsOfClass().bar()
```

### Comparing `jedi-0.8.1-final0/test/completion/generators.py` & `jedi-0.9.0/test/completion/generators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -----------------
 # yield statement
 # -----------------
 def gen():
-    yield 1
-    yield ""
+    if random.choice([0, 1]):
+        yield 1
+    else:
+        yield ""
 
 gen_exe = gen()
 #? int() str()
 next(gen_exe)
 
 #? int() str() list
 next(gen_exe, list)
@@ -18,37 +20,48 @@
 
 #? int()
 next(gen_ret(1))
 
 #? []
 next(gen_ret())
 
+# generators evaluate to true if cast by bool.
+a = ''
+if gen_ret():
+    a = 3
+#? int()
+a
+
 
 # -----------------
 # generators should not be indexable
 # -----------------
 def get(param):
-    yield 1
-    yield ""
+    if random.choice([0, 1]):
+        yield 1
+    else:
+        yield ""
 
 #? []
 get()[0]
 
 # -----------------
 # __iter__
 # -----------------
 for a in get():
     #? int() str()
     a
 
 
 class Get():
     def __iter__(self):
-        yield 1
-        yield ""
+        if random.choice([0, 1]):
+            yield 1
+        else:
+            yield ""
 
 b = []
 for a in Get():
     #? int() str()
     a
     b += [a]
 
@@ -94,30 +107,32 @@
     print c
 
 
 # -----------------
 # tuples
 # -----------------
 def gen():
-    if a:
+    if random.choice([0,1]):
         yield 1, ""
     else:
         yield 2, 1.0
 
 
 a, b = next(gen())
 #? int()
 a
 #? str() float()
 b
 
 
 def simple():
-    yield 1
-    yield ''
+    if random.choice([0, 1]):
+        yield 1
+    else:
+        yield ""
 
 a, b = simple()
 #? int()
 a
 #? str()
 b
```

### Comparing `jedi-0.8.1-final0/test/completion/dynamic.py` & `jedi-0.9.0/test/completion/dynamic_arrays.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,10 @@
 """
-This is used for dynamic object completion.
-Jedi tries to guess the types with a backtracking approach.
+Checking for ``list.append`` and all the other possible array modifications.
 """
-def func(a):
-    #? int() str()
-    return a
-
-#? int()
-func(1)
-
-func
-
-int(1) + (int(2))+ func('')
-
-# Again the same function, but with another call.
-def func(a):
-    #? float()
-    return a
-
-func(1.0)
-
-# Again the same function, but with no call.
-def func(a):
-    #? 
-    return a
-
-def func(a):
-    #? float()
-    return a
-str(func(1.0))
-
-# -----------------
-# *args, **args
-# -----------------
-def arg(*args):
-    #? tuple()
-    args
-    #? int()
-    args[0]
-
-arg(1,"")
-# -----------------
-# decorators
-# -----------------
-def def_func(f):
-    def wrapper(*args, **kwargs):
-        return f(*args, **kwargs)
-    return wrapper
-
-@def_func
-def func(c):
-    #? str()
-    return c
-
-#? str()
-func("str")
-
-@def_func
-def func(c=1):
-    #? int() float()
-    return c
-
-func(1.0)
-
-# Needs to be here, because in this case func is an import -> shouldn't lead to
-# exceptions.
-import sys as func
-func.sys
-
-# -----------------
-# classes
-# -----------------
-
-class A():
-    def __init__(self, a):
-        #? str()
-        a
-
-A("s")
-
-class A():
-    def __init__(self, a):
-        #? int()
-        a
-        self.a = a
-
-    def test(self, a):
-        #? float()
-        a
-        self.c = self.test2()
-
-    def test2(self):
-        #? int()
-        return self.a
-
-    def test3(self):
-        #? int()
-        self.test2()
-        #? int()
-        self.c
-
-A(3).test(2.0)
-A(3).test2()
-
 # -----------------
 # list.append
 # -----------------
 arr = []
 for a in [1,2]:
     arr.append(a);
 
@@ -314,16 +212,16 @@
         return a
 
 #? float()
 blub()[0]
 
 # with else clause
 def blub():
-    if 1:
-        1
+    if random.choice([0, 1]):
+         1
     else:
         a = []
         a.append(1)
         return a
 
 #? int()
 blub()[0]
@@ -340,30 +238,42 @@
     def blub2(self):
         """ mapper function """
         a = self.blub(1.0)
         #? float()
         a[0]
         return a
 
-    def class_arr(self, el):
+    def literal_arr(self, el):
         self.a = []
         self.a.append(el)
         #? int()
         self.a[0]
         return self.a
 
+    def list_arr(self, el):
+        self.b = list([])
+        self.b.append(el)
+        #? float()
+        self.b[0]
+        return self.b
+
 #? int()
 C().blub(1)[0]
 #? float()
 C().blub2(1)[0]
 
 #? int()
 C().a[0]
 #? int()
-C().class_arr(1)[0]
+C().literal_arr(1)[0]
+
+#? float()
+C().b[0]
+#? float()
+C().list_arr(1.0)[0]
 
 # -----------------
 # array recursions
 # -----------------
 
 a = set([1.0])
 a.update(a)
@@ -390,18 +300,7 @@
     b = []
     b.extend
     extend()
     b.extend(first())
     return list(b)
 #? 
 third()[0]
-
-# -----------------
-# list comprehensions
-# -----------------
-
-def from_comprehension(foo):
-    #? int() float()
-    return foo
-
-[from_comprehension(1.0) for n in (1,)]
-[from_comprehension(n) for n in (1,)]
```

### Comparing `jedi-0.8.1-final0/test/completion/arrays.py` & `jedi-0.9.0/test/completion/arrays.py`

 * *Files 4% similar despite different names*

```diff
@@ -220,15 +220,15 @@
 #? 9 ['str']
 {str: str}
 
 # iteration problem (detected with sith)
 d = dict({'a':''})
 def y(a):
     return a
-#? 
+#?
 y(**d)
 
 # problem with more complicated casts
 dic = {str(key): ''}
 #? str()
 dic['']
 
@@ -293,15 +293,15 @@
 
 a = [1, ""]
 #? int() str()
 list(a)[1]
 
 #? int() str()
 list(a)[0]
-#? 
+#?
 set(a)[0]
 
 #? int() str()
 list(set(a))[1]
 #? int() str()
 list(list(set(a)))[1]
 
@@ -334,21 +334,34 @@
 #? int()
 tuple((1,))[0]
 
 # implementation detail for lists, should not be visible
 #? []
 list().__iterable
 
+# With a list comprehension.
+for i in set(a for a in [1]):
+    #? int()
+    i
+
 
 # -----------------
 # Recursions
 # -----------------
 
 def to_list(iterable):
     return list(set(iterable))
 
 
 def recursion1(foo):
     return to_list(to_list(foo)) + recursion1(foo)
 
 #? int()
 recursion1([1,2])[0]
+
+# -----------------
+# Merged Arrays
+# -----------------
+
+for x in [1] + ['']:
+    #? int() str()
+    x
```

### Comparing `jedi-0.8.1-final0/test/completion/imports.py` & `jedi-0.9.0/test/completion/imports.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,24 +65,14 @@
 
     # With the latest changes this completion also works, because submodules
     # are always included (some nested import structures lead to this,
     # typically).
     #? ['rename1']
     import_tree.rename1
 
-def from_names():
-    #? ['mod1']
-    from import_tree.pkg.
-    #? ['path']
-    from os.
-
-def builtin_test():
-    #? ['math']
-    import math
-
 def scope_from_import_variable():
     """
     All of them shouldn't work, because "fake" imports don't work in python
     without the use of ``sys.modules`` modifications (e.g. ``os.path`` see also
     github issue #213 for clarification.
     """
     #? 
@@ -93,21 +83,57 @@
     #? 
     a
     #? 
     c
 
 def scope_from_import_variable_with_parenthesis():
     from import_tree.mod2.fake import (
-        a, c
+        a, foobarbaz
     )
 
     #? 
     a
     #? 
-    c
+    foobarbaz
+    # shouldn't complete, should still list the name though.
+    #? ['foobarbaz']
+    foobarbaz
+
+
+def as_imports():
+    from import_tree.mod1 import a as xyz
+    #? int()
+    xyz
+    import not_existant, import_tree.mod1 as foo
+    #? int()
+    foo.a
+    import import_tree.mod1 as bar
+    #? int()
+    bar.a
+
+
+def test_import_priorities():
+    """
+    It's possible to overwrite import paths in an ``__init__.py`` file, by
+    just assigining something there.
+
+    See also #536.
+    """
+    from import_tree import the_pkg, invisible_pkg
+    #? int()
+    invisible_pkg
+    # In real Python, this would be the module, but it's not, because Jedi
+    # doesn't care about most stateful issues such as __dict__, which it would
+    # need to, to do this in a correct way.
+    #? int()
+    the_pkg
+    # Importing foo is still possible, even though inivisible_pkg got changed.
+    #? float()
+    from import_tree.invisible_pkg import foo
+
 
 # -----------------
 # std lib modules
 # -----------------
 import tokenize
 #? ['tok_name']
 tokenize.tok_name
@@ -117,17 +143,14 @@
 #? ['readmodule_ex']
 readmodule_ex
 import os
 
 #? ['dirname']
 os.path.dirname
 
-#? os.path.join
-from os.path import join
-
 from os.path import (
     expanduser
 )
 
 #? os.path.expanduser
 expanduser
 
@@ -170,36 +193,14 @@
     import time
     return time
 
 #? ['sleep']
 func_with_import().sleep
 
 # -----------------
-# completions within imports
-# -----------------
-
-#? ['sqlite3']
-import sqlite3
-
-#? ['classes']
-import classes
-
-#? ['timedelta']
-from datetime import timedel
-
-# should not be possible, because names can only be looked up 1 level deep.
-#? []
-from datetime.timedelta import resolution
-#? []
-from datetime.timedelta import 
-
-#? ['Cursor']
-from sqlite3 import Cursor
-
-# -----------------
 # relative imports
 # -----------------
 
 from .import_tree import mod1
 #? int()
 mod1.a
 
@@ -227,73 +228,18 @@
 #? str()
 imp_tree.a
 
 from . import datetime as mod1
 #? []
 mod1.
 
-#? str()
-imp_tree.a
-
-#? ['some_variable']
-from . import some_variable
-#? ['arrays']
-from . import arrays
-#? []
-from . import import_tree as ren
-
-
-# -----------------
-# special positions -> edge cases
-# -----------------
-import datetime
-
-#? 6 datetime
-from datetime.time import time
-
-#? []
-import datetime.
-#? []
-import datetime.date
-
-#? 18 ['import']
-from import_tree. import pkg
-#? 17 ['mod1', 'mod2', 'random', 'pkg', 'rename1', 'rename2', 'recurse_class1', 'recurse_class2']
-from import_tree. import pkg
-
-#? 18 ['pkg']
-from import_tree.p import pkg
-
-#? 17 ['import_tree']
-from .import_tree import 
-#? 10 ['run']
-from ..run import 
-#? ['run']
-from .. import run
-
-#? []
-from not_a_module import 
-
 # self import
 # this can cause recursions
 from imports import *
 
-#137
-import json
-#? 23 json.dump
-from json import load, dump
-#? 17 json.load
-from json import load, dump
-# without the from clause:
-import json, datetime
-#? 7 json
-import json, datetime
-#? 13 datetime
-import json, datetime
-
 # -----------------
 # packages
 # -----------------
 
 from import_tree.mod1 import c
 #? set
 c
```

### Comparing `jedi-0.8.1-final0/test/completion/stdlib.py` & `jedi-0.9.0/test/completion/stdlib.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 next(reversed(arr))
 next(reversed(arr))
 
 # should not fail if there's no return value.
 def yielder():
     yield None
 
-#? 
+#? None
 next(reversed(yielder()))
 
 # empty reversed should not raise an error
-#? 
+#?
 next(reversed())
 
 #? str()
 next(open(''))
 
 #? int()
 {'a':2}.setdefault('a', 3)
@@ -60,37 +60,44 @@
 # ref
 # -----------------
 import weakref
 
 #? int()
 weakref.proxy(1)
 
-#? weakref.ref
+#? weakref.ref()
 weakref.ref(1)
 #? int()
 weakref.ref(1)()
 
 # -----------------
 # functools
 # -----------------
 import functools
 
 basetwo = functools.partial(int, base=2)
 #? int()
 basetwo()
 
-def a(a, b):
+def function(a, b):
     return a, b
-a = functools.partial(a, 0)
+a = functools.partial(function, 0)
 
 #? int()
 a('')[0]
 #? str()
 a('')[1]
 
+kw = functools.partial(function, b=1.0)
+tup = kw(1)
+#? int()
+tup[0]
+#? float()
+tup[1]
+
 def my_decorator(f):
     @functools.wraps(f)
     def wrapper(*args, **kwds):
         return f(*args, **kwds)
     return wrapper
 
 @my_decorator
@@ -136,20 +143,33 @@
 # copy
 # -----------------
 
 import copy
 #? int()
 copy.deepcopy(1)
 
-#? 
+#?
 copy.copy()
 
 # -----------------
 # json
 # -----------------
 
 # We don't want any results for json, because it depends on IO.
 import json
-#? 
+#?
 json.load('asdf')
-#? 
+#?
 json.loads('[1]')
+
+# -----------------
+# random
+# -----------------
+
+import random
+class A(object):
+    def say(self): pass
+class B(object):
+    def shout(self): pass
+cls = random.choice([A, B])
+#? ['say', 'shout']
+cls().s
```

### Comparing `jedi-0.8.1-final0/test/test_jedi_system.py` & `jedi-0.9.0/test/test_jedi_system.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/test_integration_import.py` & `jedi-0.9.0/test/test_integration_import.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,27 +2,40 @@
 Tests of various import related things that could not be tested with "Black Box
 Tests".
 """
 from jedi import Script
 from .helpers import cwd_at
 from jedi._compatibility import is_py26
 
+import pytest
+
 
 def test_goto_definition_on_import():
     assert Script("import sys_blabla", 1, 8).goto_definitions() == []
     assert len(Script("import sys", 1, 8).goto_definitions()) == 1
 
 
 @cwd_at('jedi')
 def test_complete_on_empty_import():
+    assert Script("from datetime import").completions()[0].name == 'import'
     # should just list the files in the directory
     assert 10 < len(Script("from .", path='').completions()) < 30
-    assert 10 < len(Script("from . import", 1, 5, '').completions()) < 30
-    assert 10 < len(Script("from . import classes", 1, 5, '').completions()) < 30
-    assert len(Script("import").completions()) == 0
+
+    # Global import
+    assert len(Script("from . import", 1, 5, '').completions()) > 30
+    # relative import
+    assert 10 < len(Script("from . import", 1, 6, '').completions()) < 30
+
+    # Global import
+    assert len(Script("from . import classes", 1, 5, '').completions()) > 30
+    # relative import
+    assert 10 < len(Script("from . import classes", 1, 6, '').completions()) < 30
+
+    wanted = set(['ImportError', 'import', 'ImportWarning'])
+    assert set([c.name for c in Script("import").completions()]) == wanted
     if not is_py26:  # python 2.6 doesn't always come with a library `import*`.
         assert len(Script("import import", path='').completions()) > 0
 
     # 111
     assert Script("from datetime import").completions()[0].name == 'import'
     assert Script("from datetime import ").completions()
 
@@ -44,25 +57,27 @@
 def test_named_import():
     """named import - jedi-vim issue #8"""
     s = "import time as dt"
     assert len(Script(s, 1, 15, '/').goto_definitions()) == 1
     assert len(Script(s, 1, 10, '/').goto_definitions()) == 1
 
 
+@pytest.mark.skipif('True', reason='The nested import stuff is still very messy.')
 def test_goto_following_on_imports():
     s = "import multiprocessing.dummy; multiprocessing.dummy"
     g = Script(s).goto_assignments()
     assert len(g) == 1
     assert (g[0].line, g[0].column) != (0, 0)
 
 
 def test_after_from():
     def check(source, result, column=None):
         completions = Script(source, column=column).completions()
         assert [c.name for c in completions] == result
 
+    check('\nfrom os. ', ['path'])
     check('\nfrom os ', ['import'])
     check('from os ', ['import'])
     check('\nfrom os import whatever', ['import'], len('from os im'))
 
     check('from os\\\n', ['import'])
     check('from os \\\n', ['import'])
```

### Comparing `jedi-0.8.1-final0/test/test_speed.py` & `jedi-0.9.0/test/test_speed.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/test_regression.py` & `jedi-0.9.0/test/test_regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import pytest
 import jedi
 from jedi._compatibility import u
 from jedi import Script
 from jedi import api
 from jedi.evaluate import imports
-from jedi.parser import Parser
+from jedi.parser import Parser, load_grammar
 
 #jedi.set_debug_function()
 
 
 class TestRegression(TestCase):
     def test_goto_definition_cursor(self):
 
@@ -51,15 +51,15 @@
         diff_line = get_def(diff_line)
 
         assert should1 == in_name
         assert should1 == under_score
 
         assert should2 == diff_line
 
-        self.assertRaises(jedi.NotFoundError, get_def, cls)
+        assert get_def(cls) == []
 
     @pytest.mark.skipif('True', reason='Skip for now, test case is not really supported.')
     @cwd_at('jedi')
     def test_add_dynamic_mods(self):
         fname = '__main__.py'
         api.settings.additional_dynamic_modules = [fname]
         # Fictional module that defines a function.
@@ -88,27 +88,26 @@
         source = textwrap.dedent("""
         def f():
             pass
 
         class C:
             pass
 
-        variable = f or C""")
+        variable = f if random.choice([0, 1]) else C""")
         defs = Script(source, column=3).goto_definitions()
         defs = sorted(defs, key=lambda d: d.line)
         self.assertEqual([d.description for d in defs],
                          ['def f', 'class C'])
 
-    def test_end_pos(self):
+    def test_end_pos_line(self):
         # jedi issue #150
         s = u("x()\nx( )\nx(  )\nx (  )")
-        parser = Parser(s)
-        for i, s in enumerate(parser.module.statements, 3):
-            for c in s.expression_list():
-                self.assertEqual(c.execution.end_pos[1], i)
+        parser = Parser(load_grammar(), s)
+        for i, s in enumerate(parser.module.statements):
+            assert s.end_pos == (i + 1, i + 3)
 
     def check_definition_by_marker(self, source, after_cursor, names):
         r"""
         Find definitions specified by `after_cursor` and check what found
 
         For example, for the following configuration, you can pass
         ``after_cursor = 'y)'``.::
@@ -166,8 +165,8 @@
     else:
         data = "# coding: latin-1\nfoo = 'm\xf6p'\n".encode("latin-1")
 
     with open(filename1, "wb") as f:
         f.write(data)
     s = Script("from test1 import foo\nfoo.",
                line=2, column=4, path=filename2)
-    s.complete()
+    s.completions()
```

### Comparing `jedi-0.8.1-final0/test/refactor.py` & `jedi-0.9.0/test/refactor.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/test_evaluate/test_pyc.py` & `jedi-0.9.0/test/test_evaluate/test_pyc.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/test_evaluate/test_namespace_package.py` & `jedi-0.9.0/test/test_evaluate/test_namespace_package.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,17 +25,19 @@
             ass = jedi.Script(source).goto_assignments()
             assert len(ass) == 1
             assert ass[0].description == "foo = '%s'" % solution
 
         # completion
         completions = jedi.Script('from pkg import ').completions()
         names = [str(c.name) for c in completions]  # str because of unicode
-        compare = ['foo', 'ns1_file', 'ns1_folder', 'ns2_folder', 'ns2_file']
+        compare = ['foo', 'ns1_file', 'ns1_folder', 'ns2_folder', 'ns2_file',
+                   'pkg_resources', 'pkgutil', '__name__', '__path__',
+                   '__package__', '__file__', '__doc__']
         # must at least contain these items, other items are not important
-        assert not (set(compare) - set(names))
+        assert set(compare) == set(names)
 
         tests = {
             'from pkg import ns2_folder as x': 'ns2_folder!',
             'from pkg import ns2_file as x': 'ns2_file!',
             'from pkg.ns2_folder import nested as x': 'nested!',
             'from pkg import ns1_folder as x': 'ns1_folder!',
             'from pkg import ns1_file as x': 'ns1_file!',
```

### Comparing `jedi-0.8.1-final0/test/test_evaluate/test_buildout_detection.py` & `jedi-0.9.0/test/test_evaluate/test_buildout_detection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
+from textwrap import dedent
 
 from jedi._compatibility import u
 from jedi.evaluate.sys_path import (_get_parent_dir_with_file,
                                     _get_buildout_scripts,
+                                    sys_path_with_modifications,
                                     _check_module)
-from jedi.parser import Parser
+from jedi.evaluate import Evaluator
+from jedi.parser import Parser, load_grammar
 
 from ..helpers import cwd_at
 
 
 @cwd_at('test/test_evaluate/buildout_project/src/proj_name')
 def test_parent_dir_with_file():
     parent = _get_parent_dir_with_file(
@@ -23,49 +26,64 @@
     assert len(scripts) == 1
     curdir = os.path.abspath(os.curdir)
     appdir_path = os.path.normpath(os.path.join(curdir, '../../bin/app'))
     assert scripts[0] == appdir_path
 
 
 def test_append_on_non_sys_path():
-    SRC = u("""
-class Dummy(object):
-    path = []
-
-d = Dummy()
-d.path.append('foo')""")
-    p = Parser(SRC)
-    paths = _check_module(p.module)
+    SRC = dedent(u("""
+        class Dummy(object):
+            path = []
+
+        d = Dummy()
+        d.path.append('foo')"""))
+    grammar = load_grammar()
+    p = Parser(grammar, SRC)
+    paths = _check_module(Evaluator(grammar), p.module)
     assert len(paths) > 0
     assert 'foo' not in paths
 
 
 def test_path_from_invalid_sys_path_assignment():
-    SRC = u("""
-import sys
-sys.path = 'invalid'""")
-    p = Parser(SRC)
-    paths = _check_module(p.module)
+    SRC = dedent(u("""
+        import sys
+        sys.path = 'invalid'"""))
+    grammar = load_grammar()
+    p = Parser(grammar, SRC)
+    paths = _check_module(Evaluator(grammar), p.module)
     assert len(paths) > 0
     assert 'invalid' not in paths
 
 
+@cwd_at('test/test_evaluate/buildout_project/src/proj_name/')
+def test_sys_path_with_modifications():
+    SRC = dedent(u("""
+        import os
+    """))
+    grammar = load_grammar()
+    p = Parser(grammar, SRC)
+    p.module.path = os.path.abspath(os.path.join(os.curdir, 'module_name.py'))
+    paths = sys_path_with_modifications(Evaluator(grammar), p.module)
+    assert '/tmp/.buildout/eggs/important_package.egg' in paths
+
+
 def test_path_from_sys_path_assignment():
-    SRC = u("""
-#!/usr/bin/python
+    SRC = dedent(u("""
+        #!/usr/bin/python
 
-import sys
-sys.path[0:0] = [
-  '/usr/lib/python3.4/site-packages',
-  '/home/test/.buildout/eggs/important_package.egg'
-  ]
-
-path[0:0] = [1]
-
-import important_package
-
-if __name__ == '__main__':
-    sys.exit(important_package.main())""")
-    p = Parser(SRC)
-    paths = _check_module(p.module)
+        import sys
+        sys.path[0:0] = [
+          '/usr/lib/python3.4/site-packages',
+          '/home/test/.buildout/eggs/important_package.egg'
+          ]
+
+        path[0:0] = [1]
+
+        import important_package
+
+        if __name__ == '__main__':
+            sys.exit(important_package.main())"""))
+    grammar = load_grammar()
+    p = Parser(grammar, SRC)
+    paths = _check_module(Evaluator(grammar), p.module)
     assert 1 not in paths
     assert '/home/test/.buildout/eggs/important_package.egg' in paths
```

### Comparing `jedi-0.8.1-final0/test/test_evaluate/test_compiled.py` & `jedi-0.9.0/test/test_evaluate/test_compiled.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from jedi._compatibility import builtins, is_py3
-from jedi.parser.representation import Function
-from jedi.evaluate import compiled
+from jedi.parser import load_grammar
+from jedi.parser.tree import Function
+from jedi.evaluate import compiled, representation
 from jedi.evaluate import Evaluator
 from jedi import Script
 
 
 def test_simple():
-    e = Evaluator()
+    e = Evaluator(load_grammar())
     bltn = compiled.CompiledObject(builtins)
     obj = compiled.CompiledObject('_str_', bltn)
     upper = e.find_types(obj, 'upper')
     assert len(upper) == 1
     objs = list(e.execute(upper[0]))
     assert len(objs) == 1
-    assert objs[0].obj is str
+    assert isinstance(objs[0], representation.Instance)
 
 
 def test_fake_loading():
-    assert isinstance(compiled.create(Evaluator(), next), Function)
+    assert isinstance(compiled.create(Evaluator(load_grammar()), next), Function)
 
     string = compiled.builtin.get_subscope_by_name('str')
     from_name = compiled._create_from_name(
         compiled.builtin,
         string,
         '__init__'
     )
     assert isinstance(from_name, Function)
 
 
 def test_fake_docstr():
-    assert compiled.create(Evaluator(), next).raw_doc == next.__doc__
+    assert compiled.create(Evaluator(load_grammar()), next).raw_doc == next.__doc__
 
 
 def test_parse_function_doc_illegal_docstr():
     docstr = """
     test_func(o
 
     doesn't have a closing bracket.
```

### Comparing `jedi-0.8.1-final0/test/test_evaluate/test_extension.py` & `jedi-0.9.0/test/test_evaluate/test_extension.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Test compiled module
 """
 import os
 
 import jedi
+from ..helpers import cwd_at
+import pytest
 
 
 def test_completions():
     s = jedi.Script('import _ctypes; _ctypes.')
     assert len(s.completions()) >= 15
 
 
@@ -25,7 +27,31 @@
 
 
 def test_call_signatures_stdlib():
     s = jedi.Script('import math; math.cos(')
     sigs = s.call_signatures()
     assert len(sigs) == 1
     assert len(sigs[0].params) == 1
+
+
+# Check only on linux 64 bit platform and Python3.4.
+@pytest.mark.skipif('sys.platform != "linux" or sys.maxsize <= 2**32 or sys.version_info[:2] != (3, 4)')
+@cwd_at('test/test_evaluate')
+def test_init_extension_module():
+    """
+    ``__init__`` extension modules are also packages and Jedi should understand
+    that.
+
+    Originally coming from #472.
+
+    This test was built by the module.c and setup.py combination you can find
+    in the init_extension_module folder. You can easily build the
+    `__init__.cpython-34m.so` by compiling it (create a virtualenv and run
+    `setup.py install`.
+
+    This is also why this test only runs on certain systems (and Python 3.4).
+    """
+    s = jedi.Script('import init_extension_module as i\ni.', path='not_existing.py')
+    assert 'foo' in [c.name for c in s.completions()]
+
+    s = jedi.Script('from init_extension_module import foo\nfoo', path='not_existing.py')
+    assert ['foo'] == [c.name for c in s.completions()]
```

### Comparing `jedi-0.8.1-final0/test/test_evaluate/test_absolute_import.py` & `jedi-0.9.0/test/test_evaluate/test_absolute_import.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
 Tests ``from __future__ import absolute_import`` (only important for
 Python 2.X)
 """
 import jedi
 from jedi._compatibility import u
-from jedi.parser import Parser
+from jedi.parser import Parser, load_grammar
 from .. import helpers
 
 
 def test_explicit_absolute_imports():
     """
     Detect modules with ``from __future__ import absolute_import``.
     """
-    parser = Parser(u("from __future__ import absolute_import"), "test.py")
+    parser = Parser(load_grammar(), u("from __future__ import absolute_import"), "test.py")
     assert parser.module.has_explicit_absolute_import
 
 
 def test_no_explicit_absolute_imports():
     """
      Detect modules without ``from __future__ import absolute_import``.
     """
-    parser = Parser(u("1"), "test.py")
+    parser = Parser(load_grammar(), u("1"), "test.py")
     assert not parser.module.has_explicit_absolute_import
 
 
 def test_dont_break_imports_without_namespaces():
     """
     The code checking for ``from __future__ import absolute_import`` shouldn't
     assume that all imports have non-``None`` namespaces.
     """
     src = u("from __future__ import absolute_import\nimport xyzzy")
-    parser = Parser(src, "test.py")
+    parser = Parser(load_grammar(), src, "test.py")
     assert parser.module.has_explicit_absolute_import
 
 
 @helpers.cwd_at("test/test_evaluate/absolute_import")
 def test_can_complete_when_shadowing():
     script = jedi.Script(path="unittest.py")
     assert script.completions()
```

### Comparing `jedi-0.8.1-final0/test/helpers.py` & `jedi-0.9.0/test/helpers.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/test/conftest.py` & `jedi-0.9.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/jedi/evaluate/recursion.py` & `jedi-0.9.0/jedi/evaluate/recursion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Recursions are the recipe of |jedi| to conquer Python code. However, someone
 must stop recursions going mad. Some settings are here to make |jedi| stop at
 the right time. You can read more about them :ref:`here <settings-recursion>`.
 
 Next to :mod:`jedi.evaluate.cache` this module also makes |jedi| not
-thread-safe. Why?  ``ExecutionRecursionDecorator`` uses class variables to
+thread-safe. Why?  ``execution_recursion_decorator`` uses class variables to
 count the function calls.
 """
-from jedi.parser import representation as pr
 from jedi import debug
 from jedi import settings
 from jedi.evaluate import compiled
 from jedi.evaluate import iterable
 
 
 def recursion_decorator(func):
@@ -77,39 +76,32 @@
         self.position = stmt.start_pos
         self.parent = parent
         self.stmt = stmt
 
         # Don't check param instances, they are not causing recursions
         # The same's true for the builtins, because the builtins are really
         # simple.
-        self.is_ignored = isinstance(stmt, pr.Param) \
-            or (self.script == compiled.builtin)
+        self.is_ignored = self.script == compiled.builtin
 
     def __eq__(self, other):
         if not other:
             return None
 
-        # List Comprehensions start on the same line as its statement.
-        # Therefore we have the unfortunate situation of the same start_pos for
-        # two statements.
-        is_list_comp = lambda x: isinstance(x, pr.ListComprehension)
         return self.script == other.script \
             and self.position == other.position \
-            and not is_list_comp(self.stmt.parent) \
-            and not is_list_comp(other.parent) \
             and not self.is_ignored and not other.is_ignored
 
 
 def execution_recursion_decorator(func):
-    def run(execution, evaluate_generator=False):
+    def run(execution, **kwargs):
         detector = execution._evaluator.execution_recursion_detector
-        if detector.push_execution(execution, evaluate_generator):
+        if detector.push_execution(execution):
             result = []
         else:
-            result = func(execution, evaluate_generator)
+            result = func(execution, **kwargs)
         detector.pop_execution()
         return result
 
     return run
 
 
 class ExecutionRecursionDetector(object):
@@ -119,43 +111,43 @@
     """
     def __init__(self):
         self.recursion_level = 0
         self.parent_execution_funcs = []
         self.execution_funcs = set()
         self.execution_count = 0
 
-    def __call__(self, execution, evaluate_generator=False):
+    def __call__(self, execution):
         debug.dbg('Execution recursions: %s', execution, self.recursion_level,
                   self.execution_count, len(self.execution_funcs))
-        if self.check_recursion(execution, evaluate_generator):
+        if self.check_recursion(execution):
             result = []
         else:
-            result = self.func(execution, evaluate_generator)
+            result = self.func(execution)
         self.pop_execution()
         return result
 
     def pop_execution(cls):
         cls.parent_execution_funcs.pop()
         cls.recursion_level -= 1
 
-    def push_execution(cls, execution, evaluate_generator):
+    def push_execution(cls, execution):
         in_par_execution_funcs = execution.base in cls.parent_execution_funcs
         in_execution_funcs = execution.base in cls.execution_funcs
         cls.recursion_level += 1
         cls.execution_count += 1
         cls.execution_funcs.add(execution.base)
         cls.parent_execution_funcs.append(execution.base)
 
         if cls.execution_count > settings.max_executions:
             return True
 
         if isinstance(execution.base, (iterable.Array, iterable.Generator)):
             return False
         module = execution.get_parent_until()
-        if evaluate_generator or module == compiled.builtin:
+        if module == compiled.builtin:
             return False
 
         if in_par_execution_funcs:
             if cls.recursion_level > settings.max_function_recursion_level:
                 return True
         if in_execution_funcs and \
                 len(cls.execution_funcs) > settings.max_until_execution_unique:
```

### Comparing `jedi-0.8.1-final0/jedi/evaluate/__init__.py` & `jedi-0.9.0/jedi/evaluate/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,382 +1,379 @@
 """
 Evaluation of Python code in |jedi| is based on three assumptions:
 
-* Code is recursive (to weaken this assumption, the
-  :mod:`jedi.evaluate.dynamic` module exists).
+* The code uses as least side effects as possible. Jedi understands certain
+  list/tuple/set modifications, but there's no guarantee that Jedi detects
+  everything (list.append in different modules for example).
 * No magic is being used:
 
   - metaclasses
   - ``setattr()`` / ``__import__()``
   - writing to ``globals()``, ``locals()``, ``object.__dict__``
 * The programmer is not a total dick, e.g. like `this
   <https://github.com/davidhalter/jedi/issues/24>`_ :-)
 
-That said, there's mainly one entry point in this script: ``eval_statement``.
-This is where autocompletion starts. Everything you want to complete is either
-a ``Statement`` or some special name like ``class``, which is easy to complete.
+The actual algorithm is based on a principle called lazy evaluation. If you
+don't know about it, google it.  That said, the typical entry point for static
+analysis is calling ``eval_statement``. There's separate logic for
+autocompletion in the API, the evaluator is all about evaluating an expression.
 
-Therefore you need to understand what follows after ``eval_statement``. Let's
+Now you need to understand what follows after ``eval_statement``. Let's
 make an example::
 
     import datetime
     datetime.date.toda# <-- cursor here
 
 First of all, this module doesn't care about completion. It really just cares
 about ``datetime.date``. At the end of the procedure ``eval_statement`` will
-return the ``datetime`` class.
+return the ``date`` class.
 
 To *visualize* this (simplified):
 
-- ``eval_statement`` - ``<Statement: datetime.date>``
+- ``Evaluator.eval_statement`` doesn't do much, because there's no assignment.
+- ``Evaluator.eval_element`` cares for resolving the dotted path
+- ``Evaluator.find_types`` searches for global definitions of datetime, which
+  it finds in the definition of an import, by scanning the syntax tree.
+- Using the import logic, the datetime module is found.
+- Now ``find_types`` is called again by ``eval_element`` to find ``date``
+  inside the datetime module.
+
+Now what would happen if we wanted ``datetime.date.foo.bar``? Two more
+calls to ``find_types``. However the second call would be ignored, because the
+first one would return nothing (there's no foo attribute in ``date``).
 
-    - Unpacking of the statement into ``[[<Call: datetime.date>]]``
-- ``eval_expression_list``, calls ``eval_call`` with ``<Call: datetime.date>``
-- ``eval_call`` - searches the ``datetime`` name within the module.
-
-This is exactly where it starts to get complicated. Now recursions start to
-kick in. The statement has not been resolved fully, but now we need to resolve
-the datetime import. So it continues
-
-- follow import, which happens in the :mod:`jedi.evaluate.imports` module.
-- now the same ``eval_call`` as above calls ``follow_path`` to follow the
-  second part of the statement ``date``.
-- After ``follow_path`` returns with the desired ``datetime.date`` class, the
-  result is being returned and the recursion finishes.
-
-Now what would happen if we wanted ``datetime.date.foo.bar``? Just two more
-calls to ``follow_path`` (which calls itself with a recursion). What if the
-import would contain another Statement like this::
+What if the import would contain another ``ExprStmt`` like this::
 
     from foo import bar
     Date = bar.baz
 
 Well... You get it. Just another ``eval_statement`` recursion. It's really
-easy. Just that Python is not that easy sometimes. To understand tuple
-assignments and different class scopes, a lot more code had to be written.  Yet
-we're still not talking about Descriptors and Nested List Comprehensions, just
-the simple stuff.
-
-So if you want to change something, write a test and then just change what you
-want. This module has been tested by about 600 tests. Don't be afraid to break
-something. The tests are good enough.
+easy. Python can obviously get way more complicated then this. To understand
+tuple assignments, list comprehensions and everything else, a lot more code had
+to be written.
+
+Jedi has been tested very well, so you can just start modifying code. It's best
+to write your own test first for your "new" feature. Don't be scared of
+breaking stuff. As long as the tests pass, you're most likely to be fine.
 
-I need to mention now that this recursive approach is really good because it
+I need to mention now that lazy evaluation is really good because it
 only *evaluates* what needs to be *evaluated*. All the statements and modules
-that are not used are just being ignored. It's a little bit similar to the
-backtracking algorithm.
-
-
-.. todo:: nonlocal statement, needed or can be ignored? (py3k)
+that are not used are just being ignored.
 """
-import itertools
 
-from jedi._compatibility import next, hasattr, unicode
-from jedi.parser import representation as pr
-from jedi.parser.tokenize import Token
-from jedi.parser import fast
+import copy
+from itertools import chain
+
+from jedi.parser import tree
 from jedi import debug
 from jedi.evaluate import representation as er
 from jedi.evaluate import imports
 from jedi.evaluate import recursion
 from jedi.evaluate import iterable
 from jedi.evaluate.cache import memoize_default
 from jedi.evaluate import stdlib
 from jedi.evaluate import finder
 from jedi.evaluate import compiled
 from jedi.evaluate import precedence
-from jedi.evaluate.helpers import FakeStatement
+from jedi.evaluate import param
+from jedi.evaluate import helpers
 
 
 class Evaluator(object):
-    def __init__(self):
+    def __init__(self, grammar):
+        self.grammar = grammar
         self.memoize_cache = {}  # for memoize decorators
-        self.import_cache = {}  # like `sys.modules`.
+        # To memorize modules -> equals `sys.modules`.
+        self.modules = {}  # like `sys.modules`.
         self.compiled_cache = {}  # see `compiled.create()`
         self.recursion_detector = recursion.RecursionDetector()
         self.execution_recursion_detector = recursion.ExecutionRecursionDetector()
         self.analysis = []
 
+    def wrap(self, element):
+        if isinstance(element, tree.Class):
+            return er.Class(self, element)
+        elif isinstance(element, tree.Function):
+            if isinstance(element, tree.Lambda):
+                return er.LambdaWrapper(self, element)
+            else:
+                return er.Function(self, element)
+        elif isinstance(element, (tree.Module)) \
+                and not isinstance(element, er.ModuleWrapper):
+            return er.ModuleWrapper(self, element)
+        else:
+            return element
+
     def find_types(self, scope, name_str, position=None, search_global=False,
-                   is_goto=False, resolve_decorator=True):
+                   is_goto=False):
         """
         This is the search function. The most important part to debug.
         `remove_statements` and `filter_statements` really are the core part of
         this completion.
 
         :param position: Position of the last statement -> tuple of line, column
         :return: List of Names. Their parents are the types.
         """
         f = finder.NameFinder(self, scope, name_str, position)
         scopes = f.scopes(search_global)
         if is_goto:
             return f.filter_name(scopes)
-        return f.find(scopes, resolve_decorator, search_global)
+        return f.find(scopes, search_global)
 
     @memoize_default(default=[], evaluator_is_first_arg=True)
     @recursion.recursion_decorator
     @debug.increase_indent
     def eval_statement(self, stmt, seek_name=None):
         """
         The starting point of the completion. A statement always owns a call
         list, which are the calls, that a statement does. In case multiple
         names are defined in the statement, `seek_name` returns the result for
         this name.
 
-        :param stmt: A `pr.Statement`.
+        :param stmt: A `tree.ExprStmt`.
         """
         debug.dbg('eval_statement %s (%s)', stmt, seek_name)
-        expression_list = stmt.expression_list()
-        if isinstance(stmt, FakeStatement):
-            return expression_list  # Already contains the results.
-
-        result = self.eval_expression_list(expression_list)
-
-        ass_details = stmt.assignment_details
-        if ass_details and ass_details[0][1] != '=' and not isinstance(stmt, er.InstanceElement):  # TODO don't check for this.
-            expr_list, operator = ass_details[0]
+        types = self.eval_element(stmt.get_rhs())
+
+        if seek_name:
+            types = finder.check_tuple_assignments(types, seek_name)
+
+        first_operation = stmt.first_operation()
+        if first_operation not in ('=', None) and not isinstance(stmt, er.InstanceElement):  # TODO don't check for this.
             # `=` is always the last character in aug assignments -> -1
-            operator = operator[:-1]
-            name = str(expr_list[0].name)
-            parent = stmt.parent
-            if isinstance(parent, (pr.SubModule, fast.Module)):
-                parent = er.ModuleWrapper(self, parent)
-            left = self.find_types(parent, name, stmt.start_pos)
-            if isinstance(stmt.parent, pr.ForFlow):
-                # iterate through result and add the values, that's possible
+            operator = copy.copy(first_operation)
+            operator.value = operator.value[:-1]
+            name = str(stmt.get_defined_names()[0])
+            parent = self.wrap(stmt.get_parent_scope())
+            left = self.find_types(parent, name, stmt.start_pos, search_global=True)
+            if isinstance(stmt.get_parent_until(tree.ForStmt), tree.ForStmt):
+                # Iterate through result and add the values, that's possible
                 # only in for loops without clutter, because they are
                 # predictable.
-                for r in result:
+                for r in types:
                     left = precedence.calculate(self, left, operator, [r])
-                result = left
-            else:
-                result = precedence.calculate(self, left, operator, result)
-        elif len(stmt.get_defined_names()) > 1 and seek_name and ass_details:
-            # Assignment checking is only important if the statement defines
-            # multiple variables.
-            new_result = []
-            for ass_expression_list, op in ass_details:
-                new_result += finder.find_assignments(ass_expression_list[0], result, seek_name)
-            result = new_result
-        return result
-
-    def eval_expression_list(self, expression_list):
-        """
-        `expression_list` can be either `pr.Array` or `list of list`.
-        It is used to evaluate a two dimensional object, that has calls, arrays and
-        operators in it.
-        """
-        debug.dbg('eval_expression_list: %s', expression_list)
-        p = precedence.create_precedence(expression_list)
-        return self.process_precedence_element(p) or []
-
-    def process_precedence_element(self, el):
-        if el is None:
-            return None
-        else:
-            if isinstance(el, precedence.Precedence):
-                return self._eval_precedence(el)
+                types = left
             else:
-                # normal element, no operators
-                return self.eval_statement_element(el)
-
-    def _eval_precedence(self, _precedence):
-        left = self.process_precedence_element(_precedence.left)
-        right = self.process_precedence_element(_precedence.right)
-        return precedence.calculate(self, left, _precedence.operator, right)
-
-    def eval_statement_element(self, element):
-        if pr.Array.is_type(element, pr.Array.NOARRAY):
-            try:
-                lst_cmp = element[0].expression_list()[0]
-                if not isinstance(lst_cmp, pr.ListComprehension):
-                    raise IndexError
-            except IndexError:
-                r = list(itertools.chain.from_iterable(self.eval_statement(s)
-                                                       for s in element))
+                types = precedence.calculate(self, left, operator, types)
+        debug.dbg('eval_statement result %s', types)
+        return types
+
+    @memoize_default(evaluator_is_first_arg=True)
+    def eval_element(self, element):
+        if isinstance(element, iterable.AlreadyEvaluated):
+            return list(element)
+        elif isinstance(element, iterable.MergedNodes):
+            return iterable.unite(self.eval_element(e) for e in element)
+
+        debug.dbg('eval_element %s@%s', element, element.start_pos)
+        if isinstance(element, (tree.Name, tree.Literal)) or tree.is_node(element, 'atom'):
+            return self._eval_atom(element)
+        elif isinstance(element, tree.Keyword):
+            # For False/True/None
+            if element.value in ('False', 'True', 'None'):
+                return [compiled.builtin.get_by_name(element.value)]
             else:
-                r = [iterable.GeneratorComprehension(self, lst_cmp)]
-            call_path = element.generate_call_path()
-            next(call_path, None)  # the first one has been used already
-            return self.follow_path(call_path, r, element.parent)
-        elif isinstance(element, pr.ListComprehension):
-            return self.eval_statement(element.stmt)
-        elif isinstance(element, pr.Lambda):
-            return [er.Function(self, element)]
-        # With things like params, these can also be functions...
-        elif isinstance(element, pr.Base) and element.isinstance(
-                er.Function, er.Class, er.Instance, iterable.ArrayInstance):
-            return [element]
-        # The string tokens are just operations (+, -, etc.)
-        elif isinstance(element, compiled.CompiledObject):
-            return [element]
-        elif isinstance(element, Token):
-            return []
+                return []
+        elif element.isinstance(tree.Lambda):
+            return [er.LambdaWrapper(self, element)]
+        elif element.isinstance(er.LambdaWrapper):
+            return [element]  # TODO this is no real evaluation.
+        elif element.type == 'expr_stmt':
+            return self.eval_statement(element)
+        elif element.type == 'power':
+            types = self._eval_atom(element.children[0])
+            for trailer in element.children[1:]:
+                if trailer == '**':  # has a power operation.
+                    raise NotImplementedError
+                types = self.eval_trailer(types, trailer)
+
+            return types
+        elif element.type in ('testlist_star_expr', 'testlist',):
+            # The implicit tuple in statements.
+            return [iterable.ImplicitTuple(self, element)]
+        elif element.type in ('not_test', 'factor'):
+            types = self.eval_element(element.children[-1])
+            for operator in element.children[:-1]:
+                types = list(precedence.factor_calculate(self, types, operator))
+            return types
+        elif element.type == 'test':
+            # `x if foo else y` case.
+            return (self.eval_element(element.children[0]) +
+                    self.eval_element(element.children[-1]))
+        elif element.type == 'operator':
+            # Must be an ellipsis, other operators are not evaluated.
+            return []  # Ignore for now.
+        elif element.type == 'dotted_name':
+            types = self._eval_atom(element.children[0])
+            for next_name in element.children[2::2]:
+                types = list(chain.from_iterable(self.find_types(typ, next_name)
+                                                 for typ in types))
+            return types
         else:
-            return self.eval_call(element)
-
-    def eval_call(self, call):
-        """Follow a call is following a function, variable, string, etc."""
-        path = call.generate_call_path()
-
-        # find the statement of the Scope
-        s = call
-        while not s.parent.isinstance(pr.IsScope):
-            s = s.parent
-        par = s.parent
-        return self.eval_call_path(path, par, s.start_pos)
+            return precedence.calculate_children(self, element.children)
 
-    def eval_call_path(self, path, scope, position):
+    def _eval_atom(self, atom):
         """
-        Follows a path generated by `pr.StatementElement.generate_call_path()`.
-        """
-        current = next(path)
-
-        if isinstance(current, pr.Array):
-            types = [iterable.Array(self, current)]
+        Basically to process ``atom`` nodes. The parser sometimes doesn't
+        generate the node (because it has just one child). In that case an atom
+        might be a name or a literal as well.
+        """
+        if isinstance(atom, tree.Name):
+            # This is the first global lookup.
+            stmt = atom.get_definition()
+            scope = stmt.get_parent_until(tree.IsScope, include_current=True)
+            if isinstance(stmt, tree.CompFor):
+                stmt = stmt.get_parent_until((tree.ClassOrFunc, tree.ExprStmt))
+            if stmt.type != 'expr_stmt':
+                # We only need to adjust the start_pos for statements, because
+                # there the name cannot be used.
+                stmt = atom
+            return self.find_types(scope, atom, stmt.start_pos, search_global=True)
+        elif isinstance(atom, tree.Literal):
+            return [compiled.create(self, atom.eval())]
         else:
-            if isinstance(current, pr.NamePart):
-                # This is the first global lookup.
-                types = self.find_types(scope, current, position=position,
-                                        search_global=True)
-            else:
-                # for pr.Literal
-                types = [compiled.create(self, current.value)]
-            types = imports.follow_imports(self, types)
-
-        return self.follow_path(path, types, scope)
-
-    def follow_path(self, path, types, call_scope):
-        """
-        Follows a path like::
-
-            self.follow_path(iter(['Foo', 'bar']), [a_type], from_somewhere)
-
-        to follow a call like ``module.a_type.Foo.bar`` (in ``from_somewhere``).
-        """
-        results_new = []
-        iter_paths = itertools.tee(path, len(types))
-
-        for i, typ in enumerate(types):
-            fp = self._follow_path(iter_paths[i], typ, call_scope)
-            if fp is not None:
-                results_new += fp
+            c = atom.children
+            # Parentheses without commas are not tuples.
+            if c[0] == '(' and not len(c) == 2 \
+                    and not(tree.is_node(c[1], 'testlist_comp')
+                            and len(c[1].children) > 1):
+                return self.eval_element(c[1])
+            try:
+                comp_for = c[1].children[1]
+            except (IndexError, AttributeError):
+                pass
             else:
-                # This means stop iteration.
-                return types
-        return results_new
+                if isinstance(comp_for, tree.CompFor):
+                    return [iterable.Comprehension.from_atom(self, atom)]
+            return [iterable.Array(self, atom)]
+
+    def eval_trailer(self, types, trailer):
+        trailer_op, node = trailer.children[:2]
+        if node == ')':  # `arglist` is optional.
+            node = ()
+        new_types = []
+        for typ in types:
+            debug.dbg('eval_trailer: %s in scope %s', trailer, typ)
+            if trailer_op == '.':
+                new_types += self.find_types(typ, node)
+            elif trailer_op == '(':
+                new_types += self.execute(typ, node, trailer)
+            elif trailer_op == '[':
+                try:
+                    get = typ.get_index_types
+                except AttributeError:
+                    debug.warning("TypeError: '%s' object is not subscriptable"
+                                  % typ)
+                else:
+                    new_types += get(self, node)
+        return new_types
 
-    def _follow_path(self, path, typ, scope):
+    def execute_evaluated(self, obj, *args):
         """
-        Uses a generator and tries to complete the path, e.g.::
-
-            foo.bar.baz
-
-        `_follow_path` is only responsible for completing `.bar.baz`, the rest
-        is done in the `follow_call` function.
+        Execute a function with already executed arguments.
         """
-        # current is either an Array or a Scope.
-        try:
-            current = next(path)
-        except StopIteration:
-            return None
-        debug.dbg('_follow_path: %s in scope %s', current, typ)
-
-        result = []
-        if isinstance(current, pr.Array):
-            # This must be an execution, either () or [].
-            if current.type == pr.Array.LIST:
-                if hasattr(typ, 'get_index_types'):
-                    if isinstance(typ, compiled.CompiledObject):
-                        # CompiledObject doesn't contain an evaluator instance.
-                        result = typ.get_index_types(self, current)
-                    else:
-                        result = typ.get_index_types(current)
-            elif current.type not in [pr.Array.DICT]:
-                # Scope must be a class or func - make an instance or execution.
-                result = self.execute(typ, current)
-            else:
-                # Curly braces are not allowed, because they make no sense.
-                debug.warning('strange function call with {} %s %s', current, typ)
-        else:
-            # The function must not be decorated with something else.
-            if typ.isinstance(er.Function):
-                typ = typ.get_magic_function_scope()
-            else:
-                # This is the typical lookup while chaining things.
-                if filter_private_variable(typ, scope, current):
-                    return []
-            types = self.find_types(typ, current)
-            result = imports.follow_imports(self, types)
-        return self.follow_path(path, result, scope)
+        args = [iterable.AlreadyEvaluated([arg]) for arg in args]
+        return self.execute(obj, args)
 
     @debug.increase_indent
-    def execute(self, obj, params=(), evaluate_generator=False):
+    def execute(self, obj, arguments=(), trailer=None):
+        if not isinstance(arguments, param.Arguments):
+            arguments = param.Arguments(self, arguments, trailer)
+
         if obj.isinstance(er.Function):
             obj = obj.get_decorated_func()
 
-        debug.dbg('execute: %s %s', obj, params)
+        debug.dbg('execute: %s %s', obj, arguments)
         try:
-            return stdlib.execute(self, obj, params)
+            # Some stdlib functions like super(), namedtuple(), etc. have been
+            # hard-coded in Jedi to support them.
+            return stdlib.execute(self, obj, arguments)
         except stdlib.NotInStdLib:
             pass
 
-        if isinstance(obj, iterable.GeneratorMethod):
-            return obj.execute()
-        elif obj.isinstance(compiled.CompiledObject):
-            if obj.is_executable_class():
-                return [er.Instance(self, obj, params)]
-            else:
-                return list(obj.execute_function(self, params))
-        elif obj.isinstance(er.Class):
-            # There maybe executions of executions.
-            return [er.Instance(self, obj, params)]
+        try:
+            func = obj.py__call__
+        except AttributeError:
+            debug.warning("no execution possible %s", obj)
+            return []
         else:
-            stmts = []
-            if obj.isinstance(er.Function):
-                stmts = er.FunctionExecution(self, obj, params).get_return_types(evaluate_generator)
-            else:
-                if hasattr(obj, 'execute_subscope_by_name'):
-                    try:
-                        stmts = obj.execute_subscope_by_name('__call__', params)
-                    except KeyError:
-                        debug.warning("no __call__ func available %s", obj)
+            types = func(self, arguments)
+            debug.dbg('execute result: %s in %s', types, obj)
+            return types
+
+    def goto_definition(self, name):
+        def_ = name.get_definition()
+        if def_.type == 'expr_stmt' and name in def_.get_defined_names():
+            return self.eval_statement(def_, name)
+        call = helpers.call_of_name(name)
+        return self.eval_element(call)
+
+    def goto(self, name):
+        def resolve_implicit_imports(names):
+            for name in names:
+                if isinstance(name.parent, helpers.FakeImport):
+                    # Those are implicit imports.
+                    s = imports.ImportWrapper(self, name)
+                    for n in s.follow(is_goto=True):
+                        yield n
                 else:
-                    debug.warning("no execution possible %s", obj)
-
-            debug.dbg('execute result: %s in %s', stmts, obj)
-            return imports.follow_imports(self, stmts)
+                    yield name
 
-    def goto(self, stmt, call_path):
-        scope = stmt.get_parent_until(pr.IsScope)
-        pos = stmt.start_pos
-        call_path, search_name_part = call_path[:-1], call_path[-1]
-
-        if call_path:
-            scopes = self.eval_call_path(iter(call_path), scope, pos)
-            search_global = False
-            pos = None
+        stmt = name.get_definition()
+        par = name.parent
+        if par.type == 'argument' and par.children[1] == '=' and par.children[0] == name:
+            # Named param goto.
+            trailer = par.parent
+            if trailer.type == 'arglist':
+                trailer = trailer.parent
+            if trailer.type != 'classdef':
+                if trailer.type == 'decorator':
+                    types = self.eval_element(trailer.children[1])
+                else:
+                    i = trailer.parent.children.index(trailer)
+                    to_evaluate = trailer.parent.children[:i]
+                    types = self.eval_element(to_evaluate[0])
+                    for trailer in to_evaluate[1:]:
+                        types = self.eval_trailer(types, trailer)
+                param_names = []
+                for typ in types:
+                    try:
+                        params = typ.params
+                    except AttributeError:
+                        pass
+                    else:
+                        param_names += [param.name for param in params
+                                        if param.name.value == name.value]
+                return param_names
+        elif isinstance(par, tree.ExprStmt) and name in par.get_defined_names():
+            # Only take the parent, because if it's more complicated than just
+            # a name it's something you can "goto" again.
+            return [name]
+        elif isinstance(par, (tree.Param, tree.Function, tree.Class)) and par.name is name:
+            return [name]
+        elif isinstance(stmt, tree.Import):
+            modules = imports.ImportWrapper(self, name).follow(is_goto=True)
+            return list(resolve_implicit_imports(modules))
+        elif par.type == 'dotted_name':  # Is a decorator.
+            index = par.children.index(name)
+            if index > 0:
+                new_dotted = helpers.deep_ast_copy(par)
+                new_dotted.children[index - 1:] = []
+                types = self.eval_element(new_dotted)
+                return resolve_implicit_imports(iterable.unite(
+                    self.find_types(typ, name, is_goto=True) for typ in types
+                ))
+
+        scope = name.get_parent_scope()
+        if tree.is_node(name.parent, 'trailer'):
+            call = helpers.call_of_name(name, cut_own_trailer=True)
+            types = self.eval_element(call)
+            return resolve_implicit_imports(iterable.unite(
+                self.find_types(typ, name, is_goto=True) for typ in types
+            ))
         else:
-            # TODO does this exist? i don't think so
-            scopes = [scope]
-            search_global = True
-        follow_res = []
-        for s in scopes:
-            follow_res += self.find_types(s, search_name_part, pos,
-                                          search_global=search_global, is_goto=True)
-        return follow_res, search_name_part
-
-
-def filter_private_variable(scope, call_scope, var_name):
-    """private variables begin with a double underline `__`"""
-    var_name = str(var_name)  # var_name could be a NamePart
-    if isinstance(var_name, (str, unicode)) and isinstance(scope, er.Instance)\
-            and var_name.startswith('__') and not var_name.endswith('__'):
-        s = call_scope.get_parent_until((pr.Class, er.Instance, compiled.CompiledObject))
-        if s != scope:
-            if isinstance(scope.base, compiled.CompiledObject):
-                if s != scope.base:
-                    return True
-            else:
-                if s != scope.base.base:
-                    return True
-    return False
+            if stmt.type != 'expr_stmt':
+                # We only need to adjust the start_pos for statements, because
+                # there the name cannot be used.
+                stmt = name
+            return self.find_types(scope, name, stmt.start_pos,
+                                   search_global=True, is_goto=True)
```

### Comparing `jedi-0.8.1-final0/jedi/evaluate/representation.py` & `jedi-0.9.0/jedi/evaluate/iterable.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,569 +1,631 @@
 """
-Like described in the :mod:`jedi.evaluate.parsing_representation` module,
-there's a need for an ast like module to represent the states of parsed
-modules.
-
-But now there are also structures in Python that need a little bit more than
-that. An ``Instance`` for example is only a ``Class`` before it is
-instantiated. This class represents these cases.
+Contains all classes and functions to deal with lists, dicts, generators and
+iterators in general.
 
-So, why is there also a ``Class`` class here? Well, there are decorators and
-they change classes in Python 3.
+Array modifications
+*******************
+
+If the content of an array (``set``/``list``) is requested somewhere, the
+current module will be checked for appearances of ``arr.append``,
+``arr.insert``, etc.  If the ``arr`` name points to an actual array, the
+content will be added
+
+This can be really cpu intensive, as you can imagine. Because |jedi| has to
+follow **every** ``append`` and check wheter it's the right array. However this
+works pretty good, because in *slow* cases, the recursion detector and other
+settings will stop this process.
+
+It is important to note that:
+
+1. Array modfications work only in the current module.
+2. Jedi only checks Array additions; ``list.pop``, etc are ignored.
 """
-import copy
-import os
-import pkgutil
-
-from jedi._compatibility import use_metaclass, unicode
-from jedi.parser import representation as pr
-from jedi.parser.tokenize import Token
-from jedi import debug
+from itertools import chain
+
 from jedi import common
-from jedi.evaluate.cache import memoize_default, CachedMetaClass
+from jedi import debug
+from jedi import settings
+from jedi._compatibility import use_metaclass, is_py3, unicode
+from jedi.parser import tree
 from jedi.evaluate import compiled
-from jedi.evaluate import recursion
-from jedi.evaluate import iterable
-from jedi.evaluate import docstrings
 from jedi.evaluate import helpers
-from jedi.evaluate import param
+from jedi.evaluate.cache import CachedMetaClass, memoize_default
+from jedi.evaluate import analysis
 
 
-class Executable(pr.IsScope):
-    """
-    An instance is also an executable - because __init__ is called
-    :param var_args: The param input array, consist of `pr.Array` or list.
-    """
-    def __init__(self, evaluator, base, var_args=()):
-        self._evaluator = evaluator
-        self.base = base
-        self.var_args = var_args
-
-    def get_parent_until(self, *args, **kwargs):
-        return self.base.get_parent_until(*args, **kwargs)
+def unite(iterable):
+    """Turns a two dimensional array into a one dimensional."""
+    return list(chain.from_iterable(iterable))
 
-    @common.safe_property
-    def parent(self):
-        return self.base.parent
 
+class IterableWrapper(tree.Base):
+    def is_class(self):
+        return False
 
-class Instance(use_metaclass(CachedMetaClass, Executable)):
-    """
-    This class is used to evaluate instances.
-    """
-    def __init__(self, evaluator, base, var_args=()):
-        super(Instance, self).__init__(evaluator, base, var_args)
-        if str(base.name) in ['list', 'set'] \
-                and compiled.builtin == base.get_parent_until():
-            # compare the module path with the builtin name.
-            self.var_args = iterable.check_array_instances(evaluator, self)
-        else:
-            # need to execute the __init__ function, because the dynamic param
-            # searching needs it.
-            with common.ignored(KeyError):
-                self.execute_subscope_by_name('__init__', self.var_args)
-        # Generated instances are classes that are just generated by self
-        # (No var_args) used.
-        self.is_generated = False
 
+class GeneratorMixin(object):
     @memoize_default()
-    def _get_method_execution(self, func):
-        func = InstanceElement(self._evaluator, self, func, True)
-        return FunctionExecution(self._evaluator, func, self.var_args)
+    def names_dicts(self, search_global=False):  # is always False
+        dct = {}
+        executes_generator = '__next__', 'send', 'next'
+        for names in compiled.generator_obj.names_dict.values():
+            for name in names:
+                if name.value in executes_generator:
+                    parent = GeneratorMethod(self, name.parent)
+                    dct[name.value] = [helpers.FakeName(name.name, parent, is_definition=True)]
+                else:
+                    dct[name.value] = [name]
+        yield dct
+
+    def get_index_types(self, evaluator, index_array):
+        #debug.warning('Tried to get array access on a generator: %s', self)
+        analysis.add(self._evaluator, 'type-error-generator', index_array)
+        return []
 
-    def _get_func_self_name(self, func):
+    def get_exact_index_types(self, index):
         """
-        Returns the name of the first param in a class method (which is
-        normally self.
+        Exact lookups are used for tuple lookups, which are perfectly fine if
+        used with generators.
         """
-        try:
-            return str(func.params[0].get_name())
-        except IndexError:
-            return None
+        return [self.iter_content()[index]]
 
-    @memoize_default([])
-    def get_self_attributes(self):
-        def add_self_dot_name(name):
-            """
-            Need to copy and rewrite the name, because names are now
-            ``instance_usage.variable`` instead of ``self.variable``.
-            """
-            n = copy.copy(name)
-            n.names = n.names[1:]
-            n._get_code = unicode(n.names[-1])
-            names.append(InstanceElement(self._evaluator, self, n))
-
-        names = []
-        # This loop adds the names of the self object, copies them and removes
-        # the self.
-        for sub in self.base.subscopes:
-            if isinstance(sub, pr.Class):
-                continue
-            # Get the self name, if there's one.
-            self_name = self._get_func_self_name(sub)
-            if not self_name:
-                continue
+    def py__bool__(self):
+        return True
 
-            if sub.name.get_code() == '__init__':
-                # ``__init__`` is special because the params need are injected
-                # this way. Therefore an execution is necessary.
-                if not sub.decorators:
-                    # __init__ decorators should generally just be ignored,
-                    # because to follow them and their self variables is too
-                    # complicated.
-                    sub = self._get_method_execution(sub)
-            for n in sub.get_defined_names():
-                # Only names with the selfname are being added.
-                # It is also important, that they have a len() of 2,
-                # because otherwise, they are just something else
-                if unicode(n.names[0]) == self_name and len(n.names) == 2:
-                    add_self_dot_name(n)
-
-        if not isinstance(self.base, compiled.CompiledObject):
-            for s in self.base.get_super_classes():
-                for inst in self._evaluator.execute(s):
-                    names += inst.get_self_attributes()
-        return names
-
-    def get_subscope_by_name(self, name):
-        sub = self.base.get_subscope_by_name(name)
-        return InstanceElement(self._evaluator, self, sub, True)
-
-    def execute_subscope_by_name(self, name, args=()):
-        method = self.get_subscope_by_name(name)
-        return self._evaluator.execute(method, args)
-
-    def get_descriptor_return(self, obj):
-        """ Throws a KeyError if there's no method. """
-        # Arguments in __get__ descriptors are obj, class.
-        # `method` is the new parent of the array, don't know if that's good.
-        args = [obj, obj.base] if isinstance(obj, Instance) else [None, obj]
-        return self.execute_subscope_by_name('__get__', args)
 
-    def scope_names_generator(self, position=None):
-        """
-        An Instance has two scopes: The scope with self names and the class
-        scope. Instance variables have priority over the class scope.
-        """
-        yield self, self.get_self_attributes()
+class Generator(use_metaclass(CachedMetaClass, IterableWrapper, GeneratorMixin)):
+    """Handling of `yield` functions."""
+    def __init__(self, evaluator, func, var_args):
+        super(Generator, self).__init__()
+        self._evaluator = evaluator
+        self.func = func
+        self.var_args = var_args
 
-        names = []
-        for var in self.base.instance_names():
-            names.append(InstanceElement(self._evaluator, self, var, True))
-        yield self, names
+    def iter_content(self):
+        """ returns the content of __iter__ """
+        # Directly execute it, because with a normal call to py__call__ a
+        # Generator will be returned.
+        from jedi.evaluate.representation import FunctionExecution
+        f = FunctionExecution(self._evaluator, self.func, self.var_args)
+        return f.get_return_types(check_yields=True)
 
-    def is_callable(self):
-        try:
-            self.get_subscope_by_name('__call__')
-            return True
-        except KeyError:
-            return False
+    def __getattr__(self, name):
+        if name not in ['start_pos', 'end_pos', 'parent', 'get_imports',
+                        'doc', 'docstr', 'get_parent_until',
+                        'get_code', 'subscopes']:
+            raise AttributeError("Accessing %s of %s is not allowed."
+                                 % (self, name))
+        return getattr(self.func, name)
 
-    def get_index_types(self, index_array):
+    def __repr__(self):
+        return "<%s of %s>" % (type(self).__name__, self.func)
 
-        indexes = iterable.create_indexes_or_slices(self._evaluator, index_array)
-        if any([isinstance(i, iterable.Slice) for i in indexes]):
-            # Slice support in Jedi is very marginal, at the moment, so just
-            # ignore them in case of __getitem__.
-            # TODO support slices in a more general way.
-            indexes = []
 
-        index = helpers.FakeStatement(indexes, parent=compiled.builtin)
-        try:
-            return self.execute_subscope_by_name('__getitem__', [index])
-        except KeyError:
-            debug.warning('No __getitem__, cannot access the array.')
-            return []
+class GeneratorMethod(IterableWrapper):
+    """``__next__`` and ``send`` methods."""
+    def __init__(self, generator, builtin_func):
+        self._builtin_func = builtin_func
+        self._generator = generator
+
+    def py__call__(self, evaluator, params):
+        # TODO add TypeError if params are given.
+        return self._generator.iter_content()
 
     def __getattr__(self, name):
-        if name not in ['start_pos', 'end_pos', 'name', 'get_imports',
-                        'doc', 'raw_doc', 'asserts']:
-            raise AttributeError("Instance %s: Don't touch this (%s)!"
-                                 % (self, name))
-        return getattr(self.base, name)
+        return getattr(self._builtin_func, name)
 
-    def __repr__(self):
-        return "<e%s of %s (var_args: %s)>" % \
-            (type(self).__name__, self.base, len(self.var_args or []))
 
+class Comprehension(IterableWrapper):
+    @staticmethod
+    def from_atom(evaluator, atom):
+        mapping = {
+            '(': GeneratorComprehension,
+            '[': ListComprehension
+        }
+        return mapping[atom.children[0]](evaluator, atom)
 
-class InstanceElement(use_metaclass(CachedMetaClass, pr.Base)):
-    """
-    InstanceElement is a wrapper for any object, that is used as an instance
-    variable (e.g. self.variable or class methods).
-    """
-    def __init__(self, evaluator, instance, var, is_class_var=False):
+    def __init__(self, evaluator, atom):
         self._evaluator = evaluator
-        if isinstance(var, pr.Function):
-            var = Function(evaluator, var)
-        elif isinstance(var, pr.Class):
-            var = Class(evaluator, var)
-        self.instance = instance
-        self.var = var
-        self.is_class_var = is_class_var
+        self._atom = atom
 
-    @common.safe_property
     @memoize_default()
-    def parent(self):
-        par = self.var.parent
-        if isinstance(par, Class) and par == self.instance.base \
-                or isinstance(par, pr.Class) \
-                and par == self.instance.base.base:
-            par = self.instance
-        elif not isinstance(par, (pr.Module, compiled.CompiledObject)):
-            par = InstanceElement(self.instance._evaluator, self.instance, par, self.is_class_var)
-        return par
-
-    def get_parent_until(self, *args, **kwargs):
-        return pr.Simple.get_parent_until(self, *args, **kwargs)
-
-    def get_decorated_func(self):
-        """ Needed because the InstanceElement should not be stripped """
-        func = self.var.get_decorated_func()
-        func = InstanceElement(self._evaluator, self.instance, func)
-        return func
-
-    def expression_list(self):
-        # Copy and modify the array.
-        return [InstanceElement(self._evaluator, self.instance, command, self.is_class_var)
-                if not isinstance(command, (pr.Operator, Token)) else command
-                for command in self.var.expression_list()]
-
-    def __iter__(self):
-        for el in self.var.__iter__():
-            yield InstanceElement(self.instance._evaluator, self.instance, el,
-                                  self.is_class_var)
-
-    def __getitem__(self, index):
-        return InstanceElement(self._evaluator, self.instance, self.var[index],
-                               self.is_class_var)
+    def eval_node(self):
+        """
+        The first part `x + 1` of the list comprehension:
 
-    def __getattr__(self, name):
-        return getattr(self.var, name)
+            [x + 1 for x in foo]
+        """
+        comprehension = self._atom.children[1]
+        # For nested comprehensions we need to search the last one.
+        last = comprehension.children[-1]
+        last_comp = comprehension.children[1]
+        while True:
+            if isinstance(last, tree.CompFor):
+                last_comp = last
+            elif not tree.is_node(last, 'comp_if'):
+                break
+            last = last.children[-1]
 
-    def isinstance(self, *cls):
-        return isinstance(self.var, cls)
+        return helpers.deep_ast_copy(comprehension.children[0], parent=last_comp)
 
-    def is_callable(self):
-        return self.var.is_callable()
+    def get_exact_index_types(self, index):
+        return [self._evaluator.eval_element(self.eval_node())[index]]
 
     def __repr__(self):
-        return "<%s of %s>" % (type(self).__name__, self.var)
+        return "<e%s of %s>" % (type(self).__name__, self._atom)
 
 
-class Class(use_metaclass(CachedMetaClass, pr.IsScope)):
-    """
-    This class is not only important to extend `pr.Class`, it is also a
-    important for descriptors (if the descriptor methods are evaluated or not).
-    """
-    def __init__(self, evaluator, base):
-        self._evaluator = evaluator
-        self.base = base
+class ArrayMixin(object):
+    @memoize_default()
+    def names_dicts(self, search_global=False):  # Always False.
+        # `array.type` is a string with the type, e.g. 'list'.
+        scope = self._evaluator.find_types(compiled.builtin, self.type)[0]
+        # builtins only have one class -> [0]
+        scope = self._evaluator.execute(scope, (AlreadyEvaluated((self,)),))[0]
+        return scope.names_dicts(search_global)
 
-    @memoize_default(default=())
-    def get_super_classes(self):
-        supers = []
-        # TODO care for mro stuff (multiple super classes).
-        for s in self.base.supers:
-            # Super classes are statements.
-            for cls in self._evaluator.eval_statement(s):
-                if not isinstance(cls, (Class, compiled.CompiledObject)):
-                    debug.warning('Received non class as a super class.')
-                    continue  # Just ignore other stuff (user input error).
-                supers.append(cls)
-        if not supers and self.base.parent != compiled.builtin:
-            # add `object` to classes
-            supers += self._evaluator.find_types(compiled.builtin, 'object')
-        return supers
-
-    @memoize_default(default=())
-    def instance_names(self):
-        def in_iterable(name, iterable):
-            """ checks if the name is in the variable 'iterable'. """
-            for i in iterable:
-                # Only the last name is important, because these names have a
-                # maximal length of 2, with the first one being `self`.
-                if unicode(i.names[-1]) == unicode(name.names[-1]):
-                    return True
-            return False
-
-        result = self.base.get_defined_names()
-        super_result = []
-        # TODO mro!
-        for cls in self.get_super_classes():
-            # Get the inherited names.
-            for i in cls.instance_names():
-                if not in_iterable(i, result):
-                    super_result.append(i)
-        result += super_result
-        return result
+    def py__bool__(self):
+        return None  # We don't know the length, because of appends.
 
-    def scope_names_generator(self, position=None):
-        yield self, self.instance_names()
-        yield self, compiled.type_names
-
-    def get_subscope_by_name(self, name):
-        for s in [self] + self.get_super_classes():
-            for sub in reversed(s.subscopes):
-                if sub.name.get_code() == name:
-                    return sub
-        raise KeyError("Couldn't find subscope.")
 
-    def is_callable(self):
-        return True
+class ListComprehension(Comprehension, ArrayMixin):
+    type = 'list'
 
-    @common.safe_property
+    def get_index_types(self, evaluator, index):
+        return self.iter_content()
+
+    def iter_content(self):
+        return self._evaluator.eval_element(self.eval_node())
+
+    @property
     def name(self):
-        return self.base.name
+        return FakeSequence(self._evaluator, [], 'list').name
 
-    def __getattr__(self, name):
-        if name not in ['start_pos', 'end_pos', 'parent', 'asserts', 'raw_doc',
-                        'doc', 'get_imports', 'get_parent_until', 'get_code',
-                        'subscopes']:
-            raise AttributeError("Don't touch this: %s of %s !" % (name, self))
-        return getattr(self.base, name)
 
-    def __repr__(self):
-        return "<e%s of %s>" % (type(self).__name__, self.base)
+class GeneratorComprehension(Comprehension, GeneratorMixin):
+    def iter_content(self):
+        return self._evaluator.eval_element(self.eval_node())
 
 
-class Function(use_metaclass(CachedMetaClass, pr.IsScope)):
-    """
-    Needed because of decorators. Decorators are evaluated here.
-    """
-    def __init__(self, evaluator, func, is_decorated=False):
-        """ This should not be called directly """
+class Array(IterableWrapper, ArrayMixin):
+    mapping = {'(': 'tuple',
+               '[': 'list',
+               '{': 'dict'}
+
+    def __init__(self, evaluator, atom):
         self._evaluator = evaluator
-        self.base_func = func
-        self.is_decorated = is_decorated
+        self.atom = atom
+        self.type = Array.mapping[atom.children[0]]
+        """The builtin name of the array (list, set, tuple or dict)."""
+
+        c = self.atom.children
+        array_node = c[1]
+        if self.type == 'dict' and array_node != '}' \
+                and (not hasattr(array_node, 'children')
+                     or ':' not in array_node.children):
+            self.type = 'set'
+
+    @property
+    def name(self):
+        return helpers.FakeName(self.type, parent=self)
 
     @memoize_default()
-    def _decorated_func(self):
+    def get_index_types(self, evaluator, index=()):
         """
-        Returns the function, that is to be executed in the end.
-        This is also the places where the decorators are processed.
+        Get the types of a specific index or all, if not given.
+
+        :param index: A subscriptlist node (or subnode).
         """
-        f = self.base_func
+        indexes = create_indexes_or_slices(evaluator, index)
+        lookup_done = False
+        types = []
+        for index in indexes:
+            if isinstance(index, Slice):
+                types += [self]
+                lookup_done = True
+            elif isinstance(index, compiled.CompiledObject) \
+                    and isinstance(index.obj, (int, str, unicode)):
+                with common.ignored(KeyError, IndexError, TypeError):
+                    types += self.get_exact_index_types(index.obj)
+                    lookup_done = True
 
-        # Only enter it, if has not already been processed.
-        if not self.is_decorated:
-            for dec in reversed(self.base_func.decorators):
-                debug.dbg('decorator: %s %s', dec, f)
-                dec_results = self._evaluator.eval_statement(dec)
-                if not len(dec_results):
-                    debug.warning('decorator not found: %s on %s', dec, self.base_func)
-                    return None
-                decorator = dec_results.pop()
-                if dec_results:
-                    debug.warning('multiple decorators found %s %s',
-                                  self.base_func, dec_results)
-                # Create param array.
-                old_func = Function(self._evaluator, f, is_decorated=True)
-
-                wrappers = self._evaluator.execute(decorator, (old_func,))
-                if not len(wrappers):
-                    debug.warning('no wrappers found %s', self.base_func)
-                    return None
-                if len(wrappers) > 1:
-                    # TODO resolve issue with multiple wrappers -> multiple types
-                    debug.warning('multiple wrappers found %s %s',
-                                  self.base_func, wrappers)
-                f = wrappers[0]
-
-                debug.dbg('decorator end %s', f)
-
-        if isinstance(f, pr.Function):
-            f = Function(self._evaluator, f, True)
-        return f
+        return types if lookup_done else self.values()
 
-    def get_decorated_func(self):
-        """
-        This function exists for the sole purpose of returning itself if the
-        decorator doesn't turn out to "work".
+    @memoize_default()
+    def values(self):
+        result = unite(self._evaluator.eval_element(v) for v in self._values())
+        result += check_array_additions(self._evaluator, self)
+        return result
 
-        We just ignore the decorator here, because sometimes decorators are
-        just really complicated and Jedi cannot understand them.
-        """
-        return self._decorated_func() \
-            or Function(self._evaluator, self.base_func, True)
+    def get_exact_index_types(self, mixed_index):
+        """ Here the index is an int/str. Raises IndexError/KeyError """
+        if self.type == 'dict':
+            for key, values in self._items():
+                # Because we only want the key to be a string.
+                keys = self._evaluator.eval_element(key)
+
+                for k in keys:
+                    if isinstance(k, compiled.CompiledObject) \
+                            and mixed_index == k.obj:
+                        for value in values:
+                            return self._evaluator.eval_element(value)
+            raise KeyError('No key found in dictionary %s.' % self)
 
-    def get_magic_function_names(self):
-        return compiled.magic_function_class.get_defined_names()
+        # Can raise an IndexError
+        return self._evaluator.eval_element(self._items()[mixed_index])
 
-    def get_magic_function_scope(self):
-        return compiled.magic_function_class
+    def iter_content(self):
+        return self.values()
 
-    def is_callable(self):
-        return True
+    @common.safe_property
+    def parent(self):
+        return compiled.builtin
+
+    def get_parent_until(self):
+        return compiled.builtin
 
     def __getattr__(self, name):
-        return getattr(self.base_func, name)
+        if name not in ['start_pos', 'get_only_subelement', 'parent',
+                        'get_parent_until', 'items']:
+            raise AttributeError('Strange access on %s: %s.' % (self, name))
+        return getattr(self.atom, name)
+
+    def _values(self):
+        """Returns a list of a list of node."""
+        if self.type == 'dict':
+            return list(chain.from_iterable(v for k, v in self._items()))
+        else:
+            return self._items()
+
+    def _items(self):
+        c = self.atom.children
+        array_node = c[1]
+        if array_node in (']', '}', ')'):
+            return []  # Direct closing bracket, doesn't contain items.
+
+        if tree.is_node(array_node, 'testlist_comp'):
+            return array_node.children[::2]
+        elif tree.is_node(array_node, 'dictorsetmaker'):
+            kv = []
+            iterator = iter(array_node.children)
+            for key in iterator:
+                op = next(iterator, None)
+                if op is None or op == ',':
+                    kv.append(key)  # A set.
+                elif op == ':':  # A dict.
+                    kv.append((key, [next(iterator)]))
+                    next(iterator, None)  # Possible comma.
+                else:
+                    raise NotImplementedError('dict/set comprehensions')
+            return kv
+        else:
+            return [array_node]
+
+    def __iter__(self):
+        return iter(self._items())
 
     def __repr__(self):
-        dec_func = self._decorated_func()
-        dec = ''
-        if not self.is_decorated and self.base_func.decorators:
-            dec = " is " + repr(dec_func)
-        return "<e%s of %s%s>" % (type(self).__name__, self.base_func, dec)
+        return "<%s of %s>" % (type(self).__name__, self.atom)
 
 
-class FunctionExecution(Executable):
-    """
-    This class is used to evaluate functions and their returns.
+class _FakeArray(Array):
+    def __init__(self, evaluator, container, type):
+        self.type = type
+        self._evaluator = evaluator
+        self.atom = container
 
-    This is the most complicated class, because it contains the logic to
-    transfer parameters. It is even more complicated, because there may be
-    multiple calls to functions and recursion has to be avoided. But this is
-    responsibility of the decorators.
-    """
-    @memoize_default(default=())
-    @recursion.execution_recursion_decorator
-    def get_return_types(self, evaluate_generator=False):
-        func = self.base
-        # Feed the listeners, with the params.
-        for listener in func.listeners:
-            listener.execute(self._get_params())
-        if func.listeners:
-            # If we do have listeners, that means that there's not a regular
-            # execution ongoing. In this case Jedi is interested in the
-            # inserted params, not in the actual execution of the function.
-            return []
 
-        if func.is_generator and not evaluate_generator:
-            return [iterable.Generator(self._evaluator, func, self.var_args)]
-        else:
-            stmts = list(docstrings.find_return_types(self._evaluator, func))
-            for r in self.returns:
-                if r is not None:
-                    stmts += self._evaluator.eval_statement(r)
-            return stmts
+class ImplicitTuple(_FakeArray):
+    def __init__(self, evaluator, testlist):
+        super(ImplicitTuple, self).__init__(evaluator, testlist, 'tuple')
+        self._testlist = testlist
 
-    @memoize_default(default=())
-    def _get_params(self):
-        """
-        This returns the params for an TODO and is injected as a
-        'hack' into the pr.Function class.
-        This needs to be here, because Instance can have __init__ functions,
-        which act the same way as normal functions.
-        """
-        return param.get_params(self._evaluator, self.base, self.var_args)
+    def _items(self):
+        return self._testlist.children[::2]
 
-    def get_defined_names(self):
-        """
-        Call the default method with the own instance (self implements all
-        the necessary functions). Add also the params.
-        """
-        return self._get_params() + pr.Scope.get_defined_names(self)
 
-    def scope_names_generator(self, position=None):
-        names = pr.filter_after_position(pr.Scope.get_defined_names(self), position)
-        yield self, self._get_params() + names
+class FakeSequence(_FakeArray):
+    def __init__(self, evaluator, sequence_values, type):
+        super(FakeSequence, self).__init__(evaluator, sequence_values, type)
+        self._sequence_values = sequence_values
 
-    def _copy_properties(self, prop):
-        """
-        Literally copies a property of a Function. Copying is very expensive,
-        because it is something like `copy.deepcopy`. However, these copied
-        objects can be used for the executions, as if they were in the
-        execution.
-        """
-        # Copy all these lists into this local function.
-        attr = getattr(self.base, prop)
-        objects = []
-        for element in attr:
-            if element is None:
-                copied = element
-            else:
-                copied = helpers.fast_parent_copy(element)
-                copied.parent = self._scope_copy(copied.parent)
-                if isinstance(copied, pr.Function):
-                    copied = Function(self._evaluator, copied)
-            objects.append(copied)
-        return objects
+    def _items(self):
+        return self._sequence_values
 
-    def __getattr__(self, name):
-        if name not in ['start_pos', 'end_pos', 'imports', '_sub_module']:
-            raise AttributeError('Tried to access %s: %s. Why?' % (name, self))
-        return getattr(self.base, name)
+    def get_exact_index_types(self, index):
+        value = self._sequence_values[index]
+        return self._evaluator.eval_element(value)
 
-    @memoize_default()
-    def _scope_copy(self, scope):
-        """ Copies a scope (e.g. if) in an execution """
-        # TODO method uses different scopes than the subscopes property.
-
-        # just check the start_pos, sometimes it's difficult with closures
-        # to compare the scopes directly.
-        if scope.start_pos == self.start_pos:
-            return self
-        else:
-            copied = helpers.fast_parent_copy(scope)
-            copied.parent = self._scope_copy(copied.parent)
-            return copied
 
-    @common.safe_property
-    @memoize_default([])
-    def returns(self):
-        return self._copy_properties('returns')
+class AlreadyEvaluated(frozenset):
+    """A simple container to add already evaluated objects to an array."""
+    def get_code(self):
+        # For debugging purposes.
+        return str(self)
 
-    @common.safe_property
-    @memoize_default([])
-    def asserts(self):
-        return self._copy_properties('asserts')
 
-    @common.safe_property
-    @memoize_default([])
-    def statements(self):
-        return self._copy_properties('statements')
+class MergedNodes(frozenset):
+    pass
 
-    @common.safe_property
-    @memoize_default([])
-    def subscopes(self):
-        return self._copy_properties('subscopes')
 
-    def get_statement_for_position(self, pos):
-        return pr.Scope.get_statement_for_position(self, pos)
+class FakeDict(_FakeArray):
+    def __init__(self, evaluator, dct):
+        super(FakeDict, self).__init__(evaluator, dct, 'dict')
+        self._dct = dct
 
-    def __repr__(self):
-        return "<%s of %s>" % (type(self).__name__, self.base)
+    def get_exact_index_types(self, index):
+        return list(chain.from_iterable(self._evaluator.eval_element(v)
+                                        for v in self._dct[index]))
+
+    def _items(self):
+        return self._dct.items()
+
+
+class MergedArray(_FakeArray):
+    def __init__(self, evaluator, arrays):
+        super(MergedArray, self).__init__(evaluator, arrays, arrays[-1].type)
+        self._arrays = arrays
+
+    def get_exact_index_types(self, mixed_index):
+        raise IndexError
 
+    def values(self):
+        return list(chain(*(a.values() for a in self._arrays)))
 
-class ModuleWrapper(use_metaclass(CachedMetaClass, pr.Module)):
-    def __init__(self, evaluator, module):
+    def __iter__(self):
+        for array in self._arrays:
+            for a in array:
+                yield a
+
+    def __len__(self):
+        return sum(len(a) for a in self._arrays)
+
+
+def get_iterator_types(inputs):
+    """Returns the types of any iterator (arrays, yields, __iter__, etc)."""
+    iterators = []
+    # Take the first statement (for has always only
+    # one, remember `in`). And follow it.
+    for it in inputs:
+        if isinstance(it, (Generator, Array, ArrayInstance, Comprehension)):
+            iterators.append(it)
+        else:
+            if not hasattr(it, 'execute_subscope_by_name'):
+                debug.warning('iterator/for loop input wrong: %s', it)
+                continue
+            try:
+                iterators += it.execute_subscope_by_name('__iter__')
+            except KeyError:
+                debug.warning('iterators: No __iter__ method found.')
+
+    result = []
+    from jedi.evaluate.representation import Instance
+    for it in iterators:
+        if isinstance(it, Array):
+            # Array is a little bit special, since this is an internal array,
+            # but there's also the list builtin, which is another thing.
+            result += it.values()
+        elif isinstance(it, Instance):
+            # __iter__ returned an instance.
+            name = '__next__' if is_py3 else 'next'
+            try:
+                result += it.execute_subscope_by_name(name)
+            except KeyError:
+                debug.warning('Instance has no __next__ function in %s.', it)
+        else:
+            # TODO this is not correct, __iter__ can return arbitrary input!
+            # Is a generator.
+            result += it.iter_content()
+    return result
+
+
+def check_array_additions(evaluator, array):
+    """ Just a mapper function for the internal _check_array_additions """
+    if array.type not in ('list', 'set'):
+        # TODO also check for dict updates
+        return []
+
+    is_list = array.type == 'list'
+    try:
+        current_module = array.atom.get_parent_until()
+    except AttributeError:
+        # If there's no get_parent_until, it's a FakeSequence or another Fake
+        # type. Those fake types are used inside Jedi's engine. No values may
+        # be added to those after their creation.
+        return []
+    return _check_array_additions(evaluator, array, current_module, is_list)
+
+
+@memoize_default([], evaluator_is_first_arg=True)
+def _check_array_additions(evaluator, compare_array, module, is_list):
+    """
+    Checks if a `Array` has "add" (append, insert, extend) statements:
+
+    >>> a = [""]
+    >>> a.append(1)
+    """
+    if not settings.dynamic_array_additions or isinstance(module, compiled.CompiledObject):
+        return []
+
+    def check_additions(arglist, add_name):
+        params = list(param.Arguments(evaluator, arglist).unpack())
+        result = []
+        if add_name in ['insert']:
+            params = params[1:]
+        if add_name in ['append', 'add', 'insert']:
+            for key, nodes in params:
+                result += unite(evaluator.eval_element(node) for node in nodes)
+        elif add_name in ['extend', 'update']:
+            for key, nodes in params:
+                iterators = unite(evaluator.eval_element(node) for node in nodes)
+                result += get_iterator_types(iterators)
+        return result
+
+    from jedi.evaluate import representation as er, param
+
+    def get_execution_parent(element):
+        """ Used to get an Instance/FunctionExecution parent """
+        if isinstance(element, Array):
+            node = element.atom
+        else:
+            # Is an Instance with an
+            # Arguments([AlreadyEvaluated([ArrayInstance])]) inside
+            # Yeah... I know... It's complicated ;-)
+            node = list(element.var_args.argument_node[0])[0].var_args.trailer
+        if isinstance(node, er.InstanceElement):
+            return node
+        return node.get_parent_until(er.FunctionExecution)
+
+    temp_param_add, settings.dynamic_params_for_other_modules = \
+        settings.dynamic_params_for_other_modules, False
+
+    search_names = ['append', 'extend', 'insert'] if is_list else ['add', 'update']
+    comp_arr_parent = get_execution_parent(compare_array)
+
+    added_types = []
+    for add_name in search_names:
+        try:
+            possible_names = module.used_names[add_name]
+        except KeyError:
+            continue
+        else:
+            for name in possible_names:
+                # Check if the original scope is an execution. If it is, one
+                # can search for the same statement, that is in the module
+                # dict. Executions are somewhat special in jedi, since they
+                # literally copy the contents of a function.
+                if isinstance(comp_arr_parent, er.FunctionExecution):
+                    if comp_arr_parent.start_pos < name.start_pos < comp_arr_parent.end_pos:
+                        name = comp_arr_parent.name_for_position(name.start_pos)
+                    else:
+                        # Don't check definitions that are not defined in the
+                        # same function. This is not "proper" anyway. It also
+                        # improves Jedi's speed for array lookups, since we
+                        # don't have to check the whole source tree anymore.
+                        continue
+                trailer = name.parent
+                power = trailer.parent
+                trailer_pos = power.children.index(trailer)
+                try:
+                    execution_trailer = power.children[trailer_pos + 1]
+                except IndexError:
+                    continue
+                else:
+                    if execution_trailer.type != 'trailer' \
+                            or execution_trailer.children[0] != '(' \
+                            or execution_trailer.children[1] == ')':
+                        continue
+                power = helpers.call_of_name(name, cut_own_trailer=True)
+                # InstanceElements are special, because they don't get copied,
+                # but have this wrapper around them.
+                if isinstance(comp_arr_parent, er.InstanceElement):
+                    power = er.get_instance_el(evaluator, comp_arr_parent.instance, power)
+
+                if evaluator.recursion_detector.push_stmt(power):
+                    # Check for recursion. Possible by using 'extend' in
+                    # combination with function calls.
+                    continue
+                if compare_array in evaluator.eval_element(power):
+                    # The arrays match. Now add the results
+                    added_types += check_additions(execution_trailer.children[1], add_name)
+
+                evaluator.recursion_detector.pop_stmt()
+    # reset settings
+    settings.dynamic_params_for_other_modules = temp_param_add
+    return added_types
+
+
+def check_array_instances(evaluator, instance):
+    """Used for set() and list() instances."""
+    if not settings.dynamic_array_additions:
+        return instance.var_args
+
+    ai = ArrayInstance(evaluator, instance)
+    from jedi.evaluate import param
+    return param.Arguments(evaluator, [AlreadyEvaluated([ai])])
+
+
+class ArrayInstance(IterableWrapper):
+    """
+    Used for the usage of set() and list().
+    This is definitely a hack, but a good one :-)
+    It makes it possible to use set/list conversions.
+
+    In contrast to Array, ListComprehension and all other iterable types, this
+    is something that is only used inside `evaluate/compiled/fake/builtins.py`
+    and therefore doesn't need `names_dicts`, `py__bool__` and so on, because
+    we don't use these operations in `builtins.py`.
+    """
+    def __init__(self, evaluator, instance):
         self._evaluator = evaluator
-        self._module = module
+        self.instance = instance
+        self.var_args = instance.var_args
 
-    def scope_names_generator(self, position=None):
-        yield self, pr.filter_after_position(self._module.get_defined_names(), position)
-        yield self, self._module_attributes()
-        sub_modules = self._sub_modules()
-        if sub_modules:
-            yield self, self._sub_modules()
+    def iter_content(self):
+        """
+        The index is here just ignored, because of all the appends, etc.
+        lists/sets are too complicated too handle that.
+        """
+        items = []
+        for key, nodes in self.var_args.unpack():
+            for node in nodes:
+                for typ in self._evaluator.eval_element(node):
+                    items += get_iterator_types([typ])
 
-    @memoize_default()
-    def _module_attributes(self):
-        names = ['__file__', '__package__', '__doc__', '__name__', '__version__']
-        # All the additional module attributes are strings.
-        parent = Instance(self._evaluator, compiled.create(self._evaluator, str))
-        return [helpers.FakeName(n, parent) for n in names]
+        module = self.var_args.get_parent_until()
+        is_list = str(self.instance.name) == 'list'
+        items += _check_array_additions(self._evaluator, self.instance, module, is_list)
+        return items
 
-    @memoize_default()
-    def _sub_modules(self):
+
+class Slice(object):
+    def __init__(self, evaluator, start, stop, step):
+        self._evaluator = evaluator
+        # all of them are either a Precedence or None.
+        self._start = start
+        self._stop = stop
+        self._step = step
+
+    @property
+    def obj(self):
         """
-        Lists modules in the directory of this module (if this module is a
-        package).
+        Imitate CompiledObject.obj behavior and return a ``builtin.slice()``
+        object.
         """
-        path = self._module.path
-        names = []
-        if path is not None and path.endswith(os.path.sep + '__init__.py'):
-            mods = pkgutil.iter_modules([os.path.dirname(path)])
-            for module_loader, name, is_pkg in mods:
-                name = helpers.FakeName(name)
-                # It's obviously a relative import to the current module.
-                imp = helpers.FakeImport(name, self, level=1)
-                name.parent = imp
-                names.append(name)
-        return names
+        def get(element):
+            if element is None:
+                return None
 
-    def __getattr__(self, name):
-        return getattr(self._module, name)
+            result = self._evaluator.eval_element(element)
+            if len(result) != 1:
+                # We want slices to be clear defined with just one type.
+                # Otherwise we will return an empty slice object.
+                raise IndexError
+            try:
+                return result[0].obj
+            except AttributeError:
+                return None
 
-    def __repr__(self):
-        return "<%s: %s>" % (type(self).__name__, self._module)
+        try:
+            return slice(get(self._start), get(self._stop), get(self._step))
+        except IndexError:
+            return slice(None, None, None)
+
+
+def create_indexes_or_slices(evaluator, index):
+    if tree.is_node(index, 'subscript'):  # subscript is a slice operation.
+        start, stop, step = None, None, None
+        result = []
+        for el in index.children:
+            if el == ':':
+                if not result:
+                    result.append(None)
+            elif tree.is_node(el, 'sliceop'):
+                if len(el.children) == 2:
+                    result.append(el.children[1])
+            else:
+                result.append(el)
+        result += [None] * (3 - len(result))
+
+        return (Slice(evaluator, *result),)
+    return evaluator.eval_element(index)
```

### Comparing `jedi-0.8.1-final0/jedi/evaluate/compiled/__init__.py` & `jedi-0.9.0/jedi/evaluate/compiled/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,122 +1,178 @@
 """
 Imitate the parser representation.
 """
 import inspect
 import re
 import sys
 import os
+from functools import partial
 
 from jedi._compatibility import builtins as _builtins, unicode
 from jedi import debug
-from jedi.cache import underscore_memoization, memoize
+from jedi.cache import underscore_memoization, memoize_method
 from jedi.evaluate.sys_path import get_sys_path
-from jedi.parser.representation import Param, SubModule, Base, IsScope, Operator
+from jedi.parser.tree import Param, Base, Operator, zero_position_modifier
 from jedi.evaluate.helpers import FakeName
 from . import fake
 
 
 _sep = os.path.sep
 if os.path.altsep is not None:
     _sep += os.path.altsep
 _path_re = re.compile('(?:\.[^{0}]+|[{0}]__init__\.py)$'.format(re.escape(_sep)))
 del _sep
 
 
+class CheckAttribute(object):
+    """Raises an AttributeError if the attribute X isn't available."""
+    def __init__(self, func):
+        self.func = func
+        # Remove the py in front of e.g. py__call__.
+        self.check_name = func.__name__[2:]
+
+    def __get__(self, instance, owner):
+        # This might raise an AttributeError. That's wanted.
+        getattr(instance.obj, self.check_name)
+        return partial(self.func, instance)
+
+
 class CompiledObject(Base):
     # comply with the parser
     start_pos = 0, 0
-    asserts = []
     path = None  # modules have this attribute - set it to None.
+    used_names = {}  # To be consistent with modules.
 
     def __init__(self, obj, parent=None):
         self.obj = obj
         self.parent = parent
 
     @property
+    def py__call__(self):
+        def actual(evaluator, params):
+            if inspect.isclass(self.obj):
+                from jedi.evaluate.representation import Instance
+                return [Instance(evaluator, self, params)]
+            else:
+                return list(self._execute_function(evaluator, params))
+
+        # Might raise an AttributeError, which is intentional.
+        self.obj.__call__
+        return actual
+
+    @CheckAttribute
+    def py__class__(self, evaluator):
+        return CompiledObject(self.obj.__class__, parent=self.parent)
+
+    @CheckAttribute
+    def py__mro__(self, evaluator):
+        return tuple(create(evaluator, cls, self.parent) for cls in self.obj.__mro__)
+
+    @CheckAttribute
+    def py__bases__(self, evaluator):
+        return tuple(create(evaluator, cls) for cls in self.obj.__bases__)
+
+    def py__bool__(self):
+        return bool(self.obj)
+
+    def py__file__(self):
+        return self.obj.__file__
+
+    def is_class(self):
+        return inspect.isclass(self.obj)
+
+    @property
     def doc(self):
         return inspect.getdoc(self.obj) or ''
 
     @property
     def params(self):
         params_str, ret = self._parse_function_doc()
         tokens = params_str.split(',')
+        if inspect.ismethoddescriptor(self._cls().obj):
+            tokens.insert(0, 'self')
         params = []
-        module = SubModule(self.get_parent_until().name)
-        # it seems like start_pos/end_pos is always (0, 0) for a compiled
-        # object
-        start_pos, end_pos = (0, 0), (0, 0)
         for p in tokens:
             parts = [FakeName(part) for part in p.strip().split('=')]
-            if len(parts) >= 2:
-                parts.insert(1, Operator(module, '=', module, (0, 0)))
-            params.append(Param(module, parts, start_pos,
-                                end_pos, builtin))
+            if len(parts) > 1:
+                parts.insert(1, Operator(zero_position_modifier, '=', (0, 0)))
+            params.append(Param(parts, self))
         return params
 
     def __repr__(self):
         return '<%s: %s>' % (type(self).__name__, repr(self.obj))
 
     @underscore_memoization
     def _parse_function_doc(self):
         if self.doc is None:
             return '', ''
 
         return _parse_function_doc(self.doc)
 
-    def type(self):
+    def api_type(self):
+        if fake.is_class_instance(self.obj):
+            return 'instance'
+
         cls = self._cls().obj
         if inspect.isclass(cls):
             return 'class'
         elif inspect.ismodule(cls):
             return 'module'
         elif inspect.isbuiltin(cls) or inspect.ismethod(cls) \
                 or inspect.ismethoddescriptor(cls):
             return 'function'
 
-    def is_executable_class(self):
-        return inspect.isclass(self.obj)
+    @property
+    def type(self):
+        """Imitate the tree.Node.type values."""
+        cls = self._cls().obj
+        if inspect.isclass(cls):
+            return 'classdef'
+        elif inspect.ismodule(cls):
+            return 'file_input'
+        elif inspect.isbuiltin(cls) or inspect.ismethod(cls) \
+                or inspect.ismethoddescriptor(cls):
+            return 'funcdef'
 
     @underscore_memoization
     def _cls(self):
         # Ensures that a CompiledObject is returned that is not an instance (like list)
         if fake.is_class_instance(self.obj):
             try:
                 c = self.obj.__class__
             except AttributeError:
                 # happens with numpy.core.umath._UFUNC_API (you get it
                 # automatically by doing `import numpy`.
                 c = type(None)
             return CompiledObject(c, self.parent)
         return self
 
-    def get_defined_names(self):
-        if inspect.ismodule(self.obj):
-            return self.instance_names()
-        else:
-            return type_names + self.instance_names()
+    @property
+    def names_dict(self):
+        # For compatibility with `representation.Class`.
+        return self.names_dicts(False)[0]
 
-    def scope_names_generator(self, position=None):
-        yield self, self.get_defined_names()
+    def names_dicts(self, search_global, is_instance=False):
+        return self._names_dict_ensure_one_dict(is_instance)
 
-    @underscore_memoization
-    def instance_names(self):
-        names = []
-        cls = self._cls()
-        for name in dir(cls.obj):
-            names.append(CompiledName(cls, name))
-        return names
+    @memoize_method
+    def _names_dict_ensure_one_dict(self, is_instance):
+        """
+        search_global shouldn't change the fact that there's one dict, this way
+        there's only one `object`.
+        """
+        return [LazyNamesDict(self._cls(), is_instance)]
 
     def get_subscope_by_name(self, name):
         if name in dir(self._cls().obj):
             return CompiledName(self._cls(), name).parent
         else:
             raise KeyError("CompiledObject doesn't have an attribute '%s'." % name)
 
-    def get_index_types(self, evaluator, index_array):
+    def get_index_types(self, evaluator, index_array=()):
         # If the object doesn't have `__getitem__`, just raise the
         # AttributeError.
         if not hasattr(self.obj, '__getitem__'):
             debug.warning('Tried to call __getitem__ on non-iterable.')
             return []
         if type(self.obj) not in (str, list, tuple, unicode, bytes, bytearray, dict):
             # Get rid of side effects, we won't call custom `__getitem__`s.
@@ -142,33 +198,31 @@
             except TypeError:
                 pass  # self.obj maynot have an __iter__ method.
         return result
 
     @property
     def name(self):
         # might not exist sometimes (raises AttributeError)
-        return self._cls().obj.__name__
+        return FakeName(self._cls().obj.__name__, self)
 
-    def execute_function(self, evaluator, params):
-        if self.type() != 'function':
+    def _execute_function(self, evaluator, params):
+        if self.type != 'funcdef':
             return
 
         for name in self._parse_function_doc()[1].split():
             try:
                 bltn_obj = _create_from_name(builtin, builtin, name)
             except AttributeError:
                 continue
             else:
-                if isinstance(bltn_obj, CompiledObject):
+                if isinstance(bltn_obj, CompiledObject) and bltn_obj.obj is None:
                     # We want everything except None.
-                    if bltn_obj.obj is not None:
-                        yield bltn_obj
-                else:
-                    for result in evaluator.execute(bltn_obj, params):
-                        yield result
+                    continue
+                for result in evaluator.execute(bltn_obj, params):
+                    yield result
 
     @property
     @underscore_memoization
     def subscopes(self):
         """
         Returns only the faked scopes - the other ones are not important for
         internal analysis.
@@ -187,33 +241,67 @@
 
     def get_self_attributes(self):
         return []  # Instance compatibility
 
     def get_imports(self):
         return []  # Builtins don't have imports
 
-    def is_callable(self):
-        """Check if the object has a ``__call__`` method."""
-        return hasattr(self.obj, '__call__')
+
+class LazyNamesDict(object):
+    """
+    A names_dict instance for compiled objects, resembles the parser.tree.
+    """
+    def __init__(self, compiled_obj, is_instance):
+        self._compiled_obj = compiled_obj
+        self._is_instance = is_instance
+
+    def __iter__(self):
+        return (v[0].value for v in self.values())
+
+    @memoize_method
+    def __getitem__(self, name):
+        try:
+            getattr(self._compiled_obj.obj, name)
+        except AttributeError:
+            raise KeyError('%s in %s not found.' % (name, self._compiled_obj))
+        return [CompiledName(self._compiled_obj, name)]
+
+    def values(self):
+        obj = self._compiled_obj.obj
+
+        values = []
+        for name in dir(obj):
+            try:
+                values.append(self[name])
+            except KeyError:
+                # The dir function can be wrong.
+                pass
+
+        # dir doesn't include the type names.
+        if not inspect.ismodule(obj) and obj != type and not self._is_instance:
+            values += _type_names_dict.values()
+        return values
 
 
 class CompiledName(FakeName):
     def __init__(self, obj, name):
         super(CompiledName, self).__init__(name)
         self._obj = obj
         self.name = name
-        self.start_pos = 0, 0  # an illegal start_pos, to make sorting easy.
 
     def __repr__(self):
         try:
             name = self._obj.name  # __name__ is not defined all the time
         except AttributeError:
             name = None
         return '<%s: (%s).%s>' % (type(self).__name__, name, self.name)
 
+    def is_definition(self):
+        return True
+
     @property
     @underscore_memoization
     def parent(self):
         module = self._obj.get_parent_until()
         return _create_from_name(module, self._obj, self.name)
 
     @parent.setter
@@ -226,74 +314,69 @@
     Changes `/usr/lib/python3.4/email/utils.py` to `email.utils`.  I.e.
     compares the path with sys.path and then returns the dotted_path. If the
     path is not in the sys.path, just returns None.
     """
     if sys_path is None:
         sys_path = get_sys_path()
 
+    if os.path.basename(fs_path).startswith('__init__.'):
+        # We are calculating the path. __init__ files are not interesting.
+        fs_path = os.path.dirname(fs_path)
+
     # prefer
     #   - UNIX
     #     /path/to/pythonX.Y/lib-dynload
     #     /path/to/pythonX.Y/site-packages
     #   - Windows
     #     C:\path\to\DLLs
     #     C:\path\to\Lib\site-packages
     # over
     #   - UNIX
     #     /path/to/pythonX.Y
     #   - Windows
     #     C:\path\to\Lib
     path = ''
     for s in sys_path:
-        if (fs_path.startswith(s) and
-            len(path) < len(s)):
+        if (fs_path.startswith(s) and len(path) < len(s)):
             path = s
     return _path_re.sub('', fs_path[len(path):].lstrip(os.path.sep)).replace(os.path.sep, '.')
 
 
-def load_module(path, name):
-    """
-    if not name:
-        name = os.path.basename(path)
-        name = name.rpartition('.')[0]  # cut file type (normally .so)
-
-    # sometimes there are endings like `_sqlite3.cpython-32mu`
-    name = re.sub(r'\..*', '', name)
-
-    dot_path = []
-    if path:
-        p = path
-        # if path is not in sys.path, we need to make a well defined import
-        # like `from numpy.core import umath.`
-        while p and p not in sys.path:
-            p, sep, mod = p.rpartition(os.path.sep)
-            dot_path.insert(0, mod.partition('.')[0])
-        if p:
-            name = ".".join(dot_path)
-            path = p
-        else:
-            path = os.path.dirname(path)
-
-    """
+def load_module(path=None, name=None):
     if path is not None:
         dotted_path = dotted_from_fs_path(path)
     else:
         dotted_path = name
 
     sys_path = get_sys_path()
     if dotted_path is None:
         p, _, dotted_path = path.partition(os.path.sep)
         sys_path.insert(0, p)
 
     temp, sys.path = sys.path, sys_path
-    __import__(dotted_path)
+    try:
+        __import__(dotted_path)
+    except RuntimeError:
+        if 'PySide' in dotted_path or 'PyQt' in dotted_path:
+            # RuntimeError: the PyQt4.QtCore and PyQt5.QtCore modules both wrap
+            # the QObject class.
+            # See https://github.com/davidhalter/jedi/pull/483
+            return None
+        raise
+    except ImportError:
+        # If a module is "corrupt" or not really a Python module or whatever.
+        debug.warning('Module %s not importable.', path)
+        return None
+    finally:
+        sys.path = temp
+
     # Just access the cache after import, because of #59 as well as the very
     # complicated import structure of Python.
     module = sys.modules[dotted_path]
-    sys.path = temp
+
     return CompiledObject(module)
 
 
 docstr_defaults = {
     'floating point number': 'float',
     'character': 'str',
     'integer': 'int',
@@ -358,19 +441,18 @@
         ret_str = re.sub(r'[nN]ew (.*)', r'\1()', ret_str)
 
         ret = docstr_defaults.get(ret_str, ret_str)
 
     return param_str, ret
 
 
-class Builtin(CompiledObject, IsScope):
-    @memoize
+class Builtin(CompiledObject):
+    @memoize_method
     def get_by_name(self, name):
-        item = [n for n in self.get_defined_names() if n.get_code() == name][0]
-        return item.parent
+        return self.names_dict[name][0].parent
 
 
 def _a_generator(foo):
     """Used to have an object to return for generators."""
     yield 42
     yield foo
 
@@ -391,16 +473,30 @@
         obj = None
     return CompiledObject(obj, parent)
 
 
 builtin = Builtin(_builtins)
 magic_function_class = CompiledObject(type(load_module), parent=builtin)
 generator_obj = CompiledObject(_a_generator(1.0))
-type_names = []  # Need this, because it's return in get_defined_names.
-type_names = builtin.get_by_name('type').get_defined_names()
+_type_names_dict = builtin.get_by_name('type').names_dict
+none_obj = builtin.get_by_name('None')
+false_obj = builtin.get_by_name('False')
+true_obj = builtin.get_by_name('True')
+object_obj = builtin.get_by_name('object')
+
+
+def keyword_from_value(obj):
+    if obj is None:
+        return none_obj
+    elif obj is False:
+        return false_obj
+    elif obj is True:
+        return true_obj
+    else:
+        raise NotImplementedError
 
 
 def compiled_objects_cache(func):
     def wrapper(evaluator, obj, parent=builtin, module=None):
         # Do a very cheap form of caching here.
         key = id(obj), id(parent), id(module)
         try:
@@ -422,8 +518,14 @@
 
     if not inspect.ismodule(obj):
         faked = fake.get_faked(module and module.obj, obj)
         if faked is not None:
             faked.parent = parent
             return faked
 
+    try:
+        if parent == builtin and obj.__module__ in ('builtins', '__builtin__'):
+            return builtin.get_by_name(obj.__name__)
+    except AttributeError:
+        pass
+
     return CompiledObject(obj, parent)
```

### Comparing `jedi-0.8.1-final0/jedi/evaluate/compiled/fake/builtins.pym` & `jedi-0.9.0/jedi/evaluate/compiled/fake/builtins.pym`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 This code is not going to be executed anywhere.
 These implementations are not always correct, but should work as good as
 possible for the auto completion.
 """
 
 
 def next(iterator, default=None):
-    if hasattr("next"):
-        return iterator.next()
+    if random.choice([0, 1]):
+        if hasattr("next"):
+            return iterator.next()
+        else:
+            return iterator.__next__()
     else:
-        return iterator.__next__()
-    return default
+        if default is not None:
+            return default
 
 
 def iter(collection, sentinel=None):
     if sentinel:
         yield collection()
     else:
         for c in collection:
@@ -149,15 +152,15 @@
         self.__iterable = iterable
 
     def __iter__(self):
         for i in self.__iterable:
             yield i
 
     def pop(self):
-        return self.__iterable.pop()
+        return list(self.__iterable)[-1]
 
     def copy(self):
         return self
 
     def difference(self, other):
         return self - other
```

### Comparing `jedi-0.8.1-final0/jedi/evaluate/compiled/fake/_sre.pym` & `jedi-0.9.0/jedi/evaluate/compiled/fake/_sre.pym`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/jedi/evaluate/compiled/fake.py` & `jedi-0.9.0/jedi/evaluate/compiled/fake.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 mixing in Python code, the autocompletion should work much better for builtins.
 """
 
 import os
 import inspect
 
 from jedi._compatibility import is_py3, builtins, unicode
-from jedi.parser import Parser
-from jedi.parser import tokenize
-from jedi.parser.representation import Class
+from jedi.parser import Parser, load_grammar
+from jedi.parser import tree as pt
 from jedi.evaluate.helpers import FakeName
 
 modules = {}
 
 
 def _load_faked_module(module):
     module_name = module.__name__
@@ -27,24 +26,25 @@
         path = os.path.dirname(os.path.abspath(__file__))
         try:
             with open(os.path.join(path, 'fake', module_name) + '.pym') as f:
                 source = f.read()
         except IOError:
             modules[module_name] = None
             return
-        module = Parser(unicode(source), module_name).module
+        grammar = load_grammar('grammar3.4')
+        module = Parser(grammar, unicode(source), module_name).module
         modules[module_name] = module
 
         if module_name == 'builtins' and not is_py3:
             # There are two implementations of `open` for either python 2/3.
             # -> Rename the python2 version (`look at fake/builtins.pym`).
             open_func = search_scope(module, 'open')
-            open_func.name = FakeName('open_python3')
+            open_func.children[1] = FakeName('open_python3')
             open_func = search_scope(module, 'open_python2')
-            open_func.name = FakeName('open')
+            open_func.children[1] = FakeName('open')
         return module
 
 
 def search_scope(scope, obj_name):
     for s in scope.subscopes:
         if str(s.name) == obj_name:
             return s
@@ -96,19 +96,26 @@
                 return
             return search_scope(cls, name)
 
 
 def get_faked(module, obj, name=None):
     obj = obj.__class__ if is_class_instance(obj) else obj
     result = _faked(module, obj, name)
-    if not isinstance(result, Class) and result is not None:
+    if result is None or isinstance(result, pt.Class):
+        # We're not interested in classes. What we want is functions.
+        return None
+    else:
         # Set the docstr which was previously not set (faked modules don't
         # contain it).
-        doc = '''"""%s"""''' % obj.__doc__  # TODO need escapes.
-        result.add_docstr(tokenize.Token(tokenize.STRING, doc, (0, 0)))
+        doc = '"""%s"""' % obj.__doc__  # TODO need escapes.
+        suite = result.children[-1]
+        string = pt.String(pt.zero_position_modifier, doc, (0, 0), '')
+        new_line = pt.Whitespace('\n', (0, 0), '')
+        docstr_node = pt.Node('simple_stmt', [string, new_line])
+        suite.children.insert(2, docstr_node)
         return result
 
 
 def is_class_instance(obj):
     """Like inspect.* methods."""
     return not (inspect.isclass(obj) or inspect.ismodule(obj)
                 or inspect.isbuiltin(obj) or inspect.ismethod(obj)
```

### Comparing `jedi-0.8.1-final0/jedi/evaluate/finder.py` & `jedi-0.9.0/jedi/evaluate/finder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,567 +1,547 @@
 """
-Searcjing for names with given scope and name. This is very central in Jedi and
+Searching for names with given scope and name. This is very central in Jedi and
 Python. The name resolution is quite complicated with descripter,
 ``__getattribute__``, ``__getattr__``, ``global``, etc.
 
 Flow checks
 +++++++++++
 
 Flow checks are not really mature. There's only a check for ``isinstance``.  It
 would check whether a flow has the form of ``if isinstance(a, type_or_tuple)``.
 Unfortunately every other thing is being ignored (e.g. a == '' would be easy to
 check for -> a is a string). There's big potential in these checks.
 """
 from itertools import chain
 
-from jedi._compatibility import hasattr, unicode, u
-from jedi.parser import representation as pr, tokenize
-from jedi.parser import fast
+from jedi._compatibility import unicode, u
+from jedi.parser import tree
 from jedi import debug
 from jedi import common
 from jedi import settings
 from jedi.evaluate import representation as er
 from jedi.evaluate import dynamic
 from jedi.evaluate import compiled
 from jedi.evaluate import docstrings
 from jedi.evaluate import iterable
 from jedi.evaluate import imports
 from jedi.evaluate import analysis
-from jedi.evaluate import precedence
+from jedi.evaluate import flow_analysis
+from jedi.evaluate import param
+from jedi.evaluate import helpers
+from jedi.evaluate.cache import memoize_default
+
+
+def filter_after_position(names, position):
+    """
+    Removes all names after a certain position. If position is None, just
+    returns the names list.
+    """
+    if position is None:
+        return names
+
+    names_new = []
+    for n in names:
+        # Filter positions and also allow list comprehensions and lambdas.
+        if n.start_pos[0] is not None and n.start_pos < position \
+                or isinstance(n.get_definition(), (tree.CompFor, tree.Lambda)):
+            names_new.append(n)
+    return names_new
+
+
+def filter_definition_names(names, origin, position=None):
+    """
+    Filter names that are actual definitions in a scope. Names that are just
+    used will be ignored.
+    """
+    # Just calculate the scope from the first
+    stmt = names[0].get_definition()
+    scope = stmt.get_parent_scope()
+
+    if not (isinstance(scope, er.FunctionExecution)
+            and isinstance(scope.base, er.LambdaWrapper)):
+        names = filter_after_position(names, position)
+    names = [name for name in names if name.is_definition()]
+
+    # Private name mangling (compile.c) disallows access on names
+    # preceeded by two underscores `__` if used outside of the class. Names
+    # that also end with two underscores (e.g. __id__) are not affected.
+    for name in list(names):
+        if name.value.startswith('__') and not name.value.endswith('__'):
+            if filter_private_variable(scope, origin):
+                names.remove(name)
+    return names
 
 
 class NameFinder(object):
     def __init__(self, evaluator, scope, name_str, position=None):
         self._evaluator = evaluator
-        self.scope = scope
+        # Make sure that it's not just a syntax tree node.
+        self.scope = evaluator.wrap(scope)
         self.name_str = name_str
         self.position = position
 
     @debug.increase_indent
-    def find(self, scopes, resolve_decorator=True, search_global=False):
-        if unicode(self.name_str) == 'None':
-            # Filter None, because it's really just a keyword, nobody wants to
-            # access it.
-            return []
-
+    def find(self, scopes, search_global=False):
+        # TODO rename scopes to names_dicts
         names = self.filter_name(scopes)
-        types = self._names_to_types(names, resolve_decorator)
+        types = self._names_to_types(names, search_global)
 
         if not names and not types \
-                and not (isinstance(self.name_str, pr.NamePart)
-                         and isinstance(self.name_str.parent.parent, pr.Param)):
+                and not (isinstance(self.name_str, tree.Name)
+                         and isinstance(self.name_str.parent.parent, tree.Param)):
             if not isinstance(self.name_str, (str, unicode)):  # TODO Remove?
                 if search_global:
                     message = ("NameError: name '%s' is not defined."
                                % self.name_str)
                     analysis.add(self._evaluator, 'name-error', self.name_str,
                                  message)
                 else:
                     analysis.add_attribute_error(self._evaluator,
                                                  self.scope, self.name_str)
 
         debug.dbg('finder._names_to_types: %s -> %s', names, types)
-        return self._resolve_descriptors(types)
+        return types
 
     def scopes(self, search_global=False):
         if search_global:
-            return get_names_of_scope(self._evaluator, self.scope, self.position)
+            return global_names_dict_generator(self._evaluator, self.scope, self.position)
         else:
-            return self.scope.scope_names_generator(self.position)
+            return ((n, None) for n in self.scope.names_dicts(search_global))
+
+    def names_dict_lookup(self, names_dict, position):
+        def get_param(scope, el):
+            if isinstance(el.get_parent_until(tree.Param), tree.Param):
+                return scope.param_by_name(str(el))
+            return el
+
+        search_str = str(self.name_str)
+        try:
+            names = names_dict[search_str]
+            if not names:  # We want names, otherwise stop.
+                return []
+        except KeyError:
+            return []
+
+        names = filter_definition_names(names, self.name_str, position)
+
+        name_scope = None
+        # Only the names defined in the last position are valid definitions.
+        last_names = []
+        for name in reversed(sorted(names, key=lambda name: name.start_pos)):
+            stmt = name.get_definition()
+            name_scope = self._evaluator.wrap(stmt.get_parent_scope())
+
+            if isinstance(self.scope, er.Instance) and not isinstance(name_scope, er.Instance):
+                # Instances should not be checked for positioning, because we
+                # don't know in which order the functions are called.
+                last_names.append(name)
+                continue
+
+            if isinstance(name_scope, compiled.CompiledObject):
+                # Let's test this. TODO need comment. shouldn't this be
+                # filtered before?
+                last_names.append(name)
+                continue
+
+            if isinstance(name, compiled.CompiledName) \
+                    or isinstance(name, er.InstanceName) and isinstance(name._origin_name, compiled.CompiledName):
+                last_names.append(name)
+                continue
+
+            if isinstance(self.name_str, tree.Name):
+                origin_scope = self.name_str.get_parent_until(tree.Scope, reverse=True)
+            else:
+                origin_scope = None
+            if isinstance(stmt.parent, compiled.CompiledObject):
+                # TODO seriously? this is stupid.
+                continue
+            check = flow_analysis.break_check(self._evaluator, name_scope,
+                                              stmt, origin_scope)
+            if check is not flow_analysis.UNREACHABLE:
+                last_names.append(name)
+            if check is flow_analysis.REACHABLE:
+                break
+
+        if isinstance(name_scope, er.FunctionExecution):
+            # Replace params
+            return [get_param(name_scope, n) for n in last_names]
+        return last_names
 
-    def filter_name(self, scope_names_generator):
+    def filter_name(self, names_dicts):
         """
-        Filters all variables of a scope (which are defined in the
-        `scope_names_generator`), until the name fits.
+        Searches names that are defined in a scope (the different
+        `names_dicts`), until a name fits.
         """
-        result = []
-        for name_list_scope, name_list in scope_names_generator:
-            break_scopes = []
-            if not isinstance(name_list_scope, compiled.CompiledObject):
-                # Here is the position stuff happening (sorting of variables).
-                # Compiled objects don't need that, because there's only one
-                # reference.
-                name_list = sorted(name_list, key=lambda n: n.start_pos, reverse=True)
-
-            for name in name_list:
-                if unicode(self.name_str) != name.get_code():
-                    continue
-
-                scope = name.parent.parent
-                if scope in break_scopes:
-                    continue
-
-                # Exclude `arr[1] =` from the result set.
-                if not self._name_is_array_assignment(name):
-                    result.append(name)
-
-                if result and self._is_name_break_scope(name):
-                    if self._does_scope_break_immediately(scope, name_list_scope):
-                        break
-                    else:
-                        break_scopes.append(scope)
-            if result:
+        names = []
+        for names_dict, position in names_dicts:
+            names = self.names_dict_lookup(names_dict, position)
+            if names:
                 break
 
-        scope_txt = (self.scope if self.scope == name_list_scope
-                     else '%s-%s' % (self.scope, name_list_scope))
         debug.dbg('finder.filter_name "%s" in (%s): %s@%s', self.name_str,
-                  scope_txt, u(result), self.position)
-        return result
+                  self.scope, u(names), self.position)
+        return list(self._clean_names(names))
+
+    def _clean_names(self, names):
+        """
+        ``NameFinder.filter_name`` should only output names with correct
+        wrapper parents. We don't want to see AST classes out in the
+        evaluation, so remove them already here!
+        """
+        for n in names:
+            definition = n.parent
+            if isinstance(definition, (tree.Function, tree.Class, tree.Module)):
+                yield self._evaluator.wrap(definition).name
+            else:
+                yield n
 
     def _check_getattr(self, inst):
         """Checks for both __getattr__ and __getattribute__ methods"""
         result = []
-        # str is important to lose the NamePart!
+        # str is important, because it shouldn't be `Name`!
         name = compiled.create(self._evaluator, str(self.name_str))
         with common.ignored(KeyError):
-            result = inst.execute_subscope_by_name('__getattr__', [name])
+            result = inst.execute_subscope_by_name('__getattr__', name)
         if not result:
             # this is a little bit special. `__getattribute__` is executed
             # before anything else. But: I know no use case, where this
             # could be practical and the jedi would return wrong types. If
             # you ever have something, let me know!
             with common.ignored(KeyError):
-                result = inst.execute_subscope_by_name('__getattribute__', [name])
+                result = inst.execute_subscope_by_name('__getattribute__', name)
         return result
 
-    def _is_name_break_scope(self, name):
-        """
-        Returns True except for nested imports and instance variables.
-        """
-        par = name.parent
-        if par.isinstance(pr.Statement):
-            if isinstance(name, er.InstanceElement) and not name.is_class_var:
-                return False
-        elif isinstance(par, pr.Import) and par.is_nested():
-            return False
-        return True
-
-    def _does_scope_break_immediately(self, scope, name_list_scope):
-        """
-        In comparison to everthing else, if/while/etc doesn't break directly,
-        because there are multiple different places in which a variable can be
-        defined.
-        """
-        if isinstance(scope, pr.Flow) \
-                or isinstance(scope, pr.KeywordStatement) and scope.name == 'global':
-
-            # Check for `if foo is not None`, because Jedi is not interested in
-            # None values, so this is the only branch we actually care about.
-            # ATM it carries the same issue as the isinstance checks. It
-            # doesn't work with instance variables (self.foo).
-            if isinstance(scope, pr.Flow) and scope.command in ('if', 'while'):
-                try:
-                    expression_list = scope.inputs[0].expression_list()
-                except IndexError:
-                    pass
-                else:
-                    p = precedence.create_precedence(expression_list)
-                    if (isinstance(p, precedence.Precedence)
-                            and p.operator.string == 'is not'
-                            and p.right.get_code() == 'None'
-                            and p.left.get_code() == unicode(self.name_str)):
-                        return True
-
-            if isinstance(name_list_scope, er.Class):
-                name_list_scope = name_list_scope.base
-            return scope == name_list_scope
-        else:
-            return True
-
-    def _name_is_array_assignment(self, name):
-        if name.parent.isinstance(pr.Statement):
-            def is_execution(calls):
-                for c in calls:
-                    if isinstance(c, (unicode, str, tokenize.Token)):
-                        continue
-                    if c.isinstance(pr.Array):
-                        if is_execution(c):
-                            return True
-                    elif c.isinstance(pr.Call):
-                        # Compare start_pos, because names may be different
-                        # because of executions.
-                        if c.name.start_pos == name.start_pos \
-                                and c.execution:
-                            return True
-                return False
-
-            is_exe = False
-            for assignee, op in name.parent.assignment_details:
-                is_exe |= is_execution(assignee)
-
-            if is_exe:
-                # filter array[3] = ...
-                # TODO check executions for dict contents
-                return True
-        return False
-
-    def _names_to_types(self, names, resolve_decorator):
+    def _names_to_types(self, names, search_global):
         types = []
+
         # Add isinstance and other if/assert knowledge.
-        flow_scope = self.scope
-        evaluator = self._evaluator
-        while flow_scope:
-            # TODO check if result is in scope -> no evaluation necessary
-            n = check_flow_information(evaluator, flow_scope,
-                                       self.name_str, self.position)
-            if n:
-                return n
-            flow_scope = flow_scope.parent
+        if isinstance(self.name_str, tree.Name):
+            # Ignore FunctionExecution parents for now.
+            flow_scope = self.name_str
+            until = flow_scope.get_parent_until(er.FunctionExecution)
+            while not isinstance(until, er.FunctionExecution):
+                flow_scope = flow_scope.get_parent_scope(include_flows=True)
+                if flow_scope is None:
+                    break
+                # TODO check if result is in scope -> no evaluation necessary
+                n = check_flow_information(self._evaluator, flow_scope,
+                                           self.name_str, self.position)
+                if n:
+                    return n
 
         for name in names:
-            typ = name.parent
-            if typ.isinstance(pr.ForFlow):
-                types += self._handle_for_loops(typ)
-            elif isinstance(typ, pr.Param):
-                types += self._eval_param(typ)
-            elif typ.isinstance(pr.Statement):
-                if typ.is_global():
-                    # global keyword handling.
-                    types += evaluator.find_types(typ.parent.parent, str(name))
-                else:
-                    types += self._remove_statements(typ, name)
+            new_types = _name_to_types(self._evaluator, name, self.scope)
+            if isinstance(self.scope, (er.Class, er.Instance)) and not search_global:
+                types += self._resolve_descriptors(name, new_types)
             else:
-                if isinstance(typ, pr.Class):
-                    typ = er.Class(evaluator, typ)
-                elif isinstance(typ, pr.Function):
-                    typ = er.Function(evaluator, typ)
-                elif isinstance(typ, pr.Module):
-                    typ = er.ModuleWrapper(evaluator, typ)
-
-                if typ.isinstance(er.Function) and resolve_decorator:
-                    typ = typ.get_decorated_func()
-                types.append(typ)
-
+                types += new_types
         if not names and isinstance(self.scope, er.Instance):
             # handling __getattr__ / __getattribute__
             types = self._check_getattr(self.scope)
 
         return types
 
-    def _remove_statements(self, stmt, name):
-        """
-        This is the part where statements are being stripped.
+    def _resolve_descriptors(self, name, types):
+        # The name must not be in the dictionary, but part of the class
+        # definition. __get__ is only called if the descriptor is defined in
+        # the class dictionary.
+        name_scope = name.get_definition().get_parent_scope()
+        if not isinstance(name_scope, (er.Instance, tree.Class)):
+            return types
 
-        Due to lazy evaluation, statements like a = func; b = a; b() have to be
-        evaluated.
-        """
-        evaluator = self._evaluator
-        types = []
-        # Remove the statement docstr stuff for now, that has to be
-        # implemented with the evaluator class.
-        #if stmt.docstr:
-            #res_new.append(stmt)
-
-        check_instance = None
-        if isinstance(stmt, er.InstanceElement) and stmt.is_class_var:
-            check_instance = stmt.instance
-            stmt = stmt.var
-
-        types += evaluator.eval_statement(stmt, seek_name=unicode(self.name_str))
-
-        # check for `except X as y` usages, because y needs to be instantiated.
-        p = stmt.parent
-        # TODO this looks really hacky, improve parser representation!
-        if isinstance(p, pr.Flow) and p.command == 'except' \
-                and p.inputs and p.inputs[0].as_names == [name]:
-            # TODO check for types that are not classes and add it to the
-            # static analysis report.
-            types = list(chain.from_iterable(
-                         evaluator.execute(t) for t in types))
-
-        if check_instance is not None:
-            # class renames
-            types = [er.InstanceElement(evaluator, check_instance, a, True)
-                     if isinstance(a, (er.Function, pr.Function))
-                     else a for a in types]
-        return types
-
-    def _eval_param(self, param):
-        evaluator = self._evaluator
-        res_new = []
-        func = param.parent
-
-        cls = func.parent.get_parent_until((pr.Class, pr.Function))
-
-        from jedi.evaluate.param import ExecutedParam
-        if isinstance(cls, pr.Class) and param.position_nr == 0 \
-                and not isinstance(param, ExecutedParam):
-            # This is where we add self - if it has never been
-            # instantiated.
-            if isinstance(self.scope, er.InstanceElement):
-                res_new.append(self.scope.instance)
-            else:
-                for inst in evaluator.execute(er.Class(evaluator, cls)):
-                    inst.is_generated = True
-                    res_new.append(inst)
-            return res_new
-
-        # Instances are typically faked, if the instance is not called from
-        # outside. Here we check it for __init__ functions and return.
-        if isinstance(func, er.InstanceElement) \
-                and func.instance.is_generated and str(func.name) == '__init__':
-            param = func.var.params[param.position_nr]
-
-        # Add docstring knowledge.
-        doc_params = docstrings.follow_param(evaluator, param)
-        if doc_params:
-            return doc_params
-
-        if not param.is_generated:
-            # Param owns no information itself.
-            res_new += dynamic.search_params(evaluator, param)
-            if not res_new:
-                if param.stars:
-                    t = 'tuple' if param.stars == 1 else 'dict'
-                    typ = evaluator.find_types(compiled.builtin, t)[0]
-                    res_new = evaluator.execute(typ)
-            if not param.assignment_details:
-                # this means that there are no default params,
-                # so just ignore it.
-                return res_new
-        return res_new + evaluator.eval_statement(param, seek_name=unicode(self.name_str))
-
-    def _handle_for_loops(self, loop):
-        # Take the first statement (for has always only one`in`).
-        if not loop.inputs:
-            return []
-        result = iterable.get_iterator_types(self._evaluator.eval_statement(loop.inputs[0]))
-        if len(loop.set_vars) > 1:
-            expression_list = loop.set_stmt.expression_list()
-            # loops with loop.set_vars > 0 only have one command
-            result = _assign_tuples(expression_list[0], result, unicode(self.name_str))
-        return result
-
-    def _resolve_descriptors(self, types):
-        """Processes descriptors"""
         result = []
         for r in types:
-            if isinstance(self.scope, (er.Instance, er.Class)) \
-                    and hasattr(r, 'get_descriptor_return'):
-                # handle descriptors
-                with common.ignored(KeyError):
-                    result += r.get_descriptor_return(self.scope)
-                    continue
-            result.append(r)
+            try:
+                desc_return = r.get_descriptor_returns
+            except AttributeError:
+                result.append(r)
+            else:
+                result += desc_return(self.scope)
         return result
 
 
-def check_flow_information(evaluator, flow, search_name_part, pos):
+@memoize_default([], evaluator_is_first_arg=True)
+def _name_to_types(evaluator, name, scope):
+    types = []
+    typ = name.get_definition()
+    if typ.isinstance(tree.ForStmt):
+        for_types = evaluator.eval_element(typ.children[3])
+        for_types = iterable.get_iterator_types(for_types)
+        types += check_tuple_assignments(for_types, name)
+    elif typ.isinstance(tree.CompFor):
+        for_types = evaluator.eval_element(typ.children[3])
+        for_types = iterable.get_iterator_types(for_types)
+        types += check_tuple_assignments(for_types, name)
+    elif isinstance(typ, tree.Param):
+        types += _eval_param(evaluator, typ, scope)
+    elif typ.isinstance(tree.ExprStmt):
+        types += _remove_statements(evaluator, typ, name)
+    elif typ.isinstance(tree.WithStmt):
+        types += evaluator.eval_element(typ.node_from_name(name))
+    elif isinstance(typ, tree.Import):
+        types += imports.ImportWrapper(evaluator, name).follow()
+    elif isinstance(typ, tree.GlobalStmt):
+        # TODO theoretically we shouldn't be using search_global here, it
+        # doesn't make sense, because it's a local search (for that name)!
+        # However, globals are not that important and resolving them doesn't
+        # guarantee correctness in any way, because we don't check for when
+        # something is executed.
+        types += evaluator.find_types(typ.get_parent_scope(), str(name),
+                                      search_global=True)
+    elif isinstance(typ, tree.TryStmt):
+        # TODO an exception can also be a tuple. Check for those.
+        # TODO check for types that are not classes and add it to
+        # the static analysis report.
+        exceptions = evaluator.eval_element(name.prev_sibling().prev_sibling())
+        types = list(chain.from_iterable(
+                     evaluator.execute(t) for t in exceptions))
+    else:
+        if typ.isinstance(er.Function):
+            typ = typ.get_decorated_func()
+        types.append(typ)
+    return types
+
+
+def _remove_statements(evaluator, stmt, name):
+    """
+    This is the part where statements are being stripped.
+
+    Due to lazy evaluation, statements like a = func; b = a; b() have to be
+    evaluated.
+    """
+    types = []
+    # Remove the statement docstr stuff for now, that has to be
+    # implemented with the evaluator class.
+    #if stmt.docstr:
+        #res_new.append(stmt)
+
+    check_instance = None
+    if isinstance(stmt, er.InstanceElement) and stmt.is_class_var:
+        check_instance = stmt.instance
+        stmt = stmt.var
+
+    types += evaluator.eval_statement(stmt, seek_name=name)
+
+    if check_instance is not None:
+        # class renames
+        types = [er.get_instance_el(evaluator, check_instance, a, True)
+                 if isinstance(a, (er.Function, tree.Function))
+                 else a for a in types]
+    return types
+
+
+def _eval_param(evaluator, param, scope):
+    res_new = []
+    func = param.get_parent_scope()
+
+    cls = func.parent.get_parent_until((tree.Class, tree.Function))
+
+    from jedi.evaluate.param import ExecutedParam, Arguments
+    if isinstance(cls, tree.Class) and param.position_nr == 0 \
+            and not isinstance(param, ExecutedParam):
+        # This is where we add self - if it has never been
+        # instantiated.
+        if isinstance(scope, er.InstanceElement):
+            res_new.append(scope.instance)
+        else:
+            inst = er.Instance(evaluator, evaluator.wrap(cls),
+                               Arguments(evaluator, ()), is_generated=True)
+            res_new.append(inst)
+        return res_new
+
+    # Instances are typically faked, if the instance is not called from
+    # outside. Here we check it for __init__ functions and return.
+    if isinstance(func, er.InstanceElement) \
+            and func.instance.is_generated and str(func.name) == '__init__':
+        param = func.var.params[param.position_nr]
+
+    # Add docstring knowledge.
+    doc_params = docstrings.follow_param(evaluator, param)
+    if doc_params:
+        return doc_params
+
+    if isinstance(param, ExecutedParam):
+        return res_new + param.eval(evaluator)
+    else:
+        # Param owns no information itself.
+        res_new += dynamic.search_params(evaluator, param)
+        if not res_new:
+            if param.stars:
+                t = 'tuple' if param.stars == 1 else 'dict'
+                typ = evaluator.find_types(compiled.builtin, t)[0]
+                res_new = evaluator.execute(typ)
+        if param.default:
+            res_new += evaluator.eval_element(param.default)
+        return res_new
+
+
+def check_flow_information(evaluator, flow, search_name, pos):
     """ Try to find out the type of a variable just with the information that
     is given by the flows: e.g. It is also responsible for assert checks.::
 
         if isinstance(k, str):
             k.  # <- completion here
 
     ensures that `k` is a string.
     """
     if not settings.dynamic_flow_information:
         return None
 
     result = []
-    if isinstance(flow, pr.IsScope) and not result:
-        for ass in reversed(flow.asserts):
-            if pos is None or ass.start_pos > pos:
-                continue
-            result = _check_isinstance_type(evaluator, ass, search_name_part)
-            if result:
-                break
+    if flow.is_scope():
+        # Check for asserts.
+        try:
+            names = reversed(flow.names_dict[search_name.value])
+        except (KeyError, AttributeError):
+            names = []
 
-    if isinstance(flow, pr.Flow) and not result:
-        if flow.command in ['if', 'while'] and len(flow.inputs) == 1:
-            result = _check_isinstance_type(evaluator, flow.inputs[0], search_name_part)
+        for name in names:
+            ass = name.get_parent_until(tree.AssertStmt)
+            if isinstance(ass, tree.AssertStmt) and pos is not None and ass.start_pos < pos:
+                result = _check_isinstance_type(evaluator, ass.assertion(), search_name)
+                if result:
+                    break
+
+    if isinstance(flow, (tree.IfStmt, tree.WhileStmt)):
+        element = flow.children[1]
+        result = _check_isinstance_type(evaluator, element, search_name)
     return result
 
 
-def _check_isinstance_type(evaluator, stmt, search_name_part):
+def _check_isinstance_type(evaluator, element, search_name):
     try:
-        expression_list = stmt.expression_list()
+        assert element.type == 'power'
         # this might be removed if we analyze and, etc
-        assert len(expression_list) == 1
-        call = expression_list[0]
-        assert isinstance(call, pr.Call) and str(call.name) == 'isinstance'
-        assert bool(call.execution)
-
-        # isinstance check
-        isinst = call.execution.values
-        assert len(isinst) == 2  # has two params
-        obj, classes = [statement.expression_list() for statement in isinst]
-        assert len(obj) == 1
-        assert len(classes) == 1
-        assert isinstance(obj[0], pr.Call)
-
-        # names fit?
-        assert unicode(obj[0].name) == unicode(search_name_part)
-        assert isinstance(classes[0], pr.StatementElement)  # can be type or tuple
+        assert len(element.children) == 2
+        first, trailer = element.children
+        assert isinstance(first, tree.Name) and first.value == 'isinstance'
+        assert trailer.type == 'trailer' and trailer.children[0] == '('
+        assert len(trailer.children) == 3
+
+        # arglist stuff
+        arglist = trailer.children[1]
+        args = param.Arguments(evaluator, arglist, trailer)
+        lst = list(args.unpack())
+        # Disallow keyword arguments
+        assert len(lst) == 2 and lst[0][0] is None and lst[1][0] is None
+        name = lst[0][1][0]  # first argument, values, first value
+        # Do a simple get_code comparison. They should just have the same code,
+        # and everything will be all right.
+        classes = lst[1][1][0]
+        call = helpers.call_of_name(search_name)
+        assert name.get_code() == call.get_code()
     except AssertionError:
         return []
 
     result = []
-    for c in evaluator.eval_call(classes[0]):
-        for typ in (c.values() if isinstance(c, iterable.Array) else [c]):
+    for typ in evaluator.eval_element(classes):
+        for typ in (typ.values() if isinstance(typ, iterable.Array) else [typ]):
             result += evaluator.execute(typ)
     return result
 
 
-def get_names_of_scope(evaluator, scope, position=None, star_search=True, include_builtin=True):
+def global_names_dict_generator(evaluator, scope, position):
     """
-    Get all completions (names) possible for the current scope. The star search
-    option is only here to provide an optimization. Otherwise the whole thing
-    would probably start a little recursive madness.
+    For global name lookups. Yields tuples of (names_dict, position). If the
+    position is None, the position does not matter anymore in that scope.
 
     This function is used to include names from outer scopes. For example, when
     the current scope is function:
 
-    >>> from jedi._compatibility import u
-    >>> from jedi.parser import Parser
-    >>> parser = Parser(u('''
+    >>> from jedi._compatibility import u, no_unicode_pprint
+    >>> from jedi.parser import Parser, load_grammar
+    >>> parser = Parser(load_grammar(), u('''
     ... x = ['a', 'b', 'c']
     ... def func():
     ...     y = None
     ... '''))
     >>> scope = parser.module.subscopes[0]
     >>> scope
     <Function: func@3-5>
 
-    `get_names_of_scope` is a generator.  First it yields names from most inner
-    scope.
+    `global_names_dict_generator` is a generator.  First it yields names from
+    most inner scope.
 
     >>> from jedi.evaluate import Evaluator
-    >>> pairs = list(get_names_of_scope(Evaluator(), scope))
-    >>> pairs[0]
-    (<Function: func@3-5>, [<Name: y@4,4>])
-
-    Then it yield the names from one level outer scope. For this example, this
-    is the most outer scope.
-
-    >>> pairs[1]
-    (<ModuleWrapper: <SubModule: None@1-5>>, [<Name: x@2,0>, <Name: func@3,4>])
-
-    After that we have a few underscore names that have been defined
-
-    >>> pairs[2]
-    (<ModuleWrapper: <SubModule: None@1-5>>, [<FakeName: __file__@0,0>, ...])
-
+    >>> evaluator = Evaluator(load_grammar())
+    >>> scope = evaluator.wrap(scope)
+    >>> pairs = list(global_names_dict_generator(evaluator, scope, (4, 0)))
+    >>> no_unicode_pprint(pairs[0])
+    ({'func': [], 'y': [<Name: y@4,4>]}, (4, 0))
+
+    Then it yields the names from one level "lower". In this example, this
+    is the most outer scope. As you can see, the position in the tuple is now
+    None, because typically the whole module is loaded before the function is
+    called.
+
+    >>> no_unicode_pprint(pairs[1])
+    ({'func': [<Name: func@3,4>], 'x': [<Name: x@2,0>]}, None)
+
+    After that we have a few underscore names that are part of the module.
+
+    >>> sorted(pairs[2][0].keys())
+    ['__doc__', '__file__', '__name__', '__package__']
+    >>> pairs[3]  # global names -> there are none in our example.
+    ({}, None)
+    >>> pairs[4]  # package modules -> Also none.
+    ({}, None)
 
     Finally, it yields names from builtin, if `include_builtin` is
     true (default).
 
-    >>> pairs[3]                                        #doctest: +ELLIPSIS
-    (<Builtin: ...builtin...>, [<CompiledName: ...>, ...])
-
-    :rtype: [(pr.Scope, [pr.Name])]
-    :return: Return an generator that yields a pair of scope and names.
+    >>> pairs[5][0].values()                              #doctest: +ELLIPSIS
+    [[<CompiledName: ...>], ...]
     """
-    if isinstance(scope, pr.ListComprehension):
-        position = scope.parent.start_pos
+    in_func = False
+    while scope is not None:
+        if not (scope.type == 'classdef' and in_func):
+            # Names in methods cannot be resolved within the class.
+
+            for names_dict in scope.names_dicts(True):
+                yield names_dict, position
+            if scope.type == 'funcdef':
+                # The position should be reset if the current scope is a function.
+                in_func = True
+                position = None
+        scope = evaluator.wrap(scope.get_parent_scope())
+
+    # Add builtins to the global scope.
+    for names_dict in compiled.builtin.names_dicts(True):
+        yield names_dict, None
 
-    in_func_scope = scope
-    non_flow = scope.get_parent_until(pr.Flow, reverse=True)
-    while scope:
-        # We don't want submodules to report if we have modules.
-        # As well as some non-scopes, which are parents of list comprehensions.
-        if isinstance(scope, pr.SubModule) and scope.parent or not scope.is_scope():
-            scope = scope.parent
-            continue
-        # `pr.Class` is used, because the parent is never `Class`.
-        # Ignore the Flows, because the classes and functions care for that.
-        # InstanceElement of Class is ignored, if it is not the start scope.
-        if not (scope != non_flow and scope.isinstance(pr.Class)
-                or scope.isinstance(pr.Flow)
-                or scope.isinstance(er.Instance)
-                and non_flow.isinstance(er.Function)
-                or isinstance(scope, compiled.CompiledObject)
-                and scope.type() == 'class' and in_func_scope != scope):
-
-            if isinstance(scope, (pr.SubModule, fast.Module)):
-                scope = er.ModuleWrapper(evaluator, scope)
-
-            for g in scope.scope_names_generator(position):
-                yield g
-        if scope.isinstance(pr.ListComprehension):
-            # is a list comprehension
-            yield scope, scope.get_defined_names(is_internal_call=True)
-
-        scope = scope.parent
-        # This is used, because subscopes (Flow scopes) would distort the
-        # results.
-        if scope and scope.isinstance(er.Function, pr.Function, er.FunctionExecution):
-            in_func_scope = scope
-        if in_func_scope != scope \
-                and isinstance(in_func_scope, (pr.Function, er.FunctionExecution)):
-            position = None
-
-    # Add star imports.
-    if star_search:
-        for s in imports.remove_star_imports(evaluator, non_flow.get_parent_until()):
-            for g in get_names_of_scope(evaluator, s, star_search=False):
-                yield g
-
-        # Add builtins to the global scope.
-        if include_builtin:
-            yield compiled.builtin, compiled.builtin.get_defined_names()
-
-
-def _assign_tuples(tup, results, seek_name):
-    """
-    This is a normal assignment checker. In python functions and other things
-    can return tuples:
-    >>> a, b = 1, ""
-    >>> a, (b, c) = 1, ("", 1.0)
 
-    Here, if `seek_name` is "a", the number type will be returned.
-    The first part (before `=`) is the param tuples, the second one result.
-
-    :type tup: pr.Array
+def check_tuple_assignments(types, name):
     """
-    def eval_results(index):
-        types = []
-        for r in results:
+    Checks if tuples are assigned.
+    """
+    for index in name.assignment_indexes():
+        new_types = []
+        for r in types:
             try:
                 func = r.get_exact_index_types
             except AttributeError:
-                debug.warning("invalid tuple lookup %s of result %s in %s",
-                              tup, results, seek_name)
+                debug.warning("Invalid tuple lookup #%s of result %s in %s",
+                              index, types, name)
             else:
-                with common.ignored(IndexError):
-                    types += func(index)
-        return types
-
-    result = []
-    for i, stmt in enumerate(tup):
-        # Used in assignments. There is just one call and no other things,
-        # therefore we can just assume, that the first part is important.
-        command = stmt.expression_list()[0]
-
-        if tup.type == pr.Array.NOARRAY:
-
-                # unnessecary braces -> just remove.
-            r = results
-        else:
-            r = eval_results(i)
-
-        # LHS of tuples can be nested, so resolve it recursively
-        result += find_assignments(command, r, seek_name)
-    return result
-
-
-def find_assignments(lhs, results, seek_name):
-    """
-    Check if `seek_name` is in the left hand side `lhs` of assignment.
-
-    `lhs` can simply be a variable (`pr.Call`) or a tuple/list (`pr.Array`)
-    representing the following cases::
+                try:
+                    new_types += func(index)
+                except IndexError:
+                    pass
+        types = new_types
+    return types
 
-        a = 1        # lhs is pr.Call
-        (a, b) = 2   # lhs is pr.Array
 
-    :type lhs: pr.Call
-    :type results: list
-    :type seek_name: str
-    """
-    if isinstance(lhs, pr.Array):
-        return _assign_tuples(lhs, results, seek_name)
-    elif unicode(lhs.name.names[-1]) == seek_name:
-        return results
+def filter_private_variable(scope, origin_node):
+    """Check if a variable is defined inside the same class or outside."""
+    instance = scope.get_parent_scope()
+    coming_from = origin_node
+    while coming_from is not None \
+            and not isinstance(coming_from, (tree.Class, compiled.CompiledObject)):
+        coming_from = coming_from.get_parent_scope()
+
+    # CompiledObjects don't have double underscore attributes, but Jedi abuses
+    # those for fakes (builtins.pym -> list).
+    if isinstance(instance, compiled.CompiledObject):
+        return instance != coming_from
     else:
-        return []
+        return isinstance(instance, er.Instance) and instance.base.base != coming_from
```

### Comparing `jedi-0.8.1-final0/jedi/evaluate/param.py` & `jedi-0.9.0/jedi/evaluate/param.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,375 +1,403 @@
-import copy
+from collections import defaultdict
+from itertools import chain
 
 from jedi._compatibility import unicode, zip_longest
-from jedi.parser import representation as pr
-from jedi.evaluate import iterable
+from jedi import debug
 from jedi import common
-from jedi.evaluate import helpers
+from jedi.parser import tree
+from jedi.evaluate import iterable
 from jedi.evaluate import analysis
-from jedi.evaluate.compiled import CompiledObject
+from jedi.evaluate import precedence
+from jedi.evaluate.helpers import FakeName
+from jedi.cache import underscore_memoization
+
+
+class Arguments(tree.Base):
+    def __init__(self, evaluator, argument_node, trailer=None):
+        """
+        The argument_node is either a parser node or a list of evaluated
+        objects. Those evaluated objects may be lists of evaluated objects
+        themselves (one list for the first argument, one for the second, etc).
+
+        :param argument_node: May be an argument_node or a list of nodes.
+        """
+        self.argument_node = argument_node
+        self._evaluator = evaluator
+        self.trailer = trailer  # Can be None, e.g. in a class definition.
+
+    def _split(self):
+        if isinstance(self.argument_node, (tuple, list)):
+            for el in self.argument_node:
+                yield 0, el
+        else:
+            if not tree.is_node(self.argument_node, 'arglist'):
+                yield 0, self.argument_node
+                return
+
+            iterator = iter(self.argument_node.children)
+            for child in iterator:
+                if child == ',':
+                    continue
+                elif child in ('*', '**'):
+                    yield len(child.value), next(iterator)
+                else:
+                    yield 0, child
 
+    def get_parent_until(self, *args, **kwargs):
+        if self.trailer is None:
+            try:
+                element = self.argument_node[0]
+                from jedi.evaluate.iterable import AlreadyEvaluated
+                if isinstance(element, AlreadyEvaluated):
+                    element = self._evaluator.eval_element(element)[0]
+            except IndexError:
+                return None
+            else:
+                return element.get_parent_until(*args, **kwargs)
+        else:
+            return self.trailer.get_parent_until(*args, **kwargs)
 
-class ExecutedParam(pr.Param):
-    def __init__(self):
-        """Don't use this method, it's just here to overwrite the old one."""
-        pass
-
-    @classmethod
-    def from_param(cls, param, parent, var_args):
-        instance = cls()
-        before = ()
-        for cls in param.__class__.__mro__:
-            with common.ignored(AttributeError):
-                if before == cls.__slots__:
-                    continue
-                before = cls.__slots__
-                for name in before:
-                    setattr(instance, name, getattr(param, name))
-
-        instance.original_param = param
-        instance.is_generated = True
-        instance.parent = parent
-        instance.var_args = var_args
-        return instance
+    def as_tuple(self):
+        for stars, argument in self._split():
+            if tree.is_node(argument, 'argument'):
+                argument, default = argument.children[::2]
+            else:
+                default = None
+            yield argument, default, stars
+
+    def unpack(self, func=None):
+        named_args = []
+        for stars, el in self._split():
+            if stars == 1:
+                arrays = self._evaluator.eval_element(el)
+                iterators = [_iterate_star_args(self._evaluator, a, el, func)
+                             for a in arrays]
+                iterators = list(iterators)
+                for values in list(zip_longest(*iterators)):
+                    yield None, [v for v in values if v is not None]
+            elif stars == 2:
+                arrays = self._evaluator.eval_element(el)
+                dicts = [_star_star_dict(self._evaluator, a, el, func)
+                         for a in arrays]
+                for dct in dicts:
+                    for key, values in dct.items():
+                        yield key, values
+            else:
+                if tree.is_node(el, 'argument'):
+                    c = el.children
+                    if len(c) == 3:  # Keyword argument.
+                        named_args.append((c[0].value, (c[2],)))
+                    else:  # Generator comprehension.
+                        # Include the brackets with the parent.
+                        comp = iterable.GeneratorComprehension(
+                            self._evaluator, self.argument_node.parent)
+                        yield None, (iterable.AlreadyEvaluated([comp]),)
+                elif isinstance(el, (list, tuple)):
+                    yield None, el
+                else:
+                    yield None, (el,)
+
+        # Reordering var_args is necessary, because star args sometimes appear
+        # after named argument, but in the actual order it's prepended.
+        for key_arg in named_args:
+            yield key_arg
+
+    def _reorder_var_args(var_args):
+        named_index = None
+        new_args = []
+        for i, stmt in enumerate(var_args):
+            if isinstance(stmt, tree.ExprStmt):
+                if named_index is None and stmt.assignment_details:
+                    named_index = i
+
+                if named_index is not None:
+                    expression_list = stmt.expression_list()
+                    if expression_list and expression_list[0] == '*':
+                        new_args.insert(named_index, stmt)
+                        named_index += 1
+                        continue
+
+            new_args.append(stmt)
+        return new_args
+
+    def eval_argument_clinic(self, arguments):
+        """Uses a list with argument clinic information (see PEP 436)."""
+        iterator = self.unpack()
+        for i, (name, optional, allow_kwargs) in enumerate(arguments):
+            key, va_values = next(iterator, (None, []))
+            if key is not None:
+                raise NotImplementedError
+            if not va_values and not optional:
+                debug.warning('TypeError: %s expected at least %s arguments, got %s',
+                              name, len(arguments), i)
+                raise ValueError
+            values = list(chain.from_iterable(self._evaluator.eval_element(el)
+                                              for el in va_values))
+            if not values and not optional:
+                # For the stdlib we always want values. If we don't get them,
+                # that's ok, maybe something is too hard to resolve, however,
+                # we will not proceed with the evaluation of that function.
+                debug.warning('argument_clinic "%s" not resolvable.', name)
+                raise ValueError
+            yield values
+
+    def scope(self):
+        # Returns the scope in which the arguments are used.
+        return (self.trailer or self.argument_node).get_parent_until(tree.IsScope)
+
+    def eval_args(self):
+        # TODO this method doesn't work with named args and a lot of other
+        # things. Use unpack.
+        return [self._evaluator.eval_element(el) for stars, el in self._split()]
+
+    def __repr__(self):
+        return '<%s: %s>' % (type(self).__name__, self.argument_node)
+
+    def get_calling_var_args(self):
+        if tree.is_node(self.argument_node, 'arglist', 'argument') \
+                or self.argument_node == () and self.trailer is not None:
+            return _get_calling_var_args(self._evaluator, self)
+        else:
+            return None
+
+
+class ExecutedParam(tree.Param):
+    """Fake a param and give it values."""
+    def __init__(self, original_param, var_args, values):
+        self._original_param = original_param
+        self.var_args = var_args
+        self._values = values
+
+    def eval(self, evaluator):
+        types = []
+        for v in self._values:
+            types += evaluator.eval_element(v)
+        return types
+
+    @property
+    def position_nr(self):
+        # Need to use the original logic here, because it uses the parent.
+        return self._original_param.position_nr
+
+    @property
+    @underscore_memoization
+    def name(self):
+        return FakeName(str(self._original_param.name), self, self.start_pos)
+
+    def __getattr__(self, name):
+        return getattr(self._original_param, name)
 
 
 def _get_calling_var_args(evaluator, var_args):
     old_var_args = None
     while var_args != old_var_args:
         old_var_args = var_args
-        for argument in reversed(var_args):
-            if not isinstance(argument, pr.Statement):
-                continue
-            exp_list = argument.expression_list()
-            if len(exp_list) != 2 or exp_list[0] not in ('*', '**'):
+        for name, default, stars in reversed(list(var_args.as_tuple())):
+            if not stars or not isinstance(name, tree.Name):
                 continue
 
-            names, _ = evaluator.goto(argument, [exp_list[1].get_code()])
+            names = evaluator.goto(name)
             if len(names) != 1:
                 break
-            param = names[0].parent
+            param = names[0].get_definition()
             if not isinstance(param, ExecutedParam):
-                if isinstance(param, pr.Param):
+                if isinstance(param, tree.Param):
                     # There is no calling var_args in this case - there's just
                     # a param without any input.
                     return None
                 break
             # We never want var_args to be a tuple. This should be enough for
             # now, we can change it later, if we need to.
-            if isinstance(param.var_args, pr.Array):
+            if isinstance(param.var_args, Arguments):
                 var_args = param.var_args
-    return var_args
+    return var_args.argument_node or var_args.trailer
 
 
 def get_params(evaluator, func, var_args):
-    result = []
+    param_names = []
     param_dict = {}
     for param in func.params:
-        param_dict[str(param.get_name())] = param
-    # There may be calls, which don't fit all the params, this just ignores it.
-    unpacked_va = _unpack_var_args(evaluator, var_args, func)
+        param_dict[str(param.name)] = param
+    unpacked_va = list(var_args.unpack(func))
+    from jedi.evaluate.representation import InstanceElement
+    if isinstance(func, InstanceElement):
+        # Include self at this place.
+        unpacked_va.insert(0, (None, [iterable.AlreadyEvaluated([func.instance])]))
     var_arg_iterator = common.PushBackIterator(iter(unpacked_va))
 
-    non_matching_keys = []
-    keys_used = set()
+    non_matching_keys = defaultdict(lambda: [])
+    keys_used = {}
     keys_only = False
-    va_values = None
     had_multiple_value_error = False
     for param in func.params:
         # The value and key can both be null. There, the defaults apply.
         # args / kwargs will just be empty arrays / dicts, respectively.
         # Wrong value count is just ignored. If you try to test cases that are
         # not allowed in Python, Jedi will maybe not show any completions.
-        key, va_values = next(var_arg_iterator, (None, []))
-        while key:
+        default = [] if param.default is None else [param.default]
+        key, va_values = next(var_arg_iterator, (None, default))
+        while key is not None:
             keys_only = True
             k = unicode(key)
             try:
                 key_param = param_dict[unicode(key)]
             except KeyError:
-                non_matching_keys.append((key, va_values))
+                non_matching_keys[key] += va_values
             else:
-                result.append(_gen_param_name_copy(func, var_args, key_param,
-                                                   values=va_values))
+                param_names.append(ExecutedParam(key_param, var_args, va_values).name)
 
             if k in keys_used:
                 had_multiple_value_error = True
                 m = ("TypeError: %s() got multiple values for keyword argument '%s'."
                      % (func.name, k))
                 calling_va = _get_calling_var_args(evaluator, var_args)
                 if calling_va is not None:
                     analysis.add(evaluator, 'type-error-multiple-values',
                                  calling_va, message=m)
             else:
-                keys_used.add(k)
-            key, va_values = next(var_arg_iterator, (None, []))
+                try:
+                    keys_used[k] = param_names[-1]
+                except IndexError:
+                    # TODO this is wrong stupid and whatever.
+                    pass
+            key, va_values = next(var_arg_iterator, (None, ()))
 
-        keys = []
         values = []
-        array_type = None
-        has_default_value = False
         if param.stars == 1:
             # *args param
-            array_type = pr.Array.TUPLE
-            lst_values = [va_values]
+            lst_values = [iterable.MergedNodes(va_values)] if va_values else []
             for key, va_values in var_arg_iterator:
                 # Iterate until a key argument is found.
                 if key:
                     var_arg_iterator.push_back((key, va_values))
                     break
-                lst_values.append(va_values)
-            if lst_values[0]:
-                values = [helpers.stmts_to_stmt(v) for v in lst_values]
+                if va_values:
+                    lst_values.append(iterable.MergedNodes(va_values))
+            seq = iterable.FakeSequence(evaluator, lst_values, 'tuple')
+            values = [iterable.AlreadyEvaluated([seq])]
         elif param.stars == 2:
             # **kwargs param
-            array_type = pr.Array.DICT
-            if non_matching_keys:
-                keys, values = zip(*non_matching_keys)
-                values = [helpers.stmts_to_stmt(list(v)) for v in values]
-            non_matching_keys = []
+            dct = iterable.FakeDict(evaluator, dict(non_matching_keys))
+            values = [iterable.AlreadyEvaluated([dct])]
+            non_matching_keys = {}
         else:
             # normal param
             if va_values:
                 values = va_values
             else:
-                if param.assignment_details:
-                    # No value: Return the default values.
-                    has_default_value = True
-                    result.append(param.get_name())
-                    # TODO is this allowed? it changes it long time.
-                    param.is_generated = True
-                else:
-                    # No value: Return an empty container
-                    values = []
-                    if not keys_only and isinstance(var_args, pr.Array):
-                        calling_va = _get_calling_var_args(evaluator, var_args)
-                        if calling_va is not None:
-                            m = _error_argument_count(func, len(unpacked_va))
-                            analysis.add(evaluator, 'type-error-too-few-arguments',
-                                         calling_va, message=m)
+                # No value: Return an empty container
+                values = []
+                if not keys_only:
+                    calling_va = var_args.get_calling_var_args()
+                    if calling_va is not None:
+                        m = _error_argument_count(func, len(unpacked_va))
+                        analysis.add(evaluator, 'type-error-too-few-arguments',
+                                     calling_va, message=m)
 
         # Now add to result if it's not one of the previously covered cases.
-        if not has_default_value and (not keys_only or param.stars == 2):
-            keys_used.add(unicode(param.get_name()))
-            result.append(_gen_param_name_copy(func, var_args, param,
-                                               keys=keys, values=values,
-                                               array_type=array_type))
+        if (not keys_only or param.stars == 2):
+            param_names.append(ExecutedParam(param, var_args, values).name)
+            keys_used[unicode(param.name)] = param_names[-1]
 
     if keys_only:
         # All arguments should be handed over to the next function. It's not
         # about the values inside, it's about the names. Jedi needs to now that
         # there's nothing to find for certain names.
-        for k in set(param_dict) - keys_used:
+        for k in set(param_dict) - set(keys_used):
             param = param_dict[k]
-            result.append(_gen_param_name_copy(func, var_args, param))
+            values = [] if param.default is None else [param.default]
+            param_names.append(ExecutedParam(param, var_args, values).name)
 
             if not (non_matching_keys or had_multiple_value_error
-                    or param.stars or param.assignment_details):
+                    or param.stars or param.default):
                 # add a warning only if there's not another one.
                 calling_va = _get_calling_var_args(evaluator, var_args)
                 if calling_va is not None:
                     m = _error_argument_count(func, len(unpacked_va))
                     analysis.add(evaluator, 'type-error-too-few-arguments',
                                  calling_va, message=m)
 
-    for key, va_values in non_matching_keys:
+    for key, va_values in non_matching_keys.items():
         m = "TypeError: %s() got an unexpected keyword argument '%s'." \
             % (func.name, key)
         for value in va_values:
-            analysis.add(evaluator, 'type-error-keyword-argument', value, message=m)
+            analysis.add(evaluator, 'type-error-keyword-argument', value.parent, message=m)
 
     remaining_params = list(var_arg_iterator)
     if remaining_params:
         m = _error_argument_count(func, len(unpacked_va))
-        for p in remaining_params[0][1]:
-            analysis.add(evaluator, 'type-error-too-many-arguments',
-                         p, message=m)
-    return result
-
-
-def _unpack_var_args(evaluator, var_args, func):
-    """
-    Yields a key/value pair, the key is None, if its not a named arg.
-    """
-    argument_list = []
-    from jedi.evaluate.representation import InstanceElement
-    if isinstance(func, InstanceElement):
-        # Include self at this place.
-        argument_list.append((None, [helpers.FakeStatement([func.instance])]))
-
-    # `var_args` is typically an Array, and not a list.
-    for stmt in _reorder_var_args(var_args):
-        if not isinstance(stmt, pr.Statement):
-            if stmt is None:
-                argument_list.append((None, []))
-                # TODO generate warning?
-                continue
-            old = stmt
-            # generate a statement if it's not already one.
-            stmt = helpers.FakeStatement([old])
-
-        expression_list = stmt.expression_list()
-        if not len(expression_list):
-            continue
-        # *args
-        if expression_list[0] == '*':
-            arrays = evaluator.eval_expression_list(expression_list[1:])
-            iterators = [_iterate_star_args(evaluator, a, expression_list[1:], func)
-                         for a in arrays]
-            for values in list(zip_longest(*iterators)):
-                argument_list.append((None, [v for v in values if v is not None]))
-        # **kwargs
-        elif expression_list[0] == '**':
-            dct = {}
-            for array in evaluator.eval_expression_list(expression_list[1:]):
-                # Merge multiple kwargs dictionaries, if used with dynamic
-                # parameters.
-                s = _star_star_dict(evaluator, array, expression_list[1:], func)
-                for name, (key, value) in s.items():
-                    try:
-                        dct[name][1].add(value)
-                    except KeyError:
-                        dct[name] = key, set([value])
-
-            for key, values in dct.values():
-                # merge **kwargs/*args also for dynamic parameters
-                for i, p in enumerate(func.params):
-                    if str(p.get_name()) == str(key) and not p.stars:
-                        try:
-                            k, vs = argument_list[i]
-                        except IndexError:
-                            pass
-                        else:
-                            if k is None:  # k would imply a named argument
-                                # Don't merge if they orginate at the same
-                                # place. -> type-error-multiple-values
-                                if [v.parent for v in values] != [v.parent for v in vs]:
-                                    vs.extend(values)
-                                    break
+        # Just report an error for the first param that is not needed (like
+        # cPython).
+        first_key, first_values = remaining_params[0]
+        for v in first_values:
+            if first_key is not None:
+                # Is a keyword argument, return the whole thing instead of just
+                # the value node.
+                v = v.parent
+                try:
+                    non_kw_param = keys_used[first_key]
+                except KeyError:
+                    pass
                 else:
-                    # default is to merge
-                    argument_list.append((key, values))
-        # Normal arguments (including key arguments).
-        else:
-            if stmt.assignment_details:
-                key_arr, op = stmt.assignment_details[0]
-                # Filter error tokens
-                key_arr = [x for x in key_arr if isinstance(x, pr.Call)]
-                # named parameter
-                if key_arr and isinstance(key_arr[0], pr.Call):
-                    argument_list.append((key_arr[0].name, [stmt]))
-            else:
-                argument_list.append((None, [stmt]))
-    return argument_list
-
-
-def _reorder_var_args(var_args):
-    """
-    Reordering var_args is necessary, because star args sometimes appear after
-    named argument, but in the actual order it's prepended.
-    """
-    named_index = None
-    new_args = []
-    for i, stmt in enumerate(var_args):
-        if isinstance(stmt, pr.Statement):
-            if named_index is None and stmt.assignment_details:
-                named_index = i
-
-            if named_index is not None:
-                expression_list = stmt.expression_list()
-                if expression_list and expression_list[0] == '*':
-                    new_args.insert(named_index, stmt)
-                    named_index += 1
-                    continue
-
-        new_args.append(stmt)
-    return new_args
+                    origin_args = non_kw_param.parent.var_args.argument_node
+                    # TODO  calculate the var_args tree and check if it's in
+                    # the tree (if not continue).
+                    # print('\t\tnonkw', non_kw_param.parent.var_args.argument_node, )
+                    if origin_args not in [f.parent.parent for f in first_values]:
+                        continue
+            analysis.add(evaluator, 'type-error-too-many-arguments',
+                         v, message=m)
+    return param_names
 
 
-def _iterate_star_args(evaluator, array, expression_list, func):
+def _iterate_star_args(evaluator, array, input_node, func=None):
     from jedi.evaluate.representation import Instance
     if isinstance(array, iterable.Array):
         for field_stmt in array:  # yield from plz!
             yield field_stmt
     elif isinstance(array, iterable.Generator):
         for field_stmt in array.iter_content():
-            yield helpers.FakeStatement([field_stmt])
-    elif isinstance(array, Instance) and array.name == 'tuple':
-        pass
+            yield iterable.AlreadyEvaluated([field_stmt])
+    elif isinstance(array, Instance) and array.name.get_code() == 'tuple':
+        debug.warning('Ignored a tuple *args input %s' % array)
     else:
-        if expression_list:
+        if func is not None:
             m = "TypeError: %s() argument after * must be a sequence, not %s" \
-                % (func.name, array)
-            analysis.add(evaluator, 'type-error-star',
-                         expression_list[0], message=m)
+                % (func.name.value, array)
+            analysis.add(evaluator, 'type-error-star', input_node, message=m)
 
 
-def _star_star_dict(evaluator, array, expression_list, func):
-    dct = {}
+def _star_star_dict(evaluator, array, input_node, func):
+    dct = defaultdict(lambda: [])
     from jedi.evaluate.representation import Instance
-    if isinstance(array, Instance) and array.name == 'dict':
+    if isinstance(array, Instance) and array.name.get_code() == 'dict':
         # For now ignore this case. In the future add proper iterators and just
         # make one call without crazy isinstance checks.
         return {}
 
-    if isinstance(array, iterable.Array) and array.type == pr.Array.DICT:
-        for key_stmt, value_stmt in array.items():
-            # first index, is the key if syntactically correct
-            call = key_stmt.expression_list()[0]
-            if isinstance(call, pr.Name):
-                key = call
-            elif isinstance(call, pr.Call):
-                key = call.name
-            else:
-                continue  # We ignore complicated statements here, for now.
+    if isinstance(array, iterable.FakeDict):
+        return array._dct
+    elif isinstance(array, iterable.Array) and array.type == 'dict':
+        # TODO bad call to non-public API
+        for key_node, values in array._items():
+            for key in evaluator.eval_element(key_node):
+                if precedence.is_string(key):
+                    dct[key.obj] += values
 
-            # If the string is a duplicate, we don't care it's illegal Python
-            # anyway.
-            dct[str(key)] = key, value_stmt
     else:
-        if expression_list:
+        if func is not None:
             m = "TypeError: %s argument after ** must be a mapping, not %s" \
-                % (func.name, array)
-            analysis.add(evaluator, 'type-error-star-star',
-                         expression_list[0], message=m)
-    return dct
-
-
-def _gen_param_name_copy(func, var_args, param, keys=(), values=(), array_type=None):
-    """
-    Create a param with the original scope (of varargs) as parent.
-    """
-    if isinstance(var_args, pr.Array):
-        parent = var_args.parent
-        start_pos = var_args.start_pos
-    else:
-        parent = func
-        start_pos = 0, 0
-
-    new_param = ExecutedParam.from_param(param, parent, var_args)
-
-    # create an Array (-> needed for *args/**kwargs tuples/dicts)
-    arr = pr.Array(helpers.FakeSubModule, start_pos, array_type, parent)
-    arr.values = list(values)  # Arrays only work with list.
-    key_stmts = []
-    for key in keys:
-        key_stmts.append(helpers.FakeStatement([key], start_pos))
-    arr.keys = key_stmts
-    arr.type = array_type
-
-    new_param.set_expression_list([arr])
-
-    name = copy.copy(param.get_name())
-    name.parent = new_param
-    return name
+                % (func.name.value, array)
+            analysis.add(evaluator, 'type-error-star-star', input_node, message=m)
+    return dict(dct)
 
 
 def _error_argument_count(func, actual_count):
-    default_arguments = sum(1 for p in func.params if p.assignment_details or p.stars)
+    default_arguments = sum(1 for p in func.params if p.default or p.stars)
 
     if default_arguments == 0:
         before = 'exactly '
     else:
         before = 'from %s to ' % (len(func.params) - default_arguments)
     return ('TypeError: %s() takes %s%s arguments (%s given).'
             % (func.name, before, len(func.params), actual_count))
```

### Comparing `jedi-0.8.1-final0/jedi/evaluate/imports.py` & `jedi-0.9.0/jedi/evaluate/imports.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,531 +7,465 @@
 
 This module uses imp for python up to 3.2 and importlib for python 3.3 on; the
 correct implementation is delegated to _compatibility.
 
 This module also supports import autocompletion, which means to complete
 statements like ``from datetim`` (curser at the end would return ``datetime``).
 """
+import imp
 import os
 import pkgutil
 import sys
 from itertools import chain
 
 from jedi._compatibility import find_module, unicode
 from jedi import common
 from jedi import debug
 from jedi import cache
 from jedi.parser import fast
-from jedi.parser import representation as pr
-from jedi.evaluate.sys_path import get_sys_path, sys_path_with_modifications
+from jedi.parser import tree
+from jedi.evaluate import sys_path
 from jedi.evaluate import helpers
 from jedi import settings
 from jedi.common import source_to_unicode
 from jedi.evaluate import compiled
 from jedi.evaluate import analysis
 from jedi.evaluate.cache import memoize_default, NO_DEFAULT
 
 
-class ModuleNotFound(Exception):
-    def __init__(self, name_part):
-        super(ModuleNotFound, self).__init__()
-        self.name_part = name_part
-
-
-class ImportWrapper(pr.Base):
-    """
-    An ImportWrapper is the path of a `pr.Import` object.
-    """
-    class GlobalNamespace(object):
-        def __init__(self):
-            self.line_offset = 0
-
-    GlobalNamespace = GlobalNamespace()
-
-    def __init__(self, evaluator, import_stmt, is_like_search=False, kill_count=0,
-                 nested_resolve=False, is_just_from=False):
-        """
-        :param is_like_search: If the wrapper is used for autocompletion.
-        :param kill_count: Placement of the import, sometimes we only want to
-            resole a part of the import.
-        :param nested_resolve: Resolves nested imports fully.
-        :param is_just_from: Bool if the second part is missing.
-        """
-        self._evaluator = evaluator
-        self.import_stmt = import_stmt
-        self.is_like_search = is_like_search
-        self.nested_resolve = nested_resolve
-        self.is_just_from = is_just_from
-
-        self.is_partial_import = bool(max(0, kill_count))
-
-        # rest is import_path resolution
+def completion_names(evaluator, imp, pos):
+    name = imp.name_for_position(pos)
+    module = evaluator.wrap(imp.get_parent_until())
+    if name is None:
+        level = 0
+        for node in imp.children:
+            if node.end_pos <= pos:
+                if node in ('.', '...'):
+                    level += len(node.value)
         import_path = []
-        if import_stmt.from_ns:
-            import_path += import_stmt.from_ns.names
-        if import_stmt.namespace:
-            if self.import_stmt.is_nested() and not nested_resolve:
-                import_path.append(import_stmt.namespace.names[0])
-            else:
-                import_path += import_stmt.namespace.names
-
-        for i in range(kill_count + int(is_like_search)):
-            if import_path:
-                import_path.pop()
-
-        module = import_stmt.get_parent_until()
-        self._importer = get_importer(self._evaluator, tuple(import_path), module,
-                                      import_stmt.relative_count)
-
-    def __repr__(self):
-        return '<%s: %s>' % (type(self).__name__, self.import_stmt)
-
-    @property
-    def import_path(self):
-        return self._importer.str_import_path()
+    else:
+        # Completion on an existing name.
 
-    def get_defined_names(self, on_import_stmt=False):
-        names = []
-        for scope in self.follow():
-            if scope is ImportWrapper.GlobalNamespace:
-                if not self._is_relative_import():
-                    names += self._get_module_names()
-
-                if self._importer.file_path is not None:
-                    path = os.path.abspath(self._importer.file_path)
-                    for i in range(self.import_stmt.relative_count - 1):
-                        path = os.path.dirname(path)
-                    names += self._get_module_names([path])
-
-                    if self._is_relative_import():
-                        rel_path = os.path.join(self._importer.get_relative_path(),
-                                                '__init__.py')
-                        if os.path.exists(rel_path):
-                            m = _load_module(rel_path)
-                            names += m.get_defined_names()
-            else:
-                if on_import_stmt and isinstance(scope, pr.Module) \
-                        and scope.path.endswith('__init__.py'):
-                    pkg_path = os.path.dirname(scope.path)
-                    paths = self._importer.namespace_packages(pkg_path,
-                                                              self.import_path)
-                    names += self._get_module_names([pkg_path] + paths)
-                if self.is_just_from:
-                    # In the case of an import like `from x.` we don't need to
-                    # add all the variables.
-                    if ('os',) == self.import_path and not self._is_relative_import():
-                        # os.path is a hardcoded exception, because it's a
-                        # ``sys.modules`` modification.
-                        names.append(self._generate_name('path'))
-                    continue
-                from jedi.evaluate import finder
-                for s, scope_names in finder.get_names_of_scope(self._evaluator,
-                                                                scope, include_builtin=False):
-                    for n in scope_names:
-                        if self.import_stmt.from_ns is None \
-                                or self.is_partial_import:
-                                # from_ns must be defined to access module
-                                # values plus a partial import means that there
-                                # is something after the import, which
-                                # automatically implies that there must not be
-                                # any non-module scope.
-                                continue
-                        names.append(n)
-        return names
-
-    def _generate_name(self, name):
-        return helpers.FakeName(name, parent=self.import_stmt)
-
-    def _get_module_names(self, search_path=None):
-        """
-        Get the names of all modules in the search_path. This means file names
-        and not names defined in the files.
-        """
+        # The import path needs to be reduced by one, because we're completing.
+        import_path = imp.path_for_name(name)[:-1]
+        level = imp.level
+
+    importer = Importer(evaluator, tuple(import_path), module, level)
+    if isinstance(imp, tree.ImportFrom):
+        c = imp.children
+        only_modules = c[c.index('import')].start_pos >= pos
+    else:
+        only_modules = True
+    return importer.completion_names(evaluator, only_modules)
 
-        names = []
-        # add builtin module names
-        if search_path is None:
-            names += [self._generate_name(name) for name in sys.builtin_module_names]
 
-        if search_path is None:
-            search_path = self._importer.sys_path_with_modifications()
-        for module_loader, name, is_pkg in pkgutil.iter_modules(search_path):
-            names.append(self._generate_name(name))
-        return names
+class ImportWrapper(tree.Base):
+    def __init__(self, evaluator, name):
+        self._evaluator = evaluator
+        self._name = name
 
-    def _is_relative_import(self):
-        return bool(self.import_stmt.relative_count)
+        self._import = name.get_parent_until(tree.Import)
+        self.import_path = self._import.path_for_name(name)
 
+    @memoize_default()
     def follow(self, is_goto=False):
-        if self._evaluator.recursion_detector.push_stmt(self.import_stmt):
+        if self._evaluator.recursion_detector.push_stmt(self._import):
             # check recursion
             return []
 
-        if self.import_path:
+        try:
+            module = self._evaluator.wrap(self._import.get_parent_until())
+            import_path = self._import.path_for_name(self._name)
+            from_import_name = None
             try:
-                module, rest = self._importer.follow_file_system()
-            except ModuleNotFound as e:
-                analysis.add(self._evaluator, 'import-error', e.name_part)
-                return []
-
-            if self.import_stmt.is_nested() and not self.nested_resolve:
-                scopes = [NestedImportModule(module, self.import_stmt)]
+                from_names = self._import.get_from_names()
+            except AttributeError:
+                # Is an import_name
+                pass
             else:
-                scopes = [module]
-
-            star_imports = remove_star_imports(self._evaluator, module)
-            if star_imports:
-                scopes = [StarImportModule(scopes[0], star_imports)]
-
-            # follow the rest of the import (not FS -> classes, functions)
-            if len(rest) > 1 or rest and self.is_like_search:
-                scopes = []
-                if ('os', 'path') == self.import_path[:2] \
-                        and not self._is_relative_import():
-                    # This is a huge exception, we follow a nested import
-                    # ``os.path``, because it's a very important one in Python
-                    # that is being achieved by messing with ``sys.modules`` in
-                    # ``os``.
-                    scopes = self._evaluator.follow_path(iter(rest), [module], module)
-            elif rest:
+                if len(from_names) + 1 == len(import_path):
+                    # We have to fetch the from_names part first and then check
+                    # if from_names exists in the modules.
+                    from_import_name = import_path[-1]
+                    import_path = from_names
+
+            importer = Importer(self._evaluator, tuple(import_path),
+                                module, self._import.level)
+
+            types = importer.follow()
+
+            #if self._import.is_nested() and not self.nested_resolve:
+            #    scopes = [NestedImportModule(module, self._import)]
+
+            if from_import_name is not None:
+                types = list(chain.from_iterable(
+                    self._evaluator.find_types(t, unicode(from_import_name),
+                                               is_goto=is_goto)
+                    for t in types))
+
+                if not types:
+                    path = import_path + [from_import_name]
+                    importer = Importer(self._evaluator, tuple(path),
+                                        module, self._import.level)
+                    types = importer.follow()
+                    # goto only accepts `Name`
+                    if is_goto:
+                        types = [s.name for s in types]
+            else:
+                # goto only accepts `Name`
                 if is_goto:
-                    scopes = list(chain.from_iterable(
-                        self._evaluator.find_types(s, rest[0], is_goto=True)
-                        for s in scopes))
-                else:
-                    scopes = list(chain.from_iterable(
-                        self._evaluator.follow_path(iter(rest), [s], s)
-                        for s in scopes))
-        else:
-            scopes = [ImportWrapper.GlobalNamespace]
-        debug.dbg('after import: %s', scopes)
-        if not scopes:
-            analysis.add(self._evaluator, 'import-error',
-                         self._importer.import_path[-1])
-        self._evaluator.recursion_detector.pop_stmt()
-        return scopes
+                    types = [s.name for s in types]
+
+            debug.dbg('after import: %s', types)
+        finally:
+            self._evaluator.recursion_detector.pop_stmt()
+        return types
 
 
-class NestedImportModule(pr.Module):
+class NestedImportModule(tree.Module):
+    """
+    TODO while there's no use case for nested import module right now, we might
+        be able to use them for static analysis checks later on.
+    """
     def __init__(self, module, nested_import):
         self._module = module
         self._nested_import = nested_import
 
     def _get_nested_import_name(self):
         """
         Generates an Import statement, that can be used to fake nested imports.
         """
         i = self._nested_import
         # This is not an existing Import statement. Therefore, set position to
         # 0 (0 is not a valid line number).
         zero = (0, 0)
-        names = [unicode(name_part) for name_part in i.namespace.names[1:]]
+        names = [unicode(name) for name in i.namespace_names[1:]]
         name = helpers.FakeName(names, self._nested_import)
-        new = pr.Import(i._sub_module, zero, zero, name)
+        new = tree.Import(i._sub_module, zero, zero, name)
         new.parent = self._module
         debug.dbg('Generated a nested import: %s', new)
-        return helpers.FakeName(str(i.namespace.names[1]), new)
-
-    def _get_defined_names(self):
-        """
-        NesteImportModule don't seem to be actively used, right now.
-        However, they might in the future. If we do more sophisticated static
-        analysis checks.
-        """
-        nested = self._get_nested_import_name()
-        return self._module.get_defined_names() + [nested]
+        return helpers.FakeName(str(i.namespace_names[1]), new)
 
     def __getattr__(self, name):
         return getattr(self._module, name)
 
     def __repr__(self):
         return "<%s: %s of %s>" % (self.__class__.__name__, self._module,
                                    self._nested_import)
 
 
-class StarImportModule(pr.Module):
-    """
-    Used if a module contains star imports.
-    """
-    def __init__(self, module, star_import_modules):
-        self._module = module
-        self.star_import_modules = star_import_modules
-
-    def scope_names_generator(self, position=None):
-        for module, names in self._module.scope_names_generator(position):
-            yield module, names
-        for s in self.star_import_modules:
-            yield s, s.get_defined_names()
-
-    def __getattr__(self, name):
-        return getattr(self._module, name)
-
-    def __repr__(self):
-        return "<%s: %s>" % (self.__class__.__name__, self._module)
+def _add_error(evaluator, name, message=None):
+    if hasattr(name, 'parent'):
+        # Should be a name, not a string!
+        analysis.add(evaluator, 'import-error', name, message)
 
 
-def get_importer(evaluator, import_path, module, level=0):
+def get_init_path(directory_path):
     """
-    Checks the evaluator caches first, which resembles the ``sys.modules``
-    cache and speeds up libraries like ``numpy``.
+    The __init__ file can be searched in a directory. If found return it, else
+    None.
     """
-    if level != 0:
-        # Only absolute imports should be cached. Otherwise we have a mess.
-        # TODO Maybe calculate the absolute import and save it here?
-        return _Importer(evaluator, import_path, module, level)
-    try:
-        return evaluator.import_cache[import_path]
-    except KeyError:
-        importer = _Importer(evaluator, import_path, module, level)
-        evaluator.import_cache[import_path] = importer
-        return importer
+    for suffix, _, _ in imp.get_suffixes():
+        path = os.path.join(directory_path, '__init__' + suffix)
+        if os.path.exists(path):
+            return path
+    return None
 
 
-class _Importer(object):
+class Importer(object):
     def __init__(self, evaluator, import_path, module, level=0):
         """
-        An implementation similar to ``__import__``. Use `follow_file_system`
+        An implementation similar to ``__import__``. Use `follow`
         to actually follow the imports.
 
         *level* specifies whether to use absolute or relative imports. 0 (the
         default) means only perform absolute imports. Positive values for level
         indicate the number of parent directories to search relative to the
         directory of the module calling ``__import__()`` (see PEP 328 for the
         details).
 
-        :param import_path: List of namespaces (strings).
+        :param import_path: List of namespaces (strings or Names).
         """
         debug.speed('import %s' % (import_path,))
         self._evaluator = evaluator
-        self.import_path = import_path
         self.level = level
         self.module = module
-        path = module.path
-        # TODO abspath
-        self.file_path = os.path.dirname(path) if path is not None else None
+        try:
+            self.file_path = module.py__file__()
+        except AttributeError:
+            # Can be None for certain compiled modules like 'builtins'.
+            self.file_path = None
+
+        if level:
+            base = module.py__package__().split('.')
+            if base == ['']:
+                base = []
+            if level > len(base):
+                path = module.py__file__()
+                import_path = list(import_path)
+                for i in range(level):
+                    path = os.path.dirname(path)
+                dir_name = os.path.basename(path)
+                # This is not the proper way to do relative imports. However, since
+                # Jedi cannot be sure about the entry point, we just calculate an
+                # absolute path here.
+                if dir_name:
+                    import_path.insert(0, dir_name)
+                else:
+                    _add_error(self._evaluator, import_path[-1])
+                    import_path = []
+                    # TODO add import error.
+                    debug.warning('Attempted relative import beyond top-level package.')
+            else:
+                # Here we basically rewrite the level to 0.
+                import_path = tuple(base) + import_path
+        self.import_path = import_path
 
+    @property
     def str_import_path(self):
-        """Returns the import path as pure strings instead of NameParts."""
-        return tuple(str(name_part) for name_part in self.import_path)
-
-    def get_relative_path(self):
-        path = self.file_path
-        for i in range(self.level - 1):
-            path = os.path.dirname(path)
-        return path
+        """Returns the import path as pure strings instead of `Name`."""
+        return tuple(str(name) for name in self.import_path)
 
     @memoize_default()
     def sys_path_with_modifications(self):
-        # If you edit e.g. gunicorn, there will be imports like this:
-        # `from gunicorn import something`. But gunicorn is not in the
-        # sys.path. Therefore look if gunicorn is a parent directory, #56.
         in_path = []
-        if self.import_path:
-            parts = self.file_path.split(os.path.sep)
-            for i, p in enumerate(parts):
-                if p == unicode(self.import_path[0]):
-                    new = os.path.sep.join(parts[:i])
-                    in_path.append(new)
-
-        return in_path + sys_path_with_modifications(self._evaluator, self.module)
-
-    def follow(self, evaluator):
-        scope, rest = self.follow_file_system()
-        if rest:
-            # follow the rest of the import (not FS -> classes, functions)
-            return evaluator.follow_path(iter(rest), [scope], scope)
-        return [scope]
+        sys_path_mod = list(sys_path.sys_path_with_modifications(self._evaluator, self.module))
+        if self.file_path is not None:
+            # If you edit e.g. gunicorn, there will be imports like this:
+            # `from gunicorn import something`. But gunicorn is not in the
+            # sys.path. Therefore look if gunicorn is a parent directory, #56.
+            if self.import_path:  # TODO is this check really needed?
+                for path in sys_path.traverse_parents(self.file_path):
+                    if os.path.basename(path) == self.str_import_path[0]:
+                        in_path.append(os.path.dirname(path))
+
+            # Since we know nothing about the call location of the sys.path,
+            # it's a possibility that the current directory is the origin of
+            # the Python execution.
+            sys_path_mod.insert(0, os.path.dirname(self.file_path))
 
-    @memoize_default(NO_DEFAULT)
-    def follow_file_system(self):
-        if self.file_path:
-            sys_path_mod = list(self.sys_path_with_modifications())
-            if not self.module.has_explicit_absolute_import:
-                # If the module explicitly asks for absolute imports,
-                # there's probably a bogus local one.
-                sys_path_mod.insert(0, self.file_path)
-
-            # First the sys path is searched normally and if that doesn't
-            # succeed, try to search the parent directories, because sometimes
-            # Jedi doesn't recognize sys.path modifications (like py.test
-            # stuff).
-            old_path, temp_path = self.file_path, os.path.dirname(self.file_path)
-            while old_path != temp_path:
-                sys_path_mod.append(temp_path)
-                old_path, temp_path = temp_path, os.path.dirname(temp_path)
-        else:
-            sys_path_mod = list(get_sys_path())
+        return in_path + sys_path_mod
 
-        from jedi.evaluate.representation import ModuleWrapper
-        module, rest = self._follow_sys_path(sys_path_mod)
-        if isinstance(module, pr.Module):
-            return ModuleWrapper(self._evaluator, module), rest
-        return module, rest
+    @memoize_default(NO_DEFAULT)
+    def follow(self):
+        if not self.import_path:
+            return []
+        return self._do_import(self.import_path, self.sys_path_with_modifications())
 
-    def namespace_packages(self, found_path, import_path):
+    def _do_import(self, import_path, sys_path):
         """
-        Returns a list of paths of possible ``pkgutil``/``pkg_resources``
-        namespaces. If the package is no "namespace package", an empty list is
-        returned.
+        This method is very similar to importlib's `_gcd_import`.
         """
-        def follow_path(directories, paths):
-            try:
-                directory = next(directories)
-            except StopIteration:
-                return paths
+        import_parts = [str(i) for i in import_path]
+
+        # Handle "magic" Flask extension imports:
+        # ``flask.ext.foo`` is really ``flask_foo`` or ``flaskext.foo``.
+        if len(import_path) > 2 and import_parts[:2] == ['flask', 'ext']:
+            # New style.
+            ipath = ('flask_' + str(import_parts[2]),) + import_path[3:]
+            modules = self._do_import(ipath, sys_path)
+            if modules:
+                return modules
             else:
-                deeper_paths = []
-                for p in paths:
-                    new = os.path.join(p, directory)
-                    if os.path.isdir(new) and new != found_path:
-                        deeper_paths.append(new)
-                return follow_path(directories, deeper_paths)
-
-        with open(os.path.join(found_path, '__init__.py'), 'rb') as f:
-            content = common.source_to_unicode(f.read())
-            # these are strings that need to be used for namespace packages,
-            # the first one is ``pkgutil``, the second ``pkg_resources``.
-            options = ('declare_namespace(__name__)', 'extend_path(__path__')
-            if options[0] in content or options[1] in content:
-                # It is a namespace, now try to find the rest of the modules.
-                return follow_path(iter(import_path), sys.path)
-        return []
+                # Old style
+                return self._do_import(('flaskext',) + import_path[2:], sys_path)
 
-    def _follow_sys_path(self, sys_path):
-        """
-        Find a module with a path (of the module, like usb.backend.libusb10).
-        """
-        def follow_str(ns_path, string):
-            debug.dbg('follow_module %s %s', ns_path, string)
-            path = None
-            if ns_path:
-                path = ns_path
-            elif self.level > 0:  # is a relative import
-                path = self.get_relative_path()
+        module_name = '.'.join(import_parts)
+        try:
+            return [self._evaluator.modules[module_name]]
+        except KeyError:
+            pass
 
-            if path is not None:
-                importing = find_module(string, [path])
+        if len(import_path) > 1:
+            # This is a recursive way of importing that works great with
+            # the module cache.
+            bases = self._do_import(import_path[:-1], sys_path)
+            if not bases:
+                return []
+            # We can take the first element, because only the os special
+            # case yields multiple modules, which is not important for
+            # further imports.
+            base = bases[0]
+
+            # This is a huge exception, we follow a nested import
+            # ``os.path``, because it's a very important one in Python
+            # that is being achieved by messing with ``sys.modules`` in
+            # ``os``.
+            if [str(i) for i in import_path] == ['os', 'path']:
+                return self._evaluator.find_types(base, 'path')
+
+            try:
+                # It's possible that by giving it always the sys path (and not
+                # the __path__ attribute of the parent, we get wrong results
+                # and nested namespace packages don't work.  But I'm not sure.
+                paths = base.py__path__(sys_path)
+            except AttributeError:
+                # The module is not a package.
+                _add_error(self._evaluator, import_path[-1])
+                return []
             else:
-                debug.dbg('search_module %s %s', string, self.file_path)
+                debug.dbg('search_module %s in paths %s', module_name, paths)
+                for path in paths:
+                    # At the moment we are only using one path. So this is
+                    # not important to be correct.
+                    try:
+                        module_file, module_path, is_pkg = \
+                            find_module(import_parts[-1], [path])
+                        break
+                    except ImportError:
+                        module_path = None
+                if module_path is None:
+                    _add_error(self._evaluator, import_path[-1])
+                    return []
+        else:
+            try:
+                debug.dbg('search_module %s in %s', import_parts[-1], self.file_path)
                 # Override the sys.path. It works only good that way.
                 # Injecting the path directly into `find_module` did not work.
                 sys.path, temp = sys_path, sys.path
                 try:
-                    importing = find_module(string)
+                    module_file, module_path, is_pkg = \
+                        find_module(import_parts[-1])
                 finally:
                     sys.path = temp
-
-            return importing
-
-        current_namespace = (None, None, None)
-        # now execute those paths
-        rest = []
-        for i, s in enumerate(self.import_path):
-            try:
-                current_namespace = follow_str(current_namespace[1], unicode(s))
             except ImportError:
-                _continue = False
-                if self.level >= 1 and len(self.import_path) == 1:
-                    # follow `from . import some_variable`
-                    rel_path = self.get_relative_path()
-                    with common.ignored(ImportError):
-                        current_namespace = follow_str(rel_path, '__init__')
-                elif current_namespace[2]:  # is a package
-                    path = self.str_import_path()[:i]
-                    for n in self.namespace_packages(current_namespace[1], path):
-                        try:
-                            current_namespace = follow_str(n, unicode(s))
-                            if current_namespace[1]:
-                                _continue = True
-                                break
-                        except ImportError:
-                            pass
-
-                if not _continue:
-                    if current_namespace[1]:
-                        rest = self.str_import_path()[i:]
-                        break
-                    else:
-                        raise ModuleNotFound(s)
+                # The module is not a package.
+                _add_error(self._evaluator, import_path[-1])
+                return []
 
-        path = current_namespace[1]
-        is_package_directory = current_namespace[2]
+        source = None
+        if is_pkg:
+            # In this case, we don't have a file yet. Search for the
+            # __init__ file.
+            module_path = get_init_path(module_path)
+        elif module_file:
+            source = module_file.read()
+            module_file.close()
 
-        f = None
-        if is_package_directory or current_namespace[0]:
-            # is a directory module
-            if is_package_directory:
-                path = os.path.join(path, '__init__.py')
-                with open(path, 'rb') as f:
-                    source = f.read()
-            else:
-                source = current_namespace[0].read()
-                current_namespace[0].close()
-            return _load_module(path, source, sys_path=sys_path), rest
+        if module_file is None and not module_path.endswith('.py'):
+            module = compiled.load_module(module_path)
         else:
-            return _load_module(name=path, sys_path=sys_path), rest
+            module = _load_module(self._evaluator, module_path, source, sys_path)
 
+        self._evaluator.modules[module_name] = module
+        return [module]
 
-def follow_imports(evaluator, scopes):
-    """
-    Here we strip the imports - they don't get resolved necessarily.
-    Really used anymore? Merge with remove_star_imports?
-    """
-    result = []
-    for s in scopes:
-        if isinstance(s, pr.Import):
-            for r in ImportWrapper(evaluator, s).follow():
-                result.append(r)
-        else:
-            result.append(s)
-    return result
+    def _generate_name(self, name):
+        return helpers.FakeName(name, parent=self.module)
 
+    def _get_module_names(self, search_path=None):
+        """
+        Get the names of all modules in the search_path. This means file names
+        and not names defined in the files.
+        """
 
-@cache.cache_star_import
-def remove_star_imports(evaluator, scope, ignored_modules=()):
-    """
-    Check a module for star imports::
+        names = []
+        # add builtin module names
+        if search_path is None:
+            names += [self._generate_name(name) for name in sys.builtin_module_names]
 
-        from module import *
+        if search_path is None:
+            search_path = self.sys_path_with_modifications()
+        for module_loader, name, is_pkg in pkgutil.iter_modules(search_path):
+            names.append(self._generate_name(name))
+        return names
 
-    and follow these modules.
-    """
-    if isinstance(scope, StarImportModule):
-        return scope.star_import_modules
-    modules = follow_imports(evaluator, (i for i in scope.get_imports() if i.star))
-    new = []
-    for m in modules:
-        if m not in ignored_modules:
-            new += remove_star_imports(evaluator, m, modules)
-    modules += new
+    def completion_names(self, evaluator, only_modules=False):
+        """
+        :param only_modules: Indicates wheter it's possible to import a
+            definition that is not defined in a module.
+        """
+        from jedi.evaluate import finder
+        names = []
+        if self.import_path:
+            # flask
+            if self.str_import_path == ('flask', 'ext'):
+                # List Flask extensions like ``flask_foo``
+                for mod in self._get_module_names():
+                    modname = str(mod)
+                    if modname.startswith('flask_'):
+                        extname = modname[len('flask_'):]
+                        names.append(self._generate_name(extname))
+                # Now the old style: ``flaskext.foo``
+                for dir in self.sys_path_with_modifications():
+                    flaskext = os.path.join(dir, 'flaskext')
+                    if os.path.isdir(flaskext):
+                        names += self._get_module_names([flaskext])
+
+            for scope in self.follow():
+                # Non-modules are not completable.
+                if not scope.type == 'file_input':  # not a module
+                    continue
 
-    # Filter duplicate modules.
-    return set(modules)
+                # namespace packages
+                if isinstance(scope, tree.Module) and scope.path.endswith('__init__.py'):
+                    paths = scope.py__path__(self.sys_path_with_modifications())
+                    names += self._get_module_names(paths)
+
+                if only_modules:
+                    # In the case of an import like `from x.` we don't need to
+                    # add all the variables.
+                    if ('os',) == self.str_import_path and not self.level:
+                        # os.path is a hardcoded exception, because it's a
+                        # ``sys.modules`` modification.
+                        names.append(self._generate_name('path'))
+
+                    continue
+
+                for names_dict in scope.names_dicts(search_global=False):
+                    _names = list(chain.from_iterable(names_dict.values()))
+                    if not _names:
+                        continue
+                    _names = finder.filter_definition_names(_names, scope)
+                    names += _names
+        else:
+            # Empty import path=completion after import
+            if not self.level:
+                names += self._get_module_names()
+
+            if self.file_path is not None:
+                path = os.path.abspath(self.file_path)
+                for i in range(self.level - 1):
+                    path = os.path.dirname(path)
+                names += self._get_module_names([path])
+
+        return names
 
 
-def _load_module(path=None, source=None, name=None, sys_path=None):
+def _load_module(evaluator, path=None, source=None, sys_path=None):
     def load(source):
         dotted_path = path and compiled.dotted_from_fs_path(path, sys_path)
         if path is not None and path.endswith('.py') \
                 and not dotted_path in settings.auto_import_modules:
             if source is None:
                 with open(path, 'rb') as f:
                     source = f.read()
         else:
-            return compiled.load_module(path, name)
-        p = path or name
-        p = fast.FastParser(common.source_to_unicode(source), p)
-        cache.save_parser(path, name, p)
+            return compiled.load_module(path)
+        p = path
+        p = fast.FastParser(evaluator.grammar, common.source_to_unicode(source), p)
+        cache.save_parser(path, p)
         return p.module
 
-    cached = cache.load_parser(path, name)
-    return load(source) if cached is None else cached.module
+    cached = cache.load_parser(path)
+    module = load(source) if cached is None else cached.module
+    module = evaluator.wrap(module)
+    return module
+
+
+def add_module(evaluator, module_name, module):
+    if '.' not in module_name:
+        # We cannot add paths with dots, because that would collide with
+        # the sepatator dots for nested packages. Therefore we return
+        # `__main__` in ModuleWrapper.py__name__(), which is similar to
+        # Python behavior.
+        evaluator.modules[module_name] = module
 
 
-def get_modules_containing_name(mods, name):
+def get_modules_containing_name(evaluator, mods, name):
     """
     Search a name in the directories of modules.
     """
     def check_python_file(path):
         try:
             return cache.parser_cache[path].parser.module
         except KeyError:
@@ -540,15 +474,18 @@
             except IOError:
                 return None
 
     def check_fs(path):
         with open(path, 'rb') as f:
             source = source_to_unicode(f.read())
             if name in source:
-                return _load_module(path, source)
+                module_name = os.path.basename(path)[:-3]  # Remove `.py`.
+                module = _load_module(evaluator, path, source)
+                add_module(evaluator, module_name, module)
+                return module
 
     # skip non python modules
     mods = set(m for m in mods if not isinstance(m, compiled.CompiledObject))
     mod_paths = set()
     for m in mods:
         mod_paths.add(m.path)
         yield m
@@ -562,9 +499,9 @@
                     if entry not in mod_paths:
                         if entry.endswith('.py'):
                             paths.add(d + os.path.sep + entry)
 
         for p in sorted(paths):
             # make testing easier, sort it - same results on every interpreter
             c = check_python_file(p)
-            if c is not None and c not in mods:
+            if c is not None and c not in mods and not isinstance(c, compiled.CompiledObject):
                 yield c
```

### Comparing `jedi-0.8.1-final0/jedi/evaluate/cache.py` & `jedi-0.9.0/jedi/evaluate/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 - the popular ``memoize_default`` works like a typical memoize and returns the
   default otherwise.
 - ``CachedMetaClass`` uses ``memoize_default`` to do the same with classes.
 """
 
+import inspect
+
 NO_DEFAULT = object()
 
 
-def memoize_default(default=None, evaluator_is_first_arg=False, second_arg_is_evaluator=False):
+def memoize_default(default=NO_DEFAULT, evaluator_is_first_arg=False, second_arg_is_evaluator=False):
     """ This is a typical memoization decorator, BUT there is one difference:
     To prevent recursion it sets defaults.
 
     Preventing recursion is in this case the much bigger use than speed. I
     don't think, that there is a big speed difference, but there are many cases
     where recursion could happen (think about a = b; b = a).
     """
@@ -33,22 +35,24 @@
             key = (obj, args, frozenset(kwargs.items()))
             if key in memo:
                 return memo[key]
             else:
                 if default is not NO_DEFAULT:
                     memo[key] = default
                 rv = function(obj, *args, **kwargs)
+                if inspect.isgenerator(rv):
+                    rv = list(rv)
                 memo[key] = rv
                 return rv
         return wrapper
     return func
 
 
 class CachedMetaClass(type):
     """
     This is basically almost the same than the decorator above, it just caches
-    class initializations. I haven't found any other way, so I'm doing it with
-    meta classes.
+    class initializations. Either you do it this way or with decorators, but
+    with decorators you lose class access (isinstance, etc).
     """
     @memoize_default(None, second_arg_is_evaluator=True)
     def __call__(self, *args, **kwargs):
         return super(CachedMetaClass, self).__call__(*args, **kwargs)
```

### Comparing `jedi-0.8.1-final0/jedi/__init__.py` & `jedi-0.9.0/jedi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
-Jedi is an autocompletion tool for Python that can be used in IDEs/editors.
-Jedi works. Jedi is fast. It understands all of the basic Python syntax
-elements including many builtin functions.
-
-Additionaly, Jedi suports two different goto functions and has support for
-renaming as well as Pydoc support and some other IDE features.
+Jedi is a static analysis tool for Python that can be used in IDEs/editors. Its
+historic focus is autocompletion, but does static analysis for now as well.
+Jedi is fast and is very well tested. It understands Python on a deeper level
+than all other static analysis frameworks for Python.
+
+Jedi has support for two different goto functions. It's possible to search for
+related names and to list all names in a Python file and infer them. Jedi
+understands docstrings and you can use Jedi autocompletion in your REPL as
+well.
 
 Jedi uses a very simple API to connect with IDE's. There's a reference
-implementation as a `VIM-Plugin <http://github.com/davidhalter/jedi-vim>`_,
-which uses Jedi's autocompletion.  I encourage you to use Jedi in your IDEs.
-It's really easy. If there are any problems (also with licensing), just contact
-me.
+implementation as a `VIM-Plugin <https://github.com/davidhalter/jedi-vim>`_,
+which uses Jedi's autocompletion.  We encourage you to use Jedi in your IDEs.
+It's really easy.
 
 To give you a simple example how you can use the Jedi library, here is an
 example for the autocompletion feature:
 
 >>> import jedi
 >>> source = '''
 ... import datetime
@@ -30,12 +32,12 @@
 >>> print(completions[0].name)
 date
 
 As you see Jedi is pretty simple and allows you to concentrate on writing a
 good text editor, while still having very good IDE features for Python.
 """
 
-__version__ = '0.8.1-final0'
+__version__ = '0.9.0'
 
 from jedi.api import Script, Interpreter, NotFoundError, set_debug_function
-from jedi.api import preload_module, defined_names
+from jedi.api import preload_module, defined_names, names
 from jedi import settings
```

### Comparing `jedi-0.8.1-final0/jedi/__main__.py` & `jedi-0.9.0/jedi/__main__.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/jedi/parser/tokenize.py` & `jedi-0.9.0/jedi/parser/tokenize.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,103 +10,34 @@
 memory optimizations here.
 """
 from __future__ import absolute_import
 
 import string
 import re
 from io import StringIO
-from token import (tok_name, N_TOKENS, ENDMARKER, STRING, NUMBER, NAME, OP,
-                   ERRORTOKEN, NEWLINE)
+from jedi.parser.token import (tok_name, N_TOKENS, ENDMARKER, STRING, NUMBER,
+                               NAME, OP, ERRORTOKEN, NEWLINE, INDENT, DEDENT)
+from jedi._compatibility import is_py3
 
-from jedi._compatibility import u
 
 cookie_re = re.compile("coding[:=]\s*([-\w.]+)")
 
 
-# From here on we have custom stuff (everything before was originally Python
-# internal code).
-FLOWS = ['if', 'else', 'elif', 'while', 'with', 'try', 'except', 'finally']
-
-
-namechars = string.ascii_letters + '_'
+if is_py3:
+    # Python 3 has str.isidentifier() to check if a char is a valid identifier
+    is_identifier = str.isidentifier
+else:
+    namechars = string.ascii_letters + '_'
+    is_identifier = lambda s: s in namechars
 
 
 COMMENT = N_TOKENS
 tok_name[COMMENT] = 'COMMENT'
 
 
-class Token(object):
-    """
-    The token object is an efficient representation of the structure
-    (type, token, (start_pos_line, start_pos_col)). It has indexer
-    methods that maintain compatibility to existing code that expects the above
-    structure.
-
-    >>> repr(Token(1, "test", (1, 1)))
-    "<Token: ('NAME', 'test', (1, 1))>"
-    >>> Token(1, 'bar', (3, 4)).__getstate__()
-    (1, 'bar', 3, 4)
-    >>> a = Token(0, 'baz', (0, 0))
-    >>> a.__setstate__((1, 'foo', 3, 4))
-    >>> a
-    <Token: ('NAME', 'foo', (3, 4))>
-    >>> a.start_pos
-    (3, 4)
-    >>> a.string
-    'foo'
-    >>> a._start_pos_col
-    4
-    >>> Token(1, u("😷"), (1 ,1)).string + "p" == u("😷p")
-    True
-    """
-    __slots__ = ("type", "string", "_start_pos_line", "_start_pos_col")
-
-    def __init__(self, type, string, start_pos):
-        self.type = type
-        self.string = string
-        self._start_pos_line = start_pos[0]
-        self._start_pos_col = start_pos[1]
-
-    def __repr__(self):
-        typ = tok_name[self.type]
-        content = typ, self.string, (self._start_pos_line, self._start_pos_col)
-        return "<%s: %s>" % (type(self).__name__, content)
-
-    @property
-    def start_pos(self):
-        return (self._start_pos_line, self._start_pos_col)
-
-    @property
-    def end_pos(self):
-        """Returns end position respecting multiline tokens."""
-        end_pos_line = self._start_pos_line
-        lines = self.string.split('\n')
-        if self.string.endswith('\n'):
-            lines = lines[:-1]
-            lines[-1] += '\n'
-        end_pos_line += len(lines) - 1
-        end_pos_col = self._start_pos_col
-        # Check for multiline token
-        if self._start_pos_line == end_pos_line:
-            end_pos_col += len(lines[-1])
-        else:
-            end_pos_col = len(lines[-1])
-        return (end_pos_line, end_pos_col)
-
-    # Make cache footprint smaller for faster unpickling
-    def __getstate__(self):
-        return (self.type, self.string, self._start_pos_line, self._start_pos_col)
-
-    def __setstate__(self, state):
-        self.type = state[0]
-        self.string = state[1]
-        self._start_pos_line = state[2]
-        self._start_pos_col = state[3]
-
-
 def group(*choices):
     return '(' + '|'.join(choices) + ')'
 
 
 def maybe(*choices):
     return group(*choices) + '?'
 
@@ -133,15 +64,15 @@
 single = r"[^'\\]*(?:\\.[^'\\]*)*'"
 # Tail end of " string.
 double = r'[^"\\]*(?:\\.[^"\\]*)*"'
 # Tail end of ''' string.
 single3 = r"[^'\\]*(?:(?:\\.|'(?!''))[^'\\]*)*'''"
 # Tail end of """ string.
 double3 = r'[^"\\]*(?:(?:\\.|"(?!""))[^"\\]*)*"""'
-triple = group("[bB]?[rR]?'''", '[bB]?[rR]?"""')
+triple = group("[uUbB]?[rR]?'''", '[uUbB]?[rR]?"""')
 # Single-line ' or " string.
 
 # Because of leftmost-then-longest match semantics, be sure to put the
 # longest operators first (e.g., if = came before ==, == would get
 # recognized as two instances of =).
 operator = group(r"\*\*=?", r">>=?", r"<<=?", r"!=",
                  r"//=?", r"->",
@@ -154,146 +85,206 @@
 
 # First (or only) line of ' or " string.
 cont_str = group(r"[bBuU]?[rR]?'[^\n'\\]*(?:\\.[^\n'\\]*)*" +
                  group("'", r'\\\r?\n'),
                  r'[bBuU]?[rR]?"[^\n"\\]*(?:\\.[^\n"\\]*)*' +
                  group('"', r'\\\r?\n'))
 pseudo_extras = group(r'\\\r?\n', comment, triple)
-pseudo_token = whitespace + group(pseudo_extras, number, funny, cont_str, name)
+pseudo_token = group(whitespace) + \
+    group(pseudo_extras, number, funny, cont_str, name)
 
 
 def _compile(expr):
     return re.compile(expr, re.UNICODE)
 
 
 pseudoprog, single3prog, double3prog = map(
     _compile, (pseudo_token, single3, double3))
+
 endprogs = {"'": _compile(single), '"': _compile(double),
             "'''": single3prog, '"""': double3prog,
             "r'''": single3prog, 'r"""': double3prog,
             "b'''": single3prog, 'b"""': double3prog,
             "u'''": single3prog, 'u"""': double3prog,
-            "br'''": single3prog, 'br"""': double3prog,
             "R'''": single3prog, 'R"""': double3prog,
             "B'''": single3prog, 'B"""': double3prog,
             "U'''": single3prog, 'U"""': double3prog,
+            "br'''": single3prog, 'br"""': double3prog,
             "bR'''": single3prog, 'bR"""': double3prog,
             "Br'''": single3prog, 'Br"""': double3prog,
             "BR'''": single3prog, 'BR"""': double3prog,
+            "ur'''": single3prog, 'ur"""': double3prog,
+            "uR'''": single3prog, 'uR"""': double3prog,
+            "Ur'''": single3prog, 'Ur"""': double3prog,
+            "UR'''": single3prog, 'UR"""': double3prog,
             'r': None, 'R': None, 'b': None, 'B': None}
 
 triple_quoted = {}
 for t in ("'''", '"""',
           "r'''", 'r"""', "R'''", 'R"""',
           "b'''", 'b"""', "B'''", 'B"""',
           "u'''", 'u"""', "U'''", 'U"""',
           "br'''", 'br"""', "Br'''", 'Br"""',
-          "bR'''", 'bR"""', "BR'''", 'BR"""'):
+          "bR'''", 'bR"""', "BR'''", 'BR"""',
+          "ur'''", 'ur"""', "Ur'''", 'Ur"""',
+          "uR'''", 'uR"""', "UR'''", 'UR"""'):
     triple_quoted[t] = t
 single_quoted = {}
 for t in ("'", '"',
           "r'", 'r"', "R'", 'R"',
           "b'", 'b"', "B'", 'B"',
-          "u'", 'u""', "U'", 'U"',
+          "u'", 'u"', "U'", 'U"',
           "br'", 'br"', "Br'", 'Br"',
-          "bR'", 'bR"', "BR'", 'BR"'):
+          "bR'", 'bR"', "BR'", 'BR"',
+          "ur'", 'ur"', "Ur'", 'Ur"',
+          "uR'", 'uR"', "UR'", 'UR"'):
     single_quoted[t] = t
 
 del _compile
 
 tabsize = 8
 
+ALWAYS_BREAK_TOKENS = (';', 'import', 'from', 'class', 'def', 'try', 'except',
+                       'finally', 'while', 'return')
 
-def source_tokens(source, line_offset=0):
+
+def source_tokens(source):
     """Generate tokens from a the source code (string)."""
     source = source + '\n'  # end with \n, because the parser needs it
     readline = StringIO(source).readline
-    return generate_tokens(readline, line_offset)
+    return generate_tokens(readline)
 
 
-def generate_tokens(readline, line_offset=0):
+def generate_tokens(readline):
     """
-    The original stdlib Python version with minor modifications.
-    Modified to not care about dedents.
+    A heavily modified Python standard library tokenizer.
+
+    Additionally to the default information, yields also the prefix of each
+    token. This idea comes from lib2to3. The prefix contains all information
+    that is irrelevant for the parser like newlines in parentheses or comments.
     """
-    lnum = line_offset
+    paren_level = 0  # count parentheses
+    indents = [0]
+    lnum = 0
     numchars = '0123456789'
     contstr = ''
     contline = None
-    while True:             # loop over lines in stream
-        line = readline()  # readline returns empty if it's finished. See StringIO
+    # We start with a newline. This makes indent at the first position
+    # possible. It's not valid Python, but still better than an INDENT in the
+    # second line (and not in the first). This makes quite a few things in
+    # Jedi's fast parser possible.
+    new_line = True
+    prefix = ''  # Should never be required, but here for safety
+    additional_prefix = ''
+    while True:            # loop over lines in stream
+        line = readline()  # readline returns empty when finished. See StringIO
         if not line:
             if contstr:
-                yield Token(ERRORTOKEN, contstr, contstr_start)
+                yield ERRORTOKEN, contstr, contstr_start, prefix
             break
 
         lnum += 1
         pos, max = 0, len(line)
 
         if contstr:                                         # continued string
             endmatch = endprog.match(line)
             if endmatch:
                 pos = endmatch.end(0)
-                yield Token(STRING, contstr + line[:pos], contstr_start)
+                yield STRING, contstr + line[:pos], contstr_start, prefix
                 contstr = ''
                 contline = None
             else:
                 contstr = contstr + line
                 contline = contline + line
                 continue
 
         while pos < max:
             pseudomatch = pseudoprog.match(line, pos)
             if not pseudomatch:                             # scan for tokens
                 txt = line[pos]
                 if line[pos] in '"\'':
                     # If a literal starts but doesn't end the whole rest of the
                     # line is an error token.
-                    txt = txt = line[pos:]
-                yield Token(ERRORTOKEN, txt, (lnum, pos))
+                    txt = line[pos:]
+                yield ERRORTOKEN, txt, (lnum, pos), prefix
                 pos += 1
                 continue
 
-            start, pos = pseudomatch.span(1)
+            prefix = additional_prefix + pseudomatch.group(1)
+            additional_prefix = ''
+            start, pos = pseudomatch.span(2)
             spos = (lnum, start)
             token, initial = line[start:pos], line[start]
 
+            if new_line and initial not in '\r\n#':
+                new_line = False
+                if paren_level == 0:
+                    if start > indents[-1]:
+                        yield INDENT, '', spos, ''
+                        indents.append(start)
+                    while start < indents[-1]:
+                        yield DEDENT, '', spos, ''
+                        indents.pop()
+
             if (initial in numchars or                      # ordinary number
                     (initial == '.' and token != '.' and token != '...')):
-                yield Token(NUMBER, token, spos)
+                yield NUMBER, token, spos, prefix
             elif initial in '\r\n':
-                yield Token(NEWLINE, token, spos)
-            elif initial == '#':
+                if not new_line and paren_level == 0:
+                    yield NEWLINE, token, spos, prefix
+                else:
+                    additional_prefix = prefix + token
+                new_line = True
+            elif initial == '#':  # Comments
                 assert not token.endswith("\n")
-                yield Token(COMMENT, token, spos)
+                additional_prefix = prefix + token
             elif token in triple_quoted:
                 endprog = endprogs[token]
                 endmatch = endprog.match(line, pos)
                 if endmatch:                                # all on one line
                     pos = endmatch.end(0)
                     token = line[start:pos]
-                    yield Token(STRING, token, spos)
+                    yield STRING, token, spos, prefix
                 else:
-                    contstr_start = (lnum, start)                # multiple lines
+                    contstr_start = (lnum, start)           # multiple lines
                     contstr = line[start:]
                     contline = line
                     break
             elif initial in single_quoted or \
                     token[:2] in single_quoted or \
                     token[:3] in single_quoted:
                 if token[-1] == '\n':                       # continued string
                     contstr_start = lnum, start
-                    endprog = (endprogs[initial] or endprogs[token[1]] or
-                               endprogs[token[2]])
+                    endprog = (endprogs.get(initial) or endprogs.get(token[1])
+                               or endprogs.get(token[2]))
                     contstr = line[start:]
                     contline = line
                     break
                 else:                                       # ordinary string
-                    yield Token(STRING, token, spos)
-            elif initial in namechars:                      # ordinary name
-                yield Token(NAME, token, spos)
-            elif initial == '\\' and line[start:] == '\\\n':  # continued stmt
-                continue
+                    yield STRING, token, spos, prefix
+            elif is_identifier(initial):                      # ordinary name
+                if token in ALWAYS_BREAK_TOKENS:
+                    paren_level = 0
+                    while True:
+                        indent = indents.pop()
+                        if indent > start:
+                            yield DEDENT, '', spos, ''
+                        else:
+                            indents.append(indent)
+                            break
+                yield NAME, token, spos, prefix
+            elif initial == '\\' and line[start:] in ('\\\n', '\\\r\n'):  # continued stmt
+                additional_prefix += prefix + line[start:]
+                break
             else:
-                yield Token(OP, token, spos)
-
-    yield Token(ENDMARKER, '', (lnum, 0))
+                if token in '([{':
+                    paren_level += 1
+                elif token in ')]}':
+                    paren_level -= 1
+                yield OP, token, spos, prefix
+
+    end_pos = (lnum, max - 1)
+    # As the last position we just take the maximally possible position. We
+    # remove -1 for the last new line.
+    for indent in indents[1:]:
+        yield DEDENT, '', end_pos, ''
+    yield ENDMARKER, '', end_pos, prefix
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jedi-0.8.1-final0/jedi/utils.py` & `jedi-0.9.0/jedi/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,11 +104,11 @@
 
 
 def version_info():
     """
     Returns a namedtuple of Jedi's version, similar to Python's
     ``sys.version_info``.
     """
-    Version = namedtuple('Version', 'major, minor, micro, releaselevel, serial')
+    Version = namedtuple('Version', 'major, minor, micro')
     from jedi import __version__
     tupl = re.findall('[a-z]+|\d+', __version__)
     return Version(*[x if i == 3 else int(x) for i, x in enumerate(tupl)])
```

### Comparing `jedi-0.8.1-final0/jedi/refactoring.py` & `jedi-0.9.0/jedi/refactoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 - extract variable
 - inline variable
 """
 import difflib
 
 from jedi import common
 from jedi.evaluate import helpers
-from jedi.parser import representation as pr
+from jedi.parser import tree as pt
 
 
 class Refactoring(object):
     def __init__(self, change_dct):
         """
         :param change_dct: dict(old_path=(new_path, old_lines, new_lines))
         """
```

### Comparing `jedi-0.8.1-final0/jedi/_compatibility.py` & `jedi-0.9.0/jedi/_compatibility.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 is_py26 = not is_py3 and sys.version_info[1] < 7
 
 
 def find_module_py33(string, path=None):
     loader = importlib.machinery.PathFinder.find_module(string, path)
 
     if loader is None and path is None:  # Fallback to find builtins
-        loader = importlib.find_loader(string)
+        try:
+            loader = importlib.find_loader(string)
+        except ValueError as e:
+            # See #491. Importlib might raise a ValueError, to avoid this, we
+            # just raise an ImportError to fix the issue.
+            raise ImportError("Originally ValueError: " + e.message)
 
     if loader is None:
         raise ImportError("Couldn't find a loader for {0}".format(string))
 
     try:
         is_package = loader.is_package(string)
         if is_package:
@@ -61,31 +66,14 @@
 This function isolates the differences in importing libraries introduced with
 python 3.3 on; it gets a module name and optionally a path. It will return a
 tuple containin an open file for the module (if not builtin), the filename
 or the name of the module if it is a builtin one and a boolean indicating
 if the module is contained in a package.
 """
 
-# next was defined in python 2.6, in python 3 obj.next won't be possible
-# anymore
-try:
-    next = next
-except NameError:
-    _raiseStopIteration = object()
-
-    def next(iterator, default=_raiseStopIteration):
-        if not hasattr(iterator, 'next'):
-            raise TypeError("not an iterator")
-        try:
-            return iterator.next()
-        except StopIteration:
-            if default is _raiseStopIteration:
-                raise
-            else:
-                return default
 
 # unicode function
 try:
     unicode = unicode
 except NameError:
     unicode = str
 
@@ -121,26 +109,14 @@
 
 Usage::
 
     reraise(Exception, sys.exc_info()[2])
 
 """
 
-# hasattr function used because python
-if is_py3:
-    hasattr = hasattr
-else:
-    def hasattr(obj, name):
-        try:
-            getattr(obj, name)
-            return True
-        except AttributeError:
-            return False
-
-
 class Python3Method(object):
     def __init__(self, func):
         self.func = func
 
     def __get__(self, obj, objtype):
         if obj is None:
             return lambda *args, **kwargs: self.func(*args, **kwargs)
@@ -193,7 +169,37 @@
     return ast.literal_eval(string)
 
 
 try:
     from itertools import zip_longest
 except ImportError:
     from itertools import izip_longest as zip_longest  # Python 2
+
+
+def no_unicode_pprint(dct):
+    """
+    Python 2/3 dict __repr__ may be different, because of unicode differens
+    (with or without a `u` prefix). Normally in doctests we could use `pprint`
+    to sort dicts and check for equality, but here we have to write a separate
+    function to do that.
+    """
+    import pprint
+    s = pprint.pformat(dct)
+    print(re.sub("u'", "'", s))
+
+
+def utf8_repr(func):
+    """
+    ``__repr__`` methods in Python 2 don't allow unicode objects to be
+    returned. Therefore cast them to utf-8 bytes in this decorator.
+    """
+    def wrapper(self):
+        result = func(self)
+        if isinstance(result, unicode):
+            return result.encode('utf-8')
+        else:
+            return result
+
+    if is_py3:
+        return func
+    else:
+        return wrapper
```

### Comparing `jedi-0.8.1-final0/jedi/common.py` & `jedi-0.9.0/jedi/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 """ A universal module with functions / classes without dependencies. """
 import sys
 import contextlib
 import functools
 import re
 from ast import literal_eval
 
-from jedi._compatibility import unicode, next, reraise
+from jedi._compatibility import unicode, reraise
 from jedi import settings
 
 
-class MultiLevelStopIteration(Exception):
-    """
-    StopIteration's get catched pretty easy by for loops, let errors propagate.
-    """
-
-
 class UncaughtAttributeError(Exception):
     """
     Important, because `__getattr__` and `hasattr` catch AttributeErrors
     implicitly. This is really evil (mainly because of `__getattr__`).
     `hasattr` in Python 2 is even more evil, because it catches ALL exceptions.
     Therefore this class originally had to be derived from `BaseException`
     instead of `Exception`.  But because I removed relevant `hasattr` from
@@ -88,17 +82,19 @@
 
 @contextlib.contextmanager
 def scale_speed_settings(factor):
     a = settings.max_executions
     b = settings.max_until_execution_unique
     settings.max_executions *= factor
     settings.max_until_execution_unique *= factor
-    yield
-    settings.max_executions = a
-    settings.max_until_execution_unique = b
+    try:
+        yield
+    finally:
+        settings.max_executions = a
+        settings.max_until_execution_unique = b
 
 
 def indent_block(text, indention='    '):
     """This function indents a text block with a default of four spaces."""
     temp = ''
     while text and text[-1] == '\n':
         temp += text[-1]
```

### Comparing `jedi-0.8.1-final0/jedi/settings.py` & `jedi-0.9.0/jedi/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 .. autodata:: fast_parser
 
 
 Dynamic stuff
 ~~~~~~~~~~~~~
 
-.. autodata:: dynamic_arrays_instances
 .. autodata:: dynamic_array_additions
 .. autodata:: dynamic_params
 .. autodata:: dynamic_params_for_other_modules
 .. autodata:: additional_dynamic_modules
 .. autodata:: auto_import_modules
 
 
@@ -144,22 +143,17 @@
 function is being reparsed.
 """
 
 # ----------------
 # dynamic stuff
 # ----------------
 
-dynamic_arrays_instances = True
-"""
-Check for `append`, etc. on array instances like list()
-"""
-
 dynamic_array_additions = True
 """
-check for `append`, etc. on arrays: [], {}, ()
+check for `append`, etc. on arrays: [], {}, () as well as list/set calls.
 """
 
 dynamic_params = True
 """
 A dynamic param completion, finds the callees of the function, which define
 the params of a function.
 """
```

### Comparing `jedi-0.8.1-final0/jedi/debug.py` & `jedi-0.9.0/jedi/debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from jedi._compatibility import encoding, is_py3
+from jedi._compatibility import encoding, is_py3, u
 import inspect
 import os
 import time
 
 try:
     if os.name == 'nt':
         # does not work on Windows, as pyreadline and colorama interfere
@@ -44,34 +44,36 @@
 
 
 def increase_indent(func):
     """Decorator for makin """
     def wrapper(*args, **kwargs):
         global _debug_indent
         _debug_indent += 1
-        result = func(*args, **kwargs)
-        _debug_indent -= 1
+        try:
+            result = func(*args, **kwargs)
+        finally:
+            _debug_indent -= 1
         return result
     return wrapper
 
 
 def dbg(message, *args):
     """ Looks at the stack, to see if a debug message should be printed. """
     if debug_function and enable_notice:
         frm = inspect.stack()[1]
         mod = inspect.getmodule(frm[0])
         if not (mod.__name__ in ignored_modules):
             i = ' ' * _debug_indent
-            debug_function(NOTICE, i + 'dbg: ' + message % args)
+            debug_function(NOTICE, i + 'dbg: ' + message % tuple(u(repr(a)) for a in args))
 
 
 def warning(message, *args):
     if debug_function and enable_warning:
         i = ' ' * _debug_indent
-        debug_function(WARNING, i + 'warning: ' + message % args)
+        debug_function(WARNING, i + 'warning: ' + message % tuple(u(repr(a)) for a in args))
 
 
 def speed(name):
     if debug_function and enable_speed:
         now = time.time()
         i = ' ' * _debug_indent
         debug_function(SPEED, i + 'speed: ' + '%s %s' % (name, now - _start_time))
```

### Comparing `jedi-0.8.1-final0/jedi/api/__init__.py` & `jedi-0.9.0/jedi/api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 """
 The API basically only provides one class. You can create a :class:`Script` and
 use its methods.
 
-Additionally you can add a debug function with :func:`set_debug_function` and
-catch :exc:`NotFoundError` which is being raised if your completion is not
-possible.
+Additionally you can add a debug function with :func:`set_debug_function`.
 
 .. warning:: Please, note that Jedi is **not thread safe**.
 """
 import re
 import os
 import warnings
 import sys
 from itertools import chain
 
-from jedi._compatibility import next, unicode, builtins
-from jedi.parser import Parser
+from jedi._compatibility import unicode, builtins
+from jedi.parser import Parser, load_grammar
 from jedi.parser.tokenize import source_tokens
-from jedi.parser import representation as pr
+from jedi.parser import tree
 from jedi.parser.user_context import UserContext, UserContextParser
 from jedi import debug
 from jedi import settings
 from jedi import common
 from jedi import cache
 from jedi.api import keywords
 from jedi.api import classes
 from jedi.api import interpreter
 from jedi.api import usages
 from jedi.api import helpers
-from jedi.evaluate import Evaluator, filter_private_variable
+from jedi.evaluate import Evaluator
 from jedi.evaluate import representation as er
 from jedi.evaluate import compiled
 from jedi.evaluate import imports
-from jedi.evaluate.helpers import FakeName
-from jedi.evaluate.finder import get_names_of_scope
-from jedi.evaluate.helpers import search_call_signatures
+from jedi.evaluate.cache import memoize_default
+from jedi.evaluate.helpers import FakeName, get_module_names
+from jedi.evaluate.finder import global_names_dict_generator, filter_definition_names
 from jedi.evaluate import analysis
 
 # Jedi uses lots and lots of recursion. By setting this a little bit higher, we
 # can remove some "maximum recursion depth" errors.
 sys.setrecursionlimit(2000)
 
 
 class NotFoundError(Exception):
-    """A custom error to avoid catching the wrong exceptions."""
+    """A custom error to avoid catching the wrong exceptions.
+
+    .. deprecated:: 0.9.0
+       Not in use anymore, Jedi just returns no goto result if you're not on a
+       valid name.
+    .. todo:: Remove!
+    """
 
 
 class Script(object):
     """
     A Script is the base for completions, goto or whatever you want to do with
     |jedi|.
 
@@ -94,21 +98,28 @@
 
         line_len = len(lines[line - 1])
         column = line_len if column is None else column
         if not (0 <= column <= line_len):
             raise ValueError('`column` parameter is not in a valid range.')
         self._pos = line, column
 
-        cache.clear_caches()
+        cache.clear_time_caches()
         debug.reset_time()
+        self._grammar = load_grammar('grammar%s.%s' % sys.version_info[:2])
         self._user_context = UserContext(self.source, self._pos)
-        self._parser = UserContextParser(self.source, path, self._pos, self._user_context)
-        self._evaluator = Evaluator()
+        self._parser = UserContextParser(self._grammar, self.source, path,
+                                         self._pos, self._user_context,
+                                         self._parsed_callback)
+        self._evaluator = Evaluator(self._grammar)
         debug.speed('init')
 
+    def _parsed_callback(self, parser):
+        module = self._evaluator.wrap(parser.module)
+        imports.add_module(self._evaluator, unicode(module.name), module)
+
     @property
     def source_path(self):
         """
         .. deprecated:: 0.7.0
            Use :attr:`.path` instead.
         .. todo:: Remove!
         """
@@ -123,121 +134,133 @@
         Return :class:`classes.Completion` objects. Those objects contain
         information about the completions, more than just names.
 
         :return: Completion objects, sorted by name and __ comes last.
         :rtype: list of :class:`classes.Completion`
         """
         def get_completions(user_stmt, bs):
-            if isinstance(user_stmt, pr.Import):
-                context = self._user_context.get_context()
-                next(context)  # skip the path
+            # TODO this closure is ugly. it also doesn't work with
+            # simple_complete (used for Interpreter), somehow redo.
+            module = self._evaluator.wrap(self._parser.module())
+            names, level, only_modules, unfinished_dotted = \
+                helpers.check_error_statements(module, self._pos)
+            completion_names = []
+            if names is not None:
+                imp_names = tuple(str(n) for n in names if n.end_pos < self._pos)
+                i = imports.Importer(self._evaluator, imp_names, module, level)
+                completion_names = i.completion_names(self._evaluator, only_modules)
+
+            # TODO this paragraph is necessary, but not sure it works.
+            context = self._user_context.get_context()
+            if not next(context).startswith('.'):  # skip the path
                 if next(context) == 'from':
                     # completion is just "import" if before stands from ..
-                    return ((k, bs) for k in keywords.keyword_names('import'))
-            return self._simple_complete(path, like)
-
-        def completion_possible(path):
-            """
-            The completion logic is kind of complicated, because we strip the
-            last word part. To ignore certain strange patterns with dots, just
-            use regex.
-            """
-            if re.match('\d+\.\.$|\.{4}$', path):
-                return True  # check Ellipsis and float literal `1.`
+                    if unfinished_dotted:
+                        return completion_names
+                    else:
+                        return keywords.keyword_names('import')
 
-            return not re.search(r'^\.|^\d\.$|\.\.$', path)
+            if isinstance(user_stmt, tree.Import):
+                module = self._parser.module()
+                completion_names += imports.completion_names(self._evaluator,
+                                                             user_stmt, self._pos)
+                return completion_names
+
+            if names is None and not isinstance(user_stmt, tree.Import):
+                if not path and not dot:
+                    # add keywords
+                    completion_names += keywords.keyword_names(all=True)
+                    # TODO delete? We should search for valid parser
+                    # transformations.
+                completion_names += self._simple_complete(path, dot, like)
+            return completion_names
 
         debug.speed('completions start')
         path = self._user_context.get_path_until_cursor()
-        if not completion_possible(path):
+        # Dots following an int are not the start of a completion but a float
+        # literal.
+        if re.search(r'^\d\.$', path):
             return []
         path, dot, like = helpers.completion_parts(path)
 
         user_stmt = self._parser.user_stmt_with_whitespace()
+
         b = compiled.builtin
-        completions = get_completions(user_stmt, b)
+        completion_names = get_completions(user_stmt, b)
 
         if not dot:
             # add named params
             for call_sig in self.call_signatures():
-                # allow protected access, because it's a public API.
-                module = call_sig._definition.get_parent_until()
+                # Allow protected access, because it's a public API.
+                module = call_sig._name.get_parent_until()
                 # Compiled modules typically don't allow keyword arguments.
                 if not isinstance(module, compiled.CompiledObject):
                     for p in call_sig.params:
                         # Allow access on _definition here, because it's a
                         # public API and we don't want to make the internal
                         # Name object public.
                         if p._definition.stars == 0:  # no *args/**kwargs
-                            completions.append((p._definition.get_name(), p))
-
-            if not path and not isinstance(user_stmt, pr.Import):
-                # add keywords
-                completions += ((k, b) for k in keywords.keyword_names(all=True))
+                            completion_names.append(p._name)
 
         needs_dot = not dot and path
 
         comps = []
         comp_dct = {}
-        for c, s in set(completions):
-            n = str(c.names[-1])
+        for c in set(completion_names):
+            n = str(c)
             if settings.case_insensitive_completion \
                     and n.lower().startswith(like.lower()) \
                     or n.startswith(like):
-                if not filter_private_variable(s, user_stmt or self._parser.user_scope(), n):
-                    new = classes.Completion(self._evaluator, c, needs_dot, len(like), s)
-                    k = (new.name, new.complete)  # key
-                    if k in comp_dct and settings.no_completion_duplicates:
-                        comp_dct[k]._same_name_completions.append(new)
-                    else:
-                        comp_dct[k] = new
-                        comps.append(new)
+                if isinstance(c.parent, (tree.Function, tree.Class)):
+                    # TODO I think this is a hack. It should be an
+                    #   er.Function/er.Class before that.
+                    c = self._evaluator.wrap(c.parent).name
+                new = classes.Completion(self._evaluator, c, needs_dot, len(like))
+                k = (new.name, new.complete)  # key
+                if k in comp_dct and settings.no_completion_duplicates:
+                    comp_dct[k]._same_name_completions.append(new)
+                else:
+                    comp_dct[k] = new
+                    comps.append(new)
 
         debug.speed('completions end')
 
         return sorted(comps, key=lambda x: (x.name.startswith('__'),
                                             x.name.startswith('_'),
                                             x.name.lower()))
 
-    def _simple_complete(self, path, like):
-        try:
-            scopes = list(self._prepare_goto(path, True))
-        except NotFoundError:
-            scopes = []
-            scope_names_generator = get_names_of_scope(self._evaluator,
-                                                       self._parser.user_scope(),
-                                                       self._pos)
-            completions = []
-            for scope, name_list in scope_names_generator:
-                for c in name_list:
-                    completions.append((c, scope))
+    def _simple_complete(self, path, dot, like):
+        if not path and not dot:
+            scope = self._parser.user_scope()
+            if not scope.is_scope():  # Might be a flow (if/while/etc).
+                scope = scope.get_parent_scope()
+            names_dicts = global_names_dict_generator(
+                self._evaluator,
+                self._evaluator.wrap(scope),
+                self._pos
+            )
+            completion_names = []
+            for names_dict, pos in names_dicts:
+                names = list(chain.from_iterable(names_dict.values()))
+                if not names:
+                    continue
+                completion_names += filter_definition_names(names, self._parser.user_stmt(), pos)
+        elif self._get_under_cursor_stmt(path) is None:
+            return []
         else:
-            completions = []
+            scopes = list(self._prepare_goto(path, True))
+            completion_names = []
             debug.dbg('possible completion scopes: %s', scopes)
             for s in scopes:
-                if s.isinstance(er.Function):
-                    names = s.get_magic_function_names()
-                elif isinstance(s, imports.ImportWrapper):
-                    under = like + self._user_context.get_path_after_cursor()
-                    if under == 'import':
-                        current_line = self._user_context.get_position_line()
-                        if not current_line.endswith('import import'):
-                            continue
-                    a = s.import_stmt.alias
-                    if a and a.start_pos <= self._pos <= a.end_pos:
-                        continue
-                    names = s.get_defined_names(on_import_stmt=True)
-                else:
-                    names = []
-                    for _, new_names in s.scope_names_generator():
-                        names += new_names
-
-                for c in names:
-                    completions.append((c, s))
-        return completions
+                names = []
+                for names_dict in s.names_dicts(search_global=False):
+                    names += chain.from_iterable(names_dict.values())
+
+                completion_names += filter_definition_names(names, self._parser.user_stmt())
+        return completion_names
 
     def _prepare_goto(self, goto_path, is_completion=False):
         """
         Base for completions/goto. Basically it returns the resolved scopes
         under cursor.
         """
         debug.dbg('start: %s in %s', goto_path, self._parser.user_scope())
@@ -245,116 +268,61 @@
         user_stmt = self._parser.user_stmt_with_whitespace()
         if not user_stmt and len(goto_path.split('\n')) > 1:
             # If the user_stmt is not defined and the goto_path is multi line,
             # something's strange. Most probably the backwards tokenizer
             # matched to much.
             return []
 
-        if isinstance(user_stmt, pr.Import):
-            scopes = [helpers.get_on_import_stmt(self._evaluator, self._user_context,
-                                                 user_stmt, is_completion)[0]]
+        if isinstance(user_stmt, tree.Import):
+            i, _ = helpers.get_on_import_stmt(self._evaluator, self._user_context,
+                                              user_stmt, is_completion)
+            if i is None:
+                return []
+            scopes = [i]
         else:
             # just parse one statement, take it and evaluate it
             eval_stmt = self._get_under_cursor_stmt(goto_path)
+            if eval_stmt is None:
+                return []
+
+            module = self._evaluator.wrap(self._parser.module())
+            names, level, _, _ = helpers.check_error_statements(module, self._pos)
+            if names:
+                names = [str(n) for n in names]
+                i = imports.Importer(self._evaluator, names, module, level)
+                return i.follow()
+
+            scopes = self._evaluator.eval_element(eval_stmt)
 
-            if not is_completion:
-                # goto_definition returns definitions of its statements if the
-                # cursor is on the assignee. By changing the start_pos of our
-                # "pseudo" statement, the Jedi evaluator can find the assignees.
-                if user_stmt is not None:
-                    eval_stmt.start_pos = user_stmt.end_pos
-            scopes = self._evaluator.eval_statement(eval_stmt)
         return scopes
 
-    def _get_under_cursor_stmt(self, cursor_txt):
-        tokenizer = source_tokens(cursor_txt, line_offset=self._pos[0] - 1)
-        r = Parser(cursor_txt, no_docstr=True, tokenizer=tokenizer)
+    @memoize_default()
+    def _get_under_cursor_stmt(self, cursor_txt, start_pos=None):
+        tokenizer = source_tokens(cursor_txt)
+        r = Parser(self._grammar, cursor_txt, tokenizer=tokenizer)
         try:
-            # Take the last statement available.
-            stmt = r.module.statements[-1]
-        except IndexError:
-            raise NotFoundError()
-        if isinstance(stmt, pr.KeywordStatement):
-            stmt = stmt.stmt
-        if not isinstance(stmt, pr.Statement):
-            raise NotFoundError()
+            # Take the last statement available that is not an endmarker.
+            # And because it's a simple_stmt, we need to get the first child.
+            stmt = r.module.children[-2].children[0]
+        except (AttributeError, IndexError):
+            return None
 
         user_stmt = self._parser.user_stmt()
         if user_stmt is None:
-            # Set the start_pos to a pseudo position, that doesn't exist but works
-            # perfectly well (for both completions in docstrings and statements).
-            stmt.start_pos = self._pos
+            # Set the start_pos to a pseudo position, that doesn't exist but
+            # works perfectly well (for both completions in docstrings and
+            # statements).
+            pos = start_pos or self._pos
         else:
-            stmt.start_pos = user_stmt.start_pos
+            pos = user_stmt.start_pos
+
+        stmt.move(pos[0] - 1, pos[1])  # Moving the offset.
         stmt.parent = self._parser.user_scope()
         return stmt
 
-    def complete(self):
-        """
-        .. deprecated:: 0.6.0
-           Use :attr:`.completions` instead.
-        .. todo:: Remove!
-        """
-        warnings.warn("Use completions instead.", DeprecationWarning)
-        return self.completions()
-
-    def goto(self):
-        """
-        .. deprecated:: 0.6.0
-           Use :attr:`.goto_assignments` instead.
-        .. todo:: Remove!
-        """
-        warnings.warn("Use goto_assignments instead.", DeprecationWarning)
-        return self.goto_assignments()
-
-    def definition(self):
-        """
-        .. deprecated:: 0.6.0
-           Use :attr:`.goto_definitions` instead.
-        .. todo:: Remove!
-        """
-        warnings.warn("Use goto_definitions instead.", DeprecationWarning)
-        return self.goto_definitions()
-
-    def get_definition(self):
-        """
-        .. deprecated:: 0.5.0
-           Use :attr:`.goto_definitions` instead.
-        .. todo:: Remove!
-        """
-        warnings.warn("Use goto_definitions instead.", DeprecationWarning)
-        return self.goto_definitions()
-
-    def related_names(self):
-        """
-        .. deprecated:: 0.6.0
-           Use :attr:`.usages` instead.
-        .. todo:: Remove!
-        """
-        warnings.warn("Use usages instead.", DeprecationWarning)
-        return self.usages()
-
-    def get_in_function_call(self):
-        """
-        .. deprecated:: 0.6.0
-           Use :attr:`.call_signatures` instead.
-        .. todo:: Remove!
-        """
-        return self.function_definition()
-
-    def function_definition(self):
-        """
-        .. deprecated:: 0.6.0
-           Use :attr:`.call_signatures` instead.
-        .. todo:: Remove!
-        """
-        warnings.warn("Use call_signatures instead.", DeprecationWarning)
-        sig = self.call_signatures()
-        return sig[0] if sig else None
-
     def goto_definitions(self):
         """
         Return the definitions of a the path under the cursor.  goto function!
         This follows complicated paths and returns the end, not the first
         definition. The big difference between :meth:`goto_assignments` and
         :meth:`goto_definitions` is that :meth:`goto_assignments` doesn't
         follow imports and statements. Multiple objects may be returned,
@@ -366,55 +334,53 @@
         def resolve_import_paths(scopes):
             for s in scopes.copy():
                 if isinstance(s, imports.ImportWrapper):
                     scopes.remove(s)
                     scopes.update(resolve_import_paths(set(s.follow())))
             return scopes
 
-        user_stmt = self._parser.user_stmt_with_whitespace()
         goto_path = self._user_context.get_path_under_cursor()
         context = self._user_context.get_context()
         definitions = set()
         if next(context) in ('class', 'def'):
-            definitions = set([self._parser.user_scope()])
+            definitions = set([self._evaluator.wrap(self._parser.user_scope())])
         else:
             # Fetch definition of callee, if there's no path otherwise.
             if not goto_path:
-                (call, _) = search_call_signatures(user_stmt, self._pos)
-                if call is not None:
-                    while call.next is not None:
-                        call = call.next
-                    # reset cursor position:
-                    (row, col) = call.name.end_pos
-                    pos = (row, max(col - 1, 0))
-                    self._user_context = UserContext(self.source, pos)
-                    # then try to find the path again
-                    goto_path = self._user_context.get_path_under_cursor()
-
-        if not definitions:
-            if goto_path:
-                definitions = set(self._prepare_goto(goto_path))
+                definitions = set(signature._definition
+                                  for signature in self.call_signatures())
+
+        if re.match('\w[\w\d_]*$', goto_path) and not definitions:
+            user_stmt = self._parser.user_stmt()
+            if user_stmt is not None and user_stmt.type == 'expr_stmt':
+                for name in user_stmt.get_defined_names():
+                    if name.start_pos <= self._pos <= name.end_pos:
+                        # TODO scaning for a name and then using it should be
+                        # the default.
+                        definitions = set(self._evaluator.goto_definition(name))
+
+        if not definitions and goto_path:
+            definitions = set(self._prepare_goto(goto_path))
 
         definitions = resolve_import_paths(definitions)
-        d = set([classes.Definition(self._evaluator, s) for s in definitions
-                 if s is not imports.ImportWrapper.GlobalNamespace])
-        return helpers.sorted_definitions(d)
+        names = [s.name for s in definitions]
+        defs = [classes.Definition(self._evaluator, name) for name in names]
+        return helpers.sorted_definitions(set(defs))
 
     def goto_assignments(self):
         """
         Return the first definition found. Imports and statements aren't
         followed. Multiple objects may be returned, because Python itself is a
         dynamic language, which means depending on an option you can have two
         different versions of a function.
 
         :rtype: list of :class:`classes.Definition`
         """
-        results, _ = self._goto()
-        d = [classes.Definition(self._evaluator, d) for d in set(results)
-             if d is not imports.ImportWrapper.GlobalNamespace]
+        results = self._goto()
+        d = [classes.Definition(self._evaluator, d) for d in set(results)]
         return helpers.sorted_definitions(d)
 
     def _goto(self, add_import_name=False):
         """
         Used for goto_assignments and usages.
 
         :param add_import_name: Add the the name (if import) to the result.
@@ -422,124 +388,112 @@
         def follow_inexistent_imports(defs):
             """ Imports can be generated, e.g. following
             `multiprocessing.dummy` generates an import dummy in the
             multiprocessing module. The Import doesn't exist -> follow.
             """
             definitions = set(defs)
             for d in defs:
-                if isinstance(d.parent, pr.Import) \
+                if isinstance(d.parent, tree.Import) \
                         and d.start_pos == (0, 0):
                     i = imports.ImportWrapper(self._evaluator, d.parent).follow(is_goto=True)
                     definitions.remove(d)
                     definitions |= follow_inexistent_imports(i)
             return definitions
 
         goto_path = self._user_context.get_path_under_cursor()
         context = self._user_context.get_context()
         user_stmt = self._parser.user_stmt()
+        user_scope = self._parser.user_scope()
+
+        stmt = self._get_under_cursor_stmt(goto_path)
+        if stmt is None:
+            return []
+
+        if user_scope is None:
+            last_name = None
+        else:
+            # Try to use the parser if possible.
+            last_name = user_scope.name_for_position(self._pos)
+
+        if last_name is None:
+            last_name = stmt
+            while not isinstance(last_name, tree.Name):
+                try:
+                    last_name = last_name.children[-1]
+                except AttributeError:
+                    # Doesn't have a name in it.
+                    return []
+
         if next(context) in ('class', 'def'):
+            # The cursor is on a class/function name.
             user_scope = self._parser.user_scope()
             definitions = set([user_scope.name])
-            search_name = unicode(user_scope.name)
-        elif isinstance(user_stmt, pr.Import):
-            s, name_part = helpers.get_on_import_stmt(self._evaluator,
-                                                      self._user_context, user_stmt)
-            try:
-                definitions = [s.follow(is_goto=True)[0]]
-            except IndexError:
-                definitions = []
-            search_name = unicode(name_part)
-
-            if add_import_name:
-                import_name = user_stmt.get_defined_names()
-                # imports have only one name
-                if not user_stmt.star \
-                        and unicode(name_part) == unicode(import_name[0].names[-1]):
-                    definitions.append(import_name[0])
-        else:
-            stmt = self._get_under_cursor_stmt(goto_path)
+        elif isinstance(user_stmt, tree.Import):
+            s, name = helpers.get_on_import_stmt(self._evaluator,
+                                                 self._user_context, user_stmt)
 
-            def test_lhs():
-                """
-                Special rule for goto, left hand side of the statement returns
-                itself, if the name is ``foo``, but not ``foo.bar``.
-                """
-                if isinstance(user_stmt, pr.Statement):
-                    for name in user_stmt.get_defined_names():
-                        if name.start_pos <= self._pos <= name.end_pos \
-                                and len(name.names) == 1:
-                            return name, unicode(name.names[-1])
-                return None, None
-
-            lhs, search_name = test_lhs()
-            if lhs is None:
-                expression_list = stmt.expression_list()
-                if len(expression_list) == 0:
-                    return [], ''
-                # Only the first command is important, the rest should basically not
-                # happen except in broken code (e.g. docstrings that aren't code).
-                call = expression_list[0]
-                if isinstance(call, pr.Call):
-                    call_path = list(call.generate_call_path())
-                else:
-                    call_path = [call]
-
-                defs, search_name_part = self._evaluator.goto(stmt, call_path)
-                search_name = unicode(search_name_part)
-                definitions = follow_inexistent_imports(defs)
-            else:
-                definitions = [lhs]
-            if isinstance(user_stmt, pr.Statement):
-                c = user_stmt.expression_list()
-                if c and not isinstance(c[0], (str, unicode)) \
-                        and c[0].start_pos > self._pos \
-                        and not re.search(r'\.\w+$', goto_path):
-                    # The cursor must be after the start, otherwise the
-                    # statement is just an assignee.
-                    definitions = [user_stmt]
-        return definitions, search_name
+            definitions = self._evaluator.goto(name)
+        else:
+            # The Evaluator.goto function checks for definitions, but since we
+            # use a reverse tokenizer, we have new name_part objects, so we
+            # have to check the user_stmt here for positions.
+            if isinstance(user_stmt, tree.ExprStmt) \
+                    and isinstance(last_name.parent, tree.ExprStmt):
+                for name in user_stmt.get_defined_names():
+                    if name.start_pos <= self._pos <= name.end_pos:
+                        return [name]
+
+            defs = self._evaluator.goto(last_name)
+            definitions = follow_inexistent_imports(defs)
+        return definitions
 
     def usages(self, additional_module_paths=()):
         """
         Return :class:`classes.Definition` objects, which contain all
         names that point to the definition of the name under the cursor. This
         is very useful for refactoring (renaming), or to show all usages of a
         variable.
 
         .. todo:: Implement additional_module_paths
 
         :rtype: list of :class:`classes.Definition`
         """
         temp, settings.dynamic_flow_information = \
             settings.dynamic_flow_information, False
-        user_stmt = self._parser.user_stmt()
-        definitions, search_name = self._goto(add_import_name=True)
-        if isinstance(user_stmt, pr.Statement):
-            c = user_stmt.expression_list()[0]
-            if not isinstance(c, unicode) and self._pos < c.start_pos:
-                # the search_name might be before `=`
-                definitions = [v for v in user_stmt.get_defined_names()
-                               if unicode(v.names[-1]) == search_name]
-        if not isinstance(user_stmt, pr.Import):
-            # import case is looked at with add_import_name option
-            definitions = usages.usages_add_import_modules(self._evaluator, definitions, search_name)
-
-        module = set([d.get_parent_until() for d in definitions])
-        module.add(self._parser.module())
-        names = usages.usages(self._evaluator, definitions, search_name, module)
-
-        for d in set(definitions):
-            try:
-                name_part = d.names[-1]
-            except AttributeError:
+        try:
+            user_stmt = self._parser.user_stmt()
+            definitions = self._goto(add_import_name=True)
+            if not definitions and isinstance(user_stmt, tree.Import):
+                # For not defined imports (goto doesn't find something, we take
+                # the name as a definition. This is enough, because every name
+                # points to it.
+                name = user_stmt.name_for_position(self._pos)
+                if name is None:
+                    # Must be syntax
+                    return []
+                definitions = [name]
+
+            if not definitions:
+                # Without a definition for a name we cannot find references.
+                return []
+
+            if not isinstance(user_stmt, tree.Import):
+                # import case is looked at with add_import_name option
+                definitions = usages.usages_add_import_modules(self._evaluator,
+                                                               definitions)
+
+            module = set([d.get_parent_until() for d in definitions])
+            module.add(self._parser.module())
+            names = usages.usages(self._evaluator, definitions, module)
+
+            for d in set(definitions):
                 names.append(classes.Definition(self._evaluator, d))
-            else:
-                names.append(classes.Definition(self._evaluator, name_part))
+        finally:
+            settings.dynamic_flow_information = temp
 
-        settings.dynamic_flow_information = temp
         return helpers.sorted_definitions(set(names))
 
     def call_signatures(self):
         """
         Return the function object of the call you're currently in.
 
         E.g. if the cursor is here::
@@ -550,60 +504,51 @@
 
             abs()# <-- cursor is here
 
         This would return ``None``.
 
         :rtype: list of :class:`classes.CallSignature`
         """
-        user_stmt = self._parser.user_stmt_with_whitespace()
-        call, index = search_call_signatures(user_stmt, self._pos)
-        if call is None:
+        call_txt, call_index, key_name, start_pos = self._user_context.call_signature()
+        if call_txt is None:
             return []
 
-        stmt_el = call
-        while isinstance(stmt_el.parent, pr.StatementElement):
-            # Go to parent literal/variable until not possible anymore. This
-            # makes it possible to return the whole expression.
-            stmt_el = stmt_el.parent
-        # We can reset the execution since it's a new object
-        # (fast_parent_copy).
-        execution_arr, call.execution = call.execution, None
+        stmt = self._get_under_cursor_stmt(call_txt, start_pos)
+        if stmt is None:
+            return []
 
         with common.scale_speed_settings(settings.scale_call_signatures):
-            _callable = lambda: self._evaluator.eval_call(stmt_el)
-            origins = cache.cache_call_signatures(_callable, self.source,
-                                                  self._pos, user_stmt)
+            origins = cache.cache_call_signatures(self._evaluator, stmt,
+                                                  self.source, self._pos)
         debug.speed('func_call followed')
 
-        key_name = None
-        try:
-            detail = execution_arr[index].assignment_details[0]
-        except IndexError:
-            pass
-        else:
-            try:
-                key_name = unicode(detail[0][0].name)
-            except (IndexError, AttributeError):
-                pass
-        return [classes.CallSignature(self._evaluator, o, call, index, key_name)
-                for o in origins if o.is_callable()]
+        return [classes.CallSignature(self._evaluator, o.name, stmt, call_index, key_name)
+                for o in origins if hasattr(o, 'py__call__')]
 
     def _analysis(self):
+        def check_types(types):
+            for typ in types:
+                try:
+                    f = typ.iter_content
+                except AttributeError:
+                    pass
+                else:
+                    check_types(f())
+
         #statements = set(chain(*self._parser.module().used_names.values()))
-        stmts, imps = analysis.get_module_statements(self._parser.module())
+        nodes, imp_names, decorated_funcs = \
+            analysis.get_module_statements(self._parser.module())
         # Sort the statements so that the results are reproducible.
-        for i in imps:
-            iw = imports.ImportWrapper(self._evaluator, i,
-                                       nested_resolve=True).follow()
-            if i.is_nested() and any(not isinstance(i, pr.Module) for i in iw):
-                analysis.add(self._evaluator, 'import-error', i.namespace.names[-1])
-        for stmt in sorted(stmts, key=lambda obj: obj.start_pos):
-            if not (isinstance(stmt.parent, pr.ForFlow)
-                    and stmt.parent.set_stmt == stmt):
-                self._evaluator.eval_statement(stmt)
+        for n in imp_names:
+            imports.ImportWrapper(self._evaluator, n).follow()
+        for node in sorted(nodes, key=lambda obj: obj.start_pos):
+            check_types(self._evaluator.eval_element(node))
+
+        for dec_func in decorated_funcs:
+            er.Function(self._evaluator, dec_func).get_decorated_func()
 
         ana = [a for a in self._evaluator.analysis if self.path == a.path]
         return sorted(set(ana), key=lambda x: x.line)
 
 
 class Interpreter(Script):
     """
@@ -617,39 +562,50 @@
     >>> from os.path import join
     >>> namespace = locals()
     >>> script = Interpreter('join().up', [namespace])
     >>> print(script.completions()[0].name)
     upper
     """
 
-    def __init__(self, source, namespaces=[], **kwds):
+    def __init__(self, source, namespaces, **kwds):
         """
         Parse `source` and mixin interpreted Python objects from `namespaces`.
 
         :type source: str
         :arg  source: Code to parse.
         :type namespaces: list of dict
         :arg  namespaces: a list of namespace dictionaries such as the one
                           returned by :func:`locals`.
 
         Other optional arguments are same as the ones for :class:`Script`.
         If `line` and `column` are None, they are assumed be at the end of
         `source`.
         """
+        if type(namespaces) is not list or len(namespaces) == 0 or \
+           any([type(x) is not dict for x in namespaces]):
+            raise TypeError("namespaces must be a non-empty list of dict")
+
         super(Interpreter, self).__init__(source, **kwds)
         self.namespaces = namespaces
 
-        # Here we add the namespaces to the current parser.
-        interpreter.create(self._evaluator, namespaces[0], self._parser.module())
+        # Don't use the fast parser, because it does crazy stuff that we don't
+        # need in our very simple and small code here (that is always
+        # changing).
+        self._parser = UserContextParser(self._grammar, self.source,
+                                         self._orig_path, self._pos,
+                                         self._user_context, self._parsed_callback,
+                                         use_fast_parser=False)
+        interpreter.add_namespaces_to_parser(self._evaluator, namespaces,
+                                             self._parser.module())
 
-    def _simple_complete(self, path, like):
+    def _simple_complete(self, path, dot, like):
         user_stmt = self._parser.user_stmt_with_whitespace()
         is_simple_path = not path or re.search('^[\w][\w\d.]*$', path)
-        if isinstance(user_stmt, pr.Import) or not is_simple_path:
-            return super(Interpreter, self)._simple_complete(path, like)
+        if isinstance(user_stmt, tree.Import) or not is_simple_path:
+            return super(Interpreter, self)._simple_complete(path, dot, like)
         else:
             class NamespaceModule(object):
                 def __getattr__(_, name):
                     for n in self.namespaces:
                         try:
                             return n[name]
                         except KeyError:
@@ -664,44 +620,72 @@
 
             namespaces = (NamespaceModule(), builtins)
             for p in paths:
                 old, namespaces = namespaces, []
                 for n in old:
                     try:
                         namespaces.append(getattr(n, p))
-                    except AttributeError:
+                    except Exception:
                         pass
 
-            completions = []
+            completion_names = []
             for namespace in namespaces:
                 for name in dir(namespace):
                     if name.lower().startswith(like.lower()):
                         scope = self._parser.module()
                         n = FakeName(name, scope)
-                        completions.append((n, scope))
-            return completions
+                        completion_names.append(n)
+            return completion_names
 
 
 def defined_names(source, path=None, encoding='utf-8'):
     """
     Get all definitions in `source` sorted by its position.
 
     This functions can be used for listing functions, classes and
     data defined in a file.  This can be useful if you want to list
     them in "sidebar".  Each element in the returned list also has
     `defined_names` method which can be used to get sub-definitions
     (e.g., methods in class).
 
     :rtype: list of classes.Definition
+
+    .. deprecated:: 0.9.0
+       Use :func:`names` instead.
+    .. todo:: Remove!
+    """
+    warnings.warn("Use call_signatures instead.", DeprecationWarning)
+    return names(source, path, encoding)
+
+
+def names(source=None, path=None, encoding='utf-8', all_scopes=False,
+          definitions=True, references=False):
+    """
+    Returns a list of `Definition` objects, containing name parts.
+    This means you can call ``Definition.goto_assignments()`` and get the
+    reference of a name.
+    The parameters are the same as in :py:class:`Script`, except or the
+    following ones:
+
+    :param all_scopes: If True lists the names of all scopes instead of only
+        the module namespace.
+    :param definitions: If True lists the names that have been defined by a
+        class, function or a statement (``a = b`` returns ``a``).
+    :param references: If True lists all the names that are not listed by
+        ``definitions=True``. E.g. ``a = b`` returns ``b``.
     """
-    parser = Parser(
-        common.source_to_unicode(source, encoding),
-        module_path=path,
-    )
-    return classes.defined_names(Evaluator(), parser.module)
+    def def_ref_filter(_def):
+        is_def = _def.is_definition()
+        return definitions and is_def or references and not is_def
+
+    # Set line/column to a random position, because they don't matter.
+    script = Script(source, line=1, column=0, path=path, encoding=encoding)
+    defs = [classes.Definition(script._evaluator, name_part)
+            for name_part in get_module_names(script._parser.module(), all_scopes)]
+    return sorted(filter(def_ref_filter, defs), key=lambda x: (x.line, x.column))
 
 
 def preload_module(*modules):
     """
     Preloading modules tells Jedi to load a module now, instead of lazy parsing
     of modules. Usful for IDEs, to control which modules to load on startup.
```

### Comparing `jedi-0.8.1-final0/jedi/api/classes.py` & `jedi-0.9.0/jedi/api/classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 """
 The :mod:`jedi.api.classes` module contains the return classes of the API.
 These classes are the much bigger part of the whole API, because they contain
 the interesting information about completion and goto operations.
 """
 import warnings
 from itertools import chain
+import re
 
-from jedi._compatibility import next, unicode, use_metaclass
+from jedi._compatibility import unicode, use_metaclass
 from jedi import settings
 from jedi import common
-from jedi.parser import representation as pr
-from jedi.cache import underscore_memoization
+from jedi.parser import tree
 from jedi.evaluate.cache import memoize_default, CachedMetaClass
 from jedi.evaluate import representation as er
 from jedi.evaluate import iterable
 from jedi.evaluate import imports
 from jedi.evaluate import compiled
 from jedi.api import keywords
-from jedi.evaluate.finder import get_names_of_scope
+from jedi.evaluate.finder import filter_definition_names
 
 
 def defined_names(evaluator, scope):
     """
     List sub-definitions (e.g., methods in class).
 
     :type scope: Scope
     :rtype: list of Definition
     """
-    # Calling get_names_of_scope doesn't make sense always. It might include
-    # star imports or inherited stuff. Wanted?
-    # TODO discuss!
-    if isinstance(scope, pr.Module):
-        pair = scope, scope.get_defined_names()
-    else:
-        pair = next(get_names_of_scope(evaluator, scope, star_search=False,
-                                       include_builtin=False), None)
-    names = pair[1] if pair else []
-    names = [n for n in names if isinstance(n, pr.Import) or (len(n) == 1)]
+    dct = scope.names_dict
+    names = list(chain.from_iterable(dct.values()))
+    names = filter_definition_names(names, scope)
     return [Definition(evaluator, d) for d in sorted(names, key=lambda s: s.start_pos)]
 
 
 class BaseDefinition(object):
     _mapping = {
         'posixpath': 'os.path',
         'riscospath': 'os.path',
@@ -58,40 +51,51 @@
 
     _tuple_mapping = dict((tuple(k.split('.')), v) for (k, v) in {
         'argparse._ActionsContainer': 'argparse.ArgumentParser',
         '_sre.SRE_Match': 're.MatchObject',
         '_sre.SRE_Pattern': 're.RegexObject',
     }.items())
 
-    def __init__(self, evaluator, definition, start_pos):
+    def __init__(self, evaluator, name):
         self._evaluator = evaluator
-        self._start_pos = start_pos
-        self._definition = definition
+        self._name = name
         """
-        An instance of :class:`jedi.parsing_representation.Base` subclass.
+        An instance of :class:`jedi.parser.reprsentation.Name` subclass.
         """
-        self.is_keyword = isinstance(definition, keywords.Keyword)
+        self._definition = evaluator.wrap(self._name.get_definition())
+        self.is_keyword = isinstance(self._definition, keywords.Keyword)
 
         # generate a path to the definition
-        self._module = definition.get_parent_until()
+        self._module = name.get_parent_until()
         if self.in_builtin_module():
             self.module_path = None
         else:
             self.module_path = self._module.path
             """Shows the file path of a module. e.g. ``/usr/lib/python2.7/os.py``"""
 
     @property
+    def name(self):
+        """
+        Name of variable/function/class/module.
+
+        For example, for ``x = None`` it returns ``'x'``.
+
+        :rtype: str or None
+        """
+        return unicode(self._name)
+
+    @property
     def start_pos(self):
         """
         .. deprecated:: 0.7.0
            Use :attr:`.line` and :attr:`.column` instead.
         .. todo:: Remove!
         """
         warnings.warn("Use line/column instead.", DeprecationWarning)
-        return self._start_pos
+        return self._name.start_pos
 
     @property
     def type(self):
         """
         The type of the definition.
 
         Here is an example of the value of this attribute.  Let's consider
@@ -110,16 +114,18 @@
         ...     pass
         ...
         ... x = D()
         ...
         ... def f():
         ...     pass
         ...
-        ... variable = keyword or f or C or x'''
-        >>> script = Script(source, len(source.splitlines()), 3, 'example.py')
+        ... for variable in [keyword, f, C, x]:
+        ...     variable'''
+
+        >>> script = Script(source)
         >>> defs = script.goto_definitions()
 
         Before showing what is in ``defs``, let's sort it by :attr:`line`
         so that it is easy to relate the result to the source code.
 
         >>> defs = sorted(defs, key=lambda d: d.line)
         >>> defs                           # doctest: +NORMALIZE_WHITESPACE
@@ -134,45 +140,52 @@
         'class'
         >>> defs[2].type
         'instance'
         >>> defs[3].type
         'function'
 
         """
-        # generate the type
         stripped = self._definition
-        if isinstance(stripped, compiled.CompiledObject):
-            return stripped.type()
         if isinstance(stripped, er.InstanceElement):
             stripped = stripped.var
-        if isinstance(stripped, pr.NamePart):
-            stripped = stripped.parent
-        if isinstance(stripped, pr.Name):
-            stripped = stripped.parent
-        return type(stripped).__name__.lower().replace('wrapper', '')
+
+        if isinstance(stripped, compiled.CompiledObject):
+            return stripped.api_type()
+        elif isinstance(stripped, iterable.Array):
+            return 'instance'
+        elif isinstance(stripped, tree.Import):
+            return 'import'
+
+        string = type(stripped).__name__.lower().replace('wrapper', '')
+        if string == 'exprstmt':
+            return 'statement'
+        else:
+            return string
 
     def _path(self):
-        """The module path."""
+        """The path to a module/class/function definition."""
         path = []
-
-        def insert_nonnone(x):
-            if x:
-                path.insert(0, x)
-
-        if not isinstance(self._definition, keywords.Keyword):
-            par = self._definition
-            while par is not None:
-                if isinstance(par, pr.Import):
-                    insert_nonnone(par.namespace)
-                    insert_nonnone(par.from_ns)
-                    if par.relative_count == 0:
-                        break
-                with common.ignored(AttributeError):
-                    path.insert(0, par.name)
-                par = par.parent
+        par = self._definition
+        while par is not None:
+            if isinstance(par, tree.Import):
+                path += imports.ImportWrapper(self._evaluator, self._name).import_path
+                break
+            try:
+                name = par.name
+            except AttributeError:
+                pass
+            else:
+                if isinstance(par, er.ModuleWrapper):
+                    # TODO just make the path dotted from the beginning, we
+                    # shouldn't really split here.
+                    path[0:0] = par.py__name__().split('.')
+                    break
+                else:
+                    path.insert(0, unicode(name))
+            par = par.parent
         return path
 
     @property
     def module_name(self):
         """
         The module name.
 
@@ -186,36 +199,26 @@
         return str(self._module.name)
 
     def in_builtin_module(self):
         """Whether this is a builtin module."""
         return isinstance(self._module, compiled.CompiledObject)
 
     @property
-    def line_nr(self):
-        """
-        .. deprecated:: 0.5.0
-           Use :attr:`.line` instead.
-        .. todo:: Remove!
-        """
-        warnings.warn("Use line instead.", DeprecationWarning)
-        return self.line
-
-    @property
     def line(self):
         """The line where the definition occurs (starting with 1)."""
         if self.in_builtin_module():
             return None
-        return self._start_pos[0]
+        return self._name.start_pos[0]
 
     @property
     def column(self):
         """The column where the definition occurs (starting with 0)."""
         if self.in_builtin_module():
             return None
-        return self._start_pos[1]
+        return self._name.start_pos[1]
 
     def docstring(self, raw=False):
         r"""
         Return a document string for this completion object.
 
         Example:
 
@@ -223,15 +226,15 @@
         >>> source = '''\
         ... def f(a, b=1):
         ...     "Document for function f."
         ... '''
         >>> script = Script(source, 1, len('def f'), 'example.py')
         >>> doc = script.goto_definitions()[0].docstring()
         >>> print(doc)
-        f(a, b = 1)
+        f(a, b=1)
         <BLANKLINE>
         Document for function f.
 
         Notice that useful extra information is added to the actual
         docstring.  For function, it is call signature.  If you need
         actual docstring, use ``raw=True`` instead.
 
@@ -263,15 +266,15 @@
         """
         warnings.warn("Use docstring() instead.", DeprecationWarning)
         return self.docstring(raw=True)
 
     @property
     def description(self):
         """A textual description of the object."""
-        return unicode(self._definition)
+        return unicode(self._name)
 
     @property
     def full_name(self):
         """
         Dot-separated path of this object.
 
         It is in the form of ``<module>[.<submodule>[...]][.<object>]``.
@@ -301,106 +304,95 @@
             path[0] = self._mapping[path[0]]
         for key, repl in self._tuple_mapping.items():
             if tuple(path[:len(key)]) == key:
                 path = [repl] + path[len(key):]
 
         return '.'.join(path if path[0] else path[1:])
 
+    def goto_assignments(self):
+        defs = self._evaluator.goto(self._name)
+        return [Definition(self._evaluator, d) for d in defs]
+
     @memoize_default()
     def _follow_statements_imports(self):
         """
         Follow both statements and imports, as far as possible.
         """
-        stripped = self._definition
-        if isinstance(stripped, pr.Name):
-            stripped = stripped.parent
-
-        # We should probably work in `Finder._names_to_types` here.
-        if isinstance(stripped, pr.Function):
-            stripped = er.Function(self._evaluator, stripped)
-        elif isinstance(stripped, pr.Class):
-            stripped = er.Class(self._evaluator, stripped)
-
-        if stripped.isinstance(pr.Statement):
-            return self._evaluator.eval_statement(stripped)
-        elif stripped.isinstance(pr.Import):
-            return imports.follow_imports(self._evaluator, [stripped])
+        if self._definition.isinstance(tree.ExprStmt):
+            return self._evaluator.eval_statement(self._definition)
+        elif self._definition.isinstance(tree.Import):
+            return imports.ImportWrapper(self._evaluator, self._name).follow()
         else:
-            return [stripped]
+            return [self._definition]
 
     @property
     @memoize_default()
     def params(self):
         """
         Raises an ``AttributeError``if the definition is not callable.
         Otherwise returns a list of `Definition` that represents the params.
         """
         followed = self._follow_statements_imports()
-        if not followed or not followed[0].is_callable():
+        if not followed or not hasattr(followed[0], 'py__call__'):
             raise AttributeError()
         followed = followed[0]  # only check the first one.
 
-        if followed.isinstance(er.Function):
+        if followed.type == 'funcdef':
             if isinstance(followed, er.InstanceElement):
                 params = followed.params[1:]
             else:
                 params = followed.params
         elif followed.isinstance(er.compiled.CompiledObject):
             params = followed.params
         else:
             try:
                 sub = followed.get_subscope_by_name('__init__')
                 params = sub.params[1:]  # ignore self
             except KeyError:
                 return []
-        return [_Param(self._evaluator, p) for p in params]
+        return [_Param(self._evaluator, p.name) for p in params]
 
     def parent(self):
-        if isinstance(self._definition, compiled.CompiledObject):
-            non_flow = self._definition.parent
-        else:
-            scope = self._definition.get_parent_until(pr.IsScope, include_current=False)
-            non_flow = scope.get_parent_until(pr.Flow, reverse=True)
-        return Definition(self._evaluator, non_flow)
+        scope = self._definition.get_parent_scope()
+        scope = self._evaluator.wrap(scope)
+        return Definition(self._evaluator, scope.name)
 
     def __repr__(self):
         return "<%s %s>" % (type(self).__name__, self.description)
 
 
 class Completion(BaseDefinition):
     """
     `Completion` objects are returned from :meth:`api.Script.completions`. They
     provide additional information about a completion.
     """
-    def __init__(self, evaluator, name, needs_dot, like_name_length, base):
-        super(Completion, self).__init__(evaluator, name.parent, name.start_pos)
+    def __init__(self, evaluator, name, needs_dot, like_name_length):
+        super(Completion, self).__init__(evaluator, name)
 
-        self._name = name
         self._needs_dot = needs_dot
         self._like_name_length = like_name_length
-        self._base = base
 
         # Completion objects with the same Completion name (which means
         # duplicate items in the completion)
         self._same_name_completions = []
 
     def _complete(self, like_name):
         dot = '.' if self._needs_dot else ''
         append = ''
         if settings.add_bracket_after_function \
                 and self.type == 'Function':
             append = '('
 
         if settings.add_dot_after_module:
-            if isinstance(self._base, pr.Module):
+            if isinstance(self._definition, tree.Module):
                 append += '.'
-        if isinstance(self._base, pr.Param):
+        if isinstance(self._definition, tree.Param):
             append += '='
 
-        name = str(self._name.names[-1])
+        name = str(self._name)
         if like_name:
             name = name[self._like_name_length:]
         return dot + name + append
 
     @property
     def complete(self):
         """
@@ -410,56 +402,33 @@
 
         would return the string 'ce'. It also adds additional stuff, depending
         on your `settings.py`.
         """
         return self._complete(True)
 
     @property
-    def name(self):
-        """
-        Similar to :attr:`complete`, but return the whole word, for
-        example::
-
-            isinstan
-
-        would return `isinstance`.
-        """
-        return unicode(self._name.names[-1])
-
-    @property
     def name_with_symbols(self):
         """
         Similar to :attr:`name`, but like :attr:`name`
         returns also the symbols, for example::
 
             list()
 
         would return ``.append`` and others (which means it adds a dot).
         """
         return self._complete(False)
 
     @property
-    def word(self):
-        """
-        .. deprecated:: 0.6.0
-           Use :attr:`.name` instead.
-        .. todo:: Remove!
-        """
-        warnings.warn("Use name instead.", DeprecationWarning)
-        return self.name
-
-    @property
     def description(self):
         """Provide a description of the completion object."""
-        parent = self._name.parent
-        if parent is None:
+        if self._definition is None:
             return ''
         t = self.type
         if t == 'statement' or t == 'import':
-            desc = self._definition.get_code(False)
+            desc = self._definition.get_code()
         else:
             desc = '.'.join(unicode(p) for p in self._path())
 
         line = '' if self.in_builtin_module else '@%s' % self.line
         return '%s: %s%s' % (t, desc, line)
 
     def __repr__(self):
@@ -470,16 +439,16 @@
         :param fast: Don't follow imports that are only one level deep like
             ``import foo``, but follow ``from foo import bar``. This makes
             sense for speed reasons. Completing `import a` is slow if you use
             the ``foo.docstring(fast=False)`` on every object, because it
             parses all libraries starting with ``a``.
         """
         definition = self._definition
-        if isinstance(self._definition, pr.Import):
-            i = imports.ImportWrapper(self._evaluator, self._definition)
+        if isinstance(definition, tree.Import):
+            i = imports.ImportWrapper(self._evaluator, self._name)
             if len(i.import_path) > 1 or not fast:
                 followed = self._follow_statements_imports()
                 if followed:
                     # TODO: Use all of the followed objects as input to Documentation.
                     definition = followed[0]
 
         if raw:
@@ -489,16 +458,16 @@
 
     @property
     def type(self):
         """
         The type of the completion objects. Follows imports. For a further
         description, look at :attr:`jedi.api.classes.BaseDefinition.type`.
         """
-        if isinstance(self._definition, pr.Import):
-            i = imports.ImportWrapper(self._evaluator, self._definition)
+        if isinstance(self._definition, tree.Import):
+            i = imports.ImportWrapper(self._evaluator, self._name)
             if len(i.import_path) <= 1:
                 return 'module'
 
             followed = self.follow_definition()
             if followed:
                 # Caveat: Only follows the first one, ignore the other ones.
                 # This is ok, since people are almost never interested in
@@ -506,89 +475,41 @@
                 return followed[0].type
         return super(Completion, self).type
 
     @memoize_default()
     def _follow_statements_imports(self):
         # imports completion is very complicated and needs to be treated
         # separately in Completion.
-        if self._definition.isinstance(pr.Import) and self._definition.alias is None:
-            i = imports.ImportWrapper(self._evaluator, self._definition, True)
-            import_path = i.import_path + (unicode(self._name),)
-            try:
-                return imports.get_importer(self._evaluator, import_path,
-                                            i._importer.module).follow(self._evaluator)
-            except imports.ModuleNotFound:
-                pass
+        definition = self._definition
+        if definition.isinstance(tree.Import):
+            i = imports.ImportWrapper(self._evaluator, self._name)
+            return i.follow()
         return super(Completion, self)._follow_statements_imports()
 
     @memoize_default()
     def follow_definition(self):
         """
         Return the original definitions. I strongly recommend not using it for
         your completions, because it might slow down |jedi|. If you want to
         read only a few objects (<=20), it might be useful, especially to get
         the original docstrings. The basic problem of this function is that it
         follows all results. This means with 1000 completions (e.g.  numpy),
         it's just PITA-slow.
         """
         defs = self._follow_statements_imports()
-        return [Definition(self._evaluator, d) for d in defs]
+        return [Definition(self._evaluator, d.name) for d in defs]
 
 
 class Definition(use_metaclass(CachedMetaClass, BaseDefinition)):
     """
     *Definition* objects are returned from :meth:`api.Script.goto_assignments`
     or :meth:`api.Script.goto_definitions`.
     """
     def __init__(self, evaluator, definition):
-        super(Definition, self).__init__(evaluator, definition, definition.start_pos)
-
-    @property
-    @underscore_memoization
-    def name(self):
-        """
-        Name of variable/function/class/module.
-
-        For example, for ``x = None`` it returns ``'x'``.
-
-        :rtype: str or None
-        """
-        d = self._definition
-        if isinstance(d, er.InstanceElement):
-            d = d.var
-
-        if isinstance(d, (compiled.CompiledObject, compiled.CompiledName)):
-            name = d.name
-        elif isinstance(d, pr.Name):
-            name = d.names[-1]
-        elif isinstance(d, iterable.Array):
-            name = d.type
-        elif isinstance(d, (pr.Class, er.Class, er.Instance,
-                            er.Function, pr.Function)):
-            name = d.name
-        elif isinstance(d, pr.Module):
-            name = self.module_name
-        elif isinstance(d, pr.Import):
-            try:
-                name = d.get_defined_names()[0].names[-1]
-            except (AttributeError, IndexError):
-                return None
-        elif isinstance(d, pr.Param):
-            name = d.get_name()
-        elif isinstance(d, pr.Statement):
-            try:
-                expression_list = d.assignment_details[0][0]
-                name = expression_list[0].name.names[-1]
-            except IndexError:
-                return None
-        elif isinstance(d, iterable.Generator):
-            return None
-        elif isinstance(d, pr.NamePart):
-            name = d
-        return unicode(name)
+        super(Definition, self).__init__(evaluator, definition)
 
     @property
     def description(self):
         """
         A description of the :class:`.Definition` object, which is heavily used
         in testing. e.g. for ``isinstance`` it returns ``def isinstance``.
 
@@ -598,48 +519,65 @@
         >>> source = '''
         ... def f():
         ...     pass
         ...
         ... class C:
         ...     pass
         ...
-        ... variable = f or C'''
+        ... variable = f if random.choice([0,1]) else C'''
         >>> script = Script(source, column=3)  # line is maximum by default
         >>> defs = script.goto_definitions()
         >>> defs = sorted(defs, key=lambda d: d.line)
         >>> defs
         [<Definition def f>, <Definition class C>]
         >>> str(defs[0].description)  # strip literals in python2
         'def f'
         >>> str(defs[1].description)
         'class C'
 
         """
         d = self._definition
         if isinstance(d, er.InstanceElement):
             d = d.var
-        if isinstance(d, pr.Name):
-            d = d.parent
 
         if isinstance(d, compiled.CompiledObject):
-            d = d.type() + ' ' + d.name
+            typ = d.api_type()
+            if typ == 'instance':
+                typ = 'class'  # The description should be similar to Py objects.
+            d = typ + ' ' + d.name.get_code()
         elif isinstance(d, iterable.Array):
             d = 'class ' + d.type
-        elif isinstance(d, (pr.Class, er.Class, er.Instance)):
+        elif isinstance(d, (tree.Class, er.Class, er.Instance)):
             d = 'class ' + unicode(d.name)
-        elif isinstance(d, (er.Function, pr.Function)):
+        elif isinstance(d, (er.Function, tree.Function)):
             d = 'def ' + unicode(d.name)
-        elif isinstance(d, pr.Module):
+        elif isinstance(d, tree.Module):
             # only show module name
             d = 'module %s' % self.module_name
-        elif self.is_keyword:
-            d = 'keyword %s' % d.name
-        else:
-            d = d.get_code().replace('\n', '').replace('\r', '')
-        return d
+        elif isinstance(d, tree.Param):
+            d = d.get_code().strip()
+            if d.endswith(','):
+                d = d[:-1]  # Remove the comma.
+        else:  # ExprStmt
+            try:
+                first_leaf = d.first_leaf()
+            except AttributeError:
+                # `d` is already a Leaf (Name).
+                first_leaf = d
+            # Remove the prefix, because that's not what we want for get_code
+            # here.
+            old, first_leaf.prefix = first_leaf.prefix, ''
+            try:
+                d = d.get_code()
+            finally:
+                first_leaf.prefix = old
+        # Delete comments:
+        d = re.sub('#[^\n]+\n', ' ', d)
+        # Delete multi spaces/newlines
+        return re.sub('\s+', ' ', d).strip()
 
     @property
     def desc_with_module(self):
         """
         In addition to the definition, also return the module.
 
         .. warning:: Don't use this function yet, its behaviour may change. If
@@ -661,97 +599,101 @@
         defs = self._follow_statements_imports()
         # For now we don't want base classes or evaluate decorators.
         defs = [d.base if isinstance(d, (er.Class, er.Function)) else d for d in defs]
         iterable = (defined_names(self._evaluator, d) for d in defs)
         iterable = list(iterable)
         return list(chain.from_iterable(iterable))
 
+    def is_definition(self):
+        """
+        Returns True, if defined as a name in a statement, function or class.
+        Returns False, if it's a reference to such a definition.
+        """
+        return self._name.is_definition()
+
     def __eq__(self, other):
-        return self._start_pos == other._start_pos \
+        return self._name.start_pos == other._name.start_pos \
             and self.module_path == other.module_path \
             and self.name == other.name \
             and self._evaluator == other._evaluator
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __hash__(self):
-        return hash((self._start_pos, self.module_path, self.name, self._evaluator))
+        return hash((self._name.start_pos, self.module_path, self.name, self._evaluator))
 
 
 class CallSignature(Definition):
     """
     `CallSignature` objects is the return value of `Script.function_definition`.
     It knows what functions you are currently in. e.g. `isinstance(` would
     return the `isinstance` function. without `(` it would return nothing.
     """
-    def __init__(self, evaluator, executable, call, index, key_name):
-        super(CallSignature, self).__init__(evaluator, executable)
+    def __init__(self, evaluator, executable_name, call_stmt, index, key_name):
+        super(CallSignature, self).__init__(evaluator, executable_name)
         self._index = index
         self._key_name = key_name
-        self._call = call
+        self._call_stmt = call_stmt
 
     @property
     def index(self):
         """
         The Param index of the current call.
-        Returns None if the index doesn't is not defined.
+        Returns None if the index cannot be found in the curent call.
         """
         if self._key_name is not None:
             for i, param in enumerate(self.params):
                 if self._key_name == param.name:
                     return i
-            if self.params and self.params[-1]._definition.stars == 2:
+            if self.params and self.params[-1]._name.get_definition().stars == 2:
                 return i
             else:
                 return None
 
         if self._index >= len(self.params):
 
             for i, param in enumerate(self.params):
                 # *args case
-                if param._definition.stars == 1:
+                if param._name.get_definition().stars == 1:
                     return i
             return None
         return self._index
 
     @property
     def bracket_start(self):
         """
         The indent of the bracket that is responsible for the last function
         call.
         """
-        c = self._call
-        while c.next is not None:
-            c = c.next
-        return c.name.end_pos
+        return self._call_stmt.end_pos
 
     @property
     def call_name(self):
         """
         .. deprecated:: 0.8.0
            Use :attr:`.name` instead.
         .. todo:: Remove!
 
         The name (e.g. 'isinstance') as a string.
         """
         warnings.warn("Use name instead.", DeprecationWarning)
-        return unicode(self._definition.name)
+        return unicode(self.name)
 
     @property
     def module(self):
         """
         .. deprecated:: 0.8.0
            Use :attr:`.module_name` for the module name.
         .. todo:: Remove!
         """
         return self._executable.get_parent_until()
 
     def __repr__(self):
-        return '<%s: %s index %s>' % (type(self).__name__, self._definition,
+        return '<%s: %s index %s>' % (type(self).__name__, self._name,
                                       self.index)
 
 
 class _Param(Definition):
     """
     Just here for backwards compatibility.
     """
@@ -769,25 +711,25 @@
 
 class _Help(object):
     """
     Temporary implementation, will be used as `Script.help() or something in
     the future.
     """
     def __init__(self, definition):
-        self._definition = definition
+        self._name = definition
 
     def full(self):
         try:
-            return self._definition.doc
+            return self._name.doc
         except AttributeError:
             return self.raw()
 
     def raw(self):
         """
         The raw docstring ``__doc__`` for any object.
 
         See :attr:`doc` for example.
         """
         try:
-            return self._definition.raw_doc
+            return self._name.raw_doc
         except AttributeError:
             return ''
```

### Comparing `jedi-0.8.1-final0/jedi/api/keywords.py` & `jedi-0.9.0/jedi/api/keywords.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pydoc
 import keyword
 
 from jedi._compatibility import is_py3
 from jedi import common
 from jedi.evaluate import compiled
+from jedi.evaluate.helpers import FakeName
 
 try:
     from pydoc_data import topics as pydoc_topics
 except ImportError:
     # Python 2.6
     import pydoc_topics
 
@@ -22,39 +23,24 @@
         return set([Keyword(k, pos) for k in keys])
     if string in keys:
         return set([Keyword(string, pos)])
     return set()
 
 
 def keyword_names(*args, **kwargs):
-    kwds = []
-    for k in keywords(*args, **kwargs):
-        start = k.start_pos
-        kwds.append(KeywordName(k, k.name, start))
-    return kwds
+    return [k.name for k in keywords(*args, **kwargs)]
 
 
 def get_operator(string, pos):
     return Keyword(string, pos)
 
 
-class KeywordName(object):
-    def __init__(self, parent, name, start_pos):
-        self.parent = parent
-        self.names = [name]
-        self.start_pos = start_pos
-
-    @property
-    def end_pos(self):
-        return self.start_pos[0], self.start_pos[1] + len(self.name)
-
-
 class Keyword(object):
     def __init__(self, name, pos):
-        self.name = name
+        self.name = FakeName(name, self, pos)
         self.start_pos = pos
         self.parent = compiled.builtin
 
     def get_parent_until(self):
         return self.parent
 
     @property
```

### Comparing `jedi-0.8.1-final0/jedi/api/replstartup.py` & `jedi-0.9.0/jedi/api/replstartup.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/jedi/api/interpreter.py` & `jedi-0.9.0/jedi/api/interpreter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,58 @@
+"""
+TODO Some parts of this module are still not well documented.
+"""
 import inspect
 import re
 
 from jedi._compatibility import builtins
 from jedi import debug
 from jedi.common import source_to_unicode
 from jedi.cache import underscore_memoization
 from jedi.evaluate import compiled
 from jedi.evaluate.compiled.fake import get_module
-from jedi.parser import representation as pr
+from jedi.parser import tree as pt
+from jedi.parser import load_grammar
 from jedi.parser.fast import FastParser
 from jedi.evaluate import helpers
+from jedi.evaluate import iterable
+from jedi.evaluate import representation as er
 
 
-class InterpreterNamespace(pr.Module):
-    def __init__(self, evaluator, namespace, parser_module):
-        self.namespace = namespace
-        self.parser_module = parser_module
-        self._evaluator = evaluator
-
-    @underscore_memoization
-    def get_defined_names(self):
-        for name in self.parser_module.get_defined_names():
-            yield name
-        for key, value in self.namespace.items():
-            yield LazyName(self._evaluator, key, value)
-
-    def scope_names_generator(self, position=None):
-        yield self, list(self.get_defined_names())
-
-    def __getattr__(self, name):
-        return getattr(self.parser_module, name)
+def add_namespaces_to_parser(evaluator, namespaces, parser_module):
+    for namespace in namespaces:
+        for key, value in namespace.items():
+            # Name lookups in an ast tree work by checking names_dict.
+            # Therefore we just add fake names to that and we're done.
+            arr = parser_module.names_dict.setdefault(key, [])
+            arr.append(LazyName(evaluator, parser_module, key, value))
 
 
 class LazyName(helpers.FakeName):
-    def __init__(self, evaluator, name, value):
+    def __init__(self, evaluator, module, name, value):
         super(LazyName, self).__init__(name)
+        self._module = module
         self._evaluator = evaluator
         self._value = value
         self._name = name
 
+    def is_definition(self):
+        return True
+
     @property
     @underscore_memoization
     def parent(self):
+        """
+        Creating fake statements for the interpreter.
+        """
         obj = self._value
         parser_path = []
         if inspect.ismodule(obj):
             module = obj
         else:
-            class FakeParent(pr.Base):
-                parent = None  # To avoid having no parent for NamePart.
-                path = None
-
             names = []
             try:
                 o = obj.__objclass__
                 names.append(obj.__name__)
                 obj = o
             except AttributeError:
                 pass
@@ -62,47 +60,50 @@
             try:
                 module_name = obj.__module__
                 names.insert(0, obj.__name__)
             except AttributeError:
                 # Unfortunately in some cases like `int` there's no __module__
                 module = builtins
             else:
+                # TODO this import is wrong. Yields x for x.y.z instead of z
                 module = __import__(module_name)
-            fake_name = helpers.FakeName(names, FakeParent())
-            parser_path = fake_name.names
+            parser_path = names
         raw_module = get_module(self._value)
 
+        found = []
         try:
             path = module.__file__
         except AttributeError:
             pass
         else:
             path = re.sub('c$', '', path)
             if path.endswith('.py'):
                 # cut the `c` from `.pyc`
                 with open(path) as f:
                     source = source_to_unicode(f.read())
-                mod = FastParser(source, path[:-1]).module
-                if not parser_path:
-                    return mod
-                found = self._evaluator.eval_call_path(iter(parser_path), mod, None)
-                if found:
-                    return found[0]
-                debug.warning('Interpreter lookup for Python code failed %s',
-                              mod)
-
-        module = compiled.CompiledObject(raw_module)
-        if raw_module == builtins:
-            # The builtins module is special and always cached.
-            module = compiled.builtin
-        return compiled.create(self._evaluator, self._value, module, module)
+                mod = FastParser(load_grammar(), source, path[:-1]).module
+                if parser_path:
+                    assert len(parser_path) == 1
+                    found = self._evaluator.find_types(mod, parser_path[0], search_global=True)
+                else:
+                    found = [self._evaluator.wrap(mod)]
+
+                if not found:
+                    debug.warning('Possibly an interpreter lookup for Python code failed %s',
+                                  parser_path)
+
+        if not found:
+            evaluated = compiled.CompiledObject(obj)
+            if evaluated == builtins:
+                # The builtins module is special and always cached.
+                evaluated = compiled.builtin
+            found = [evaluated]
+
+        content = iterable.AlreadyEvaluated(found)
+        stmt = pt.ExprStmt([self, pt.Operator(pt.zero_position_modifier,
+                                              '=', (0, 0), ''), content])
+        stmt.parent = self._module
+        return stmt
 
     @parent.setter
     def parent(self, value):
-        """Needed because of the ``representation.Simple`` super class."""
-
-
-def create(evaluator, namespace, parser_module):
-    ns = InterpreterNamespace(evaluator, namespace, parser_module)
-    for attr_name in pr.SCOPE_CONTENTS:
-        for something in getattr(parser_module, attr_name):
-            something.parent = ns
+        """Needed because the super class tries to set parent."""
```

### Comparing `jedi-0.8.1-final0/jedi/cache.py` & `jedi-0.9.0/jedi/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,92 +27,96 @@
 except ImportError:
     import pickle
 
 from jedi import settings
 from jedi import common
 from jedi import debug
 
-_time_caches = []
-
-_star_import_cache = {}
+_time_caches = {}
 
 # for fast_parser, should not be deleted
 parser_cache = {}
 
 
 class ParserCacheItem(object):
     def __init__(self, parser, change_time=None):
         self.parser = parser
         if change_time is None:
             change_time = time.time()
         self.change_time = change_time
 
 
-def clear_caches(delete_all=False):
+def clear_time_caches(delete_all=False):
     """ Jedi caches many things, that should be completed after each completion
     finishes.
 
     :param delete_all: Deletes also the cache that is normally not deleted,
         like parser cache, which is important for faster parsing.
     """
     global _time_caches
 
     if delete_all:
-        _time_caches = []
-        _star_import_cache.clear()
+        for cache in _time_caches.values():
+            cache.clear()
         parser_cache.clear()
     else:
         # normally just kill the expired entries, not all
-        for tc in _time_caches:
+        for tc in _time_caches.values():
             # check time_cache for expired entries
             for key, (t, value) in list(tc.items()):
                 if t < time.time():
                     # delete expired entries
                     del tc[key]
 
 
 def time_cache(time_add_setting):
-    """ This decorator works as follows: Call it with a setting and after that
+    """
+    s
+    This decorator works as follows: Call it with a setting and after that
     use the function with a callable that returns the key.
     But: This function is only called if the key is not available. After a
     certain amount of time (`time_add_setting`) the cache is invalid.
     """
     def _temp(key_func):
         dct = {}
-        _time_caches.append(dct)
+        _time_caches[time_add_setting] = dct
 
-        def wrapper(optional_callable, *args, **kwargs):
-            key = key_func(*args, **kwargs)
-            value = None
-            if key in dct:
+        def wrapper(*args, **kwargs):
+            generator = key_func(*args, **kwargs)
+            key = next(generator)
+            try:
                 expiry, value = dct[key]
                 if expiry > time.time():
                     return value
-            value = optional_callable()
+            except KeyError:
+                pass
+
+            value = next(generator)
             time_add = getattr(settings, time_add_setting)
             if key is not None:
                 dct[key] = time.time() + time_add, value
             return value
         return wrapper
     return _temp
 
 
 @time_cache("call_signatures_validity")
-def cache_call_signatures(source, user_pos, stmt):
+def cache_call_signatures(evaluator, call, source, user_pos):
     """This function calculates the cache key."""
     index = user_pos[0] - 1
     lines = common.splitlines(source)
 
     before_cursor = lines[index][:user_pos[1]]
-    other_lines = lines[stmt.start_pos[0]:index]
+    other_lines = lines[call.start_pos[0]:index]
     whole = '\n'.join(other_lines + [before_cursor])
     before_bracket = re.match(r'.*\(', whole, re.DOTALL)
 
-    module_path = stmt.get_parent_until().path
-    return None if module_path is None else (module_path, before_bracket, stmt.start_pos)
+    module_path = call.get_parent_until().path
+    yield None if module_path is None else (module_path, before_bracket, call.start_pos)
+    yield evaluator.eval_element(call)
 
 
 def underscore_memoization(func):
     """
     Decorator for methods::
 
         class A(object):
@@ -141,113 +145,91 @@
                 result = list(result)
             setattr(self, name, result)
             return result
 
     return wrapper
 
 
-def memoize(func):
+def memoize_method(method):
     """A normal memoize function."""
-    dct = {}
-
-    def wrapper(*args, **kwargs):
+    def wrapper(self, *args, **kwargs):
+        dct = self.__dict__.setdefault('_memoize_method_dct', {})
         key = (args, frozenset(kwargs.items()))
         try:
             return dct[key]
         except KeyError:
-            result = func(*args, **kwargs)
+            result = method(self, *args, **kwargs)
             dct[key] = result
             return result
     return wrapper
 
 
 def cache_star_import(func):
-    def wrapper(evaluator, scope, *args, **kwargs):
-        with common.ignored(KeyError):
-            mods = _star_import_cache[scope]
-            if mods[0] + settings.star_import_cache_validity > time.time():
-                return mods[1]
-        # cache is too old and therefore invalid or not available
-        _invalidate_star_import_cache_module(scope)
-        mods = func(evaluator, scope, *args, **kwargs)
-        _star_import_cache[scope] = time.time(), mods
-
-        return mods
+    @time_cache("star_import_cache_validity")
+    def wrapper(self):
+        yield self.base  # The cache key
+        yield func(self)
     return wrapper
 
 
 def _invalidate_star_import_cache_module(module, only_main=False):
     """ Important if some new modules are being reparsed """
-    with common.ignored(KeyError):
-        t, mods = _star_import_cache[module]
-
-        del _star_import_cache[module]
-
-        for m in mods:
-            _invalidate_star_import_cache_module(m, only_main=True)
-
-    if not only_main:
-        # We need a list here because otherwise the list is being changed
-        # during the iteration in py3k: iteritems -> items.
-        for key, (t, mods) in list(_star_import_cache.items()):
-            if module in mods:
-                _invalidate_star_import_cache_module(key)
+    try:
+        t, modules = _time_caches['star_import_cache_validity'][module]
+    except KeyError:
+        pass
+    else:
+        del _time_caches['star_import_cache_validity'][module]
 
 
 def invalidate_star_import_cache(path):
     """On success returns True."""
     try:
         parser_cache_item = parser_cache[path]
     except KeyError:
-        return False
+        pass
     else:
         _invalidate_star_import_cache_module(parser_cache_item.parser.module)
-        return True
 
 
-def load_parser(path, name):
+def load_parser(path):
     """
     Returns the module or None, if it fails.
     """
-    if path is None and name is None:
-        return None
-
     p_time = os.path.getmtime(path) if path else None
-    n = name if path is None else path
     try:
-        parser_cache_item = parser_cache[n]
+        parser_cache_item = parser_cache[path]
         if not path or p_time <= parser_cache_item.change_time:
             return parser_cache_item.parser
         else:
             # In case there is already a module cached and this module
             # has to be reparsed, we also need to invalidate the import
             # caches.
             _invalidate_star_import_cache_module(parser_cache_item.parser.module)
     except KeyError:
         if settings.use_filesystem_cache:
-            return ParserPickling.load_parser(n, p_time)
+            return ParserPickling.load_parser(path, p_time)
 
 
-def save_parser(path, name, parser, pickling=True):
+def save_parser(path, parser, pickling=True):
     try:
-        p_time = None if not path else os.path.getmtime(path)
+        p_time = None if path is None else os.path.getmtime(path)
     except OSError:
         p_time = None
         pickling = False
 
-    n = name if path is None else path
     item = ParserCacheItem(parser, p_time)
-    parser_cache[n] = item
+    parser_cache[path] = item
     if settings.use_filesystem_cache and pickling:
-        ParserPickling.save_parser(n, item)
+        ParserPickling.save_parser(path, item)
 
 
 class ParserPickling(object):
 
-    version = 13
+    version = 24
     """
     Version number (integer) for file system cache.
 
     Increment this number when there are any incompatible changes in
     parser representation classes.  For example, the following changes
     are regarded as incompatible.
```

### Comparing `jedi-0.8.1-final0/conftest.py` & `jedi-0.9.0/conftest.py`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/setup.py` & `jedi-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,41 +7,44 @@
     # Distribute is not actually required to install
     from distutils.core import setup
 
 __AUTHOR__ = 'David Halter'
 __AUTHOR_EMAIL__ = 'davidhalter88@gmail.com'
 
 readme = open('README.rst').read() + '\n\n' + open('CHANGELOG.rst').read()
+packages = ['jedi', 'jedi.parser', 'jedi.parser.pgen2',
+            'jedi.evaluate', 'jedi.evaluate.compiled', 'jedi.api']
 
 import jedi
 
 setup(name='jedi',
       version=jedi.__version__,
       description='An autocompletion tool for Python that can be used for text editors.',
       author=__AUTHOR__,
       author_email=__AUTHOR_EMAIL__,
       maintainer=__AUTHOR__,
       maintainer_email=__AUTHOR_EMAIL__,
       url='https://github.com/davidhalter/jedi',
       license='MIT',
       keywords='python completion refactoring vim',
       long_description=readme,
-      packages=['jedi', 'jedi.parser', 'jedi.evaluate', 'jedi.evaluate.compiled', 'jedi.api'],
-      package_data={'jedi': ['evaluate/compiled/fake/*.pym']},
+      packages=packages,
+      package_data={'jedi': ['evaluate/compiled/fake/*.pym', 'parser/grammar*.txt']},
       platforms=['any'],
       classifiers=[
           'Development Status :: 4 - Beta',
           'Environment :: Plugins',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: MIT License',
           'Operating System :: OS Independent',
           'Programming Language :: Python :: 2',
           'Programming Language :: Python :: 2.6',
           'Programming Language :: Python :: 2.7',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.2',
           'Programming Language :: Python :: 3.3',
+          'Programming Language :: Python :: 3.4',
           'Topic :: Software Development :: Libraries :: Python Modules',
           'Topic :: Text Editors :: Integrated Development Environments (IDE)',
           'Topic :: Utilities',
       ],
       )
```

### Comparing `jedi-0.8.1-final0/CHANGELOG.rst` & `jedi-0.9.0/CHANGELOG.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 .. :changelog:
 
 Changelog
 ---------
 
-0.8.1 (2014-07-15)
+0.9.0 (2015-04-10)
+++++++++++++++++++
+
+- Integrated the parser of 2to3. This will make refactoring possible. It will
+  also be possible to check for error messages (like compiling an AST would give)
+  in the future.
+- With the new parser, the evaluation also completely changed. It's now simpler
+  and more readable.
+- Completely rewritten REPL completion.
+- Added ``jedi.names``, a command to do static analysis. Thanks to that
+  sourcegraph guys for sponsoring this!
+- Alpha version of the linter.
+
+
+0.8.1 (2014-07-23)
 +++++++++++++++++++
 
-* Bugfix release, the last release forgot to include files that improve
-    autocompletion for builtin libraries. Fixed.
+- Bugfix release, the last release forgot to include files that improve
+  autocompletion for builtin libraries. Fixed.
 
 0.8.0 (2014-05-05)
 +++++++++++++++++++
 
 - Memory Consumption for compiled modules (e.g. builtins, sys) has been reduced
   drastically. Loading times are down as well (it takes basically as long as an
   import).
 - REPL completion is starting to become usable.
-- Various small API changes. Generally this released focuses on stability and
+- Various small API changes. Generally this release focuses on stability and
   refactoring of internal APIs.
-- Introducing operator precedence, which makes calculating correct Array indices
-  and ``__getattr__`` strings possible.
+- Introducing operator precedence, which makes calculating correct Array
+  indices and ``__getattr__`` strings possible.
 
 0.7.0 (2013-08-09)
 ++++++++++++++++++
 
-- Switched from LGPL to MIT license
-- Added an Interpreter class to the API to make autocompletion in REPL possible.
-- Added autocompletion support for namespace packages
-- Add sith.py, a new random testing method
+- Switched from LGPL to MIT license.
+- Added an Interpreter class to the API to make autocompletion in REPL
+  possible.
+- Added autocompletion support for namespace packages.
+- Add sith.py, a new random testing method.
 
 0.6.0 (2013-05-14)
 ++++++++++++++++++
 
-- Much faster parser with builtin part caching
-- A test suite, thanks @tkf
+- Much faster parser with builtin part caching.
+- A test suite, thanks @tkf.
 
 0.5 versions (2012)
 +++++++++++++++++++
 
-- Initial development
+- Initial development.
```

### Comparing `jedi-0.8.1-final0/LICENSE.txt` & `jedi-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jedi-0.8.1-final0/jedi.egg-info/PKG-INFO` & `jedi-0.9.0/jedi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,132 +1,166 @@
 Metadata-Version: 1.1
 Name: jedi
-Version: 0.8.1-final0
+Version: 0.9.0
 Summary: An autocompletion tool for Python that can be used for text editors.
 Home-page: https://github.com/davidhalter/jedi
 Author: David Halter
 Author-email: davidhalter88@gmail.com
 License: MIT
-Description: ###################################################
-        Jedi - an awesome autocompletion library for Python
-        ###################################################
+Description: ###################################################################
+        Jedi - an awesome autocompletion/static analysis library for Python
+        ###################################################################
         
         .. image:: https://secure.travis-ci.org/davidhalter/jedi.png?branch=master
             :target: http://travis-ci.org/davidhalter/jedi
             :alt: Travis-CI build status
         
         .. image:: https://coveralls.io/repos/davidhalter/jedi/badge.png?branch=master
             :target: https://coveralls.io/r/davidhalter/jedi
             :alt: Coverage Status
         
-        .. image:: https://pypip.in/d/jedi/badge.png
-            :target: https://crate.io/packages/jedi/
-            :alt: Number of PyPI downloads
-        
-        .. image:: https://pypip.in/v/jedi/badge.png
-            :target: https://crate.io/packages/jedi/
-            :alt: Latest PyPI version
-        
-        Jedi is an autocompletion tool for Python that can be used in IDEs/editors.
-        Jedi works. Jedi is fast. It understands all of the basic Python syntax
-        elements including many builtin functions.
         
-        Additionaly, Jedi suports two different goto functions and has support for
-        renaming as well as Pydoc support and some other IDE features.
+        *If you have specific questions, please add an issue or ask on* `stackoverflow
+        <https://stackoverflow.com>`_ *with the label* ``python-jedi``.
+        
+        
+        Jedi is a static analysis tool for Python that can be used in IDEs/editors. Its
+        historic focus is autocompletion, but does static analysis for now as well.
+        Jedi is fast and is very well tested. It understands Python on a deeper level
+        than all other static analysis frameworks for Python.
+        
+        Jedi has support for two different goto functions. It's possible to search for
+        related names and to list all names in a Python file and infer them. Jedi
+        understands docstrings and you can use Jedi autocompletion in your REPL as
+        well.
         
         Jedi uses a very simple API to connect with IDE's. There's a reference
         implementation as a `VIM-Plugin <https://github.com/davidhalter/jedi-vim>`_,
-        which uses Jedi's autocompletion.  I encourage you to use Jedi in your IDEs.
-        It's really easy. If there are any problems (also with licensing), just contact
-        me.
+        which uses Jedi's autocompletion.  We encourage you to use Jedi in your IDEs.
+        It's really easy.
         
-        Jedi can be used with the following editors:
+        Jedi can currently be used with the following editors:
         
         - Vim (jedi-vim_, YouCompleteMe_)
-        - Emacs (Jedi.el_, elpy_, anaconda-mode_)
+        - Emacs (Jedi.el_, elpy_, anaconda-mode_, ycmd_)
         - Sublime Text (SublimeJEDI_ [ST2 + ST3], anaconda_ [only ST3])
         - SynWrite_
         - TextMate_ (Not sure if it's actually working)
         - Kate_ version 4.13+ supports it natively, you have to enable it, though. [`proof
           <https://projects.kde.org/projects/kde/applications/kate/repository/show?rev=KDE%2F4.13>`_]
         
         And it powers the following projects:
         
         - wdb_ - Web Debugger
         
         
-        Here are some pictures:
+        Here are some pictures taken from jedi-vim_:
         
         .. image:: https://github.com/davidhalter/jedi/raw/master/docs/_screenshots/screenshot_complete.png
         
         Completion for almost anything (Ctrl+Space).
         
         .. image:: https://github.com/davidhalter/jedi/raw/master/docs/_screenshots/screenshot_function.png
         
         Display of function/class bodies, docstrings.
         
         .. image:: https://github.com/davidhalter/jedi/raw/master/docs/_screenshots/screenshot_pydoc.png
         
-        Pydoc support (with highlighting, Shift+k).
+        Pydoc support (Shift+k).
         
         There is also support for goto and renaming.
         
         Get the latest version from `github <https://github.com/davidhalter/jedi>`_
         (master branch should always be kind of stable/working).
         
-        Docs are available at `https://jedi.jedidjah.ch/
-        <https://jedi.jedidjah.ch/>`_. Pull requests with documentation
+        Docs are available at `https://jedi.readthedocs.org/en/latest/
+        <https://jedi.readthedocs.org/en/latest/>`_. Pull requests with documentation
         enhancements and/or fixes are awesome and most welcome. Jedi uses `semantic
         versioning <http://semver.org/>`_.
         
         
         Installation
         ============
         
             pip install jedi
         
         Note: This just installs the Jedi library, not the editor plugins. For
         information about how to make it work with your editor, refer to the
         corresponding documentation.
         
         You don't want to use ``pip``? Please refer to the `manual
-        <https://jedi.jedidjah.ch/en/latest/docs/installation.html>`_.
+        <https://jedi.readthedocs.org/en/latest/docs/installation.html>`_.
         
         
         Feature Support and Caveats
         ===========================
         
         Jedi really understands your Python code. For a comprehensive list what Jedi
-        can do, see: `Features
-        <https://jedi.jedidjah.ch/en/latest/docs/features.html>`_. A list of
+        understands, see: `Features
+        <https://jedi.readthedocs.org/en/latest/docs/features.html>`_. A list of
         caveats can be found on the same page.
         
-        You can run Jedi on cPython 2.6, 2.7, 3.2 or 3.3, but it should also
+        You can run Jedi on cPython 2.6, 2.7, 3.2, 3.3 or 3.4, but it should also
         understand/parse code older than those versions.
         
         Tips on how to use Jedi efficiently can be found `here
-        <https://jedi.jedidjah.ch/en/latest/docs/recipes.html>`_.
+        <https://jedi.readthedocs.org/en/latest/docs/recipes.html>`_.
         
+        API
+        ---
         
-        API for IDEs
-        ============
+        You can find the documentation for the `API here <https://jedi.readthedocs.org/en/latest/docs/plugin-api.html>`_.
+        
+        
+        Autocompletion / Goto / Pydoc
+        -----------------------------
+        
+        Please check the API for a good explanation. There are the following commands:
+        
+        - ``jedi.Script.goto_assignments``
+        - ``jedi.Script.completions``
+        - ``jedi.Script.usages``
+        
+        The returned objects are very powerful and really all you might need.
+        
+        
+        Autocompletion in your REPL (IPython, etc.)
+        -------------------------------------------
         
-        It's very easy to create an editor plugin that uses Jedi. See `Plugin API
-        <https://jedi.jedidjah.ch/en/latest/docs/plugin-api.html>`_ for more
-        information.
+        It's possible to have Jedi autocompletion in REPL modes - `example video <https://vimeo.com/122332037>`_.
+        This means that IPython and others are `supported
+        <https://jedi.readthedocs.org/en/latest/docs/usage.html#tab-completion-in-the-python-shell>`_.
         
-        If you have specific questions, please add an issue or ask on `stackoverflow
-        <https://stackoverflow.com>`_ with the label ``python-jedi``.
+        
+        Static Analysis / Linter
+        ------------------------
+        
+        To do all forms of static analysis, please try to use ``jedi.names``. It will
+        return a list of names that you can use to infer types and so on.
+        
+        Linting is another thing that is going to be part of Jedi. For now you can try
+        an alpha version ``python -m jedi linter``. The API might change though and
+        it's still buggy. It's Jedi's goal to be smarter than classic linter and
+        understand ``AttributeError`` and other code issues.
+        
+        
+        Refactoring
+        -----------
+        
+        Jedi would in theory support refactoring, but we have never publicized it,
+        because it's not production ready. If you're interested in helping out here,
+        let me know. With the latest parser changes, it should be very easy to actually
+        make it work.
         
         
         Development
         ===========
         
         There's a pretty good and extensive `development documentation
-        <https://jedi.jedidjah.ch/en/latest/docs/development.html>`_.
+        <https://jedi.readthedocs.org/en/latest/docs/development.html>`_.
         
         
         Testing
         =======
         
         The test suite depends on ``tox`` and ``pytest``::
         
@@ -141,81 +175,98 @@
         
             tox -e py27
         
         Tests are also run automatically on `Travis CI
         <https://travis-ci.org/davidhalter/jedi/>`_.
         
         For more detailed information visit the `testing documentation
-        <https://jedi.jedidjah.ch/en/latest/docs/testing.html>`_
+        <https://jedi.readthedocs.org/en/latest/docs/testing.html>`_
         
         
         .. _jedi-vim: https://github.com/davidhalter/jedi-vim
         .. _youcompleteme: http://valloric.github.io/YouCompleteMe/
         .. _Jedi.el: https://github.com/tkf/emacs-jedi
         .. _elpy: https://github.com/jorgenschaefer/elpy
         .. _anaconda-mode: https://github.com/proofit404/anaconda-mode
+        .. _ycmd: https://github.com/abingham/emacs-ycmd
         .. _sublimejedi: https://github.com/srusskih/SublimeJEDI
         .. _anaconda: https://github.com/DamnWidget/anaconda
         .. _SynWrite: http://uvviewsoft.com/synjedi/
         .. _wdb: https://github.com/Kozea/wdb
         .. _TextMate: https://github.com/lawrenceakka/python-jedi.tmbundle
         .. _Kate: http://kate-editor.org
         
         
         .. :changelog:
         
         Changelog
         ---------
         
-        0.8.1 (2014-07-15)
+        0.9.0 (2015-04-10)
+        ++++++++++++++++++
+        
+        - Integrated the parser of 2to3. This will make refactoring possible. It will
+          also be possible to check for error messages (like compiling an AST would give)
+          in the future.
+        - With the new parser, the evaluation also completely changed. It's now simpler
+          and more readable.
+        - Completely rewritten REPL completion.
+        - Added ``jedi.names``, a command to do static analysis. Thanks to that
+          sourcegraph guys for sponsoring this!
+        - Alpha version of the linter.
+        
+        
+        0.8.1 (2014-07-23)
         +++++++++++++++++++
         
-        * Bugfix release, the last release forgot to include files that improve
-            autocompletion for builtin libraries. Fixed.
+        - Bugfix release, the last release forgot to include files that improve
+          autocompletion for builtin libraries. Fixed.
         
         0.8.0 (2014-05-05)
         +++++++++++++++++++
         
         - Memory Consumption for compiled modules (e.g. builtins, sys) has been reduced
           drastically. Loading times are down as well (it takes basically as long as an
           import).
         - REPL completion is starting to become usable.
-        - Various small API changes. Generally this released focuses on stability and
+        - Various small API changes. Generally this release focuses on stability and
           refactoring of internal APIs.
-        - Introducing operator precedence, which makes calculating correct Array indices
-          and ``__getattr__`` strings possible.
+        - Introducing operator precedence, which makes calculating correct Array
+          indices and ``__getattr__`` strings possible.
         
         0.7.0 (2013-08-09)
         ++++++++++++++++++
         
-        - Switched from LGPL to MIT license
-        - Added an Interpreter class to the API to make autocompletion in REPL possible.
-        - Added autocompletion support for namespace packages
-        - Add sith.py, a new random testing method
+        - Switched from LGPL to MIT license.
+        - Added an Interpreter class to the API to make autocompletion in REPL
+          possible.
+        - Added autocompletion support for namespace packages.
+        - Add sith.py, a new random testing method.
         
         0.6.0 (2013-05-14)
         ++++++++++++++++++
         
-        - Much faster parser with builtin part caching
-        - A test suite, thanks @tkf
+        - Much faster parser with builtin part caching.
+        - A test suite, thanks @tkf.
         
         0.5 versions (2012)
         +++++++++++++++++++
         
-        - Initial development
+        - Initial development.
         
 Keywords: python completion refactoring vim
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
 Classifier: Topic :: Utilities
```

### Comparing `jedi-0.8.1-final0/jedi.egg-info/SOURCES.txt` & `jedi-0.9.0/jedi.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 jedi/api/usages.py
 jedi/evaluate/__init__.py
 jedi/evaluate/analysis.py
 jedi/evaluate/cache.py
 jedi/evaluate/docstrings.py
 jedi/evaluate/dynamic.py
 jedi/evaluate/finder.py
+jedi/evaluate/flow_analysis.py
 jedi/evaluate/helpers.py
 jedi/evaluate/imports.py
 jedi/evaluate/iterable.py
 jedi/evaluate/param.py
 jedi/evaluate/precedence.py
 jedi/evaluate/recursion.py
 jedi/evaluate/representation.py
@@ -78,58 +79,73 @@
 jedi/evaluate/compiled/fake/_weakref.pym
 jedi/evaluate/compiled/fake/builtins.pym
 jedi/evaluate/compiled/fake/datetime.pym
 jedi/evaluate/compiled/fake/io.pym
 jedi/evaluate/compiled/fake/posix.pym
 jedi/parser/__init__.py
 jedi/parser/fast.py
-jedi/parser/representation.py
+jedi/parser/grammar2.7.txt
+jedi/parser/grammar3.4.txt
+jedi/parser/token.py
 jedi/parser/tokenize.py
+jedi/parser/tree.py
 jedi/parser/user_context.py
+jedi/parser/pgen2/__init__.py
+jedi/parser/pgen2/grammar.py
+jedi/parser/pgen2/parse.py
+jedi/parser/pgen2/pgen.py
 test/__init__.py
 test/conftest.py
 test/helpers.py
 test/refactor.py
 test/run.py
 test/test_cache.py
 test/test_debug.py
 test/test_integration.py
+test/test_integration_analysis.py
 test/test_integration_import.py
 test/test_integration_keyword.py
+test/test_integration_stdlib.py
 test/test_jedi_system.py
+test/test_new_parser.py
 test/test_regression.py
 test/test_speed.py
 test/test_utils.py
 test/completion/__init__.py
 test/completion/arrays.py
 test/completion/basic.py
 test/completion/classes.py
 test/completion/complex.py
+test/completion/comprehensions.py
 test/completion/decorators.py
 test/completion/definition.py
 test/completion/descriptors.py
 test/completion/docstring.py
-test/completion/dynamic.py
+test/completion/dynamic_arrays.py
+test/completion/dynamic_params.py
+test/completion/flow_analysis.py
 test/completion/functions.py
 test/completion/generators.py
 test/completion/goto.py
 test/completion/imports.py
 test/completion/invalid.py
 test/completion/isinstance.py
 test/completion/keywords.py
 test/completion/lambdas.py
 test/completion/named_param.py
+test/completion/on_import.py
 test/completion/ordering.py
 test/completion/parser.py
 test/completion/precedence.py
 test/completion/stdlib.py
 test/completion/sys_path.py
 test/completion/types.py
 test/completion/usages.py
 test/completion/import_tree/__init__.py
+test/completion/import_tree/invisible_pkg.py
 test/completion/import_tree/mod1.py
 test/completion/import_tree/mod2.py
 test/completion/import_tree/random.py
 test/completion/import_tree/recurse_class1.py
 test/completion/import_tree/recurse_class2.py
 test/completion/import_tree/rename1.py
 test/completion/import_tree/rename2.py
@@ -154,48 +170,61 @@
 test/static_analysis/star_arguments.py
 test/static_analysis/try_except.py
 test/static_analysis/import_tree/__init__.py
 test/static_analysis/import_tree/a.py
 test/static_analysis/import_tree/b.py
 test/test_api/__init__.py
 test/test_api/test_api.py
-test/test_api/test_api_classes.py
 test/test_api/test_api_classes_follow_definition.py
 test/test_api/test_call_signatures.py
+test/test_api/test_classes.py
 test/test_api/test_defined_names.py
 test/test_api/test_full_name.py
 test/test_api/test_interpreter.py
 test/test_api/test_unicode.py
 test/test_evaluate/__init__.py
 test/test_evaluate/test_absolute_import.py
+test/test_evaluate/test_annotations.py
 test/test_evaluate/test_buildout_detection.py
 test/test_evaluate/test_compiled.py
 test/test_evaluate/test_docstring.py
 test/test_evaluate/test_extension.py
 test/test_evaluate/test_imports.py
 test/test_evaluate/test_namespace_package.py
-test/test_evaluate/test_precedence.py
 test/test_evaluate/test_pyc.py
 test/test_evaluate/test_representation.py
+test/test_evaluate/test_sys_path.py
 test/test_evaluate/absolute_import/local_module.py
 test/test_evaluate/absolute_import/unittest.py
 test/test_evaluate/buildout_project/buildout.cfg
 test/test_evaluate/buildout_project/bin/app
 test/test_evaluate/buildout_project/bin/empty_file
 test/test_evaluate/buildout_project/src/proj_name/module_name.py
+test/test_evaluate/egg-link/venv/lib/python3.4/site-packages/egg_link.egg-link
+test/test_evaluate/flask-site-packages/flask_foo.py
+test/test_evaluate/flask-site-packages/flask/__init__.py
+test/test_evaluate/flask-site-packages/flask/ext/__init__.py
+test/test_evaluate/flask-site-packages/flask_baz/__init__.py
+test/test_evaluate/flask-site-packages/flaskext/__init__.py
+test/test_evaluate/flask-site-packages/flaskext/bar.py
+test/test_evaluate/flask-site-packages/flaskext/moo/__init__.py
+test/test_evaluate/init_extension_module/__init__.cpython-34m.so
+test/test_evaluate/init_extension_module/module.c
+test/test_evaluate/init_extension_module/setup.py
 test/test_evaluate/namespace_package/ns1/pkg/__init__.py
 test/test_evaluate/namespace_package/ns1/pkg/ns1_file.py
 test/test_evaluate/namespace_package/ns1/pkg/ns1_folder/__init__.py
 test/test_evaluate/namespace_package/ns2/pkg/ns2_file.py
 test/test_evaluate/namespace_package/ns2/pkg/ns2_folder/__init__.py
 test/test_evaluate/namespace_package/ns2/pkg/ns2_folder/nested/__init__.py
+test/test_evaluate/not_in_sys_path/__init__.py
 test/test_evaluate/not_in_sys_path/not_in_sys_path.py
 test/test_evaluate/not_in_sys_path/not_in_sys_path_package/__init__.py
 test/test_evaluate/not_in_sys_path/not_in_sys_path_package/module.py
+test/test_evaluate/not_in_sys_path/pkg/__init__.py
 test/test_evaluate/not_in_sys_path/pkg/module.py
 test/test_parser/__init__.py
 test/test_parser/test_fast_parser.py
 test/test_parser/test_get_code.py
 test/test_parser/test_parser.py
-test/test_parser/test_representation.py
-test/test_parser/test_token.py
+test/test_parser/test_tokenize.py
 test/test_parser/test_user_context.py
```

