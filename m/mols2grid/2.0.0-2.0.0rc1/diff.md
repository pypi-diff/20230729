# Comparing `tmp/mols2grid-2.0.0.tar.gz` & `tmp/mols2grid-2.0.0rc1.tar.gz`

## Comparing `mols2grid-2.0.0.tar` & `mols2grid-2.0.0rc1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mols2grid-2.0.0/.eslintrc.json
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mols2grid-2.0.0/.npmignore
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 mols2grid-2.0.0/.prettierignore
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 mols2grid-2.0.0/.prettierrc.json
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 mols2grid-2.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0    15615 2020-02-02 00:00:00.000000 mols2grid-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 mols2grid-2.0.0/CITATION.cff
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 mols2grid-2.0.0/DEVELOPMENT.md
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 mols2grid-2.0.0/babel.config.js
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mols2grid-2.0.0/codecov.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mols2grid-2.0.0/install.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid.json
--rw-r--r--   0        0        0   450809 2020-02-02 00:00:00.000000 mols2grid-2.0.0/package-lock.json
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 mols2grid-2.0.0/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mols2grid-2.0.0/setup.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 mols2grid-2.0.0/tsconfig.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 mols2grid-2.0.0/webpack.config.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mols2grid-2.0.0/css/widget.css
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/Makefile
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/conf.py
--rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/contents.md
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/environment.yml
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/make.bat
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/_static/custom.css
--rw-r--r--   0        0        0    95735 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/_static/demo.png
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/_static/mols2grid_logo.png
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/api/callbacks.rst
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/api/molgrid.rst
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/api/simple.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/api/utils.rst
--rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/notebooks/callbacks.ipynb
--rw-r--r--   0        0        0     5916 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/notebooks/customization.ipynb
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/notebooks/filtering.ipynb
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 mols2grid-2.0.0/docs/notebooks/quickstart.ipynb
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/_version.py
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/callbacks.py
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/dispatch.py
--rw-r--r--   0        0        0    42066 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/molgrid.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/select.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/utils.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/labextension/package.json
--rw-r--r--   0        0        0     8633 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/labextension/static/480.dd173b97aba0b97d49dc.js
--rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/labextension/static/568.191b3db4a3e041ee051a.js
--rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/labextension/static/remoteEntry.38d390f0df7a4c62007d.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/nbextension/extension.js
--rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/nbextension/index.js
--rw-r--r--   0        0        0    24423 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/__init__.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/interactive.html
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/static.html
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/css/common.css
--rw-r--r--   0        0        0    20688 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/css/interactive.css
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/css/static.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/html/common_header.html
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/html/iframe.html
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/html/interactive_header.html
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/js/draw_mol.js
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/js/filter.js
--rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/js/grid_interaction.js
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/js/interactive.js
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/js/kernel.js
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/js/molstorage.js
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/js/popup.js
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/js/search.js
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/js/sort.js
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/js/callbacks/external_link.js
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/templates/js/callbacks/show_3d.js
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/widget/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/widget/_frontend.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 mols2grid-2.0.0/mols2grid/widget/widget.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 mols2grid-2.0.0/src/extension.ts
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 mols2grid-2.0.0/src/index.ts
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 mols2grid-2.0.0/src/plugin.ts
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 mols2grid-2.0.0/src/version.ts
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 mols2grid-2.0.0/src/widget.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mols2grid-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 mols2grid-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mols2grid-2.0.0/tests/pytest.ini
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 mols2grid-2.0.0/tests/test_callbacks.py
--rw-r--r--   0        0        0    27754 2020-02-02 00:00:00.000000 mols2grid-2.0.0/tests/test_interface.py
--rw-r--r--   0        0        0    10528 2020-02-02 00:00:00.000000 mols2grid-2.0.0/tests/test_molgrid.py
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 mols2grid-2.0.0/tests/test_select.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 mols2grid-2.0.0/tests/test_utils.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 mols2grid-2.0.0/tests/webdriver_utils.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 mols2grid-2.0.0/.gitignore
--rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 mols2grid-2.0.0/LICENSE
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 mols2grid-2.0.0/README.md
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 mols2grid-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    16668 2020-02-02 00:00:00.000000 mols2grid-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/.eslintrc.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/.npmignore
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/.prettierignore
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/.prettierrc.json
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/.readthedocs.yaml
+-rw-r--r--   0        0        0    15615 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/CITATION.cff
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/babel.config.js
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/codecov.yml
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/environment.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/install.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid.json
+-rw-r--r--   0        0        0   450813 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/package-lock.json
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/package.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/setup.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/tsconfig.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/webpack.config.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/css/widget.css
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/Makefile
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/conf.py
+-rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/contents.md
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/environment.yml
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/make.bat
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/_static/custom.css
+-rw-r--r--   0        0        0    95735 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/_static/demo.png
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/_static/mols2grid_logo.png
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/api/callbacks.rst
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/api/molgrid.rst
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/api/simple.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/api/utils.rst
+-rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/notebooks/callbacks.ipynb
+-rw-r--r--   0        0        0     5916 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/notebooks/customization.ipynb
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/notebooks/filtering.ipynb
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/docs/notebooks/quickstart.ipynb
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/__init__.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/_version.py
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/callbacks.py
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/dispatch.py
+-rw-r--r--   0        0        0    42066 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/molgrid.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/select.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/utils.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/labextension/package.json
+-rw-r--r--   0        0        0     8637 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/labextension/static/480.a99394933b0f23a624ab.js
+-rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/labextension/static/568.d44a1a2f4790f58ec0e3.js
+-rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/labextension/static/remoteEntry.791f11d71f83b76ea703.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/nbextension/extension.js
+-rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/nbextension/index.js
+-rw-r--r--   0        0        0    24423 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/__init__.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/interactive.html
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/static.html
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/css/common.css
+-rw-r--r--   0        0        0    20688 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/css/interactive.css
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/css/static.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/html/common_header.html
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/html/iframe.html
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/html/interactive_header.html
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/js/draw_mol.js
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/js/filter.js
+-rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/js/grid_interaction.js
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/js/interactive.js
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/js/kernel.js
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/js/molstorage.js
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/js/popup.js
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/js/search.js
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/js/sort.js
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/js/callbacks/external_link.js
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/templates/js/callbacks/show_3d.js
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/widget/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/widget/_frontend.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/mols2grid/widget/widget.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/src/extension.ts
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/src/index.ts
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/src/plugin.ts
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/src/version.ts
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/src/widget.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/tests/pytest.ini
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/tests/test_callbacks.py
+-rw-r--r--   0        0        0    27754 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/tests/test_interface.py
+-rw-r--r--   0        0        0    10528 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/tests/test_molgrid.py
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/tests/test_select.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/tests/test_utils.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/tests/webdriver_utils.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/.gitignore
+-rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/README.md
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    16646 2020-02-02 00:00:00.000000 mols2grid-2.0.0rc1/PKG-INFO
```

### Comparing `mols2grid-2.0.0/CHANGELOG.md` & `mols2grid-2.0.0rc1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 ---
 
-## [2.0.0] - 2023/07/23
+## [2.0.0] - ????/??/??
 
 This release is a major change on the UI contributed by @themoenen, refer to
 [PR#55](https://github.com/cbouy/mols2grid/pull/55) for the full list of changes:
 
 ### Added
 - `background_color="white"` parameter added to `display` and `save` to control the background
   color of each cell.
```

### Comparing `mols2grid-2.0.0/package-lock.json` & `mols2grid-2.0.0rc1/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'version'": "'2.0.0-rc1'"}*

```diff
@@ -10816,9 +10816,9 @@
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "lockfileVersion": 1,
     "name": "mols2grid",
     "requires": true,
-    "version": "2.0.0"
+    "version": "2.0.0-rc1"
 }
```

### Comparing `mols2grid-2.0.0/package.json` & `mols2grid-2.0.0rc1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'2.0.0-rc1'"}*

```diff
@@ -86,9 +86,9 @@
         "prepack": "yarn run build:lib",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "2.0.0-rc1"
 }
```

### Comparing `mols2grid-2.0.0/tsconfig.json` & `mols2grid-2.0.0rc1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/webpack.config.js` & `mols2grid-2.0.0rc1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/docs/Makefile` & `mols2grid-2.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/docs/conf.py` & `mols2grid-2.0.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/docs/contents.md` & `mols2grid-2.0.0rc1/docs/contents.md`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/docs/index.rst` & `mols2grid-2.0.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/docs/make.bat` & `mols2grid-2.0.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/docs/_static/demo.png` & `mols2grid-2.0.0rc1/docs/_static/demo.png`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/docs/_static/mols2grid_logo.png` & `mols2grid-2.0.0rc1/docs/_static/mols2grid_logo.png`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/docs/notebooks/callbacks.ipynb` & `mols2grid-2.0.0rc1/docs/notebooks/callbacks.ipynb`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/docs/notebooks/customization.ipynb` & `mols2grid-2.0.0rc1/docs/notebooks/customization.ipynb`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/docs/notebooks/filtering.ipynb` & `mols2grid-2.0.0rc1/docs/notebooks/filtering.ipynb`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/docs/notebooks/quickstart.ipynb` & `mols2grid-2.0.0rc1/docs/notebooks/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/callbacks.py` & `mols2grid-2.0.0rc1/mols2grid/callbacks.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/dispatch.py` & `mols2grid-2.0.0rc1/mols2grid/dispatch.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/molgrid.py` & `mols2grid-2.0.0rc1/mols2grid/molgrid.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/select.py` & `mols2grid-2.0.0rc1/mols2grid/select.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/utils.py` & `mols2grid-2.0.0rc1/mols2grid/utils.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/labextension/package.json` & `mols2grid-2.0.0rc1/mols2grid/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9677734375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.791f11d71f83b76ea703.js'}}",*

 * * "'version'": "'2.0.0-rc1'"}*

```diff
@@ -48,15 +48,15 @@
         "dist/*.map",
         "css/*.css"
     ],
     "homepage": "https://github.com/cbouy/mols2grid",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.38d390f0df7a4c62007d.js"
+            "load": "static/remoteEntry.791f11d71f83b76ea703.js"
         },
         "extension": "lib/plugin",
         "outputDir": "mols2grid/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -90,9 +90,9 @@
         "prepack": "yarn run build:lib",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "2.0.0-rc1"
 }
```

### Comparing `mols2grid-2.0.0/mols2grid/labextension/static/480.dd173b97aba0b97d49dc.js` & `mols2grid-2.0.0rc1/mols2grid/labextension/static/480.a99394933b0f23a624ab.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -280,11 +280,11 @@
                         n = l
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"mols2grid","version":"2.0.0","description":"Custom widget for the Python mols2grid package","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","dist/*.map","css/*.css"],"homepage":"https://github.com/cbouy/mols2grid","bugs":{"url":"https://github.com/cbouy/mols2grid/issues"},"license":"Apache-2.0","author":{"name":"Cedric Bouysset","email":"cedric@bouysset.net"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cbouy/mols2grid"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf mols2grid/labextension","clean:nbextension":"rimraf mols2grid/nbextension/static/index.js","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^8.8.0","eslint-plugin-prettier":"^4.2.1","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.8","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"mols2grid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"mols2grid","version":"2.0.0-rc1","description":"Custom widget for the Python mols2grid package","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","dist/*.map","css/*.css"],"homepage":"https://github.com/cbouy/mols2grid","bugs":{"url":"https://github.com/cbouy/mols2grid/issues"},"license":"Apache-2.0","author":{"name":"Cedric Bouysset","email":"cedric@bouysset.net"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cbouy/mols2grid"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf mols2grid/labextension","clean:nbextension":"rimraf mols2grid/nbextension/static/index.js","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^8.8.0","eslint-plugin-prettier":"^4.2.1","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.8","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"mols2grid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `mols2grid-2.0.0/mols2grid/labextension/static/568.191b3db4a3e041ee051a.js` & `mols2grid-2.0.0rc1/mols2grid/labextension/static/568.d44a1a2f4790f58ec0e3.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -252,11 +252,11 @@
                         n = l
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"mols2grid","version":"2.0.0","description":"Custom widget for the Python mols2grid package","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","dist/*.map","css/*.css"],"homepage":"https://github.com/cbouy/mols2grid","bugs":{"url":"https://github.com/cbouy/mols2grid/issues"},"license":"Apache-2.0","author":{"name":"Cedric Bouysset","email":"cedric@bouysset.net"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cbouy/mols2grid"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf mols2grid/labextension","clean:nbextension":"rimraf mols2grid/nbextension/static/index.js","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^8.8.0","eslint-plugin-prettier":"^4.2.1","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.8","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"mols2grid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"mols2grid","version":"2.0.0-rc1","description":"Custom widget for the Python mols2grid package","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","dist/*.map","css/*.css"],"homepage":"https://github.com/cbouy/mols2grid","bugs":{"url":"https://github.com/cbouy/mols2grid/issues"},"license":"Apache-2.0","author":{"name":"Cedric Bouysset","email":"cedric@bouysset.net"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cbouy/mols2grid"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf mols2grid/labextension","clean:nbextension":"rimraf mols2grid/nbextension/static/index.js","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^8.8.0","eslint-plugin-prettier":"^4.2.1","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.8","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"mols2grid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `mols2grid-2.0.0/mols2grid/labextension/static/remoteEntry.38d390f0df7a4c62007d.js` & `mols2grid-2.0.0rc1/mols2grid/labextension/static/remoteEntry.791f11d71f83b76ea703.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -37,20 +37,20 @@
     }
     b.m = g, b.c = m, b.d = (e, r) => {
         for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
-        480: "dd173b97aba0b97d49dc",
-        568: "191b3db4a3e041ee051a",
+        480: "a99394933b0f23a624ab",
+        568: "d44a1a2f4790f58ec0e3",
         829: "d620f53947100b9acdd6"
     } [e] + ".js?v=" + {
-        480: "dd173b97aba0b97d49dc",
-        568: "191b3db4a3e041ee051a",
+        480: "a99394933b0f23a624ab",
+        568: "d44a1a2f4790f58ec0e3",
         829: "d620f53947100b9acdd6"
     } [e], b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -96,15 +96,15 @@
                     var o = i[e] = i[e] || {},
                         l = o[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : a > l.from)) && (o[r] = {
                         get: () => Promise.all([b.e(829), b.e(568)]).then((() => () => b(568))),
                         from: a,
                         eager: !1
                     })
-                })("mols2grid", "2.0.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("mols2grid", "2.0.0-rc1"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         b.g.importScripts && (e = b.g.location + "");
         var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `mols2grid-2.0.0/mols2grid/labextension/static/third-party-licenses.json` & `mols2grid-2.0.0rc1/mols2grid/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/nbextension/index.js` & `mols2grid-2.0.0rc1/mols2grid/nbextension/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -275,15 +275,15 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"mols2grid","version":"2.0.0","description":"Custom widget for the Python mols2grid package","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","dist/*.map","css/*.css"],"homepage":"https://github.com/cbouy/mols2grid","bugs":{"url":"https://github.com/cbouy/mols2grid/issues"},"license":"Apache-2.0","author":{"name":"Cedric Bouysset","email":"cedric@bouysset.net"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cbouy/mols2grid"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf mols2grid/labextension","clean:nbextension":"rimraf mols2grid/nbextension/static/index.js","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^8.8.0","eslint-plugin-prettier":"^4.2.1","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.8","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"mols2grid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                e.exports = JSON.parse('{"name":"mols2grid","version":"2.0.0-rc1","description":"Custom widget for the Python mols2grid package","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","dist/*.map","css/*.css"],"homepage":"https://github.com/cbouy/mols2grid","bugs":{"url":"https://github.com/cbouy/mols2grid/issues"},"license":"Apache-2.0","author":{"name":"Cedric Bouysset","email":"cedric@bouysset.net"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cbouy/mols2grid"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf mols2grid/labextension","clean:nbextension":"rimraf mols2grid/nbextension/static/index.js","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^8.8.0","eslint-plugin-prettier":"^4.2.1","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.8","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"mols2grid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         n = {};
 
     function i(e) {
         var r = n[e];
         if (void 0 !== r) return r.exports;
```

### Comparing `mols2grid-2.0.0/mols2grid/nbextension/index.js.map` & `mols2grid-2.0.0rc1/mols2grid/nbextension/index.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'mappings'": "'iEAEAA,EADkC,EAAQ,IAChCC,EAA4B,IAE9BC,KAAK,CAACC,EAAOC,GAAI,sHAAuH,KAEhJD,EAAOH,QAAUA,C,uBCEjBG,EAAOH,QAAU,SAAUK,GACzB,IAAIC,EAAO,GAuDX,OArDAA,EAAKC,SAAW,WACd,OAAOC,KAAKC,KAAI,SAAUC,GACxB,IAAIC,EAsDV,SAAgCD,EAAML,GACpC,IAoBiBO,EAEbC,EACAC,EAvBAH,EAAUD,EAAK,IAAM,GAErBK,EAAaL,EAAK,GAEtB,IAAKK,EACH,OAAOJ,EAGT,GAAIN,GAAgC,mBAATW,KAAqB,CAC9C,IAAIC,GAWWL,EAXeG,EAa5BF,EAASG,KAAKE,SAASC,mBAAmBC,KAAKC,UAAUT,MACzDE,EAAO,+DAA+DQ,OAAOT,GAC1E,OAAOS,OAAOR,EAAM,QAdrBS,EAAaR,EAAWS,QAAQf,KAAI,SAAUgB,GAChD,M […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "index.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "exports",
         "___CSS_LOADER_API_IMPORT___",
         "push",
         "module",
         "id",
         "useSourceMap",
```

### Comparing `mols2grid-2.0.0/mols2grid/templates/interactive.html` & `mols2grid-2.0.0rc1/mols2grid/templates/interactive.html`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/static.html` & `mols2grid-2.0.0rc1/mols2grid/templates/static.html`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/css/common.css` & `mols2grid-2.0.0rc1/mols2grid/templates/css/common.css`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/css/interactive.css` & `mols2grid-2.0.0rc1/mols2grid/templates/css/interactive.css`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/css/static.css` & `mols2grid-2.0.0rc1/mols2grid/templates/css/static.css`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/html/common_header.html` & `mols2grid-2.0.0rc1/mols2grid/templates/html/common_header.html`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/html/iframe.html` & `mols2grid-2.0.0rc1/mols2grid/templates/html/iframe.html`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/js/draw_mol.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/draw_mol.js`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/js/grid_interaction.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/grid_interaction.js`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/js/interactive.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/interactive.js`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/js/kernel.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/kernel.js`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/js/molstorage.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/molstorage.js`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/js/popup.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/popup.js`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/js/search.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/search.js`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/js/sort.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/sort.js`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/templates/js/callbacks/show_3d.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/callbacks/show_3d.js`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/widget/__init__.py` & `mols2grid-2.0.0rc1/mols2grid/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/mols2grid/widget/widget.py` & `mols2grid-2.0.0rc1/mols2grid/widget/widget.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/src/extension.ts` & `mols2grid-2.0.0rc1/src/extension.ts`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/src/plugin.ts` & `mols2grid-2.0.0rc1/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/src/version.ts` & `mols2grid-2.0.0rc1/src/version.ts`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/src/widget.ts` & `mols2grid-2.0.0rc1/src/widget.ts`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/tests/conftest.py` & `mols2grid-2.0.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/tests/test_callbacks.py` & `mols2grid-2.0.0rc1/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/tests/test_interface.py` & `mols2grid-2.0.0rc1/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/tests/test_molgrid.py` & `mols2grid-2.0.0rc1/tests/test_molgrid.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/tests/test_select.py` & `mols2grid-2.0.0rc1/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/tests/test_utils.py` & `mols2grid-2.0.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/tests/webdriver_utils.py` & `mols2grid-2.0.0rc1/tests/webdriver_utils.py`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/.gitignore` & `mols2grid-2.0.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/LICENSE` & `mols2grid-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mols2grid-2.0.0/README.md` & `mols2grid-2.0.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [![Code coverage](https://codecov.io/gh/cbouy/mols2grid/branch/master/graph/badge.svg?token=QDI1XQSDUC)](https://codecov.io/gh/cbouy/mols2grid)
 
 [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
 [![Knime Hub](https://img.shields.io/badge/Available%20on-KNIME-ffd500.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC/xhBQAAAAFzUkdCAK7OHOkAAABdUExURUxpcf/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAPfHMOMAAAAfdFJOUwCyq6CEYtAEApEspncGDpjxVlAYgDSdiEBHbMrCHtmwXwB/AAAAT3pUWHRSYXcgcHJvZmlsZSB0eXBlIGlwdGMAAHic48osKEnmUgADIwsuYwsTIxNLkxQDEyBEgDTDZAMjs1Qgy9jUyMTMxBzEB8uASKBKLgAolQ7jKiJtHwAAAIxJREFUGNNdjFkSgyAQBYdtYADZVNxz/2NGjSlj+q9fvWqAD1rDk1Ke3nJqH4NnpH7d4iCFvV1XVJ3r7u6URPZiHb8eeFJ25sjDNahlKRDUkq7u5njd32ZC3A433g2+h3bKCuUx9FHOecyV/CzXfi/KSJG9EjJB0lEAS9UxxriINMiOLJim0SfNiYF/3szTBp6mEP9HAAAAAElFTkSuQmCC)](https://hub.knime.com/cbouy/spaces/Public/latest/Interactive%20Grid%20of%20Molecules)
 
 **mols2grid** is an interactive molecule viewer for 2D structures, based on RDKit.
 
-![Demo image](https://raw.githubusercontent.com/cbouy/mols2grid/master/docs/_static/demo.png)
+![Demo image](docs/_static/demo.png)
 
 ## [Documentation](https://mols2grid.readthedocs.io/en/latest/contents.html)
 
 Installation, basic usage, links to resources...*etc.*
 
 ## [Notebooks](https://mols2grid.readthedocs.io/en/latest/notebooks/quickstart.html)
```

### Comparing `mols2grid-2.0.0/PKG-INFO` & `mols2grid-2.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mols2grid
-Version: 2.0.0
+Version: 2.0.0rc1
 Summary: Interactive 2D small molecule viewer
 Project-URL: Homepage, https://github.com/cbouy/mols2grid
 Project-URL: Documentation, https://mols2grid.readthedocs.io/en/latest/
 Project-URL: Discussions, https://github.com/cbouy/mols2grid/discussions
 Project-URL: Issues, https://github.com/cbouy/mols2grid/issues
 Project-URL: Changelog, https://github.com/cbouy/mols2grid/blob/master/CHANGELOG.md
 Author-email: Cédric Bouysset <cedric@bouysset.net>
@@ -201,15 +201,16 @@
 Requires-Dist: ipywidgets<8,>=7
 Requires-Dist: jinja2>=2.11.0
 Requires-Dist: numpy
 Requires-Dist: pandas
 Provides-Extra: build
 Requires-Dist: build; extra == 'build'
 Provides-Extra: dev
-Requires-Dist: mols2grid[build,docs,tests]; extra == 'dev'
+Requires-Dist: mols2grid[build,tests]; extra == 'dev'
+Requires-Dist: tbump; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mistune<3.0.0; extra == 'docs'
 Provides-Extra: tests
 Requires-Dist: cairosvg==2.5.2; extra == 'tests'
 Requires-Dist: flaky==3.7.0; extra == 'tests'
 Requires-Dist: imagehash~=4.3; extra == 'tests'
 Requires-Dist: ipython==7.12.0; extra == 'tests'
@@ -230,15 +231,15 @@
 [![Code coverage](https://codecov.io/gh/cbouy/mols2grid/branch/master/graph/badge.svg?token=QDI1XQSDUC)](https://codecov.io/gh/cbouy/mols2grid)
 
 [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
 [![Knime Hub](https://img.shields.io/badge/Available%20on-KNIME-ffd500.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC/xhBQAAAAFzUkdCAK7OHOkAAABdUExURUxpcf/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAPfHMOMAAAAfdFJOUwCyq6CEYtAEApEspncGDpjxVlAYgDSdiEBHbMrCHtmwXwB/AAAAT3pUWHRSYXcgcHJvZmlsZSB0eXBlIGlwdGMAAHic48osKEnmUgADIwsuYwsTIxNLkxQDEyBEgDTDZAMjs1Qgy9jUyMTMxBzEB8uASKBKLgAolQ7jKiJtHwAAAIxJREFUGNNdjFkSgyAQBYdtYADZVNxz/2NGjSlj+q9fvWqAD1rDk1Ke3nJqH4NnpH7d4iCFvV1XVJ3r7u6URPZiHb8eeFJ25sjDNahlKRDUkq7u5njd32ZC3A433g2+h3bKCuUx9FHOecyV/CzXfi/KSJG9EjJB0lEAS9UxxriINMiOLJim0SfNiYF/3szTBp6mEP9HAAAAAElFTkSuQmCC)](https://hub.knime.com/cbouy/spaces/Public/latest/Interactive%20Grid%20of%20Molecules)
 
 **mols2grid** is an interactive molecule viewer for 2D structures, based on RDKit.
 
-![Demo image](https://raw.githubusercontent.com/cbouy/mols2grid/master/docs/_static/demo.png)
+![Demo image](docs/_static/demo.png)
 
 ## [Documentation](https://mols2grid.readthedocs.io/en/latest/contents.html)
 
 Installation, basic usage, links to resources...*etc.*
 
 ## [Notebooks](https://mols2grid.readthedocs.io/en/latest/notebooks/quickstart.html)
```

